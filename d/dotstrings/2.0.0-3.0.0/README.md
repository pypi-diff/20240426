# Comparing `tmp/dotstrings-2.0.0.tar.gz` & `tmp/dotstrings-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotstrings-2.0.0.tar", max compression
+gzip compressed data, was "dotstrings-3.0.0.tar", max compression
```

## Comparing `dotstrings-2.0.0.tar` & `dotstrings-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1162 2023-08-09 07:57:55.854410 dotstrings-2.0.0/LICENSE
--rw-r--r--   0        0        0     1358 2023-08-09 07:57:55.854410 dotstrings-2.0.0/README.md
--rwxr-xr-x   0        0        0     6652 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/__init__.py
--rw-r--r--   0        0        0     1706 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/dot_strings_entry.py
--rw-r--r--   0        0        0     6852 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/dot_stringsdict_entry.py
--rw-r--r--   0        0        0     4562 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/genstrings.py
--rw-r--r--   0        0        0     5418 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/localized_bundle.py
--rw-r--r--   0        0        0     7069 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/localized_string.py
--rwxr-xr-x   0        0        0     5940 2023-08-09 07:57:55.854410 dotstrings-2.0.0/dotstrings/parser.py
--rw-r--r--   0        0        0     1099 2023-08-09 07:57:55.854410 dotstrings-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2288 1970-01-01 00:00:00.000000 dotstrings-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1162 2023-10-19 10:54:40.764978 dotstrings-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1358 2023-10-19 10:54:40.765150 dotstrings-3.0.0/README.md
+-rwxr-xr-x   0        0        0     6668 2024-04-23 06:34:38.846008 dotstrings-3.0.0/dotstrings/__init__.py
+-rw-r--r--   0        0        0     1681 2024-04-23 06:34:04.350586 dotstrings-3.0.0/dotstrings/dot_strings_entry.py
+-rw-r--r--   0        0        0     6960 2024-04-23 06:33:57.647784 dotstrings-3.0.0/dotstrings/dot_stringsdict_entry.py
+-rwxr-xr-x   0        0        0      112 2024-04-23 06:26:23.917514 dotstrings-3.0.0/dotstrings/exceptions.py
+-rw-r--r--   0        0        0     4623 2024-04-23 06:34:56.820933 dotstrings-3.0.0/dotstrings/genstrings.py
+-rw-r--r--   0        0        0     5495 2024-04-23 06:34:50.371371 dotstrings-3.0.0/dotstrings/localized_bundle.py
+-rw-r--r--   0        0        0     7174 2024-04-23 06:38:15.844151 dotstrings-3.0.0/dotstrings/localized_string.py
+-rwxr-xr-x   0        0        0     6011 2024-04-26 09:25:38.651419 dotstrings-3.0.0/dotstrings/parser.py
+-rw-r--r--   0        0        0     1095 2024-04-23 06:37:36.697716 dotstrings-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2340 1970-01-01 00:00:00.000000 dotstrings-3.0.0/PKG-INFO
```

### Comparing `dotstrings-2.0.0/LICENSE` & `dotstrings-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotstrings-2.0.0/README.md` & `dotstrings-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dotstrings-2.0.0/dotstrings/__init__.py` & `dotstrings-3.0.0/dotstrings/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities for dealing with .strings files"""
 
 import os
-from typing import Dict, List, Optional, Set
 
 from dotstrings.parser import load, loads, load_dict, loads_dict
 from dotstrings.dot_strings_entry import DotStringsEntry
 from dotstrings.dot_stringsdict_entry import DotStringsDictEntry, Variable
+from dotstrings.exceptions import DotStringsException
 from dotstrings.localized_bundle import LocalizedBundle
 from dotstrings.localized_string import LocalizedString
 
 
 def language_folder_path(strings_folder: str, language: str) -> str:
     """Generate the folder path for a language.
 
