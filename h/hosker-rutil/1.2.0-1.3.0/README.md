# Comparing `tmp/hosker_rutil-1.2.0.tar.gz` & `tmp/hosker_rutil-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosker_rutil-1.2.0.tar", last modified: Wed Feb 28 20:22:40 2024, max compression
+gzip compressed data, was "hosker_rutil-1.3.0.tar", last modified: Fri Apr 26 18:38:00 2024, max compression
```

## Comparing `hosker_rutil-1.2.0.tar` & `hosker_rutil-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1050 2022-11-13 15:45:04.000000 hosker_rutil-1.2.0/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       95 2024-02-28 20:22:16.000000 hosker_rutil-1.2.0/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)      260 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1035 2024-02-28 20:13:43.000000 hosker_rutil-1.2.0/README.md
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/hosker_rutil.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)      260 2024-02-28 20:22:40.000000 hosker_rutil-1.2.0/hosker_rutil.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)      386 2024-02-28 20:22:40.000000 hosker_rutil-1.2.0/hosker_rutil.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-02-28 20:22:40.000000 hosker_rutil-1.2.0/hosker_rutil.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       19 2024-02-28 20:22:40.000000 hosker_rutil-1.2.0/hosker_rutil.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       13 2024-02-28 20:22:40.000000 hosker_rutil-1.2.0/hosker_rutil.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/scripts/
--rw-rw-r--   0 tom       (1000) tom       (1000)      598 2024-01-22 17:28:31.000000 hosker_rutil-1.2.0/scripts/hosker-rutil-install-specials
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/setup.cfg
--rw-rw-r--   0 tom       (1000) tom       (1000)      945 2024-02-28 20:22:36.000000 hosker_rutil-1.2.0/setup.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/source/
--rw-rw-r--   0 tom       (1000) tom       (1000)       95 2024-01-23 18:40:46.000000 hosker_rutil-1.2.0/source/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2801 2024-02-28 20:13:43.000000 hosker_rutil-1.2.0/source/primes.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.877847 hosker_rutil-1.2.0/source/rust/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/source/rust/hosker_primes/
--rw-rw-r--   0 tom       (1000) tom       (1000)      261 2024-02-28 20:13:43.000000 hosker_rutil-1.2.0/source/rust/hosker_primes/Cargo.toml
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-02-28 20:22:40.881847 hosker_rutil-1.2.0/source/rust/hosker_primes/src/
--rw-rw-r--   0 tom       (1000) tom       (1000)     3262 2024-02-28 20:13:43.000000 hosker_rutil-1.2.0/source/rust/hosker_primes/src/lib.rs
--rw-rw-r--   0 tom       (1000) tom       (1000)     3169 2024-02-28 20:13:43.000000 hosker_rutil-1.2.0/source/rust_utils.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1050 2022-11-13 15:45:04.000000 hosker_rutil-1.3.0/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       95 2024-02-28 20:22:16.000000 hosker_rutil-1.3.0/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)      260 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1398 2024-04-22 17:49:28.000000 hosker_rutil-1.3.0/README.md
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/hosker_rutil.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      260 2024-04-26 18:37:59.000000 hosker_rutil-1.3.0/hosker_rutil.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)      416 2024-04-26 18:37:59.000000 hosker_rutil-1.3.0/hosker_rutil.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2024-04-26 18:37:59.000000 hosker_rutil-1.3.0/hosker_rutil.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       19 2024-04-26 18:37:59.000000 hosker_rutil-1.3.0/hosker_rutil.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       13 2024-04-26 18:37:59.000000 hosker_rutil-1.3.0/hosker_rutil.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/scripts/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      351 2024-04-22 17:41:20.000000 hosker_rutil-1.3.0/scripts/hosker-rutil-compile-rust
+-rw-rw-r--   0 tom       (1000) tom       (1000)      327 2024-04-25 16:32:49.000000 hosker_rutil-1.3.0/scripts/hosker-rutil-install-rust
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/setup.cfg
+-rw-rw-r--   0 tom       (1000) tom       (1000)      987 2024-04-26 18:32:56.000000 hosker_rutil-1.3.0/setup.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/source/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      153 2024-04-26 18:33:50.000000 hosker_rutil-1.3.0/source/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3768 2024-04-26 18:35:17.000000 hosker_rutil-1.3.0/source/primes.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/source/rust/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/source/rust/hosker_primes/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      261 2024-04-25 17:35:09.000000 hosker_rutil-1.3.0/source/rust/hosker_primes/Cargo.toml
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2024-04-26 18:38:00.008196 hosker_rutil-1.3.0/source/rust/hosker_primes/src/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3369 2024-04-26 18:27:50.000000 hosker_rutil-1.3.0/source/rust/hosker_primes/src/lib.rs
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3169 2024-04-26 17:17:30.000000 hosker_rutil-1.3.0/source/rust_utils.py
```

### Comparing `hosker_rutil-1.2.0/LICENSE` & `hosker_rutil-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hosker_rutil-1.2.0/README.md` & `hosker_rutil-1.3.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # RUtil: Rust Utilities for Python
 
 This code defines a library of Rust functions, and a Python middleman from which to call those functions. It is modelled on the `shutil` module from the Python standard library.
 
 ## Installation
 
