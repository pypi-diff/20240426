# Comparing `tmp/django_sync_env-0.3.0.tar.gz` & `tmp/django_sync_env-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.0.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a0.tar", max compression
```

## Comparing `django_sync_env-0.3.0.tar` & `django_sync_env-0.3.1a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-04-10 02:17:37.067178 django_sync_env-0.3.0/README.md
--rw-r--r--   0        0        0      497 2024-04-10 02:21:08.041198 django_sync_env-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-10 02:17:37.069573 django_sync_env-0.3.0/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-04-10 02:17:37.069705 django_sync_env-0.3.0/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-10 02:17:37.069823 django_sync_env-0.3.0/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      194 2024-04-10 02:17:37.069930 django_sync_env-0.3.0/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-04-10 02:17:37.070048 django_sync_env-0.3.0/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-04-10 02:17:37.070328 django_sync_env-0.3.0/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-04-10 02:17:37.070503 django_sync_env-0.3.0/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-04-10 02:17:37.070659 django_sync_env-0.3.0/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-04-10 02:17:37.070809 django_sync_env-0.3.0/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-10 03:54:56.625179 django_sync_env-0.3.0/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-04-10 02:17:37.071078 django_sync_env-0.3.0/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-04-10 02:17:37.071194 django_sync_env-0.3.0/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-04-10 02:17:37.071310 django_sync_env-0.3.0/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:17:37.071665 django_sync_env-0.3.0/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5237 2024-04-10 02:17:37.072154 django_sync_env-0.3.0/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-04-10 02:17:37.072564 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-04-10 02:17:37.072820 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-10 03:29:10.073282 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2467 2024-04-10 02:17:37.072996 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-04-10 02:17:37.073125 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-04-10 02:17:37.073512 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-04-10 02:17:37.073807 django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-04-10 02:17:37.074063 django_sync_env-0.3.0/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1634 2024-04-10 02:59:23.723343 django_sync_env-0.3.0/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-04-10 02:17:37.074329 django_sync_env-0.3.0/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-04-10 02:17:37.074407 django_sync_env-0.3.0/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14531 2024-04-10 02:17:37.074621 django_sync_env-0.3.0/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2700 1970-01-01 00:00:00.000000 django_sync_env-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a0/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 02:02:20.303368 django_sync_env-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a0/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a0/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      959 2024-04-26 02:52:33.848432 django_sync_env-0.3.1a0/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.3.1a0/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a0/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a0/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a0/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a0/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a0/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a0/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a0/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a0/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a0/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5237 2024-02-07 19:58:44.770356 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2468 2024-04-26 02:39:16.857937 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a0/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.3.1a0/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a0/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a0/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14576 2024-04-26 02:52:33.855072 django_sync_env-0.3.1a0/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a0/PKG-INFO
```

### Comparing `django_sync_env-0.3.0/README.md` & `django_sync_env-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a0/src/django_sync_env/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 W002 = Warning(
     "SYNC_ENV_RESTORE_CONFIG setting has not be configured",
     hint="Set up settings.SYNC_ENV_RESTORE_CONFIG see syncenv readme",
     id="syncenv.W002",
 )
 
 W005 = Warning(
-    "Invalid DATE_FORMAT parameter",
+    "Invalid SYNC_ENV_DATE_FORMAT parameter",
     hint="settings.SYNC_ENV_DATE_FORMAT can contain only [A-Za-z0-9%_-]",
     id="syncenv.W005",
 )
 
 
 @register(Tags.compatibility)
 def check_settings(app_configs, **kwargs):
@@ -29,11 +29,11 @@
 
     if not settings.SYNC_ENV_BACKUP_CONFIG:
         errors.append(W001)
 
     if not settings.SYNC_ENV_RESTORE_CONFIG:
         errors.append(W001)
 
-    if re.search(r"[^A-Za-z0-9%_-]", settings.DATE_FORMAT):
+    if re.search(r"[^A-Za-z0-9%_-]", settings.SYNC_ENV_DATE_FORMAT):
         errors.append(W005)
 
     return errors
```

### Comparing `django_sync_env-0.3.0/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a0/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a0/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a0/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a0/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a0/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
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
 
@@ -57,9 +57,11 @@
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
             title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
                                         content_type="Content Type")
             self.stdout.write(title)
         for file_attr in files_attr:
+
+
             row = ROW_TEMPLATE.format(**file_attr)
             self.stdout.write(row)
```

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a0/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a0/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a0/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a0/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a0/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.0/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a0/src/django_sync_env/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,15 @@
     :param value: a datetime object
     :type value: datetime.datetime
 
     :return: the timestamp
     :rtype: str
     """
     value = value if timezone.is_naive(value) else timezone.localtime(value)
-    return value.strftime(settings.DATE_FORMAT)
+    return value.strftime(settings.SYNC_ENV_DATE_FORMAT)
 
 
 def filename_details(filepath):
     # TODO: What was this function made for ?
     return ""
 
 
@@ -360,33 +360,33 @@
     :param datefmt: strftime format string, ``settings.DATE_FORMAT`` is used
                     if is ``None``
     :type datefmt: ``str`` or ``None``
 
     :returns: Date part or nothing if not found
     :rtype: ``str`` or ``NoneType``
     """
-    datefmt = datefmt or settings.DATE_FORMAT
+    datefmt = datefmt or settings.SYNC_ENV_DATE_FORMAT
     regex = datefmt_to_regex(datefmt)
     search = regex.search(filename)
     if search:
         return search.groups()[0]
 
 
 def filename_to_date(filename, datefmt=None):
     """
     Return a datetime from a file name.
 
-    :param datefmt: strftime format string, ``settings.DATE_FORMAT`` is used
+    :param datefmt: strftime format string, ``settings.SYNC_ENV_DATE_FORMAT`` is used
                     if is ``None``
     :type datefmt: ``str`` or ``NoneType``
 
     :returns: Date guessed or nothing if no date found
     :rtype: ``datetime.datetime`` or ``NoneType``
     """
-    datefmt = datefmt or settings.DATE_FORMAT
+    datefmt = datefmt or settings.SYNC_ENV_DATE_FORMAT
     datestring = filename_to_datestring(filename, datefmt)
     if datestring is not None:
         return datetime.strptime(datestring, datefmt)
 
 
 def filename_generate(
         extension,
@@ -430,15 +430,15 @@
         template = settings.MEDIA_FILENAME_TEMPLATE
     else:
         template = settings.FILENAME_TEMPLATE
 
     params = {
         "environment": environment,
         "projectname": projectname or settings.SYNC_ENV_PROJECT_NAME,
-        "datetime": wildcard or datetime.now().strftime(settings.DATE_FORMAT),
+        "datetime": wildcard or datetime.now().strftime(settings.SYNC_ENV_DATE_FORMAT),
         "databasename": database_name,
         "extension": extension,
         "content_type": content_type,
     }
     if callable(template):
         filename = template(**params)
     else:
```

### Comparing `django_sync_env-0.3.0/PKG-INFO` & `django_sync_env-0.3.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.0
+Version: 0.3.1a0
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: django-storages (>=1.14.2,<2.0.0)
-Requires-Dist: inquirer (>=3.2.1,<4.0.0)
-Requires-Dist: slack-sdk (>=3.26.0,<4.0.0)
+Requires-Dist: inquirer (>=3.2.4,<4.0.0)
+Requires-Dist: slack-sdk (>=3.27.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Django sync env
 
 django-sync-env is a Django app to manage backing up and restoring django databases and media assets easily.
 
 Detailed documentation is in the "docs" directory (it's a work in progress).
```

