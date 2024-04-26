# Comparing `tmp/ccml2021-0.2.5.tar.gz` & `tmp/ccml2021-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccml2021-0.2.5.tar", last modified: Thu Feb 22 06:46:51 2024, max compression
+gzip compressed data, was "ccml2021-0.2.6.tar", last modified: Fri Apr 26 06:15:12 2024, max compression
```

## Comparing `ccml2021-0.2.5.tar` & `ccml2021-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-02-22 06:46:51.919647 ccml2021-0.2.5/
--rw-r--r--   0 mrok       (501) staff       (20)      220 2024-02-22 06:46:51.919436 ccml2021-0.2.5/PKG-INFO
--rw-r--r--   0 mrok       (501) staff       (20)       37 2024-02-04 06:11:56.000000 ccml2021-0.2.5/README.md
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-02-22 06:46:51.917570 ccml2021-0.2.5/ccml2021/
--rw-r--r--   0 mrok       (501) staff       (20)        0 2024-02-04 03:28:17.000000 ccml2021-0.2.5/ccml2021/__init__.py
--rw-r--r--   0 mrok       (501) staff       (20)     6604 2024-02-22 06:22:53.000000 ccml2021-0.2.5/ccml2021/checker.py
--rw-r--r--   0 mrok       (501) staff       (20)     1155 2024-02-04 03:28:17.000000 ccml2021-0.2.5/ccml2021/gp.py
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-02-22 06:46:51.918611 ccml2021-0.2.5/ccml2021.egg-info/
--rw-r--r--   0 mrok       (501) staff       (20)      220 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/PKG-INFO
--rw-r--r--   0 mrok       (501) staff       (20)      347 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/SOURCES.txt
--rw-r--r--   0 mrok       (501) staff       (20)        1 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/dependency_links.txt
--rw-r--r--   0 mrok       (501) staff       (20)       84 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/entry_points.txt
--rw-r--r--   0 mrok       (501) staff       (20)        1 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/not-zip-safe
--rw-r--r--   0 mrok       (501) staff       (20)       12 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/requires.txt
--rw-r--r--   0 mrok       (501) staff       (20)        9 2024-02-22 06:46:51.000000 ccml2021-0.2.5/ccml2021.egg-info/top_level.txt
--rw-r--r--   0 mrok       (501) staff       (20)       38 2024-02-22 06:46:51.919713 ccml2021-0.2.5/setup.cfg
--rw-r--r--   0 mrok       (501) staff       (20)     1109 2024-02-22 06:41:34.000000 ccml2021-0.2.5/setup.py
-drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-02-22 06:46:51.919070 ccml2021-0.2.5/tests/
--rw-r--r--   0 mrok       (501) staff       (20)      902 2024-02-04 03:28:17.000000 ccml2021-0.2.5/tests/test_gp.py
--rw-r--r--   0 mrok       (501) staff       (20)      262 2024-02-04 03:28:17.000000 ccml2021-0.2.5/tests/test_virtual_reaction.py
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-04-26 06:15:12.709401 ccml2021-0.2.6/
+-rw-r--r--   0 mrok       (501) staff       (20)      256 2024-04-26 06:15:12.709276 ccml2021-0.2.6/PKG-INFO
+-rw-r--r--   0 mrok       (501) staff       (20)       37 2024-02-04 06:11:56.000000 ccml2021-0.2.6/README.md
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-04-26 06:15:12.708276 ccml2021-0.2.6/ccml2021/
+-rw-r--r--   0 mrok       (501) staff       (20)        0 2024-02-04 03:28:17.000000 ccml2021-0.2.6/ccml2021/__init__.py
+-rw-r--r--   0 mrok       (501) staff       (20)     6631 2024-04-26 06:12:06.000000 ccml2021-0.2.6/ccml2021/checker.py
+-rw-r--r--   0 mrok       (501) staff       (20)     1155 2024-02-04 03:28:17.000000 ccml2021-0.2.6/ccml2021/gp.py
+drwxr-xr-x   0 mrok       (501) staff       (20)        0 2024-04-26 06:15:12.709136 ccml2021-0.2.6/ccml2021.egg-info/
+-rw-r--r--   0 mrok       (501) staff       (20)      256 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/PKG-INFO
+-rw-r--r--   0 mrok       (501) staff       (20)      299 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/SOURCES.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        1 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/dependency_links.txt
+-rw-r--r--   0 mrok       (501) staff       (20)       85 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/entry_points.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        1 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/not-zip-safe
+-rw-r--r--   0 mrok       (501) staff       (20)       12 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/requires.txt
+-rw-r--r--   0 mrok       (501) staff       (20)        9 2024-04-26 06:15:12.000000 ccml2021-0.2.6/ccml2021.egg-info/top_level.txt
+-rw-r--r--   0 mrok       (501) staff       (20)       38 2024-04-26 06:15:12.709446 ccml2021-0.2.6/setup.cfg
+-rw-r--r--   0 mrok       (501) staff       (20)     1109 2024-04-26 06:12:46.000000 ccml2021-0.2.6/setup.py
```

### Comparing `ccml2021-0.2.5/ccml2021/checker.py` & `ccml2021-0.2.6/ccml2021/checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,16 @@
             "X_test_scaled",
             "models",
             "y_train_preds",
             "y_test_preds",
             "df",
             "importance_PLS",
             "importance_RF",
-        ]
+        ],
+        notebook_globals,
     )
 
     do_file_exists(
         ["PLS.png", "SVR.png", "RF.png", "importance_PLS.png", "importance_RF.png"]
     )
```

### Comparing `ccml2021-0.2.5/ccml2021/gp.py` & `ccml2021-0.2.6/ccml2021/gp.py`

 * *Files identical despite different names*

### Comparing `ccml2021-0.2.5/setup.py` & `ccml2021-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 for val in extras_dict.values():
     extras_list.extend(val)
 
 if __name__ == "__main__":
     setup(
         name="ccml2021",
-        version="0.2.5",
+        version="0.2.6",
         description="ccml2021",
         long_description=open(os.path.join(module_dir, "README.md")).read(),
         url="https://github.com/kmu/ccml2021",
         author="Koki Muraoka",
         author_email="muraok_k@chemsys.t.u-tokyo.ac.jp",
         packages=find_packages(),
         zip_safe=False,
```

