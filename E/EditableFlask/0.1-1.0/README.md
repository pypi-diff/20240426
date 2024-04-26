# Comparing `tmp/EditableFlask-0.1.tar.gz` & `tmp/EditableFlask-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EditableFlask-0.1.tar", last modified: Wed Apr 24 02:06:04 2024, max compression
+gzip compressed data, was "EditableFlask-1.0.tar", last modified: Fri Apr 26 15:13:49 2024, max compression
```

## Comparing `EditableFlask-0.1.tar` & `EditableFlask-1.0.tar`

### file list

```diff
@@ -1,17 +1,52 @@
-drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-24 02:06:04.686338 EditableFlask-0.1/
-drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-24 02:06:04.684337 EditableFlask-0.1/EditableFlask/
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     5638 2024-04-24 00:52:02.000000 EditableFlask-0.1/EditableFlask/__init__.py
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     1645 2024-04-12 07:18:20.000000 EditableFlask-0.1/EditableFlask/editable.py
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9333 2024-04-24 01:11:25.000000 EditableFlask-0.1/EditableFlask/views.py
-drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-24 02:06:04.685337 EditableFlask-0.1/EditableFlask.egg-info/
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9171 2024-04-24 02:06:04.000000 EditableFlask-0.1/EditableFlask.egg-info/PKG-INFO
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)      307 2024-04-24 02:06:04.000000 EditableFlask-0.1/EditableFlask.egg-info/SOURCES.txt
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)        1 2024-04-24 02:06:04.000000 EditableFlask-0.1/EditableFlask.egg-info/dependency_links.txt
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       18 2024-04-24 02:06:04.000000 EditableFlask-0.1/EditableFlask.egg-info/requires.txt
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       14 2024-04-24 02:06:04.000000 EditableFlask-0.1/EditableFlask.egg-info/top_level.txt
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     1060 2024-04-04 05:06:22.000000 EditableFlask-0.1/LICENSE
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       81 2024-02-29 09:56:31.000000 EditableFlask-0.1/MANIFEST.in
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9171 2024-04-24 02:06:04.686338 EditableFlask-0.1/PKG-INFO
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     8673 2024-04-24 02:05:37.000000 EditableFlask-0.1/README.md
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)      618 2024-04-24 02:06:04.687337 EditableFlask-0.1/setup.cfg
--rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)      824 2024-04-24 02:05:57.000000 EditableFlask-0.1/setup.py
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.256684 EditableFlask-1.0/
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.250684 EditableFlask-1.0/EditableFlask/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     5638 2024-04-24 00:52:02.000000 EditableFlask-1.0/EditableFlask/__init__.py
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.252684 EditableFlask-1.0/EditableFlask/assets/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     6148 2024-02-29 09:56:32.000000 EditableFlask-1.0/EditableFlask/assets/.DS_Store
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.249684 EditableFlask-1.0/EditableFlask/assets/bootstrap/
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.253684 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    21368 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap-theme.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    23071 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap-theme.css.map
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    18860 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap-theme.min.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)   132546 2024-02-29 09:56:35.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)   220790 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)   109518 2024-02-29 09:56:35.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       90 2024-02-29 09:56:35.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/css/navbar.css
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.254684 EditableFlask-1.0/EditableFlask/assets/bootstrap/fonts/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    20335 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    62927 2024-02-29 09:56:33.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    41280 2024-02-29 09:56:33.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    23320 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.254684 EditableFlask-1.0/EditableFlask/assets/bootstrap/js/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    60681 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/js/bootstrap.js
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    31819 2024-02-29 09:56:34.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.249684 EditableFlask-1.0/EditableFlask/assets/bootstrap-switch/
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.252684 EditableFlask-1.0/EditableFlask/assets/bootstrap-switch/css/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     5655 2021-01-02 23:20:40.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap-switch/css/bootstrap-switch.min.css
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.252684 EditableFlask-1.0/EditableFlask/assets/bootstrap-switch/js/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    14327 2021-01-02 23:20:40.000000 EditableFlask-1.0/EditableFlask/assets/bootstrap-switch/js/bootstrap-switch.min.js
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)   209790 2024-04-26 14:40:27.000000 EditableFlask-1.0/EditableFlask/assets/favicon.ico
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     4890 2024-04-22 02:35:07.000000 EditableFlask-1.0/EditableFlask/assets/script.js
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     4829 2024-04-22 02:16:58.000000 EditableFlask-1.0/EditableFlask/assets/style.css
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.255684 EditableFlask-1.0/EditableFlask/assets/summernote/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)   147671 2024-02-29 09:56:33.000000 EditableFlask-1.0/EditableFlask/assets/summernote/summernote-bs3.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    10412 2024-02-29 09:56:33.000000 EditableFlask-1.0/EditableFlask/assets/summernote/summernote.css
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    56537 2024-02-29 09:56:33.000000 EditableFlask-1.0/EditableFlask/assets/summernote/summernote.min.js
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     1773 2024-04-26 14:31:56.000000 EditableFlask-1.0/EditableFlask/editable.py
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.255684 EditableFlask-1.0/EditableFlask/templates/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     6897 2024-04-26 14:40:55.000000 EditableFlask-1.0/EditableFlask/templates/edits-admin.html
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     2376 2024-04-26 14:41:04.000000 EditableFlask-1.0/EditableFlask/templates/login_prompt.html
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)    20738 2024-04-26 14:41:07.000000 EditableFlask-1.0/EditableFlask/templates/static.html
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9333 2024-04-24 01:11:25.000000 EditableFlask-1.0/EditableFlask/views.py
+drwxr-xr-x   0 mahirshah  (1000) mahirshah  (1001)        0 2024-04-26 15:13:49.256684 EditableFlask-1.0/EditableFlask.egg-info/
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9626 2024-04-26 15:13:49.000000 EditableFlask-1.0/EditableFlask.egg-info/PKG-INFO
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     1585 2024-04-26 15:13:49.000000 EditableFlask-1.0/EditableFlask.egg-info/SOURCES.txt
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)        1 2024-04-26 15:13:49.000000 EditableFlask-1.0/EditableFlask.egg-info/dependency_links.txt
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       18 2024-04-26 15:13:49.000000 EditableFlask-1.0/EditableFlask.egg-info/requires.txt
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       14 2024-04-26 15:13:49.000000 EditableFlask-1.0/EditableFlask.egg-info/top_level.txt
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     1067 2024-04-23 15:46:21.000000 EditableFlask-1.0/LICENSE
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)       70 2024-04-26 09:24:31.000000 EditableFlask-1.0/MANIFEST.in
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9626 2024-04-26 15:13:49.256684 EditableFlask-1.0/PKG-INFO
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)     9128 2024-04-26 14:56:18.000000 EditableFlask-1.0/README.md
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)      618 2024-04-26 15:13:49.257684 EditableFlask-1.0/setup.cfg
+-rw-r--r--   0 mahirshah  (1000) mahirshah  (1001)      910 2024-04-26 15:13:11.000000 EditableFlask-1.0/setup.py
```

### Comparing `EditableFlask-0.1/EditableFlask/__init__.py` & `EditableFlask-1.0/EditableFlask/__init__.py`

 * *Files identical despite different names*

### Comparing `EditableFlask-0.1/EditableFlask/editable.py` & `EditableFlask-1.0/EditableFlask/editable.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,17 +18,19 @@
         if isinstance(section, Template):
             original = section.render()
         elif isinstance(section, list):
             original = "".join(str(s) for s in section)
         else:
             original = section
         new = ''
