# Comparing `tmp/cofutils-1.1.4.tar.gz` & `tmp/cofutils-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cofutils-1.1.4.tar", last modified: Sat Apr 20 03:26:24 2024, max compression
+gzip compressed data, was "cofutils-1.1.5.tar", last modified: Fri Apr 26 10:46:08 2024, max compression
```

## Comparing `cofutils-1.1.4.tar` & `cofutils-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.202470 cofutils-1.1.4/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-20 03:26:24.198470 cofutils-1.1.4/PKG-INFO
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7542 2024-04-20 03:26:01.000000 cofutils-1.1.4/README.md
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.090469 cofutils-1.1.4/cofutils/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      319 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils/__init__.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7791 2024-04-20 03:26:01.000000 cofutils-1.1.4/cofutils/cofprofiler.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7456 2023-11-25 11:55:29.000000 cofutils-1.1.4/cofutils/cofwriter.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)    16627 2024-04-20 03:26:01.000000 cofutils-1.1.4/cofutils/dispatch.py
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.194470 cofutils-1.1.4/cofutils/parse/
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      657 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/__init__.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      721 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/__main__.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     2191 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/db.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     7151 2023-12-08 07:46:16.000000 cofutils-1.1.4/cofutils/parse/kernel.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7681 2023-12-02 09:09:57.000000 cofutils-1.1.4/cofutils/parse/nsight.py
--rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)    11211 2023-11-30 06:42:14.000000 cofutils-1.1.4/cofutils/parse/nvvp.py
--rwxrwxr-x   0 haiqwa    (1008) haiqwa    (1008)     7669 2023-12-08 08:20:35.000000 cofutils-1.1.4/cofutils/parse/parse.py
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      480 2024-03-05 07:38:00.000000 cofutils-1.1.4/cofutils/torch_version.py
-drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-20 03:26:24.146470 cofutils-1.1.4/cofutils.egg-info/
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/PKG-INFO
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      498 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/SOURCES.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        1 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/dependency_links.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       50 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/entry_points.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       35 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/requires.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        9 2024-04-20 03:26:23.000000 cofutils-1.1.4/cofutils.egg-info/top_level.txt
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       38 2024-04-20 03:26:24.202470 cofutils-1.1.4/setup.cfg
--rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     2286 2024-04-20 03:26:01.000000 cofutils-1.1.4/setup.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-26 10:46:08.426736 cofutils-1.1.5/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-26 10:46:08.426736 cofutils-1.1.5/PKG-INFO
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7542 2024-04-20 03:26:01.000000 cofutils-1.1.5/README.md
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-26 10:46:08.306735 cofutils-1.1.5/cofutils/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      319 2024-04-26 10:46:07.000000 cofutils-1.1.5/cofutils/__init__.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7791 2024-04-20 03:26:01.000000 cofutils-1.1.5/cofutils/cofprofiler.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7456 2023-11-25 11:55:29.000000 cofutils-1.1.5/cofutils/cofwriter.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)    16722 2024-04-26 10:44:01.000000 cofutils-1.1.5/cofutils/dispatch.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-26 10:46:08.418736 cofutils-1.1.5/cofutils/parse/
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      657 2023-11-30 06:42:14.000000 cofutils-1.1.5/cofutils/parse/__init__.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)      721 2023-11-30 06:42:14.000000 cofutils-1.1.5/cofutils/parse/__main__.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     2191 2023-11-30 06:42:14.000000 cofutils-1.1.5/cofutils/parse/db.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)     7151 2023-12-08 07:46:16.000000 cofutils-1.1.5/cofutils/parse/kernel.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7681 2023-12-02 09:09:57.000000 cofutils-1.1.5/cofutils/parse/nsight.py
+-rw-rw-r--   0 haiqwa    (1008) haiqwa    (1008)    11211 2023-11-30 06:42:14.000000 cofutils-1.1.5/cofutils/parse/nvvp.py
+-rwxrwxr-x   0 haiqwa    (1008) haiqwa    (1008)     7669 2023-12-08 08:20:35.000000 cofutils-1.1.5/cofutils/parse/parse.py
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      480 2024-03-05 07:38:00.000000 cofutils-1.1.5/cofutils/torch_version.py
+drwxr-xr-x   0 haiqwa    (1008) haiqwa    (1008)        0 2024-04-26 10:46:08.358736 cofutils-1.1.5/cofutils.egg-info/
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     7889 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/PKG-INFO
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)      498 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/SOURCES.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        1 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/dependency_links.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       50 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/entry_points.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       54 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/requires.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)        9 2024-04-26 10:46:08.000000 cofutils-1.1.5/cofutils.egg-info/top_level.txt
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)       38 2024-04-26 10:46:08.430736 cofutils-1.1.5/setup.cfg
+-rw-r--r--   0 haiqwa    (1008) haiqwa    (1008)     2286 2024-04-26 10:45:44.000000 cofutils-1.1.5/setup.py
```

### Comparing `cofutils-1.1.4/PKG-INFO` & `cofutils-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofutils
-Version: 1.1.4
+Version: 1.1.5
 Summary: Experiment toolkits
 Home-page: https://gitee.com/haiqwa/cofutils.git
 Author: whq1516@mail.ustc.edu.cn
 Maintainer: whq1516@mail.ustc.edu.cn
 License: See https://gitee.com/haiqwa/cofutils/blob/main/LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cofutils-1.1.4/README.md` & `cofutils-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/cofprofiler.py` & `cofutils-1.1.5/cofutils/cofprofiler.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/cofwriter.py` & `cofutils-1.1.5/cofutils/cofwriter.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/dispatch.py` & `cofutils-1.1.5/cofutils/dispatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                     int_range += list(range(start, end))
                 else:
                     int_range.append(int(integers[0]))
             return int_range
         candidate_config_file_list = [config_file_list[each] for each in parse_str_range(GLOBAL_ARGS.range)] if GLOBAL_ARGS.range is not None else config_file_list
         GLOBAL_ARGS.config_file_list=candidate_config_file_list
         GLOBAL_ARGS.log_file_list=[]
