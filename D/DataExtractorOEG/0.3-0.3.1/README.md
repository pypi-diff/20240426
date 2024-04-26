# Comparing `tmp/dataextractoroeg-0.3.tar.gz` & `tmp/dataextractoroeg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\dataextractoroeg-0.3.tar", last modified: Thu Apr 25 13:34:53 2024, max compression
+gzip compressed data, was "dist\dataextractoroeg-0.3.1.tar", last modified: Thu Apr 25 14:20:01 2024, max compression
```

## Comparing `dataextractoroeg-0.3.tar` & `dataextractoroeg-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 13:34:53.641370 dataextractoroeg-0.3/
--rw-rw-rw-   0        0        0       55 2024-04-23 15:14:35.000000 dataextractoroeg-0.3/.gitignore
-drwxrwxrwx   0        0        0        0 2024-04-25 13:34:53.637370 dataextractoroeg-0.3/DataExtractorOEG.egg-info/
--rw-rw-rw-   0        0        0     2401 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-25 13:34:53.000000 dataextractoroeg-0.3/DataExtractorOEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2401 2024-04-25 13:34:53.638369 dataextractoroeg-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2164 2024-04-25 13:30:41.000000 dataextractoroeg-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-25 13:34:53.625769 dataextractoroeg-0.3/doiExtractor/
--rw-rw-rw-   0        0        0       21 2024-04-25 13:33:42.000000 dataextractoroeg-0.3/doiExtractor/__init__.py
--rw-rw-rw-   0        0        0     5989 2024-04-22 09:37:48.000000 dataextractoroeg-0.3/doiExtractor/doiExtractor.py
--rw-rw-rw-   0        0        0     2120 2024-04-25 12:54:18.000000 dataextractoroeg-0.3/doiExtractor/main.py
--rw-rw-rw-   0        0        0     4682 2024-04-25 09:37:12.000000 dataextractoroeg-0.3/doiExtractor/openAlex.py
--rw-rw-rw-   0        0        0       42 2024-04-25 13:34:53.641603 dataextractoroeg-0.3/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-04-25 13:34:22.000000 dataextractoroeg-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 14:20:01.452147 dataextractoroeg-0.3.1/
+-rw-rw-rw-   0        0        0       72 2024-04-25 13:36:35.000000 dataextractoroeg-0.3.1/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-25 14:20:01.448146 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/
+-rw-rw-rw-   0        0        0     2626 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-25 14:20:01.000000 dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-15 10:32:04.000000 dataextractoroeg-0.3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2626 2024-04-25 14:20:01.449147 dataextractoroeg-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2387 2024-04-25 14:13:29.000000 dataextractoroeg-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 14:20:01.445992 dataextractoroeg-0.3.1/doiExtractor/
+-rw-rw-rw-   0        0        0       21 2024-04-25 13:35:45.000000 dataextractoroeg-0.3.1/doiExtractor/__init__.py
+-rw-rw-rw-   0        0        0     5989 2024-04-22 09:37:48.000000 dataextractoroeg-0.3.1/doiExtractor/doiExtractor.py
+-rw-rw-rw-   0        0        0     2146 2024-04-25 14:16:38.000000 dataextractoroeg-0.3.1/doiExtractor/main.py
+-rw-rw-rw-   0        0        0     4682 2024-04-25 09:37:12.000000 dataextractoroeg-0.3.1/doiExtractor/openAlex.py
+-rw-rw-rw-   0        0        0       42 2024-04-25 14:20:01.452147 dataextractoroeg-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      560 2024-04-25 14:17:49.000000 dataextractoroeg-0.3.1/setup.py
```

### Comparing `dataextractoroeg-0.3/DataExtractorOEG.egg-info/PKG-INFO` & `dataextractoroeg-0.3.1/DataExtractorOEG.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3
+Version: 0.3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
 
@@ -68,13 +68,19 @@
 ```source .env/bin/activate``` (Linux) or ```.env\Scripts\activate``` (Windows)
 
 5. Install the package dependencies:
 ```pip install -e .```
 
 ## Usage
 The tool can be used from the command line with the following argument:
-- ```--start``` - To start the doi extraction 
+- ```--start``` - To start the doi extraction
 
 The script will execute and extract DOIs from the specified webpage and then merge them with the ones from ExistingPapers.
 
