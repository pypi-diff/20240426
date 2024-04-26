# Comparing `tmp/bibiinstaller-0.1.2.tar.gz` & `tmp/bibiinstaller-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibiinstaller-0.1.2.tar", last modified: Wed Apr 17 14:11:29 2024, max compression
+gzip compressed data, was "bibiinstaller-0.1.3.tar", last modified: Fri Apr 26 06:16:34 2024, max compression
```

## Comparing `bibiinstaller-0.1.2.tar` & `bibiinstaller-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.251905 bibiinstaller-0.1.2/
--rw-rw-rw-   0        0        0     1251 2024-04-13 13:51:35.000000 bibiinstaller-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      305 2024-04-13 10:21:15.000000 bibiinstaller-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3306 2024-04-17 14:11:29.250904 bibiinstaller-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2517 2024-04-15 03:15:54.000000 bibiinstaller-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.776904 bibiinstaller-0.1.2/docs/
--rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiinstaller-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiinstaller-0.1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.803916 bibiinstaller-0.1.2/docs/source/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.836903 bibiinstaller-0.1.2/docs/source/_static/
--rw-rw-rw-   0        0        0    35080 2024-04-13 10:50:31.000000 bibiinstaller-0.1.2/docs/source/_static/bibiinstaller.png
--rw-rw-rw-   0        0        0     6986 2024-04-13 10:52:53.000000 bibiinstaller-0.1.2/docs/source/conf.py
--rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiinstaller-0.1.2/docs/source/install.rst
--rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiinstaller-0.1.2/docs/source/quickstart.rst
--rw-rw-rw-   0        0        0     1028 2024-04-17 14:10:12.000000 bibiinstaller-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 14:11:29.251905 bibiinstaller-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1055 2024-04-17 14:10:03.000000 bibiinstaller-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.748904 bibiinstaller-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.858905 bibiinstaller-0.1.2/src/bibiinstaller/
--rw-rw-rw-   0        0        0      106 2024-04-17 14:10:31.000000 bibiinstaller-0.1.2/src/bibiinstaller/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.748904 bibiinstaller-0.1.2/src/bibiinstaller/assets/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.908904 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/
--rw-rw-rw-   0        0        0      450 2024-03-21 05:16:41.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.939905 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/exes/
--rwxrwxrwx   0        0        0    62464 2024-04-13 03:52:45.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe
--rw-rw-rw-   0        0        0       69 2024-04-13 03:59:40.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/exes/config.ini
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.067905 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/
--rwxrwxrwx   0        0        0  6142464 2023-11-19 10:07:11.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe
--rw-rw-rw-   0        0        0      551 2024-04-17 03:15:20.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini
--rw-rw-rw-   0        0        0      217 2024-04-13 11:12:54.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/commands.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.092905 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/micromamba/
--rwxrwxrwx   0        0        0  9011200 2024-04-10 22:44:34.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.124903 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/mirrors/
--rw-rw-rw-   0        0        0      810 2024-04-12 10:39:24.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/mirrors/.condarc
--rw-rw-rw-   0        0        0      123 2024-04-12 10:38:00.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/mirrors/.mambarc
--rw-rw-rw-   0        0        0      503 2024-04-12 10:39:44.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/mirrors/pip.ini
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.135903 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:28.750906 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/Plugins/
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.153940 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/
--rw-rw-rw-   0        0        0     3072 2024-03-06 07:19:53.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll
--rw-rw-rw-   0        0        0  1640084 2024-04-13 11:06:42.000000 bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip
--rw-rw-rw-   0        0        0      642 2024-04-13 14:50:20.000000 bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_configs.py
--rw-rw-rw-   0        0        0    41809 2024-04-17 02:33:30.000000 bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_windows.py
--rw-rw-rw-   0        0        0     3244 2024-04-16 14:56:38.000000 bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_windows.yaml
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.203939 bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/
--rw-rw-rw-   0        0        0    14917 2024-04-04 09:53:45.000000 bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/application.nsi
--rw-rw-rw-   0        0        0    14990 2024-04-04 09:53:13.000000 bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/bibiinstaller.nsi
--rw-rw-rw-   0        0        0    14917 2024-03-06 07:19:53.000000 bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/spyder.nsi
--rw-rw-rw-   0        0        0     1479 2024-04-04 15:14:40.000000 bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/test_nsi_templates.py
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.236932 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/
--rw-rw-rw-   0        0        0      219 2024-04-05 12:09:46.000000 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/add_packages.txt
--rw-rw-rw-   0        0        0      121 2024-04-04 14:14:53.000000 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/editable_packages.txt
--rw-rw-rw-   0        0        0      143 2024-04-04 14:13:18.000000 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/extra_packages.txt
--rw-rw-rw-   0        0        0      216 2024-04-08 09:43:12.000000 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/skip_packages.txt
--rw-rw-rw-   0        0        0      188 2024-04-04 14:13:52.000000 bibiinstaller-0.1.2/src/bibiinstaller/package_configs/unwanted_packages.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.249905 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/
--rw-rw-rw-   0        0        0     3306 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 14:11:28.000000 bibiinstaller-0.1.2/src/bibiinstaller.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 14:11:29.247905 bibiinstaller-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2024-04-02 14:37:56.000000 bibiinstaller-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2476 2024-04-17 02:30:31.000000 bibiinstaller-0.1.2/tests/learn_env_path.py
--rw-rw-rw-   0        0        0     1731 2024-04-13 13:28:32.000000 bibiinstaller-0.1.2/tests/learn_pypi_yarg.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.507533 bibiinstaller-0.1.3/
+-rw-rw-rw-   0        0        0     1251 2024-04-13 13:51:35.000000 bibiinstaller-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      305 2024-04-13 10:21:15.000000 bibiinstaller-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3306 2024-04-26 06:16:34.507533 bibiinstaller-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2517 2024-04-15 03:15:54.000000 bibiinstaller-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.592954 bibiinstaller-0.1.3/docs/
+-rw-rw-rw-   0        0        0      584 2021-10-13 17:26:42.000000 bibiinstaller-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0       96 2024-04-10 05:06:00.000000 bibiinstaller-0.1.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.655632 bibiinstaller-0.1.3/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.686876 bibiinstaller-0.1.3/docs/source/_static/
+-rw-rw-rw-   0        0        0    35080 2024-04-13 10:50:31.000000 bibiinstaller-0.1.3/docs/source/_static/bibiinstaller.png
+-rw-rw-rw-   0        0        0     6986 2024-04-13 10:52:53.000000 bibiinstaller-0.1.3/docs/source/conf.py
+-rw-rw-rw-   0        0        0      396 2021-10-28 07:29:17.000000 bibiinstaller-0.1.3/docs/source/install.rst
+-rw-rw-rw-   0        0        0      782 2021-10-28 07:29:27.000000 bibiinstaller-0.1.3/docs/source/quickstart.rst
+-rw-rw-rw-   0        0        0     1028 2024-04-26 06:15:38.000000 bibiinstaller-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-26 06:16:34.507533 bibiinstaller-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1055 2024-04-17 14:10:03.000000 bibiinstaller-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.541665 bibiinstaller-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.702328 bibiinstaller-0.1.3/src/bibiinstaller/
+-rw-rw-rw-   0        0        0      106 2024-04-26 06:15:52.000000 bibiinstaller-0.1.3/src/bibiinstaller/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.541665 bibiinstaller-0.1.3/src/bibiinstaller/assets/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.733583 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/
+-rw-rw-rw-   0        0        0      450 2024-03-21 05:16:41.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.780453 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/exes/
+-rwxrwxrwx   0        0        0    62464 2024-04-13 03:52:45.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe
+-rw-rw-rw-   0        0        0       69 2024-04-13 03:59:40.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/exes/config.ini
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.997295 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/
+-rwxrwxrwx   0        0        0  6142464 2023-11-19 10:07:11.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe
+-rw-rw-rw-   0        0        0      551 2024-04-17 03:15:20.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini
+-rw-rw-rw-   0        0        0      217 2024-04-13 11:12:54.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/commands.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.149352 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/micromamba/
+-rwxrwxrwx   0        0        0  9011200 2024-04-10 22:44:34.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.243110 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/mirrors/
+-rw-rw-rw-   0        0        0      810 2024-04-12 10:39:24.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/mirrors/.condarc
+-rw-rw-rw-   0        0        0      123 2024-04-12 10:38:00.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/mirrors/.mambarc
+-rw-rw-rw-   0        0        0      503 2024-04-12 10:39:44.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/mirrors/pip.ini
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.305759 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:33.557272 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/Plugins/
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.355722 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/
+-rw-rw-rw-   0        0        0     3072 2024-03-06 07:19:53.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll
+-rw-rw-rw-   0        0        0  1640084 2024-04-13 11:06:42.000000 bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip
+-rw-rw-rw-   0        0        0      744 2024-04-26 06:00:32.000000 bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_configs.py
+-rw-rw-rw-   0        0        0    42784 2024-04-26 06:13:14.000000 bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_windows.py
+-rw-rw-rw-   0        0        0     3244 2024-04-16 14:56:38.000000 bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_windows.yaml
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.445059 bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/
+-rw-rw-rw-   0        0        0    14917 2024-04-04 09:53:45.000000 bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/application.nsi
+-rw-rw-rw-   0        0        0    14990 2024-04-04 09:53:13.000000 bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/bibiinstaller.nsi
+-rw-rw-rw-   0        0        0    14917 2024-03-06 07:19:53.000000 bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/spyder.nsi
+-rw-rw-rw-   0        0        0     1479 2024-04-04 15:14:40.000000 bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/test_nsi_templates.py
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.476275 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/
+-rw-rw-rw-   0        0        0      219 2024-04-05 12:09:46.000000 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/add_packages.txt
+-rw-rw-rw-   0        0        0      121 2024-04-04 14:14:53.000000 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/editable_packages.txt
+-rw-rw-rw-   0        0        0      143 2024-04-04 14:13:18.000000 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/extra_packages.txt
+-rw-rw-rw-   0        0        0      216 2024-04-08 09:43:12.000000 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/skip_packages.txt
+-rw-rw-rw-   0        0        0      188 2024-04-04 14:13:52.000000 bibiinstaller-0.1.3/src/bibiinstaller/package_configs/unwanted_packages.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.507533 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/
+-rw-rw-rw-   0        0        0     3306 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       75 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-26 06:16:33.000000 bibiinstaller-0.1.3/src/bibiinstaller.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-26 06:16:34.491927 bibiinstaller-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-02 14:37:56.000000 bibiinstaller-0.1.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2476 2024-04-17 02:30:31.000000 bibiinstaller-0.1.3/tests/learn_env_path.py
+-rw-rw-rw-   0        0        0     1731 2024-04-13 13:28:32.000000 bibiinstaller-0.1.3/tests/learn_pypi_yarg.py
```

### Comparing `bibiinstaller-0.1.2/LICENSE.txt` & `bibiinstaller-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/PKG-INFO` & `bibiinstaller-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibiinstaller
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bibi Installer using pynsist for Windows
 Home-page: https://github.com/bibiparrot/bibiinstaller
 Author: Chunqi Shi
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiinstaller
 Project-URL: Issues, https://github.com/bibiparrot/bibiinstaller/issues
