# Comparing `tmp/unireport-0.0.7-py3-none-any.whl.zip` & `tmp/unireport-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 8969 bytes, number of entries: 16
+Zip file size: 9223 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      115 b- defN 20-Feb-02 00:00 unireport/__init__.py
 -rw-r--r--  2.0 unx      102 b- defN 20-Feb-02 00:00 unireport/exceptions.py
 -rw-r--r--  2.0 unx       63 b- defN 20-Feb-02 00:00 unireport/logger.py
 -rw-r--r--  2.0 unx     2432 b- defN 20-Feb-02 00:00 unireport/plugin.py
 -rw-r--r--  2.0 unx     1725 b- defN 20-Feb-02 00:00 unireport/renderer.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 unireport/plugins/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 unireport/plugins/builtin.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 unireport/plugins/external/__init__.py
 -rw-r--r--  2.0 unx      171 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/__init__.py
--rw-r--r--  2.0 unx     1909 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/api.py
+-rw-r--r--  2.0 unx     1924 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/api.py
 -rw-r--r--  2.0 unx     2565 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/client.py
--rw-r--r--  2.0 unx     2224 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/plugin.py
-?rw-r--r--  2.0 unx     1034 b- defN 20-Feb-02 00:00 unireport-0.0.7.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 unireport-0.0.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 unireport-0.0.7.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1354 b- defN 20-Feb-02 00:00 unireport-0.0.7.dist-info/RECORD
-16 files, 14853 bytes uncompressed, 6707 bytes compressed:  54.8%
+-rw-r--r--  2.0 unx     2868 b- defN 20-Feb-02 00:00 unireport/plugins/external/grafana/plugin.py
+?rw-r--r--  2.0 unx     1089 b- defN 20-Feb-02 00:00 unireport-0.0.8.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 unireport-0.0.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1072 b- defN 20-Feb-02 00:00 unireport-0.0.8.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1354 b- defN 20-Feb-02 00:00 unireport-0.0.8.dist-info/RECORD
+16 files, 15567 bytes uncompressed, 6961 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: unireport/plugins/external/grafana/client.py
 Comment: 
 
 Filename: unireport/plugins/external/grafana/plugin.py
 Comment: 
 
-Filename: unireport-0.0.7.dist-info/METADATA
+Filename: unireport-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: unireport-0.0.7.dist-info/WHEEL
+Filename: unireport-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: unireport-0.0.7.dist-info/licenses/LICENSE
+Filename: unireport-0.0.8.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: unireport-0.0.7.dist-info/RECORD
+Filename: unireport-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## unireport/plugins/external/grafana/api.py

```diff
@@ -14,15 +14,15 @@
         auth=None,
         host="localhost",
         port=None,
         url_path_prefix="",
         protocol="http",
         timeout=DEFAULT_TIMEOUT,
     ):
-        self.client = GrafanaClient(
+        self.client: GrafanaClient = GrafanaClient(
             auth,
             host=host,
             port=port,
             url_path_prefix=url_path_prefix,
             protocol=protocol,
             timeout=timeout,
         )
```

## unireport/plugins/external/grafana/plugin.py

```diff
@@ -10,44 +10,62 @@
 
 from .api import GrafanaAPI
 
 
 class GrafanaPlugin(Plugin):
     def __init__(
         self,
-        api: GrafanaAPI,
+        apis: list[GrafanaAPI],
         render_path_template="/render{path}",
         stub_dashboard_image_on_exception=False,
     ):
         super().__init__()
 
-        self.api: GrafanaAPI = api
+        # backward compatibility
+        if isinstance(apis, GrafanaAPI):
+            apis = [apis]
+
+        self.apis: list[GrafanaAPI] = apis
         self.render_path_template: str = render_path_template
         self.stub_dashboard_image_on_exception: bool = stub_dashboard_image_on_exception
 
     def setup(self, env: Environment):
         super().setup(env)
 
         env.globals["render_grafana_dashboard"] = self.render_grafana_dashboard
 
-    def render_grafana_dashboard(self, url: str, **kwargs) -> str:
+    def _get_api(self, host):
+        for api in self.apis:
+            if api.client.url_host == host:
+                return api
+
+        raise RendererException(f"Can't find GrafanaAPI for {host}")
+
+    def render_grafana_dashboard(self, url: str, height: int = -1, **kwargs) -> str:
+        # default height because of that
+        # https://github.com/grafana/grafana-image-renderer/issues/488
+        return self._render_grafana_dashboard_impl(url, height=height, **kwargs)
+
+    def _render_grafana_dashboard_impl(self, url: str, **kwargs) -> str:
         logger.info(f"render grafana dashboard {url}, {kwargs}")
 
         result = urlparse(url)
         params = parse_qs(result.query)
         params.update(**kwargs)
 
+        api = self._get_api(result.hostname)
+
         render_url = self.render_path_template.format(path=result.path)
 
         dashboard_id = "_".join(result.path.split("/")[-2:])
         dashboard_filename = (
             self.context.get_images_dir() / f"{dashboard_id}_{uuid.uuid1()}.png"
         )
         try:
-            response = self.api.query_raw(render_url, params=params)
+            response = api.query_raw(render_url, params=params)
             response.raise_for_status()
 
             header = response.headers
             content_type = header.get("content-type")
             if content_type not in ("image/png",):
                 raise RendererException(f"Invalid content-type {content_type}")
```

