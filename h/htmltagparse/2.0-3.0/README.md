# Comparing `tmp/htmltagparse-2.0.tar.gz` & `tmp/htmltagparse-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmltagparse-2.0.tar", last modified: Wed Apr 10 00:20:04 2024, max compression
+gzip compressed data, was "htmltagparse-3.0.tar", last modified: Fri Apr 26 04:09:00 2024, max compression
```

## Comparing `htmltagparse-2.0.tar` & `htmltagparse-3.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.508975 htmltagparse-2.0/
--rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-03 11:14:27.000000 htmltagparse-2.0/MANIFEST.in
--rw-r--r--   0 xyz       (1000) xyz       (1000)     3374 2024-04-10 00:20:04.508975 htmltagparse-2.0/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2591 2024-04-10 00:16:09.000000 htmltagparse-2.0/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.507975 htmltagparse-2.0/htmltagparse/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      704 2024-04-10 00:18:19.000000 htmltagparse-2.0/htmltagparse/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      747 2024-04-08 02:07:57.000000 htmltagparse-2.0/htmltagparse/build.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      316 2024-04-06 17:27:54.000000 htmltagparse-2.0/htmltagparse/exceptions.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1696 2024-04-06 23:56:18.000000 htmltagparse-2.0/htmltagparse/html_tags.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     8397 2024-04-09 23:46:17.000000 htmltagparse-2.0/htmltagparse/parser.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-10 00:20:04.508975 htmltagparse-2.0/htmltagparse.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     3374 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      349 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       65 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/requires.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-10 00:20:04.000000 htmltagparse-2.0/htmltagparse.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       64 2024-04-03 11:47:50.000000 htmltagparse-2.0/requirements.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-10 00:20:04.508975 htmltagparse-2.0/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1011 2024-04-06 15:43:41.000000 htmltagparse-2.0/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-26 04:09:00.360122 htmltagparse-3.0/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       24 2024-04-03 11:14:27.000000 htmltagparse-3.0/MANIFEST.in
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3583 2024-04-26 04:09:00.360122 htmltagparse-3.0/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2785 2024-04-26 04:01:13.000000 htmltagparse-3.0/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-26 04:09:00.359122 htmltagparse-3.0/htmltagparse/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1400 2024-04-26 04:08:33.000000 htmltagparse-3.0/htmltagparse/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      747 2024-04-08 02:07:57.000000 htmltagparse-3.0/htmltagparse/build.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1603 2024-04-26 02:41:35.000000 htmltagparse-3.0/htmltagparse/cleaner.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      333 2024-04-21 05:38:18.000000 htmltagparse-3.0/htmltagparse/exceptions.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1696 2024-04-06 23:56:18.000000 htmltagparse-3.0/htmltagparse/html_tags.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)    11246 2024-04-26 04:05:23.000000 htmltagparse-3.0/htmltagparse/parser.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-26 04:09:00.360122 htmltagparse-3.0/htmltagparse.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3583 2024-04-26 04:09:00.000000 htmltagparse-3.0/htmltagparse.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      373 2024-04-26 04:09:00.000000 htmltagparse-3.0/htmltagparse.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-26 04:09:00.000000 htmltagparse-3.0/htmltagparse.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       48 2024-04-26 04:09:00.000000 htmltagparse-3.0/htmltagparse.egg-info/requires.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       13 2024-04-26 04:09:00.000000 htmltagparse-3.0/htmltagparse.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       47 2024-04-24 08:12:28.000000 htmltagparse-3.0/requirements.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-26 04:09:00.360122 htmltagparse-3.0/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1057 2024-04-24 08:29:42.000000 htmltagparse-3.0/setup.py
```

### Comparing `htmltagparse-2.0/PKG-INFO` & `htmltagparse-3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 Metadata-Version: 2.1
 Name: htmltagparse
-Version: 2.0
+Version: 3.0
 Summary: A tool designed to quickly parse html tags and elements.
 Home-page: https://github.com/xyzpw/htmltagparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: timeoutcall==1.*
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: requests==2.*
 Requires-Dist: html5lib==1.*
 
 # htmltagparse
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/htmltagparse)
 
-A tool designed to quickly parse html tags and elements.
+A tool designed to quickly parse HTML tags and elements.
 
 ## Prerequisites
 - Pip packages:
-  - timeoutcall==1.*
   - beautifulsoup4==4.*
   - html5lib==1.*
   - requests==2.*
 
+- Optional packages:
+  - timeoutcall==1.*
+
 ## Usage
 ### Reading Page Titles