+        RemoveString = """Output(nodes=[TemplateData(data=" """
+        RemoveString = RemoveString[:-1]
         for i in original:
             new = new + str(i)
-            if new == "Output(nodes=[TemplateData(data='":
+            if new == "Output(nodes=[TemplateData(data='" or new == RemoveString:
                 new = ''
         original = new[:-4]
         _db.setdefault(parser.name, OrderedDict())
         _db[parser.name].setdefault(key, OrderedDict())
         _db[parser.name][key].setdefault("original", original)
         _db[parser.name][key].setdefault("edited", None)
         if _db[parser.name][key].get("edited", None):
```

### Comparing `EditableFlask-0.1/EditableFlask/views.py` & `EditableFlask-1.0/EditableFlask/views.py`

 * *Files identical despite different names*

### Comparing `EditableFlask-0.1/EditableFlask.egg-info/PKG-INFO` & `EditableFlask-1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: EditableFlask
-Version: 0.1
-Summary: Addon to Library named flask which helps to edit html content in running app0
-Home-page: https://github.com/MahirShah07/
-Author: Mahir Shah
-Author-email: mahir.shah.sd@gmail.com
-License: MIT
-Keywords: editable_flask
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Flask
-Requires-Dist: flask_login
-
 
 # Editable Flask
 
 Tired of constant client requests to tweak that elusive snippet or image on your **/about** page?
 
 Enter **EditableFlask**. Simply mark sections of your templates with **{% editable %}**, and voilà, they're ready for modification in a sleek admin panel. Say goodbye to the hassle of copy adjustments.
 