@@ -46,30 +46,30 @@
     :returns: The path to the strings file
     """
     return os.path.join(
         language_folder_path(stringsdict_folder, language), f"{table_name}.stringsdict"
     )
 
 
-def languages_in_folder(strings_folder: str) -> Set[str]:
+def languages_in_folder(strings_folder: str) -> set[str]:
     """Find all the languages in a folder
 
     This looks for *.lproj folders.
 
     :param strings_folder: The location of the strings folder (which contains
                            all the *.lproj folders)
 
     :returns: A set containing all the languages.
     """
     languages = os.listdir(strings_folder)
     languages = [language for language in languages if language.endswith(".lproj")]
     return {language.replace(".lproj", "") for language in languages}
 
 
-def load_table(strings_folder: str, language: str, table_name: str) -> List[LocalizedString]:
+def load_table(strings_folder: str, language: str, table_name: str) -> list[LocalizedString]:
     """Load the specified .strings table
 
     :param strings_folder: The location of the strings folder (which contains
                            all the *.lproj folders)
     :param language: The language code to load
     :param table_name: The name of the table to load
 
@@ -79,15 +79,15 @@
     table_path = strings_file_path(strings_folder, language, table_name)
     strings = load(table_path)
     return LocalizedString.from_dotstring_entries(
         entries=strings, language=language, table=table_name
     )
 
 
-def load_language_tables(strings_folder: str, language: str) -> Dict[str, List[LocalizedString]]:
+def load_language_tables(strings_folder: str, language: str) -> dict[str, list[LocalizedString]]:
     """Load the .strings tables for a given language
 
     :param strings_folder: The location of the strings folder (which contains
                            all the *.lproj folders)
     :param language: The language code to load
 
     :returns: A dictionary of results. The key is the table, the value is the
@@ -125,15 +125,15 @@
         results[language] = load_language_tables(strings_folder, language)
 
     return LocalizedBundle(results)
 
 
 def normalize(
     strings_path: str,
-    output_path: Optional[str] = None,
+    output_path: str | None = None,
     remove_duplicates: bool = True,
     sort_comments: bool = True,
 ) -> None:
     """Load in the specified .strings table, normalize it, and write it back out.
 
     Normalizing consists of sorting by key, then comments, and (usually)
     deduplicating before writing back out.
@@ -161,15 +161,15 @@
         if deduped_entries[-1].key != entry.key:
             deduped_entries.append(entry)
             continue
 
         # If we have duplicate keys but the values don't match, that's an
         # exception, whether or not we are removing duplicates
         if deduped_entries[-1].value != entry.value or not remove_duplicates:
-            raise Exception(f"Found duplicate strings with key: {entry.key}")
+            raise DotStringsException(f"Found duplicate strings with key: {entry.key}")
 
         deduped_entries[-1].comments.extend(entry.comments)
 
     if sort_comments:
         for entry in deduped_entries:
             entry.comments = list(set(entry.comments))
             entry.comments.sort()
```

### Comparing `dotstrings-2.0.0/dotstrings/dot_strings_entry.py` & `dotstrings-3.0.0/dotstrings/dot_strings_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """Base types for the dotstrings library."""
 
-from typing import List
-
 
 class DotStringsEntry:
     """Represents a .strings entry.
 
     :param key: The key for the entry
     :param value: The value for the entry
     :param comments: Any comments associated with the entry
     """
 
     key: str
     value: str
-    comments: List[str]
+    comments: list[str]
 
-    def __init__(self, key: str, value: str, comments: List[str]) -> None:
+    def __init__(self, key: str, value: str, comments: list[str]) -> None:
         self.key = key
         self.value = value
         self.comments = comments
 
     def strings_format(self) -> str:
         """Return the entry as would be formatted in a .strings file
```

### Comparing `dotstrings-2.0.0/dotstrings/dot_stringsdict_entry.py` & `dotstrings-3.0.0/dotstrings/dot_stringsdict_entry.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base types for the dotstrings library."""
 
