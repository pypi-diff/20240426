# Comparing `tmp/django_sync_env-0.3.1a4.tar.gz` & `tmp/django_sync_env-0.3.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.1a4.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a5.tar", max compression
```

## Comparing `django_sync_env-0.3.1a4.tar` & `django_sync_env-0.3.1a5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a4/README.md
--rw-r--r--   0        0        0      499 2024-04-26 04:32:43.549072 django_sync_env-0.3.1a4/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a4/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a4/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a4/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a4/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a4/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a4/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a4/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a4/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a4/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a4/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a4/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a4/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a4/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2580 2024-04-26 04:30:31.126411 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-04-26 04:28:57.973219 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a4/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1707 2024-04-26 04:18:27.387772 django_sync_env-0.3.1a4/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a4/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a4/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14753 2024-04-26 04:32:31.944563 django_sync_env-0.3.1a4/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a4/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a5/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 04:39:52.684491 django_sync_env-0.3.1a5/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a5/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a5/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a5/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a5/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a5/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a5/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a5/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a5/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a5/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a5/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a5/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a5/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a5/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2579 2024-04-26 04:39:40.131579 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-04-26 04:28:57.973219 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a5/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1707 2024-04-26 04:39:03.314940 django_sync_env-0.3.1a5/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a5/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a5/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14753 2024-04-26 04:32:31.944563 django_sync_env-0.3.1a5/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a5/PKG-INFO
```

### Comparing `django_sync_env-0.3.1a4/README.md` & `django_sync_env-0.3.1a5/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a5/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a5/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a5/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a5/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a5/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a5/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             default=None,
             dest="compressed",
         ),
     )
 
     def custom_sort(self, item):
         """Custom sort method to return the file list in environment grouped descending order based on date"""
-        date_format = "%x %X"  # aka "%m/%d/%y %H:%M:%S"
+        date_format = settings.DISPLAY_DATE_TIME_FORMAT
         # First, sort by the 'environment' key
         environment_key = item['environment']
         # Second, sort by the 'datetime' key (converted to datetime, as it's a string)
         date_key = datetime.datetime.strptime(item['datetime'], date_format)
         return environment_key, date_key
 
     def handle(self, **options):
```

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a5/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a5/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a5/src/django_sync_env/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 CLEANUP_KEEP_MEDIA = getattr(settings, "SYNC_ENV_CLEANUP_KEEP_MEDIA", CLEANUP_KEEP)
 CLEANUP_KEEP_FILTER = getattr(settings, "SYNC_ENV_CLEANUP_KEEP_FILTER", lambda x: False)
 
 MEDIA_PATH = settings.MEDIA_ROOT
 
 DATE_FORMAT = "%d-%m-%Y-%H%M%S"
 
-DISPLAY_DATE_TIME_FORMAT = "%-d %B %y %X"  # e.g. 4 April 2025 14:46:25
+DISPLAY_DATE_TIME_FORMAT = "%d %B %y %X"  # e.g. 14 April 2025 14:46:25
 
 FILENAME_TEMPLATE = "{projectname}-{environment}-{databasename}-{datetime}.{extension}"
 
 MEDIA_FILENAME_TEMPLATE = "{projectname}-{environment}-media-{datetime}.{extension}"
 
 CONNECTORS = getattr(settings, "SYNC_ENV_CONNECTORS", {})
```

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a5/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a5/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a5/src/django_sync_env/utils.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a4/PKG-INFO` & `django_sync_env-0.3.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.1a4
+Version: 0.3.1a5
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

