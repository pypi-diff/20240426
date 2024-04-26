# Comparing `tmp/damnit-0.1.1.tar.gz` & `tmp/damnit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damnit-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "damnit-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `damnit-0.1.1.tar` & `damnit-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1548 2024-04-24 11:28:42.079800 damnit-0.1.1/LICENSE
--rw-r--r--   0        0        0      340 2024-04-24 11:28:42.079800 damnit-0.1.1/README.md
--rw-r--r--   0        0        0      144 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/__init__.py
--rw-r--r--   0        0        0    12828 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/api.py
--rw-r--r--   0        0        0       74 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/__init__.py
--rw-r--r--   0        0        0    15744 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/db.py
--rw-r--r--   0        0        0    14590 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/extract_data.py
--rw-r--r--   0        0        0     6203 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/listener.py
--rw-r--r--   0        0        0      397 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/supervisord.conf
--rw-r--r--   0        0        0     5965 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/supervisord.py
--rw-r--r--   0        0        0     2511 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/test_listener.py
--rw-r--r--   0        0        0     2851 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/backend/user_variables.py
--rw-r--r--   0        0        0     1528 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/base_context_file.py
--rw-r--r--   0        0        0     9646 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/cli.py
--rw-r--r--   0        0        0      381 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/context.py
--rw-r--r--   0        0        0      266 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/ctxsupport/README.md
--rw-r--r--   0        0        0    25775 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/ctxsupport/ctxrunner.py
--rw-r--r--   0        0        0     2146 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/ctxsupport/damnit_ctx.py
--rw-r--r--   0        0        0      252 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/definitions.py
--rw-r--r--   0        0        0       30 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/__init__.py
--rw-r--r--   0        0        0     4214 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/editor.py
--rw-r--r--   0        0        0     9930 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/AMORE.png
--rw-r--r--   0        0        0     9825 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/closed-hover.png
--rw-r--r--   0        0        0     8086 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/closed.png
--rw-r--r--   0        0        0      750 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/export.png
--rw-r--r--   0        0        0     1317 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/green_circle.svg
--rw-r--r--   0        0        0     4022 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/lock_closed_icon.png
--rw-r--r--   0        0        0     3710 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/lock_open_icon.png
--rw-r--r--   0        0        0     4053 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/lock_opening_icon.png
--rw-r--r--   0        0        0     9751 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/open-hover.png
--rw-r--r--   0        0        0     8219 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/open.png
--rw-r--r--   0        0        0     1291 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/red_circle.svg
--rw-r--r--   0        0        0      991 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/search_icon.png
--rw-r--r--   0        0        0     1317 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/ico/yellow_circle.svg
--rw-r--r--   0        0        0     2738 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/kafka.py
--rw-r--r--   0        0        0    39083 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/main_window.py
--rw-r--r--   0        0        0     3392 2024-04-24 11:28:42.079800 damnit-0.1.1/damnit/gui/open_dialog.py
--rw-r--r--   0        0        0     4569 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/open_dialog.ui
--rw-r--r--   0        0        0     4137 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/open_dialog_ui.py
--rw-r--r--   0        0        0    26360 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/plot.py
--rw-r--r--   0        0        0    32504 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/table.py
--rw-r--r--   0        0        0     7444 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/user_variables.py
--rw-r--r--   0        0        0     2075 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/widgets.py
--rw-r--r--   0        0        0    12238 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/gui/zulip_messenger.py
--rw-r--r--   0        0        0    14257 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/migrations.py
--rw-r--r--   0        0        0     1455 2024-04-24 11:28:42.083800 damnit-0.1.1/damnit/util.py
--rw-r--r--   0        0        0     1439 2024-04-24 11:28:42.099800 damnit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 damnit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1548 2024-04-26 17:00:52.989340 damnit-0.1.2/LICENSE
+-rw-r--r--   0        0        0      340 2024-04-26 17:00:52.989340 damnit-0.1.2/README.md
+-rw-r--r--   0        0        0      144 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/__init__.py
+-rw-r--r--   0        0        0    13250 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/api.py
+-rw-r--r--   0        0        0       74 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/__init__.py
+-rw-r--r--   0        0        0    15744 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/db.py
+-rw-r--r--   0        0        0    14590 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/extract_data.py
+-rw-r--r--   0        0        0     6203 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/listener.py
+-rw-r--r--   0        0        0      397 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/supervisord.conf
+-rw-r--r--   0        0        0     5965 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/supervisord.py
+-rw-r--r--   0        0        0     2511 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/test_listener.py
+-rw-r--r--   0        0        0     2851 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/backend/user_variables.py
+-rw-r--r--   0        0        0     1528 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/base_context_file.py
+-rw-r--r--   0        0        0     9646 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/cli.py
+-rw-r--r--   0        0        0      381 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/context.py
+-rw-r--r--   0        0        0      266 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/ctxsupport/README.md
+-rw-r--r--   0        0        0    25775 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/ctxsupport/ctxrunner.py
+-rw-r--r--   0        0        0     2146 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/ctxsupport/damnit_ctx.py
+-rw-r--r--   0        0        0      252 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/definitions.py
+-rw-r--r--   0        0        0       30 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/__init__.py
+-rw-r--r--   0        0        0     4214 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/editor.py
+-rw-r--r--   0        0        0     9930 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/AMORE.png
+-rw-r--r--   0        0        0     9825 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/closed-hover.png
+-rw-r--r--   0        0        0     8086 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/closed.png
+-rw-r--r--   0        0        0      750 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/export.png
+-rw-r--r--   0        0        0     1317 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/green_circle.svg
+-rw-r--r--   0        0        0     4022 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/lock_closed_icon.png
+-rw-r--r--   0        0        0     3710 2024-04-26 17:00:52.989340 damnit-0.1.2/damnit/gui/ico/lock_open_icon.png
+-rw-r--r--   0        0        0     4053 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/lock_opening_icon.png
+-rw-r--r--   0        0        0     9751 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/open-hover.png
+-rw-r--r--   0        0        0     8219 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/open.png
+-rw-r--r--   0        0        0     1291 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/red_circle.svg
+-rw-r--r--   0        0        0      991 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/search_icon.png
+-rw-r--r--   0        0        0     1317 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/ico/yellow_circle.svg
+-rw-r--r--   0        0        0     2738 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/kafka.py
+-rw-r--r--   0        0        0    39083 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/main_window.py
+-rw-r--r--   0        0        0     3392 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/open_dialog.py
+-rw-r--r--   0        0        0     4569 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/open_dialog.ui
+-rw-r--r--   0        0        0     4137 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/open_dialog_ui.py
+-rw-r--r--   0        0        0    26360 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/plot.py
+-rw-r--r--   0        0        0    32504 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/table.py
+-rw-r--r--   0        0        0     7444 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/user_variables.py
+-rw-r--r--   0        0        0     2075 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/widgets.py
+-rw-r--r--   0        0        0    12238 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/gui/zulip_messenger.py
+-rw-r--r--   0        0        0    14257 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/migrations.py
+-rw-r--r--   0        0        0     1455 2024-04-26 17:00:52.993340 damnit-0.1.2/damnit/util.py
+-rw-r--r--   0        0        0     1439 2024-04-26 17:00:53.009340 damnit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 damnit-0.1.2/PKG-INFO
```

### Comparing `damnit-0.1.1/LICENSE` & `damnit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/api.py` & `damnit-0.1.2/damnit/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -233,16 +233,28 @@
         it.
         """
         return sorted(self._key_locations().keys())
 
     def _var_titles(self):
         result = self._db.conn.execute("SELECT name, title FROM variables").fetchall()
         available_vars = self.keys()
-        return { row[0]: row[1] if row[1] is not None else row[0] for row in result
-                 if row[0] in available_vars }
+        titles = { row[0]: row[1] if row[1] is not None else row[0] for row in result
+                   if row[0] in available_vars }
+
+        # These variables are created automatically, but they aren't included in
+        # the `variables` table (yet) so we need to explicitly add their titles.
+        special_vars = {
+            "start_time": "Timestamp",
+            "comment": "Comment"
+        }
+        for name, title in special_vars.items():
+            if name in available_vars:
+                titles[name] = title
+
+        return titles
 
     def titles(self) -> list:
         """The titles of available variables.
 
         As with [RunVariables.keys()][damnit.api.RunVariables.keys], only
         variables that have data for the run will be included.
         """
```

### Comparing `damnit-0.1.1/damnit/backend/db.py` & `damnit-0.1.2/damnit/backend/db.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/backend/extract_data.py` & `damnit-0.1.2/damnit/backend/extract_data.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/backend/listener.py` & `damnit-0.1.2/damnit/backend/listener.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/backend/supervisord.py` & `damnit-0.1.2/damnit/backend/supervisord.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/backend/test_listener.py` & `damnit-0.1.2/damnit/backend/test_listener.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/backend/user_variables.py` & `damnit-0.1.2/damnit/backend/user_variables.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/base_context_file.py` & `damnit-0.1.2/damnit/base_context_file.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/cli.py` & `damnit-0.1.2/damnit/cli.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/ctxsupport/ctxrunner.py` & `damnit-0.1.2/damnit/ctxsupport/ctxrunner.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/ctxsupport/damnit_ctx.py` & `damnit-0.1.2/damnit/ctxsupport/damnit_ctx.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/editor.py` & `damnit-0.1.2/damnit/gui/editor.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/AMORE.png` & `damnit-0.1.2/damnit/gui/ico/AMORE.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/closed-hover.png` & `damnit-0.1.2/damnit/gui/ico/closed-hover.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/closed.png` & `damnit-0.1.2/damnit/gui/ico/closed.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/export.png` & `damnit-0.1.2/damnit/gui/ico/export.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/green_circle.svg` & `damnit-0.1.2/damnit/gui/ico/green_circle.svg`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/lock_closed_icon.png` & `damnit-0.1.2/damnit/gui/ico/lock_closed_icon.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/lock_open_icon.png` & `damnit-0.1.2/damnit/gui/ico/lock_open_icon.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/lock_opening_icon.png` & `damnit-0.1.2/damnit/gui/ico/lock_opening_icon.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/open-hover.png` & `damnit-0.1.2/damnit/gui/ico/open-hover.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/open.png` & `damnit-0.1.2/damnit/gui/ico/open.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/red_circle.svg` & `damnit-0.1.2/damnit/gui/ico/red_circle.svg`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/search_icon.png` & `damnit-0.1.2/damnit/gui/ico/search_icon.png`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/ico/yellow_circle.svg` & `damnit-0.1.2/damnit/gui/ico/yellow_circle.svg`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/kafka.py` & `damnit-0.1.2/damnit/gui/kafka.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/main_window.py` & `damnit-0.1.2/damnit/gui/main_window.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/open_dialog.py` & `damnit-0.1.2/damnit/gui/open_dialog.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/open_dialog.ui` & `damnit-0.1.2/damnit/gui/open_dialog.ui`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/open_dialog_ui.py` & `damnit-0.1.2/damnit/gui/open_dialog_ui.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/plot.py` & `damnit-0.1.2/damnit/gui/plot.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/table.py` & `damnit-0.1.2/damnit/gui/table.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/user_variables.py` & `damnit-0.1.2/damnit/gui/user_variables.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/widgets.py` & `damnit-0.1.2/damnit/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/gui/zulip_messenger.py` & `damnit-0.1.2/damnit/gui/zulip_messenger.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/migrations.py` & `damnit-0.1.2/damnit/migrations.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/damnit/util.py` & `damnit-0.1.2/damnit/util.py`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/pyproject.toml` & `damnit-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `damnit-0.1.1/PKG-INFO` & `damnit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damnit
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Data And Metadata iNspection Interactive Thing
 Author-email: Thomas Kluyver <thomas.kluyver@xfel.eu>, Luca Gelisio <luca.gelisio@xfel.eu>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Requires-Dist: h5netcdf
 Requires-Dist: h5py
```

