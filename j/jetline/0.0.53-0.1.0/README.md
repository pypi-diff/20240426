# Comparing `tmp/jetline-0.0.53.tar.gz` & `tmp/jetline-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetline-0.0.53.tar", last modified: Fri Apr 19 11:56:45 2024, max compression
+gzip compressed data, was "jetline-0.1.0.tar", last modified: Fri Apr 26 05:54:25 2024, max compression
```

## Comparing `jetline-0.0.53.tar` & `jetline-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.684975 jetline-0.0.53/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1028 2024-04-19 11:56:45.684744 jetline-0.0.53/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      137 2024-04-19 10:26:37.000000 jetline-0.0.53/README.txt
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.679976 jetline-0.0.53/jetline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/__init__.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.682552 jetline-0.0.53/jetline/commands/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/_helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/analyze_project.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     4145 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/create_pipe.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/info.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/installer.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1210 2024-04-19 11:38:04.000000 jetline-0.0.53/jetline/commands/run_pipeline.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)    13304 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/commands/to_exe.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.682976 jetline-0.0.53/jetline/data/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/data/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/data/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     3242 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/data/helper.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     2743 2024-04-19 11:33:50.000000 jetline-0.0.53/jetline/logging.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.683365 jetline-0.0.53/jetline/pipeline/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/pipeline/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/pipeline/node.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     6038 2024-04-19 11:55:53.000000 jetline-0.0.53/jetline/pipeline/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.684157 jetline-0.0.53/jetline/templates/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/templates/__init__.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      709 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/templates/data.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      664 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/templates/main.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      603 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/templates/nodes.py
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      804 2024-04-19 10:26:39.000000 jetline-0.0.53/jetline/templates/pipeline.py
-drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-19 11:56:45.684484 jetline-0.0.53/jetline.egg-info/
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1028 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/PKG-INFO
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      777 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/SOURCES.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/dependency_links.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/entry_points.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)      109 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/requires.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-19 11:56:45.000000 jetline-0.0.53/jetline.egg-info/top_level.txt
--rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-19 11:56:45.685021 jetline-0.0.53/setup.cfg
--rw-r--r--   0 johanneskanthak   (501) staff       (20)     1626 2024-04-19 11:56:17.000000 jetline-0.0.53/setup.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.493190 jetline-0.1.0/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 05:54:25.492964 jetline-0.1.0/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1103 2024-04-25 16:42:38.000000 jetline-0.1.0/README.md
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.488142 jetline-0.1.0/jetline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/__init__.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.490608 jetline-0.1.0/jetline/commands/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1998 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/_helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    10737 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/analyze_project.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     4145 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/create_pipe.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2086 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/info.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     2866 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/installer.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1106 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/run_pipeline.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)    13304 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/commands/to_exe.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.491045 jetline-0.1.0/jetline/data/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/data/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     5221 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/data/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     3222 2024-04-26 05:41:26.000000 jetline-0.1.0/jetline/data/helper.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      127 2024-04-26 05:52:47.000000 jetline-0.1.0/jetline/logging.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.491530 jetline-0.1.0/jetline/pipeline/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/pipeline/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1684 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/pipeline/node.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     6042 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/pipeline/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.492451 jetline-0.1.0/jetline/templates/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        0 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/templates/__init__.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      709 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/templates/data.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      664 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/templates/main.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      603 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/templates/nodes.py
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      804 2024-04-25 16:41:25.000000 jetline-0.1.0/jetline/templates/pipeline.py
+drwxr-xr-x   0 johanneskanthak   (501) staff       (20)        0 2024-04-26 05:54:25.492687 jetline-0.1.0/jetline.egg-info/
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1050 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/PKG-INFO
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      776 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/SOURCES.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        1 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/dependency_links.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      317 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/entry_points.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)      117 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/requires.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)        8 2024-04-26 05:54:25.000000 jetline-0.1.0/jetline.egg-info/top_level.txt
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)       38 2024-04-26 05:54:25.493240 jetline-0.1.0/setup.cfg
+-rw-r--r--   0 johanneskanthak   (501) staff       (20)     1639 2024-04-26 05:54:11.000000 jetline-0.1.0/setup.py
```

### Comparing `jetline-0.0.53/PKG-INFO` & `jetline-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.0.53
+Version: 0.1.0
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,8 @@
 Requires-Dist: click==8.1.7
 Requires-Dist: colorama==0.4.6
 Requires-Dist: toml==0.10.2
 Requires-Dist: pandas==2.2.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: fastapi==0.110.0
+Requires-Dist: vulture
```

### Comparing `jetline-0.0.53/jetline/commands/_helper.py` & `jetline-0.1.0/jetline/commands/_helper.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/commands/analyze_project.py` & `jetline-0.1.0/jetline/commands/analyze_project.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/commands/create_pipe.py` & `jetline-0.1.0/jetline/commands/create_pipe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/commands/info.py` & `jetline-0.1.0/jetline/commands/info.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/commands/installer.py` & `jetline-0.1.0/jetline/commands/installer.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/commands/run_pipeline.py` & `jetline-0.1.0/jetline/commands/run_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 import click
 import os
-import sys
 
