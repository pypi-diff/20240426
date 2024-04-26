# Comparing `tmp/django_sync_env-0.3.1a2.tar.gz` & `tmp/django_sync_env-0.3.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.1a2.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a3.tar", max compression
```

## Comparing `django_sync_env-0.3.1a2.tar` & `django_sync_env-0.3.1a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a2/README.md
--rw-r--r--   0        0        0      499 2024-04-26 03:25:54.586531 django_sync_env-0.3.1a2/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a2/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a2/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a2/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.3.1a2/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a2/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a2/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a2/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a2/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a2/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a2/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a2/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a2/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a2/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5549 2024-04-26 03:25:34.613321 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2466 2024-04-26 03:16:30.351022 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a2/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.3.1a2/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a2/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a2/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14789 2024-04-26 03:25:50.132834 django_sync_env-0.3.1a2/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a2/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a3/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 04:18:43.888523 django_sync_env-0.3.1a3/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a3/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a3/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a3/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a3/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a3/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a3/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a3/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a3/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a3/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a3/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a3/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a3/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a3/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2504 2024-04-26 04:19:21.347464 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a3/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1707 2024-04-26 04:18:27.387772 django_sync_env-0.3.1a3/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a3/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a3/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14908 2024-04-26 03:34:18.982332 django_sync_env-0.3.1a3/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a3/PKG-INFO
```

### Comparing `django_sync_env-0.3.1a2/README.md` & `django_sync_env-0.3.1a3/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a3/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a3/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a3/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a3/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a3/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a3/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 from optparse import make_option as optparse_make_option
 from shutil import copyfileobj
 import inquirer
 import django
 from django.core.management.base import BaseCommand, CommandError
 
+from django_sync_env import settings
 from django_sync_env import utils
 from django_sync_env.storage import StorageError
 
 ROW_TEMPLATE = "{name:80} {environment:40} {datetime:20}"
 FILTER_KEYS = ("encrypted", "compressed", "content_type", "database")
 USELESS_ARGS = ("callback", "callback_args", "callback_kwargs", "metavar")
 
@@ -134,22 +135,18 @@
 
     def get_backups_attrs(self, storage, options, environment):
         filters = {k: v for k, v in options.items() if k in FILTER_KEYS}
 
         backups = []
         filenames = storage.list_backups(**filters)
         for filename in filenames:
-            print('DEBUG: _base:get_backups_attrs: filename: ', filename)
-            print('DEBUG: _base:get_backups_attrs: utils.filename_to_date(filename): ', utils.filename_to_date(filename))
-            print('DEBUG: _base:get_backups_attrs:datetime: ', utils.filename_to_date(filename).strftime("%x %X"))
-
             backups.append(
                 {
                     "environment": environment,
-                    "datetime": utils.filename_to_date(filename).strftime("%x %X"),
+                    "datetime": utils.filename_to_date(filename).strftime(settings.DISPLAY_DATE_TIME_FORMAT),
                     "name": filename,
                 }
             )
         return backups
 
     def _cleanup_old_backups(self, database=None, environment=None):
         """
```

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,13 +53,17 @@
             if not storage:
                 continue
             files_attr += self.get_backups_attrs(storage, options, env)
             # Sort the list of file dictionaries using the custom_sort function
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
-            title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
-                                        content_type="Content Type")
+            title = ROW_TEMPLATE.format(
+                name="Name",
+                environment="Environment",
+                datetime="Datetime",
+                content_type="Content Type"
+            )
             self.stdout.write(title)
         for file_attr in files_attr:
             row = ROW_TEMPLATE.format(**file_attr)
             self.stdout.write(row)
```

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a3/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a3/src/django_sync_env/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 CLEANUP_KEEP_MEDIA = getattr(settings, "SYNC_ENV_CLEANUP_KEEP_MEDIA", CLEANUP_KEEP)
 CLEANUP_KEEP_FILTER = getattr(settings, "SYNC_ENV_CLEANUP_KEEP_FILTER", lambda x: False)
 
 MEDIA_PATH = settings.MEDIA_ROOT
 
 DATE_FORMAT = "%d-%m-%Y-%H%M%S"
 
+DISPLAY_DATE_TIME_FORMAT = "%-d %B %y %X"  # e.g. 4 April 2025 14:46:25
+
 FILENAME_TEMPLATE = "{projectname}-{environment}-{databasename}-{datetime}.{extension}"
 
 MEDIA_FILENAME_TEMPLATE = "{projectname}-{environment}-media-{datetime}.{extension}"
 
 CONNECTORS = getattr(settings, "SYNC_ENV_CONNECTORS", {})
 
 CUSTOM_CONNECTOR_MAPPING = getattr(settings, "SYNC_ENV_CONNECTOR_MAPPING", {})
```

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a3/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a3/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a2/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a3/src/django_sync_env/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,18 +362,18 @@
     :type datefmt: ``str`` or ``None``
 
     :returns: Date part or nothing if not found
     :rtype: ``str`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
 
-    print('DEBUG: filename_to_datestring:datefmt:', datefmt)
+    print('DEBUG: filename_to_datestring:datefmt:', datefmt)  # %d-%m-%Y-%H%M%S
     regex = datefmt_to_regex(datefmt)
     search = regex.search(filename)
-    print('DEBUG: filename_to_datestring:filename: ', regex.search(filename))
+    print('DEBUG: filename_to_datestring:filename: ', regex.search(filename)) # <re.Match object; span=(32, 49), match='16-04-2024-144625'>
     if search:
         return search.groups()[0]
 
 
 def filename_to_date(filename, datefmt=None):
     """
     Return a datetime from a file name.
@@ -382,17 +382,17 @@
                     if is ``None``
     :type datefmt: ``str`` or ``NoneType``
 
     :returns: Date guessed or nothing if no date found
     :rtype: ``datetime.datetime`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
-    print('DEBUG: filename_to_date:datefmt: ', datefmt)
+    print('DEBUG: filename_to_date:datefmt: ', datefmt) # %d-%m-%Y-%H%M%S
     datestring = filename_to_datestring(filename, datefmt)
-    print('DEBUG: filename_to_date:datestring: ', datestring)
+    print('DEBUG: filename_to_date:datestring: ', datestring) # 16-04-2024-144625
     if datestring is not None:
         return datetime.strptime(datestring, datefmt)
 
 
 def filename_generate(
         extension,
         database_name="",
```

### Comparing `django_sync_env-0.3.1a2/PKG-INFO` & `django_sync_env-0.3.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.1a2
+Version: 0.3.1a3
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

