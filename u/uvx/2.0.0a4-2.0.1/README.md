# Comparing `tmp/uvx-2.0.0a4.tar.gz` & `tmp/uvx-2.0.1.tar.gz`

## Comparing `uvx-2.0.0a4.tar` & `uvx-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1438 1970-01-01 00:00:00.000000 uvx-2.0.0a4/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.0a4/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.0a4/.gitignore
--rw-rw-r--   0     1000     1000      242 2024-04-24 20:55:06.000000 uvx-2.0.0a4/CHANGELOG.md
--rw-rw-r--   0     1000     1000    86391 2024-04-26 18:39:46.000000 uvx-2.0.0a4/Cargo.lock
--rw-rw-r--   0     1000     1000     1582 2024-04-24 21:12:17.000000 uvx-2.0.0a4/README.md
--rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.0a4/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.0a4/rustfmt.toml
--rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.0a4/src/animate.rs
--rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.0a4/src/cli.rs
--rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.0a4/src/cmd.rs
--rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.0a4/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.0a4/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.0a4/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.0a4/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.0a4/src/commands/list.rs
--rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.0a4/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.0a4/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.0a4/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.0a4/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.0a4/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.0a4/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.0a4/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     2934 2024-04-24 20:42:03.000000 uvx-2.0.0a4/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.0a4/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.0a4/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.0a4/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.0a4/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.0a4/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.0a4/src/helpers.rs
--rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.0a4/src/main.rs
--rw-rw-r--   0     1000     1000     7501 2024-04-24 20:51:14.000000 uvx-2.0.0a4/src/metadata.rs
--rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.0a4/src/pip.rs
--rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.0a4/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.0a4/src/uv.rs
--rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.0a4/src/venv.rs
--rw-rw-r--   0     1000     1000      819 2024-04-26 18:39:26.000000 uvx-2.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     2058 1970-01-01 00:00:00.000000 uvx-2.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 uvx-2.0.1/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.0.1/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.0.1/.gitignore
+-rw-rw-r--   0     1000     1000      334 2024-04-26 20:38:53.000000 uvx-2.0.1/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    86384 2024-04-26 20:32:25.000000 uvx-2.0.1/Cargo.lock
+-rw-rw-r--   0     1000     1000     2203 2024-04-26 19:03:51.000000 uvx-2.0.1/README.md
+-rwxrwxr-x   0     1000     1000      235 2024-04-26 18:24:22.000000 uvx-2.0.1/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.0.1/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1821 2024-04-24 20:50:38.000000 uvx-2.0.1/src/animate.rs
+-rw-rw-r--   0     1000     1000     9727 2024-04-24 20:50:21.000000 uvx-2.0.1/src/cli.rs
+-rw-rw-r--   0     1000     1000     2253 2024-04-24 20:50:02.000000 uvx-2.0.1/src/cmd.rs
+-rw-rw-r--   0     1000     1000      618 2024-04-24 20:49:18.000000 uvx-2.0.1/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     2250 2024-04-24 20:49:13.000000 uvx-2.0.1/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1617 2024-04-24 20:48:26.000000 uvx-2.0.1/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5022 2024-04-24 20:48:10.000000 uvx-2.0.1/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2511 2024-04-24 20:45:17.000000 uvx-2.0.1/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      312 2024-04-15 19:40:37.000000 uvx-2.0.1/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2200 2024-04-24 20:43:02.000000 uvx-2.0.1/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1346 2024-04-24 20:41:37.000000 uvx-2.0.1/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4039 2024-04-24 20:42:18.000000 uvx-2.0.1/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.0.1/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1195 2024-04-24 20:39:49.000000 uvx-2.0.1/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.0.1/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     2934 2024-04-24 20:42:03.000000 uvx-2.0.1/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     1631 2024-04-24 20:35:19.000000 uvx-2.0.1/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2019 2024-04-24 20:34:30.000000 uvx-2.0.1/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000      948 2024-04-24 20:34:02.000000 uvx-2.0.1/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4054 2024-04-24 20:33:47.000000 uvx-2.0.1/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1021 2024-04-24 20:32:19.000000 uvx-2.0.1/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.0.1/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1026 2024-04-24 20:02:25.000000 uvx-2.0.1/src/main.rs
+-rw-rw-r--   0     1000     1000     8457 2024-04-26 20:37:12.000000 uvx-2.0.1/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4477 2024-04-24 20:41:56.000000 uvx-2.0.1/src/pip.rs
+-rw-rw-r--   0     1000     1000     3692 2024-04-24 20:26:38.000000 uvx-2.0.1/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3768 2024-04-24 20:51:25.000000 uvx-2.0.1/src/uv.rs
+-rw-rw-r--   0     1000     1000     2352 2024-04-24 20:51:25.000000 uvx-2.0.1/src/venv.rs
+-rw-rw-r--   0     1000     1000      819 2024-04-26 18:46:18.000000 uvx-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 uvx-2.0.1/PKG-INFO
```

### Comparing `uvx-2.0.0a4/Cargo.toml` & `uvx-2.0.1/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "uvx"
-version = "2.0.0-alpha4"
+version = "2.0.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 # [lib]
 # name = "uvx"
 # crate-type = ["cdylib"]
