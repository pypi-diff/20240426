# Comparing `tmp/pyreportgen-0.1.8.tar.gz` & `tmp/pyreportgen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyreportgen-0.1.8.tar", last modified: Fri Dec  8 08:48:45 2023, max compression
+gzip compressed data, was "pyreportgen-0.1.9.tar", last modified: Fri Dec  8 15:00:06 2023, max compression
```

## Comparing `pyreportgen-0.1.8.tar` & `pyreportgen-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 08:48:45.489695 pyreportgen-0.1.8/
--rwxr-xr-x   0 runner    (1001) docker     (127)       18 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-08 08:48:45.489695 pyreportgen-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 08:48:45.489695 pyreportgen-0.1.8/pyreportgen/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5999 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      304 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/gis.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      654 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2249 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/layout.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/statistic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1384 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/pyreportgen/style.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 08:48:45.489695 pyreportgen-0.1.8/pyreportgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-08 08:48:45.000000 pyreportgen-0.1.8/pyreportgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-08 08:48:45.000000 pyreportgen-0.1.8/pyreportgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 08:48:45.000000 pyreportgen-0.1.8/pyreportgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-08 08:48:45.000000 pyreportgen-0.1.8/pyreportgen.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      581 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 08:48:45.489695 pyreportgen-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2023-12-08 08:48:29.000000 pyreportgen-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:00:06.782750 pyreportgen-0.1.9/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       18 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-08 15:00:06.782750 pyreportgen-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:00:06.782750 pyreportgen-0.1.9/pyreportgen/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6622 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      304 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7235 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/gis.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1449 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2249 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/layout.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1884 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/statistic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1384 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/pyreportgen/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 15:00:06.782750 pyreportgen-0.1.9/pyreportgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2023-12-08 15:00:06.000000 pyreportgen-0.1.9/pyreportgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2023-12-08 15:00:06.000000 pyreportgen-0.1.9/pyreportgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 15:00:06.000000 pyreportgen-0.1.9/pyreportgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-08 15:00:06.000000 pyreportgen-0.1.9/pyreportgen.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      581 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 15:00:06.782750 pyreportgen-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2023-12-08 14:59:58.000000 pyreportgen-0.1.9/setup.py
```

### Comparing `pyreportgen-0.1.8/PKG-INFO` & `pyreportgen-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreportgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for creating reports and other pdf documents.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyreportgen-0.1.8/pyreportgen/__init__.py` & `pyreportgen-0.1.9/pyreportgen/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,35 @@
 
 if not (_DATA_DIR in os.listdir()):
     os.makedirs(_DATA_DIR, exist_ok=True)
 
 
 _RE_COMBINE_WHITESPACE = re.compile(r"\s+")
 
+class MailAttachment:
+    def __init__(self, path, filename) -> None:
+        self.path = path
+        self.filename = filename
+    
+    def get_attachment(self) -> MIMEBase:
+        with open(self.path, "rb") as attachment:
+            # Add file as application/octet-stream
+            # Email client can usually download this automatically as attachment
+            att = MIMEBase("application", "octet-stream")
+            att.set_payload(attachment.read())
 
+            # Encode file in ASCII characters to send by email    
+            encoders.encode_base64(att)
+
+            # Add header as key/value pair to attachment part
+            att.add_header(
+                "Content-Disposition",
+                f"attachment; filename={self.filename}",
+            )
+            return att
 
 class Report(Component):
     def __init__(self, children:list[Component]=[], style:str=style.STYLE_NORMAL):
         super().__init__()
         self.children = children
         self.style = style
 
@@ -51,20 +71,20 @@
         return _RE_COMBINE_WHITESPACE.sub(" ", html).strip()
     
     def pdf(self, path:str, html:str=""):
         import pdfkit 
         if html == "":
             html = self.render()
 
-        with open(_DATA_DIR+'/out.html', 'w', encoding="UTF-8") as f:
+        with open(os.path.join(_DATA_DIR,'out.html'), 'w', encoding="UTF-8") as f:
             f.write(html)
 
-        pdfkit.from_file(_DATA_DIR+'/out.html', path, options={"--enable-local-file-access":None, "--print-media-type":None})
+        pdfkit.from_file(os.path.join(_DATA_DIR,'out.html'), path, options={"--enable-local-file-access":None, "--print-media-type":None})
     
-    def email(self, user:str, password:str, subject:str, sender:str, recipient:str, smtp_server:str, smtp_port:int, context=ssl.create_default_context(), include_pdf=False, pdfname:str="Report"):
+    def email(self, user:str, password:str, subject:str, sender:str, recipient:str, smtp_server:str, smtp_port:int, context=ssl.create_default_context(), attachments:list[MailAttachment] = []):
         message = MIMEMultipart("alternative")
         message["Subject"] = subject
         message["From"] = sender
         message["To"] = recipient
 
 
         html = self.render()
@@ -100,37 +120,17 @@
             fp.close()
 
             # Define the image's ID as referenced above
             msgImage.add_header('Content-ID', f'<{image_lookup[i]}>')
             message.attach(msgImage)
 
         
-        if include_pdf:
-
-            # Open PDF file in binary mode
-            self.pdf(f"{_DATA_DIR}/tmp.pdf")
-            with open(f"{_DATA_DIR}/tmp.pdf", "rb") as attachment:
-                # Add file as application/octet-stream
-                # Email client can usually download this automatically as attachment
-                pdf = MIMEBase("application", "octet-stream")
-                pdf.set_payload(attachment.read())
-
-            # Encode file in ASCII characters to send by email    
-            encoders.encode_base64(pdf)
-
-            # Add header as key/value pair to attachment part
-            pdf.add_header(
-                "Content-Disposition",
-                f"attachment; filename={pdfname}.pdf",
-            )
-
-
-
+        for i in attachments:
             # Add attachment to message and convert message to string
