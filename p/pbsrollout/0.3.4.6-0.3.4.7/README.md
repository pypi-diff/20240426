# Comparing `tmp/pbsrollout-0.3.4.6.tar.gz` & `tmp/pbsrollout-0.3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.4.6.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.4.7.tar", max compression
```

## Comparing `pbsrollout-0.3.4.6.tar` & `pbsrollout-0.3.4.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.4.6/LICENSE
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.4.6/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.4.6/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.4.6/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.4.6/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.4.6/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.4.6/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.4.6/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1316 2024-02-23 16:37:00.272734 pbsrollout-0.3.4.6/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.4.6/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.4.6/pbsrollout/internal/test_utils.py
--rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.4.6/pbsrollout/internal/test_utils_gh.py
--rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.4.6/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     2966 2024-02-23 16:37:00.274265 pbsrollout-0.3.4.6/pbsrollout/internal/utils_gh.py
--rw-r--r--   0        0        0     6532 2024-03-06 20:14:46.534649 pbsrollout-0.3.4.6/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.4.6/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9973 2024-02-23 16:37:00.276000 pbsrollout-0.3.4.6/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.4.6/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     7281 2024-02-23 16:37:00.276748 pbsrollout-0.3.4.6/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.4.6/pbsrollout/test_main.py
--rw-r--r--   0        0        0      585 2024-03-06 20:13:56.793912 pbsrollout-0.3.4.6/pyproject.toml
--rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.269208 pbsrollout-0.3.4.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271482 pbsrollout-0.3.4.7/pbsrollout/__init__.py
+-rw-r--r--   0        0        0       48 2024-04-26 16:50:25.049516 pbsrollout-0.3.4.7/pbsrollout/config/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.271688 pbsrollout-0.3.4.7/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1226 2024-02-23 16:37:00.271816 pbsrollout-0.3.4.7/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2024-02-23 16:37:00.271939 pbsrollout-0.3.4.7/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3955 2024-02-23 16:37:00.272073 pbsrollout-0.3.4.7/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0    11453 2024-02-23 16:37:00.272228 pbsrollout-0.3.4.7/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2024-02-23 16:37:00.272403 pbsrollout-0.3.4.7/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1344 2024-04-26 16:50:20.323610 pbsrollout-0.3.4.7/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      443 2024-02-23 16:37:00.273014 pbsrollout-0.3.4.7/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      151 2024-02-23 16:37:00.273172 pbsrollout-0.3.4.7/pbsrollout/internal/test_utils.py
+-rw-r--r--   0        0        0     1076 2024-02-23 16:37:00.273488 pbsrollout-0.3.4.7/pbsrollout/internal/test_utils_gh.py
+-rw-r--r--   0        0        0     1159 2024-02-23 16:37:00.274011 pbsrollout-0.3.4.7/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     2958 2024-04-25 22:53:25.462662 pbsrollout-0.3.4.7/pbsrollout/internal/utils_gh.py
+-rw-r--r--   0        0        0     6571 2024-04-26 16:50:46.668815 pbsrollout-0.3.4.7/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.275238 pbsrollout-0.3.4.7/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0    10013 2024-04-26 16:51:05.778066 pbsrollout-0.3.4.7/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2024-02-23 16:37:00.276397 pbsrollout-0.3.4.7/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-26 16:51:36.835899 pbsrollout-0.3.4.7/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      225 2024-02-23 16:37:00.277701 pbsrollout-0.3.4.7/pbsrollout/test_main.py
+-rw-r--r--   0        0        0      585 2024-04-26 16:51:57.664991 pbsrollout-0.3.4.7/pyproject.toml
+-rw-r--r--   0        0        0      763 1970-01-01 00:00:00.000000 pbsrollout-0.3.4.7/PKG-INFO
```

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/test_k8s_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 from unittest import TestCase
 
 from kubernetes import config
 
 from pbsrollout.internal.k8s_utils import import_kube_config, get_pods_for_daemonsets, get_all_pbs_daemonset, get_services
+from pbsrollout.config import REPOSITORY_NAME
 
 
 class Test(TestCase):
     def test_get_pods_for_daemonset(self):
-        path = os.environ['GOPATH'] + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.eu-west-1-eks-16-v3'
+        path = os.environ['GOPATH'] + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.eu-west-1-eks-16-v3'
         api_client = config.new_client_from_config(config_file=import_kube_config(path + '/.k8s-assets/kubeconfig'))
 
         pods = get_pods_for_daemonsets(api_client, [802, 803])
         print(pods)
 
     def test_get_all_pbs_daemonset(self):
-        path = os.environ['GOPATH'] + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.us-east-1-eks-23-v3'
+        path = os.environ['GOPATH'] + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-23-v3'
         api_client = config.new_client_from_config(config_file=import_kube_config(path + '/.k8s-assets/kubeconfig'))
 
         pbs_daemonsets = get_all_pbs_daemonset(api_client, True)
         names = [d.metadata.name for d in pbs_daemonsets]
         print(names)
 
     def test_get_services(self):
-        path = os.environ['GOPATH'] + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.eu-west-1-eks-16-v3'
+        path = os.environ['GOPATH'] + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.eu-west-1-eks-16-v3'
         api_client = config.new_client_from_config(config_file=import_kube_config(path + '/.k8s-assets/kubeconfig'))
 
         get_services(api_client, 'pbs-prod')
```

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/test_utils_gh.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/test_utils_gh.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/utils.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.4.6/pbsrollout/internal/utils_gh.py` & `pbsrollout-0.3.4.7/pbsrollout/internal/utils_gh.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             if name in gh_handle_to_name:
                 return gh_handle_to_name[name]
             return name
         except:
             return '?'
 
     if isinstance(hash, str):