-from typing import Optional
+from dotstrings.exceptions import DotStringsException
 
 VARIABLE_VALUE_TYPE_KEY = "NSStringFormatValueTypeKey"
 VARIABLE_VALUE_SPEC_KEY = "NSStringFormatSpecTypeKey"
 FORMAT_KEY = "NSStringLocalizedFormatKey"
 
 VARIABLE_VALUE_SPEC_PLURAL = "NSStringPluralRuleType"
 
@@ -17,21 +17,21 @@
     :param one_value: Value for one
     :param two_value: Value for two
     :param few_value: Value for few
     :param many_value: Value for many
     :param other_value: Value for other
     """
 
-    value_type: Optional[str]
-    zero_value: Optional[str]
-    one_value: Optional[str]
-    two_value: Optional[str]
-    few_value: Optional[str]
-    many_value: Optional[str]
-    other_value: Optional[str]
+    value_type: str | None
+    zero_value: str | None
+    one_value: str | None
+    two_value: str | None
+    few_value: str | None
+    many_value: str | None
+    other_value: str | None
 
     def __init__(self) -> None:
         self.value_type = None
         self.zero_value = None
         self.one_value = None
         self.two_value = None
         self.few_value = None
@@ -46,22 +46,24 @@
 
         :returns: The parsed stringsdict variable entry
         """
         # Check NSStringFormatSpecTypeKey, should always be NSStringPluralRuleType
 
         variable = Variable()
         if VARIABLE_VALUE_SPEC_KEY not in contents:
-            raise Exception("NSStringFormatSpecTypeKey missing in entry")
+            raise DotStringsException("NSStringFormatSpecTypeKey missing in entry")
 
         if contents[VARIABLE_VALUE_SPEC_KEY] != VARIABLE_VALUE_SPEC_PLURAL:
-            raise Exception("Value of NSStringFormatSpecTypeKey is not NSStringPluralRuleType")
+            raise DotStringsException(
+                "Value of NSStringFormatSpecTypeKey is not NSStringPluralRuleType"
+            )
 
         # When initializing from a dict (parsing), be sure NSStringFormatValueTypeKey exists
         if VARIABLE_VALUE_TYPE_KEY not in contents:
-            raise Exception("NSStringFormatValueTypeKey missing in entry")
+            raise DotStringsException("NSStringFormatValueTypeKey missing in entry")
 
         variable.value_type = contents[VARIABLE_VALUE_TYPE_KEY]
 
         variable.zero_value = contents.get("zero")
         variable.one_value = contents.get("one")
         variable.two_value = contents.get("two")
         variable.few_value = contents.get("few")
@@ -112,15 +114,15 @@
         self.variables = variables
 
     def stringsdict_format(self) -> dict:
         """Return the entry as would be formatted in a .stringsdict file
 
         :returns: The dict representation of this entry
         """
-        result = {}
+        result: dict[str, str | dict[str, str]] = {}
         result[FORMAT_KEY] = self.value
         for variable_name, variable in self.variables.items():
             variable_dict = {}
             variable_dict[VARIABLE_VALUE_SPEC_KEY] = VARIABLE_VALUE_SPEC_PLURAL
             if variable.value_type is not None:
                 variable_dict[VARIABLE_VALUE_TYPE_KEY] = variable.value_type
             if variable.zero_value is not None:
@@ -161,15 +163,15 @@
 
         :param key: The key of the entry
         :param contents: The contents of the entry
 
         :returns: The parsed stringsdict entry
         """
         if FORMAT_KEY not in contents:
-            raise Exception("NSStringLocalizedFormatKey missing in entry")
+            raise DotStringsException("NSStringLocalizedFormatKey missing in entry")
 
         entry_format = contents[FORMAT_KEY]
 
         variables = {}
         for variable_name, variable_entry in contents.items():
             if variable_name == FORMAT_KEY:
                 # Ignore the format key
```

### Comparing `dotstrings-2.0.0/dotstrings/genstrings.py` & `dotstrings-3.0.0/dotstrings/genstrings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Wrapper around the genstrings command"""
 
 import os
 import shutil
 import subprocess
 import tempfile
