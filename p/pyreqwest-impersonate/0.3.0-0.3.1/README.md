# Comparing `tmp/pyreqwest_impersonate-0.3.0.tar.gz` & `tmp/pyreqwest_impersonate-0.3.1.tar.gz`

## Comparing `pyreqwest_impersonate-0.3.0.tar` & `pyreqwest_impersonate-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.0/Cargo.toml
--rw-r--r--   0     1001      127     4802 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/.gitignore
--rw-r--r--   0     1001      127     7594 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/README.md
--rw-r--r--   0     1001      127      271 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/1_threads.csv
--rw-r--r--   0     1001      127      273 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/4_threads.csv
--rw-r--r--   0     1001      127      343 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/README.md
--rw-r--r--   0     1001      127     3299 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/benchmark.py
--rw-r--r--   0     1001      127       83 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/requirements.txt
--rw-r--r--   0     1001      127      799 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/benchmark/server.py
--rw-r--r--   0     1001      127    19307 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/src/lib.rs
--rw-r--r--   0     1001      127     3036 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/src/response.rs
--rw-r--r--   0     1001      127     3800 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/tests/test_client.py
--rw-r--r--   0     1001      127    41713 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-04-25 11:43:10.000000 pyreqwest_impersonate-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8663 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     4854 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/.gitignore
+-rw-r--r--   0     1001      127     7758 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/README.md
+-rw-r--r--   0     1001      127      271 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/1_threads.csv
+-rw-r--r--   0     1001      127      273 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/4_threads.csv
+-rw-r--r--   0     1001      127      343 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/README.md
+-rw-r--r--   0     1001      127     3299 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/benchmark.py
+-rw-r--r--   0     1001      127       83 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      799 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/benchmark/server.py
+-rw-r--r--   0     1001      127    23737 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      127     3033 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/src/response.rs
+-rw-r--r--   0     1001      127     3922 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/tests/test_client.py
+-rw-r--r--   0     1001      127     5573 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/tests/test_defs.py
+-rw-r--r--   0     1001      127    41713 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-04-26 21:34:34.000000 pyreqwest_impersonate-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8827 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.3.1/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.3.0/Cargo.toml` & `pyreqwest_impersonate-0.3.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.3.0"
+version = "0.3.1"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `pyreqwest_impersonate-0.3.0/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.3.1/.github/workflows/CI.yml`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
           name: wheels-linux-${{ matrix.platform.target }}
           path: dist
       - name: pytest
         if: ${{ startsWith(matrix.platform.target, 'x86_64') }}
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'x86') && matrix.platform.target != 'ppc64' }}
         uses: uraimo/run-on-arch-action@v2.5.0
         with:
           arch: ${{ matrix.platform.target }}
@@ -66,15 +66,15 @@
           githubToken: ${{ github.token }}
           install: |
             apt-get update
             apt-get install -y --no-install-recommends python3 python3-pip
             pip3 install -U pip pytest
           run: |
             set -e
-            pip3 install pyreqwest_impersonate --find-links dist --force-reinstall
+            pip3 install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
             pytest
 
   windows:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
         platform:
@@ -100,15 +100,15 @@
           name: wheels-windows-${{ matrix.platform.target }}
           path: dist
       - name: pytest
         if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
         shell: bash
         run: |
           set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
+          pip install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
           pip install pytest
           pytest
 
   macos:
     runs-on: ${{ matrix.platform.runner }}
     strategy:
       matrix:
@@ -129,22 +129,22 @@
           args: --release --out dist
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v4
         with:
           name: wheels-macos-${{ matrix.platform.target }}
           path: dist
-      - name: pytest
-        if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
-        shell: bash
-        run: |
-          set -e
-          pip install pyreqwest_impersonate --find-links dist --force-reinstall
-          pip install pytest
-          pytest
+      #- name: pytest
+      #  if: ${{ !startsWith(matrix.platform.target, 'aarch64') }}
+      #  shell: bash
+      #  run: |
+      #    set -e
+      #    pip install pyreqwest_impersonate --no-index --find-links dist --force-reinstall
+      #    pip install pytest
+      #    pytest
 
   sdist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
```

### Comparing `pyreqwest_impersonate-0.3.0/.gitignore` & `pyreqwest_impersonate-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.0/README.md` & `pyreqwest_impersonate-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123"
             Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5","safari_17_2_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
             Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
