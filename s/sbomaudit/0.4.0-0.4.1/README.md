# Comparing `tmp/sbomaudit-0.4.0-py2.py3-none-any.whl.zip` & `tmp/sbomaudit-0.4.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 16381 bytes, number of entries: 10
+Zip file size: 16669 bytes, number of entries: 10
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:08 sbomaudit/__init__.py
--rw-r--r--  2.0 unx    25165 b- defN 24-Feb-22 16:22 sbomaudit/audit.py
+-rw-r--r--  2.0 unx    26570 b- defN 24-Apr-25 19:06 sbomaudit/audit.py
 -rw-r--r--  2.0 unx     5125 b- defN 24-Feb-22 16:17 sbomaudit/cli.py
--rw-r--r--  2.0 unx      100 b- defN 24-Feb-22 15:00 sbomaudit/version.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18275 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      797 b- defN 24-Feb-22 16:37 sbomaudit-0.4.0.dist-info/RECORD
-10 files, 61064 bytes uncompressed, 15027 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx      100 b- defN 24-Apr-25 17:24 sbomaudit/version.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18839 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      797 b- defN 24-Apr-26 14:44 sbomaudit-0.4.1.dist-info/RECORD
+10 files, 63033 bytes uncompressed, 15315 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: sbomaudit/cli.py
 Comment: 
 
 Filename: sbomaudit/version.py
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/LICENSE
+Filename: sbomaudit-0.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/METADATA
+Filename: sbomaudit-0.4.1.dist-info/METADATA
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/WHEEL
+Filename: sbomaudit-0.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/entry_points.txt
+Filename: sbomaudit-0.4.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/top_level.txt
+Filename: sbomaudit-0.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: sbomaudit-0.4.0.dist-info/RECORD
+Filename: sbomaudit-0.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbomaudit/audit.py

