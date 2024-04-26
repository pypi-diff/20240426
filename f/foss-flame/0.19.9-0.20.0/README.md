# Comparing `tmp/foss-flame-0.19.9.tar.gz` & `tmp/foss-flame-0.20.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foss-flame-0.19.9.tar", last modified: Fri Feb  2 15:20:07 2024, max compression
+gzip compressed data, was "foss-flame-0.20.0.tar", last modified: Fri Apr 26 08:03:01 2024, max compression
```

## Comparing `foss-flame-0.19.9.tar` & `foss-flame-0.20.0.tar`

### file list

```diff
@@ -1,233 +1,281 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/BSD-2-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-02-02 15:19:54.000000 foss-flame-0.19.9/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-02 15:19:54.000000 foss-flame-0.19.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-02 15:20:07.302974 foss-flame-0.19.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-02-02 15:19:54.000000 foss-flame-0.19.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/flame/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8700 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-02 15:20:07.000000 foss-flame-0.19.9/flame/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    24541 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/license_db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.270974 foss-flame-0.19.9/flame/var/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/ambiguities.json
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/compounds.json
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/duals.json
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/license_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/flame/var/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/0BSD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/0BSD.json
--rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Apache-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.json
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.json
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BSL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Beerware.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Beerware.json
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.json
--rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC0-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CC0-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/FTL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/FTL.json
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.json
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    35269 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/HPND.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/HPND.json
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ICU.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ICU.json
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/IJG.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/IJG.json
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ISC.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ISC.json
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/JSON.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/JSON.json
--rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    26075 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.json
--rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.json
--rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.json
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Latex2e.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Latex2e.json
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Libpng.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Libpng.json
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.json
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-iso-8879.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-iso-8879.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-public-domain.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-public-domain.json
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-advertising.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-advertising.json
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-open-group.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT-open-group.json
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MIT.json
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MITNFA.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MITNFA.json
--rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    23255 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0-no-copyleft-exception.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0-no-copyleft-exception.json
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/MPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NCSA.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NCSA.json
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NTP.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/NTP.json
--rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OFL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OML.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OML.json
--rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OpenSSL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/OpenSSL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Plexus.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Plexus.json
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/PostgreSQL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/PostgreSQL.json
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Python-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/RSA-MD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/RSA-MD.json
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SAX-PD.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SAX-PD.json
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SWL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/SWL.json
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Sendmail.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Sendmail.json
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TCL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TCL.json
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Unlicense.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Unlicense.json
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Vim.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Vim.json
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/W3C.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/W3C.json
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/WTFPL.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/WTFPL.json
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.json
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/X11.json
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Zlib.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/Zlib.json
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/blessing.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/blessing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.json
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/curl.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/curl.json
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libpng-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libpng-2.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libtiff.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/libtiff.json
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-02 15:19:54.000000 foss-flame-0.19.9/flame/var/operators.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 15:20:07.302974 foss-flame-0.19.9/foss_flame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-02 15:20:07.000000 foss-flame-0.19.9/foss_flame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-02 15:19:54.000000 foss-flame-0.19.9/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-02 15:19:54.000000 foss-flame-0.19.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-02 15:20:07.302974 foss-flame-0.19.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-02 15:19:54.000000 foss-flame-0.19.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.635876 foss-flame-0.20.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.595876 foss-flame-0.20.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-26 08:02:50.000000 foss-flame-0.20.0/LICENSES/BSD-2-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17023 2024-04-26 08:02:50.000000 foss-flame-0.20.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34674 2024-04-26 08:02:50.000000 foss-flame-0.20.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-26 08:02:50.000000 foss-flame-0.20.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-26 08:03:01.635876 foss-flame-0.20.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-04-26 08:02:50.000000 foss-flame-0.20.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.599876 foss-flame-0.20.0/flame/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10513 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-26 08:03:01.000000 foss-flame-0.20.0/flame/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15310 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26274 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/license_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.599876 foss-flame-0.20.0/flame/var/
+-rw-r--r--   0 runner    (1001) docker     (127)     4982 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/ambiguities.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/compounds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/duals.json
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/license_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.635876 foss-flame-0.20.0/flame/var/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/0BSD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/0BSD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-1.2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10250 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AFL-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34639 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35156 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Apache-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Artistic-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Artistic-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Artistic-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Artistic-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Autoconf-exception-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Autoconf-exception-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Autoconf-exception-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Autoconf-exception-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-1-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-1-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause-Patent.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause-Patent.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-3-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-3-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause-UC.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause-UC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-Source-Code.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSD-Source-Code.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BSL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Beerware.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Beerware.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Bitstream-Vera.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Bitstream-Vera.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BlueOak-1.0.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/BlueOak-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14075 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-2.5.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-2.5.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22239 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-3.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-3.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20131 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-4.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-4.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-PDDC.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC-PDDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC0-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CC0-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16768 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CDDL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CDDL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17212 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CDDL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CDDL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11757 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/CPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Classpath-exception-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Classpath-exception-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ECL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ECL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11248 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12931 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13133 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12796 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.2.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/EUPL-1.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFAP.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFAP.json
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFUL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFUL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFULLR.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFULLR.json
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFULLRWD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FSFULLRWD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FTL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/FTL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GCC-exception-3.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GCC-exception-3.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-1.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-1.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13277 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-1.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-1.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-2.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-2.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-2.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-2.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35269 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35762 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/GPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/HPND.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/HPND.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ICU.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ICU.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/IJG-short.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/IJG-short.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/IJG.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/IJG.json
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ISC.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ISC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/JSON.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/JSON.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25372 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26075 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26613 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-only.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-only.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8356 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-or-later.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-or-later.json
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LLVM-exception.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LLVM-exception.json
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Latex2e.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Latex2e.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Libpng.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Libpng.json
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-boost-original.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-boost-original.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-docbook.json
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-g10-permissive.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-g10-permissive.json
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-iso-8879.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-iso-8879.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-public-domain.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-public-domain.json
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-zpl-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Linux-syscall-note.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Linux-syscall-note.json
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-advertising.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-advertising.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-open-group.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT-open-group.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MIT.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MITNFA.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MITNFA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17912 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23255 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-2.0-no-copyleft-exception.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-2.0-no-copyleft-exception.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/MPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/NCSA.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/NCSA.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/NTP.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/NTP.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19775 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ODC-By-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ODC-By-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OFL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OFL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OFL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OFL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OML.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OML.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5751 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OpenSSL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/OpenSSL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Plexus.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Plexus.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/PostgreSQL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/PostgreSQL.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Python-2.0.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Python-2.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Python-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Python-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/RSA-MD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/RSA-MD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SAX-PD.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SAX-PD.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SGI-B-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SGI-B-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SSPL-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SSPL-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SWL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/SWL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Sendmail.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Sendmail.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Sleepycat.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Sleepycat.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TCL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TCL.json
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TU-Berlin-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TU-Berlin-1.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TU-Berlin-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/TU-Berlin-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Unlicense.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Unlicense.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Vim.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Vim.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/W3C.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/W3C.json
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/WTFPL.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/WTFPL.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/X11-distribute-modifications-variant.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/X11-distribute-modifications-variant.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/X11.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/X11.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-1.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-1.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-2.1.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/ZPL-2.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Zlib.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/Zlib.json
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/blessing.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/blessing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/bzip2-1.0.6.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/bzip2-1.0.6.json
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/curl.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/curl.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/libpng-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/libpng-2.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/libtiff.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/libtiff.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/x11-keith-packard.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/licenses/x11-keith-packard.json
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-26 08:02:50.000000 foss-flame-0.20.0/flame/var/operators.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 08:03:01.635876 foss-flame-0.20.0/foss_flame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-26 08:03:01.000000 foss-flame-0.20.0/foss_flame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-26 08:02:50.000000 foss-flame-0.20.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-26 08:02:50.000000 foss-flame-0.20.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-26 08:03:01.639876 foss-flame-0.20.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-26 08:02:50.000000 foss-flame-0.20.0/setup.py
```

### Comparing `foss-flame-0.19.9/LICENSES/BSD-2-Clause.txt` & `foss-flame-0.20.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/LICENSES/CC-BY-4.0.txt` & `foss-flame-0.20.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/LICENSES/GPL-3.0-or-later.txt` & `foss-flame-0.20.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/PKG-INFO` & `foss-flame-0.20.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: foss-flame
-Version: 0.19.9
+Version: 0.20.0
 Summary: FOSS License Additional Metadata
