# Comparing `tmp/pyap2-0.0.1.tar.gz` & `tmp/pyap2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyap2-0.0.1.tar", max compression
+gzip compressed data, was "pyap2-0.1.0.tar", max compression
```

## Comparing `pyap2-0.0.1.tar` & `pyap2-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1085 2024-04-22 17:02:55.315520 pyap2-0.0.1/LICENSE
--rw-r--r--   0        0        0     2189 2024-04-22 17:02:55.315520 pyap2-0.0.1/README.rst
--rw-r--r--   0        0        0      225 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/address.py
--rw-r--r--   0        0        0      741 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/api.py
--rw-r--r--   0        0        0      534 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/exceptions.py
--rw-r--r--   0        0        0     4289 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/parser.py
--rw-r--r--   0        0        0        0 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/py.typed
--rw-r--r--   0        0        0        0 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_CA/__init__.py
--rw-r--r--   0        0        0    21374 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_CA/data.py
--rw-r--r--   0        0        0        0 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_GB/__init__.py
--rw-r--r--   0        0        0    15020 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_GB/data.py
--rw-r--r--   0        0        0        0 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_US/__init__.py
--rw-r--r--   0        0        0    25298 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/source_US/data.py
--rw-r--r--   0        0        0     1060 2024-04-22 17:02:55.315520 pyap2-0.0.1/pyap/utils.py
--rw-r--r--   0        0        0     2418 2024-04-22 17:03:08.123457 pyap2-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 pyap2-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-04-26 11:07:29.455882 pyap2-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2189 2024-04-26 11:07:29.455882 pyap2-0.1.0/README.rst
+-rw-r--r--   0        0        0      225 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/address.py
+-rw-r--r--   0        0        0      741 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/api.py
+-rw-r--r--   0        0        0      534 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/exceptions.py
+-rw-r--r--   0        0        0     4289 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/parser.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/py.typed
+-rw-r--r--   0        0        0        0 2024-04-26 11:07:29.455882 pyap2-0.1.0/pyap/source_CA/__init__.py
+-rw-r--r--   0        0        0    21374 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_CA/data.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_GB/__init__.py
+-rw-r--r--   0        0        0    15020 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_GB/data.py
+-rw-r--r--   0        0        0        0 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_US/__init__.py
+-rw-r--r--   0        0        0    26198 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/source_US/data.py
+-rw-r--r--   0        0        0     1060 2024-04-26 11:07:29.459882 pyap2-0.1.0/pyap/utils.py
+-rw-r--r--   0        0        0     2418 2024-04-26 11:07:47.016028 pyap2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 pyap2-0.1.0/PKG-INFO
```

### Comparing `pyap2-0.0.1/LICENSE` & `pyap2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/README.rst` & `pyap2-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/address.py` & `pyap2-0.1.0/pyap/address.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/api.py` & `pyap2-0.1.0/pyap/api.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/exceptions.py` & `pyap2-0.1.0/pyap/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/parser.py` & `pyap2-0.1.0/pyap/parser.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/source_CA/data.py` & `pyap2-0.1.0/pyap/source_CA/data.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/source_GB/data.py` & `pyap2-0.1.0/pyap/source_GB/data.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyap/source_US/data.py` & `pyap2-0.1.0/pyap/source_US/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     :copyright: (c) 2015 by Vladimir Goncharov.
     :license: MIT, see LICENSE for more details.
 """
 
 import string
 from typing import List
+from typing import Optional
 
 
 def str_list_to_upper_lower_regex(str_list: List[str]) -> str:
     regex = "|".join(set(str_list)).lower()
     for letter in string.ascii_lowercase:
         regex = regex.replace(
             letter, "[{upper}{lower}]".format(upper=letter.upper(), lower=letter)
@@ -155,17 +156,19 @@
                     (?:
                         [Nn][Oo][Rr][Tt][Hh]|
                         [Ss][Oo][Uu][Tt][Hh]|
                         [Ee][Aa][Ss][Tt]|
                         [Ww][Ee][Ss][Tt]
                     )
                     |
-                    (?:NW|NE|SW|SE)\b
+                    \b(?:NW|NE|SW|SE)\b
                     |
-                    (?:N|S|E|W)\b\.?
+                    \b(?:N\.W\.|N\.E\.|S\.W\.|S\.E\.)
+                    |
+                    \b(?:N|S|E|W)\b\.?
                 )
                 """
 
 numbered_avenue_re = r"""
                 (?:{post_direction_re}\ [Aa][Vv][Ee](?:\.|[Nn][Uu][Ee])?\ \d{{1,2}})
 """.format(
     post_direction_re=post_direction_re
@@ -585,14 +588,15 @@
     "Point",
     "Points",
     "Port",
     "Ports",
     "Pr",
     "Prairie",
     "Prk",
+    "Promenade",
     "Prr",
     "Prt",
     "Prts",
     "Psge",
     "Pt",
     "Pts",
     "Rad",
@@ -763,15 +767,15 @@
     "Xrd",
     "Xrds",
 ]
 
 street_type_leading_list = ["Camino", "El\ Camino"]
 
 