```diff
@@ -25,71 +25,85 @@
         self.license_check = options.get("license_check", True)
         self.age = int(options.get("age", "0"))
         self.debug = options.get("debug", False)
         DAYS_IN_YEAR = 365
         self.maxage = int(options.get("maxage", "2")) * DAYS_IN_YEAR
         self.license_scanner = LicenseScanner()
         self.check_count = {"Fail": 0, "Pass": 0}
+        self.policy_check_count = {"Fail": 0, "Pass": 0}
         self.allow_list = {}
         self.deny_list = {}
         # Audit data in JSON
         self.audit = {}
         self.package_component = []
         self.file_component = []
         self.relationship_component = []
+        self.policy_component = []
         self.component = []
         self.element = {}
         self.console_out = output == ""
 
     def get_audit(self):
         return self.audit
 
-    def _component_message(self, message, state="Fail"):
+    def _component_message(self, message, state="Fail", policy=False):
         element = {"text": message, "state": state}
-        if len(self.component) > 0:
-            self.component.append(element)
+        if not policy:
+            if len(self.component) > 0:
+                self.component.append(element)
+            else:
+                self.component = [element]
         else:
-            self.component = [element]
+            if len(self.policy_component) > 0:
+                self.policy_component.append(element)
+            else:
+                self.policy_component = [element]
 
     def _send_to_console(self, text, colour):
         if self.console_out:
             print(Text.styled(text, colour))
 
-    def _show_text(self, text):
+    def _show_text(self, text, policy=False):
         self._send_to_console(f"[x] {text}", "green")
-        self._component_message(f"{text}", state="Pass")
+        self._component_message(f"{text}", state="Pass", policy=policy)
 
-    def _show_result(self, text, state, value=None, failure_text="MISSING"):
+    def _show_result(self, text, state, value=None, failure_text="MISSING", policy=False):
         if state:
             # Green
             if self.verbose:
-                self._show_text(text)
-            self.check_count["Pass"] = self.check_count["Pass"] + 1
+                self._show_text(text, policy=policy)
+            if not policy:
+                self.check_count["Pass"] = self.check_count["Pass"] + 1
+            else:
+                self.policy_check_count["Pass"] = self.policy_check_count["Pass"] + 1
         else:
             # Red
             if value is not None:
                 self._send_to_console(f"[ ] {text}: {value}", "red")
-                self._component_message(f"{text}: {value}")
+                self._component_message(f"{text}: {value}", policy=policy)
             elif len(failure_text) > 0:
                 self._send_to_console(f"[ ] {text}: {failure_text}", "red")
-                self._component_message(f"{text}: {failure_text}")
+                self._component_message(f"{text}: {failure_text}", policy=policy)
             else:
                 self._send_to_console(f"[ ] {text}", "red")
-                self._component_message(f"{text}")
-            self.check_count["Fail"] = self.check_count["Fail"] + 1
+                self._component_message(f"{text}", policy=policy)
+            if not policy:
+                self.check_count["Fail"] = self.check_count["Fail"] + 1
+            else:
+                self.policy_check_count["Fail"] = self.policy_check_count["Fail"] + 1
 
     def _heading(self, title):
         if self.console_out:
             print(Panel(title, style="bold", expand=False))
 
     def _check_value(self, text, values, data_item):
         self._show_result(text, data_item in values, data_item)
 
-    def _check(self, text, value, failure_text="MISSING"):
-        self._show_result(text, value, failure_text=failure_text)
+    def _check(self, text, value, failure_text="MISSING", policy=False):
+        self._show_result(text, value, failure_text=failure_text, policy=policy)
 
     def find_latest_version(self, name, version=None):
         """Returns the version and release date of the package available at PyPI."""
 
         url: str = f"https://pypi.org/pypi/{name}/json"
         pypi_version = None
         pypi_date = None
@@ -237,20 +251,22 @@
                                 not self.license_scanner.deprecated(license),
                             )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
+                                policy = True,
                             )
                         if deny_licenses is not None:
                             self._check(
                                 f"Denied License check for {name}",
                                 not (license in deny_licenses),
                                 failure_text=f"{license} not allowed",
+                                policy=True,
                             )
                         self._check(
                             f"Copyright defined - {name} : {copyright}",
                             not (copyright in [None, "NOASSERTION"]),
                             failure_text="",
                         )
                     else:
@@ -278,20 +294,22 @@
                                 not self.license_scanner.deprecated(license),
                             )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for {id}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
+                                policy = True,
                             )
                         if deny_licenses is not None:
                             self._check(
                                 f"Denied License check for {id}",
                                 not (license in deny_licenses),
                                 failure_text=f"{license} not allowed",
+                                policy=True,
                             )
                         self._check(
                             f"Copyright defined - {id} : {copyright}",
                             not (copyright in [None, "NOASSERTION"]),
                             failure_text="",
                         )
                 if len(self.component) > 0:
@@ -380,21 +398,23 @@
 
                     # Now summarise
                     if name is not None:
                         if allow_packages is not None:
                             self._check(
                                 f"Allowed Package check for package {name}",
                                 name in allow_packages,
-                                failure_text=f"{package} not allowed",
+                                failure_text=f"{name} not allowed",
+                                policy=True,
                             )
                         if deny_packages is not None:
                             self._check(
                                 f"Denied Package check for package {name}",
                                 not (name in deny_packages),
                                 failure_text=f"{name} not allowed",
+                                policy=True,
                             )
                         self._check(f"Supplier included for package {name}", supplier)
                         self._check(f"Version included for package {name}", version)
                         self._check(
                             f"License included for package {name}",
                             not (license in ["NOT KNOWN", "NOASSERTION"]),
                         )
@@ -416,20 +436,22 @@
                                 not self.license_scanner.deprecated(license),
                             )
                         if allow_licenses is not None:
                             self._check(
                                 f"Allowed License check for package {name}",
                                 license in allow_licenses,
                                 failure_text=f"{license} not allowed",
+                                policy=True,
                             )
                         if deny_licenses is not None:
                             self._check(
                                 f"Denied License check for package {name}",
                                 not (license in deny_licenses),
                                 failure_text=f"{license} not allowed",
+                                policy=True,
                             )
                         if latest_version is not None:
                             report = f"Version is {version}; latest is {latest_version}"
                             self._check(
                                 f"Using latest version of package {name}",
                                 latest_version == version,
                                 failure_text=report,
@@ -442,21 +464,23 @@
                             )
 
                             report = f"Age of release is {release_age.days} days"
                             self._check(
                                 f"Using mature version of package {name}",
                                 release_age.days > self.age,
                                 failure_text=report,
+                                policy=True,
                             )
                             # Check age of release if not using the latest version
                             if latest_version is not None and latest_version != version:
                                 self._check(
                                     f"Using old version of package {name}",
                                     release_age.days < self.maxage,
                                     failure_text=report,
+                                    policy=True,
                                 )
                         if self.cpe_check:
                             self._check(
                                 f"CPE name included for package {name}", cpe_used
                             )
                         if self.purl_check:
                             self._check(
@@ -496,14 +520,16 @@
                 if self.check_count["Fail"] == fail_count:
                     # No tests failed
                     self._show_text("Package Summary")
 
             self.audit["packages"] = self.package_component
             self.component = []
 
+        self.audit["policy"] = self.policy_component
+
         self._heading("Relationships Summary")
         fail_count = self.check_count["Fail"]
 
         self._check(
             "Dependency relationships provided for NTIA compliance", relationships_valid
         )
 
@@ -557,10 +583,12 @@
                 self._show_text("NTIA Summary")
 
         self._heading("SBOM Audit Summary")
         # Overide verbose setting to ensure always shown
         self.verbose = True
         self._show_text(f"Checks passed {self.check_count['Pass']}")
         self._show_text(f"Checks failed {self.check_count['Fail']}")
+        self._show_text(f"Policy checks passed {self.policy_check_count['Pass']}")
+        self._show_text(f"Policy checks failed {self.policy_check_count['Fail']}")
         self.audit["summary"] = self.component
 
         return valid_sbom
```