-        cmd = f"gh pr list -S {hash} --repo publica-project/platform --json author,title"
+        cmd = f"gh pr list -S {hash} --repo integralads/platform --json author,title"
     else:
-        cmd = 'gh pr list --repo=publica-project/platform --json=author,commits,title --search="sort:updated-desc" --limit=20'
+        cmd = 'gh pr list --repo=integralads/platform --json=author,commits,title --search="sort:updated-desc" --limit=20'
 
     ret = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, timeout=10, shell=True)
     ret.stderr = clean_stderr(ret.stderr)
     if ret.returncode != 0 or ret.stderr != "":
         print_error_body(f"ERROR:\n\ncmd:\n{cmd}\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
         return []
```

### Comparing `pbsrollout-0.3.4.6/pbsrollout/main.py` & `pbsrollout-0.3.4.7/pbsrollout/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import List
 
 from botocore.exceptions import ClientError
 from kubernetes.client import ApiException
 from rich.console import Console
 from simple_term_menu import TerminalMenu
 
+from pbsrollout.config import REPOSITORY_NAME
 from pbsrollout.internal.utils import notify, get_latest_version, is_dev
 
 VERSION = ""
 try:
     import importlib.metadata
 
     VERSION = importlib.metadata.version("pbsrollout")
@@ -160,15 +161,15 @@
             console.print("[bold red]\nerror: please run `zaws_ctv_engineer` to login")
             return 1
         elif isinstance(e, RuntimeError):
             console.print(f"[bold red]\nError: {e}")
         elif isinstance(e, TimeoutExpired):
             console.print(f"[bold red]\nerror: {e}")
         elif isinstance(e, UnicodeDecodeError) and 'codec can\'t decode byte' in e.reason:
-            console.print(f"\nerror: {e}\n\n[bold red] You might want to run `git-crypt unlock` in the `pb-prebid-kube-manifests` repository\nit should fix this issue. Otherwise please send this to Dimitri Wyzlic on Slack!")
+            console.print(f"\nerror: {e}\n\n[bold red] You might want to run `git-crypt unlock` in the `{REPOSITORY_NAME}` repository\nit should fix this issue. Otherwise please send this to Dimitri Wyzlic on Slack!")
         else:
             console.print_exception()
             console.print('[orange3]please send this to Dimitri Wyzlic on Slack!')
             return 1
     except KeyboardInterrupt:
         console.print("\n\n[bold red]Interrupted by user (CTRL-C)")
     return 0
```

### Comparing `pbsrollout-0.3.4.6/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.4.7/pbsrollout/pbs_release/main_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from kubernetes.client import ApiException, ApiClient
 from rich.columns import Columns
 from rich.console import Console
 from rich.markdown import Markdown
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
+from pbsrollout.config import REPOSITORY_NAME
 from pbsrollout.internal.check_cluster_ready import check_cluster_ready
 from pbsrollout.internal.k8s_utils import import_kube_config
 from pbsrollout.internal.process_cluster import cutover_service, launch_pods, remove_old_pods, Status
 from pbsrollout.internal.utils import notify
 
 CLUSTERS = [
     "aws.us-east-1-eks-23-v3",
@@ -160,15 +161,15 @@
     #  - plz git pull
     if not no_interaction:
         console.print(
             "[bold red]Please run[/bold red] [italic misty_rose1]git pull --rebase[italic misty_rose1] [bold red]before running this script![/bold red]")
         ask_if_git_pull()
 
     # 1. CD Inside the prebid kube manifest directory
-    prebid_k8s_path = gopath + '/src/github.com/integralads/pb-prebid-kube-manifests'
+    prebid_k8s_path = gopath + f'/src/github.com/integralads/{REPOSITORY_NAME}'
     with Dir(prebid_k8s_path):
         console.print("\n\n[bold]Step 1: updating prebid tag")
         tag = tag_from_args if tag_from_args != "" else ask_for_tag()
         if tag == "":
             print("error: tag must not be empty")
             return
```

### Comparing `pbsrollout-0.3.4.6/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.4.7/pbsrollout/stg_release/main_view.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from copy import copy
 from typing import Tuple, Callable, List, Any
 
 from rich.console import Console
 from shellpython.helpers import Dir
 from simple_term_menu import TerminalMenu
 
+from pbsrollout.config import REPOSITORY_NAME
 from pbsrollout.internal.aws_utils import get_ecr_images
 from pbsrollout.internal.utils import clean_stderr, print_error_body
 from pbsrollout.internal.utils_gh import get_pr_titles_and_author_from_commit_hash, does_gh_cli_exist
 
 NB_STAGINGS = 20
 
 def get_and_enforce_go_path(console: Console) -> str:
@@ -91,51 +92,51 @@
     else:
         for f in full_img:
             if f.endswith(tag[:len('cd1ef6b73')]):
                 tag = f
                 break
 
     # put it in the file
-    dir_path = go_path + '/src/github.com/integralads/pb-prebid-kube-manifests/namespace/stg/'
+    dir_path = go_path + f'/src/github.com/integralads{REPOSITORY_NAME}/namespace/stg/'
     for stg in stg_idx:
         console.print(f"Updating tag to [bold blue_violet]{tag}[/bold blue_violet] in file:")
         for pod in ['pbs', 'logger', 'console-api']:
             tag_file_path = dir_path + f"z{stg}-{pod}.tag"
             console.print(f"[bold light_steel_blue1]{tag_file_path}[/bold light_steel_blue1]")
             with open(tag_file_path, "w") as f:
                 f.write(tag)
 
     # step 2: release pods
     for stg in stg_idx:
         launch_staging_pod(stg,
-                           go_path + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.us-east-1-eks-27-v3/')
+                           go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/')
         console.print('\t[bold green]success!')
 
 
 def exit_fn(console: Console, stg_idx: List[str], go_path: str):
     return
 
 
 def migrate_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
-        dir_path = go_path + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.us-east-1-eks-27-v3/'
+        dir_path = go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tMigrating staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/migrate-staging-db {stg.lstrip('0')}"
             ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
                 print_error_body(f"ERROR:\n\nstdout:\n{ret.stdout}\nstderr:\n{ret.stderr}")
                 return False
 
 
 def sync_staging_db(console: Console, stg_idx: List[str], go_path: str):
     for stg in stg_idx:
-        dir_path = go_path + '/src/github.com/integralads/pb-prebid-kube-manifests/aws.us-east-1-eks-27-v3/'
+        dir_path = go_path + f'/src/github.com/integralads/{REPOSITORY_NAME}/aws.us-east-1-eks-27-v3/'
         with Dir(dir_path):
             print(f'\tSyncing staging db for stg: {stg}')
             # run make clean deploy-new-pbs-prod
             cmd = f"direnv exec . ../scripts/sync-staging-db {stg.lstrip('0')}"
             ret = subprocess.run(cmd.split(" "), stderr=subprocess.PIPE, text=True, timeout=200)
             ret.stderr = clean_stderr(ret.stderr)
             if ret.returncode != 0 or ret.stderr != "":
```

### Comparing `pbsrollout-0.3.4.6/pyproject.toml` & `pbsrollout-0.3.4.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.4.6"
+version = "0.3.4.7"
 description = "A tool to help Publica engineer test and release the platform"
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.4.6/PKG-INFO` & `pbsrollout-0.3.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.4.6
+Version: 0.3.4.7
 Summary: A tool to help Publica engineer test and release the platform
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