-        verify (bool, optional): Verify SSL certificates. Default is True.
+        verify (bool, optional): Verify SSL certificates. Default is False.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
 ```
 
 #### Client Methods
@@ -103,31 +103,36 @@
 
     """
 ```
 
 #### Example
 
 ```python
-from pyreqwest_impersonate import Client
+import pyreqwest_impersonate as pri
 
-client = Client(impersonate="chrome_123")
+client = pri.Client(impersonate="chrome_123")
 
 # get request
 resp = client.get("https://tls.peet.ws/api/all")
 print(resp.json())
 
 # post request
 data = {"key1": "value1", "key2": "value2"}
 auth = ("user", "password")
 resp = client.post(url="https://httpbin.org/anything", data=data, auth=auth)
-print(response.content)  # Get the content as bytes
-print(response.cookies)  # Access cookies
-print(response.headers)  # Access headers
-print(response.json())  # Parse the content as JSON
-print(response.status_code)  # Access the status code
-print(response.text)  # Decode the content as text
-print(response.url)  # Access the URL
+print(resp.content)
+print(resp.cookies)
+print(resp.headers)
+print(resp.json())
+print(resp.status_code)
+print(resp.text)
+print(resp.url)
+
+# You can also use convenience functions that use a default Client instance under the hood:
+# pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
+resp = pri.get("https://httpbin.org/anything") # Default Client does not impersonate a browser
+resp = pri.Client(impersonate="chrome_123").get("https://httpbin.org/anything")  
 ```
 ### II. AsyncClient
 
 TODO
```

### Comparing `pyreqwest_impersonate-0.3.0/benchmark/benchmark.py` & `pyreqwest_impersonate-0.3.1/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.0/benchmark/server.py` & `pyreqwest_impersonate-0.3.1/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.0/src/lib.rs` & `pyreqwest_impersonate-0.3.1/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ///         in additional requests. Default is `true`.
     /// * `referer` - Enable or disable automatic setting of the `Referer` header. Default is `true`.
     /// * `proxy` - An optional proxy URL for HTTP requests.
     /// * `timeout` - An optional timeout for HTTP requests in seconds.
     /// * `impersonate` - An optional entity to impersonate. Supported browsers and versions include Chrome, Safari, OkHttp, and Edge.
     /// * `follow_redirects` - A boolean to enable or disable following redirects. Default is `true`.
     /// * `max_redirects` - The maximum number of redirects to follow. Default is 20. Applies if `follow_redirects` is `true`.
-    /// * `verify` - An optional boolean indicating whether to verify SSL certificates. Default is `true`.
+    /// * `verify` - An optional boolean indicating whether to verify SSL certificates. Default is `false`.
     /// * `http1` - An optional boolean indicating whether to use only HTTP/1.1. Default is `false`.
     /// * `http2` - An optional boolean indicating whether to use only HTTP/2. Default is `false`.
     ///
     /// # Example
     ///
     /// ```
     /// from reqwest_impersonate import Client
@@ -145,18 +145,17 @@
         if follow_redirects.unwrap_or(true) {
             client_builder = client_builder.redirect(Policy::limited(max_redirects));
         } else {
             client_builder = client_builder.redirect(Policy::none());
         }
 
         // Verify