## sbomaudit/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2024 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.4.0"
+VERSION: str = "0.4.1"
```

## Comparing `sbomaudit-0.4.0.dist-info/LICENSE` & `sbomaudit-0.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sbomaudit-0.4.0.dist-info/METADATA` & `sbomaudit-0.4.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbomaudit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Audit SBOM contents
 Home-page: https://github.com/anthonyharrison/sbomaudit
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -122,14 +122,16 @@
 The files are text files consisting of two sections
 
 - List of SPDX license identifiers
 - Lst of Package names
 
 Each section is optional.
 
+These files can be used to enforce a development policy e.g. use the deny list to report on licences which are not approved.
+
 In this sample allow file, this would only allow cemponents with the MIT, Apache-2.0 or BSD-3-Clause licenses.
 It is also only expecting a single package 'click'.
 
 ```bash
 # This is an example ALLOW list file for SBOMAUDIT
 # Allowed licenses
 [license]
@@ -234,14 +236,20 @@
 
 ### NTIA Conformance
 
 The following checks are performed:
 
 - Check that the contents of the SBOM meet the minimum requirements for an SBOM as defined by the [NTIA](https://www.ntia.doc.gov/files/ntia/publications/sbom_minimum_elements_report.pdf).
 
+### Implementing a Development Policy
+
+The use of the `--age`, `--maxage`, `--allow` and `--deny` options can be used to enforce a development policy.
+
+A report of the checks which violate against the development policy is contained in a section within the output file.
+
 ## Example
 
 Given the following SBOM (click.json)
 
 ```
 {
   "$schema": "http://cyclonedx.org/schema/bom-1.4.schema.json",
@@ -466,50 +474,60 @@
           "state": "Pass"
         },
         {
           "text": "Non-deprecated license for click",
           "state": "Pass"
         },
         {
-          "text": "Using latest version of package click: Version is 8.0.3; latest is 8.1.6",
+          "text": "Using latest version of package click: Version is 8.0.3; latest is 8.1.7",
           "state": "Fail"
-        },
-        {
-          "text": "Using mature version of package click",
-          "state": "Pass"
-        },
-        {
-          "text": "Using old version of package click",
-          "state": "Pass"
         }
       ]
     }
   ],
