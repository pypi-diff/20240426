# Comparing `tmp/ratesb_python-0.2.4.tar.gz` & `tmp/ratesb_python-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratesb_python-0.2.4.tar", last modified: Thu Feb 22 00:22:33 2024, max compression
+gzip compressed data, was "ratesb_python-0.2.5.tar", last modified: Fri Apr 26 01:06:19 2024, max compression
```

## Comparing `ratesb_python-0.2.4.tar` & `ratesb_python-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,20 @@
-drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-02-22 00:22:33.649423 ratesb_python-0.2.4/
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     1069 2023-08-08 09:17:31.000000 ratesb_python-0.2.4/LICENSE
--rw-r--r--   0 fanlongxuan   (501) staff       (20)    11633 2024-02-22 00:22:33.649318 ratesb_python-0.2.4/PKG-INFO
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     9878 2024-02-22 00:21:58.000000 ratesb_python-0.2.4/README.md
--rw-r--r--   0 fanlongxuan   (501) staff       (20)      436 2024-02-22 00:22:23.000000 ratesb_python-0.2.4/pyproject.toml
-drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-02-22 00:22:33.646127 ratesb_python-0.2.4/ratesb_python/
--rw-r--r--   0 fanlongxuan   (501) staff       (20)       50 2023-12-11 17:20:13.000000 ratesb_python-0.2.4/ratesb_python/__init__.py
-drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-02-22 00:22:33.648084 ratesb_python-0.2.4/ratesb_python/common/
--rw-r--r--   0 fanlongxuan   (501) staff       (20)        0 2023-08-08 09:24:25.000000 ratesb_python-0.2.4/ratesb_python/common/__init__.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)    38505 2024-02-09 18:21:04.000000 ratesb_python-0.2.4/ratesb_python/common/analyzer.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)    15139 2024-02-09 08:33:40.000000 ratesb_python-0.2.4/ratesb_python/common/custom_classifier.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     5247 2023-11-13 09:08:13.000000 ratesb_python-0.2.4/ratesb_python/common/default_classifier.json
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     5566 2023-12-28 01:53:57.000000 ratesb_python-0.2.4/ratesb_python/common/messages.json
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     4023 2023-12-31 05:59:50.000000 ratesb_python-0.2.4/ratesb_python/common/results.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     4150 2024-02-09 08:14:40.000000 ratesb_python-0.2.4/ratesb_python/common/util.py
-drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-02-22 00:22:33.649048 ratesb_python-0.2.4/ratesb_python.egg-info/
--rw-r--r--   0 fanlongxuan   (501) staff       (20)    11633 2024-02-22 00:22:33.000000 ratesb_python-0.2.4/ratesb_python.egg-info/PKG-INFO
--rw-r--r--   0 fanlongxuan   (501) staff       (20)      608 2024-02-22 00:22:33.000000 ratesb_python-0.2.4/ratesb_python.egg-info/SOURCES.txt
--rw-r--r--   0 fanlongxuan   (501) staff       (20)        1 2024-02-22 00:22:33.000000 ratesb_python-0.2.4/ratesb_python.egg-info/dependency_links.txt
--rw-r--r--   0 fanlongxuan   (501) staff       (20)       43 2024-02-22 00:22:33.000000 ratesb_python-0.2.4/ratesb_python.egg-info/requires.txt
--rw-r--r--   0 fanlongxuan   (501) staff       (20)       20 2024-02-22 00:22:33.000000 ratesb_python-0.2.4/ratesb_python.egg-info/top_level.txt
--rw-r--r--   0 fanlongxuan   (501) staff       (20)      623 2024-02-22 00:22:33.649735 ratesb_python-0.2.4/setup.cfg
-drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-02-22 00:22:33.648851 ratesb_python-0.2.4/tests/
--rw-r--r--   0 fanlongxuan   (501) staff       (20)        0 2023-08-08 09:23:25.000000 ratesb_python-0.2.4/tests/__init__.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)    19370 2023-12-30 02:15:44.000000 ratesb_python-0.2.4/tests/test_analyzer.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     7956 2023-12-30 07:16:46.000000 ratesb_python-0.2.4/tests/test_classifier.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     3259 2023-12-30 07:00:33.000000 ratesb_python-0.2.4/tests/test_results.py
--rw-r--r--   0 fanlongxuan   (501) staff       (20)     4005 2023-12-30 06:57:11.000000 ratesb_python-0.2.4/tests/test_util.py
+drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-04-26 01:06:19.786467 ratesb_python-0.2.5/
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)     1069 2023-08-08 09:17:31.000000 ratesb_python-0.2.5/LICENSE
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)      739 2024-02-27 09:23:15.000000 ratesb_python-0.2.5/MANIFEST.in
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)    12136 2024-04-26 01:06:19.786343 ratesb_python-0.2.5/PKG-INFO
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)    10381 2024-04-26 00:57:37.000000 ratesb_python-0.2.5/README.md
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)      436 2024-04-26 01:05:52.000000 ratesb_python-0.2.5/pyproject.toml
+drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-04-26 01:06:19.784124 ratesb_python-0.2.5/ratesb_python/
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)      104 2024-04-17 21:15:03.000000 ratesb_python-0.2.5/ratesb_python/__init__.py
+drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-04-26 01:06:19.785786 ratesb_python-0.2.5/ratesb_python/common/
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)        0 2023-08-08 09:24:25.000000 ratesb_python-0.2.5/ratesb_python/common/__init__.py
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)    33575 2024-04-26 00:19:44.000000 ratesb_python-0.2.5/ratesb_python/common/analyzer.py
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)    15383 2024-04-26 00:55:04.000000 ratesb_python-0.2.5/ratesb_python/common/custom_classifier.py
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)     5247 2023-11-13 09:08:13.000000 ratesb_python-0.2.5/ratesb_python/common/default_classifier.json
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)     5566 2023-12-28 01:53:57.000000 ratesb_python-0.2.5/ratesb_python/common/messages.json
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)    12218 2024-04-17 21:06:16.000000 ratesb_python-0.2.5/ratesb_python/common/reaction_data.py
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)     4112 2024-04-16 20:15:02.000000 ratesb_python-0.2.5/ratesb_python/common/results.py
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)     5338 2024-04-26 00:32:54.000000 ratesb_python-0.2.5/ratesb_python/common/util.py
+drwxr-xr-x   0 fanlongxuan   (501) staff       (20)        0 2024-04-26 01:06:19.786000 ratesb_python-0.2.5/ratesb_python.egg-info/
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)      367 2024-04-26 01:06:19.000000 ratesb_python-0.2.5/ratesb_python.egg-info/SOURCES.txt
+-rw-r--r--   0 fanlongxuan   (501) staff       (20)      623 2024-04-26 01:06:19.786888 ratesb_python-0.2.5/setup.cfg
```

### Comparing `ratesb_python-0.2.4/LICENSE` & `ratesb_python-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ratesb_python-0.2.4/PKG-INFO` & `ratesb_python-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratesb_python
-Version: 0.2.4
+Version: 0.2.5
 Summary: rate law analysis for systems biology
 Home-page: https://github.com/sys-bio/ratesb_python
 Author: Longxuan Fan
 Author-email: Longxuan Fan <longxuan@usc.edu>
 License: MIT License
         
         Copyright (c) 2023 UW Sauro Lab
