# Comparing `tmp/neon-mana-utils-0.2.3a1.tar.gz` & `tmp/neon-mana-utils-0.2.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-mana-utils-0.2.3a1.tar", last modified: Tue Nov 14 02:46:30 2023, max compression
+gzip compressed data, was "neon-mana-utils-0.2.3a2.tar", last modified: Fri Apr 26 01:38:11 2024, max compression
```

## Comparing `neon-mana-utils-0.2.3a1.tar` & `neon-mana-utils-0.2.3a2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 02:46:30.529140 neon-mana-utils-0.2.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-11-14 02:46:30.525140 neon-mana-utils-0.2.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 02:46:30.525140 neon-mana-utils-0.2.3a1/neon_mana_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/bus_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15516 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/core_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/messagebus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/skills.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/neon_mana_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 02:46:30.525140 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-14 02:46:30.000000 neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 02:46:30.529140 neon-mana-utils-0.2.3a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-11-14 02:46:25.000000 neon-mana-utils-0.2.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:38:11.369182 neon-mana-utils-0.2.3a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-26 01:38:11.369182 neon-mana-utils-0.2.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:38:11.369182 neon-mana-utils-0.2.3a2/neon_mana_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/bus_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/core_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/messagebus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/skills.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/neon_mana_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 01:38:11.369182 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 01:38:11.000000 neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 01:38:11.369182 neon-mana-utils-0.2.3a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-26 01:38:07.000000 neon-mana-utils-0.2.3a2/setup.py
```

### Comparing `neon-mana-utils-0.2.3a1/LICENSE.md` & `neon-mana-utils-0.2.3a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/PKG-INFO` & `neon-mana-utils-0.2.3a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.2.3a1/README.md` & `neon-mana-utils-0.2.3a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/__init__.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/bus_api.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/bus_api.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/cli.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/cli.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/config.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/config.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/constants.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/constants.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/core_commands.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/core_commands.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/messagebus.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/messagebus.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/skills.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/skills.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/status.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/status.py`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils/version.py` & `neon-mana-utils-0.2.3a2/neon_mana_utils/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.2.3a1"
+__version__ = "0.2.3a2"
```

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/PKG-INFO` & `neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-mana-utils
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: Message Application for Neon AI
 Home-page: https://github.com/neongeckocom/neon-mana-utils
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-mana-utils-0.2.3a1/neon_mana_utils.egg-info/SOURCES.txt` & `neon-mana-utils-0.2.3a2/neon_mana_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-mana-utils-0.2.3a1/setup.py` & `neon-mana-utils-0.2.3a2/setup.py`

 * *Files identical despite different names*