@@ -42,14 +26,29 @@
 from EditableFlask import Edits
 import os
 
 app = Flask(__name__)
 app.config['FILE_PATH'] = os.path.dirname(__file__)
 edits = Edits(app)
 
+@app.route("/")
+    def index():
+        return render_template('index.html')
+```
+```html
+<!--index.html-->
+<!DOCTYPE html>
+<html>
+<body>
+    <!--Add these editable jinja tags to mark them editable-->
+<h1>{% editable 'heading' %}My First Heading{% endeditable %}</h1>
+<p>{% editable 'paragraph' %}My first paragraph.{% endeditable %}</p>
+</body>
+</html>
+
 ```
 
 ## Edits Seaction
 Edit any page with registered editable sections directly in the interface. Currently, only static HTML is supported, with Jinja2 support on the roadmap.
 
 ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image2.png)
 
@@ -73,25 +72,29 @@
 
 Now you can access all your edits from **/edits** (default) but to make it secure so that no one else could access it is advised to add a security system. There are two ways this can be done:
 
 ## Security
 **Security Reminder**: EditableFlask doesn't presume your authentication method by default. Protect the admin interface from following methods from developer.
 * **Automatic Lock** (Reccomended): In EditableFlask itself there is an **sqlalchamy** based login manager if you want to use that use the following code. There are few points to consider before using the method.
     ```bash
-    from flask import Flask
+    from flask import Flask, render_template
     from EditableFlask import Edits
     import os
 
     app = Flask(__name__)
     app.secret_key = 'your_secret_key_here' #DO NOT SHARE THIS WITH ANYONE
     app.config['FILE_PATH'] = os.path.dirname(__file__)
     app.config['SQL_EDITS_LOCKED'] = True
     app.config['EDITS_USERNAME'] = 'your_username'
     app.config['EDITS_PASSWORD'] = 'your_password'
     edits = Edits(app)
+
+    @app.route("/")
+    def index():
+        return render_template('index.html')
     ```
     ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image3.png)
     * **EDITS_USERNAME & EDITS_PASSWORD**
         * **Remove EDITS_USERNAME & EDITS_PASSWORD**: After running the app for first time remove EDITS_USERNAME & EDITS_PASSWORD from congif as as soon as the app recives the  EDITS_USERNAME & EDITS_PASSWORD it creates users and keeping USAMENAME and PASSSWORD in your file is not reecomended for deployment purposes.
         * **Using only EDITS_USERNAME or EDITS_PASSWORD**: In the EditableFlask there is a function where if only EDITS_USERNAME or only EDITS_PASSWORD is provided then your username and password will be same.
     * **Few other Terms you could define:**
         * **EDITS_URL**: It is the url where you will be able to access you dashbaord. Here is an example of how you could define it.
```