-            message.attach(pdf)
+            message.attach(i.get_attachment())
 
         with smtplib.SMTP_SSL(smtp_server, smtp_port, context=context) as server:
             server.login(user, password)
             server.sendmail(sender, recipient, message.as_string())
     
 class Html(Component):
     def __init__(self, html:str):
@@ -177,14 +177,28 @@
     
     def render(self) -> str:
         return super().render()
 
 class Image(Component):
     def __init__(self, src: str):
         super().__init__()
-        self.src: str = src
+        
+        self.src: str = os.path.abspath(src)
+    
+    def render(self) -> str:
+        return helpers.tagwrap("", "img", "Image", f"src='{self.src}'", close=False)
+
+class ConditionalImage(Component):
+    def __init__(self, filepath:str, children:list[Component] = []):
+        super().__init__()
+        self.filepath:str = filepath
+        self.children:list[Component] = children
     
     def render(self) -> str:
-        localizer = "../"
-        if self.src.startswith("/"):
-            localizer = ""
-        return helpers.tagwrap("", "img", "Image", f"src='{localizer}{self.src}'", close=False)
+        if os.path.isfile(self.filepath):
+            html = helpers.tagwrap("", "img", "Image", f"src='{os.path.abspath(self.filepath)}'", close=False)
+        else:
+            html = ""
+            for i in self.children:
+                html += i.render()
+            html = helpers.tagwrap(html, "div")
+        return html
```

### Comparing `pyreportgen-0.1.8/pyreportgen/gis.py` & `pyreportgen-0.1.9/pyreportgen/gis.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,21 +87,25 @@
             ] 
             for y in range(from_tile[1], to_tile[1]+1)
             ]
 
         full_image = Image.new('RGB',(tile_size*grid_size[0], tile_size*grid_size[1]), (0,0,0))
 
         images = grid_size[0] * grid_size[1]
+        current_image = 0
 
-
+        pb = helpers.ProgressBar(images, "Collecting tiles")
 
         for y, row in enumerate(grid):
             for x, tile in enumerate(row):
+                current_image += 1
                 im = open_image_from_url(tile)
                 full_image.paste(im, (x*tile_size, y*tile_size))
+                pb.print(current_image)
+
 
 
         image_size = full_image.size
         cropped = full_image.crop((int(tile_size*start_xoverflow),int(tile_size*start_yoverflow),image_size[0]-int(tile_size * end_xoverflow),image_size[1]-int(tile_size * end_yoverflow)))
         return cropped
     
     def render(self) -> str:
@@ -142,15 +146,14 @@
         bottom_left[0] -= padding
         bottom_left[1] -= padding
 
         upper_right[0] += padding
         upper_right[1] += padding
 
         bbox = [bottom_left, upper_right]
-        print(bbox)
         super().__init__(bbox, zoom, tile_host)
         self.geojson = geojson
         self.padding = padding
 
     def make_image(self):
         map = super().make_image()
         size = map.size
@@ -160,26 +163,22 @@
         for feature in self.geojson["features"]:
             if feature["type"] != "Feature":
                 continue
             geom = feature["geometry"]
             
             if geom["type"] == "Point":
                 geom["coordinates"].reverse()
-                print(geom["coordinates"])
-                print(self.bottom_left)
-                print(self.upper_right)
                 y, x = translate_coord(geom["coordinates"], self.bottom_left, self.upper_right, (1,0),(0,1))
                 draw.regular_polygon(((int(x*size[0]), int((y)*size[1])), 6), 128, fill="red")
             elif geom["type"] == "LineString":
                 points = []
                 for i in geom["coordinates"]:
                     i.reverse()
                     y, x = translate_coord(i, self.bottom_left, self.upper_right, (1,0), (0, 1))
                     points.append((int(x*size[0]),int(y*size[1])))
-                print(points)
                 draw.line(points, fill="red", width=6)
             elif geom["type"] == "Polygon":
                 for poly in geom["coordinates"]:
                     points = []
                     for i in poly:
                         i.reverse()
                         y, x = translate_coord(i, self.bottom_left, self.upper_right, (1,0), (0, 1))
```

### Comparing `pyreportgen-0.1.8/pyreportgen/layout.py` & `pyreportgen-0.1.9/pyreportgen/layout.py`

 * *Files identical despite different names*

### Comparing `pyreportgen-0.1.8/pyreportgen/statistic.py` & `pyreportgen-0.1.9/pyreportgen/statistic.py`

 * *Files identical despite different names*

### Comparing `pyreportgen-0.1.8/pyreportgen/style.py` & `pyreportgen-0.1.9/pyreportgen/style.py`

 * *Files identical despite different names*

### Comparing `pyreportgen-0.1.8/pyreportgen.egg-info/PKG-INFO` & `pyreportgen-0.1.9/pyreportgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyreportgen
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for creating reports and other pdf documents.
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pyreportgen-0.1.8/readme.md` & `pyreportgen-0.1.9/readme.md`

 * *Files identical despite different names*

### Comparing `pyreportgen-0.1.8/setup.py` & `pyreportgen-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 readme = open("./readme.md").read()
 
 setup(
     name="pyreportgen",
-    version="0.1.8",
+    version="0.1.9",
     description="A package for creating reports and other pdf documents.",
     long_description=readme,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

