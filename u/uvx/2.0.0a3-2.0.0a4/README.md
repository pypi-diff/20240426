# Comparing `tmp/uvx-2.0.0a3.tar.gz` & `tmp/uvx-2.0.0a4.tar.gz`

## Comparing `uvx-2.0.0a3.tar` & `uvx-2.0.0a4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 uvx-2.0.0a3/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a3/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a3/.gitignore
--rw-rw-r--   0     1000     1000      242 2024-04-24 20:55:06.000000 uvx-2.0.0a3/CHANGELOG.md
--rw-rw-r--   0     1000     1000    86391 2024-04-26 18:22:01.000000 uvx-2.0.0a3/Cargo.lock
--rw-rw-r--   0     1000     1000     1582 2024-04-24 21:12:17.000000 uvx-2.0.0a3/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.0a3/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a3/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.0a3/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.0a3/src/cli.rs
--rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.0a3/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.0a3/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.0a3/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.0a3/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.0a3/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.0a3/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.0a3/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.0a3/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.0a3/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.0a3/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.0a3/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.0a3/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.0a3/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     2934 2024-04-24 20:42:03.000000 uvx-2.0.0a3/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.0a3/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.0a3/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.0a3/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.0a3/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.0a3/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.0a3/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.0a3/src/main.rs
--rw-rw-r--   0     1000     1000     7501 2024-04-24 20:51:14.000000 uvx-2.0.0a3/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.0a3/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.0a3/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.0a3/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.0a3/src/venv.rs
--rw-rw-r--   0     1000     1000      749 2024-04-26 18:28:24.000000 uvx-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     2183 1970-01-01 00:00:00.000000 uvx-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 uvx-2.0.0a4/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a4/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a4/.gitignore
+-rw-rw-r--   0     1000     1000      242 2024-04-24 20:55:06.000000 uvx-2.0.0a4/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    86391 2024-04-26 18:39:46.000000 uvx-2.0.0a4/Cargo.lock
+-rw-rw-r--   0     1000     1000     1582 2024-04-24 21:12:17.000000 uvx-2.0.0a4/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.0a4/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a4/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.0a4/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.0a4/src/cli.rs
+-rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.0a4/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.0a4/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.0a4/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.0a4/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.0a4/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.0a4/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.0a4/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.0a4/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.0a4/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.0a4/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.0a4/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.0a4/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.0a4/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     2934 2024-04-24 20:42:03.000000 uvx-2.0.0a4/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.0a4/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.0a4/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.0a4/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.0a4/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.0a4/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.0a4/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.0a4/src/main.rs
+-rw-rw-r--   0     1000     1000     7501 2024-04-24 20:51:14.000000 uvx-2.0.0a4/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.0a4/src/pip.rs
+-rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.0a4/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.0a4/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.0a4/src/venv.rs
+-rw-rw-r--   0     1000     1000      819 2024-04-26 18:39:26.000000 uvx-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2058 1970-01-01 00:00:00.000000 uvx-2.0.0a4/PKG-INFO
```

### Comparing `uvx-2.0.0a3/Cargo.toml` & `uvx-2.0.0a4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.0-alpha3"
+version = "2.0.0-alpha4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.0a3/.gitignore` & `uvx-2.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/Cargo.lock` & `uvx-2.0.0a4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3084,15 +3084,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.0-alpha3"
+version = "2.0.0-alpha4"
 dependencies = [
  "anstyle",
  "async_http_range_reader",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
```

### Comparing `uvx-2.0.0a3/README.md` & `uvx-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/animate.rs` & `uvx-2.0.0a4/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/cli.rs` & `uvx-2.0.0a4/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/cmd.rs` & `uvx-2.0.0a4/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/completions.rs` & `uvx-2.0.0a4/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/ensurepath.rs` & `uvx-2.0.0a4/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/inject.rs` & `uvx-2.0.0a4/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/install.rs` & `uvx-2.0.0a4/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/list.rs` & `uvx-2.0.0a4/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/reinstall.rs` & `uvx-2.0.0a4/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/reinstall_all.rs` & `uvx-2.0.0a4/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/run.rs` & `uvx-2.0.0a4/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/runpip.rs` & `uvx-2.0.0a4/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/runpython.rs` & `uvx-2.0.0a4/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/runuv.rs` & `uvx-2.0.0a4/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/self_update.rs` & `uvx-2.0.0a4/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/uninject.rs` & `uvx-2.0.0a4/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/uninstall.rs` & `uvx-2.0.0a4/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/uninstall_all.rs` & `uvx-2.0.0a4/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/upgrade.rs` & `uvx-2.0.0a4/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/commands/upgrade_all.rs` & `uvx-2.0.0a4/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/helpers.rs` & `uvx-2.0.0a4/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/main.rs` & `uvx-2.0.0a4/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/metadata.rs` & `uvx-2.0.0a4/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/pip.rs` & `uvx-2.0.0a4/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/symlinks.rs` & `uvx-2.0.0a4/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/uv.rs` & `uvx-2.0.0a4/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/src/venv.rs` & `uvx-2.0.0a4/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a3/pyproject.toml` & `uvx-2.0.0a4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
-requires = ["maturin>=1.5,<2.0"]
+requires = [
+    "maturin>=1.5,<2.0",
+    # Add a fake dependency for unsupported platforms
+    "please-use-uvx-v1-on-this-platform; sys_platform != 'linux' or (platform_machine != 'x86_64' and platform_machine != 'aarch64')",
+]
 build-backend = "maturin"
 
 [project]
 name = "uvx"
 requires-python = ">=3.10"
 
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
-
     "Operating System :: POSIX :: Linux",
-
-#    "Architecture :: x86_64",
-#    "Architecture :: aarch64",
+    #    "Architecture :: x86_64",
+    #    "Architecture :: aarch64",
 
     "Development Status :: 4 - Beta",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
-    "uv",
-    "patchelf",
-
-    # Add a fake dependency for unsupported platforms
-    "please-use-uvx-v1-on-this-platform; sys_platform != 'linux' or (platform_machine != 'x86_64' and platform_machine != 'aarch64')"
+    "uv", # obviously
+    "pip", # self-update
+    "patchelf", # idk, but required
 ]
 
 
 [tool.maturin]
 bindings = "bin"
```

### Comparing `uvx-2.0.0a3/PKG-INFO` & `uvx-2.0.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.0a3
+Version: 2.0.0a4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
+Requires-Dist: pip
 Requires-Dist: patchelf
-Requires-Dist: please-use-uvx-v1-on-this-platform ; sys_platform != 'linux' or (platform_machine != 'x86_64' and platform_machine != 'aarch64')
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # uvx: pipx for uv
 
 Inspired by:
```

