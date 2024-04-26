# Comparing `tmp/clocking-0.1.1.tar.gz` & `tmp/clocking-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clocking-0.1.1.tar", last modified: Wed Feb 21 10:27:58 2024, max compression
+gzip compressed data, was "clocking-0.1.2.tar", last modified: Fri Apr 26 10:45:08 2024, max compression
```

## Comparing `clocking-0.1.1.tar` & `clocking-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-02-21 10:27:58.282353 clocking-0.1.1/
--rwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)    34916 2022-10-10 08:42:42.000000 clocking-0.1.1/LICENSE.md
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    17331 2024-02-21 10:27:58.282353 clocking-0.1.1/PKG-INFO
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    16457 2024-01-31 09:32:59.000000 clocking-0.1.1/README.md
-drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-02-21 10:27:58.280354 clocking-0.1.1/clocking/
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1015 2024-02-21 10:24:53.000000 clocking-0.1.1/clocking/__init__.py
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    31107 2024-02-21 10:24:53.000000 clocking-0.1.1/clocking/cli.py
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    28989 2024-02-21 10:24:53.000000 clocking-0.1.1/clocking/core.py
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1098 2024-01-31 09:32:59.000000 clocking-0.1.1/clocking/exception.py
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     5396 2024-02-21 10:19:27.000000 clocking-0.1.1/clocking/util.py
-drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-02-21 10:27:58.281354 clocking-0.1.1/clocking.egg-info/
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    17331 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/PKG-INFO
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      362 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/SOURCES.txt
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        1 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/dependency_links.txt
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       71 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/entry_points.txt
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       12 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/requires.txt
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        9 2024-02-21 10:27:58.000000 clocking-0.1.1/clocking.egg-info/top_level.txt
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1060 2024-02-21 10:24:53.000000 clocking-0.1.1/pyproject.toml
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       38 2024-02-21 10:27:58.282353 clocking-0.1.1/setup.cfg
-drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-02-21 10:27:58.281354 clocking-0.1.1/tests/
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    52193 2023-09-06 09:33:54.000000 clocking-0.1.1/tests/test_core.py
--rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    36637 2024-02-21 10:24:53.000000 clocking-0.1.1/tests/test_parser.py
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-26 10:45:08.566064 clocking-0.1.2/
+-rwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)    34916 2022-10-10 08:42:42.000000 clocking-0.1.2/LICENSE.md
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    17331 2024-04-26 10:45:08.566064 clocking-0.1.2/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    16457 2024-01-31 09:32:59.000000 clocking-0.1.2/README.md
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-26 10:45:08.565065 clocking-0.1.2/clocking/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1015 2024-04-26 10:42:13.000000 clocking-0.1.2/clocking/__init__.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    31241 2024-04-26 10:42:13.000000 clocking-0.1.2/clocking/cli.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    28989 2024-02-21 10:24:53.000000 clocking-0.1.2/clocking/core.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1098 2024-01-31 09:32:59.000000 clocking-0.1.2/clocking/exception.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     5396 2024-02-21 10:19:27.000000 clocking-0.1.2/clocking/util.py
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-26 10:45:08.566064 clocking-0.1.2/clocking.egg-info/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    17331 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/PKG-INFO
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)      362 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/SOURCES.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        1 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/dependency_links.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       71 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/entry_points.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       12 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/requires.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)        9 2024-04-26 10:45:08.000000 clocking-0.1.2/clocking.egg-info/top_level.txt
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)     1060 2024-04-26 10:42:13.000000 clocking-0.1.2/pyproject.toml
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)       38 2024-04-26 10:45:08.566064 clocking-0.1.2/setup.cfg
+drwxr-xr-x   0 matteoguadrini  (1000) matteoguadrini  (1000)        0 2024-04-26 10:45:08.566064 clocking-0.1.2/tests/
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    52193 2023-09-06 09:33:54.000000 clocking-0.1.2/tests/test_core.py
+-rw-r--r--   0 matteoguadrini  (1000) matteoguadrini  (1000)    36662 2024-04-26 10:42:13.000000 clocking-0.1.2/tests/test_parser.py
```

### Comparing `clocking-0.1.1/LICENSE.md` & `clocking-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/PKG-INFO` & `clocking-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clocking
-Version: 0.1.1
+Version: 0.1.2
 Summary: Track the worked time.
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
 Project-URL: homepage, https://github.com/MatteoGuadrini/clocking
 Project-URL: documentation, https://clocking.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/MatteoGuadrini/clocking.git