@@ -64,14 +64,20 @@
 # Analyze the model for rate law correctness
 analyzer.check_all()
 results = analyzer.results
 
 # Display all errors and warnings
 print(results)
 
+# Check selected errors and warnings
+analyzer.checks([1, 2, 1001, 1002])
+
+# No need to set results = analyzer.results again as results updates automatically
+print(results)
+
 # Display only warnings
 warnings = results.get_warnings()
 for reaction, messages in warnings.items():
     print(reaction, messages)
 
 # Retrieve messages for a specific reaction
 messages = results.get_messages_by_reaction("Reaction1")
@@ -181,14 +187,21 @@
         "optional_symbols": ["symbols that do not have to include in a rate law"],
         "power_limited_species": ["RateSB will pay attention to the power of these species (power matters in this case) symbols that have to be set to a certain power in a rate law (please specify power in the expression)"]
     }
     // Add more custom rate laws as needed
 ]
 ```
 
+## Testing
+
+For testing, run 
+```bash
+python -m unittest
+```
+
 ## Release Notes
 
 ### 0.1.0
 * initial release, used SBMLKinetics for rate law classifications
 
 ### 0.2.0
 * removed numpy dependency
@@ -211,14 +224,20 @@
 ### 0.2.3
 * include .json files
 * fixed path finding issue
 
 ### 0.2.4
 * updated instructions in readme
 
+### 0.2.5
+* Separated model reading from analysis
+* Tested on 1054 biomodels and fixed bugs
+* Added check_model method to allow user to use the package with one line
+* Solved when running sympy with sympy builtin symbols that raise error such as "S", a reaction like "S->P;k1*S" would work now
+
 ## Contributing
 
 Contributions to `ratesb_python` are welcomed! Whether it's bug reports, feature requests, or new code contributions, we value your feedback and contributions. Please submit a pull request or open an issue on our [GitHub repo](https://github.com/sys-bio/ratesb_python).
 
 ## Developing
 
 
@@ -227,18 +246,19 @@
 
 `ratesb_python` is licensed under the MIT license. Please see the LICENSE file for more information.
 
 ## Future Works
 
 * Implement stoichiometry checks for mass actions.
 * Perform checks after default classification to optimize performance.
+* Give user option to not use the default rate law classification to improve performance
 
 ## Known Issues
 
-There are some sympy builtin symbols that will raise error such as "S", so a reaction like "S->P; k1*S" would not work.
+N/A
 
 ## Contact
 
 For additional queries, please contact Longxuan Fan at longxuan@usc.edu.
 
 We hope ratesb_python assists you effectively in your model rate law analysis!
```

