# Comparing `tmp/django_sync_env-0.3.1a1.tar.gz` & `tmp/django_sync_env-0.3.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_sync_env-0.3.1a1.tar", max compression
+gzip compressed data, was "django_sync_env-0.3.1a2.tar", max compression
```

## Comparing `django_sync_env-0.3.1a1.tar` & `django_sync_env-0.3.1a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a1/README.md
--rw-r--r--   0        0        0      499 2024-04-26 03:01:59.472360 django_sync_env-0.3.1a1/pyproject.toml
--rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a1/src/django_sync_env/__init__.py
--rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a1/src/django_sync_env/apps.py
--rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a1/src/django_sync_env/checks.py
--rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.3.1a1/src/django_sync_env/constants.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a1/src/django_sync_env/db/__init__.py
--rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a1/src/django_sync_env/db/base.py
--rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a1/src/django_sync_env/db/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a1/src/django_sync_env/db/mongodb.py
--rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a1/src/django_sync_env/db/mysql.py
--rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a1/src/django_sync_env/db/postgresql.py
--rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a1/src/django_sync_env/db/sqlite.py
--rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a1/src/django_sync_env/log.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a1/src/django_sync_env/management/__init__.py
--rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/__init__.py
--rw-r--r--   0        0        0     5237 2024-02-07 19:58:44.770356 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/_base.py
--rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_backup_db.py
--rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_backup_media.py
--rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_download_db.py
--rw-r--r--   0        0        0     2506 2024-04-26 03:01:35.855960 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_list_db_backups.py
--rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_list_media_backups.py
--rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_restore_db.py
--rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_restore_media.py
--rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a1/src/django_sync_env/notifications.py
--rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.3.1a1/src/django_sync_env/settings.py
--rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a1/src/django_sync_env/storage.py
--rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a1/src/django_sync_env/tasks.py
--rw-r--r--   0        0        0    14531 2024-04-26 02:58:53.362147 django_sync_env-0.3.1a1/src/django_sync_env/utils.py
--rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a1/PKG-INFO
+-rw-r--r--   0        0        0     2086 2024-02-07 19:58:44.763491 django_sync_env-0.3.1a2/README.md
+-rw-r--r--   0        0        0      499 2024-04-26 03:25:54.586531 django_sync_env-0.3.1a2/pyproject.toml
+-rw-r--r--   0        0        0      303 2024-04-26 01:27:56.013634 django_sync_env-0.3.1a2/src/django_sync_env/__init__.py
+-rw-r--r--   0        0        0      420 2024-02-07 19:58:44.767427 django_sync_env-0.3.1a2/src/django_sync_env/apps.py
+-rw-r--r--   0        0        0      941 2024-04-26 03:00:14.920473 django_sync_env-0.3.1a2/src/django_sync_env/checks.py
+-rw-r--r--   0        0        0      194 2024-02-07 19:58:44.767857 django_sync_env-0.3.1a2/src/django_sync_env/constants.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.768034 django_sync_env-0.3.1a2/src/django_sync_env/db/__init__.py
+-rw-r--r--   0        0        0     6328 2024-02-07 19:58:44.768361 django_sync_env-0.3.1a2/src/django_sync_env/db/base.py
+-rw-r--r--   0        0        0      305 2024-02-07 19:58:44.768575 django_sync_env-0.3.1a2/src/django_sync_env/db/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-02-07 19:58:44.768752 django_sync_env-0.3.1a2/src/django_sync_env/db/mongodb.py
+-rw-r--r--   0        0        0     1721 2024-02-07 19:58:44.768922 django_sync_env-0.3.1a2/src/django_sync_env/db/mysql.py
+-rw-r--r--   0        0        0     5116 2024-04-26 01:27:56.014625 django_sync_env-0.3.1a2/src/django_sync_env/db/postgresql.py
+-rw-r--r--   0        0        0     3394 2024-02-07 19:58:44.769378 django_sync_env-0.3.1a2/src/django_sync_env/db/sqlite.py
+-rw-r--r--   0        0        0      346 2024-02-07 19:58:44.769633 django_sync_env-0.3.1a2/src/django_sync_env/log.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.769884 django_sync_env-0.3.1a2/src/django_sync_env/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-07 19:58:44.770115 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/__init__.py
+-rw-r--r--   0        0        0     5549 2024-04-26 03:25:34.613321 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/_base.py
+-rw-r--r--   0        0        0     7537 2024-02-07 21:28:28.096372 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_db.py
+-rw-r--r--   0        0        0     8274 2024-02-07 21:28:28.096907 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_media.py
+-rw-r--r--   0        0        0     5758 2024-04-26 01:27:56.015448 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_download_db.py
+-rw-r--r--   0        0        0     2466 2024-04-26 03:16:30.351022 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_db_backups.py
+-rw-r--r--   0        0        0     2386 2024-02-07 21:28:28.098312 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_media_backups.py
+-rw-r--r--   0        0        0     6718 2024-02-07 21:28:28.098801 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_db.py
+-rw-r--r--   0        0        0     5586 2024-02-07 21:28:28.099473 django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_media.py
+-rw-r--r--   0        0        0     1163 2024-02-07 19:58:44.772084 django_sync_env-0.3.1a2/src/django_sync_env/notifications.py
+-rw-r--r--   0        0        0     1634 2024-02-07 19:58:44.772377 django_sync_env-0.3.1a2/src/django_sync_env/settings.py
+-rw-r--r--   0        0        0     9331 2024-02-07 21:28:28.100529 django_sync_env-0.3.1a2/src/django_sync_env/storage.py
+-rw-r--r--   0        0        0      893 2024-02-07 19:58:44.772805 django_sync_env-0.3.1a2/src/django_sync_env/tasks.py
+-rw-r--r--   0        0        0    14789 2024-04-26 03:25:50.132834 django_sync_env-0.3.1a2/src/django_sync_env/utils.py
+-rw-r--r--   0        0        0     2702 1970-01-01 00:00:00.000000 django_sync_env-0.3.1a2/PKG-INFO
```

### Comparing `django_sync_env-0.3.1a1/README.md` & `django_sync_env-0.3.1a2/README.md`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/checks.py` & `django_sync_env-0.3.1a2/src/django_sync_env/checks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/db/base.py` & `django_sync_env-0.3.1a2/src/django_sync_env/db/base.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/db/mongodb.py` & `django_sync_env-0.3.1a2/src/django_sync_env/db/mongodb.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/db/mysql.py` & `django_sync_env-0.3.1a2/src/django_sync_env/db/mysql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/db/postgresql.py` & `django_sync_env-0.3.1a2/src/django_sync_env/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/db/sqlite.py` & `django_sync_env-0.3.1a2/src/django_sync_env/db/sqlite.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/_base.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -134,14 +134,18 @@
 
     def get_backups_attrs(self, storage, options, environment):
         filters = {k: v for k, v in options.items() if k in FILTER_KEYS}
 
         backups = []
         filenames = storage.list_backups(**filters)
         for filename in filenames:
+            print('DEBUG: _base:get_backups_attrs: filename: ', filename)
+            print('DEBUG: _base:get_backups_attrs: utils.filename_to_date(filename): ', utils.filename_to_date(filename))
+            print('DEBUG: _base:get_backups_attrs:datetime: ', utils.filename_to_date(filename).strftime("%x %X"))
+
             backups.append(
                 {
                     "environment": environment,
                     "datetime": utils.filename_to_date(filename).strftime("%x %X"),
                     "name": filename,
                 }
             )
```

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_backup_db.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_backup_media.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_backup_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_download_db.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_download_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_list_db_backups.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_db_backups.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,10 +57,9 @@
             files_attr = sorted(files_attr, key=self.custom_sort, reverse=True)
 
         if not self.quiet:
             title = ROW_TEMPLATE.format(name="Name", environment="Environment", datetime="Datetime",
                                         content_type="Content Type")
             self.stdout.write(title)
         for file_attr in files_attr:
-            import pdb; pdb.set_trace()
             row = ROW_TEMPLATE.format(**file_attr)
             self.stdout.write(row)
```

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_list_media_backups.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_list_media_backups.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_restore_db.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_db.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/management/commands/sync_env_restore_media.py` & `django_sync_env-0.3.1a2/src/django_sync_env/management/commands/sync_env_restore_media.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/notifications.py` & `django_sync_env-0.3.1a2/src/django_sync_env/notifications.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/settings.py` & `django_sync_env-0.3.1a2/src/django_sync_env/settings.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/storage.py` & `django_sync_env-0.3.1a2/src/django_sync_env/storage.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/tasks.py` & `django_sync_env-0.3.1a2/src/django_sync_env/tasks.py`

 * *Files identical despite different names*

### Comparing `django_sync_env-0.3.1a1/src/django_sync_env/utils.py` & `django_sync_env-0.3.1a2/src/django_sync_env/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -361,16 +361,19 @@
                     if is ``None``
     :type datefmt: ``str`` or ``None``
 
     :returns: Date part or nothing if not found
     :rtype: ``str`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
+
+    print('DEBUG: filename_to_datestring:datefmt:', datefmt)
     regex = datefmt_to_regex(datefmt)
     search = regex.search(filename)
+    print('DEBUG: filename_to_datestring:filename: ', regex.search(filename))
     if search:
         return search.groups()[0]
 
 
 def filename_to_date(filename, datefmt=None):
     """
     Return a datetime from a file name.
@@ -379,15 +382,17 @@
                     if is ``None``
     :type datefmt: ``str`` or ``NoneType``
 
     :returns: Date guessed or nothing if no date found
     :rtype: ``datetime.datetime`` or ``NoneType``
     """
     datefmt = datefmt or settings.DATE_FORMAT
+    print('DEBUG: filename_to_date:datefmt: ', datefmt)
     datestring = filename_to_datestring(filename, datefmt)
+    print('DEBUG: filename_to_date:datestring: ', datestring)
     if datestring is not None:
         return datetime.strptime(datestring, datefmt)
 
 
 def filename_generate(
         extension,
         database_name="",
```

### Comparing `django_sync_env-0.3.1a1/PKG-INFO` & `django_sync_env-0.3.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sync-env
-Version: 0.3.1a1
+Version: 0.3.1a2
 Summary: Backup, Sync and Restore Databases and Media
 Author: Dan Brosnan
 Author-email: dan.brosnan@octave.nz
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