-        GLOBAL_ARGS.total_time=0
+        
         for idx, config_file in enumerate(candidate_config_file_list):
             logging(f"{idx+1}/{len(candidate_config_file_list)} executing: {config_file}")
             GLOBAL_ARGS.config_file = config_file
             process_file()
             logging(f"estimated remaining time: {GLOBAL_ARGS.total_time/(idx+1)*(len(candidate_config_file_list)-idx-1)}s")
 
 def task_setup():
@@ -275,14 +275,16 @@
             process_batched_files()
         else:
             GLOBAL_ARGS.config_file = GLOBAL_ARGS.file
             process_file()
 
 def summary():
     global GLOBAL_ARGS
+    if GLOBAL_ARGS.summary is None:
+        return
     if not (hasattr(GLOBAL_ARGS, 'config_file_list') and hasattr(GLOBAL_ARGS, 'log_file_list')):
         sub_dir_list = sorted([each for each in os.listdir(GLOBAL_ARGS.summary) if os.path.isdir(os.path.join(GLOBAL_ARGS.summary,each))])
         GLOBAL_ARGS.config_file_list = [os.path.join(GLOBAL_ARGS.summary, sub_dir, 'config.json') for sub_dir in sub_dir_list]
         GLOBAL_ARGS.log_file_list = [os.path.join(GLOBAL_ARGS.summary, sub_dir, 'log') for sub_dir in sub_dir_list]
     logging(f"tasks summary: cofrun executes {len(GLOBAL_ARGS.config_file_list)} tasks and generate {len(GLOBAL_ARGS.log_file_list)} logs at all")
     if len(GLOBAL_ARGS.config_file_list)!=len(GLOBAL_ARGS.log_file_list) or len(GLOBAL_ARGS.log_file_list)==0:
         print("some tasks did not generate log files properly, skipping summary!")
@@ -293,15 +295,15 @@
         for file in file_paths:
             with open(file, 'r') as fp:
                 log_data = fp.read()
             pattern = r' iteration        \d+/       \d+ \| .*throughput per GPU \(TFLOP/s/GPU\): (\d+\.\d+|\d+) \|.*'
             matches = re.findall(pattern, log_data)
             # print(matches)
             throughput_value_list.append(0)