```

### Comparing `clocking-0.1.1/README.md` & `clocking-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/clocking/__init__.py` & `clocking-0.1.2/clocking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 #     but WITHOUT ANY WARRANTY; without even the implied warranty of
 #     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #     GNU General Public License for more details.
 #
 #     You should have received a copy of the GNU General Public License
 #     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 from .core import *  # noqa: F403
 from .exception import *  # noqa: F403
 from .util import *  # noqa: F403
```

### Comparing `clocking-0.1.1/clocking/cli.py` & `clocking-0.1.2/clocking/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # region imports
 import argparse
 import os.path
 import sqlite3
 from getpass import getuser
 
 from clocking import (
+    datestring_to_datetime,
     database_exists,
     make_database,
     delete_database,
     get_current_version,
     update_version,
     create_configuration_table,
     add_configuration,
@@ -594,15 +595,19 @@
     db = options.get("database")
     verbosity = options.get("verbose")
     user = options.get("user")
     # Get force for deletion
     force = options.get("force")
     vprint(f"insert data into database {db} for user {user}", verbose=verbosity)
     # Set filled daily values
-    today = datetime.today()
+    today = (
+        datestring_to_datetime(options.get("date"))
+        if options.get("date")
+        else datetime.today()
+    )
     today_name = today.strftime("%a")
     year = today.year if not options.get("year") else options.get("year")
     month = today.month if not options.get("month") else options.get("month")
     day = today.day if not options.get("day") else options.get("day")
     if options.get("date"):
         vprint(f"setting date is {options.get('date')}", verbose=verbosity)
     else:
@@ -687,26 +692,26 @@
             print("warning: no permit and extraordinary hours in the same day")
             permit = 0
             extraordinary = 0
         # Check if hours value contains extraordinary hours
         more_extraordinary = find_extraordinary_hours(
             hours_value, user_configuration.daily_hours
         )
+        hours_value = hours_value - more_extraordinary
         if more_extraordinary:
             extraordinary = extraordinary + more_extraordinary
-            hours_value = hours_value - extraordinary
     # Default: check location value
     location = (
         options.get("location")
         if options.get("location")
         else user_configuration.location
     )
     vprint(
         f"setting hours={hours_value}, location={location}, "
-        f"extraordinary={extraordinary}, permit={permit}, other={other}"
+        f"extraordinary={extraordinary}, permit={permit}, other={other} "
         f"description={description}",
         verbose=verbosity,
     )
     err_msg = "error: working day {} failed"
     # Insert day(s)
     holiday_days = options.get("holidays_range")
     if holiday_days:
```

### Comparing `clocking-0.1.1/clocking/core.py` & `clocking-0.1.2/clocking/core.py`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/clocking/exception.py` & `clocking-0.1.2/clocking/exception.py`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/clocking/util.py` & `clocking-0.1.2/clocking/util.py`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/clocking.egg-info/PKG-INFO` & `clocking-0.1.2/clocking.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clocking
-Version: 0.1.1
+Version: 0.1.2
 Summary: Track the worked time.
 Author-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 Maintainer-email: Matteo Guadrini <matteo.guadrini@hotmail.it>
 License: GNU General Public License v3.0
 Project-URL: homepage, https://github.com/MatteoGuadrini/clocking
 Project-URL: documentation, https://clocking.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/MatteoGuadrini/clocking.git
```

### Comparing `clocking-0.1.1/pyproject.toml` & `clocking-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clocking"
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = { text = "GNU General Public License v3.0" }
 keywords = ['track', 'worked', 'time', 'stamp', 'mark']
 authors = [{ name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" }]
 maintainers = [
     { name = "Matteo Guadrini", email = "matteo.guadrini@hotmail.it" },
 ]
```

### Comparing `clocking-0.1.1/tests/test_core.py` & `clocking-0.1.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `clocking-0.1.1/tests/test_parser.py` & `clocking-0.1.2/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
     )
     assert rv == 0
     assert (
         out
         == """+----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+
 | date_id  | year | month | day | hours | description | location | extraordinary | permit_hours | other_hours | holiday | disease |
 +----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+
-| 20220111 | 2022 |   1   |  11 |  7.0  |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
+| 20220111 | 2022 |   1   |  11 |  8.0  |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
 | 20220125 | 2022 |   1   |  25 |  8.0  |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
 +----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+"""
     )
 
 
 # --------------------------------------------------
 def test_print_permit():
@@ -809,19 +809,19 @@
     rv, out = getstatusoutput(
         f"python3 {prg} print --database {TEMP_DB} --user test "
         "--other-hours --year 2022"
     )
     assert rv == 0
     assert (
         out
-        == """+----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+
-| date_id  | year | month | day | hours | description | location | extraordinary | permit_hours | other_hours | holiday | disease |
-+----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+
-| 20220122 | 2022 |   1   |  22 |  8.0  |     None    |  Milan   |      0.0      |     0.0      |     1.0     |    0    |    0    |
-+----------+------+-------+-----+-------+-------------+----------+---------------+--------------+-------------+---------+---------+"""
+        == """+----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+
+| date_id  | year | month | day |   hours    | description | location | extraordinary | permit_hours | other_hours | holiday | disease |
++----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+
+| 20220122 | 2022 |   1   |  22 | Not worked |     None    |  Milan   |      8.0      |     0.0      |     1.0     |    0    |    0    |
++----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+"""
     )
 
 
 # --------------------------------------------------
 def test_print_all():
     """print all"""
 
@@ -839,17 +839,17 @@
         out
         == """+----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+
 | date_id  | year | month | day |   hours    | description | location | extraordinary | permit_hours | other_hours | holiday | disease |
 +----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+
 | 20220103 | 2022 |   1   |  3  |    8.0     |     None    |  Milan   |      0.0      |     0.0      |     0.0     |    0    |    0    |
 | 20220104 | 2022 |   1   |  4  | Not worked |     None    |  Milan   |      0.0      |     0.0      |     0.0     |    1    |    0    |
 | 20220105 | 2022 |   1   |  5  | Not worked |   Disease   |  Milan   |      0.0      |     0.0      |     0.0     |    0    |    1    |
-| 20220111 | 2022 |   1   |  11 |    7.0     |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
+| 20220111 | 2022 |   1   |  11 |    8.0     |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
 | 20220121 | 2022 |   1   |  21 |    7.0     |     None    |  Milan   |      0.0      |     1.0      |     0.0     |    0    |    0    |
-| 20220122 | 2022 |   1   |  22 |    8.0     |     None    |  Milan   |      0.0      |     0.0      |     1.0     |    0    |    0    |
+| 20220122 | 2022 |   1   |  22 | Not worked |     None    |  Milan   |      8.0      |     0.0      |     1.0     |    0    |    0    |
 | 20220124 | 2022 |   1   |  24 |    8.0     |     None    |  Milan   |      0.0      |     0.0      |     0.0     |    0    |    0    |
 | 20220125 | 2022 |   1   |  25 |    8.0     |     None    |  Milan   |      1.0      |     0.0      |     0.0     |    0    |    0    |
 | 20220203 | 2022 |   2   |  3  |    8.0     |     None    |  Milan   |      0.0      |     0.0      |     0.0     |    0    |    0    |
 +----------+------+-------+-----+------------+-------------+----------+---------------+--------------+-------------+---------+---------+"""
     )
```

