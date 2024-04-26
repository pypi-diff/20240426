# Comparing `tmp/pbsrollout-0.3.4.7.tar.gz` & `tmp/pbsrollout-0.3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.4.7.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.4.8.tar", max compression
```

## Comparing `pbsrollout-0.3.4.7.tar` & `pbsrollout-0.3.4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.4.7/LICENSE
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.4.7/pbsrollout/__init__.py
--rw-r--r--   0        0        0       48 2024-04-26 16:50:25.049516 pbsrollout-0.3.4.7/pbsrollout/config/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.4.7/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.4.7/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.4.7/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.4.7/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.4.7/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.4.7/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1344 2024-04-26 16:50:20.323610 pbsrollout-0.3.4.7/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.4.7/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.4.7/pbsrollout/internal/test_utils.py
--rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.4.7/pbsrollout/internal/test_utils_gh.py
--rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.4.7/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     2958 2024-04-25 22:53:25.462662 pbsrollout-0.3.4.7/pbsrollout/internal/utils_gh.py
--rw-r--r--   0        0        0     6571 2024-04-26 16:50:46.668815 pbsrollout-0.3.4.7/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.4.7/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0    10013 2024-04-26 16:51:05.778066 pbsrollout-0.3.4.7/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.4.7/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     7302 2024-04-26 16:51:36.835899 pbsrollout-0.3.4.7/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.4.7/pbsrollout/test_main.py
--rw-r--r--   0        0        0      585 2024-04-26 16:51:57.664991 pbsrollout-0.3.4.7/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.4.8/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.4.8/pbsrollout/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-26 16:50:25.049516 pbsrollout-0.3.4.8/pbsrollout/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.4.8/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.4.8/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.4.8/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.4.8/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.4.8/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.4.8/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1344 2024-04-26 16:50:20.323610 pbsrollout-0.3.4.8/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.4.8/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.4.8/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.4.8/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.4.8/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2958 2024-04-25 22:53:25.462662 pbsrollout-0.3.4.8/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     6571 2024-04-26 16:50:46.668815 pbsrollout-0.3.4.8/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.4.8/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0    10013 2024-04-26 16:51:05.778066 pbsrollout-0.3.4.8/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.4.8/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     7410 2024-04-26 18:13:16.165122 pbsrollout-0.3.4.8/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.4.8/pbsrollout/test_main.py
+-rw-r--r--   0        0        0      585 2024-04-26 18:13:28.987578 pbsrollout-0.3.4.8/pyproject.toml
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.8/PKG-INFO
```

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/test_utils_gh.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/test_utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/utils.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/internal/utils_gh.py` & `pbsrollout-0.3.4.8/pbsrollout/internal/utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/main.py` & `pbsrollout-0.3.4.8/pbsrollout/main.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.4.8/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.7/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.4.8/pbsrollout/stg_release/main_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,52 +52,54 @@
     # step 1: choose and write tags for .tag files
     # load tags
 
     gh_cli_exist = does_gh_cli_exist()
     if not gh_cli_exist:
         console.print('[bold gold1]you should install the gh cli to add more informations about the tags!\n[italic]brew install gh[/italic][/bold gold1]')
 
-    with console.status("[bold green]Fetching tags for 'pbs'...") as status:
-        images = get_ecr_images('pbs')
-        full_img = copy(images)
-        images = [x[17:] for x in images]
+    tag = 'manual input'
 
-        # enrich tags with github data
-
-        # let's only display tags with open PR!
-        github_infos = []
-        if gh_cli_exist:
-            status.update("[bold green]Fetching github description for those tags...")
-            github_infos = get_pr_titles_and_author_from_commit_hash(images)
-            biggest_name_len = 0
-            for g in github_infos:
-                biggest_name_len = max(biggest_name_len, len(g[0]))
-
-            enriched_data = []
-            for g in github_infos:
-                for idx, tag in enumerate(images):
-                    if g[2] == tag:
-                        enriched_data.append(f'{tag}  {g[0].ljust(biggest_name_len + 4)} {g[1]}')
-            if len(enriched_data) > 0:
-                images = enriched_data
-
-    # choose image
-    images.append("manual input")
-    terminal_menu = TerminalMenu(images, title="Select tag:",
-                                 raise_error_on_interrupt=True)
-    menu_entry_index = terminal_menu.show()
-    tag = images[menu_entry_index]
+    # with console.status("[bold green]Fetching tags for 'pbs'...") as status:
+    #     images = get_ecr_images('pbs')
+    #     full_img = copy(images)
+    #     images = [x[17:] for x in images]
+    #
+    #     # enrich tags with github data
+    #
+    #     # let's only display tags with open PR!
+    #     github_infos = []
+    #     if gh_cli_exist:
+    #         status.update("[bold green]Fetching github description for those tags...")
+    #         github_infos = get_pr_titles_and_author_from_commit_hash(images)
+    #         biggest_name_len = 0
+    #         for g in github_infos:
+    #             biggest_name_len = max(biggest_name_len, len(g[0]))
+    #
+    #         enriched_data = []
+    #         for g in github_infos:
+    #             for idx, tag in enumerate(images):
+    #                 if g[2] == tag:
+    #                     enriched_data.append(f'{tag}  {g[0].ljust(biggest_name_len + 4)} {g[1]}')
+    #         if len(enriched_data) > 0:
+    #             images = enriched_data
+    #
+    # # choose image
+    # images.append("manual input")
+    # terminal_menu = TerminalMenu(images, title="Select tag:",
+    #                              raise_error_on_interrupt=True)
+    # menu_entry_index = terminal_menu.show()
+    # tag = images[menu_entry_index]
 
     if tag == 'manual input':
         tag = str(input('enter your image tag: '))
-    else:
-        for f in full_img:
-            if f.endswith(tag[:len('cd1ef6b73')]):
-                tag = f
-                break
+    # else:
+    #     for f in full_img:
+    #         if f.endswith(tag[:len('cd1ef6b73')]):
+    #             tag = f
+    #             break
 
     # put it in the file
     dir_path = go_path + f'/src/github.com/integralads{REPOSITORY_NAME}/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
         for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
```

### Comparing `pbsrollout-0.3.4.7/pyproject.toml` & `pbsrollout-0.3.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.4.7"
+version = "0.3.4.8"
 description = "A tool to help Publica engineer test and release the platform"
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.4.7/PKG-INFO` & `pbsrollout-0.3.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.4.7
+Version: 0.3.4.8
 Summary: A tool to help Publica engineer test and release the platform
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