+Note that this package is designed for Debian-based Linux platforms only. Some portions of it may well work on other platforms, but you do so at your own risk.
+
 ### Installing the Python Code
 
 * If you're installing remotely, **`pip install hosker-rutil`** should do the trick.
 * If, on the other hand, you're installing locally, then use **`pip install .`** from this directory.
 
 ### Compiling the Rust Library
 
-By installing the PIP package as described above, you will also have installed the command `hosker-rutil-install-specials`. Running this command will compile the Rust libraries from their source code, as well as installing Cargo, if you don't have it already.
+By installing the PIP package as described above, you will also have installed the commands `hosker-rutil-install-rust` and `hosker-rutil-compile-rust`. Run `hosker-rutil-install-rust` first - this installs Cargo, but even if you already have Cargo installed it shouldn't do any harm - then run `hosker-rutil-compile-rust` - this compiles the Rust code into binaries which your machine can execute. Running those two commands completes the installation process.
 
 ## Examples
 
 ### Primes
 
 This code should find whether a nine-digit number is prime or not - and do so far quicker than anything in pure Python:
```

### Comparing `hosker_rutil-1.2.0/setup.py` & `hosker_rutil-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 """
 
 # Non-standard imports.
 from setuptools import setup
 
 # Local constants.
 PACKAGE_NAME = "hosker_rutil"
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 DESCRIPTION = "Rust utility functions"
 GIT_URL_STEM = "https://github.com/tomhosker"
 AUTHOR = "Tom Hosker"
 AUTHOR_EMAIL = "tomdothosker@gmail.com"
-SCRIPT_PATHS = ("scripts/hosker-rutil-install-specials",)
-INSTALL_REQUIRES = ("hosker_utils", "numpy")
+SCRIPT_PATHS = (
+    "scripts/hosker-rutil-install-rust",
+    "scripts/hosker-rutil-compile-rust"
+)
+INSTALL_REQUIRES = ("hosker_utils", "sympy")
 INCLUDE_PACKAGE_DATA = True
 
 ###################################
 # THIS IS WHERE THE MAGIC HAPPENS #
 ###################################
 
 setup(
```

### Comparing `hosker_rutil-1.2.0/source/rust/hosker_primes/src/lib.rs` & `hosker_rutil-1.3.0/source/rust/hosker_primes/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,54 @@
 /// This library defines some utility functions for working with primes.
 
 // Standard imports.
 use std::ffi::CString;
 
 // Non-standard imports.
 use libc::{c_char, c_void};
-use num_bigint::{BigInt, Sign};
-use num_integer::Integer;
-use num_iter;
-use primes;
+use num_bigint_dig::BigUint;
+use num_bigint_dig::prime::probably_prime as is_big_prime;
+use num_prime::nt_funcs::{
+    is_prime64 as is_little_prime,
+    nth_prime as _nth_prime
+};
 
 // Local constants.
 const MAX_DIGITS: usize = 100;
 const STANDARD_RADIX: u32 = 10;
+const PSEUDORANDOMLY_CHOSEN_BASES: usize = 32;
 const TRUE_INT: i32 = 1;
 const FALSE_INT: i32 = 0;
+const MAX_PRIME_ORDINAL_I32: i32 = 105097565;
 
 /***************************
  ** FOR INTERNAL USE ONLY **
  **************************/
 
 /// Determine whether an arbitrarily large integer is prime.
-fn _is_prime_bigint(potential_prime: BigInt) -> bool {
-println!("Received: {:?}", potential_prime);
-    if potential_prime == BigInt::from(2) {
-        return true;
-    }
-    if potential_prime.is_even() {
-        return false;
-    }
-
-    let max_potential_divisor = potential_prime.sqrt();
-
-    for potential_divisor in num_iter::range_inclusive(
-        BigInt::from(3), max_potential_divisor
-    ) {
-        if potential_prime.is_multiple_of(&potential_divisor) {
-            return false;
-        }
-    }
+fn _is_prime_bigint(potential_prime: BigUint) -> bool {
+    let result = is_big_prime(&potential_prime, PSEUDORANDOMLY_CHOSEN_BASES);
 
-    return true;
+    return result;
 }
 
 /***************
  ** MIDDLEMEN **
  **************/
 
 /// Receive a big integer from outside Rust.
-unsafe fn import_bigint(digit_list: PortableDigitList) -> BigInt {
+unsafe fn import_bigint(digit_list: PortableDigitList) -> BigUint {
     let digits = Vec::from(*digit_list.array);
-    let result = BigInt::new(Sign::Plus, digits);
+    let result = BigUint::new(digits);
 
     return result;
 }
 
 /// Convert a big integer into an exportable form outside Rust.
-fn export_bigint(n: BigInt) -> *mut c_char {
+fn export_bigint(n: BigUint) -> *mut c_char {
     let result_str = n.to_str_radix(STANDARD_RADIX);
     let result = CString::new(result_str).unwrap().into_raw();
 
     return result;
 }
 
 /// Convert a boolean into an integer representation of the same.
@@ -106,18 +94,32 @@
 pub unsafe extern fn free_string(pointer: *mut c_void) {
     let _ = CString::from_raw(pointer as *mut c_char);
 }
 
 /// A wrapper for the similarly-named function above.
 #[no_mangle]
 pub extern fn is_prime_i32(n: i32) -> i32 {
-    return bool_to_int(primes::is_prime(n.try_into().unwrap()));
+    return bool_to_int(is_little_prime(n.try_into().unwrap()));
 }
 
 /// A wrapper for the similarly-named function above.
 #[no_mangle]
 pub unsafe extern fn is_prime_bigint(digit_list: PortableDigitList) -> i32 {
-    let digits = Vec::from(*digit_list.array);
-    let big_integer = BigInt::new(Sign::Plus, digits);
+    let big_integer = import_bigint(digit_list);
 
     return bool_to_int(_is_prime_bigint(big_integer));
 }
+
+/// A wrapper for the similarly-named function above.
+#[no_mangle]
+pub extern fn nth_prime_i32(n: i32) -> i32 {
+    if n > MAX_PRIME_ORDINAL_I32 {
+        println!(
+            "WARNING: Prime with ordinal {} cannot be represented in 32 bits.", 
+            n
+        );
+
+        return 0;
+    }
+
+    return _nth_prime(n.try_into().unwrap()) as i32;
+}
```

### Comparing `hosker_rutil-1.2.0/source/rust_utils.py` & `hosker_rutil-1.3.0/source/rust_utils.py`

 * *Files identical despite different names*