-python_cmd = 'python'
-if sys.version_info >= (3, 0):
-    python_cmd = 'python3'
 @click.command()
 @click.argument('pipeline_name', default=None, required=False)
 def main(pipeline_name):
     """
      Run a pipeline or all pipelines if pipeline_name is None. This is a command line tool to run a pipeline or all pipelines in the current directory.
      
      Args:
@@ -17,16 +13,16 @@
     main_file = "main.py"
     current_directory = os.getcwd()
     main_path = os.path.join(current_directory, main_file)
 
     if os.path.isfile(main_path):
         if pipeline_name is not None:
             click.secho(f"Directory successfully located. Running pipeline(s) '{pipeline_name}'...", fg='green')
-            os.system(f'{python_cmd} -c "from main import run_pipelines; run_pipelines(\'{pipeline_name}\')"')
+            os.system(f'python -c "from main import run_pipelines; run_pipelines(\'{pipeline_name}\')"')
         else:
             click.secho("Directory successfully located. Running Pipelines...", fg='green')
-            os.system(f'{python_cmd} -c "from main import run_pipelines; run_pipelines()"')
+            os.system('python -c "from main import run_pipelines; run_pipelines()"')
     else:
         click.secho(f"{main_file} not found in the current directory.", fg='red')
 
 if __name__ == "__main__":
     main()
```

### Comparing `jetline-0.0.53/jetline/commands/to_exe.py` & `jetline-0.1.0/jetline/commands/to_exe.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/data/data.py` & `jetline-0.1.0/jetline/data/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/data/helper.py` & `jetline-0.1.0/jetline/data/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import tkinter as tk
 from tkinter import filedialog
 import pandas as pd
+import os
 
 
 def choose_file():
     """
     This method opens a file dialog window to allow the user to choose a file on their system. It returns the path of the selected file.
     """
     root = tk.Tk()
     root.withdraw()
     file_path = filedialog.askopenfilename()
     return file_path
-import os
-import pandas as pd
 
 
 def load_file_to_dataframe(file_path, delimiter=';'):
     """
     Loads a file from the given file_path and loads it into a pandas dataframe
     """
     if not file_path:
```

### Comparing `jetline-0.0.53/jetline/pipeline/node.py` & `jetline-0.1.0/jetline/pipeline/node.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/pipeline/pipeline.py` & `jetline-0.1.0/jetline/pipeline/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self.caller_path = self.get_caller_path()
         self.add_project_directory_to_sys_path()
         self.data_manager = DataManager(caller_path=self.caller_path)
         self.pipelines = {}
         self.load_pipelines()
 
     @staticmethod
-    def get_caller_path():
+    def get_caller_path(self):
         """
         Description:
         This method returns the path of the file that called it.
 
         Parameters:
         - self: The instance of the calling class. This is an implicit parameter and does not need to be provided explicitly.
```

### Comparing `jetline-0.0.53/jetline/templates/data.py` & `jetline-0.1.0/jetline/templates/data.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/templates/main.py` & `jetline-0.1.0/jetline/templates/main.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/templates/nodes.py` & `jetline-0.1.0/jetline/templates/nodes.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline/templates/pipeline.py` & `jetline-0.1.0/jetline/templates/pipeline.py`

 * *Files identical despite different names*

### Comparing `jetline-0.0.53/jetline.egg-info/PKG-INFO` & `jetline-0.1.0/jetline.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetline
-Version: 0.0.53
+Version: 0.1.0
 Summary: Automated Pipeline Builder
 Home-page: https://github.com/your_username/jetline
 Author: Johannes Kanthak
 Author-email: johannes.kanthak@kdc-solutions.de
 License: MIT
 Keywords: pipeline automation
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,8 @@
 Requires-Dist: click==8.1.7
 Requires-Dist: colorama==0.4.6
 Requires-Dist: toml==0.10.2
 Requires-Dist: pandas==2.2.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: coloredlogs==15.0.1
 Requires-Dist: fastapi==0.110.0
+Requires-Dist: vulture
```

### Comparing `jetline-0.0.53/jetline.egg-info/SOURCES.txt` & `jetline-0.1.0/jetline.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-README.txt
+README.md
 setup.py
 jetline/__init__.py
 jetline/logging.py
 jetline.egg-info/PKG-INFO
 jetline.egg-info/SOURCES.txt
 jetline.egg-info/dependency_links.txt
 jetline.egg-info/entry_points.txt
```

### Comparing `jetline-0.0.53/setup.py` & `jetline-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,22 @@
     'click==8.1.7',
     'colorama==0.4.6',
     'toml==0.10.2',
     'pandas==2.2.0',
     'openpyxl==3.1.2',
     'coloredlogs==15.0.1',
     'fastapi==0.110.0',
+    'vulture'
     
 
 ]
 
 setup(
     name='jetline',
-    version='0.0.53',
+    version='0.1.0',
     description='Automated Pipeline Builder',
     url='https://github.com/your_username/jetline',
     author='Johannes Kanthak',
     author_email='johannes.kanthak@kdc-solutions.de',
     license='MIT',
     classifiers=classifiers,
     keywords='pipeline automation',
```