-            if matches:
+            if len(matches)>1:
                 throughput_value_list[-1]=float(matches[-1])
         return throughput_value_list
     
     def process_json_files(file_paths):
         json_file_table = defaultdict(list)
         same_value = dict()
         diff_value = dict()
@@ -316,15 +318,15 @@
             if len(set(v))==1:
                 same_value[k]=v[0]
             else:
                 diff_value[k]=v
         return same_value, diff_value
     same_value, diff_value = process_json_files(GLOBAL_ARGS.config_file_list)
     diff_value['throughput per GPU (TFLOP/s/GPU)']=process_log_files(GLOBAL_ARGS.log_file_list)
-    diff_value['configuration file']=GLOBAL_ARGS.config_file_list
+    diff_value['configuration file']=[os.path.dirname(file) for file in GLOBAL_ARGS.log_file_list]
     
     logging("same parameter:\n"+tabulate([[k,v] for k,v in same_value.items()], headers=["Same Argument", "Value"], tablefmt="rounded_outline"))
     logging("different parameter and result:\n"+tabulate([[value[idx] for value in diff_value.values()] for idx in range(len(GLOBAL_ARGS.config_file_list))], headers=diff_value.keys(), tablefmt="rounded_outline"))
     
     csv_table = cofcsv('summary')
     for idx in range(len(GLOBAL_ARGS.config_file_list)):
         csv_table.write({k:v[idx] for k,v in diff_value.items()})
@@ -345,15 +347,15 @@
     parser.add_argument('--list','-l', action='store_true',
                         help='list id of all input files, only available when input dir is provided')
     parser.add_argument('--range','-r', type=str, default=None,
                         help='support 3 formats: [int | int,int,int... | int-int], and int value must be > 0; for example, --range 0,1-3,6')
     parser.add_argument('--summary','-s', type=str, default=None,
                         help='provide your directory path which contains output files and cofrun would give the experiment summary in csv format')
     GLOBAL_ARGS = parser.parse_args()
-
+    GLOBAL_ARGS.total_time=0
     logging("\n\n\n"+"-"*20+"cofrun begin"+"-"*20)
 
     args_str = "cofrun arguments\n"
     # alignment
     argument_table_data = list()
     for arg in vars(GLOBAL_ARGS):
         argument_table_data.append([arg, getattr(GLOBAL_ARGS, arg)])
```

### Comparing `cofutils-1.1.4/cofutils/parse/__init__.py` & `cofutils-1.1.5/cofutils/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/__main__.py` & `cofutils-1.1.5/cofutils/parse/__main__.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/db.py` & `cofutils-1.1.5/cofutils/parse/db.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/kernel.py` & `cofutils-1.1.5/cofutils/parse/kernel.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/nsight.py` & `cofutils-1.1.5/cofutils/parse/nsight.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/nvvp.py` & `cofutils-1.1.5/cofutils/parse/nvvp.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils/parse/parse.py` & `cofutils-1.1.5/cofutils/parse/parse.py`

 * *Files identical despite different names*

### Comparing `cofutils-1.1.4/cofutils.egg-info/PKG-INFO` & `cofutils-1.1.5/cofutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cofutils
-Version: 1.1.4
+Version: 1.1.5
 Summary: Experiment toolkits
 Home-page: https://gitee.com/haiqwa/cofutils.git
 Author: whq1516@mail.ustc.edu.cn
 Maintainer: whq1516@mail.ustc.edu.cn
 License: See https://gitee.com/haiqwa/cofutils/blob/main/LICENSE
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `cofutils-1.1.4/setup.py` & `cofutils-1.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     return [x.strip() for x in content]
 install_requires = req_file("requirements.txt")
 entry_points = {
     'console_scripts': [
         'cofrun = cofutils.dispatch:main',
     ]
 }
-__version__="1.1.4"
+__version__="1.1.5"
 __contact_names__="whq1516@mail.ustc.edu.cn"
 __url__="https://gitee.com/haiqwa/cofutils.git"
 __keywords__ = 'Python tools'
 __license__ = 'See https://gitee.com/haiqwa/cofutils/blob/main/LICENSE'
 __description__ = 'Experiment toolkits'
 __package_name__ = 'cofutils'
```

