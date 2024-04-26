# Comparing `tmp/r_shepard-0.1.0.tar.gz` & `tmp/r_shepard-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r_shepard-0.1.0.tar", max compression
+gzip compressed data, was "r_shepard-0.1.1.tar", max compression
```

## Comparing `r_shepard-0.1.0.tar` & `r_shepard-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2423 2024-04-25 08:53:22.258656 r_shepard-0.1.0/README.md
--rw-r--r--   0        0        0      559 2024-04-25 08:54:49.906130 r_shepard-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      174 2024-04-25 07:52:12.024837 r_shepard-0.1.0/r_shepard/__init__.py
--rw-r--r--   0        0        0      276 2024-04-23 15:09:26.819096 r_shepard-0.1.0/r_shepard/api/admin.py
--rw-r--r--   0        0        0      149 2024-04-23 15:10:07.254460 r_shepard-0.1.0/r_shepard/api/apps.py
--rw-r--r--   0        0        0     1137 2024-04-20 16:40:07.830596 r_shepard-0.1.0/r_shepard/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      442 2024-04-20 17:08:30.708782 r_shepard-0.1.0/r_shepard/api/migrations/0002_project_is_active.py
--rw-r--r--   0        0        0      505 2024-04-20 17:39:58.221267 r_shepard-0.1.0/r_shepard/api/migrations/0003_project_url.py
--rw-r--r--   0        0        0      460 2024-04-20 17:49:45.047866 r_shepard-0.1.0/r_shepard/api/migrations/0004_project_rstudio_version.py
--rw-r--r--   0        0        0     1103 2024-04-21 17:44:57.288648 r_shepard-0.1.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
--rw-r--r--   0        0        0     3210 2024-04-21 18:32:44.456273 r_shepard-0.1.0/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
--rw-r--r--   0        0        0      491 2024-04-22 05:25:57.373534 r_shepard-0.1.0/r_shepard/api/migrations/0007_alter_container_container_id.py
--rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
--rw-r--r--   0        0        0      506 2024-04-22 07:28:12.933948 r_shepard-0.1.0/r_shepard/api/migrations/0009_alter_container_port.py
--rw-r--r--   0        0        0      479 2024-04-22 08:58:14.828153 r_shepard-0.1.0/r_shepard/api/migrations/0010_alter_container_port.py
--rw-r--r--   0        0        0      518 2024-04-22 08:59:48.236196 r_shepard-0.1.0/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
--rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.0/r_shepard/api/migrations/0012_project_slug.py
--rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py
--rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.0/r_shepard/api/migrations/0014_project_max_containers.py
--rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.0/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
--rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
--rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.0/r_shepard/api/migrations/__init__.py
--rw-r--r--   0        0        0     5069 2024-04-25 07:52:12.024837 r_shepard-0.1.0/r_shepard/api/models.py
--rw-r--r--   0        0        0     4346 2024-04-25 07:49:10.152645 r_shepard-0.1.0/r_shepard/api/podman.py
--rw-r--r--   0        0        0     2213 2024-04-25 07:47:41.407870 r_shepard-0.1.0/r_shepard/api/static/custom.css
--rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.0/r_shepard/api/static/htmx.min.js
--rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.0/r_shepard/api/static/pico.blue.min.css
--rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.0/r_shepard/api/static/pico.colors.min.css
--rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.0/r_shepard/api/tailscale.py
--rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.0/r_shepard/api/tasks.py
--rw-r--r--   0        0        0       60 2024-04-20 15:09:46.014593 r_shepard-0.1.0/r_shepard/api/tests.py
--rw-r--r--   0        0        0     5402 2024-04-25 07:51:40.716987 r_shepard-0.1.0/r_shepard/api/views.py
--rw-r--r--   0        0        0      395 2024-04-22 08:52:47.486285 r_shepard-0.1.0/r_shepard/asgi.py
--rw-r--r--   0        0        0      226 2024-04-24 14:31:19.992868 r_shepard-0.1.0/r_shepard/celery.py
--rw-r--r--   0        0        0     4116 2024-04-25 07:52:49.580151 r_shepard-0.1.0/r_shepard/settings.py
--rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.0/r_shepard/urls.py
--rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.0/r_shepard/wsgi.py
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 r_shepard-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2423 2024-04-25 09:13:31.720347 r_shepard-0.1.1/README.md
+-rw-r--r--   0        0        0      576 2024-04-25 09:15:36.828216 r_shepard-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      174 2024-04-25 07:52:12.024837 r_shepard-0.1.1/r_shepard/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-23 15:09:26.819096 r_shepard-0.1.1/r_shepard/api/admin.py
+-rw-r--r--   0        0        0      149 2024-04-23 15:10:07.254460 r_shepard-0.1.1/r_shepard/api/apps.py
+-rw-r--r--   0        0        0     1137 2024-04-20 16:40:07.830596 r_shepard-0.1.1/r_shepard/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      442 2024-04-20 17:08:30.708782 r_shepard-0.1.1/r_shepard/api/migrations/0002_project_is_active.py
+-rw-r--r--   0        0        0      505 2024-04-20 17:39:58.221267 r_shepard-0.1.1/r_shepard/api/migrations/0003_project_url.py
+-rw-r--r--   0        0        0      460 2024-04-20 17:49:45.047866 r_shepard-0.1.1/r_shepard/api/migrations/0004_project_rstudio_version.py
+-rw-r--r--   0        0        0     1103 2024-04-21 17:44:57.288648 r_shepard-0.1.1/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py
+-rw-r--r--   0        0        0     3210 2024-04-21 18:32:44.456273 r_shepard-0.1.1/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py
+-rw-r--r--   0        0        0      491 2024-04-22 05:25:57.373534 r_shepard-0.1.1/r_shepard/api/migrations/0007_alter_container_container_id.py
+-rw-r--r--   0        0        0     1688 2024-04-22 08:54:16.989356 r_shepard-0.1.1/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py
+-rw-r--r--   0        0        0      506 2024-04-22 07:28:12.933948 r_shepard-0.1.1/r_shepard/api/migrations/0009_alter_container_port.py
+-rw-r--r--   0        0        0      479 2024-04-22 08:58:14.828153 r_shepard-0.1.1/r_shepard/api/migrations/0010_alter_container_port.py
+-rw-r--r--   0        0        0      518 2024-04-22 08:59:48.236196 r_shepard-0.1.1/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py
+-rw-r--r--   0        0        0      586 2024-04-23 09:28:07.929488 r_shepard-0.1.1/r_shepard/api/migrations/0012_project_slug.py
+-rw-r--r--   0        0        0      656 2024-04-23 11:30:47.550693 r_shepard-0.1.1/r_shepard/api/migrations/0013_remove_project_password_container_password.py
+-rw-r--r--   0        0        0      541 2024-04-24 10:26:22.152733 r_shepard-0.1.1/r_shepard/api/migrations/0014_project_max_containers.py
+-rw-r--r--   0        0        0      918 2024-04-24 13:21:19.864083 r_shepard-0.1.1/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py
+-rw-r--r--   0        0        0     1381 2024-04-24 13:32:06.450029 r_shepard-0.1.1/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-20 15:09:46.014593 r_shepard-0.1.1/r_shepard/api/migrations/__init__.py
+-rw-r--r--   0        0        0     5069 2024-04-25 07:52:12.024837 r_shepard-0.1.1/r_shepard/api/models.py
+-rw-r--r--   0        0        0     4346 2024-04-25 07:49:10.152645 r_shepard-0.1.1/r_shepard/api/podman.py
+-rw-r--r--   0        0        0     2213 2024-04-25 07:47:41.407870 r_shepard-0.1.1/r_shepard/api/static/custom.css
+-rw-r--r--   0        0        0    48101 2024-04-22 17:57:33.717054 r_shepard-0.1.1/r_shepard/api/static/htmx.min.js
+-rw-r--r--   0        0        0    82210 2024-04-22 16:54:30.950446 r_shepard-0.1.1/r_shepard/api/static/pico.blue.min.css
+-rw-r--r--   0        0        0    74999 2024-04-23 06:39:38.438525 r_shepard-0.1.1/r_shepard/api/static/pico.colors.min.css
+-rw-r--r--   0        0        0     2982 2024-04-23 09:15:45.253107 r_shepard-0.1.1/r_shepard/api/tailscale.py
+-rw-r--r--   0        0        0     1397 2024-04-25 07:52:49.580151 r_shepard-0.1.1/r_shepard/api/tasks.py
+-rw-r--r--   0        0        0       60 2024-04-20 15:09:46.014593 r_shepard-0.1.1/r_shepard/api/tests.py
+-rw-r--r--   0        0        0     5402 2024-04-25 07:51:40.716987 r_shepard-0.1.1/r_shepard/api/views.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:52:47.486285 r_shepard-0.1.1/r_shepard/asgi.py
+-rw-r--r--   0        0        0      226 2024-04-24 14:31:19.992868 r_shepard-0.1.1/r_shepard/celery.py
+-rw-r--r--   0        0        0     4116 2024-04-25 07:52:49.580151 r_shepard-0.1.1/r_shepard/settings.py
+-rw-r--r--   0        0        0     2527 2024-04-23 09:40:06.216686 r_shepard-0.1.1/r_shepard/urls.py
+-rw-r--r--   0        0        0      395 2024-04-22 08:53:11.183304 r_shepard-0.1.1/r_shepard/wsgi.py
+-rw-r--r--   0        0        0     3210 1970-01-01 00:00:00.000000 r_shepard-0.1.1/PKG-INFO
```

### Comparing `r_shepard-0.1.0/README.md` & `r_shepard-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/pyproject.toml` & `r_shepard-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
-name = "r_shepard"
-version = "0.1.0"
+name = "r-shepard"
+version = "0.1.1"
 description = ""
 authors = ["linozen <linus@sehn.dev>"]
 license = "GPL-3.0"
 readme = "README.md"