-from typing import List
+
+from dotstrings.exceptions import DotStringsException
 
 
 def _convert_to_utf8(file_path: str) -> None:
     """Take a UTF-16 file and convert to UTF-8.
 
     NOTE: This will replace the existing file
 
@@ -18,21 +19,21 @@
     """
 
     temp_file_path = tempfile.mktemp()
 
     iconv_command = f'iconv -f UTF-16 -t UTF-8 "{file_path}" > "{temp_file_path}"'
 
     if subprocess.run(iconv_command, shell=True, check=False).returncode != 0:
-        raise Exception("Unable to convert from UTF-16 to UTF-8!")
+        raise DotStringsException("Unable to convert from UTF-16 to UTF-8!")
 
     shutil.move(temp_file_path, file_path)
 
 
 def generate_strings(
-    *, output_directory: str, file_paths: List[str], clear_existing: bool = True
+    *, output_directory: str, file_paths: list[str], clear_existing: bool = True
 ) -> None:
     """Run the genstrings command over the files passed in.
 
     Genstrings scans code files for usage of the `NSLocalizedString` macro. It
     the generates the corresponding .strings file from these. e.g. If you have:
 
     ```objc
@@ -49,15 +50,15 @@
 
     However, if you specify a table in your `NSLocalizedString` call, then
     instead of using the default `Localizable.strings` file, it will generate
     `MyTable.strings`.
 
     :param str output_directory: The location to place the output files (this
                                  folder will contain an en.lproj folder after)
-    :param List[str] file_paths: The paths to the files that should be scanned
+    :param list[str] file_paths: The paths to the files that should be scanned
     :param bool clear_existing: Set to True when the existing files in the
                                 output directory should be wiped before
                                 generating the new strings. Defaults to True.
 
     :raises Exception: If we can't generate the .strings files
     """
 
@@ -106,17 +107,17 @@
             # until the end of the command and then decoding, we avoid this
             # issue.
             output = output_bytes.decode("utf-8", errors="backslashreplace")
 
             output = output.strip()
 
             if len(output) > 0:
-                raise Exception(f"Encountered an error generating strings: {output}")
+                raise DotStringsException(f"Encountered an error generating strings: {output}")
         except subprocess.CalledProcessError as ex:
-            raise Exception(f"Unable generate .strings files! {ex}") from ex
+            raise DotStringsException(f"Unable generate .strings files! {ex}") from ex
 
     # Convert all .strings files to UTF-8
     for file_name in os.listdir(english_strings_directory):
         file_path = os.path.join(english_strings_directory, file_name)
         # Check for file type and .strings extension
         if file_name.endswith(".strings") and os.path.isfile(file_path):
             _convert_to_utf8(file_path)
```

### Comparing `dotstrings-2.0.0/dotstrings/localized_bundle.py` & `dotstrings-3.0.0/dotstrings/localized_bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """Representation of a localized bundle."""
 
-from typing import cast, Dict, List, Set
+from typing import cast
 
+from dotstrings.exceptions import DotStringsException
 from dotstrings.localized_string import LocalizedString
 
 
 class LocalizedBundle:
     """Representation of a localized bundle.
 
     :param raw_entries: The raw dictionary entries that were parsed from disk
     """
 
-    def __init__(self, raw_entries: Dict[str, Dict[str, List[LocalizedString]]]) -> None:
+    def __init__(self, raw_entries: dict[str, dict[str, list[LocalizedString]]]) -> None:
         self.raw_entries = raw_entries
 
-    def languages(self) -> List[str]:
+    def languages(self) -> list[str]:
         """Return the languages supported in the bundle
 
         :returns: A list of language codes
         """
         return list(self.raw_entries.keys())
 
