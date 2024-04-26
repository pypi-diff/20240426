# Comparing `tmp/gramps_ql-0.2.1.tar.gz` & `tmp/gramps_ql-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gramps_ql-0.2.1.tar", last modified: Sun Apr 21 06:20:36 2024, max compression
+gzip compressed data, was "gramps_ql-0.3.0.tar", last modified: Fri Apr 26 15:17:24 2024, max compression
```

## Comparing `gramps_ql-0.2.1.tar` & `gramps_ql-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/mypy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/src/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 06:20:35.000000 gramps_ql-0.2.1/src/gramps_ql/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/src/gramps_ql/gql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/src/gramps_ql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-21 06:20:36.000000 gramps_ql-0.2.1/src/gramps_ql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.020545 gramps_ql-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 06:20:36.024545 gramps_ql-0.2.1/tests/gramps_ql/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3640 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-21 06:20:31.000000 gramps_ql-0.2.1/tests/gramps_ql/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.458334 gramps_ql-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/mypy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.458334 gramps_ql-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/src/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/src/gramps_ql/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/src/gramps_ql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/src/gramps_ql/gql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/src/gramps_ql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12842 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 15:17:24.000000 gramps_ql-0.3.0/src/gramps_ql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.458334 gramps_ql-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:17:24.462334 gramps_ql-0.3.0/tests/gramps_ql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/tests/gramps_ql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/tests/gramps_ql/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/tests/gramps_ql/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-26 15:17:19.000000 gramps_ql-0.3.0/tests/gramps_ql/test_parse.py
```

### Comparing `gramps_ql-0.2.1/.github/workflows/python-publish.yml` & `gramps_ql-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gramps_ql-0.2.1/.github/workflows/test.yml` & `gramps_ql-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `gramps_ql-0.2.1/LICENSE` & `gramps_ql-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gramps_ql-0.2.1/PKG-INFO` & `gramps_ql-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-Metadata-Version: 2.1
-Name: gramps-ql
-Version: 0.2.1
-Summary: A Python library to filter Gramps objects by a query syntax
-Author-email: "David M. Straub" <straub@protonmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/DavidMStraub/gramps-ql
-Project-URL: repository, https://github.com/DavidMStraub/gramps-ql
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyparsing>=3
-
 # GQL &ndash; the Gramps Query Language
 
 This Python library provides GQL, a query language to a [Gramps](https://github.com/gramps-project/gramps) database. The syntax is inspired by JQL, the Jira Query Language.
 
 ## Installation
 
 ```
 python -m pip install gramps-ql
 ```
 
 ## Usage
 
+You can iterate over objects in a database matching the query:
+
 ```python
-from gramps_ql import iter_objects
+import gramps_ql  as gql
 
 db = ... # A Gramps DbReadBase instance
 
 # iterate over private people
-query = 'type=person AND private'
+query = 'class=person AND private'
 