-def street_type_list_to_regex(street_type_list):
+def street_type_list_to_regex(street_type_list: list[str]) -> str:
     """Converts a list of street types into a regex"""
     street_types = str_list_to_upper_lower_regex(street_type_list)
 
     # Use \b to check that there are word boundaries before and after the street type
     # Optionally match zero to two of " ", ",", or "." after the street name
     street_types = street_types.replace("|", r"\b|\b")
     street_types = r"\b" + r"(?:" + street_types + r")" + r"\b\.?"
@@ -797,22 +801,26 @@
 )
 
 
 typed_street_name = r"""
             (?:      
                 (?:{street_name_a}{space_div}{street_type_a})
                 |
-                (?:{street_type_b}{space_div}{street_name_b})
+                (?:
+                    (?:{post_direction_re}{space_div})?
+                    {street_type_b}{space_div}{street_name_b}
+                )
             )
 """.format(
     space_div=space_div,
     street_name_a=rf"(?P<street_name_a>{street_name_multi_word_re})",
     street_type_a=street_type_extended,
     street_type_b=rf"(?P<street_type_b>{street_types_leading_re})",
     street_name_b=rf"(?P<street_name_b>{street_name_one_word_re})",
+    post_direction_re=post_direction_re,
 )
 
 floor_indic = r"""
             (?:
                 (?:[Ff][Ll][Oo][Oo][Rr]|[Ff][Ll][Rr]?\.?)
                 (?:\ (?:[Hh][Oo][Rr][Ii][Zz][Oo][Nn][Tt][Aa][Ll]|[Hh][Oo][Rr][Ii][Zz]))?
             )
@@ -887,14 +895,16 @@
                             |
                             # Bay
                             [Bb][Aa][Yy]
                         )\b[\ \,\.]+
                         (?:
                             [A-Za-z\#\&\-\d]{1,7}(?:\s?[SWNE])?
                         )?
+                        |
+                        \d{2,4}\ [Ss][Tt][Ee](?:\ \*)?
                     )
                     |
                     (?:
                         \#\ ?[0-9]{,4}[A-Za-z]{1}
                     )
                     |
                     (?:
@@ -924,15 +934,15 @@
                 |
                 (?:[Dd][Rr][Aa][Ww][Ee][Rr]\ +[A-Z]\b)
             )
         """
 
 phone_number = r"""
             (?:
-                \*?
+                \*?(?:[Pp][Hh]\ )?
                 (?P<phone_number>
                     \(?\d{3}\)?\-?\ ?\d{3}\-?\ ?\-?\d{4}
                 )
             )
             """
 
 part_div = r"(?:[\,\s]{1,3}|\ \-\ |$)"  # allows for line breaks
