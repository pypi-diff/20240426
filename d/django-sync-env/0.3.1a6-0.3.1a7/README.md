# Comparing `tmp/django_sync_env-0.3.1a6.tar.gz` & `tmp/django_sync_env-0.3.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.1a6.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a7.tar", max compression
```

## Comparing `django_sync_env-0.3.1a6.tar` & `django_sync_env-0.3.1a7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a6/README.md
--rw-r--r--   0        0        0      499 2024-04-26 04:55:26.642753 django_sync_env-0.3.1a6/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a6/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a6/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a6/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a6/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a6/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a6/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a6/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a6/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a6/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a6/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a6/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a6/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a6/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2768 2024-04-26 04:55:06.446050 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2649 2024-04-26 04:55:06.450881 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a6/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1707 2024-04-26 04:39:03.314940 django_sync_env-0.3.1a6/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a6/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a6/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14753 2024-04-26 04:32:31.944563 django_sync_env-0.3.1a6/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a6/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a7/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 05:16:45.050653 django_sync_env-0.3.1a7/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a7/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a7/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a7/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a7/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a7/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a7/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a7/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a7/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a7/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a7/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a7/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a7/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a7/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2197 2024-04-26 05:15:12.578222 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2649 2024-04-26 04:55:06.450881 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a7/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1707 2024-04-26 04:39:03.314940 django_sync_env-0.3.1a7/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a7/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a7/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14531 2024-04-26 05:03:51.264854 django_sync_env-0.3.1a7/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a7/PKG-INFO
```

### Comparing `django_sync_env-0.3.1a6/README.md` & `django_sync_env-0.3.1a7/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a7/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a7/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a7/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a7/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a7/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a7/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 from django_sync_env.storage import get_storage
 from django_sync_env.management.commands._base import BaseSyncBackupCommand, make_option, ROW_TEMPLATE
 from django_sync_env import settings
 import logging
 
 
 class Command(BaseSyncBackupCommand):
-    help = "Connect to configured storage endpoints to get a list of database backups"
+    help = "Connect to configured storage endpoints to get a list of media backups"
     logger = logging.getLogger("sync_env")
     storages = []
 
     option_list = (
-        make_option("-d", "--database", help="Filter by database name"),
         make_option(
             "-z",
             "--compressed",
             help="Exclude non-compressed",
             action="store_true",
             default=None,
             dest="compressed",
@@ -40,33 +39,29 @@
         environment_key = item['environment']
         # Second, sort by the 'datetime' key (converted to datetime, as it's a string)
         date_key = datetime.datetime.strptime(item['datetime'], date_format)
         return environment_key, date_key
 
     def handle(self, **options):
         self.quiet = options.get("quiet")
-        self.logger.info("Connecting to configured storage endpoints to get a list of database backups")
-        files_attr = []
+        self.logger.info("Connecting to configured storage endpoints to get a list of media backups")
 
+        files_attr = []
         for env, config in settings.SYNC_ENV_ENVIRONMENTS.items():
-            options.update({"content_type": "db"})
+            options.update({"content_type": "media"})
             storage = get_storage(env, config)
             if not storage:
                 continue
             files_attr += self.get_backups_attrs(storage, options, env)
-            # Sort the list of file dictionaries using the custom_sort function
+            # Sort the list of dictionaries using the custom_sort function
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
-            title = ROW_TEMPLATE.format(
-                name="Name",
-                environment="Environment",
-                datetime="Datetime",
-                content_type="Content Type"
-            )
+            title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
+                                        content_type="Content Type")
             line = '-' * len(title)
             self.stdout.write(line)
             self.stdout.write(title)
             self.stdout.write(line)
 
             for idx, file_attr in enumerate(files_attr):
                 row = ROW_TEMPLATE.format(**file_attr)
```

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,67 +5,52 @@
 from django_sync_env.storage import get_storage
 from django_sync_env.management.commands._base import BaseSyncBackupCommand, make_option, ROW_TEMPLATE
 from django_sync_env import settings
 import logging
 
 
 class Command(BaseSyncBackupCommand):
-    help = "Connect to configured storage endpoints to get a list of media backups"
+    help = "Connect to configured storage endpoints to get a list of database backups"
     logger = logging.getLogger("sync_env")
     storages = []
-
-    option_list = (
-        make_option(
-            "-z",
-            "--compressed",
-            help="Exclude non-compressed",
-            action="store_true",
-            default=None,
-            dest="compressed",
-        ),
-        make_option(
-            "-Z",
-            "--not-compressed",
-            help="Exclude compressed",
-            action="store_false",
-            default=None,
-            dest="compressed",
-        ),
-    )
+    option_list = ()
 
     def custom_sort(self, item):
         """Custom sort method to return the file list in environment grouped descending order based on date"""
         date_format = settings.DISPLAY_DATE_TIME_FORMAT
         # First, sort by the 'environment' key
         environment_key = item['environment']
         # Second, sort by the 'datetime' key (converted to datetime, as it's a string)
         date_key = datetime.datetime.strptime(item['datetime'], date_format)
         return environment_key, date_key
 
     def handle(self, **options):
         self.quiet = options.get("quiet")
-        self.logger.info("Connecting to configured storage endpoints to get a list of media backups")
-
+        self.logger.info("Connecting to configured storage endpoints to get a list of database backups")
         files_attr = []
-        for env, config in settings.SYNC_ENV_ENVIRONMENTS.items():
-            options.update({"content_type": "media"})
+
+        for idx, (env, config) in enumerate(settings.SYNC_ENV_ENVIRONMENTS.items()):
+            options.update({"content_type": "db"})
             storage = get_storage(env, config)
             if not storage:
                 continue
             files_attr += self.get_backups_attrs(storage, options, env)
-            # Sort the list of dictionaries using the custom_sort function
+            # Sort the list of file dictionaries using the custom_sort function
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
             line = '-' * len(title)
             self.stdout.write(line)
             self.stdout.write(title)
             self.stdout.write(line)
 
             for idx, file_attr in enumerate(files_attr):
                 row = ROW_TEMPLATE.format(**file_attr)
                 self.stdout.write(row)
-                line = '-' * len(row)
-                if idx == len(file_attr) - 1:
-                    self.stdout.write(line)
+
+            self.stdout.write('-' * 80)
```

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a7/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a7/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a7/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a7/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a7/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a6/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a7/src/django_sync_env/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,14 @@
 
     :returns: Date part or nothing if not found
     :rtype: ``str`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
     regex = datefmt_to_regex(datefmt)
     search = regex.search(filename)
-    print('DEBUG: filename_to_datestring:filename: ', regex.search(filename)) # <re.Match object; span=(32, 49), match='16-04-2024-144625'>
     if search:
         return search.groups()[0]
 
 
 def filename_to_date(filename, datefmt=None):
     """
     Return a datetime from a file name.
@@ -381,15 +380,14 @@
     :type datefmt: ``str`` or ``NoneType``
 
     :returns: Date guessed or nothing if no date found
     :rtype: ``datetime.datetime`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
     datestring = filename_to_datestring(filename, datefmt)
-    print('DEBUG: filename_to_date:datestring: ', datestring) # 16-04-2024-144625
     if datestring is not None:
         return datetime.strptime(datestring, datefmt)
 
 
 def filename_generate(
         extension,
         database_name="",
```

### Comparing `django_sync_env-0.3.1a6/PKG-INFO` & `django_sync_env-0.3.1a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.1a6
+Version: 0.3.1a7
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