-    def table_names(self, validate_identical: bool = False) -> List[str]:
+    def table_names(self, validate_identical: bool = False) -> list[str]:
         """Return the tables in the bundle.
 
         :param validate_identical: Set to True to confirm all languages have the
                                    same tables in them
 
         :returns: A list of table names
         """
 
         if validate_identical:
 
             # Build up a map of languages to table names
 
-            found_tables: Dict[str, Set[str]] = {}
+            found_tables: dict[str, set[str]] = {}
             for language, table_map in self.raw_entries.items():
                 # table_map is a dictionary of names to lists of strings
                 found_tables[language] = set(table_map.keys())
 
             if len(found_tables) == 0:
                 return []
 
@@ -46,53 +47,53 @@
             base_language_tables = found_tables[base_language]
 
             for language, table_names in found_tables.items():
                 extra_tables = table_names - base_language_tables
                 missing_tables = base_language_tables - table_names
 
                 if len(extra_tables) > 0:
-                    raise Exception(
+                    raise DotStringsException(
                         f"The following table names were in {language}"
                         + f" but not in {base_language}: {extra_tables}"
                     )
 
                 if len(missing_tables) > 0:
-                    raise Exception(
+                    raise DotStringsException(
                         f"The following table names were in {base_language}"
                         + f" but not in {language}: {missing_tables}"
                     )
 
             return list(base_language_tables)
 
         all_table_names = set()
 
         for table_map in self.raw_entries.values():
             for table in table_map.keys():
                 all_table_names.add(table)
 
         return list(all_table_names)
 
-    def tables_for_language(self, language: str) -> Dict[str, List[LocalizedString]]:
+    def tables_for_language(self, language: str) -> dict[str, list[LocalizedString]]:
         """Return the tables for a language.
 
         :param language: The language to get the tables for
 
         :returns: A dictionary of table names to lists of strings
         """
         sentinel = object()
         result = self.raw_entries.get(language, sentinel)
 
         if result is sentinel:
-            raise Exception(f"There were no entries for language: {language}")
+            raise DotStringsException(f"There were no entries for language: {language}")
 
-        return cast(Dict[str, List[LocalizedString]], result)
+        return cast(dict[str, list[LocalizedString]], result)
 
     def table_for_languages(
         self, table: str, *, allow_missing: bool = False
-    ) -> Dict[str, List[LocalizedString]]:
+    ) -> dict[str, list[LocalizedString]]:
         """Return a dictionary of languages to strings for a given table.
 
         :param table: The table to load the data for
         :param bool allow_missing: Set to True to allow a table to be missing for any languages
 
         :returns: A dictionary of language codes to a list of strings
         """
@@ -102,23 +103,23 @@
             sentinel = object()
             table_data = table_map.get(table, sentinel)
 
             if table_data is sentinel and language == "Base":
                 continue
 
             if table_data is sentinel and not allow_missing:
-                raise Exception(f"Could not find table {table} for language {language}")
+                raise DotStringsException(f"Could not find table {table} for language {language}")
 
-            results[language] = cast(List[LocalizedString], table_data)
+            results[language] = cast(list[LocalizedString], table_data)
 
         return results
 
     def tables(
         self, *, validate_missing: bool = True
-    ) -> Dict[str, Dict[str, List[LocalizedString]]]:
+    ) -> dict[str, dict[str, list[LocalizedString]]]:
         """Return the entries in the bundle, first keyed by table, then by language.
 
         :param bool validate_missing: Set to False to disable the check that a table exists for every language
 
         Example response:
 
         ```
```

### Comparing `dotstrings-2.0.0/dotstrings/localized_string.py` & `dotstrings-3.0.0/dotstrings/localized_string.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Localized string types"""
 
 import hashlib
 import re
-from typing import ClassVar, List, Optional, Pattern
+from typing import ClassVar, Pattern
 
 from dotstrings.dot_strings_entry import DotStringsEntry
