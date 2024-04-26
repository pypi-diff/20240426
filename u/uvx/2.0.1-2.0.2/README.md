# Comparing `tmp/uvx-2.0.1.tar.gz` & `tmp/uvx-2.0.2.tar.gz`

## Comparing `uvx-2.0.1.tar` & `uvx-2.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.1/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.1/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.1/.gitignore
--rw-rw-r--   0     1000     1000      334 2024-04-26 20:38:53.000000 uvx-2.0.1/CHANGELOG.md
--rw-rw-r--   0     1000     1000    86384 2024-04-26 20:32:25.000000 uvx-2.0.1/Cargo.lock
--rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.1/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.1/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.1/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.1/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.1/src/cli.rs
--rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.1/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.1/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.1/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.1/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.1/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.1/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.1/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.1/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.1/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.1/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.1/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.1/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.1/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     2934 2024-04-24 20:42:03.000000 uvx-2.0.1/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.1/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.1/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.1/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.1/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.1/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.1/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.1/src/main.rs
--rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.1/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.1/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.1/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.1/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.1/src/venv.rs
--rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.2/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.2/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.2/.gitignore
+-rw-rw-r--   0     1000     1000      436 2024-04-26 20:42:41.000000 uvx-2.0.2/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    86384 2024-04-26 20:43:13.000000 uvx-2.0.2/Cargo.lock
+-rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.2/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.2/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.2/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.2/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.2/src/cli.rs
+-rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.2/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.2/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.2/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.2/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.2/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.2/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.2/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.2/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.2/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.2/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.2/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.2/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.2/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     2934 2024-04-26 20:41:57.000000 uvx-2.0.2/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.2/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.2/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.2/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.2/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.2/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.2/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.2/src/main.rs
+-rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.2/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.2/src/pip.rs
+-rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.2/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.2/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.2/src/venv.rs
+-rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.2/PKG-INFO
```

### Comparing `uvx-2.0.1/Cargo.toml` & `uvx-2.0.2/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.1"
+version = "2.0.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.1/.gitignore` & `uvx-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/Cargo.lock` & `uvx-2.0.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3084,15 +3084,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.1"
+version = "2.0.2"
 dependencies = [
  "anstyle",
  "async_http_range_reader",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
```

### Comparing `uvx-2.0.1/README.md` & `uvx-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/animate.rs` & `uvx-2.0.2/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/cli.rs` & `uvx-2.0.2/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/cmd.rs` & `uvx-2.0.2/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/completions.rs` & `uvx-2.0.2/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/ensurepath.rs` & `uvx-2.0.2/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/inject.rs` & `uvx-2.0.2/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/install.rs` & `uvx-2.0.2/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/list.rs` & `uvx-2.0.2/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/reinstall.rs` & `uvx-2.0.2/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/reinstall_all.rs` & `uvx-2.0.2/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/run.rs` & `uvx-2.0.2/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/runpip.rs` & `uvx-2.0.2/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/runpython.rs` & `uvx-2.0.2/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/runuv.rs` & `uvx-2.0.2/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/self_update.rs` & `uvx-2.0.2/src/commands/self_update.rs`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         AnimationSettings::default(),
     )
     .await?;
 
     let new = get_package_versions(&exe, &to_track).await;
 
     for (versions, package) in new.iter().zip(old.iter()).zip(to_track.iter()) {
-        let (before, after) = versions;
+        let (after, before) = versions;
         if before == after {
             println!(
                 "🌟 '{}' not updated (version: {})",
                 package.blue(),
                 before.green()
             )
         } else {
```

### Comparing `uvx-2.0.1/src/commands/uninject.rs` & `uvx-2.0.2/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/uninstall.rs` & `uvx-2.0.2/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/uninstall_all.rs` & `uvx-2.0.2/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/upgrade.rs` & `uvx-2.0.2/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/commands/upgrade_all.rs` & `uvx-2.0.2/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/helpers.rs` & `uvx-2.0.2/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/main.rs` & `uvx-2.0.2/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/metadata.rs` & `uvx-2.0.2/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/pip.rs` & `uvx-2.0.2/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/symlinks.rs` & `uvx-2.0.2/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/uv.rs` & `uvx-2.0.2/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/src/venv.rs` & `uvx-2.0.2/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/pyproject.toml` & `uvx-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.0.1/PKG-INFO` & `uvx-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.1
+Version: 2.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