### Comparing `ratesb_python-0.2.4/README.md` & `ratesb_python-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 # Analyze the model for rate law correctness
 analyzer.check_all()
 results = analyzer.results
 
 # Display all errors and warnings
 print(results)
 
+# Check selected errors and warnings
+analyzer.checks([1, 2, 1001, 1002])
+
+# No need to set results = analyzer.results again as results updates automatically
+print(results)
+
 # Display only warnings
 warnings = results.get_warnings()
 for reaction, messages in warnings.items():
     print(reaction, messages)
 
 # Retrieve messages for a specific reaction
 messages = results.get_messages_by_reaction("Reaction1")
@@ -142,14 +148,21 @@
         "optional_symbols": ["symbols that do not have to include in a rate law"],
         "power_limited_species": ["RateSB will pay attention to the power of these species (power matters in this case) symbols that have to be set to a certain power in a rate law (please specify power in the expression)"]
     }
     // Add more custom rate laws as needed
 ]
 ```
 
+## Testing
+
+For testing, run 
+```bash
+python -m unittest
+```
+
 ## Release Notes
 
 ### 0.1.0
 * initial release, used SBMLKinetics for rate law classifications
 
 ### 0.2.0
 * removed numpy dependency
@@ -172,14 +185,20 @@
 ### 0.2.3
 * include .json files
 * fixed path finding issue
 
 ### 0.2.4
 * updated instructions in readme
 
+### 0.2.5
+* Separated model reading from analysis
+* Tested on 1054 biomodels and fixed bugs
+* Added check_model method to allow user to use the package with one line
+* Solved when running sympy with sympy builtin symbols that raise error such as "S", a reaction like "S->P;k1*S" would work now
+
 ## Contributing
 
 Contributions to `ratesb_python` are welcomed! Whether it's bug reports, feature requests, or new code contributions, we value your feedback and contributions. Please submit a pull request or open an issue on our [GitHub repo](https://github.com/sys-bio/ratesb_python).
 
 ## Developing
 
 
@@ -188,18 +207,19 @@
 
 `ratesb_python` is licensed under the MIT license. Please see the LICENSE file for more information.
 
 ## Future Works
 
 * Implement stoichiometry checks for mass actions.
 * Perform checks after default classification to optimize performance.
+* Give user option to not use the default rate law classification to improve performance
 
 ## Known Issues
 
-There are some sympy builtin symbols that will raise error such as "S", so a reaction like "S->P; k1*S" would not work.
+N/A
 
 ## Contact
 
 For additional queries, please contact Longxuan Fan at longxuan@usc.edu.
 
 We hope ratesb_python assists you effectively in your model rate law analysis!
```