-packages = [
-    { include = "r_shepard", from = "." }
-]
+packages = [{ include = "r_shepard", from = "." }]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 django = "^5.0.4"
 podman = "^5.0.0"
 django-two-factor-auth = "^1.16.0"
 django-otp-yubikey = "^1.1.0"
 phonenumberslite = "^8.13.35"
 celery = "^5.4.0"
 redis = "^5.0.4"
 
 
 [tool.poetry.group.dev.dependencies]
 djlint = "^1.34.1"
+bumpversion = "^0.6.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0001_initial.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0005_remove_project_url_project_local_url_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0006_remove_project_cpus_remove_project_is_active_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0008_container_port_alter_container_container_id_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0011_alter_container_tailscale_serve_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0012_project_slug.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0012_project_slug.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0013_remove_project_password_container_password.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0013_remove_project_password_container_password.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0014_project_max_containers.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0014_project_max_containers.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0015_project_auto_commit_enabled_project_git_repo_url.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py` & `r_shepard-0.1.1/r_shepard/api/migrations/0016_project_commit_interval_project_last_commit_time_and_more.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/models.py` & `r_shepard-0.1.1/r_shepard/api/models.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/podman.py` & `r_shepard-0.1.1/r_shepard/api/podman.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/static/custom.css` & `r_shepard-0.1.1/r_shepard/api/static/custom.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/static/htmx.min.js` & `r_shepard-0.1.1/r_shepard/api/static/htmx.min.js`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/static/pico.blue.min.css` & `r_shepard-0.1.1/r_shepard/api/static/pico.blue.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/static/pico.colors.min.css` & `r_shepard-0.1.1/r_shepard/api/static/pico.colors.min.css`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/tailscale.py` & `r_shepard-0.1.1/r_shepard/api/tailscale.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/tasks.py` & `r_shepard-0.1.1/r_shepard/api/tasks.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/api/views.py` & `r_shepard-0.1.1/r_shepard/api/views.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/settings.py` & `r_shepard-0.1.1/r_shepard/settings.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/r_shepard/urls.py` & `r_shepard-0.1.1/r_shepard/urls.py`

 * *Files identical despite different names*

### Comparing `r_shepard-0.1.0/PKG-INFO` & `r_shepard-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
-Name: r_shepard
-Version: 0.1.0
+Name: r-shepard
+Version: 0.1.1
 Summary: 
 License: GPL-3.0
 Author: linozen
 Author-email: linus@sehn.dev
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: celery (>=5.4.0,<6.0.0)
 Requires-Dist: django (>=5.0.4,<6.0.0)
 Requires-Dist: django-otp-yubikey (>=1.1.0,<2.0.0)
 Requires-Dist: django-two-factor-auth (>=1.16.0,<2.0.0)
 Requires-Dist: phonenumberslite (>=8.13.35,<9.0.0)
```