-        if let Some(verify) = verify {
-            if !verify {
-                client_builder = client_builder.danger_accept_invalid_certs(true);
-            }
+        let verify = verify.unwrap_or(false);
+        if !verify {
+            client_builder = client_builder.danger_accept_invalid_certs(true);
         }
 
         // Http version: http1 || http2
         match (http1, http2) {
             (Some(true), Some(true)) => {
                 return Err(PyErr::new::<exceptions::PyValueError, _>(
                     "Both http1 and http2 cannot be true",
@@ -350,15 +349,15 @@
             let value_str = value.to_str().unwrap_or("");
             headers_dict.set_item(key_str, value_str)?;
         }
         let headers = headers_dict.unbind();
 
         let status_code = resp.status().as_u16().into_py(py);
 
-        let url = PyString::new_bound(py, &resp.url().to_string()).into();
+        let url = PyString::new_bound(py, resp.url().as_ref()).into();
 
         let buf = resp.bytes().map_err(|e| {
             PyErr::new::<exceptions::PyException, _>(format!("Error reading response bytes: {}", e))
         })?;
         let content = PyBytes::new_bound(py, &buf).unbind();
 
         Ok(Response {
@@ -369,16 +368,16 @@
             status_code,
             url,
         })
     }
 
     fn get(
         &self,
-        url: &str,
         py: Python,
+        url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
@@ -547,12 +546,174 @@
             auth,
             auth_bearer,
             timeout,
         )
     }
 }
 
+/// Convenience functions that use a default Client instance under the hood
+#[pyfunction]
+fn get(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.get(py, url, params, headers, auth, auth_bearer, timeout)
+}
+
+#[pyfunction]
+fn head(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.head(py, url, params, headers, auth, auth_bearer, timeout)
+}
+
+#[pyfunction]
+fn options(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.options(py, url, params, headers, auth, auth_bearer, timeout)
+}
+
+#[pyfunction]
+fn delete(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.delete(py, url, params, headers, auth, auth_bearer, timeout)
+}
+
+#[pyfunction]
+fn post(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    content: Option<Vec<u8>>,
+    data: Option<HashMap<String, String>>,
+    files: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.post(
+        py,
+        url,
+        params,
+        headers,
+        content,
+        data,
+        files,
+        auth,
+        auth_bearer,
+        timeout,
+    )
+}
+
+#[pyfunction]
+fn put(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    content: Option<Vec<u8>>,
+    data: Option<HashMap<String, String>>,
+    files: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.put(
+        py,
+        url,
+        params,
+        headers,
+        content,
+        data,
+        files,
+        auth,
+        auth_bearer,
+        timeout,
+    )
+}
+
+#[pyfunction]
+fn patch(
+    py: Python,
+    url: &str,
+    params: Option<HashMap<String, String>>,
+    headers: Option<HashMap<String, String>>,
+    content: Option<Vec<u8>>,
+    data: Option<HashMap<String, String>>,
+    files: Option<HashMap<String, String>>,
+    auth: Option<(String, Option<String>)>,
+    auth_bearer: Option<String>,
+    timeout: Option<f64>,
+) -> PyResult<Response> {
+    let client = Client::new(
+        None, None, None, None, None, None, None, None, None, None, None, None, None, None,
+    )?;
+    client.patch(
+        py,
+        url,
+        params,
+        headers,
+        content,
+        data,
+        files,
+        auth,
+        auth_bearer,
+        timeout,
+    )
+}
+
 #[pymodule]
 fn pyreqwest_impersonate(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<Client>()?;
+    m.add_function(wrap_pyfunction!(get, m)?)?;
+    m.add_function(wrap_pyfunction!(head, m)?)?;
+    m.add_function(wrap_pyfunction!(options, m)?)?;
+    m.add_function(wrap_pyfunction!(delete, m)?)?;
+    m.add_function(wrap_pyfunction!(post, m)?)?;
+    m.add_function(wrap_pyfunction!(patch, m)?)?;
+    m.add_function(wrap_pyfunction!(put, m)?)?;
     Ok(())
 }
```

### Comparing `pyreqwest_impersonate-0.3.0/src/response.rs` & `pyreqwest_impersonate-0.3.1/src/response.rs`

 * *Files 3% similar despite different names*

```diff
@@ -33,21 +33,21 @@
         let encoding_bytes = &self.encoding.bind(py).to_string().as_bytes().to_vec();
 
         // Convert Py<PyBytes> to &[u8]
         let raw_bytes = &self.content.bind(py).as_bytes();
 
         // Release the GIL here because decoding can be CPU-intensive
         let (decoded_str, detected_encoding_name) = py.allow_threads(move || {
-            let encoding = Encoding::for_label(&encoding_bytes).ok_or_else(|| {
+            let encoding = Encoding::for_label(encoding_bytes).ok_or_else(|| {
                 PyErr::new::<exceptions::PyValueError, _>(format!(
                     "Unsupported charset: {}",
-                    String::from_utf8_lossy(&encoding_bytes)
+                    String::from_utf8_lossy(encoding_bytes)
                 ))
             })?;
-            let (decoded_str, detected_encoding, _) = encoding.decode(&raw_bytes);
+            let (decoded_str, detected_encoding, _) = encoding.decode(raw_bytes);
             // Return the decoded string and the name of the detected encoding
             Ok::<(String, String), PyErr>((
                 decoded_str.to_string(),
                 detected_encoding.name().to_string(),
             ))
         })?;
```

### Comparing `pyreqwest_impersonate-0.3.0/tests/test_client.py` & `pyreqwest_impersonate-0.3.1/tests/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "https://httpbin.org/anything",
         auth_bearer=auth_bearer,
         headers=headers,
         params=params,
     )
     assert response.status_code == 200
     json_data = response.json()
+    assert json_data["method"] == "GET"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
     assert "Bearer bearerXXXXXXXXXXXXXXXXXXXX" in response.text
     assert b"Bearer bearerXXXXXXXXXXXXXXXXXXXX" in response.content
 
 
@@ -68,14 +69,15 @@
         auth=auth,
         headers=headers,
         params=params,
         content=content,
     )
     assert response.status_code == 200
     json_data = response.json()
+    assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Basic dXNlcjpwYXNzd29yZA=="
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
     assert json_data["data"] == "test content"
 
 
 @retry()
@@ -90,14 +92,15 @@
         auth_bearer=auth_bearer,
         headers=headers,
         params=params,
         data=data,
     )
     assert response.status_code == 200
     json_data = response.json()