@@ -946,15 +956,15 @@
                 (?:
                     (?:{typed_street_name}(?![A-Za-z\d\.]))
                     |
                     (?:{single_street_name})
                     |
                     (?:
                         {post_direction_re}\ 
-                        [A-z0-9\.\-]{{2,31}}
+                        \d{{,3}}[A-Za-z\-]{{1,31}}
                     )
                 )
                 (?:{space_div}{post_direction})?
                 (?:{part_div}{floor})?
                 (?:{part_div}{building})?
                 (?:{part_div}{occupancy})?
                 (?:{part_div}(?P<po_box_a>{po_box}))?
@@ -974,48 +984,48 @@
     building=building,
     occupancy=occupancy,
     po_box=po_box,
 )
 
 
 def states_abbrvs_regex() -> str:
-    state_abbrs = [
+    # Some abbreviations are non-standard
+    _STATE_ABBRS = {
         "AL",
         "AK",
         "AZ",
         "AR",
         "CA",
         "CO",
         "CT",
         "DE",
-        "DC",
         "FL",
         "GA",
         "HI",
         "ID",
         "IL",
         "IN",
         "IA",
         "KS",
         "KY",
         "LA",
         "ME",
         "MD",
         "MA",
-        "MI(?:CH)?",
+        "MI(?:CH)?\.?",
         "MN",
         "MS",
         "MO",
         "MT",
         "NE",
         "NV",
         "NH",
         "NJ",
         "NM",
-        "NY",
+        "NY|N\.Y\.",
         "NC",
         "ND",
         "OH",
         "OK",
         "OR",
         "PA",
         "RI",
@@ -1026,33 +1036,35 @@
         "UT",
         "VT",
         "VA",
         "WA",
         "WV",
         "WI",
         "WY",
-        # unincorporated & commonwealth territories
+    }
+    _NON_STATE_ABBRS = {
         "AS",
         "GU",
         "MP",
         "PR",
         "VI",
-    ]
-
-    def to_abbr_with_optional_dots(abbr: str) -> str:
-        return "".join((c + r"\.?") if c in string.ascii_uppercase else c for c in abbr)
-
-    return str_list_to_upper_lower_regex(
-        [to_abbr_with_optional_dots(abbr) for abbr in state_abbrs]
+        "D\.?C\.?",
+    }
+    return (
+        r"(?:"
+        + str_list_to_upper_lower_regex(list(_STATE_ABBRS | _NON_STATE_ABBRS))
+        + r")(?![A-Za-z])"
     )
 
 
 # region1 is actually a "state"
-region1 = r"""
-        (?P<region1>
+def make_region1(idx: Optional[str] = None):
+    maybe_idx = f"_{idx}" if idx else ""
+    return r"""
+        (?P<region1{maybe_idx}>
             (?:
                 # states full
                 [Aa][Ll][Aa][Bb][Aa][Mm][Aa]|
                 [Aa][Ll][Aa][Ss][Kk][Aa]|
                 [Aa][Rr][Ii][Zz][Oo][Nn][Aa]|
                 [Aa][Rr][Kk][Aa][Nn][Ss][Aa][Ss]|
                 [Cc][Aa][Ll][Ii][Ff][Oo][Rr][Nn][Ii][Aa]|
@@ -1114,16 +1126,17 @@
             |
             (?:
                 # states abbreviations
                 {state_abbrvs}
             )
         )
         """.format(
-    state_abbrvs=states_abbrvs_regex()
-)
+        state_abbrvs=states_abbrvs_regex(), maybe_idx=maybe_idx
+    )
+
 
 # TODO: doesn't catch cities containing French characters
 # We require short city names to contain a vowel
 city = r"""
         (?P<city>
             [A-Za-z]{1}[a-zA-Z\ \-\'\.]{3,20}?
             |
@@ -1133,55 +1146,66 @@
             |
             [A-Za-z][AaEeIiUuOo][A-Za-z]
             |
             [A-Za-z]{2}[AaEeIiUuOoYy]
         )
         """
 
-postal_code = r"""
-            (?P<postal_code>
-                (?:\d{5}(?:\-\d{4})?(?!\d))
-            )
-            """
+postal_code_re = r"""(?:\d{5}(?:\-\d{4})?(?!\d))"""
+postal_code = rf"""(?P<postal_code>{postal_code_re})"""
 
 country = r"""
             (?:
-                [Uu]\.?[Ss]\.?[Aa]\.?|
+                [Uu]\.?[Ss]\.?(?:[Aa]\.?)?|
                 [Uu][Nn][Ii][Tt][Ee][Dd]\ [Ss][Tt][Aa][Tt][Ee][Ss](?:\ [Oo][Ff]\ [Aa][Mm][Ee][Rr][Ii][Cc][Aa])?
             )
             """
 
 
+def make_region1_postal_code(
+    part_div: str = part_div, postal_code: str = postal_code
+) -> str:
+    """This should match region1 (state) and postal code each at most once,
+    but require at least one of the two."""
+
+    def _indexed_region1(idx: Optional[str] = None):
+        return rf"""(?:{part_div} {make_region1(idx)})"""
+
+    _postal_code = f"""(?:{part_div}|\-)? {postal_code}"""
+    return rf"""
+            (?:{_indexed_region1("a")}?(?:{part_div}{country})?{_postal_code}{_indexed_region1("b")}?
+            |{_indexed_region1("c")}(?![-,.\sA-Za-z]{{0,10}}{postal_code_re}))
+        """
+
+
+region1_postal_code = make_region1_postal_code()
+
+
 def make_full_address(
     *,
     full_street: str = full_street,
     part_div: str = part_div,
     city: str = city,
-    region1: str = region1,
+    region1_postal_code: str = region1_postal_code,
     country: str = country,
-    postal_code: str = postal_code,
     phone_number: str = phone_number,
 ) -> str:
+
     return r"""
                 (?P<full_address>
                     {full_street}
                     (?:{part_div} {phone_number})?
                     {part_div}{city}
-                    (?:
-                        {part_div} {region1} (?![A-Za-z])
-                        | 
-                        (?:{part_div}|\-)? {postal_code}
-                    ){{1,2}}
+                    {region1_postal_code}
                     (?:{part_div} {country})?
                 )
                 """.format(
         full_street=full_street,
         part_div=part_div,
         city=city,
-        region1=region1,
+        region1_postal_code=region1_postal_code,
         country=country,
-        postal_code=postal_code,
         phone_number=phone_number,
     )
 
 
 full_address = make_full_address()
```

### Comparing `pyap2-0.0.1/pyap/utils.py` & `pyap2-0.1.0/pyap/utils.py`

 * *Files identical despite different names*

### Comparing `pyap2-0.0.1/pyproject.toml` & `pyap2-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyap2"
-version = "0.0.1"
+version = "0.1.0"
 packages = [{ include = "pyap" }]
 description = "Pyap2 is a maintained fork of pyap, a regex-based library for parsing US, CA, and UK addresses. The fork adds typing support, handles more address formats and edge cases."
 authors = ["Argyle Developers <developers@argyle.io>"]
 documentation = "https://github.com/argyle-engineering/pyap"
 homepage = "https://github.com/argyle-engineering/pyap"
 repository = "https://github.com/argyle-engineering/pyap"
 license = "MIT"
```

### Comparing `pyap2-0.0.1/PKG-INFO` & `pyap2-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyap2
-Version: 0.0.1
+Version: 0.1.0
 Summary: Pyap2 is a maintained fork of pyap, a regex-based library for parsing US, CA, and UK addresses. The fork adds typing support, handles more address formats and edge cases.
 Home-page: https://github.com/argyle-engineering/pyap
 License: MIT
 Keywords: address,parser,regex
 Author: Argyle Developers
 Author-email: developers@argyle.io
 Requires-Python: >=3.9,<4.0
```

