# Comparing `tmp/extended_configparser-1.0.0.tar.gz` & `tmp/extended_configparser-1.0.1.tar.gz`

## Comparing `extended_configparser-1.0.0.tar` & `extended_configparser-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/noxfile.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/interpolator.py
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/matcher.py
--rw-r--r--   0        0        0    10115 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/parser.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/configuration/__init__.py
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/configuration/configuration.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/src/extended_configparser/configuration/entries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/test_config_matcher.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/test_env_interpolation.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/test_inquirer.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/test_parser.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/data/config1.cfg
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/data/config1_result.cfg
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/data/config2_result.cfg
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/tests/data/env_config.cfg
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/LICENSE
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/README.md
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 extended_configparser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/noxfile.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/__init__.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/interpolator.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/matcher.py
+-rw-r--r--   0        0        0    10406 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/parser.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/__init__.py
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/configuration.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/src/extended_configparser/configuration/entries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_config_matcher.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_env_interpolation.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_inquirer.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/test_parser.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config1.cfg
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config1_result.cfg
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/config2_result.cfg
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/tests/data/env_config.cfg
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8139 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/README.md
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 extended_configparser-1.0.1/PKG-INFO
```

### Comparing `extended_configparser-1.0.0/.pre-commit-config.yaml` & `extended_configparser-1.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/.github/workflows/python-publish.yml` & `extended_configparser-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/src/extended_configparser/interpolator.py` & `extended_configparser-1.0.1/src/extended_configparser/interpolator.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/src/extended_configparser/matcher.py` & `extended_configparser-1.0.1/src/extended_configparser/matcher.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/src/extended_configparser/parser.py` & `extended_configparser-1.0.1/src/extended_configparser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,22 @@
         """Set an option in a section.
         Optionally set a comment for the option.
         """
         super().set(section, option, value)
         if comment:
             self.set_comment(section, option, comment)
 
+    def add_section(self, section: str, comment: str | None = None):
+        """Add a section to the configuration.
+        Optionally set a comment for the section.
+        """
+        super().add_section(section)
+        if comment:
+            self.set_comment(section, comment=comment)
+
     #############################################################################
     ### ADDITIONAL GETTER METHODS
     #############################################################################
 
     @staticmethod
     def split_to_list(list_str: str, delimiter: str = ",") -> list[str]:
         if list_str is None or list_str == "":
```

### Comparing `extended_configparser-1.0.0/src/extended_configparser/configuration/configuration.py` & `extended_configparser-1.0.1/src/extended_configparser/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/src/extended_configparser/configuration/entries.py` & `extended_configparser-1.0.1/src/extended_configparser/configuration/entries.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/tests/test_config_matcher.py` & `extended_configparser-1.0.1/tests/test_config_matcher.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/tests/test_env_interpolation.py` & `extended_configparser-1.0.1/tests/test_env_interpolation.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,7 +38,9 @@
 
     assert parser.get("Section1", "a") == "a"
     assert parser.get("Section1", "b") == "a"
     assert parser.get("Section1", "c") == "EnvValue1/a"
     assert parser.get("Section1", "d") == "EnvValue2"
     assert parser.get("Section2", "a") == "a"
     assert parser.get("Section2", "b") == "EnvValue2/a/EnvValue1"
+
+    assert parser.get("Section2", "b", raw=True) == r"$TEMP_ENV_VAR2/${Section1:b}/${TEMP_ENV_VAR1}"
```

### Comparing `extended_configparser-1.0.0/tests/test_inquirer.py` & `extended_configparser-1.0.1/tests/test_inquirer.py`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/tests/test_parser.py` & `extended_configparser-1.0.1/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
 def test_change_comment(shared_datadir, tmp_path):
     contents = (shared_datadir / "config1.cfg").read_text()
     result = (shared_datadir / "config2_result.cfg").read_text()
 
     parser = ExtendedConfigParser()
     parser.read_string(contents)
+
+    parser.add_section("Section.New", "New Section")
+    parser.set("Section.New", "new_option", "new_value", "New value with new comment")
+
     parser.set_comment("Section.A", comment="New Section Comment")
     parser.set_comment("Section.A", "option2", comment="New option2 comment")
 
     output_path = tmp_path / "output.cfg"
     with open(output_path, "w") as f:
         parser.write(f)
```

