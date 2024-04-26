# Comparing `tmp/noobstuffs-2.0.5.tar.gz` & `tmp/noobstuffs-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noobstuffs-2.0.5.tar", max compression
+gzip compressed data, was "noobstuffs-2.0.6.tar", max compression
```

## Comparing `noobstuffs-2.0.5.tar` & `noobstuffs-2.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      797 2024-04-12 13:14:51.077928 noobstuffs-2.0.5/NoobStuffs/__init__.py
--rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.5/NoobStuffs/libandroid/__init__.py
--rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.5/NoobStuffs/libdatetime/__init__.py
--rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.5/NoobStuffs/libformatter/__init__.py
--rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.5/NoobStuffs/libformatter/escape.py
--rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.5/NoobStuffs/libgithub/__init__.py
--rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.5/NoobStuffs/liblogging/__init__.py
--rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.5/NoobStuffs/libpasty/__init__.py
--rwxr-xr-x   0        0        0     1985 2024-04-12 12:33:19.576889 noobstuffs-2.0.5/NoobStuffs/libtelegrambot/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.5/NoobStuffs/libtelegraph/__init__.py
--rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.5/README.md
--rw-r--r--   0        0        0      805 2024-04-12 13:14:59.606639 noobstuffs-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      797 2024-04-26 11:48:00.481641 noobstuffs-2.0.6/NoobStuffs/__init__.py
+-rw-r--r--   0        0        0     2085 2022-11-19 04:49:54.617779 noobstuffs-2.0.6/NoobStuffs/libandroid/__init__.py
+-rw-r--r--   0        0        0     1770 2022-11-19 04:49:54.628785 noobstuffs-2.0.6/NoobStuffs/libdatetime/__init__.py
+-rwxr-xr-x   0        0        0      803 2024-04-26 09:41:31.142399 noobstuffs-2.0.6/NoobStuffs/libenvconfig/__init__.py
+-rw-r--r--   0        0        0     4477 2022-11-19 04:49:54.638787 noobstuffs-2.0.6/NoobStuffs/libformatter/__init__.py
+-rw-r--r--   0        0        0     1473 2022-11-19 04:49:54.646774 noobstuffs-2.0.6/NoobStuffs/libformatter/escape.py
+-rw-r--r--   0        0        0     3414 2022-11-19 04:49:54.655784 noobstuffs-2.0.6/NoobStuffs/libgithub/__init__.py
+-rw-r--r--   0        0        0     2540 2022-11-19 04:49:54.664783 noobstuffs-2.0.6/NoobStuffs/liblogging/__init__.py
+-rw-r--r--   0        0        0     1443 2022-11-19 04:49:54.673781 noobstuffs-2.0.6/NoobStuffs/libpasty/__init__.py
+-rwxr-xr-x   0        0        0     1985 2024-04-12 14:37:30.623095 noobstuffs-2.0.6/NoobStuffs/libtelegrambot/__init__.py
+-rw-r--r--   0        0        0     2724 2024-04-07 07:05:32.639477 noobstuffs-2.0.6/NoobStuffs/libtelegraph/__init__.py
+-rw-r--r--   0        0        0      604 2022-11-19 04:49:54.687784 noobstuffs-2.0.6/README.md
+-rw-r--r--   0        0        0      805 2024-04-26 11:48:31.970915 noobstuffs-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 noobstuffs-2.0.6/PKG-INFO
```

### Comparing `noobstuffs-2.0.5/NoobStuffs/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 #
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
```

### Comparing `noobstuffs-2.0.5/NoobStuffs/libandroid/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libandroid/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libdatetime/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libdatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libformatter/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libformatter/escape.py` & `noobstuffs-2.0.6/NoobStuffs/libformatter/escape.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libgithub/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libgithub/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/liblogging/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/liblogging/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libpasty/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libpasty/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libtelegrambot/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libtelegrambot/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/NoobStuffs/libtelegraph/__init__.py` & `noobstuffs-2.0.6/NoobStuffs/libtelegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/README.md` & `noobstuffs-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `noobstuffs-2.0.5/pyproject.toml` & `noobstuffs-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "NoobStuffs"
-version = "2.0.5"
+version = "2.0.6"
 description = "Python Library for PrajjuS Projects"
 license = "GPL-3.0"
 authors = ["PrajjuS <theprajjus@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/PrajjuS/NoobStuffs"
 keywords = ["noobstuffs", "libs", "noob", "lazy"]
 classifiers = [
```

### Comparing `noobstuffs-2.0.5/PKG-INFO` & `noobstuffs-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NoobStuffs
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python Library for PrajjuS Projects
 Home-page: https://github.com/PrajjuS/NoobStuffs
 License: GPL-3.0
 Keywords: noobstuffs,libs,noob,lazy
 Author: PrajjuS
 Author-email: theprajjus@gmail.com
 Requires-Python: >=3.8,<4.0
```

