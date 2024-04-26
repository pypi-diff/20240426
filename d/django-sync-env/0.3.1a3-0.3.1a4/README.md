# Comparing `tmp/django_sync_env-0.3.1a3.tar.gz` & `tmp/django_sync_env-0.3.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.1a3.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a4.tar", max compression
```

## Comparing `django_sync_env-0.3.1a3.tar` & `django_sync_env-0.3.1a4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a3/README.md
--rw-r--r--   0        0        0      499 2024-04-26 04:18:43.888523 django_sync_env-0.3.1a3/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a3/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a3/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a3/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a3/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a3/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a3/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a3/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a3/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a3/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a3/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a3/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a3/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a3/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2504 2024-04-26 04:19:21.347464 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a3/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1707 2024-04-26 04:18:27.387772 django_sync_env-0.3.1a3/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a3/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a3/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14908 2024-04-26 03:34:18.982332 django_sync_env-0.3.1a3/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a3/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a4/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 04:32:43.549072 django_sync_env-0.3.1a4/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a4/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a4/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a4/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      193 2024-04-26 04:15:15.623564 django_sync_env-0.3.1a4/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a4/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a4/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a4/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a4/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a4/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a4/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a4/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a4/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a4/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5300 2024-04-26 04:18:06.104874 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2580 2024-04-26 04:30:31.126411 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-04-26 04:28:57.973219 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a4/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1707 2024-04-26 04:18:27.387772 django_sync_env-0.3.1a4/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a4/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a4/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14753 2024-04-26 04:32:31.944563 django_sync_env-0.3.1a4/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a4/PKG-INFO
```

### Comparing `django_sync_env-0.3.1a3/README.md` & `django_sync_env-0.3.1a4/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a4/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a4/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a4/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a4/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a4/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a4/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,21 @@
             storage = get_storage(env, config)
             if not storage:
                 continue
             files_attr += self.get_backups_attrs(storage, options, env)
             # Sort the list of file dictionaries using the custom_sort function
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
-        if not self.quiet:
-            title = ROW_TEMPLATE.format(
-                name="Name",
-                environment="Environment",
-                datetime="Datetime",
-                content_type="Content Type"
-            )
-            self.stdout.write(title)
-        for file_attr in files_attr:
-            row = ROW_TEMPLATE.format(**file_attr)
-            self.stdout.write(row)
+            print(files_attr)
+
+            if not self.quiet:
+                title = ROW_TEMPLATE.format(
+                    name="Name",
+                    environment="Environment",
+                    datetime="Datetime",
+                    content_type="Content Type"
+                )
+                self.stdout.write(title)
+
+            for file_attr in files_attr:
+                row = ROW_TEMPLATE.format(**file_attr)
+                self.stdout.write(row)
```

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             action="store_false",
             default=None,
             dest="compressed",
         ),
     )
 
     def custom_sort(self, item):
-        """Custom sort method to return the file list in environment grouped descending order baesed on date"""
+        """Custom sort method to return the file list in environment grouped descending order based on date"""
         date_format = "%x %X"  # aka "%m/%d/%y %H:%M:%S"
         # First, sort by the 'environment' key
         environment_key = item['environment']
         # Second, sort by the 'datetime' key (converted to datetime, as it's a string)
         date_key = datetime.datetime.strptime(item['datetime'], date_format)
         return environment_key, date_key
 
@@ -56,9 +56,10 @@
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
             title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
                                         content_type="Content Type")
             self.stdout.write(title)
         for file_attr in files_attr:
+
             row = ROW_TEMPLATE.format(**file_attr)
             self.stdout.write(row)
```

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a4/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a4/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a4/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a4/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a4/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a3/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a4/src/django_sync_env/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,16 +361,14 @@
                     if is ``None``
     :type datefmt: ``str`` or ``None``
 
     :returns: Date part or nothing if not found
     :rtype: ``str`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
-
-    print('DEBUG: filename_to_datestring:datefmt:', datefmt)  # %d-%m-%Y-%H%M%S
     regex = datefmt_to_regex(datefmt)
     search = regex.search(filename)
     print('DEBUG: filename_to_datestring:filename: ', regex.search(filename)) # <re.Match object; span=(32, 49), match='16-04-2024-144625'>
     if search:
         return search.groups()[0]
 
 
@@ -382,15 +380,14 @@
                     if is ``None``
     :type datefmt: ``str`` or ``NoneType``
 
     :returns: Date guessed or nothing if no date found
     :rtype: ``datetime.datetime`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
-    print('DEBUG: filename_to_date:datefmt: ', datefmt) # %d-%m-%Y-%H%M%S
     datestring = filename_to_datestring(filename, datefmt)
     print('DEBUG: filename_to_date:datestring: ', datestring) # 16-04-2024-144625
     if datestring is not None:
         return datetime.strptime(datestring, datefmt)
 
 
 def filename_generate(
@@ -457,15 +454,15 @@
     return quote(arg)
 
 
 def get_storage_config(environment, storage_configs):
     storage = storage_configs.get(environment, None)
     if not storage:
         raise FieldDoesNotExist(
-            "specified environment does not exist in configured SYNC_ENV_BACKUP_CONFIG or SYNC_ENV_RESTORE_CONFIG",
+            "Specified environment does not exist in configured SYNC_ENV_BACKUP_CONFIG or SYNC_ENV_RESTORE_CONFIG",
             {"environment": environment, "storage_configs": storage_configs}
         )
     return storage
 
 
 def get_version(version):
     """Return a PEP 440-compliant version number from VERSION."""
```

### Comparing `django_sync_env-0.3.1a3/PKG-INFO` & `django_sync_env-0.3.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.1a3
+Version: 0.3.1a4
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