+from dotstrings.exceptions import DotStringsException
 
 
 class LocalizedString:
     """Represents a localized string.
 
     Note: Automatic key generation is supported. By this, if you pass None as
     the value for your `key`, the value will automatically be derived as a hash
@@ -16,65 +17,68 @@
     for your default language (as the key will change between languages).
 
     The reason we support this is that this is a useful class to use in various
     projects, not just as the result of reading .strings files. In those cases,
     you may wish to automatically generate keys to avoid having to manually
     deal with deduplication.
 
-    :param Optional[str] key: The key for the string. If this is None, they key
+    :param str | None key: The key for the string. If this is None, they key
                               will be automatically derived from the value and
                               the key extension.
     :param str value: The value of the string
     :param str language: The language code of the string
     :param str table: The string table to use
-    :param Optional[str] comment: The comment for the string
-    :param Optional[str] key_extension: The key extension to differentiate
+    :param str | None comment: The comment for the string
+    :param str | None key_extension: The key extension to differentiate
                                         between identical strings with different
                                         meanings
     :param str bundle: The bundle the string can be found in
     """
 
-    _TOKEN_REGEX: ClassVar[
-        str
-    ] = r"(%(?:[0-9]+\$)?[0-9]*\.?[0-9]*[a-zA-Z]{0,2}[dDuUxXoOfFeEgGcCsSaAp@])"
+    _TOKEN_REGEX: ClassVar[str] = (
+        r"(%(?:[0-9]+\$)?[0-9]*\.?[0-9]*[a-zA-Z]{0,2}[dDuUxXoOfFeEgGcCsSaAp@])"
+    )
     _TOKEN_PATTERN: ClassVar[Pattern] = re.compile(_TOKEN_REGEX, flags=re.DOTALL)
 
     key: str
     value: str
     language: str
     table: str
-    comment: Optional[str]
-    key_extension: Optional[str]
+    comment: str | None
+    key_extension: str | None
     bundle: str
 
+    # pylint: disable=too-many-arguments
     def __init__(
         self,
         *,
-        key: Optional[str],
+        key: str | None,
         value: str,
         language: str,
         table: str,
-        comment: Optional[str] = None,
-        key_extension: Optional[str] = None,
+        comment: str | None = None,
+        key_extension: str | None = None,
         bundle: str = "",
     ) -> None:
         self.value = value
         self.language = language
         self.comment = comment
         self.key_extension = key_extension
         self.table = table
         self.bundle = bundle
 
         if key is not None:
             self.key = key
         else:
             self.key = LocalizedString._calculate_key(value=value, key_extension=key_extension)
 
+    # pylint: enable=too-many-arguments
+
     @staticmethod
-    def _calculate_key(*, value: str, key_extension: Optional[str]) -> str:
+    def _calculate_key(*, value: str, key_extension: str | None) -> str:
         """Calculate the unique key to use for this string.
 
         :param value: The value of the localized string
         :param key_extension: Any key extension value to use to differentiate
                               between identical values
 
         :returns: The unique key for the string
@@ -89,30 +93,30 @@
         hash_input = hash_input.replace("\\n", "\n")  # Replace "slash n" with newline character
         hash_input = hash_input.replace('\\"', '"')  # Replace "slash quote" with quote character
 
         key = hashlib.md5(hash_input.encode("utf-8")).hexdigest()
 
         return key
 
-    def tokens(self) -> List[str]:
+    def tokens(self) -> list[str]:
         """Find and return the tokens in the string.
 
         :returns: The list of tokens in the string
         """
         return LocalizedString._TOKEN_PATTERN.findall(self.value)
 
     def ns_localized_format(self) -> str:
         """Return the NSLocalizedString version of our call.
 
         :returns: The NSLocalizedString version of our call
 
         :raises Exception: If the language is not English
         """
         if self.language != "en":
-            raise Exception(f"This should only be called for English strings: {self}")
+            raise DotStringsException(f"This should only be called for English strings: {self}")
         return (
             "NSLocalizedStringWithDefaultValue("
             + f'@"{self.key}", @"{self.table}", @"{self.bundle}", @"{self.value}", @"{self.comment}");'
         )
 
     def __eq__(self, other: object) -> bool:
         """Determine if the supplied object is equal to self