-for obj in iter_objects(query, db):
+for obj in gql.iter_objects(query, db):
     f(obj) # do something with the Gramps object obj
 ```
 
+Alternatively, you can match individual objects:
+
+```python
+if gql.match(query, obj, db):
+    print("Object matches query 🙂")
+else:
+    print("Object doesn't match query 🙁")
+```
+
 ## Syntax
 
 A GQL query is a string composed of statements of the form `property operator value`, optionally combined with the keywords `and` and `or` as well as parentheses.
 
 ### Properties
 
-#### `type`
+#### `class`
 
-Filters for the Gramps object type and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
+Filters for the Gramps object class and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
 
 #### Object properties
 
 GQL supports querying nested properties of Gramps objects, e.g. `primary_name.date.calendar`. See below for a full list of properties – see also [Gramps Data Model](https://gramps-project.org/wiki/index.php/Gramps_Data_Model).
 
 #### List elements by index
 
@@ -56,19 +55,23 @@
 
 This is a special property that returns the length of an array-like Gramps property, e.g. `media_list.length > 0` to get objects with media references.
 
 #### `all`, `any`
 
 Two more special properties for array-like Gramps properties. `all` requires a condition to apply to all items of the list, `any` requires it to apply to at least one item. Both properties can be combined with other properties before and after. Examples: `media_list.any.citation_list.length > 0` to return objects with media references that have citations; `media_list.all.citation_list.length = 0` to return objects where all media objects do not have citations.
 
+#### `get_person`, etc.
+
+While all the preceding properties refer to a single Gramps object, it is also possible to filter on different objects referred to by the initial object. For instance, an event has a place handle in its `place` property. Using the `get_place` pseudo-property, GQL switches to the properties of that object. For instance, it is possible to search for `class = event and place.get_place.name.value ~ York`. This can also be combined with `any` or `all`, e.g. `class = person and event_ref_list.any.ref.get_event.description ~ farmer`.
+
 ### Operators
 
 #### `=`, `!=`
 
-Equality or inequality. Examples: `type = person`, `type != family`
+Equality or inequality. Examples: `class = person`, `class != family`
 
 #### `>`, `>=`, `<`, `<=`
 
 Comparison. Works for strings as well as numbers. Examples: `confidence <= 1`, `change > 1712477760 `, `gramps_id > "I2015"`
 
 #### `~`, `!~`
 
@@ -82,53 +85,66 @@
 ### Values
 
 Values can be numbers or strings. If numbers should be interpreted as strings or special characters like = are involved, enclose the value in strings. Examples: `gramps_id = F0001`, but `gramps_id = "0001"`.
 
 ## Commented examples
 
 ```sql
-type = note and private and text.string ~ David
+class = note and private and text.string ~ David
 ```
 
 All private notes that contain the string "David" in their text
 
 
 ```sql
 media_list.length >= 10
 ```
 
-All objects (of any type) with 10 or more media references
+All objects (of any class) with 10 or more media references
 
 ```sql
-type != person and media_list.any.rect
+class != person and media_list.any.rect
 ```
 
 All objects that are *not* a person but have a media reference that is part of an image. Here, `media_list.any.rect` means that for each of the items in the media list, it is checked whether the `rect` (rectangle) property has a truthy value, meaning it is a non-empty list. (`media_list.any.rect.length > 0` would have the same effect.)
 
 ```sql
-type = family and child_ref_list.length > 10
+class = family and child_ref_list.length > 10
 ```
 
 Families with more than 10 children.
 
 ```sql
-type = event and date.modifier = 0 and date.dateval[2] > 2020
+class = event and date.modifier = 0 and date.dateval[2] > 2020
 ```
 
 Events where the date is a normal date (not a range etc.) and the year is after 2020.
 
+```sql
+note_list.any.get_note.text.string ~ "David"
+```
+
+All objects with at least one note that contains the string "David" in their text.
+
+
+```sql
+class = family and child_ref_list.all.ref.get_person.gender = 0 child_ref_list.length = 3
+```
+
+All families with three daughters.
+
+
 ## Roadmap
 
 GQL could be used in Gramplets or in Gramps Web (API).
 
 The following improvements are currently being contemplated:
 
 - Better support for dates, e.g. comparing a string to a date
-- Support for links between objects, e.g. following a reference handle to the referenced object (`note_list.any.get_note.text.string ~ x` ...)
-- Performance improvements. Currently, the whole database needs to be read even for a simple query like `type=tag`.
+- Performance improvements. Currently, the whole database needs to be read even for a simple query like `class=tag`.
 
 Suggestions for improvment as well as contributions are welcome!
 
 ## Full list of Gramps Properties
 
 The following properties of Gramps objects exist as of Gramps 5.2.
```