```

### Comparing `bibiinstaller-0.1.2/README.md` & `bibiinstaller-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/docs/Makefile` & `bibiinstaller-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/docs/source/_static/bibiinstaller.png` & `bibiinstaller-0.1.3/docs/source/_static/bibiinstaller.png`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/docs/source/conf.py` & `bibiinstaller-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/docs/source/quickstart.rst` & `bibiinstaller-0.1.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/pyproject.toml` & `bibiinstaller-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bibiinstaller"
-version = "0.1.2"
+version = "0.1.3"
 description = "Bibi Installer using pynsist for Windows"
 authors = [
     {name = "Chunqi SHI", email = "chunqishi@gmail.com"},
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bibiinstaller-0.1.2/setup.py` & `bibiinstaller-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/exes/bibiinstaller_app.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/icon_configs/ResourceHacker.ini`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/micromamba/micromamba-1.5.7-win-64.exe`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/mirrors/.condarc` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/mirrors/.condarc`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/Plugins/x86-unicode/WinShell.dll`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip` & `bibiinstaller-0.1.3/src/bibiinstaller/assets/Windows/nsis/nsis-3.10-win.zip`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_configs.py` & `bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,11 +30,13 @@
 SKIP_PYPI_PACKAGES: list = []
 EDITABLE_PACKAGES: list = []
 UNWANTED_PACKAGES: list = []
 
 '''
 FILES 
 '''
-# ''' e.g: [ libs, data_dir, (from_file, $INSTDIR/to_dir) ] '''
+# ''' e.g: [ 'libs', 'data_dir', ('from_file', '$INSTDIR/to_dir') ] '''
 FILE_CONFIGS: list = []
+# ''' e.g: [ 'pkgs/PySide/examples',  'data_dir/ignoredfile' ] '''
+EXCLUDE_CONFIGS: list = []
 # ''' e.g: pynsist_pkgs '''
 ASSETS_PATH: str = ''
```

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_windows.py` & `bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_windows.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
 [Include]
 pypi_wheels={pypi_wheels}
 extra_wheel_sources={extra_wheel_sources}
 local_wheels={local_wheels}     
 packages={packages}  
 files={files}