## Comparing `unireport-0.0.7.dist-info/METADATA` & `unireport-0.0.8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: unireport
-Version: 0.0.7
+Version: 0.0.8
+Dynamic: Description
+Dynamic: Description-Content-Type
 Summary: Generate reports by template for lots of different external services
 Project-URL: Homepage, https://github.com/zifter/unireport
 Project-URL: Source, https://github.com/zifter/unireport
 Project-URL: Tracker, https://github.com/zifter/unireport/issues
 Author-email: Aleh Strakachuk <zifter.ai+unireport@gmail.com>
 License: MIT
 License-File: LICENSE
```

## Comparing `unireport-0.0.7.dist-info/licenses/LICENSE` & `unireport-0.0.8.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `unireport-0.0.7.dist-info/RECORD` & `unireport-0.0.8.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 unireport/logger.py,sha256=Dt0r4_3ldzsxQuh33HNUAp-jgEQlVUUrmUeXnaJv7rE,63
 unireport/plugin.py,sha256=s5hW9zJy_RyYAHq6jAgAGa936nrXvagdE-8dcqrMihU,2432
 unireport/renderer.py,sha256=OIScO0qd0me49RNyZztZjvF6WqHeDmJiq7AIOogNZvQ,1725
 unireport/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unireport/plugins/builtin.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unireport/plugins/external/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 unireport/plugins/external/grafana/__init__.py,sha256=0eRLMD-j07HF3nt4QKpqRvqaro-fNkfF_xv5rYOrtHQ,171
-unireport/plugins/external/grafana/api.py,sha256=B9D-NL26iBiw22qj3U74EeqwH3E5HHFAuOkR_ACTps4,1909
+unireport/plugins/external/grafana/api.py,sha256=W_nZWgMYqirIGAQw7vrPYYEUAwVUTzcvX5YWhAAMTMI,1924
 unireport/plugins/external/grafana/client.py,sha256=Nd6OOPJcxb9ri8PxpdTUZ9wGTK8G0vhZkBR5TR24IQQ,2565
-unireport/plugins/external/grafana/plugin.py,sha256=o83OfP_XxAfZZClrQMP08sMpV40yuE6kd4YpV3IXELk,2224
-unireport-0.0.7.dist-info/METADATA,sha256=Y_1iAD4nFJ0_DTg-zIbqbCm70C6AMHBY5N9vWyKtek0,1034
-unireport-0.0.7.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-unireport-0.0.7.dist-info/licenses/LICENSE,sha256=70fRxTEOQHUWA24YsLoHiTjhK4Z0FUhp-qgeaPi9xSw,1072
-unireport-0.0.7.dist-info/RECORD,,
+unireport/plugins/external/grafana/plugin.py,sha256=G0lseeQjazx3CWqCvUSdrlesRK5fN4Nb4F1Ztf2Ax_Y,2868
+unireport-0.0.8.dist-info/METADATA,sha256=tXBLjz6dbD9QKQt_Xfb-mWr9Lt1MOS6s_xN1osBO0vg,1089
+unireport-0.0.8.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+unireport-0.0.8.dist-info/licenses/LICENSE,sha256=70fRxTEOQHUWA24YsLoHiTjhK4Z0FUhp-qgeaPi9xSw,1072
+unireport-0.0.8.dist-info/RECORD,,
```

