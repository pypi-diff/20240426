# Comparing `tmp/badkeys-0.0.7.tar.gz` & `tmp/badkeys-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badkeys-0.0.7.tar", last modified: Sat Apr 20 20:01:14 2024, max compression
+gzip compressed data, was "badkeys-0.0.8.tar", last modified: Fri Apr 26 13:22:35 2024, max compression
```

## Comparing `badkeys-0.0.7.tar` & `badkeys-0.0.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.803102 badkeys-0.0.7/
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.796102 badkeys-0.0.7/.github/
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.797102 badkeys-0.0.7/.github/workflows/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      574 2024-04-20 19:16:48.000000 badkeys-0.0.7/.github/workflows/codeql.yml
--rw-r--r--   0 hanno     (1000) hanno     (1000)      924 2024-04-20 19:16:48.000000 badkeys-0.0.7/.github/workflows/runci.yml
--rw-r--r--   0 hanno     (1000) hanno     (1000)       58 2024-04-20 19:16:48.000000 badkeys-0.0.7/.gitignore
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1138 2024-04-20 19:16:48.000000 badkeys-0.0.7/LICENSE
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3206 2024-04-20 20:01:14.803102 badkeys-0.0.7/PKG-INFO
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2144 2024-04-20 19:16:48.000000 badkeys-0.0.7/README.md
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.798102 badkeys-0.0.7/badkeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      362 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/__init__.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.798102 badkeys-0.0.7/badkeys/allkeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      105 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/allkeys/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3324 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/allkeys/block.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     7989 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/checks.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.799102 badkeys-0.0.7/badkeys/keydata/
--rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)   255328 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/primes1024.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)    78961 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/primes2048.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)      770 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/primes4096.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)    11449 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/primes512.dat
--rw-r--r--   0 hanno     (1000) hanno     (1000)      434 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/keydata/primes768.dat
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.800102 badkeys-0.0.7/badkeys/rsakeys/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      358 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/__init__.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      587 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/fermat.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      211 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/pattern.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1046 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/roca.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      289 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/rsainvalid.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      720 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/sharedprimes.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      599 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/smallfactors.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      533 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/rsakeys/xzbackdoor.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     7216 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/runcli.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1083 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/scanssh.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      371 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/scantls.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2573 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys/update.py
--rwxr-xr-x   0 hanno     (1000) hanno     (1000)       68 2024-04-20 19:16:48.000000 badkeys-0.0.7/badkeys-cli
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.802101 badkeys-0.0.7/badkeys.egg-info/
--rw-r--r--   0 hanno     (1000) hanno     (1000)     3206 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/PKG-INFO
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1582 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/SOURCES.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)        1 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/dependency_links.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)       50 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/entry_points.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)       67 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/requires.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)        8 2024-04-20 20:01:14.000000 badkeys-0.0.7/badkeys.egg-info/top_level.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1114 2024-04-20 19:54:55.000000 badkeys-0.0.7/pyproject.toml
--rw-r--r--   0 hanno     (1000) hanno     (1000)       19 2024-04-20 19:16:48.000000 badkeys-0.0.7/requirements.txt
--rwxr-xr-x   0 hanno     (1000) hanno     (1000)      347 2024-04-20 19:16:48.000000 badkeys-0.0.7/runci.sh
--rw-r--r--   0 hanno     (1000) hanno     (1000)       38 2024-04-20 20:01:14.803102 badkeys-0.0.7/setup.cfg
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.801102 badkeys-0.0.7/tests/
--rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/__init__.py
-drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-20 20:01:14.802101 badkeys-0.0.7/tests/data/
--rw-r--r--   0 hanno     (1000) hanno     (1000)      206 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/ec-p256-rfc-example.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      149 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/ed25519-rfc-example.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      531 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-debianweak.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      453 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-e1.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      513 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-fermat-hexmodulus.txt
--rw-r--r--   0 hanno     (1000) hanno     (1000)      502 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-fermat-pkcs1.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      498 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-fermat-pkcs8.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)     1153 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-fermat.crt
--rw-r--r--   0 hanno     (1000) hanno     (1000)      935 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-fermat.csr
--rw-r--r--   0 hanno     (1000) hanno     (1000)      457 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-nprime.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      464 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-ok.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-pattern.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      426 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-roca.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      508 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-sharedprimes.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      491 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/rsa-smallfactors.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      146 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/data/x448-ok.key
--rw-r--r--   0 hanno     (1000) hanno     (1000)      771 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_ecbl.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      620 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_failures.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)     2090 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_fermat.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      560 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_pattern.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      545 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_roca.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      568 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_rsabl.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      921 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_rsainvalid.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_sharedprimes.py
--rw-r--r--   0 hanno     (1000) hanno     (1000)      591 2024-04-20 19:16:48.000000 badkeys-0.0.7/tests/test_smallprimes.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.418523 badkeys-0.0.8/
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.406524 badkeys-0.0.8/.github/
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.408523 badkeys-0.0.8/.github/workflows/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      574 2024-04-25 16:20:20.000000 badkeys-0.0.8/.github/workflows/codeql.yml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      924 2024-04-25 16:20:20.000000 badkeys-0.0.8/.github/workflows/runci.yml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       58 2024-04-25 16:20:20.000000 badkeys-0.0.8/.gitignore
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1138 2024-04-25 16:20:20.000000 badkeys-0.0.8/LICENSE
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3627 2024-04-26 13:22:35.417523 badkeys-0.0.8/PKG-INFO
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2565 2024-04-26 06:48:07.000000 badkeys-0.0.8/README.md
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.409524 badkeys-0.0.8/badkeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      362 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/__init__.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.410524 badkeys-0.0.8/badkeys/allkeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      105 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/allkeys/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3324 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/allkeys/block.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     7989 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/checks.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.412524 badkeys-0.0.8/badkeys/keydata/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)   255328 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes1024.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)    78961 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes2048.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      770 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes4096.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)    11449 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes512.dat
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      434 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/keydata/primes768.dat
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.413524 badkeys-0.0.8/badkeys/rsakeys/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      358 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/__init__.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      587 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/fermat.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      211 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/pattern.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1046 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/roca.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      192 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/rsainvalid.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      720 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/sharedprimes.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      599 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/smallfactors.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      533 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/rsakeys/xzbackdoor.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     7216 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/runcli.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1222 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/scanssh.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      380 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/scantls.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2573 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys/update.py
+-rwxr-xr-x   0 hanno     (1000) hanno     (1000)       68 2024-04-25 16:20:20.000000 badkeys-0.0.8/badkeys-cli
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.417523 badkeys-0.0.8/badkeys.egg-info/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     3627 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/PKG-INFO
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1582 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/SOURCES.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        1 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/dependency_links.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       50 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/entry_points.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       67 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/requires.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        8 2024-04-26 13:22:35.000000 badkeys-0.0.8/badkeys.egg-info/top_level.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1114 2024-04-26 13:16:19.000000 badkeys-0.0.8/pyproject.toml
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       19 2024-04-25 16:20:20.000000 badkeys-0.0.8/requirements.txt
+-rwxr-xr-x   0 hanno     (1000) hanno     (1000)      363 2024-04-26 06:39:03.000000 badkeys-0.0.8/runci.sh
+-rw-r--r--   0 hanno     (1000) hanno     (1000)       38 2024-04-26 13:22:35.418523 badkeys-0.0.8/setup.cfg
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.414523 badkeys-0.0.8/tests/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)        0 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/__init__.py
+drwxr-xr-x   0 hanno     (1000) hanno     (1000)        0 2024-04-26 13:22:35.416524 badkeys-0.0.8/tests/data/
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      206 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/ec-p256-rfc-example.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      149 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/ed25519-rfc-example.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      531 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-debianweak.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      453 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-e1.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      513 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-hexmodulus.txt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      502 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-pkcs1.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      498 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat-pkcs8.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     1153 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat.crt
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      935 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-fermat.csr
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      457 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-nprime.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      464 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-ok.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-pattern.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      426 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-roca.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      508 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-sharedprimes.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      491 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/rsa-smallfactors.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      146 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/data/x448-ok.key
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      857 2024-04-25 16:23:00.000000 badkeys-0.0.8/tests/test_ecbl.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      620 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_failures.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)     2090 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_fermat.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      560 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_pattern.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      545 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_roca.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      654 2024-04-25 16:22:54.000000 badkeys-0.0.8/tests/test_rsabl.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      651 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_rsainvalid.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      593 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_sharedprimes.py
+-rw-r--r--   0 hanno     (1000) hanno     (1000)      591 2024-04-25 16:20:20.000000 badkeys-0.0.8/tests/test_smallprimes.py
```

### Comparing `badkeys-0.0.7/.github/workflows/codeql.yml` & `badkeys-0.0.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/.github/workflows/runci.yml` & `badkeys-0.0.8/.github/workflows/runci.yml`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/LICENSE` & `badkeys-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/PKG-INFO` & `badkeys-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badkeys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Check cryptographic keys for known weaknesses
 Author: Hanno Böck
 License: MIT
 Project-URL: Homepage, https://badkeys.info/
 Project-URL: Source, https://github.com/badkeys/badkeys
 Project-URL: Bug Tracker, https://github.com/badkeys/badkeys/issues
 Keywords: security,cryptography,rsa
@@ -29,68 +29,77 @@
 
 # badkeys
 
 Tool and library to check cryptographic public keys for known vulnerabilities
 
 # what?
 
-badkeys checks public keys in a variety of formats for known vulnerabilities. A web
-version can be found at [badkeys.info](https://badkeys.info/).
+badkeys checks public keys in various formats for known vulnerabilities. A web version
+can be found at [badkeys.info](https://badkeys.info/).
 
 # install
 
 badkeys can be installed [via pip](https://pypi.org/project/badkeys/):
 ```
 pip3 install badkeys
 ```
 
-Alternatively you can call _./badkeys-cli_ directly from the git repository.
+Alternatively, you can call _./badkeys-cli_ directly from the git repository.
 
 # usage
 
-Before using badkeys you need to download the blocklist data:
+Before using badkeys, you need to download the blocklist data:
 ```
 badkeys --update-bl
 ```
 
-After that you can call _badkeys_ and pass files with cryptographic public keys as the
+After that, you can call _badkeys_ and pass files with cryptographic public keys as the
 parameter:
 ```
 badkeys test.crt my.key
 ```
 
 It will automatically try to detect the file format. Supported are public and private
 keys in PEM format (both PKCS #1 and PKCS #8), X.509 certificates, certificate signing
 requests (CSRs) and SSH public keys. You can find some test keys in the _tests/data_
 directory.
 
-By default badkeys will only output information about vulnerable keys, meaning there
-will be no output if no vulnerabilities are found. The _-a_ parameter creates output for
-all keys.
+By default, badkeys will only output information about vulnerable keys, meaning no
+output will be generated if no vulnerabilities are found. The _-a_ parameter creates
+output for all keys.
 
 # scanning
 
-badkeys can directly scan SSH and TLS hosts and automatically check their public keys.
-This can be enabled with the parameters _-s_ (for SSH) and _-t_ (for TLS). By default
-SSH will be scanned on port 22 and TLS will be scanned on several ports for common
-protocols (https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443,
-which is commonly used as a non-standard https port).
+badkeys can scan SSH and TLS hosts and automatically check their public keys. This can
+be enabled with the parameters _-s_ (SSH) and _-t_ (TLS). By default, SSH will be
+scanned on port 22 and TLS will be scanned on several ports for common protocols
+(https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443, which is
+commonly used as a non-standard https port).
 
 Alternative ports can be configured with _--tls-ports_ and _--ssh-ports_.
 
 TLS and SSH scanning can be combined:
 ```
 badkeys -ts example.org
 ```
 
+Note that the scanning modes have limitations. It is often more desirable to use other
+tools to collect TLS/SSH keys and scan them locally with badkeys.
+
+SSH scanning needs [paramiko](https://www.paramiko.org/) as an additional dependency.
+
+TLS scanning can't detect multiple certificates on one host (e.g. ECDSA and RSA). This
+is a [limitation of Python's ssl.get_server_certificate() function](
+https://bugs.python.org/issue31892).
+
 # Python module and API
 
-badkeys can also be used as a Python module. However currently the software is in alpha
+badkeys can also be used as a Python module. However, currently the software is in beta
 state and the API may change regularly.
 
 # about
 
 badkeys was written by [Hanno Böck](https://hboeck.de).
 
-This work was originally funded in 2022 by Industriens Fond through the CIDI project
+This work was initially funded in 2022 by Industriens Fond through the CIDI project
 (Cybersecure IOT in Danish Industry) and the [Center for Information Security and Trust
 (CISAT)](https://cisat.dk/) at the IT University of Copenhagen, Denmark.
```