### Comparing `ratesb_python-0.2.4/ratesb_python/common/custom_classifier.py` & `ratesb_python-0.2.5/ratesb_python/common/custom_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 sys.path.append(current_dir)
 sys.path.append(parent_dir)
 
 from common import util
 import re
 import sympy
 
+# timeout if rate law is too complex
+TIMEOUT = 10000
+
 class _CustomClassifier:
     """Custom Classifier for rate laws.
 
     This classifier validates, classifies and operates helper methods on rate laws.
     
     Attributes:
         rate_law_classifications_path (str): The path to the rate law classifications.
@@ -204,25 +207,30 @@
         for item in self.custom_classifications:
             if any_true and is_default:
                 ret[item['name']] = False
                 continue
             kinetics_expression = item['expression'].replace("^", "**")
             optional_symbols = item['optional_symbols']
             all_expr = self.get_all_expr(kinetics_expression, optional_symbols)
+            all_expr = [sympy.sympify(expr) for expr in all_expr]
             power_limited_species = item['power_limited_species']
             classified_true = False
-            for replaced_kinetics in replaced_kinetics_list:
-                replaced_kinetics_sympify = self.lower_powers(sympy.sympify(replaced_kinetics), power_limited_species)
-                replaced_kinetics_sympify = self.remove_constant_multiplier(replaced_kinetics_sympify)
-                comparison_result = any(util.check_equal(sympy.simplify(expr), replaced_kinetics_sympify) for expr in all_expr)
-                if comparison_result:
-                    ret[item['name']] = True
-                    classified_true = True
-                    any_true = True
-                    break
+            try:
+                for replaced_kinetics in replaced_kinetics_list:
+                    replaced_kinetics_sympify = self.lower_powers(sympy.sympify(replaced_kinetics), power_limited_species)
+                    replaced_kinetics_sympify = self.remove_constant_multiplier(replaced_kinetics_sympify)
+                    comparison_result = any(util.check_equal(expr, replaced_kinetics_sympify) for expr in all_expr)
+                    if comparison_result:
+                        ret[item['name']] = True
+                        classified_true = True
+                        any_true = True
+                        break
+            except:
+                ret[item['name']] = False
+                continue
             if not classified_true:
                 ret[item['name']] = False
         return ret
 
     def lower_powers(self, expr, keep=[]):
         """Lowers the power of certain elements in the expression.
```

### Comparing `ratesb_python-0.2.4/ratesb_python/common/default_classifier.json` & `ratesb_python-0.2.5/ratesb_python/common/default_classifier.json`

 * *Files identical despite different names*

### Comparing `ratesb_python-0.2.4/ratesb_python/common/messages.json` & `ratesb_python-0.2.5/ratesb_python/common/messages.json`

 * *Files identical despite different names*

### Comparing `ratesb_python-0.2.4/ratesb_python/common/results.py` & `ratesb_python-0.2.5/ratesb_python/common/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,16 @@
     def __repr__(self):
         """
         Overrides the __repr__ method.
 
         Returns:
             str: A string representation of the results.
         """
+        if self.count_messages() == 0:
+            return 'No errors or warnings found.'
         str_repr = ''
         for reaction_name, messages in self.results.items():
             str_repr += f'{reaction_name}:\n'
             for message in messages:
                 is_warning = message['is_warning']
                 code = message['code']
                 message_body = message['message']
```

### Comparing `ratesb_python-0.2.4/setup.cfg` & `ratesb_python-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ratesb_python
-version = 0.2.4
+version = 0.2.5
 author = Longxuan Fan
 author_email = longxuan@usc.edu
 description = package for analyzing the rate laws in an SBML or Antimony model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sys-bio/ratesb_python
 license = MIT
```