```

### Comparing `uvx-2.0.0a4/.gitignore` & `uvx-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/Cargo.lock` & `uvx-2.0.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3084,15 +3084,15 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.0.0-alpha4"
+version = "2.0.1"
 dependencies = [
  "anstyle",
  "async_http_range_reader",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
```

### Comparing `uvx-2.0.0a4/README.md` & `uvx-2.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,61 +3,75 @@
 Inspired by:
 
 - [pipx](https://github.com/pypa/pipx)
 - [uv](https://github.com/astral-sh/uv)
 
 ## Installation
 
-```bash
-# one of these ways:
-pip install uvx # or `uv`, `pipx`
-
-# optional (in bash):
-uvx ensurepath # make sure ~/.local/bin is in PATH
-uvx completions --install # enable tab completion
-```
-
-### Platforms
-
-Since `uvx 2.0`, this tool uses Rust for performance and compatibility with `uv`.
-Currently, only prebuilt binaries are available for x86_64 (amd64) and aarch64 (ARM64) on Linux.
-Other platforms can use `uvx 1.x`, which is written in pure Python and can be found
-at [robinvandernoord/uvx](https://github.com/robinvandernoord/uvx).
-You can also compile `uvx` for your own platform:
-
-```bash
-# install the rust toolchain:
-curl https://sh.rustup.rs -sSf | sh
-# clone the repo and enter it:
-git clone https://github.com/robinvandernoord/uvx2.git; 
-cd uvx2;
-# install a virtualenv (choose python or uv)
-python -m venv venv  # or `uv venv venv --seed`
-source venv/bin/activate
-
-# install maturin
-pip install maturin # uv pip install maturin
-
-# compile and install the binary:
-maturin develop
-
-# uvx is now available:
-./venv/bin/uvx
-```
-
-For more info about building and distribution, see [maturin](https://www.maturin.rs/distribution).
+1. Install via pip (or alternatives):
+    ```bash
+    pip install uvx  # or `uv`, `pipx`
+    ```
+
+2. Optional (for bash users):
+    - Ensure that `~/.local/bin` is in your PATH:
+        ```bash
+        uvx ensurepath
+        ```
+    - Enable tab completion for `uvx`:
+        ```bash
+        uvx completions --install
+        ```
 
 ## Usage
 
 ```bash
 uvx
 ```
 
 Run `uvx` without any arguments to see all possible subcommands.
 
+## Platform Considerations
+
+- **Rust-Powered Performance (uvx 2.0):** Starting from version 2.0, `uvx` leverages Rust for improved performance and
+  compatibility with `uv`.
+- **Prebuilt Binaries:** Currently, prebuilt binaries are available for x86_64 (amd64) and aarch64 (ARM64) on Linux.
+- **Other Platforms:** If you're on a different platform, you can still use `uvx 1.x`, which is written in pure Python.
+  Find it at [robinvandernoord/uvx](https://github.com/robinvandernoord/uvx).
+- Alternatively, you can **Compile for Your Platform**:
+    - Install the Rust toolchain:
+        ```bash
+        curl https://sh.rustup.rs -sSf | sh
+        ```
+    - Clone the `uvx2` repo and navigate to it:
+        ```bash
+        git clone https://github.com/robinvandernoord/uvx2.git
+        cd uvx2
+        ```
+    - Set up a virtual environment (choose Python or uv):
+        ```bash
+        python -m venv venv  # or `uv venv venv --seed`
+        source venv/bin/activate
+        ```
+    - Install Maturin (Python with Rust package builder):
+        ```bash
+        pip install maturin  # or `uv pip install maturin`
+        ```
+    - Compile and install the `uvx` binary:
+        ```bash
+        maturin develop
+        ```
+    - Now you can use `uvx`:
+        ```bash
+        ./venv/bin/uvx
+        ```
+
+For additional details on building and distribution, refer to [maturin](https://www.maturin.rs/distribution)
+documentation.
+
 ## License
 
 `uvx` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
 See `CHANGELOG.md` [on GitHub](https://github.com/robinvandernoord/uvx2/blob/master/CHANGELOG.md)
```

### Comparing `uvx-2.0.0a4/src/animate.rs` & `uvx-2.0.1/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/cli.rs` & `uvx-2.0.1/src/cli.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/cmd.rs` & `uvx-2.0.1/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/completions.rs` & `uvx-2.0.1/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/ensurepath.rs` & `uvx-2.0.1/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/inject.rs` & `uvx-2.0.1/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/install.rs` & `uvx-2.0.1/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/list.rs` & `uvx-2.0.1/src/commands/list.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/reinstall.rs` & `uvx-2.0.1/src/commands/reinstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/reinstall_all.rs` & `uvx-2.0.1/src/commands/reinstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/run.rs` & `uvx-2.0.1/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/runpip.rs` & `uvx-2.0.1/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/runpython.rs` & `uvx-2.0.1/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/runuv.rs` & `uvx-2.0.1/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/self_update.rs` & `uvx-2.0.1/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/uninject.rs` & `uvx-2.0.1/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/uninstall.rs` & `uvx-2.0.1/src/commands/uninstall.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/uninstall_all.rs` & `uvx-2.0.1/src/commands/uninstall_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/upgrade.rs` & `uvx-2.0.1/src/commands/upgrade.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/commands/upgrade_all.rs` & `uvx-2.0.1/src/commands/upgrade_all.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/helpers.rs` & `uvx-2.0.1/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/main.rs` & `uvx-2.0.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/metadata.rs` & `uvx-2.0.1/src/metadata.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 use tokio::io::AsyncWriteExt;
 use uv_interpreter::PythonEnvironment;
 
 const BIN_DIR: &str = ".local/bin";
 const WORK_DIR: &str = ".local/uvx";
 const INDENT: &str = "    ";
 
+// tells 'file' that a .metadata file is 'data' (instead of making it guess)
+//                           U     V     X    SOH  version(2)  STX (padding):
+const MAGIC_HEADER: &[u8] = &[0x55, 0x56, 0x58, 0x01, 0x32, 0x04, 0x00]; // hex, 7 bytes
+
 pub fn get_home_dir() -> PathBuf {
     home::home_dir().expect("Failed to get home directory")
 }
 
 pub fn get_bin_dir() -> PathBuf {
     let home_dir = get_home_dir();
     home_dir.join(BIN_DIR)
@@ -239,24 +243,44 @@
             .join(" | ");
         result.push_str(&format!("{}Scripts: {}", INDENT, formatted_scripts));
 
         result
     }
 }
 
+/// Drop the MAGIC_HEADER from a buffer (if present)
+pub fn strip_header(buf: &mut Vec<u8>) {
+    // postponed: the current header is 7 chars long.
+    //            the version should be ignored for starts_with,
+    //            and if the length should change, this must be 'match'ed based on the version
+    if buf.starts_with(MAGIC_HEADER) {
+        let _ = buf.drain(0..MAGIC_HEADER.len());
+    }
+}
+
+/// Prepend the MAGIC_HEADER to a buffer
+fn add_header(buf: &mut Vec<u8>) {
+    let mut new_buf = Vec::with_capacity(MAGIC_HEADER.len() + buf.len());
+    new_buf.extend_from_slice(MAGIC_HEADER);
+    new_buf.append(buf);
+    *buf = new_buf;
+}
+
 pub async fn load_metadata(
     filename: &Path,
     recheck_scripts: bool,
 ) -> Result<Metadata, String> {
     // Open the msgpack file
     let mut file = File::open(filename).await.map_err_to_string()?;
 
     let mut buf = Vec::new();
     file.read_to_end(&mut buf).await.map_err_to_string()?;
 
+    strip_header(&mut buf);
+
     // Read the contents of the file into a Metadata struct
     let mut metadata: Metadata = rmp_serde::decode::from_slice(&buf[..]).map_err_to_string()?;
 
     if recheck_scripts {
         if let Some(folder) = filename.parent() {
             metadata.check_scripts(folder).await
         }
@@ -269,13 +293,15 @@
     filename: &Path,
     metadata: &Metadata,
 ) -> Result<(), String> {
     // Open the msgpack file
     let mut file = File::create(filename).await.map_err_to_string()?;
 
     // Read the contents of the file into a Metadata struct
-    let bytes = rmp_serde::encode::to_vec(metadata).map_err_to_string()?;
+    let mut bytes = rmp_serde::encode::to_vec(metadata).map_err_to_string()?;
+
+    add_header(&mut bytes);
 
     file.write_all(&bytes).await.map_err_to_string()?;
 
     Ok(())
 }
```

### Comparing `uvx-2.0.0a4/src/pip.rs` & `uvx-2.0.1/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/symlinks.rs` & `uvx-2.0.1/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/uv.rs` & `uvx-2.0.1/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/src/venv.rs` & `uvx-2.0.1/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/pyproject.toml` & `uvx-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.0.0a4/PKG-INFO` & `uvx-2.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.0.0a4
+Version: 2.0.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
@@ -17,61 +17,75 @@
 Inspired by:
 
 - [pipx](https://github.com/pypa/pipx)
 - [uv](https://github.com/astral-sh/uv)
 
 ## Installation
 
-```bash
-# one of these ways:
-pip install uvx # or `uv`, `pipx`
-
-# optional (in bash):
-uvx ensurepath # make sure ~/.local/bin is in PATH
-uvx completions --install # enable tab completion
-```
-
-### Platforms
-
-Since `uvx 2.0`, this tool uses Rust for performance and compatibility with `uv`.
-Currently, only prebuilt binaries are available for x86_64 (amd64) and aarch64 (ARM64) on Linux.
-Other platforms can use `uvx 1.x`, which is written in pure Python and can be found
-at [robinvandernoord/uvx](https://github.com/robinvandernoord/uvx).
-You can also compile `uvx` for your own platform:
-
-```bash
-# install the rust toolchain:
-curl https://sh.rustup.rs -sSf | sh
-# clone the repo and enter it:
-git clone https://github.com/robinvandernoord/uvx2.git; 
-cd uvx2;
-# install a virtualenv (choose python or uv)
-python -m venv venv  # or `uv venv venv --seed`
-source venv/bin/activate
-
-# install maturin
-pip install maturin # uv pip install maturin
-
-# compile and install the binary:
-maturin develop
-
-# uvx is now available:
-./venv/bin/uvx
-```
-
-For more info about building and distribution, see [maturin](https://www.maturin.rs/distribution).
+1. Install via pip (or alternatives):
+    ```bash
+    pip install uvx  # or `uv`, `pipx`
+    ```
+
+2. Optional (for bash users):
+    - Ensure that `~/.local/bin` is in your PATH:
+        ```bash
+        uvx ensurepath
+        ```
+    - Enable tab completion for `uvx`:
+        ```bash
+        uvx completions --install
+        ```
 
 ## Usage
 
 ```bash
 uvx
 ```
 
 Run `uvx` without any arguments to see all possible subcommands.
 
+## Platform Considerations
+
+- **Rust-Powered Performance (uvx 2.0):** Starting from version 2.0, `uvx` leverages Rust for improved performance and
+  compatibility with `uv`.
+- **Prebuilt Binaries:** Currently, prebuilt binaries are available for x86_64 (amd64) and aarch64 (ARM64) on Linux.
+- **Other Platforms:** If you're on a different platform, you can still use `uvx 1.x`, which is written in pure Python.
+  Find it at [robinvandernoord/uvx](https://github.com/robinvandernoord/uvx).
+- Alternatively, you can **Compile for Your Platform**:
+    - Install the Rust toolchain:
+        ```bash
+        curl https://sh.rustup.rs -sSf | sh
+        ```
+    - Clone the `uvx2` repo and navigate to it:
+        ```bash
+        git clone https://github.com/robinvandernoord/uvx2.git
+        cd uvx2
+        ```
+    - Set up a virtual environment (choose Python or uv):
+        ```bash
+        python -m venv venv  # or `uv venv venv --seed`
+        source venv/bin/activate
+        ```
+    - Install Maturin (Python with Rust package builder):
+        ```bash
+        pip install maturin  # or `uv pip install maturin`
+        ```
+    - Compile and install the `uvx` binary:
+        ```bash
+        maturin develop
+        ```
+    - Now you can use `uvx`:
+        ```bash
+        ./venv/bin/uvx
+        ```
+
+For additional details on building and distribution, refer to [maturin](https://www.maturin.rs/distribution)
+documentation.
+
 ## License
 
 `uvx` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
 
 ## Changelog
 
 See `CHANGELOG.md` [on GitHub](https://github.com/robinvandernoord/uvx2/blob/master/CHANGELOG.md)
```