@@ -182,19 +186,19 @@
 
         :return: A string representation of the object
         """
         return self.__repr__()
 
     @staticmethod
     def from_dotstring_entries(
-        *, entries: List[DotStringsEntry], language: str, table: str
-    ) -> List["LocalizedString"]:
+        *, entries: list[DotStringsEntry], language: str, table: str
+    ) -> list["LocalizedString"]:
         """Convert a list of DotStringsEntry's into a list of LocalizedString's
 
-        :param List[DotStringsEntry] entries: The DotStringsEntry's to convert
+        :param list[DotStringsEntry] entries: The DotStringsEntry's to convert
         :param str language: The language the DotStringsEntry's are in
         :param str table: The table the DotStringsEntry's are from
 
         :returns: A list of LocalizedStrings
         """
 
         output = []
```

### Comparing `dotstrings-2.0.0/dotstrings/parser.py` & `dotstrings-3.0.0/dotstrings/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Utilities for dealing with .strings files"""
 
 import plistlib
 import re
-from typing import BinaryIO, List, Optional, Pattern, TextIO, Union
+from typing import BinaryIO, Pattern, TextIO
 
+from dotstrings.exceptions import DotStringsException
 from dotstrings.dot_strings_entry import DotStringsEntry
 from dotstrings.dot_stringsdict_entry import DotStringsDictEntry
 
 
 class Patterns:
     """The patterns used by the parser."""
 
     comment = re.compile(r"(\'(?:[^\'\\]|\\[\s\S])*\')|//.*|/\*(?:[^*]|\*(?!/))*\*/", re.MULTILINE)
     whitespace = re.compile(r"\s*", re.MULTILINE)
-    entry = re.compile(r'"(.*)" = "(.*)";')
+    entry = re.compile(r'"(.*)"\s*=\s*"(.*)";')
 
 
 class Scanner:
     """Regex string scanner."""
 
     string: str
     offset: int
@@ -29,15 +30,15 @@
     def has_more(self) -> bool:
         """Check if there is more string remaining.
 
         :returns: True if there is more string remaining, False otherwise
         """
         return self.offset < len(self.string)
 
-    def scan(self, pattern: Union[str, Pattern], flags: int = 0) -> Optional[str]:
+    def scan(self, pattern: str | Pattern, flags: int = 0) -> str | None:
         """Scan a string for a pattern and return the string if found.
 
         :param pattern: The pattern to scan for
         :param flags: Any flags to use for a string pattern
 
         :returns: The string if the pattern matches, None otherwise.
         """
@@ -52,15 +53,15 @@
         if match is not None:
             self.offset = match.end()
             return match.group(0)
 
         return None
 
 
-def load(file_details: Union[TextIO, str], encoding: Optional[str] = None) -> List[DotStringsEntry]:
+def load(file_details: TextIO | str, encoding: str | None = None) -> list[DotStringsEntry]:
     """Parse the contents of a .strings file from a file pointer.
 
     :param file_details: The file pointer or a file path
     :param encoding: The encoding the file is in
 
     :returns: A list of `DotStringEntry`s
     """
@@ -79,30 +80,30 @@
     for encoding_option in encoding_list:
         try:
             with open(file_details, "r", encoding=encoding_option) as strings_file:
                 return load(strings_file)
         except UnicodeDecodeError:
             pass
 
-    raise Exception(f"Could not determine encoding for file at path: {file_details}")
+    raise DotStringsException(f"Could not determine encoding for file at path: {file_details}")
 
 
-def loads(contents: str) -> List[DotStringsEntry]:
+def loads(contents: str) -> list[DotStringsEntry]:
     """Parse the contents of a .strings file.
 
     Note: CRLF is not supported in strings.
 
     :param contents: The contents of a .strings file
 
     :returns: A list of `DotStringsEntry`s"""
 
     # Sometimes we have CRLF. It's easier to just replace now. This could, in
     # theory, cause issues, but we just don't support it for now.
     if "\r\n" in contents:
