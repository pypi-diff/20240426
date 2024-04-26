# Comparing `tmp/neon-enclosure-1.7.0.tar.gz` & `tmp/neon-enclosure-1.7.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-enclosure-1.7.0.tar", last modified: Tue Apr 23 20:58:40 2024, max compression
+gzip compressed data, was "neon-enclosure-1.7.1a1.tar", last modified: Fri Apr 26 05:08:46 2024, max compression
```

## Comparing `neon-enclosure-1.7.0.tar` & `neon-enclosure-1.7.1a1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:40.099230 neon-enclosure-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 20:58:40.099230 neon-enclosure-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:40.095230 neon-enclosure-1.7.0/neon_enclosure/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:40.099230 neon-enclosure-1.7.0/neon_enclosure/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/admin/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/neon_enclosure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:58:40.099230 neon-enclosure-1.7.0/neon_enclosure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 20:58:40.000000 neon-enclosure-1.7.0/neon_enclosure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:58:40.099230 neon-enclosure-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-23 20:58:30.000000 neon-enclosure-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/neon_enclosure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/neon_enclosure/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/admin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/admin/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/neon_enclosure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 05:08:46.000000 neon-enclosure-1.7.1a1/neon_enclosure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 05:08:46.528860 neon-enclosure-1.7.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-26 05:08:41.000000 neon-enclosure-1.7.1a1/setup.py
```

### Comparing `neon-enclosure-1.7.0/LICENSE.md` & `neon-enclosure-1.7.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/PKG-INFO` & `neon-enclosure-1.7.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.7.0
+Version: 1.7.1a1
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.7.0/README.md` & `neon-enclosure-1.7.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/__init__.py` & `neon-enclosure-1.7.1a1/neon_enclosure/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/__main__.py` & `neon-enclosure-1.7.1a1/neon_enclosure/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from neon_utils.process_utils import start_malloc, snapshot_malloc, print_malloc
 from neon_utils.signal_utils import init_signal_bus, init_signal_handlers
-from ovos_utils.messagebus import get_mycroft_bus
+from ovos_bus_client.util import get_mycroft_bus
 from ovos_utils.process_utils import reset_sigint_handler, PIDLock
 from ovos_utils.log import LOG
 from ovos_utils import wait_for_exit_signal
 
 from neon_enclosure.service import NeonHardwareAbstractionLayer
```

### Comparing `neon-enclosure-1.7.0/neon_enclosure/admin/__init__.py` & `neon-enclosure-1.7.1a1/neon_enclosure/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/admin/__main__.py` & `neon-enclosure-1.7.1a1/neon_enclosure/admin/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/admin/service.py` & `neon-enclosure-1.7.1a1/neon_enclosure/admin/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/cli.py` & `neon-enclosure-1.7.1a1/neon_enclosure/cli.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/service.py` & `neon-enclosure-1.7.1a1/neon_enclosure/service.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure/utils.py` & `neon-enclosure-1.7.1a1/neon_enclosure/utils.py`

 * *Files identical despite different names*

### Comparing `neon-enclosure-1.7.0/neon_enclosure.egg-info/PKG-INFO` & `neon-enclosure-1.7.1a1/neon_enclosure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.7.0
+Version: 1.7.1a1
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: docker
```

### Comparing `neon-enclosure-1.7.0/setup.py` & `neon-enclosure-1.7.1a1/setup.py`

 * *Files identical despite different names*