-Firstly, if you would like to view a page title alone, you could use the `titleFromUri` function:
+Firstly, if you would like to view page info alone, you could use a few functions for this:
 ```python
-from htmltagparse import titleFromUri
+import htmltagparse
+title = htmltagparse.titleFromUri("https://github.com/")
+print(title) # ouput: GitHub: Let’s build from here · GitHub
 
-websiteTitle = titleFromUri("https://github.com/")
-print(websiteTitle) # output: GitHub: Let’s build from here · GitHub
+metadata = htmltagparse.metadataFromUri("https://github.com/") # meta tags from github
 ```
 
 ### Building Pages
 #### Building Pages via URI
 ```python
 from htmltagparse import build
 
-brave = build.fromUri("https://search.brave.com/", timeout=20)
+brave = build.fromUri("https://search.brave.com/")
+print(brave.response) #output: (200, 'OK')
 print(brave.tags) #list of tags found on the specified page
-print(brave.searchTag("footer")) #displays a list of innerHtml content to the footer tags
-print(brave.searchTag("footer", htmlFormat=False)[0]) #output: © Brave Software Brave Search API Summarizer Helpful answers Report a security issue
+print(brave.elapsed) #the time taken to create the html page class
+print(brave.title) #title of the html page
 ```
+This is not limited to these values alone; there are more values associated with an html page.
 
 #### Building Pages via HTML
 ```python
 from htmltagparse import HtmlPage
 from requests import get
 
 htmlContent = get("https://duckduckgo.com/").text
@@ -80,27 +85,23 @@
   videoTags = re.findall(r"(?:\"|\')(?P<tag>.*?)(?:\'|\")(?:\,|\])", videoTags)
 except:
   videoTags = "no tags found"
 
 print(videoTags)
 ```
 
-Another way you could get tags from a Youtube video:
+Another way you could get tags from a Youtube video is with the `find` function, example:
 ```python
 import htmltagparse
 
-#youtube video id
-videoId = ""
-video = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
-
-for i in video.metadata:
-  if i.get("name") == "keywords":
-    tags = i.get("content").split(", ")
-    break
-print(i)
+videoId = "" #video id here
+yt = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
+elTagOpening = yt.find("meta", attrs={"name": "keywords"})[0]
+videoKeywords = htmltagparse.getElementAttributeValue(elTagOpening, "content").split(", ")
+print(videoKeywords) # tags of the youtube video
 ```
 
 ## Developers
 ### Building to Wheel File
 - cd into root directory of this repository
 - run `python3 -m build`
```

### Comparing `htmltagparse-2.0/README.md` & `htmltagparse-3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # htmltagparse
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/htmltagparse)
 
-A tool designed to quickly parse html tags and elements.
+A tool designed to quickly parse HTML tags and elements.
 
 ## Prerequisites
 - Pip packages:
-  - timeoutcall==1.*
   - beautifulsoup4==4.*
   - html5lib==1.*
   - requests==2.*
 
+- Optional packages:
+  - timeoutcall==1.*
+
 ## Usage
 ### Reading Page Titles
-Firstly, if you would like to view a page title alone, you could use the `titleFromUri` function:
+Firstly, if you would like to view page info alone, you could use a few functions for this:
 ```python
-from htmltagparse import titleFromUri
+import htmltagparse
+title = htmltagparse.titleFromUri("https://github.com/")
+print(title) # ouput: GitHub: Let’s build from here · GitHub
 
-websiteTitle = titleFromUri("https://github.com/")
-print(websiteTitle) # output: GitHub: Let’s build from here · GitHub
+metadata = htmltagparse.metadataFromUri("https://github.com/") # meta tags from github
 ```
 
 ### Building Pages
 #### Building Pages via URI
 ```python
 from htmltagparse import build
 
-brave = build.fromUri("https://search.brave.com/", timeout=20)
+brave = build.fromUri("https://search.brave.com/")
+print(brave.response) #output: (200, 'OK')
 print(brave.tags) #list of tags found on the specified page
-print(brave.searchTag("footer")) #displays a list of innerHtml content to the footer tags
-print(brave.searchTag("footer", htmlFormat=False)[0]) #output: © Brave Software Brave Search API Summarizer Helpful answers Report a security issue
+print(brave.elapsed) #the time taken to create the html page class
+print(brave.title) #title of the html page
 ```
+This is not limited to these values alone; there are more values associated with an html page.
 
 #### Building Pages via HTML
 ```python
 from htmltagparse import HtmlPage
 from requests import get
 
 htmlContent = get("https://duckduckgo.com/").text
@@ -57,27 +62,23 @@
   videoTags = re.findall(r"(?:\"|\')(?P<tag>.*?)(?:\'|\")(?:\,|\])", videoTags)
 except:
   videoTags = "no tags found"
 
 print(videoTags)
 ```
 
