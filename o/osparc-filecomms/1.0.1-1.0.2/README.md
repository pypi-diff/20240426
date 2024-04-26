# Comparing `tmp/osparc_filecomms-1.0.1-py2.py3-none-any.whl.zip` & `tmp/osparc_filecomms-1.0.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5257 bytes, number of entries: 8
--rw-r--r--  2.0 unx      217 b- defN 24-Apr-16 07:58 osparc_filecomms/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Apr-16 07:58 osparc_filecomms/_version.py
--rw-r--r--  2.0 unx     5941 b- defN 24-Apr-16 07:58 osparc_filecomms/handshakers.py
--rw-r--r--  2.0 unx      678 b- defN 24-Apr-16 07:58 osparc_filecomms-1.0.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3081 b- defN 24-Apr-16 07:58 osparc_filecomms-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-16 07:58 osparc_filecomms-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-Apr-16 07:58 osparc_filecomms-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      691 b- defN 24-Apr-16 07:58 osparc_filecomms-1.0.1.dist-info/RECORD
-8 files, 11146 bytes uncompressed, 4037 bytes compressed:  63.8%
+Zip file size: 5352 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      217 b- defN 24-Apr-26 09:24 osparc_filecomms/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-26 09:24 osparc_filecomms/_version.py
+-rw-r--r--  2.0 unx     6487 b- defN 24-Apr-26 09:24 osparc_filecomms/handshakers.py
+-rw-r--r--  2.0 unx      678 b- defN 24-Apr-26 09:24 osparc_filecomms-1.0.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3081 b- defN 24-Apr-26 09:24 osparc_filecomms-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-26 09:24 osparc_filecomms-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-26 09:24 osparc_filecomms-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      691 b- defN 24-Apr-26 09:24 osparc_filecomms-1.0.2.dist-info/RECORD
+8 files, 11692 bytes uncompressed, 4132 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: osparc_filecomms/_version.py
 Comment: 
 
 Filename: osparc_filecomms/handshakers.py
 Comment: 
 
-Filename: osparc_filecomms-1.0.1.dist-info/LICENSE.txt
+Filename: osparc_filecomms-1.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: osparc_filecomms-1.0.1.dist-info/METADATA
+Filename: osparc_filecomms-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: osparc_filecomms-1.0.1.dist-info/WHEEL
+Filename: osparc_filecomms-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: osparc_filecomms-1.0.1.dist-info/top_level.txt
+Filename: osparc_filecomms-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: osparc_filecomms-1.0.1.dist-info/RECORD
+Filename: osparc_filecomms-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osparc_filecomms/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '1.0.1'
-__version_tuple__ = version_tuple = (1, 0, 1)
+__version__ = version = '1.0.2'
+__version_tuple__ = version_tuple = (1, 0, 2)
```

## osparc_filecomms/handshakers.py

```diff
@@ -24,14 +24,15 @@
     ):
         self.verbose_level = verbose_level
         logger.setLevel(self.verbose_level)
 
         self.self_uuid = str(self_uuid)
         self.other_uuid = None
 
+        self.last_write = None
         self.is_initiator = is_initiator
 
         self.input_dir_path = input_dir_path
         self.output_dir_path = output_dir_path
         self.handshake_filename = handshake_filename
         self.polling_interval = polling_interval
         self.print_polling_interval = print_polling_interval
@@ -50,24 +51,36 @@
             self.handshake_output_path.unlink()
 
         if self.is_initiator:
             return self.shake_initiator()
         else:
             return self.shake_receiver()
 
+    def write_filecontent(self, path: pl.Path, content: str):
+        path.write_text(content)
+
+        self.last_write = path, content
+
+    def retry_last_write(self):
+        if self.last_write is not None:
+            path, content = self.last_write
+            self.write_filecontent(path, content)
+
     def shake_initiator(self):
         """Shake hand by initiator"""
 
         handshake_out = {
             "command": "register",
             "uuid": self.self_uuid,
         }
         if self.handshake_output_path.exists():
             self.handshake_output_path.unlink()
-        self.handshake_output_path.write_text(json.dumps(handshake_out))
+        self.write_filecontent(
+            self.handshake_output_path, json.dumps(handshake_out)
+        )
         logger.info(f"Wrote handshake file to {self.handshake_output_path}")
 
         def try_handshake():
             handshake_input_content = self.read_until_path_exists(
                 self.handshake_input_path,
                 wait_message="Waiting for handshake confirmation at "
                 f"{self.handshake_input_path}...",
@@ -85,27 +98,31 @@
                 break
             else:
                 if waiter % self.print_polling_interval == 0:
                     logger.info(
                         "Waiting for correct handshake registration "
                         "confirmation ..."
                     )
+                    self.retry_last_write()
+
                 waiter += 1
             time.sleep(self.polling_interval)
 
         other_uuid = handshake_in["uuid"]
 
         handshake_out = {
             "command": "confirm_registration",
             "uuid": self.self_uuid,
             "confirmed_uuid": other_uuid,
         }
         if self.handshake_output_path.exists():
             self.handshake_output_path.unlink()
-        self.handshake_output_path.write_text(json.dumps(handshake_out))
+        self.write_filecontent(
+            self.handshake_output_path, json.dumps(handshake_out)
+        )
 
         assert other_uuid is not None
 
         self.other_uuid = other_uuid
 
         return self.other_uuid
 
@@ -131,17 +148,19 @@
                     if self.handshake_output_path.exists():
                         self.handshake_output_path.unlink()
                     handshake_out = {
                         "command": "confirm_registration",
                         "uuid": self.self_uuid,
                         "confirmed_uuid": other_uuid,
                     }
-                    self.handshake_output_path.write_text(
-                        json.dumps(handshake_out)
+
+                    self.write_filecontent(
+                        self.handshake_output_path, json.dumps(handshake_out)
                     )
+
                     logger.info(
                         f"Wrote handshake confirmation to {self.handshake_output_path}"
                     )
                     last_written_other_uuid = other_uuid
             elif command == "confirm_registration":
                 if (
                     other_uuid is not None
@@ -150,14 +169,16 @@
                 ):
                     break
             else:
                 raise ValueError(f"Invalid handshake command: {command}")
 
             if waiter % self.print_polling_interval == 0:
                 logger.info("Waiting for registration confirmation ...")
+                self.retry_last_write()
+
             time.sleep(self.polling_interval)
             waiter += 1
 
         assert other_uuid is not None
 
         self.other_uuid = other_uuid
 
@@ -172,9 +193,10 @@
                 except FileNotFoundError:
                     pass
                 else:
                     return file_content
 
             if waiter % self.print_polling_interval == 0:
                 logger.debug(wait_message)
+                self.retry_last_write()
             time.sleep(self.polling_interval)
             waiter += 1
```

## Comparing `osparc_filecomms-1.0.1.dist-info/LICENSE.txt` & `osparc_filecomms-1.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `osparc_filecomms-1.0.1.dist-info/METADATA` & `osparc_filecomms-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osparc_filecomms
-Version: 1.0.1
+Version: 1.0.2
 Summary: oSparc file communications
 Author: Werner Van Geit @ IT'IS Zurich
 License: Copyright (C) IT'IS Foundation - All Rights Reserved
         
         Written by Werner Van Geit <vangeit at itis.swiss>, 2023
         
         Unless required by applicable law or agreed to in writing,
```

