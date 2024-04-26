# Comparing `tmp/uvx-2.0.2.tar.gz` & `tmp/uvx-2.0.3.tar.gz`

## Comparing `uvx-2.0.2.tar` & `uvx-2.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.2/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.2/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.2/.gitignore
--rw-rw-r--   0     1000     1000      436 2024-04-26 20:42:41.000000 uvx-2.0.2/CHANGELOG.md
--rw-rw-r--   0     1000     1000    86384 2024-04-26 20:43:13.000000 uvx-2.0.2/Cargo.lock
--rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.2/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.2/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.2/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.2/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.2/src/cli.rs
--rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.2/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.2/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.2/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.2/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.2/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.2/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.2/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.2/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.2/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.2/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.2/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.2/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.2/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     2934 2024-04-26 20:41:57.000000 uvx-2.0.2/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.2/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.2/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.2/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.2/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.2/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.2/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.2/src/main.rs
--rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.2/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.2/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.2/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.2/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.2/src/venv.rs
--rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.3/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.3/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.3/.gitignore
+-rw-rw-r--   0     1000     1000      558 2024-04-26 20:59:05.000000 uvx-2.0.3/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    86384 2024-04-26 20:59:17.000000 uvx-2.0.3/Cargo.lock
+-rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.3/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.3/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.3/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.3/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.3/src/cli.rs
+-rw-rw-r--   0     1000     1000     2314 2024-04-26 20:57:40.000000 uvx-2.0.3/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.3/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.3/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.3/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.3/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.3/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.3/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.3/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.3/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.3/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.3/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.3/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.3/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3192 2024-04-26 20:57:17.000000 uvx-2.0.3/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.3/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.3/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.3/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.3/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.3/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.3/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.3/src/main.rs
+-rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.3/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.3/src/pip.rs
+-rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.3/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.3/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.3/src/venv.rs
+-rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.3/PKG-INFO
```

### Comparing `uvx-2.0.2/Cargo.toml` & `uvx-2.0.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.2"
+version = "2.0.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.2/.gitignore` & `uvx-2.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/Cargo.lock` & `uvx-2.0.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3084,15 +3084,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.2"
+version = "2.0.3"
 dependencies = [
  "anstyle",
  "async_http_range_reader",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
```

### Comparing `uvx-2.0.2/README.md` & `uvx-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/animate.rs` & `uvx-2.0.3/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/cli.rs` & `uvx-2.0.3/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/cmd.rs` & `uvx-2.0.3/src/cmd.rs`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,19 @@
     };
 
     let parent = real_path.parent()?;
     // resolve symlinks etc:
 
     let binary = parent.join(name);
 
-    Some(binary)
+    if binary.exists() {
+        Some(binary)
+    } else {
+        None
+    }
 }
 
 pub async fn run_print_output<S1: AsRef<OsStr>, S2: AsRef<OsStr>>(
     command: S1,
     args: Vec<S2>,
 ) -> Result<i32, String> {
     let mut cmd = Command::new(command);
```

### Comparing `uvx-2.0.2/src/commands/completions.rs` & `uvx-2.0.3/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/ensurepath.rs` & `uvx-2.0.3/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/inject.rs` & `uvx-2.0.3/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/install.rs` & `uvx-2.0.3/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/list.rs` & `uvx-2.0.3/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/reinstall.rs` & `uvx-2.0.3/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/reinstall_all.rs` & `uvx-2.0.3/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/run.rs` & `uvx-2.0.3/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/runpip.rs` & `uvx-2.0.3/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/runpython.rs` & `uvx-2.0.3/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/runuv.rs` & `uvx-2.0.3/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/self_update.rs` & `uvx-2.0.3/src/commands/self_update.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::path::Path;
+use std::path::{Path, PathBuf};
 
 use owo_colors::OwoColorize;
 use regex::Regex;
 
 use crate::animate::{show_loading_indicator, AnimationSettings};
 use crate::cli::{Process, SelfUpdateOptions};
 use crate::cmd::{find_sibling, run};
@@ -47,19 +47,27 @@
     packages
         .iter()
         .map(|k| extract_version(&output, k.as_ref()).unwrap_or_default())
         .collect()
 }
 
 pub async fn self_update(with_uv: bool) -> Result<i32, String> {
-    let Some(exe) = find_sibling("python").await else {
-        return Err(format!(
-            "Python could not be found! Is `{}` installed globally (without a venv)?",
-            "uvx".green()
-        ));
+    let exe = match find_sibling("python").await {
+        Some(sibling) => sibling,
+        None => {
+            let fallback = PathBuf::from("/usr/bin/python3");
+            if fallback.exists() {
+                fallback
+            } else {
+                return Err(format!(
+                    "Python could not be found! Is `{}` installed globally (without a venv)?",
+                    "uvx".green()
+                ));
+            }
+        },
     };
 
     // todo: with 'uv' instead of pip later?
     let mut args = vec!["-m", "pip", "install", "--no-cache-dir", "--upgrade", "uvx"];
 
     let mut to_track = vec!["uvx"];
     let mut msg = String::from("uvx");
```

### Comparing `uvx-2.0.2/src/commands/uninject.rs` & `uvx-2.0.3/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/uninstall.rs` & `uvx-2.0.3/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/uninstall_all.rs` & `uvx-2.0.3/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/upgrade.rs` & `uvx-2.0.3/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/commands/upgrade_all.rs` & `uvx-2.0.3/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/helpers.rs` & `uvx-2.0.3/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/main.rs` & `uvx-2.0.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/metadata.rs` & `uvx-2.0.3/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/pip.rs` & `uvx-2.0.3/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/symlinks.rs` & `uvx-2.0.3/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/uv.rs` & `uvx-2.0.3/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/src/venv.rs` & `uvx-2.0.3/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/pyproject.toml` & `uvx-2.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.0.2/PKG-INFO` & `uvx-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.2
+Version: 2.0.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