-Another way you could get tags from a Youtube video:
+Another way you could get tags from a Youtube video is with the `find` function, example:
 ```python
 import htmltagparse
 
-#youtube video id
-videoId = ""
-video = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
-
-for i in video.metadata:
-  if i.get("name") == "keywords":
-    tags = i.get("content").split(", ")
-    break
-print(i)
+videoId = "" #video id here
+yt = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
+elTagOpening = yt.find("meta", attrs={"name": "keywords"})[0]
+videoKeywords = htmltagparse.getElementAttributeValue(elTagOpening, "content").split(", ")
+print(videoKeywords) # tags of the youtube video
 ```
 
 ## Developers
 ### Building to Wheel File
 - cd into root directory of this repository
 - run `python3 -m build`
```

### Comparing `htmltagparse-2.0/htmltagparse/build.py` & `htmltagparse-3.0/htmltagparse/build.py`

 * *Files identical despite different names*

### Comparing `htmltagparse-2.0/htmltagparse/html_tags.py` & `htmltagparse-3.0/htmltagparse/html_tags.py`

 * *Files identical despite different names*

### Comparing `htmltagparse-2.0/htmltagparse.egg-info/PKG-INFO` & `htmltagparse-3.0/htmltagparse.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,67 @@
 Metadata-Version: 2.1
 Name: htmltagparse
-Version: 2.0
+Version: 3.0
 Summary: A tool designed to quickly parse html tags and elements.
 Home-page: https://github.com/xyzpw/htmltagparse/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: timeoutcall==1.*
 Requires-Dist: beautifulsoup4==4.*
 Requires-Dist: requests==2.*
 Requires-Dist: html5lib==1.*
 
 # htmltagparse
 ![Pepy Total Downlods](https://img.shields.io/pepy/dt/htmltagparse)
 
-A tool designed to quickly parse html tags and elements.
+A tool designed to quickly parse HTML tags and elements.
 
 ## Prerequisites
 - Pip packages:
-  - timeoutcall==1.*
   - beautifulsoup4==4.*
   - html5lib==1.*
   - requests==2.*
 
+- Optional packages:
+  - timeoutcall==1.*
+
 ## Usage
 ### Reading Page Titles
-Firstly, if you would like to view a page title alone, you could use the `titleFromUri` function:
+Firstly, if you would like to view page info alone, you could use a few functions for this:
 ```python
-from htmltagparse import titleFromUri
+import htmltagparse
+title = htmltagparse.titleFromUri("https://github.com/")
+print(title) # ouput: GitHub: Let’s build from here · GitHub
 
-websiteTitle = titleFromUri("https://github.com/")
-print(websiteTitle) # output: GitHub: Let’s build from here · GitHub
+metadata = htmltagparse.metadataFromUri("https://github.com/") # meta tags from github
 ```
 
 ### Building Pages
 #### Building Pages via URI
 ```python
 from htmltagparse import build
 
-brave = build.fromUri("https://search.brave.com/", timeout=20)
+brave = build.fromUri("https://search.brave.com/")
+print(brave.response) #output: (200, 'OK')
 print(brave.tags) #list of tags found on the specified page
-print(brave.searchTag("footer")) #displays a list of innerHtml content to the footer tags
-print(brave.searchTag("footer", htmlFormat=False)[0]) #output: © Brave Software Brave Search API Summarizer Helpful answers Report a security issue
+print(brave.elapsed) #the time taken to create the html page class
+print(brave.title) #title of the html page
 ```
+This is not limited to these values alone; there are more values associated with an html page.
 
 #### Building Pages via HTML
 ```python
 from htmltagparse import HtmlPage
 from requests import get
 
 htmlContent = get("https://duckduckgo.com/").text
@@ -80,27 +85,23 @@
   videoTags = re.findall(r"(?:\"|\')(?P<tag>.*?)(?:\'|\")(?:\,|\])", videoTags)
 except:
   videoTags = "no tags found"
 
 print(videoTags)
 ```
 
-Another way you could get tags from a Youtube video:
+Another way you could get tags from a Youtube video is with the `find` function, example:
 ```python
 import htmltagparse
 
-#youtube video id
-videoId = ""
-video = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
-
-for i in video.metadata:
-  if i.get("name") == "keywords":
-    tags = i.get("content").split(", ")
-    break
-print(i)
+videoId = "" #video id here
+yt = htmltagparse.build.fromUri("https://www.youtube.com/watch?v=%s" % videoId)
+elTagOpening = yt.find("meta", attrs={"name": "keywords"})[0]
+videoKeywords = htmltagparse.getElementAttributeValue(elTagOpening, "content").split(", ")
+print(videoKeywords) # tags of the youtube video
 ```
 
 ## Developers
 ### Building to Wheel File
 - cd into root directory of this repository
 - run `python3 -m build`
```

### Comparing `htmltagparse-2.0/setup.py` & `htmltagparse-3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     long_description_content_type="text/markdown",
     license=htmltagparse.__license__,
     python_requires=">=3.10",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Topic :: Text Processing :: Markup",
         "Topic :: Text Processing :: Markup :: HTML",
         "Topic :: Utilities",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Intended Audience :: Developers",
     ],
     install_requires=requirements,
```