+Options:
+- ```--url <path>``` - Specify the webpage of the group you want to extract the dois. Default: Ontology Engieniering Group
+- ```--output <path>``` - Specify the path for the output files. Default: Outputs/
+
+
+
 ### Example
 - ```DataExtractorOEG --start```
```

### Comparing `dataextractoroeg-0.3/LICENSE.txt` & `dataextractoroeg-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3/PKG-INFO` & `dataextractoroeg-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataExtractorOEG
-Version: 0.3
+Version: 0.3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: beautifulsoup4
 Requires-Dist: selenium
 Requires-Dist: requests
 Requires-Dist: pandas
 
@@ -68,13 +68,19 @@
 ```source .env/bin/activate``` (Linux) or ```.env\Scripts\activate``` (Windows)
 
 5. Install the package dependencies:
 ```pip install -e .```
 
 ## Usage
 The tool can be used from the command line with the following argument:
-- ```--start``` - To start the doi extraction 
+- ```--start``` - To start the doi extraction
 
 The script will execute and extract DOIs from the specified webpage and then merge them with the ones from ExistingPapers.
 
+Options:
+- ```--url <path>``` - Specify the webpage of the group you want to extract the dois. Default: Ontology Engieniering Group
+- ```--output <path>``` - Specify the path for the output files. Default: Outputs/
+
+
+
 ### Example
 - ```DataExtractorOEG --start```
```

### Comparing `dataextractoroeg-0.3/README.md` & `dataextractoroeg-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -58,13 +58,19 @@
 ```source .env/bin/activate``` (Linux) or ```.env\Scripts\activate``` (Windows)
 
 5. Install the package dependencies:
 ```pip install -e .```
 
 ## Usage
 The tool can be used from the command line with the following argument:
-- ```--start``` - To start the doi extraction 
+- ```--start``` - To start the doi extraction
 
 The script will execute and extract DOIs from the specified webpage and then merge them with the ones from ExistingPapers.
 
+Options:
+- ```--url <path>``` - Specify the webpage of the group you want to extract the dois. Default: Ontology Engieniering Group
+- ```--output <path>``` - Specify the path for the output files. Default: Outputs/
+
+
+
 ### Example
 - ```DataExtractorOEG --start```
```

### Comparing `dataextractoroeg-0.3/doiExtractor/doiExtractor.py` & `dataextractoroeg-0.3.1/doiExtractor/doiExtractor.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3/doiExtractor/main.py` & `dataextractoroeg-0.3.1/doiExtractor/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 logging.basicConfig(level=logging.INFO)
 
 def cli():
     parser = argparse.ArgumentParser(description="DOI Extractor Tool")
     parser.add_argument("--start", action="store_true", help="Start the extraction process")
     parser.add_argument("--url", default="https://portalcientifico.upm.es/es/ipublic/entity/16247", help="URL to extract DOIs from")
-    parser.add_argument("--output", default="Outputs", help="File path for the outputs")
+    parser.add_argument("--output", default="doiExtractor/Outputs", help="File path for the outputs")
     args = parser.parse_args()
 
     if args.start:
         url = args.url + "#14"
         url_docs = args.url
 
         # Files to write the output
         csv_filename = args.output + "/name_doi.csv"
         txt_filename = args.output + "/dois.txt"
 
         # ExistingPapers
-        papers = "ExistingPapers/name_doi_papers.csv"
+        papers = "doiExtractor/ExistingPapers/name_doi_papers.csv"
 
         logging.info("DOI Extractor Tool started")
         logging.info(f"Search in: {url}, Output csv: {csv_filename}, Output txt: {txt_filename}")
 
         # Delete contents of the files if already created
         if os.path.exists(csv_filename):
             open(csv_filename, 'w').close()
```

### Comparing `dataextractoroeg-0.3/doiExtractor/openAlex.py` & `dataextractoroeg-0.3.1/doiExtractor/openAlex.py`

 * *Files identical despite different names*

### Comparing `dataextractoroeg-0.3/setup.py` & `dataextractoroeg-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="DataExtractorOEG",
-    version="0.3",
+    version="0.3.1",
     packages=find_packages(),
     install_requires=[
         "beautifulsoup4",
         "selenium",
         "requests",
         "pandas"
     ],
```