+exclude={exclude}
 
 [Build]
 installer_name={installer_name}
 nsi_template={template}
 
 """
 try:
@@ -100,14 +101,15 @@
     SKIP_PYPI_PACKAGES: list = field(default_factory=list)
     UNWANTED_PACKAGES: list = field(default_factory=list)
 
     # '''
     # FILES
     # '''
     FILE_CONFIGS: list = field(default_factory=list)
+    EXCLUDE_CONFIGS: list = field(default_factory=list)
     ASSETS_PATH: str = ''
 
     @staticmethod
     def verify(configs: dict):
         variable_names = [fld.name for fld in fields(BibiinstallConfigs)]
         unsetting_variables = []
         for variable in variable_names:
@@ -476,30 +478,43 @@
         package_dist_info,
         entrypoint,
         package,
         unwanted_packages,
         skip_pypi_packages,
         icon_file,
         license_file,
+        asset_path,
         pynsist_config_file,
+        files,
+        excludes,
         encoding="latin1",
         suffix=None,
         nsi_template_path=None,
         local_wheel_path=None,
         is_wheel_first=False
 ):
     '''
 
     # fill extra_wheel_sources, local_wheels
     # SEE: https://pynsist.readthedocs.io/en/latest/
 
     '''
-    files = []
+    if files is None:
+        files = []
     wanted_rqmts_freeze, rqmts_wheel, rqmts_editable = separate_wheels_and_packages(python, unwanted_packages)
     skip_pypi_wheels = [package_name] + skip_pypi_packages
+
+    if asset_path is not None:
+        logger.debug(f'COPY {asset_path} into {pynsist_pkgs_dir}')
+        if len(str(asset_path).strip()) > 1 and Path(str(asset_path)).exists():
+            if Path(str(asset_path)).is_file():
+                shutil.copy2(Path(str(asset_path)), pynsist_pkgs_dir)
+            if Path(str(asset_path)).is_dir():
+                shutil.copytree(Path(str(asset_path)), pynsist_pkgs_dir, dirs_exist_ok=True)
+
     logger.info(f'is_wheel_first={is_wheel_first}')
     if not is_wheel_first:
         wheels_pypi_download = []
         packages = []
         extra_wheel_sources = []
 
         '''"import sysconfig; print(sysconfig.get_path('purelib'))"'''
@@ -531,14 +546,16 @@
 
     if not suffix:
         suffix = ""
 
     installer_exe = installer_name.format(package_name, bitness, suffix)
     changed_icon_exe = change_exe_icon(work_dir, package_name, icon_file)
     files.append(str(changed_icon_exe))
+    if excludes is None:
+        excludes = []
 
     pynsist_cfg_payload = PYNSIST_CFG_TEMPLATE.format(
         name=package_name,
         version=package_version,
         entrypoint=entrypoint,
         icon_file=icon_file,
         license_file=license_file,
@@ -548,15 +565,16 @@
         pypi_wheels="\n    ".join(wheels_pypi_download),
         extra_wheel_sources="\n    ".join(extra_wheel_sources),
         local_wheels="\n    ".join(local_wheels),
         packages="\n    ".join(packages),
         installer_name=installer_exe,
         template=nsi_template_path,
         package_dist_info=str(package_dist_info),
-        files="\n    ".join(files)
+        files="\n    ".join(files),
+        exclude="\n    ".join(excludes)
     )
 
     logger.info(f"pynsist_cfg_payload:\n{pynsist_cfg_payload}")
     with open(pynsist_config_file, "wt", encoding=encoding) as f:
         f.write(pynsist_cfg_payload)
     logger.info(f"Wrote pynsist configuration file [{pynsist_config_file}]")
     logger.info("Contents:")
@@ -685,14 +703,17 @@
 
 def run_installer(python_version,
                   bitness,
                   entrypoint,
                   package,
                   icon_path,
                   license_path,
+                  files=None,
+                  excludes=None,
+                  asset_path=None,
                   pynsist_version=2.8,
                   project_root=None,
                   extra_requirements_txt_path=None,
                   extra_packages=None,
                   editable_packages=None,
                   unwanted_packages=None,
                   skip_pypi_packages=None,
@@ -840,15 +861,17 @@
         installer_exe = create_pynsist_cfg(
             work_dir, pynsist_pkgs_dir, env_python, python_version_embed, bitness,
             package_name, package_version, package_author, package_dist_info,
             entrypoint=entrypoint,
             package=package,
             unwanted_packages=unwanted_packages,
             skip_pypi_packages=skip_pypi_packages,
-            icon_file=icon_path, license_file=license_path, pynsist_config_file=pynsist_cfg,
+            icon_file=icon_path, license_file=license_path,
+            pynsist_config_file=pynsist_cfg,
+            files=files, excludes=excludes, asset_path=asset_path,
             suffix=suffix, nsi_template_path=nsi_template_path,
             local_wheel_path=local_wheel_path,
             is_wheel_first=is_wheel_first)
 
         logger.info("Extracting nsis.")
         prepare_nsis_plugins(work_dir)
 
@@ -1009,15 +1032,15 @@
     python_version = flags.parameters.get('python_version') or configs.PYTHON_VERSION
     bitness = flags.parameters.get('bitness') or configs.BITNESS
     entrypoint = flags.parameters.get('entrypoint') or configs.ENTRYPOINT
     package = flags.parameters.get('package') or configs.PACKAGE_NAME
 
     pynsist_version = flags.parameters.get('pynsist_version')
     suffix = flags.parameters.get('suffix')
-    pypi_server = flags.parameters.get('pypi_server')
+    # pypi_server = flags.parameters.get('pypi_server')
     is_wheel_first = strtobool(flags.parameters.get('is_wheel_first', False))
 
     icon_path = get_absolute_path(project_root,
                                   flags.parameters.get('icon_path') or configs.ICON_PATH)
     if not Path(icon_path).exists():
         sys.exit(f"NOT Exist icon_path = [{icon_path}]")
 
@@ -1070,17 +1093,19 @@
 
     run_installer(
         python_version=python_version,
         bitness=bitness,
         entrypoint=entrypoint,
         package=package,
         pynsist_version=pynsist_version,
-
         icon_path=icon_path,
         license_path=license_path,
+        files=configs.FILE_CONFIGS,
+        excludes=configs.EXCLUDE_CONFIGS,
+        asset_path=configs.ASSETS_PATH,
         project_root=project_root,
         extra_requirements_txt_path=extra_requirements_txt_path,
         extra_packages=extra_packages,
         editable_packages=editable_packages,
         skip_pypi_packages=skip_pypi_packages,
         unwanted_packages=unwanted_packages,
         conda_path=conda_path,
```

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/bibiinstaller_windows.yaml` & `bibiinstaller-0.1.3/src/bibiinstaller/bibiinstaller_windows.yaml`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/application.nsi` & `bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/application.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/bibiinstaller.nsi` & `bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/bibiinstaller.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/spyder.nsi` & `bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/spyder.nsi`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller/nsi_templates/test_nsi_templates.py` & `bibiinstaller-0.1.3/src/bibiinstaller/nsi_templates/test_nsi_templates.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller.egg-info/PKG-INFO` & `bibiinstaller-0.1.3/src/bibiinstaller.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibiinstaller
-Version: 0.1.2
+Version: 0.1.3
 Summary: Bibi Installer using pynsist for Windows
 Home-page: https://github.com/bibiparrot/bibiinstaller
 Author: Chunqi Shi
 Author-email: Chunqi SHI <chunqishi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/bibiparrot/bibiinstaller
 Project-URL: Issues, https://github.com/bibiparrot/bibiinstaller/issues
```

### Comparing `bibiinstaller-0.1.2/src/bibiinstaller.egg-info/SOURCES.txt` & `bibiinstaller-0.1.3/src/bibiinstaller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/tests/learn_env_path.py` & `bibiinstaller-0.1.3/tests/learn_env_path.py`

 * *Files identical despite different names*

### Comparing `bibiinstaller-0.1.2/tests/learn_pypi_yarg.py` & `bibiinstaller-0.1.3/tests/learn_pypi_yarg.py`

 * *Files identical despite different names*