### Comparing `badkeys-0.0.7/README.md` & `badkeys-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,67 +1,76 @@
 # badkeys
 
 Tool and library to check cryptographic public keys for known vulnerabilities
 
 # what?
 
-badkeys checks public keys in a variety of formats for known vulnerabilities. A web
-version can be found at [badkeys.info](https://badkeys.info/).
+badkeys checks public keys in various formats for known vulnerabilities. A web version
+can be found at [badkeys.info](https://badkeys.info/).
 
 # install
 
 badkeys can be installed [via pip](https://pypi.org/project/badkeys/):
 ```
 pip3 install badkeys
 ```
 
-Alternatively you can call _./badkeys-cli_ directly from the git repository.
+Alternatively, you can call _./badkeys-cli_ directly from the git repository.
 
 # usage
 
-Before using badkeys you need to download the blocklist data:
+Before using badkeys, you need to download the blocklist data:
 ```
 badkeys --update-bl
 ```
 
-After that you can call _badkeys_ and pass files with cryptographic public keys as the
+After that, you can call _badkeys_ and pass files with cryptographic public keys as the
 parameter:
 ```
 badkeys test.crt my.key
 ```
 
 It will automatically try to detect the file format. Supported are public and private
 keys in PEM format (both PKCS #1 and PKCS #8), X.509 certificates, certificate signing
 requests (CSRs) and SSH public keys. You can find some test keys in the _tests/data_
 directory.
 
-By default badkeys will only output information about vulnerable keys, meaning there
-will be no output if no vulnerabilities are found. The _-a_ parameter creates output for
-all keys.
+By default, badkeys will only output information about vulnerable keys, meaning no
+output will be generated if no vulnerabilities are found. The _-a_ parameter creates
+output for all keys.
 
 # scanning
 
-badkeys can directly scan SSH and TLS hosts and automatically check their public keys.
-This can be enabled with the parameters _-s_ (for SSH) and _-t_ (for TLS). By default
-SSH will be scanned on port 22 and TLS will be scanned on several ports for common
-protocols (https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443,
-which is commonly used as a non-standard https port).
+badkeys can scan SSH and TLS hosts and automatically check their public keys. This can
+be enabled with the parameters _-s_ (SSH) and _-t_ (TLS). By default, SSH will be
+scanned on port 22 and TLS will be scanned on several ports for common protocols
+(https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443, which is
+commonly used as a non-standard https port).
 
 Alternative ports can be configured with _--tls-ports_ and _--ssh-ports_.
 
 TLS and SSH scanning can be combined:
 ```
 badkeys -ts example.org
 ```
 
+Note that the scanning modes have limitations. It is often more desirable to use other
+tools to collect TLS/SSH keys and scan them locally with badkeys.
+
+SSH scanning needs [paramiko](https://www.paramiko.org/) as an additional dependency.
+
+TLS scanning can't detect multiple certificates on one host (e.g. ECDSA and RSA). This
+is a [limitation of Python's ssl.get_server_certificate() function](
+https://bugs.python.org/issue31892).
+
 # Python module and API
 
-badkeys can also be used as a Python module. However currently the software is in alpha
+badkeys can also be used as a Python module. However, currently the software is in beta
 state and the API may change regularly.
 
 # about
 
 badkeys was written by [Hanno Böck](https://hboeck.de).
 
-This work was originally funded in 2022 by Industriens Fond through the CIDI project
+This work was initially funded in 2022 by Industriens Fond through the CIDI project
 (Cybersecure IOT in Danish Industry) and the [Center for Information Security and Trust
 (CISAT)](https://cisat.dk/) at the IT University of Copenhagen, Denmark.
```

### Comparing `badkeys-0.0.7/badkeys/allkeys/block.py` & `badkeys-0.0.8/badkeys/allkeys/block.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/checks.py` & `badkeys-0.0.8/badkeys/checks.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/keydata/primes1024.dat` & `badkeys-0.0.8/badkeys/keydata/primes1024.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/keydata/primes2048.dat` & `badkeys-0.0.8/badkeys/keydata/primes2048.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/keydata/primes4096.dat` & `badkeys-0.0.8/badkeys/keydata/primes4096.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/keydata/primes512.dat` & `badkeys-0.0.8/badkeys/keydata/primes512.dat`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/rsakeys/fermat.py` & `badkeys-0.0.8/badkeys/rsakeys/fermat.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/rsakeys/roca.py` & `badkeys-0.0.8/badkeys/rsakeys/roca.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/rsakeys/sharedprimes.py` & `badkeys-0.0.8/badkeys/rsakeys/sharedprimes.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/rsakeys/smallfactors.py` & `badkeys-0.0.8/badkeys/rsakeys/smallfactors.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/rsakeys/xzbackdoor.py` & `badkeys-0.0.8/badkeys/rsakeys/xzbackdoor.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/runcli.py` & `badkeys-0.0.8/badkeys/runcli.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys/scanssh.py` & `badkeys-0.0.8/badkeys/scanssh.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import contextlib
 import io
+import sys
 
 from .checks import checksshpubkey, allchecks
 
 
 def scanssh(host, port=22, checks=allchecks.keys()):
-    import paramiko
+    try:
+        import paramiko
+    except ModuleNotFoundError:
+        sys.stderr.write("ERROR: SSH scanning needs paramiko\n")
+        return []
 
     allkeytypes = paramiko.Transport._preferred_keys
 
     keys = []
     for keytype in ["rsa", "dss", "ecdsa", "ed25519"]:
         try:
             xnot = [x for x in allkeytypes if keytype not in x]
```

### Comparing `badkeys-0.0.7/badkeys/update.py` & `badkeys-0.0.8/badkeys/update.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/badkeys.egg-info/PKG-INFO` & `badkeys-0.0.8/badkeys.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badkeys
-Version: 0.0.7
+Version: 0.0.8
 Summary: Check cryptographic keys for known weaknesses
 Author: Hanno Böck
 License: MIT
 Project-URL: Homepage, https://badkeys.info/
 Project-URL: Source, https://github.com/badkeys/badkeys
 Project-URL: Bug Tracker, https://github.com/badkeys/badkeys/issues
 Keywords: security,cryptography,rsa
@@ -29,68 +29,77 @@
 
 # badkeys
 
 Tool and library to check cryptographic public keys for known vulnerabilities
 
 # what?
 
-badkeys checks public keys in a variety of formats for known vulnerabilities. A web
-version can be found at [badkeys.info](https://badkeys.info/).
+badkeys checks public keys in various formats for known vulnerabilities. A web version
+can be found at [badkeys.info](https://badkeys.info/).
 
 # install
 
 badkeys can be installed [via pip](https://pypi.org/project/badkeys/):
 ```
 pip3 install badkeys
 ```
 
-Alternatively you can call _./badkeys-cli_ directly from the git repository.
+Alternatively, you can call _./badkeys-cli_ directly from the git repository.
 
 # usage
 
-Before using badkeys you need to download the blocklist data:
+Before using badkeys, you need to download the blocklist data:
 ```
 badkeys --update-bl
 ```
 
-After that you can call _badkeys_ and pass files with cryptographic public keys as the
+After that, you can call _badkeys_ and pass files with cryptographic public keys as the
 parameter:
 ```
 badkeys test.crt my.key
 ```
 
 It will automatically try to detect the file format. Supported are public and private
 keys in PEM format (both PKCS #1 and PKCS #8), X.509 certificates, certificate signing
 requests (CSRs) and SSH public keys. You can find some test keys in the _tests/data_
 directory.
 
-By default badkeys will only output information about vulnerable keys, meaning there
-will be no output if no vulnerabilities are found. The _-a_ parameter creates output for
-all keys.
+By default, badkeys will only output information about vulnerable keys, meaning no
+output will be generated if no vulnerabilities are found. The _-a_ parameter creates
+output for all keys.
 
 # scanning
 
-badkeys can directly scan SSH and TLS hosts and automatically check their public keys.
-This can be enabled with the parameters _-s_ (for SSH) and _-t_ (for TLS). By default
-SSH will be scanned on port 22 and TLS will be scanned on several ports for common
-protocols (https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443,
-which is commonly used as a non-standard https port).
+badkeys can scan SSH and TLS hosts and automatically check their public keys. This can
+be enabled with the parameters _-s_ (SSH) and _-t_ (TLS). By default, SSH will be
+scanned on port 22 and TLS will be scanned on several ports for common protocols
+(https/443, smtps/465, ldaps/636, ftps/990, imaps/993, pop3s/995 and 8443, which is
+commonly used as a non-standard https port).
 
 Alternative ports can be configured with _--tls-ports_ and _--ssh-ports_.
 
 TLS and SSH scanning can be combined:
 ```
 badkeys -ts example.org
 ```
 
+Note that the scanning modes have limitations. It is often more desirable to use other
+tools to collect TLS/SSH keys and scan them locally with badkeys.
+
+SSH scanning needs [paramiko](https://www.paramiko.org/) as an additional dependency.
+
+TLS scanning can't detect multiple certificates on one host (e.g. ECDSA and RSA). This
+is a [limitation of Python's ssl.get_server_certificate() function](
+https://bugs.python.org/issue31892).
+
 # Python module and API
 
-badkeys can also be used as a Python module. However currently the software is in alpha
+badkeys can also be used as a Python module. However, currently the software is in beta
 state and the API may change regularly.
 
 # about
 
 badkeys was written by [Hanno Böck](https://hboeck.de).
 
-This work was originally funded in 2022 by Industriens Fond through the CIDI project
+This work was initially funded in 2022 by Industriens Fond through the CIDI project
 (Cybersecure IOT in Danish Industry) and the [Center for Information Security and Trust
 (CISAT)](https://cisat.dk/) at the IT University of Copenhagen, Denmark.
```

### Comparing `badkeys-0.0.7/badkeys.egg-info/SOURCES.txt` & `badkeys-0.0.8/badkeys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/pyproject.toml` & `badkeys-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "badkeys"
-version = "0.0.7"
+version = "0.0.8"
 description = "Check cryptographic keys for known weaknesses"
 readme = "README.md"
 authors = [{name = "Hanno Böck"}]
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3",
```

### Comparing `badkeys-0.0.7/tests/data/rsa-debianweak.key` & `badkeys-0.0.8/tests/data/rsa-debianweak.key`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/data/rsa-fermat-hexmodulus.txt` & `badkeys-0.0.8/tests/data/rsa-fermat-hexmodulus.txt`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/data/rsa-fermat.crt` & `badkeys-0.0.8/tests/data/rsa-fermat.crt`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/data/rsa-fermat.csr` & `badkeys-0.0.8/tests/data/rsa-fermat.csr`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/data/rsa-pattern.key` & `badkeys-0.0.8/tests/data/rsa-pattern.key`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_failures.py` & `badkeys-0.0.8/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_fermat.py` & `badkeys-0.0.8/tests/test_fermat.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_pattern.py` & `badkeys-0.0.8/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_roca.py` & `badkeys-0.0.8/tests/test_roca.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_rsabl.py` & `badkeys-0.0.8/tests/test_rsabl.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import badkeys
 
 TDPATH = f"{os.path.dirname(__file__)}/data/"
 
 
 class TestRsabl(unittest.TestCase):
+    @unittest.skipUnless(os.environ.get("RUNBLTESTS"), "Not running blocklist tests")
     def test_rsabl(self):
         with open(f"{TDPATH}rsa-debianweak.key") as f:
             key = f.read()
         r = badkeys.checkpubkey(key, checks=["blocklist"])
         self.assertTrue("blocklist" in r["results"])
         with open(f"{TDPATH}rsa-ok.key") as f:
             key = f.read()
```

### Comparing `badkeys-0.0.7/tests/test_rsainvalid.py` & `badkeys-0.0.8/tests/test_rsainvalid.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,22 @@
 import os
 
 import badkeys
 
 TDPATH = f"{os.path.dirname(__file__)}/data/"
 
 
-class TestSmallprimes(unittest.TestCase):
-    def test_smallprimes(self):
+class TestRSAInvalid(unittest.TestCase):
+    def test_rsainvalid(self):
         with open(f"{TDPATH}rsa-e1.key") as f:
             key = f.read()
         r = badkeys.checkpubkey(key, checks=["rsainvalid"])
         self.assertTrue("rsainvalid" in r["results"])
         self.assertEqual("invalid_e", r["results"]["rsainvalid"]["subtest"])
 
-        with open(f"{TDPATH}rsa-nprime.key") as f:
-            key = f.read()
-        r = badkeys.checkpubkey(key, checks=["rsainvalid"])
-        self.assertTrue("rsainvalid" in r["results"])
-        self.assertEqual("prime_n", r["results"]["rsainvalid"]["subtest"])
-
         with open(f"{TDPATH}rsa-ok.key") as f:
             key = f.read()
         r = badkeys.checkpubkey(key, checks=["rsainvalid"])
         self.assertFalse(r["results"])
 
 
 if __name__ == "__main__":
```

### Comparing `badkeys-0.0.7/tests/test_sharedprimes.py` & `badkeys-0.0.8/tests/test_sharedprimes.py`

 * *Files identical despite different names*

### Comparing `badkeys-0.0.7/tests/test_smallprimes.py` & `badkeys-0.0.8/tests/test_smallprimes.py`

 * *Files identical despite different names*