### Comparing `extended_configparser-1.0.0/.gitignore` & `extended_configparser-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/LICENSE` & `extended_configparser-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_configparser-1.0.0/README.md` & `extended_configparser-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,22 +24,23 @@
 
 ## Example Usage
 
 ```python
 from extended_configparser.parser import ExtendedConfigParser
 
 # Load the config
-config = ExtendedConfigParser()
-config.read("myconfig.cfg")
+parser = ExtendedConfigParser()
+parser.read("myconfig.cfg")
 
 # Use the configuration as usual
 ...
 
-# Update the configuration as usual
-...
+# Set sections / options together with comments
+parser.add_section("Section.New", comment="New Section with a comment")
+parser.set("Section.New", "new_option", "new_value", comment="New value with new comment")
 
 # Access and alter the comments of a section or an option
 comment = config.get_comment("Section.A")
 parser.set_comment("Section.A", comment = "New Section Comment")
 parser.set_comment("Section.A", "option1", comment = "New option comment")
 
 # Save the config back to the file
@@ -150,14 +151,17 @@
 ```
 
 ### Interactive Configuration
 
 Your configuration class can also be used for an interactive configuration setup.
 This is useful for the first setup of a configuration file.
 
+> [!NOTE]
+> To use the `config.inquire()` method, .you have to install the package in the cli configuration `pip install extended-configparser[cli]`.
+
 ```python
 config = MyConfig("myconfig.cfg")
 # Load the configuration if existing. If it does not exist, a new configuration file with default values is created.
 config.load()
 # Inquire the user for the configuration values
 # Each ConfigEntry will be asked for its value
 config.inquire()
```

### Comparing `extended_configparser-1.0.0/pyproject.toml` & `extended_configparser-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "extended-configparser"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Valentin Schröter", email = "vasc9380@th-wildau.de" }]
 description = "Extended config parser."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = []
 
 classifiers = ["Programming Language :: Python :: 3"]
```

### Comparing `extended_configparser-1.0.0/PKG-INFO` & `extended_configparser-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: extended-configparser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Extended config parser.
 Project-URL: Homepage, https://github.com/vschroeter/extended-configparser
 Project-URL: Issues, https://github.com/vschroeter/extended-configparser/issues
 Author-email: Valentin Schröter <vasc9380@th-wildau.de>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -54,22 +54,23 @@
 
 ## Example Usage
 
 ```python
 from extended_configparser.parser import ExtendedConfigParser
 
 # Load the config
-config = ExtendedConfigParser()
-config.read("myconfig.cfg")
+parser = ExtendedConfigParser()
+parser.read("myconfig.cfg")
 
 # Use the configuration as usual
 ...
 
-# Update the configuration as usual
-...
+# Set sections / options together with comments
+parser.add_section("Section.New", comment="New Section with a comment")
+parser.set("Section.New", "new_option", "new_value", comment="New value with new comment")
 
 # Access and alter the comments of a section or an option
 comment = config.get_comment("Section.A")
 parser.set_comment("Section.A", comment = "New Section Comment")
 parser.set_comment("Section.A", "option1", comment = "New option comment")
 
 # Save the config back to the file
@@ -180,14 +181,17 @@
 ```
 
 ### Interactive Configuration
 
 Your configuration class can also be used for an interactive configuration setup.
 This is useful for the first setup of a configuration file.
 
+> [!NOTE]
+> To use the `config.inquire()` method, .you have to install the package in the cli configuration `pip install extended-configparser[cli]`.
+
 ```python
 config = MyConfig("myconfig.cfg")
 # Load the configuration if existing. If it does not exist, a new configuration file with default values is created.
 config.load()
 # Inquire the user for the configuration values
 # Each ConfigEntry will be asked for its value
 config.inquire()
```