### Comparing `EditableFlask-0.1/LICENSE` & `EditableFlask-1.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,21 @@
-Copyright 2024 Mahir Shah
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2024 Mahir Shah
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `EditableFlask-0.1/PKG-INFO` & `EditableFlask-1.0/EditableFlask.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EditableFlask
-Version: 0.1
+Version: 1.0
 Summary: Addon to Library named flask which helps to edit html content in running app0
 Home-page: https://github.com/MahirShah07/
 Author: Mahir Shah
 Author-email: mahir.shah.sd@gmail.com
 License: MIT
 Keywords: editable_flask
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,14 +42,29 @@
 from EditableFlask import Edits
 import os
 
 app = Flask(__name__)
 app.config['FILE_PATH'] = os.path.dirname(__file__)
 edits = Edits(app)
 
+@app.route("/")
+    def index():
+        return render_template('index.html')
+```
+```html
+<!--index.html-->
+<!DOCTYPE html>
+<html>
+<body>
+    <!--Add these editable jinja tags to mark them editable-->
+<h1>{% editable 'heading' %}My First Heading{% endeditable %}</h1>
+<p>{% editable 'paragraph' %}My first paragraph.{% endeditable %}</p>
+</body>
+</html>
+
 ```
 
 ## Edits Seaction
 Edit any page with registered editable sections directly in the interface. Currently, only static HTML is supported, with Jinja2 support on the roadmap.
 
 ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image2.png)
 
@@ -73,25 +88,29 @@
 
 Now you can access all your edits from **/edits** (default) but to make it secure so that no one else could access it is advised to add a security system. There are two ways this can be done:
 
 ## Security
 **Security Reminder**: EditableFlask doesn't presume your authentication method by default. Protect the admin interface from following methods from developer.
 * **Automatic Lock** (Reccomended): In EditableFlask itself there is an **sqlalchamy** based login manager if you want to use that use the following code. There are few points to consider before using the method.
     ```bash
-    from flask import Flask
+    from flask import Flask, render_template
     from EditableFlask import Edits
     import os
 
     app = Flask(__name__)
     app.secret_key = 'your_secret_key_here' #DO NOT SHARE THIS WITH ANYONE
     app.config['FILE_PATH'] = os.path.dirname(__file__)
     app.config['SQL_EDITS_LOCKED'] = True
     app.config['EDITS_USERNAME'] = 'your_username'
     app.config['EDITS_PASSWORD'] = 'your_password'
     edits = Edits(app)
+
+    @app.route("/")
+    def index():
+        return render_template('index.html')
     ```
     ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image3.png)
     * **EDITS_USERNAME & EDITS_PASSWORD**
         * **Remove EDITS_USERNAME & EDITS_PASSWORD**: After running the app for first time remove EDITS_USERNAME & EDITS_PASSWORD from congif as as soon as the app recives the  EDITS_USERNAME & EDITS_PASSWORD it creates users and keeping USAMENAME and PASSSWORD in your file is not reecomended for deployment purposes.
         * **Using only EDITS_USERNAME or EDITS_PASSWORD**: In the EditableFlask there is a function where if only EDITS_USERNAME or only EDITS_PASSWORD is provided then your username and password will be same.
     * **Few other Terms you could define:**
         * **EDITS_URL**: It is the url where you will be able to access you dashbaord. Here is an example of how you could define it.
```

### Comparing `EditableFlask-0.1/README.md` & `EditableFlask-1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: EditableFlask
+Version: 1.0
+Summary: Addon to Library named flask which helps to edit html content in running app0
+Home-page: https://github.com/MahirShah07/
+Author: Mahir Shah
+Author-email: mahir.shah.sd@gmail.com
+License: MIT
+Keywords: editable_flask
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Flask
+Requires-Dist: flask_login
+
 
 # Editable Flask
 
 Tired of constant client requests to tweak that elusive snippet or image on your **/about** page?
 
 Enter **EditableFlask**. Simply mark sections of your templates with **{% editable %}**, and voilà, they're ready for modification in a sleek admin panel. Say goodbye to the hassle of copy adjustments.
 