+  "policy": [
+    {
+      "text": "Using mature version of package click",
+      "state": "Pass"
+    },
+    {
+      "text": "Using old version of package click: Age of release is 928 days",
+      "state": "Fail"
+    }
+  ],
   "relationships": [
     {
       "text": "Dependency relationships provided for NTIA compliance",
       "state": "Pass"
     },
     {
       "text": "Dependency relationship found for click",
       "state": "Pass"
     }
   ],
   "summary": [
     {
-      "text": "NTIA Summary",
+      "text": "NTIA conformant",
       "state": "Pass"
     },
     {
-      "text": "Checks passed 15",
+      "text": "Checks passed 13",
       "state": "Pass"
     },
     {
       "text": "Checks failed 1",
       "state": "Pass"
+    },
+    {
+      "text": "Policy checks passed 1",
+      "state": "Pass"
+    },
+    {
+      "text": "Policy checks failed 1",
+      "state": "Pass"
     }
   ]
 }
 ```
 
 ## Return Values
```

## Comparing `sbomaudit-0.4.0.dist-info/RECORD` & `sbomaudit-0.4.1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sbomaudit/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-sbomaudit/audit.py,sha256=Ivo98q1nGDfQRZp8Rwi8mLfpjfzYa7ph6CUkrfPjvWY,25165
+sbomaudit/audit.py,sha256=_72EffyPr2_rp3uUBSWxd7pqJdGJKLpCTKn-r3S3C84,26570
 sbomaudit/cli.py,sha256=S9Px_h4I9gRSV3TAgIm6ossPdRHd26ZuZBmBw6xL4E4,5125
-sbomaudit/version.py,sha256=_VPEo2Ij66iumFURgID5MFZwqjTi60cA-VjL4oQovi8,100
-sbomaudit-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sbomaudit-0.4.0.dist-info/METADATA,sha256=LGsy9SGWmq2mvwkXHJDg4stilK_Dm2HvUrqqEhmEn7s,18275
-sbomaudit-0.4.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-sbomaudit-0.4.0.dist-info/entry_points.txt,sha256=f8Rv8KaNsOGMapJwNvfQYJUoc8O8S2Ce49e3-Qa6n-I,49
-sbomaudit-0.4.0.dist-info/top_level.txt,sha256=8U0fCtvt4EJsO7B5XDwiiuBa7CsDVbcPJOJfWWJWcp0,10
-sbomaudit-0.4.0.dist-info/RECORD,,
+sbomaudit/version.py,sha256=r6uEkJGSmcL6vBCMWsxziiO6nVJ8oODA8Fkr1bMrbYc,100
+sbomaudit-0.4.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sbomaudit-0.4.1.dist-info/METADATA,sha256=IVjReOgm3JzoLjVsu2_RKgrLUlnfZM4kbU_tq7Xx22Q,18839
+sbomaudit-0.4.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+sbomaudit-0.4.1.dist-info/entry_points.txt,sha256=f8Rv8KaNsOGMapJwNvfQYJUoc8O8S2Ce49e3-Qa6n-I,49
+sbomaudit-0.4.1.dist-info/top_level.txt,sha256=8U0fCtvt4EJsO7B5XDwiiuBa7CsDVbcPJOJfWWJWcp0,10
+sbomaudit-0.4.1.dist-info/RECORD,,
```