-Home-page: https://github.com/hesa/license-db
+Home-page: https://github.com/hesa/foss-licenses
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -54,19 +54,19 @@
 
 # Background
 
 There are lots of software licenses out there (e.g. see [ScanCode LicenseDB](https://scancode-licensedb.aboutcode.org/)), some of them are FOSS and some not. In this project we primarily focus on FOSS licenses.
 
 ## License name proliferation
 
-When you're working with compliance you are used to liceses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information machine readable.
+When you're working with compliance you are used to licenses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information to be machine readable.
 
 ## License proliferation
 
-Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported in for example the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and not, but we need to make it possible for a machine to assist us. 
+Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported for example in the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and which are not, but we need to make it possible for a machine to assist us. 
 
 # About
 
 This projet aims at providing a database with:
 
 * "all" different names for a license in a database
```

### Comparing `foss-flame-0.19.9/README.md` & `foss-flame-0.20.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 # Background
 
 There are lots of software licenses out there (e.g. see [ScanCode LicenseDB](https://scancode-licensedb.aboutcode.org/)), some of them are FOSS and some not. In this project we primarily focus on FOSS licenses.
 
 ## License name proliferation
 
-When you're working with compliance you are used to liceses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information machine readable.
+When you're working with compliance you are used to licenses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information to be machine readable.
 
 ## License proliferation
 
-Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported in for example the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and not, but we need to make it possible for a machine to assist us. 
+Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported for example in the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and which are not, but we need to make it possible for a machine to assist us. 
 
 # About
 
 This projet aims at providing a database with:
 
 * "all" different names for a license in a database
```

### Comparing `foss-flame-0.19.9/flame/__main__.py` & `foss-flame-0.20.0/flame/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from argparse import RawTextHelpFormatter
 import argparse
 import logging
 import sys
 import traceback
+import re
 
 from flame.license_db import FossLicenses
 from flame.license_db import Validation
 import flame.config
 from flame.format import OUTPUT_FORMATS
 from flame.format import OutputFormatterFactory
 from flame.exception import FlameException
@@ -39,14 +40,20 @@
 
     parser.add_argument('-ald', '--additional-license-dir',
                         type=str,
                         dest='additional_license_dir',
                         help='Add licenses as found in the supplied directory',
                         default=None)
 
+    parser.add_argument('-lmf', '--license-matrix-file',
+                        type=str,
+                        dest='license_matrix_file',
+                        help='Supply license matrix to override OSADL\'s license compatibility matrix',
+                        default=None)
+
     parser.add_argument('-ndu', '--no-dual-update',
                         action='store_true',
                         help='do not update dual licenses (e.g. GPL-2.0-or-later -> GPL-2.0-only OR GPL-3.0-only)',
                         default=False)
 
     parser.add_argument('-of', '--output-format',
                         type=str,
@@ -58,27 +65,31 @@
                         help='output verbose information',
                         default=False)
 
     parser.add_argument('-V', '--version',
                         action='store_true',
                         help='output version information',
                         default=False)
-    parser.set_defaults(which='version', func=version_info)
+
+    parser.set_defaults(which='help', func=version_info)
 
     parser.add_argument('-d', '--debug',
                         action='store_true',
                         help='output debug information to stderr',
                         default=False)
 
     parser.add_argument('-c', '--check',
                         action='store_true',
                         help='check all license files against JSON schema when initializing. Mainly for the flame developers.',
                         default=False)
 
     subparsers = parser.add_subparsers(help='Sub commands')
+    parser.add_argument('--validate-spdx', action='store_true', dest='validate_spdx', help='Validate that the resulting license expression is valid according to SPDX syntax', default=False)
+    parser.add_argument('--validate-relaxed', action='store_true', dest='validate_relaxed', help='Validate that the resulting license expression is valid according to SPDX syntax, but allow non SPDX identifiers ', default=False)
+    parser.add_argument('--validate-osadl', action='store_true', dest='validate_osadl', help='Validate that the resulting licenses are supported by OSADL\'s compatibility matrix.', default=False)
 
     # license
     parser_e = subparsers.add_parser(
         'license', help='Convert license to SPDX identifiers and syntax')
     parser_e.set_defaults(which='license', func=show_license)
     parser_e.add_argument('license', type=str, nargs='+', help='license expression to fix')
 
@@ -89,81 +100,107 @@
     parser_e.add_argument('license', type=str, help='license to display fully. Only single license is allowed')
 
     # compatibility
     parser_c = subparsers.add_parser(
         'compat', help='Convert license to using licenses existing in the OSADL\'s matrix')
     parser_c.set_defaults(which='compat', func=compatibility)
     parser_c.add_argument('license', type=str, nargs='+', help='license name to display')
-    parser_c.add_argument('--validate-spdx', action='store_true', dest='validate_spdx', help='Validate that the resulting license expression is valid according to SPDX syntax', default=False)
-    parser_c.add_argument('--validate-relaxed', action='store_true', dest='validate_relaxed', help='Validate that the resulting license expression is valid according to SPDX syntax, but allow non SPDX identifiers ', default=False)
-    parser_c.add_argument('--validate-osadl', action='store_true', dest='validate_osadl', help='Validate that the resulting licenses are supported by OSADL\'s compatibility matrix', default=False)
 
     # simplify
     parser_s = subparsers.add_parser(
         'simplify', help='Simplify a license (SPDX syntax) expression, e.g. "MIT AND MIT" -> "MIT"')
     parser_s.set_defaults(which='simplify', func=simplify)
     parser_s.add_argument('license_expression', type=str, nargs='+', help='license expression to simplify')
 
     # aliases
     parser_a = subparsers.add_parser(
         'aliases', help='Display all aliases')
     parser_a.set_defaults(which='aliases', func=aliases)
-    parser_a.add_argument('--license', '-l', type=str, dest='alias_license', help='List only the aliases for licenses containing the given string', default=None)
+    parser_a.add_argument('--include-license', '-il', type=str, dest='include_license', help='List only the aliases for licenses containing the given string (case insensitive)', default=None)
+
+    # ambiguities
+    parser_os = subparsers.add_parser(
+        'ambiguities', help='Display all ambiguities')
+    parser_os.set_defaults(which='ambiguities', func=ambiguities)
 
     # compatbilities
     parser_cs = subparsers.add_parser(
         'compats', help='Display all compatibilities')
     parser_cs.set_defaults(which='compats', func=compats)
 
+    # licenses
+    parser_cs = subparsers.add_parser(
+        'licenses', help='show all licenses')
+    parser_cs.set_defaults(which='licenses', func=licenses)
+
     # operators
     parser_os = subparsers.add_parser(
         'operators', help='Display all operators')
     parser_os.set_defaults(which='operators', func=operators)
 
-    # licenses
-    parser_cs = subparsers.add_parser(
-        'licenses', help='show all licenses')
-    parser_cs.set_defaults(which='licenses', func=licenses)
+    # unknown
+    parser_u = subparsers.add_parser(
+        'unknown', help='Show the unknown licenses for a license expression. Intended for foss-licenses developers.')
+    parser_u.set_defaults(which='unknown', func=unknown)
+    parser_u.add_argument('license', type=str, nargs='+', help='license expression to fix')
 
     return parser
 
 def parse():
 
     return get_parser().parse_args()
 
+def ambiguities(fl, formatter, args):
+    all_ambiguities = fl.ambiguities_list()
+    return formatter.format_ambiguities(all_ambiguities)
+
 def operators(fl, formatter, args):
     all_op = fl.operators()
     return formatter.format_operators(all_op, args.verbose)
 
 def aliases(fl, formatter, args):
-    all_aliases = fl.alias_list(args.alias_license)
+    all_aliases = fl.alias_list(args.include_license)
     return formatter.format_alias_list(all_aliases, args.verbose)
 
 def licenses(fl, formatter, args):
     all_licenses = fl.licenses()
     return formatter.format_licenses(all_licenses, args.verbose)
 
+def unknown(fl, formatter, args):
+    validations = __validations(args)
+    compat_license_expression = fl.expression_license(' '.join(args.license), validations=validations, update_dual=(not args.no_dual_update))
+    compat_licenses = [x.strip() for x in re.split('\(|OR|AND|\)', compat_license_expression['identified_license'])]
+    compat_licenses = [x for x in compat_licenses if x]
+    unknown_symbols = set()
+    for compat_license in compat_licenses:
+        if compat_license not in fl.known_symbols():
+            unknown_symbols.add(compat_license)
+    if len(unknown_symbols) != 0:
+        raise FlameException('Unknown symbols identified.\n' + '\n'.join(list(unknown_symbols)))
+    return 'OK', None
+
 def simplify(fl, formatter, args):
     simplified = fl.simplify(args.license_expression)
     return str(simplified) # formatter.format_licenses(all_licenses, args.verbose)
 
 def compats(fl, formatter, args):
     all_compats = fl.compatibility_as_list()
     return formatter.format_compat_list(all_compats, args.verbose)
 
 def version_info(fl, formatter, args):
-    return flame.config.SW_VERSION
+    return flame.config.SW_VERSION, None
 
 def compatibility(fl, formatter, args):
     validations = __validations(args)
     compatibilities = fl.expression_compatibility_as(' '.join(args.license), validations)
     return formatter.format_compatibilities(compatibilities, args.verbose)
 
 def show_license(fl, formatter, args):
-    expression = fl.expression_license(' '.join(args.license), update_dual=(not args.no_dual_update))
+    validations = __validations(args)
+    expression = fl.expression_license(' '.join(args.license), validations=validations, update_dual=(not args.no_dual_update))
     return formatter.format_expression(expression, args.verbose)
 
 def full_license(fl, formatter, args):
     expr_split = fl.expression_license(args.license)['identified_license'].split()
 
     if len(expr_split) == 1:
         lic = fl.license_complete(expr_split[0])
@@ -193,14 +230,15 @@
 
     config = {}
     config['flame-config'] = args.flame_config
     config['check'] = args.check
     config['additional-license-dir'] = args.additional_license_dir
     config['license-dir'] = args.license_dir
     config['flame-config'] = args.flame_config
+    config['license-matrix-file'] = args.license_matrix_file
 
     try:
         fl = FossLicenses(config=config)
     except Exception as e:
         if args.verbose:
             print(traceback.format_exc())
             print(str(e))
@@ -215,14 +253,14 @@
             if warnings:
                 print(warnings, file=sys.stderr)
             print(formatted)
         except Exception as e:
             if args.verbose:
                 print(traceback.format_exc())
 
-            formatted = formatter.format_error(e, args.verbose)
+            formatted, warnings = formatter.format_error(e, args.verbose)
             print(formatted)
             sys.exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `foss-flame-0.19.9/flame/config.py` & `foss-flame-0.20.0/flame/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import json
 import logging
 import os
 import flame.exception
 
-SW_VERSION = '0.19.9'
+SW_VERSION = '0.20.0'
 
 PYTHON_DIR = os.path.dirname(os.path.realpath(__file__))
 VAR_DIR = os.path.join(PYTHON_DIR, 'var')
 LICENSE_DIR = os.path.join(VAR_DIR, 'licenses')
 
 LICENSE_SCHEMA_FILE = os.path.join(VAR_DIR, 'license_schema.json')
 LICENSE_OPERATORS_FILE = os.path.join(VAR_DIR, 'operators.json')
```

### Comparing `foss-flame-0.19.9/flame/format.py` & `foss-flame-0.20.0/flame/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         """
         Return a formatted string of the provided compatibilities.
 
         :param : A list of aliases as returned from FossLicenses.alias_list()
         :type all_aliases: list
         :param verbose: provide additional information
         :type verbose: boolean
-        :raise FlameException: if all_compats is not valid
+        :raise FlameException: if compats is not valid
         :return: formatted string
         :rtype: str
 
         :Example:
 
         >>> from flame.license_db import FossLicenses
         >>> fl = FossLicenses()
@@ -233,29 +233,52 @@
         """
         Return a formatted string of the provided operators
 
         :param operators: A list of operators.
         :type operators: list
         :param verbose: provide additional information
         :type verbose: boolean
-        :raise FlameException: if all_compats is not valid
+        :raise FlameException: if operators is not valid
         :return: formatted string
         :rtype: str
 
         :Example:
 
         >>> from flame.license_db import FossLicenses
         >>> fl = FossLicenses()
         >>> operators = fl.operators()
         >>> formatter = OutputFormatterFactory.formatter("TEXT")
         >>> formatted = formatter.format_operators(operators)
 
         """
         return None, None
 
+    def format_ambiguities(self, ambiguities, verbose=False):
+        """
+        Return a formatted string of the existing ambiguities
+
+        :param operators: A list of ambiguites.
+        :type operators: list
+        :param verbose: provide additional information
+        :type verbose: boolean
+        :raise FlameException: if ambiguites is not valid
+        :return: formatted string
+        :rtype: str
+
+        :Example:
+
+        >>> from flame.license_db import FossLicenses
+        >>> fl = FossLicenses()
+        >>> ambiguities = fl.ambiguities_list()
+        >>> formatter = OutputFormatterFactory.formatter("TEXT")
+        >>> formatted = formatter.format_ambiguities(ambiguities)
+
+        """
+        return None, None
+
 class JsonOutputFormatter(OutputFormatter):
 
     def format_compat(self, compat, verbose=False):
         return json.dumps(compat, indent=4), None
 
     def format_compat_list(self, all_compats, verbose=False):
         return json.dumps(all_compats, indent=4), None
@@ -263,28 +286,35 @@
     def format_expression(self, expression, verbose=False):
         return json.dumps(expression, indent=4), None
 
     def format_alias_list(self, all_aliases, verbose=False):
         return json.dumps(all_aliases, indent=4), None
 
     def format_error(self, error, verbose=False):
-        return json.dumps({'error': f'{error}'}, indent=4), None
+        new_error = {
+            'message': str(error),
+            'problems': error.problems(),
+        }
+        return json.dumps(new_error, indent=4), None
 
     def format_licenses(self, licenses, verbose=False):
         return json.dumps(licenses, indent=4), None
 
     def format_license_complete(self, _license, verbose=False):
         return json.dumps(_license, indent=4), None
 
     def format_compatibilities(self, compats, verbose=False):
         return json.dumps(compats), None
 
     def format_operators(self, operators, verbose=False):
         return json.dumps(operators), None
 
+    def format_ambiguities(self, ambiguities, verbose=False):
+        return json.dumps(ambiguities), None
+
 class YamlOutputFormatter(OutputFormatter):
 
     def format_compat(self, compat, verbose=False):
         return yaml.safe_dump(compat), None
 
     def format_compat_list(self, all_compats, verbose=False):
         return None, None
@@ -306,14 +336,17 @@
 
     def format_compatibilities(self, compats, verbose=False):
         return yaml.safe_dump(compats), None
 
     def format_operators(self, operators, verbose=False):
         return yaml.safe_dump(operators), None
 
+    def format_ambiguities(self, ambiguities, verbose=False):
+        return yaml.safe_dump(ambiguities), None
+
 class TextOutputFormatter(OutputFormatter):
 
     def format_compat(self, compat, verbose=False):
         ret = []
         id_lic = compat['identified_license']
         if verbose:
             ret.append(f'queried_name: {id_lic["queried_name"]}')
@@ -369,14 +402,20 @@
     def format_licenses(self, licenses, verbose=False):
         licenses.sort()
         return '\n'.join(licenses), None
 
     def format_operators(self, operators, verbose=False):
         return '\n'.join([f'{k} -> {v}' for k, v in operators.items()]), None
 
+    def format_ambiguities(self, ambiguities, verbose=False):
+        ret = []
+        for k, v in ambiguities.items():
+            ret += [f'{a} -> {k}' for a in v['aliases']]
+        return '\n'.join(ret), None
+
     def format_error(self, error, verbose=False):
         return f'Error: {error}', None
 
     def format_license_complete(self, lic, verbose=False):
         ret_str = []
         ret_str.append(f'{lic["name"]}')
         ret_str.append(f'    spdxid:           {lic["spdxid"]}')
```

### Comparing `foss-flame-0.19.9/flame/license_db.py` & `foss-flame-0.20.0/flame/license_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # SPDX-FileCopyrightText: 2023 Henrik Sandklef
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
+import boolean
 import collections
 import glob
 import json
 import logging
 import re
 from pathlib import Path
 import license_expression
@@ -76,14 +77,15 @@
 
         check = config.get('check', False)
         logging_level = self.__str_to_loggin_info(config)
         logging.basicConfig(level=logging_level)
 
         self.config = config
         self.license_dir = config.get('license-dir', LICENSE_DIR)
+        self.license_matrix_file = config.get('license-matrix-file', None)
         self.additional_license_dir = config.get('additional-license-dir', [])
         self.__init_license_db(check)
         self.supported_licenses = None
         self.compat_cache = {}
         self.license_cache = {}
 
     def __str_to_loggin_info(self, config):
@@ -183,14 +185,17 @@
             licenses[compound['spdxid']] = compound
             for alias in compound[FLAME_ALIASES_TAG]:
                 if alias in aliases:
                     raise FlameException(f'Alias "{alias}" -> {compound["spdxid"]} already defined as "{aliases[alias]}".')
 
                 aliases[alias] = compound['spdxid']
 
+            if COMPATIBILITY_AS_TAG in compound:
+                compats[compound['spdxid']] = compound[COMPATIBILITY_AS_TAG]
+
         # Dual licenses
         # Read license with built-in dual feature, e.g
         # "GPL-2.0-or-later" which can be seen as a dual
         # license "GPL-2.0-only OR GPL-3.0-only"
         duals_file = self.config.get('duals_file', LICENSE_DUALS_FILE)
         data = self.__read_json(duals_file)
         for dual in data[DUAL_LICENSES_TAG]:
@@ -282,15 +287,15 @@
         ret = ' '.join(new_expr)
         return {
             'input_license_expression': license_expression,
             'license_expression': ret,
             'updates': updates,
         }
 
-    def expression_license(self, license_expression, update_dual=True):
+    def expression_license(self, license_expression, validations=None, update_dual=True):
         """
         Return an object with information about the normalized license for the license given.
 
         :param license_expression: A license expression. E.g "BSD3" or "GPLv2+ || BSD3"
         :type license_expression: str
         :raise FlameException: if license_expression is not valid
         :return: a normalized license expression
@@ -304,14 +309,17 @@
         BSD-3-Clause AND LicenseRef-flame-x11-keith-packard
 
         """
 
         if not isinstance(license_expression, str):
             raise FlameException('Wrong type (type(license_expresssion)) of input to the function expression_license. Only string is allowed.')
 
+        # remove multiple blanks
+        license_expression = re.sub(' [ ]*', ' ', license_expression)
+
         cache_key = f'{license_expression}__{update_dual}'
         if cache_key in self.license_cache:
             return self.license_cache.get(cache_key)
 
         replacements = []
 
         ret = self.__update_license_expression_helper(self.license_db[FLAME_ALIASES_TAG],
@@ -329,15 +337,18 @@
                                                       ret['license_expression'],
                                                       allow_letter=True)
         replacements += ret['identifications']
 
         # Manage dual licenses (such as GPL-2.0-or-later)
         updates_object = self.__update_or_later(ret['license_expression'])
         updates = updates_object['updates']
-        updated_license = str(self.license_expression.parse(updates_object['license_expression']))
+        try:
+            updated_license = str(self.license_expression.parse(updates_object['license_expression']))
+        except boolean.boolean.ParseError as e:
+            raise FlameException(f'Could not parse \"{updates_object["license_expression"]}\". Exception: {e}')
 
         if update_dual:
             license_parsed = updated_license
         else:
             license_parsed = str(self.license_expression.parse(ret['license_expression']))
 
         ambiguities = []
@@ -352,14 +363,16 @@
                     about_license = f'An ambiguity was identified in "{ret["license_expression"]}". The ambiguous license is "{real_lic}", identified via "{alias}".'
                 else:
                     about_license = f'An ambiguity was identified in "{ret["license_expression"]}". The ambiguous license is "{real_lic}"-'
                 problem = self.license_db[AMBIG_TAG]["ambiguities"][real_lic]["problem"]
                 ambiguities.append(f'{about_license} Problem: {problem}')
                 tmp_license_expression = re.sub(needle, ' ', tmp_license_expression)
 
+        self.__validate_license(validations, license_parsed)
+
         ret = {
             'queried_license': license_expression,
             FLAME_IDENTIFIED_LICENSE_TAG: license_parsed,
             'identifications': replacements,
             'ambiguities': ambiguities,
             'updated_license': updated_license,
             'license_parsed': license_parsed,
@@ -467,18 +480,57 @@
         :Example:
 
         >>> fl = FossLicenses()
         >>> aliases = fl.alias_list()
 
         """
         if alias_license:
-            return {k: v for k, v in self.license_db[FLAME_ALIASES_TAG].items() if alias_license in v}
+            return {k: v for k, v in self.license_db[FLAME_ALIASES_TAG].items() if alias_license.lower() in v.lower()}
         # List all aliases that exist
         return self.license_db[FLAME_ALIASES_TAG]
 
+    def ambiguities_list(self):
+        """Returns a list of all the ambigious licenses.
+
+        :Example:
+
+        >>> fl = FossLicenses()
+        >>> aliases = fl.ambiguities_list()
+
+        """
+        # List all aliases that exist
+        return self.license_db[AMBIG_TAG]['ambiguities']
+
+    def known_symbols(self):
+        """Returns a list of all all known license symbols.
+
+        :Example:
+
+        >>> fl = FossLicenses()
+        >>> aliases = fl.known_symbols()
+
+        """
+        _symbols = set()
+
+        ambiguities = self.ambiguities_list()
+        for ambig in ambiguities:
+            _symbols.add(ambig)
+            _symbols.update(set(ambiguities[ambig]['aliases']))
+
+        licenses = self.license_db[LICENSES_TAG]
+        for lic in licenses:
+            _symbols.add(lic)
+            _symbols.update(set(licenses[lic]['aliases']))
+
+        operators = self.license_db[LICENSE_OPERATORS_TAG]
+        for op in operators:
+            _symbols.add(op)
+
+        return list(_symbols)
+
     def aliases(self, license_name):
         """Returns a list of all the aliases for a license
 
         :param str license_name: Exact name (SPDXID) of the license
 
         :Example:
 
@@ -534,64 +586,60 @@
 
         >>> fl = FossLicenses()
         >>> compat = fl.expression_compatibility_as('x11-keith-packard')
         >>> print(compat['compatibilities'][0]['name'])
         HPND
 
         """
+
         cache_key = f'{license_expression}__{validations}__{update_dual}'
         if cache_key in self.compat_cache:
             return self.compat_cache.get(cache_key)
 
-        expression_full = self.expression_license(license_expression, update_dual)
+        expression_full = self.expression_license(license_expression, validations, update_dual)
         compats = []
         ret = self.__update_license_expression_helper(self.license_db[COMPATS_TAG],
                                                       'compat',
                                                       expression_full[FLAME_IDENTIFIED_LICENSE_TAG])
         ret['license_expression'] = re.sub(r'\s\s*', ' ', ret['license_expression']).strip()
         compats = ret['identifications']
         compat_license_expression = ret['license_expression']
 
         compat_licenses = [x.strip() for x in re.split('\(|OR|AND|\)', compat_license_expression)]
         compat_licenses = [x for x in compat_licenses if x]
         compat_support = self.__validate_compatibilities_support(compat_licenses)
 
-        if validations:
-            if Validation.SPDX in validations:
-                self.__validate_license_spdx(compat_license_expression)
-            if Validation.RELAXED in validations:
-                self.__validate_license_relaxed(compat_license_expression)
-            if Validation.OSADL in validations:
-                self.__validate_licenses_osadl(compat_support)
+        self.__validate_license(validations, compat_license_expression)
 
         ret = {
             'ambiguities': expression_full['ambiguities'],
             'compatibilities': compats,
             'queried_license': license_expression,
             'identification': expression_full,
             FLAME_IDENTIFIED_LICENSE_TAG: expression_full[FLAME_IDENTIFIED_LICENSE_TAG],
             FLAME_COMPATIBLE_LICENSE_TAG: compat_license_expression,
             'compat_support': compat_support,
         }
         self.compat_cache[cache_key] = ret
         return ret
 
-    def __validate_compatibilities_support(self, licenses):
-        """Returns an object with information about the compatibility status for the license given.
-
-        :param str license_expression: A license expression. E.g "BSD3" or "GPLv2+ || BSD3"
-
-        :Example: supplying only one license, so look at [0]
-
-        >>> fl = FossLicenses()
-        >>> compat = fl.expression_compatibility_as('x11-keith-packard')
-        >>> print(compat['compatibilities'][0]['name'])
-        HPND
+    def __validate_license(self, validations, license_expression):
+        if validations:
+            if Validation.SPDX in validations:
+                self.__validate_license_spdx(license_expression)
+            if Validation.RELAXED in validations:
+                self.__validate_license_relaxed(license_expression)
+            if Validation.OSADL in validations:
+                compat_license_expression = self.expression_compatibility_as(license_expression)['compat_license']
+                compat_licenses = [x.strip() for x in re.split('\(|OR|AND|\)', compat_license_expression)]
+                compat_licenses = [x for x in compat_licenses if x]
+                compat_support = self.__validate_compatibilities_support(compat_licenses)
+                self.__validate_licenses_osadl(compat_support)
 
-        """
+    def __validate_compatibilities_support(self, licenses):
         compat_support = {}
         compat_support['licenses'] = []
         all_supported = True
         for lic in licenses:
             support = self.__validate_compatibility_support(lic)
             compat_support['licenses'].append({
                 'license': lic,
@@ -600,15 +648,15 @@
             all_supported = all_supported and support
         compat_support['supported'] = all_supported
 
         return compat_support
 
     def __validate_compatibility_support(self, lic):
         if not self.supported_licenses:
-            self.support_licenses = osadl_matrix.supported_licenses()
+            self.support_licenses = osadl_matrix.supported_licenses(self.license_matrix_file)
         return lic in self.support_licenses
 
     def __validate_license_spdx(self, expr):
         """
         """
 
         expr_info = self.license_expression.validate(expr)
@@ -626,8 +674,9 @@
             if " " in lic.strip():
                 raise FlameException(f'Found license with multiple words "{lic}"')
 
     def __validate_licenses_osadl(self, compat_supported):
         """
         """
         if not compat_supported['supported']:
-            raise FlameException(f'Not all licenses supported by OSADL\'s compatibility matrix "{compat_supported}"')
+            raise FlameException('Not all licenses supported by OSADL\'s compatibility matrix',
+                                 compat_supported)
```

### Comparing `foss-flame-0.19.9/flame/var/compounds.json` & `foss-flame-0.20.0/flame/var/compounds.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'compounds'": "{insert: [(1, OrderedDict([('spdxid', 'GPL-2.0-only WITH Linux-syscall-note'), "*

 * *                "('aliases', []), ('compatibility_as', 'GPL-2.0-only WITH "*

 * *                "Classpath-exception-2.0')]))]}"}*

```diff
@@ -4,14 +4,19 @@
             "aliases": [
                 "GPL-2.0-with-classpath-exception",
                 "GPL-2.0-only AND Classpath-exception-2.0"
             ],
             "spdxid": "GPL-2.0-only WITH Classpath-exception-2.0"
         },
         {
+            "aliases": [],
+            "compatibility_as": "GPL-2.0-only WITH Classpath-exception-2.0",
+            "spdxid": "GPL-2.0-only WITH Linux-syscall-note"
+        },
+        {
             "aliases": [
                 "GPL-2.0-or-later AND Classpath-exception-2.0"
             ],
             "spdxid": "GPL-2.0-or-later WITH Classpath-exception-2.0"
         },
         {
             "aliases": [
```

### Comparing `foss-flame-0.19.9/flame/var/duals.json` & `foss-flame-0.20.0/flame/var/duals.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/license_schema.json` & `foss-flame-0.20.0/flame/var/license_schema.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/0BSD.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/0BSD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-only.json` & `foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/AGPL-3.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/AGPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Apache-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/Apache-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Apache-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-1.1.json` & `foss-flame-0.20.0/flame/var/licenses/Apache-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Apache-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/Apache-2.0.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988505747126437%*

 * *Differences: {"'aliases'": "{insert: [(86, 'Apache Software License (Apache 2.0)')]}"}*

```diff
@@ -81,15 +81,16 @@
         "Apache 2.0 License",
         "Apache v2.0",
         "Apache 2.0 Software License",
         "Apache Software License (Apache-2.0)",
         "Apache Software License (Apache License, Version 2.0)",
         "Apache 2.",
         "Apache -2.0",
-        "ASL2.0"
+        "ASL2.0",
+        "Apache Software License (Apache 2.0)"
     ],
     "meta": {
         "comment": "",
         "date": "2023-08-29",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "Apache License 2.0",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Artistic-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Artistic-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/Artistic-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Artistic-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Artistic-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/Artistic-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-2-Clause.json` & `foss-flame-0.20.0/flame/var/licenses/BSD-2-Clause.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9864864864864865%*

 * *Differences: {"'aliases'": '{insert: [(32, \'BSD 2-clause license\'), (33, \'BSD 2-clause "Simplified" '*

 * *              "License'), (34, '2-Clause BSD'), (35, 'The 2-Clause BSD License'), (36, 'BSD "*

 * *              "License 2')]}"}*

```diff
@@ -27,15 +27,20 @@
         "two-clause BSD License",
         "2-Clause BSD license",
         "scancode:bsd-simplified",
         "osi:BSD-2-Clause",
         "License BSD 2-clause",
         "BSD 2-Clause \"Simplified\"",
         "BSD 2C",
-        "BSD 2-clause"
+        "BSD 2-clause",
+        "BSD 2-clause license",
+        "BSD 2-clause \"Simplified\" License",
+        "2-Clause BSD",
+        "The 2-Clause BSD License",
+        "BSD License 2"
     ],
     "meta": {
         "comment": "",
         "date": "2023-08-29",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "BSD-2-Clause",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BSD-3-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-3-Clause.json` & `foss-flame-0.20.0/flame/var/licenses/BSD-3-Clause.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9873015873015873%*

 * *Differences: {"'aliases'": "{insert: [(16, '3-Clause BSD'), (56, 'BSD 3-Clause license'), (57, 'BSD 3-Clause "*

 * *              'New\'), (58, \'BSD 3-clause "New" or "Revised" License\'), (59, \'BSD License 3\'), '*

 * *              "(60, 'BSD -3 Clause'), (61, 'BSD 3-clause')], delete: [46]}"}*

```diff
@@ -12,14 +12,15 @@
         "Revised BSD License",
         "Modified BSD License",
         "New BSD License",
         "scancode://bsd-new",
         "The BSD-3-clause License",
         "3-Clause BSD License",
         "3-clause BSD",
+        "3-Clause BSD",
         "Three-clause BSD-style",
         "bsd_3",
         "Modified BSD Licens",
         "Modified BSD Licence",
         "modified BSD Licence",
         "Modified BSD (3-clause)",
         "BSD New",
@@ -42,24 +43,29 @@
         "Three clause BSD license",
         "3 clause BSD license",
         "scancode:bsd-new",
         "osi:BSD-3",
         "osi:BSD-3-Clause",
         "BSD3-clause",
         "BSD 3-Clause",
-        "BSD3-like",
         "new BSD License",
         "BSD-3-clause New",
         "BSD-3-Clause New",
         "BSD 3-Clause \"New\"",
         "BSD License (BSD-3-Clause)",
         "BSD 3C",
         "BSD-3-Clause license",
         "BSD License (new BSD)",
-        "3-clause BSD license"
+        "3-clause BSD license",
+        "BSD 3-Clause license",
+        "BSD 3-Clause New",
+        "BSD 3-clause \"New\" or \"Revised\" License",
+        "BSD License 3",
+        "BSD -3 Clause",
+        "BSD 3-clause"
     ],
     "meta": {
         "comment": "",
         "date": "2023-08-22",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "The 3-Clause BSD License",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause-UC.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause-UC.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSD-4-Clause.json` & `foss-flame-0.20.0/flame/var/licenses/BSD-4-Clause.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666666%*

 * *Differences: {"'aliases'": "{insert: [(11, 'Original BSD license')]}"}*

```diff
@@ -6,15 +6,16 @@
         "BSD License (original)",
         "bsd-4-clause",
         "BSD 4-Clause License",
         "scancode://bsd-original",
         "BSD-Original",
         "BSD with advertising",
         "BSD 4-Clause",
-        "scancode:bsd-original"
+        "scancode:bsd-original",
+        "Original BSD license"
     ],
     "meta": {
         "comment": "",
         "date": "2023-08-29",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "BSD-4-Clause",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BSL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/BSL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/BSL-1.0.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99%*

 * *Differences: {"'aliases'": "{insert: [(18, 'Boost-1.0'), (19, 'Boost Software license 1.0')]}"}*

```diff
@@ -13,15 +13,17 @@
         "BSL 1.0",
         "BSL Version 1.0",
         "BSL v1.0",
         "Boost Software License, Version 1.0",
         "Boost Software License v1.0",
         "scancode:boost-1.0",
         "osi:BSL-1.0",
-        "BSL 1.0 License"
+        "BSL 1.0 License",
+        "Boost-1.0",
+        "Boost Software license 1.0"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "Boost Software License 1.0",
     "scancode_key": "boost-1.0",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/BlueOak-1.0.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/BlueOak-1.0.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-3.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-3.0.json` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-3.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-4.0.json` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-4.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-2.5.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-2.5.json` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-2.5.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-3.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-3.0.json` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-3.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-4.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC-BY-SA-4.0.json` & `foss-flame-0.20.0/flame/var/licenses/CC-BY-SA-4.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC0-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CC0-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CC0-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/CC0-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CDDL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CDDL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/CDDL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/CDDL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/CDDL-1.1.json` & `foss-flame-0.20.0/flame/var/licenses/CDDL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Classpath-exception-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Classpath-exception-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EPL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/EPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EPL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/EPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EPL-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/EPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EPL-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/EPL-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.1.json` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.2.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/EUPL-1.2.json` & `foss-flame-0.20.0/flame/var/licenses/EUPL-1.2.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/FTL.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/FTL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GCC-exception-3.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GCC-exception-3.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-1.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-only.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-1.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-1.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-1.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-1.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-2.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-only.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-2.0-only.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923076923076923%*

 * *Differences: {"'aliases'": "{insert: [(59, 'GPL-2.0 License'), (61, 'GNU General Public License version 2'), "*

 * *              "(62, 'GNU General Public License version 2.0 (GPLv2)'), (63, 'GPLV2'), (64, 'GPL v2 "*

 * *              "License')]}"}*

```diff
@@ -55,15 +55,20 @@
         "GNU General Public License, v. 2.0",
         "GNU General Public License (v2.0",
         "scancode:gpl-2.0",
         "osi:GPL-2.0",
         "GNU General Public License v2 (GPLv2)",
         "GPLv2.0",
         "GPL-2.0 license",
-        "version 2 of the GNU ** General Public License. */"
+        "GPL-2.0 License",
+        "version 2 of the GNU ** General Public License. */",
+        "GNU General Public License version 2",
+        "GNU General Public License version 2.0 (GPLv2)",
+        "GPLV2",
+        "GPL v2 License"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "GPL 2.0 only",
     "scancode_key": "gpl-2.0",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-2.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-2.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-2.0-or-later.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936170212765958%*

 * *Differences: {"'aliases'": "{insert: [(44, 'GPL version 2 or any later version'), (45, 'GPL (>= 2)'), (46, 'GPL "*

 * *              "2+')]}"}*

```diff
@@ -39,15 +39,18 @@
         "GNU General Public License, either Version 2 of the license, or (at your option) any later version",
         "GNU General Public License (version 2 or later)",
         "GNU General Public License as published by the Free Software Foundation (the \"GPL\"); either version 2 of the GPL, or (at your option) any later version",
         "GNU General Public License, either version 2 or (at your opinion) any newer version",
         "GNU General Public License, V2 or later",
         "scancode:gpl-2.0-plus",
         "GNU General Public License v2 or later (GPLv2+)",
-        "GPLv2.0+"
+        "GPLv2.0+",
+        "GPL version 2 or any later version",
+        "GPL (>= 2)",
+        "GPL 2+"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "GPL 2.0 or later",
     "scancode_key": "gpl-2.0-plus",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-only.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-3.0-only.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984848484848484%*

 * *Differences: {"'aliases'": "{insert: [(65, 'GPL-3.0 license')]}"}*

```diff
@@ -60,15 +60,16 @@
         "gpl_v3",
         "GPL V3",
         "scancode:gpl-3.0",
         "osi:GPL-3.0",
         "GNU General Public License v3 (GPLv3)",
         "GPLv3.0",
         "GNU Lesser General Public License (GNU Lesser GPL), version 3",
-        "GPL v. 3.0"
+        "GPL v. 3.0",
+        "GPL-3.0 license"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "GNU General Public License 3.0",
     "scancode_key": "gpl-3.0",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/GPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/GPL-3.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/GPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/HPND.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/HPND.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/HPND.json` & `foss-flame-0.20.0/flame/var/licenses/HPND.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ICU.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ICU.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/IJG.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/IJG.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ISC.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ISC.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/JSON.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/JSON.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-only.json` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-only.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960000000000001%*

 * *Differences: {"'aliases'": "{insert: [(48, 'GNU Lesser General Public License, version 2.1'), (49, 'Lesser "*

 * *              "General Public License 2.1')]}"}*

```diff
@@ -43,15 +43,17 @@
         "GNU Lesser General Public License as published by the Free Software Foundation, version 2.1",
         "This is the first released version of the Lesser GPL.  It also counts as the successor of the GNU Library Public License, version 2, hence the version number 2.1.",
         "GNU Lesser Public License (LGPL) Version 2.1",
         "GNU Lesser General Public License as published by the Free Software Foundation; version 2.1 of the License",
         "http://www.gnu.org/licenses/old-licenses/lgpl-2.1.html",
         "https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html",
         "scancode:lgpl-2.1",
-        "osi:LGPL-2.1"
+        "osi:LGPL-2.1",
+        "GNU Lesser General Public License, version 2.1",
+        "Lesser General Public License 2.1"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "GNU Lesser General Public License 2.1",
     "scancode_key": "lgpl-2.1",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-2.1-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/LGPL-2.1-or-later.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981132075471699%*

 * *Differences: {"'aliases'": "{insert: [(52, 'LGPL-2.1 or later')]}"}*

```diff
@@ -47,15 +47,16 @@
         "GNU Lesser General Public License as published by the Free Software Foundation, either version 2.1 of the License, or (at your option) any later version",
         "GNU Lesser General Public License as published by the Free Software Foundation; either version 2.1 of the License, or (at your option) any later version",
         "GNU Lesser General Public License, V2.1 or later",
         "GNU Lesser General Public License as ~ published by the Free Software Foundation; either version 2.1 of ~ the License, or (at your option) any later version",
         "scancode:lgpl-2.1-plus",
         "LGPLv2, greater",
         "GNU Lesser General Public License v2 or later (LGPLv2+)",
-        "LGPLv2.0+"
+        "LGPLv2.0+",
+        "LGPL-2.1 or later"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "GNU Lesser General Public License 2.1 or later",
     "scancode_key": "lgpl-2.1-plus",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-only.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-only.json` & `foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-only.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-or-later.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LGPL-3.0-or-later.json` & `foss-flame-0.20.0/flame/var/licenses/LGPL-3.0-or-later.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Latex2e.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Latex2e.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Libpng.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Libpng.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-docbook.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT-0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MIT-0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT-advertising.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MIT-advertising.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT-advertising.json` & `foss-flame-0.20.0/flame/var/licenses/MIT-advertising.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT-open-group.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MIT-open-group.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MIT.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MIT.json` & `foss-flame-0.20.0/flame/var/licenses/MIT.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.990625%*

 * *Differences: {"'aliases'": "{insert: [(29, 'MIT/Expat'), (30, 'The MIT License (MIT)'), (31, '[MIT] License')]}"}*

```diff
@@ -24,15 +24,18 @@
         "http://opensource.org/licenses/MIT",
         "http://opensource.org/licenses/mit-license.php",
         "Licensed under the MIT",
         "licensed under the MIT",
         "MIT LICENSE",
         "scancode:mit",
         "osi:MIT",
-        "MIT License (MIT)"
+        "MIT License (MIT)",
+        "MIT/Expat",
+        "The MIT License (MIT)",
+        "[MIT] License"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "MIT License",
     "scancode_key": "mit",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/MITNFA.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MITNFA.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/MPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-1.1.json` & `foss-flame-0.20.0/flame/var/licenses/MPL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/MPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/MPL-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/MPL-2.0.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9952380952380953%*

 * *Differences: {"'aliases'": "{insert: [(20, 'MPL-2.0+')]}"}*

```diff
@@ -15,15 +15,16 @@
         "Mozilla License Version 2.0",
         "Mozilla Public Licence 2.0",
         "Mozilla Public License 2.0 (MPL 2.0)",
         "MPLv2.0",
         "MPL-2",
         "scancode:mpl-2.0",
         "osi:MPL-2.0",
-        "MPLv2"
+        "MPLv2",
+        "MPL-2.0+"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "Mozilla Public License 2.0",
     "scancode_key": "mpl-2.0",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/NCSA.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/NCSA.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/NCSA.json` & `foss-flame-0.20.0/flame/var/licenses/NCSA.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/NTP.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/NTP.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ODC-By-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ODC-By-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/ODC-By-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/OFL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/OFL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/OFL-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/OFL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/OFL-1.1.json` & `foss-flame-0.20.0/flame/var/licenses/OFL-1.1.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/OML.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/OML.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/OpenSSL.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/OpenSSL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Plexus.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Plexus.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/PostgreSQL.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/PostgreSQL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Python-2.0.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Python-2.0.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Python-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Python-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Python-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/Python-2.0.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9882352941176471%*

 * *Differences: {"'aliases'": "{insert: [(15, 'PSF v2.0'), (16, 'PSF 2.0')]}"}*

```diff
@@ -10,15 +10,17 @@
         "scancode://psf-2.0",
         "scancode://python",
         "Python Software Foundation License 2",
         "PSF-2",
         "scancode:python",
         "osi:Python-2.0",
         "PSFv2",
-        "Python-2"
+        "Python-2",
+        "PSF v2.0",
+        "PSF 2.0"
     ],
     "meta": {
         "comment": "",
         "disclaimer": "https://github.com/hesa/license-db/tree/main/var/disclamer.md"
     },
     "name": "Python Software Foundation License v2",
     "scancode_key": "python",
```

### Comparing `foss-flame-0.19.9/flame/var/licenses/RSA-MD.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/RSA-MD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SAX-PD.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/SAX-PD.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SAX-PD.json` & `foss-flame-0.20.0/flame/var/licenses/SAX-PD.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/SGI-B-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SGI-B-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/SGI-B-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/SSPL-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SSPL-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/SSPL-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SWL.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/SWL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/SWL.json` & `foss-flame-0.20.0/flame/var/licenses/SWL.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Sendmail.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Sendmail.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/TCL.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/TCL.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/TU-Berlin-1.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-1.0.json` & `foss-flame-0.20.0/flame/var/licenses/TU-Berlin-1.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/TU-Berlin-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/TU-Berlin-2.0.json` & `foss-flame-0.20.0/flame/var/licenses/TU-Berlin-2.0.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Unlicense.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Unlicense.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Vim.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Vim.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/W3C.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/W3C.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/W3C.json` & `foss-flame-0.20.0/flame/var/licenses/W3C.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/WTFPL.json` & `foss-flame-0.20.0/flame/var/licenses/WTFPL.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/X11-distribute-modifications-variant.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/X11-distribute-modifications-variant.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/X11.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/X11.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ZPL-1.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ZPL-1.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ZPL-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ZPL-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/ZPL-2.1.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/ZPL-2.1.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Zlib.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/Zlib.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/Zlib.json` & `foss-flame-0.20.0/flame/var/licenses/Zlib.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/bzip2-1.0.6.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/bzip2-1.0.6.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/curl.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/curl.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/libpng-2.0.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/libpng-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/libtiff.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/libtiff.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.LICENSE` & `foss-flame-0.20.0/flame/var/licenses/x11-keith-packard.LICENSE`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/flame/var/licenses/x11-keith-packard.json` & `foss-flame-0.20.0/flame/var/licenses/x11-keith-packard.json`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/foss_flame.egg-info/PKG-INFO` & `foss-flame-0.20.0/foss_flame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: foss-flame
-Version: 0.19.9
+Version: 0.20.0
 Summary: FOSS License Additional Metadata
-Home-page: https://github.com/hesa/license-db
+Home-page: https://github.com/hesa/foss-licenses
 Author: Henrik Sanklef
 Author-email: hesa@sandklef.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -54,19 +54,19 @@
 
 # Background
 
 There are lots of software licenses out there (e.g. see [ScanCode LicenseDB](https://scancode-licensedb.aboutcode.org/)), some of them are FOSS and some not. In this project we primarily focus on FOSS licenses.
 
 ## License name proliferation
 
-When you're working with compliance you are used to liceses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information machine readable.
+When you're working with compliance you are used to licenses called differently in source code or by tools (e.g. `GPLv2`, `GPL (v2)` and `GNU General Public License Version 2`) when all you really want too see is the [SPDX identifier](https://spdx.org/licenses/) `GPL-2.0-only`. A seasoned compliance engineer or lawyer knows this already, but we need this information to be machine readable.
 
 ## License proliferation
 
-Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported in for example the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and not, but we need to make it possible for a machine to assist us. 
+Another problem you face when working with compliance is the need to check whether the licenses in a combined work are compatible. One example is the [`X11-Style (Keith Packard)`](https://scancode-licensedb.aboutcode.org/x11-keith-packard.html) license, which really is the same license as the [Historical Permission Notice and Disclaimer - sell variant](https://spdx.org/licenses/HPND-sell-variant.html). `X11-Style (Keith Packard)` is not supported for example in the OSADL matrix, but `HPND-sell-variant` is. Again, a seasoned license engineer or lawyer knows which licenses are compatible and which are not, but we need to make it possible for a machine to assist us. 
 
 # About
 
 This projet aims at providing a database with:
 
 * "all" different names for a license in a database
```

### Comparing `foss-flame-0.19.9/foss_flame.egg-info/SOURCES.txt` & `foss-flame-0.20.0/foss_flame.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,70 +16,106 @@
 flame/var/ambiguities.json
 flame/var/compounds.json
 flame/var/duals.json
 flame/var/license_schema.json
 flame/var/operators.json
 flame/var/licenses/0BSD.LICENSE
 flame/var/licenses/0BSD.json
+flame/var/licenses/AFL-1.1.LICENSE
+flame/var/licenses/AFL-1.1.json
+flame/var/licenses/AFL-1.2.LICENSE
+flame/var/licenses/AFL-1.2.json
+flame/var/licenses/AFL-2.0.LICENSE
+flame/var/licenses/AFL-2.0.json
+flame/var/licenses/AFL-2.1.LICENSE
+flame/var/licenses/AFL-2.1.json
+flame/var/licenses/AFL-3.0.LICENSE
+flame/var/licenses/AFL-3.0.json
 flame/var/licenses/AGPL-3.0-only.LICENSE
 flame/var/licenses/AGPL-3.0-only.json
 flame/var/licenses/AGPL-3.0-or-later.LICENSE
 flame/var/licenses/AGPL-3.0-or-later.json
 flame/var/licenses/Apache-1.0.LICENSE
 flame/var/licenses/Apache-1.0.json
 flame/var/licenses/Apache-1.1.LICENSE
 flame/var/licenses/Apache-1.1.json
 flame/var/licenses/Apache-2.0.LICENSE
 flame/var/licenses/Apache-2.0.json
 flame/var/licenses/Artistic-1.0.LICENSE
 flame/var/licenses/Artistic-1.0.json
 flame/var/licenses/Artistic-2.0.LICENSE
 flame/var/licenses/Artistic-2.0.json
+flame/var/licenses/Autoconf-exception-2.0.LICENSE
+flame/var/licenses/Autoconf-exception-2.0.json
+flame/var/licenses/Autoconf-exception-3.0.LICENSE
+flame/var/licenses/Autoconf-exception-3.0.json
+flame/var/licenses/BSD-1-Clause.LICENSE
+flame/var/licenses/BSD-1-Clause.json
+flame/var/licenses/BSD-2-Clause-Patent.LICENSE
+flame/var/licenses/BSD-2-Clause-Patent.json
 flame/var/licenses/BSD-2-Clause.LICENSE
 flame/var/licenses/BSD-2-Clause.json
 flame/var/licenses/BSD-3-Clause.LICENSE
 flame/var/licenses/BSD-3-Clause.json
 flame/var/licenses/BSD-4-Clause-UC.LICENSE
 flame/var/licenses/BSD-4-Clause-UC.json
 flame/var/licenses/BSD-4-Clause.LICENSE
 flame/var/licenses/BSD-4-Clause.json
+flame/var/licenses/BSD-Source-Code.LICENSE
+flame/var/licenses/BSD-Source-Code.json
 flame/var/licenses/BSL-1.0.LICENSE
 flame/var/licenses/BSL-1.0.json
 flame/var/licenses/Beerware.LICENSE
 flame/var/licenses/Beerware.json
+flame/var/licenses/Bitstream-Vera.LICENSE
+flame/var/licenses/Bitstream-Vera.json
 flame/var/licenses/BlueOak-1.0.0.LICENSE
 flame/var/licenses/BlueOak-1.0.0.json
 flame/var/licenses/CC-BY-3.0.LICENSE
 flame/var/licenses/CC-BY-3.0.json
 flame/var/licenses/CC-BY-4.0.LICENSE
 flame/var/licenses/CC-BY-4.0.json
 flame/var/licenses/CC-BY-SA-2.5.LICENSE
 flame/var/licenses/CC-BY-SA-2.5.json
 flame/var/licenses/CC-BY-SA-3.0.LICENSE
 flame/var/licenses/CC-BY-SA-3.0.json
 flame/var/licenses/CC-BY-SA-4.0.LICENSE
 flame/var/licenses/CC-BY-SA-4.0.json
+flame/var/licenses/CC-PDDC.LICENSE
+flame/var/licenses/CC-PDDC.json
 flame/var/licenses/CC0-1.0.LICENSE
 flame/var/licenses/CC0-1.0.json
 flame/var/licenses/CDDL-1.0.LICENSE
 flame/var/licenses/CDDL-1.0.json
 flame/var/licenses/CDDL-1.1.LICENSE
 flame/var/licenses/CDDL-1.1.json
+flame/var/licenses/CPL-1.0.LICENSE
+flame/var/licenses/CPL-1.0.json
 flame/var/licenses/Classpath-exception-2.0.LICENSE
 flame/var/licenses/Classpath-exception-2.0.json
+flame/var/licenses/ECL-1.0.LICENSE
+flame/var/licenses/ECL-1.0.json
 flame/var/licenses/EPL-1.0.LICENSE
 flame/var/licenses/EPL-1.0.json
 flame/var/licenses/EPL-2.0.LICENSE
 flame/var/licenses/EPL-2.0.json
 flame/var/licenses/EUPL-1.0.LICENSE
 flame/var/licenses/EUPL-1.0.json
 flame/var/licenses/EUPL-1.1.LICENSE
 flame/var/licenses/EUPL-1.1.json
 flame/var/licenses/EUPL-1.2.LICENSE
 flame/var/licenses/EUPL-1.2.json
+flame/var/licenses/FSFAP.LICENSE
+flame/var/licenses/FSFAP.json
+flame/var/licenses/FSFUL.LICENSE
+flame/var/licenses/FSFUL.json
+flame/var/licenses/FSFULLR.LICENSE
+flame/var/licenses/FSFULLR.json
+flame/var/licenses/FSFULLRWD.LICENSE
+flame/var/licenses/FSFULLRWD.json
 flame/var/licenses/FTL.LICENSE
 flame/var/licenses/FTL.json
 flame/var/licenses/GCC-exception-3.1.LICENSE
 flame/var/licenses/GCC-exception-3.1.json
 flame/var/licenses/GPL-1.0-only.LICENSE
 flame/var/licenses/GPL-1.0-only.json
 flame/var/licenses/GPL-1.0-or-later.LICENSE
@@ -92,14 +128,16 @@
 flame/var/licenses/GPL-3.0-only.json
 flame/var/licenses/GPL-3.0-or-later.LICENSE
 flame/var/licenses/GPL-3.0-or-later.json
 flame/var/licenses/HPND.LICENSE
 flame/var/licenses/HPND.json
 flame/var/licenses/ICU.LICENSE
 flame/var/licenses/ICU.json
+flame/var/licenses/IJG-short.LICENSE
+flame/var/licenses/IJG-short.json
 flame/var/licenses/IJG.LICENSE
 flame/var/licenses/IJG.json
 flame/var/licenses/ISC.LICENSE
 flame/var/licenses/ISC.json
 flame/var/licenses/JSON.LICENSE
 flame/var/licenses/JSON.json
 flame/var/licenses/LGPL-2.0-only.LICENSE
@@ -110,28 +148,36 @@
 flame/var/licenses/LGPL-2.1-only.json
 flame/var/licenses/LGPL-2.1-or-later.LICENSE
 flame/var/licenses/LGPL-2.1-or-later.json
 flame/var/licenses/LGPL-3.0-only.LICENSE
 flame/var/licenses/LGPL-3.0-only.json
 flame/var/licenses/LGPL-3.0-or-later.LICENSE
 flame/var/licenses/LGPL-3.0-or-later.json
+flame/var/licenses/LLVM-exception.LICENSE
+flame/var/licenses/LLVM-exception.json
 flame/var/licenses/Latex2e.LICENSE
 flame/var/licenses/Latex2e.json
 flame/var/licenses/Libpng.LICENSE
 flame/var/licenses/Libpng.json
+flame/var/licenses/LicenseRef-scancode-boost-original.LICENSE
+flame/var/licenses/LicenseRef-scancode-boost-original.json
 flame/var/licenses/LicenseRef-scancode-docbook.LICENSE
 flame/var/licenses/LicenseRef-scancode-docbook.json
+flame/var/licenses/LicenseRef-scancode-g10-permissive.LICENSE
+flame/var/licenses/LicenseRef-scancode-g10-permissive.json
 flame/var/licenses/LicenseRef-scancode-iso-8879.LICENSE
 flame/var/licenses/LicenseRef-scancode-iso-8879.json
 flame/var/licenses/LicenseRef-scancode-public-domain.LICENSE
 flame/var/licenses/LicenseRef-scancode-public-domain.json
 flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.LICENSE
 flame/var/licenses/LicenseRef-scancode-wtfpl-1.0.json
 flame/var/licenses/LicenseRef-scancode-zpl-1.0.LICENSE
 flame/var/licenses/LicenseRef-scancode-zpl-1.0.json
+flame/var/licenses/Linux-syscall-note.LICENSE
+flame/var/licenses/Linux-syscall-note.json
 flame/var/licenses/MIT-0.LICENSE
 flame/var/licenses/MIT-0.json
 flame/var/licenses/MIT-advertising.LICENSE
 flame/var/licenses/MIT-advertising.json
 flame/var/licenses/MIT-open-group.LICENSE
 flame/var/licenses/MIT-open-group.json
 flame/var/licenses/MIT.LICENSE
@@ -176,14 +222,16 @@
 flame/var/licenses/SGI-B-2.0.json
 flame/var/licenses/SSPL-1.0.LICENSE
 flame/var/licenses/SSPL-1.0.json
 flame/var/licenses/SWL.LICENSE
 flame/var/licenses/SWL.json
 flame/var/licenses/Sendmail.LICENSE
 flame/var/licenses/Sendmail.json
+flame/var/licenses/Sleepycat.LICENSE
+flame/var/licenses/Sleepycat.json
 flame/var/licenses/TCL.LICENSE
 flame/var/licenses/TCL.json
 flame/var/licenses/TU-Berlin-1.0.LICENSE
 flame/var/licenses/TU-Berlin-1.0.json
 flame/var/licenses/TU-Berlin-2.0.LICENSE
 flame/var/licenses/TU-Berlin-2.0.json
 flame/var/licenses/Unlicense.LICENSE
```

### Comparing `foss-flame-0.19.9/setup.cfg` & `foss-flame-0.20.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `foss-flame-0.19.9/setup.py` & `foss-flame-0.20.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     version=SW_VERSION,
     author="Henrik Sanklef",
     author_email="hesa@sandklef.com",
     description="FOSS License Additional Metadata",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     license_files=('LICENSES/CC-BY-4.0.txt', 'LICENSES/GPL-3.0-or-later.txt'),
-    url="https://github.com/hesa/license-db",
+    url="https://github.com/hesa/foss-licenses",
     packages=['flame'],
     entry_points={
         "console_scripts": [
             "flame = flame.__main__:main",
         ],
     },
     package_data={'flame': ['var/*.json', 'var/licenses/*.*']},
```