@@ -26,14 +42,29 @@
 from EditableFlask import Edits
 import os
 
 app = Flask(__name__)
 app.config['FILE_PATH'] = os.path.dirname(__file__)
 edits = Edits(app)
 
+@app.route("/")
+    def index():
+        return render_template('index.html')
+```
+```html
+<!--index.html-->
+<!DOCTYPE html>
+<html>
+<body>
+    <!--Add these editable jinja tags to mark them editable-->
+<h1>{% editable 'heading' %}My First Heading{% endeditable %}</h1>
+<p>{% editable 'paragraph' %}My first paragraph.{% endeditable %}</p>
+</body>
+</html>
+
 ```
 
 ## Edits Seaction
 Edit any page with registered editable sections directly in the interface. Currently, only static HTML is supported, with Jinja2 support on the roadmap.
 
 ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image2.png)
 
@@ -57,25 +88,29 @@
 
 Now you can access all your edits from **/edits** (default) but to make it secure so that no one else could access it is advised to add a security system. There are two ways this can be done:
 
 ## Security
 **Security Reminder**: EditableFlask doesn't presume your authentication method by default. Protect the admin interface from following methods from developer.
 * **Automatic Lock** (Reccomended): In EditableFlask itself there is an **sqlalchamy** based login manager if you want to use that use the following code. There are few points to consider before using the method.
     ```bash
-    from flask import Flask
+    from flask import Flask, render_template
     from EditableFlask import Edits
     import os
 
     app = Flask(__name__)
     app.secret_key = 'your_secret_key_here' #DO NOT SHARE THIS WITH ANYONE
     app.config['FILE_PATH'] = os.path.dirname(__file__)
     app.config['SQL_EDITS_LOCKED'] = True
     app.config['EDITS_USERNAME'] = 'your_username'
     app.config['EDITS_PASSWORD'] = 'your_password'
     edits = Edits(app)
+
+    @app.route("/")
+    def index():
+        return render_template('index.html')
     ```
     ![App Screenshot](https://raw.githubusercontent.com/MahirShah07/EditableFlask/main/readme-images/Image3.png)
     * **EDITS_USERNAME & EDITS_PASSWORD**
         * **Remove EDITS_USERNAME & EDITS_PASSWORD**: After running the app for first time remove EDITS_USERNAME & EDITS_PASSWORD from congif as as soon as the app recives the  EDITS_USERNAME & EDITS_PASSWORD it creates users and keeping USAMENAME and PASSSWORD in your file is not reecomended for deployment purposes.
         * **Using only EDITS_USERNAME or EDITS_PASSWORD**: In the EditableFlask there is a function where if only EDITS_USERNAME or only EDITS_PASSWORD is provided then your username and password will be same.
     * **Few other Terms you could define:**
         * **EDITS_URL**: It is the url where you will be able to access you dashbaord. Here is an example of how you could define it.
```

### Comparing `EditableFlask-0.1/setup.cfg` & `EditableFlask-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `EditableFlask-0.1/setup.py` & `EditableFlask-1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 # Read the contents of README.md
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='EditableFlask',
-    version='0.1',
+    version='1.0',
     description='Addon to Library named flask which helps to edit html content in running app0',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type as Markdown
     url='',
     author='Mahir Shah',
     author_email='mahir.shah.sd@gmail.com',
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: MIT License',
     ],
     keywords='editable_flask',
     packages=find_packages(),
+    package_data={
+        'EditableFlask': ['templates/*.html', 'assets/**'],
+    },
     install_requires=['Flask', 'flask_login']
 )
```