-        raise Exception("Strings contain CRLF")
+        raise DotStringsException("Strings contain CRLF")
     contents = contents.replace("\r\n", "\n")
 
     scanner = Scanner(contents)
 
     strings = []
 
     # Main parse loop
@@ -137,31 +138,31 @@
             _ = scanner.scan(Patterns.whitespace)
 
         # Get the entry line
         entry = scanner.scan(Patterns.entry)
 
         if entry is None:
             if scanner.has_more():
-                raise Exception(f"Expected an entry at offset {scanner.offset}")
+                raise DotStringsException(f"Expected an entry at offset {scanner.offset}")
             break
 
         # Now extract the key and value
         entry_matches = Patterns.entry.search(entry)
         if not entry_matches:
-            raise Exception(f"Failed to parse entry at offset {scanner.offset}")
+            raise DotStringsException(f"Failed to parse entry at offset {scanner.offset}")
 
         key = entry_matches.group(1)
         value = entry_matches.group(2)
 
         strings.append(DotStringsEntry(key, value, comments))
 
     return strings
 
 
-def load_dict(file_details: Union[BinaryIO, str]) -> List[DotStringsDictEntry]:
+def load_dict(file_details: BinaryIO | str) -> list[DotStringsDictEntry]:
     """Parse the contents of a .stringsdict file from a file pointer.
 
     :param file_details: The file pointer or a file path
 
     :returns: A list of `DotStringEntry`s
     """
 
@@ -170,28 +171,28 @@
         contents = file_details.read()
         return loads_dict(contents)
 
     with open(file_details, "rb") as stringsdict_file:
         return load_dict(stringsdict_file)
 
 
-def loads_dict(contents: bytes) -> List[DotStringsDictEntry]:
+def loads_dict(contents: bytes) -> list[DotStringsDictEntry]:
     """Parse the contents of a .stringsdict file from binary data.
 
     :param contents: The binary data of a .stringsdict file
 
     :returns: A list of `DotStringEntry`s
     """
 
     strings_dict = plistlib.loads(contents)
 
     if not isinstance(strings_dict, dict):
-        raise Exception("stringsdict format is incorrect")
+        raise DotStringsException("stringsdict format is incorrect")
 
     entries = []
     for key, entry in strings_dict.items():
         if not isinstance(entry, dict):
-            raise Exception("stringsdict entry format is incorrect")
+            raise DotStringsException("stringsdict entry format is incorrect")
 
         entries.append(DotStringsDictEntry.parse(key, entry))
 
     return entries
```

### Comparing `dotstrings-2.0.0/pyproject.toml` & `dotstrings-3.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dotstrings"
-version = "2.0.0"
+version = "3.0.0"
 description = "Tools for dealing with the .strings files for iOS and macOS"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
@@ -27,20 +27,20 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Software Development',
     'Topic :: Utilities'
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.10"
 
 [tool.poetry.dev-dependencies]
-black = "^22.10.0"
-mypy = "^0.991"
-pylint = "^2.15.6"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
+black = "24.4.0"
+mypy = "1.9.0"
+pylint = "3.1.0"
+pytest = "^8.1.0"
+pytest-cov = "^5.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dotstrings-2.0.0/PKG-INFO` & `dotstrings-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: dotstrings
-Version: 2.0.0
+Version: 3.0.0
 Summary: Tools for dealing with the .strings files for iOS and macOS
 Home-page: https://github.com/Microsoft/dotstrings
 License: MIT
 Keywords: localization,iOS,macOS,strings
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Project-URL: Repository, https://github.com/Microsoft/dotstrings
 Description-Content-Type: text/markdown
 
 # dotstrings
```