### Comparing `gramps_ql-0.2.1/README.md` & `gramps_ql-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,63 @@
+Metadata-Version: 2.1
+Name: gramps-ql
+Version: 0.3.0
+Summary: A Python library to filter Gramps objects by a query syntax
+Author-email: "David M. Straub" <straub@protonmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/DavidMStraub/gramps-ql
+Project-URL: repository, https://github.com/DavidMStraub/gramps-ql
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyparsing>=3
+
 # GQL &ndash; the Gramps Query Language
 
 This Python library provides GQL, a query language to a [Gramps](https://github.com/gramps-project/gramps) database. The syntax is inspired by JQL, the Jira Query Language.
 
 ## Installation
 
 ```
 python -m pip install gramps-ql
 ```
 
 ## Usage
 
+You can iterate over objects in a database matching the query:
+
 ```python
-from gramps_ql import iter_objects
+import gramps_ql  as gql
 
 db = ... # A Gramps DbReadBase instance
 
 # iterate over private people
-query = 'type=person AND private'
+query = 'class=person AND private'
 
-for obj in iter_objects(query, db):
+for obj in gql.iter_objects(query, db):
     f(obj) # do something with the Gramps object obj
 ```
 
+Alternatively, you can match individual objects:
+
+```python
+if gql.match(query, obj, db):
+    print("Object matches query 🙂")
+else:
+    print("Object doesn't match query 🙁")
+```
+
 ## Syntax
 
 A GQL query is a string composed of statements of the form `property operator value`, optionally combined with the keywords `and` and `or` as well as parentheses.
 
 ### Properties
 
-#### `type`
+#### `class`
 
-Filters for the Gramps object type and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
+Filters for the Gramps object class and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
 
 #### Object properties
 
 GQL supports querying nested properties of Gramps objects, e.g. `primary_name.date.calendar`. See below for a full list of properties – see also [Gramps Data Model](https://gramps-project.org/wiki/index.php/Gramps_Data_Model).
 
 #### List elements by index
 
@@ -44,19 +67,23 @@
 
 This is a special property that returns the length of an array-like Gramps property, e.g. `media_list.length > 0` to get objects with media references.
 
 #### `all`, `any`
 
 Two more special properties for array-like Gramps properties. `all` requires a condition to apply to all items of the list, `any` requires it to apply to at least one item. Both properties can be combined with other properties before and after. Examples: `media_list.any.citation_list.length > 0` to return objects with media references that have citations; `media_list.all.citation_list.length = 0` to return objects where all media objects do not have citations.
 
+#### `get_person`, etc.
+
+While all the preceding properties refer to a single Gramps object, it is also possible to filter on different objects referred to by the initial object. For instance, an event has a place handle in its `place` property. Using the `get_place` pseudo-property, GQL switches to the properties of that object. For instance, it is possible to search for `class = event and place.get_place.name.value ~ York`. This can also be combined with `any` or `all`, e.g. `class = person and event_ref_list.any.ref.get_event.description ~ farmer`.
+
 ### Operators
 
 #### `=`, `!=`
 
-Equality or inequality. Examples: `type = person`, `type != family`
+Equality or inequality. Examples: `class = person`, `class != family`
 
 #### `>`, `>=`, `<`, `<=`
 
 Comparison. Works for strings as well as numbers. Examples: `confidence <= 1`, `change > 1712477760 `, `gramps_id > "I2015"`
 
 #### `~`, `!~`
 
@@ -70,53 +97,66 @@
 ### Values
 
 Values can be numbers or strings. If numbers should be interpreted as strings or special characters like = are involved, enclose the value in strings. Examples: `gramps_id = F0001`, but `gramps_id = "0001"`.
 
 ## Commented examples
 
 ```sql
-type = note and private and text.string ~ David
+class = note and private and text.string ~ David
 ```
 
 All private notes that contain the string "David" in their text
 
 
 ```sql
 media_list.length >= 10
 ```
 
-All objects (of any type) with 10 or more media references
+All objects (of any class) with 10 or more media references
 
 ```sql
-type != person and media_list.any.rect
+class != person and media_list.any.rect
 ```
 
 All objects that are *not* a person but have a media reference that is part of an image. Here, `media_list.any.rect` means that for each of the items in the media list, it is checked whether the `rect` (rectangle) property has a truthy value, meaning it is a non-empty list. (`media_list.any.rect.length > 0` would have the same effect.)
 
 ```sql
-type = family and child_ref_list.length > 10
+class = family and child_ref_list.length > 10
 ```
 
 Families with more than 10 children.
 
 ```sql
-type = event and date.modifier = 0 and date.dateval[2] > 2020
+class = event and date.modifier = 0 and date.dateval[2] > 2020
 ```
 
 Events where the date is a normal date (not a range etc.) and the year is after 2020.
 
+```sql
+note_list.any.get_note.text.string ~ "David"
+```
+
+All objects with at least one note that contains the string "David" in their text.
+
+
+```sql
+class = family and child_ref_list.all.ref.get_person.gender = 0 child_ref_list.length = 3
+```
+
+All families with three daughters.
+
+
 ## Roadmap
 
 GQL could be used in Gramplets or in Gramps Web (API).
 
 The following improvements are currently being contemplated:
 
 - Better support for dates, e.g. comparing a string to a date
-- Support for links between objects, e.g. following a reference handle to the referenced object (`note_list.any.get_note.text.string ~ x` ...)
-- Performance improvements. Currently, the whole database needs to be read even for a simple query like `type=tag`.
+- Performance improvements. Currently, the whole database needs to be read even for a simple query like `class=tag`.
 
 Suggestions for improvment as well as contributions are welcome!
 
 ## Full list of Gramps Properties
 
 The following properties of Gramps objects exist as of Gramps 5.2.
```

### Comparing `gramps_ql-0.2.1/pyproject.toml` & `gramps_ql-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gramps_ql-0.2.1/src/gramps_ql/gql.py` & `gramps_ql-0.3.0/src/gramps_ql/gql.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,34 +4,45 @@
 
 import json
 from collections.abc import Generator
 from typing import Any, Optional, Union
 
 import pyparsing as pp
 from gramps.gen.db import DbReadBase
+from gramps.gen.errors import HandleError
 from gramps.gen.lib import PrimaryObject
 from gramps.gen.lib.serialize import to_json
 
 pp.ParserElement.enablePackrat()
 
 
-def match(query: str, obj: Union[PrimaryObject, dict[str, Any]]) -> bool:
+def to_dict(obj: PrimaryObject) -> dict[str, Any]:
+    """Convert a Gramps object to its dictionary representation."""
+    obj_dict = json.loads(to_json(obj))
+    obj_dict["class"] = obj_dict["_class"].lower()
+    return obj_dict
+
+
+def match(
+    query: str,
+    obj: Union[PrimaryObject, dict[str, Any]],
+    db: Optional[DbReadBase] = None,
+) -> bool:
     """Match a single object (optionally given as dictionary) to a query."""
-    gq = GQLQuery(query=query)
+    gq = GQLQuery(query=query, db=db)
     if isinstance(obj, PrimaryObject):
-        obj_dict = json.loads(to_json(obj))
-        obj_dict["type"] = obj_dict["_class"].lower()
+        obj_dict = to_dict(obj)
         return gq.match(obj_dict)
     return gq.match(obj)
 
 
 def iter_objects(query: str, db: DbReadBase) -> Generator[PrimaryObject, None, None]:
     """Iterate over primary objects in a Gramps database."""
-    gq = GQLQuery(query=query)
-    return gq.iter_objects(db)
+    gq = GQLQuery(query=query, db=db)
+    return gq.iter_objects()
 
 
 word = pp.Word(pp.alphanums + "." + "_")
 rhs = word | pp.dbl_quoted_string | pp.sgl_quoted_string
 # lhs = pp.Word(pp.identchars, pp.identbodychars + "." + "_")
 logical_and = pp.CaselessKeyword("and")
 logical_or = pp.CaselessKeyword("or")
@@ -75,17 +86,18 @@
 def parse_lhs(query: str):
     return lhs.parse_string(query, parse_all=True)
 
 
 class GQLQuery:
     """GQL query class."""
 
-    def __init__(self, query: str):
+    def __init__(self, query: str, db: Optional[DbReadBase] = None):
         self.query = query
         self.parsed = parse(self.query)
+        self.db = db
 
     @staticmethod
     def _combine_logical(op: Optional[str], value1: bool, value2: bool) -> bool:
         """Combine booleans with a logical operator as string."""
         if op == "and":
             return value1 and value2
         elif op == "or":
@@ -127,15 +139,15 @@
         self, obj: dict[str, Any], lhs: str, operator: str = "", rhs: str = ""
     ) -> bool:
         """Match an object to a single condition."""
         parsed = parse_lhs(lhs)
         if not parsed:
             raise ValueError(f"Unable to parse left-hand side: {lhs}")
         for i, part in enumerate(parsed):
-            if i == 0:
+            if i == 0 and isinstance(obj, dict):
                 result = obj.get(parsed[0])
             elif part in ["[", "]", "."]:
                 continue
             elif part == "length":
                 result = len(result)
             elif part in ["all", "any"]:
                 if i + 1 == len(parsed):  # last item
@@ -153,14 +165,24 @@
                 try:
                     if part == "all":
                         return results and all(results)  # because all([]) is True
                     else:
                         return any(results)
                 except TypeError:
                     return False
+            elif isinstance(part, str) and part.startswith("get_"):
+                if not self.db:
+                    raise ValueError("Database is needed for get")
+                try:
+                    if i == 0 and isinstance(obj, str):
+                        result = obj
+                    _obj = getattr(self.db, f"{part}_from_handle")(result)
+                except (AttributeError, HandleError):
+                    return False
+                result = to_dict(_obj)
             else:
                 try:
                     result = result[part]
                 except (KeyError, IndexError):
                     return False
             if result is None:
                 return False
@@ -172,39 +194,48 @@
             return bool(result)
         if isinstance(rhs, str):
             if rhs.isdigit():
                 rhs = int(rhs)
             else:
                 rhs = rhs.strip("\"'")
         if operator == "=":
+            if isinstance(result, str):
+                rhs = str(rhs)
+                return result.casefold() == rhs.casefold()
             return result == rhs
         if operator == "!=":
+            if isinstance(result, str):
+                rhs = str(rhs)
+                return result.casefold() != rhs.casefold()
             return result != rhs
         if operator == "~":
             if isinstance(result, str):
                 rhs = str(rhs)
+                return rhs.casefold() in result.casefold()
             return rhs in result
         if operator == "!~":
             if isinstance(result, str):
                 rhs = str(rhs)
+                return rhs.casefold() in result.casefold()
             return rhs not in result
         try:
             if operator == "<":
                 return result < rhs
             if operator == ">":
                 return result > rhs
             if operator == "<=":
                 return result <= rhs
             if operator == ">=":
                 return result >= rhs
         except TypeError:
             return False
 
-    def iter_objects(self, db: DbReadBase) -> Generator[PrimaryObject, None, None]:
+    def iter_objects(self) -> Generator[PrimaryObject, None, None]:
         """Iterate over primary objects in a Gramps database."""
+        if not self.db:
+            raise ValueError("Database is needed for iterating objects!")
         for object_name, objects_name in GRAMPS_OBJECT_NAMES.items():
-            iter_method = getattr(db, f"iter_{objects_name}")
+            iter_method = getattr(self.db, f"iter_{objects_name}")
             for obj in iter_method():
-                obj_dict = json.loads(to_json(obj))
-                obj_dict["type"] = obj_dict["_class"].lower()
+                obj_dict = to_dict(obj)
                 if self.match(obj_dict):
                     yield obj
```

### Comparing `gramps_ql-0.2.1/src/gramps_ql.egg-info/PKG-INFO` & `gramps_ql-0.3.0/src/gramps_ql.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gramps-ql
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python library to filter Gramps objects by a query syntax
 Author-email: "David M. Straub" <straub@protonmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/DavidMStraub/gramps-ql
 Project-URL: repository, https://github.com/DavidMStraub/gramps-ql
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -18,35 +18,46 @@
 
 ```
 python -m pip install gramps-ql
 ```
 
 ## Usage
 
+You can iterate over objects in a database matching the query:
+
 ```python
-from gramps_ql import iter_objects
+import gramps_ql  as gql
 
 db = ... # A Gramps DbReadBase instance
 
 # iterate over private people
-query = 'type=person AND private'
+query = 'class=person AND private'
 
-for obj in iter_objects(query, db):
+for obj in gql.iter_objects(query, db):
     f(obj) # do something with the Gramps object obj
 ```
 
+Alternatively, you can match individual objects:
+
+```python
+if gql.match(query, obj, db):
+    print("Object matches query 🙂")
+else:
+    print("Object doesn't match query 🙁")
+```
+
 ## Syntax
 
 A GQL query is a string composed of statements of the form `property operator value`, optionally combined with the keywords `and` and `or` as well as parentheses.
 
 ### Properties
 
-#### `type`
+#### `class`
 
-Filters for the Gramps object type and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
+Filters for the Gramps object class and can be one of `person`, `family`, `event`, `place`, `citation`, `source`, `repository`, `media`, or `note`.
 
 #### Object properties
 
 GQL supports querying nested properties of Gramps objects, e.g. `primary_name.date.calendar`. See below for a full list of properties – see also [Gramps Data Model](https://gramps-project.org/wiki/index.php/Gramps_Data_Model).
 
 #### List elements by index
 
@@ -56,19 +67,23 @@
 
 This is a special property that returns the length of an array-like Gramps property, e.g. `media_list.length > 0` to get objects with media references.
 
 #### `all`, `any`
 
 Two more special properties for array-like Gramps properties. `all` requires a condition to apply to all items of the list, `any` requires it to apply to at least one item. Both properties can be combined with other properties before and after. Examples: `media_list.any.citation_list.length > 0` to return objects with media references that have citations; `media_list.all.citation_list.length = 0` to return objects where all media objects do not have citations.
 
+#### `get_person`, etc.
+
+While all the preceding properties refer to a single Gramps object, it is also possible to filter on different objects referred to by the initial object. For instance, an event has a place handle in its `place` property. Using the `get_place` pseudo-property, GQL switches to the properties of that object. For instance, it is possible to search for `class = event and place.get_place.name.value ~ York`. This can also be combined with `any` or `all`, e.g. `class = person and event_ref_list.any.ref.get_event.description ~ farmer`.
+
 ### Operators
 
 #### `=`, `!=`
 
-Equality or inequality. Examples: `type = person`, `type != family`
+Equality or inequality. Examples: `class = person`, `class != family`
 
 #### `>`, `>=`, `<`, `<=`
 
 Comparison. Works for strings as well as numbers. Examples: `confidence <= 1`, `change > 1712477760 `, `gramps_id > "I2015"`
 
 #### `~`, `!~`
 
@@ -82,53 +97,66 @@
 ### Values
 
 Values can be numbers or strings. If numbers should be interpreted as strings or special characters like = are involved, enclose the value in strings. Examples: `gramps_id = F0001`, but `gramps_id = "0001"`.
 
 ## Commented examples
 
 ```sql
-type = note and private and text.string ~ David
+class = note and private and text.string ~ David
 ```
 
 All private notes that contain the string "David" in their text
 
 
 ```sql
 media_list.length >= 10
 ```
 
-All objects (of any type) with 10 or more media references
+All objects (of any class) with 10 or more media references
 
 ```sql
-type != person and media_list.any.rect
+class != person and media_list.any.rect
 ```
 
 All objects that are *not* a person but have a media reference that is part of an image. Here, `media_list.any.rect` means that for each of the items in the media list, it is checked whether the `rect` (rectangle) property has a truthy value, meaning it is a non-empty list. (`media_list.any.rect.length > 0` would have the same effect.)
 
 ```sql
-type = family and child_ref_list.length > 10
+class = family and child_ref_list.length > 10
 ```
 
 Families with more than 10 children.
 
 ```sql
-type = event and date.modifier = 0 and date.dateval[2] > 2020
+class = event and date.modifier = 0 and date.dateval[2] > 2020
 ```
 
 Events where the date is a normal date (not a range etc.) and the year is after 2020.
 
+```sql
+note_list.any.get_note.text.string ~ "David"
+```
+
+All objects with at least one note that contains the string "David" in their text.
+
+
+```sql
+class = family and child_ref_list.all.ref.get_person.gender = 0 child_ref_list.length = 3
+```
+
+All families with three daughters.
+
+
 ## Roadmap
 
 GQL could be used in Gramplets or in Gramps Web (API).
 
 The following improvements are currently being contemplated:
 
 - Better support for dates, e.g. comparing a string to a date
-- Support for links between objects, e.g. following a reference handle to the referenced object (`note_list.any.get_note.text.string ~ x` ...)
-- Performance improvements. Currently, the whole database needs to be read even for a simple query like `type=tag`.
+- Performance improvements. Currently, the whole database needs to be read even for a simple query like `class=tag`.
 
 Suggestions for improvment as well as contributions are welcome!
 
 ## Full list of Gramps Properties
 
 The following properties of Gramps objects exist as of Gramps 5.2.
```

### Comparing `gramps_ql-0.2.1/tests/gramps_ql/test_iter.py` & `gramps_ql-0.3.0/tests/gramps_ql/test_iter.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,25 +31,25 @@
 
 
 def test_fixture(db):
     assert isinstance(db, DbReadBase)
 
 
 def test_person_gramps_id(db):
-    q = GQLQuery("type=person")
-    assert len(list(q.iter_objects(db))) == 1
-    for obj in q.iter_objects(db):
+    q = GQLQuery("class=person", db=db)
+    assert len(list(q.iter_objects())) == 1
+    for obj in q.iter_objects():
         assert isinstance(obj, Person)
-    q = GQLQuery("""type=person and gramps_id="person001" """)
-    assert len(list(q.iter_objects(db))) == 1
-    q = GQLQuery("""type=person and gramps_id!="person001" """)
-    assert len(list(q.iter_objects(db))) == 0
-    q = GQLQuery("""type=person and gramps_id="person002" """)
-    assert len(list(q.iter_objects(db))) == 0
-    q = GQLQuery("""type=person and gramps_id>"person002" """)
-    assert len(list(q.iter_objects(db))) == 0
-    q = GQLQuery("""type=person and gramps_id<"person002" """)
-    assert len(list(q.iter_objects(db))) == 1
-    q = GQLQuery("type=person and gramps_id < 'person002'")
-    assert len(list(q.iter_objects(db))) == 1
-    q = GQLQuery("type=person and gramps_id < 'person002'")
-    assert len(list(q.iter_objects(db))) == 1
+    q = GQLQuery("""class=person and gramps_id="person001" """, db=db)
+    assert len(list(q.iter_objects())) == 1
+    q = GQLQuery("""class=person and gramps_id!="person001" """, db=db)
+    assert len(list(q.iter_objects())) == 0
+    q = GQLQuery("""class=person and gramps_id="person002" """, db=db)
+    assert len(list(q.iter_objects())) == 0
+    q = GQLQuery("""class=person and gramps_id>"person002" """, db=db)
+    assert len(list(q.iter_objects())) == 0
+    q = GQLQuery("""class=person and gramps_id<"person002" """, db=db)
+    assert len(list(q.iter_objects())) == 1
+    q = GQLQuery("class=person and gramps_id < 'person002'", db=db)
+    assert len(list(q.iter_objects())) == 1
+    q = GQLQuery("class=person and gramps_id < 'person002'", db=db)
+    assert len(list(q.iter_objects())) == 1
```

### Comparing `gramps_ql-0.2.1/tests/gramps_ql/test_match.py` & `gramps_ql-0.3.0/tests/gramps_ql/test_match.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,20 @@
 def test_string_contains():
     q = GQLQuery("string ~ 2")
     assert not q.match({"string": "abc"})
     assert not q.match({"string": "145"})
     assert q.match({"string": "co2"})
 
 
+def test_string_contains_case():
+    q = GQLQuery("string ~ a")
+    assert q.match({"string": "abc"})
+    assert q.match({"string": "Abc"})
+
+
 def test_any():
     q = GQLQuery("array.any = 2")
     assert not q.match({"array": []})
     assert not q.match({"array": [3, 4, 5]})
     assert q.match({"array": [1, 2, 3]})
```

### Comparing `gramps_ql-0.2.1/tests/gramps_ql/test_parse.py` & `gramps_ql-0.3.0/tests/gramps_ql/test_parse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 from gramps_ql import parse
 
 
 def test_single():
-    assert parse("type=person").as_list() == ["type", "=", "person"]
+    assert parse("class=person").as_list() == ["class", "=", "person"]
 
 
 def test_two():
-    assert parse("type=person or date.year > 2021").as_list() == [
+    assert parse("class=person or date.year > 2021").as_list() == [
         [
-            "type",
+            "class",
             "=",
             "person",
             "or",
             "date.year",
             ">",
             "2021",
         ]
     ]
 
 
 def test_three():
-    assert parse("type=person or name='John Doe' and date.year > 2021").as_list() == [
+    assert parse("class=person or name='John Doe' and date.year > 2021").as_list() == [
         [
-            "type",
+            "class",
             "=",
             "person",
             "or",
             ["name", "=", "'John Doe'", "and", "date.year", ">", "2021"],
         ]
     ]
-    assert parse("type=person and name='John Doe' or date.year > 2021").as_list() == [
+    assert parse("class=person and name='John Doe' or date.year > 2021").as_list() == [
         [
-            ["type", "=", "person", "and", "name", "=", "'John Doe'"],
+            ["class", "=", "person", "and", "name", "=", "'John Doe'"],
             "or",
             "date.year",
             ">",
             "2021",
         ]
     ]
-    assert parse("type=person and name='John Doe' or only_id").as_list() == [
+    assert parse("class=person and name='John Doe' or only_id").as_list() == [
         [
-            ["type", "=", "person", "and", "name", "=", "'John Doe'"],
+            ["class", "=", "person", "and", "name", "=", "'John Doe'"],
             "or",
             "only_id",
         ]
     ]
 
 
 def test_brackets():
-    assert parse("(type=person or name='John Doe') and date.year > 2021").as_list() == [
+    assert parse(
+        "(class=person or name='John Doe') and date.year > 2021"
+    ).as_list() == [
         [
-            ["type", "=", "person", "or", "name", "=", "'John Doe'"],
+            ["class", "=", "person", "or", "name", "=", "'John Doe'"],
             "and",
             "date.year",
             ">",
             "2021",
         ]
     ]
     assert parse(
-        "(((((((((((type=person or name='John Doe')))) and date.year > 2021)))))))"
+        "(((((((((((class=person or name='John Doe')))) and date.year > 2021)))))))"
     ).as_list() == [
         [
-            ["type", "=", "person", "or", "name", "=", "'John Doe'"],
+            ["class", "=", "person", "or", "name", "=", "'John Doe'"],
             "and",
             "date.year",
             ">",
             "2021",
         ]
     ]
```