+    assert json_data["method"] == "POST"
     assert json_data["headers"]["X-Test"] == "test"
     assert json_data["headers"]["Authorization"] == "Bearer bearerXXXXXXXXXXXXXXXXXXXX"
     assert json_data["args"] == {"x": "aaa", "y": "bbb"}
     received_data_dict = parse_qs(json_data["data"])
     assert received_data_dict == {"key1": ["value1"], "key2": ["value2"]}
```

### Comparing `pyreqwest_impersonate-0.3.0/Cargo.lock` & `pyreqwest_impersonate-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -909,15 +909,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "encoding_rs",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
 ]
```

### Comparing `pyreqwest_impersonate-0.3.0/pyproject.toml` & `pyreqwest_impersonate-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.3.0/PKG-INFO` & `pyreqwest_impersonate-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -80,15 +80,15 @@
                 "chrome_107","chrome_109","chrome_114","chrome_116","chrome_117","chrome_118","chrome_119", 
                 "chrome_120","chrome_123"
             Safari: "safari_12","safari_15_3","safari_15_5","safari_15_6_1","safari_16","safari_16_5","safari_17_2_1"
             OkHttp: "okhttp_3_9","okhttp_3_11","okhttp_3_13","okhttp_3_14","okhttp_4_9","okhttp_4_10","okhttp_5"
             Edge: "edge_99","edge_101","edge_120"
         follow_redirects (bool, optional): Whether to follow redirects. Default is True.
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
-        verify (bool, optional): Verify SSL certificates. Default is True.
+        verify (bool, optional): Verify SSL certificates. Default is False.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
          
     """
 ```
 
 #### Client Methods
@@ -127,32 +127,37 @@
 
     """
 ```
 
 #### Example
 
 ```python
-from pyreqwest_impersonate import Client
+import pyreqwest_impersonate as pri
 
-client = Client(impersonate="chrome_123")
+client = pri.Client(impersonate="chrome_123")
 
 # get request
 resp = client.get("https://tls.peet.ws/api/all")
 print(resp.json())
 
 # post request
 data = {"key1": "value1", "key2": "value2"}
 auth = ("user", "password")
 resp = client.post(url="https://httpbin.org/anything", data=data, auth=auth)
-print(response.content)  # Get the content as bytes
-print(response.cookies)  # Access cookies
-print(response.headers)  # Access headers
-print(response.json())  # Parse the content as JSON
-print(response.status_code)  # Access the status code
-print(response.text)  # Decode the content as text
-print(response.url)  # Access the URL
+print(resp.content)
+print(resp.cookies)
+print(resp.headers)
+print(resp.json())
+print(resp.status_code)
+print(resp.text)
+print(resp.url)
+
+# You can also use convenience functions that use a default Client instance under the hood:
+# pri.get() | pri.head() | pri.options() | pri.delete() | pri.post | pri.patch | pri.put
+resp = pri.get("https://httpbin.org/anything") # Default Client does not impersonate a browser
+resp = pri.Client(impersonate="chrome_123").get("https://httpbin.org/anything")  
 ```
 ### II. AsyncClient
 
 TODO
```

