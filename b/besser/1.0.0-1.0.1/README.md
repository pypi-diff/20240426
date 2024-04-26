# Comparing `tmp/besser-1.0.0.tar.gz` & `tmp/besser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser-1.0.0.tar", last modified: Mon Mar 11 16:18:06 2024, max compression
+gzip compressed data, was "besser-1.0.1.tar", last modified: Fri Apr 26 09:30:14 2024, max compression
```

## Comparing `besser-1.0.0.tar` & `besser-1.0.1.tar`

### file list

```diff
@@ -1,91 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.265621 besser-1.0.0/
--rw-rw-rw-   0        0        0     3574 2024-03-11 16:18:06.265621 besser-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2666 2024-03-07 08:40:30.000000 besser-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.201224 besser-1.0.0/besser/
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.207224 besser-1.0.0/besser/BUML/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.0.0/besser/BUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.209327 besser-1.0.0/besser/BUML/metamodel/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.0/besser/BUML/metamodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.210334 besser-1.0.0/besser/BUML/metamodel/gui/
--rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.0.0/besser/BUML/metamodel/gui/__init__.py
--rw-rw-rw-   0        0        0    25750 2024-03-08 08:46:02.000000 besser-1.0.0/besser/BUML/metamodel/gui/graphical_ui.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.212334 besser-1.0.0/besser/BUML/metamodel/object/
--rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.0.0/besser/BUML/metamodel/object/__init__.py
--rw-rw-rw-   0        0        0    10054 2024-03-07 16:34:50.000000 besser-1.0.0/besser/BUML/metamodel/object/object.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.215333 besser-1.0.0/besser/BUML/metamodel/ocl/
--rw-rw-rw-   0        0        0       20 2024-03-11 12:02:13.000000 besser-1.0.0/besser/BUML/metamodel/ocl/__init__.py
--rw-rw-rw-   0        0        0    10181 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/metamodel/ocl/rules.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.217332 besser-1.0.0/besser/BUML/metamodel/structural/
--rw-rw-rw-   0        0        0       25 2024-03-11 12:02:25.000000 besser-1.0.0/besser/BUML/metamodel/structural/__init__.py
--rw-rw-rw-   0        0        0    43682 2024-03-08 12:05:39.000000 besser-1.0.0/besser/BUML/metamodel/structural/structural.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.218333 besser-1.0.0/besser/BUML/notations/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.0/besser/BUML/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.222333 besser-1.0.0/besser/BUML/notations/objectPlantUML/
--rw-rw-rw-   0        0        0     5938 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/objectPlantUML/ODLexer.py
--rw-rw-rw-   0        0        0     4994 2024-03-07 16:34:33.000000 besser-1.0.0/besser/BUML/notations/objectPlantUML/ODListener.py
--rw-rw-rw-   0        0        0    25828 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/objectPlantUML/ODParser.py
--rw-rw-rw-   0        0        0        0 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/objectPlantUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.230387 besser-1.0.0/besser/BUML/notations/ocl/
--rw-rw-rw-   0        0        0     1468 2024-03-08 15:19:29.000000 besser-1.0.0/besser/BUML/notations/ocl/FactoryInstance.py
--rw-rw-rw-   0        0        0    22867 2024-03-07 08:29:25.000000 besser-1.0.0/besser/BUML/notations/ocl/OCLsLexer.py
--rw-rw-rw-   0        0        0    18453 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/ocl/OCLsListener.py
--rw-rw-rw-   0        0        0   200384 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/ocl/OCLsParser.py
--rw-rw-rw-   0        0        0     5640 2024-03-07 08:40:30.000000 besser-1.0.0/besser/BUML/notations/ocl/RootHandler.py
--rw-rw-rw-   0        0        0        0 2024-03-11 12:02:48.000000 besser-1.0.0/besser/BUML/notations/ocl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.236932 besser-1.0.0/besser/BUML/notations/structuralPlantUML/
--rw-rw-rw-   0        0        0    10331 2024-01-06 10:27:58.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
--rw-rw-rw-   0        0        0     6394 2024-01-06 10:27:59.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
--rw-rw-rw-   0        0        0    51575 2024-01-06 10:27:59.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
--rw-rw-rw-   0        0        0      203 2024-01-04 12:38:28.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/__init__.py
--rw-rw-rw-   0        0        0     9121 2024-01-15 16:13:03.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
--rw-rw-rw-   0        0        0     1432 2024-01-15 16:10:59.000000 besser-1.0.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
--rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.0.0/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.238932 besser-1.0.0/besser/generators/
--rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.0.0/besser/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.240600 besser-1.0.0/besser/generators/django/
--rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.0.0/besser/generators/django/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.0.0/besser/generators/django/django_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.243622 besser-1.0.0/besser/generators/django/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.0/besser/generators/django/templates/__init__.py
--rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.0.0/besser/generators/django/templates/django_fields.py.j2
--rw-rw-rw-   0        0        0     3213 2023-11-24 11:36:43.000000 besser-1.0.0/besser/generators/django/templates/django_template.py.j2
--rw-rw-rw-   0        0        0     1166 2024-03-08 16:36:51.000000 besser-1.0.0/besser/generators/generator_interface.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.245647 besser-1.0.0/besser/generators/python_classes/
--rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.0.0/besser/generators/python_classes/__init__.py
--rw-rw-rw-   0        0        0     1724 2024-01-15 16:13:59.000000 besser-1.0.0/besser/generators/python_classes/python_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.248641 besser-1.0.0/besser/generators/python_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.0/besser/generators/python_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.0.0/besser/generators/python_classes/templates/class_parameters.py.j2
--rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.0.0/besser/generators/python_classes/templates/python_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.250622 besser-1.0.0/besser/generators/rest_api/
--rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.0.0/besser/generators/rest_api/__init__.py
--rw-rw-rw-   0        0        0     2720 2024-03-07 13:36:29.000000 besser-1.0.0/besser/generators/rest_api/rest_api_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.252624 besser-1.0.0/besser/generators/rest_api/templates/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.0.0/besser/generators/rest_api/templates/__init__.py
--rw-rw-rw-   0        0        0     7985 2024-03-07 13:36:29.000000 besser-1.0.0/besser/generators/rest_api/templates/fast_api_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.254644 besser-1.0.0/besser/generators/sql/
--rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.0.0/besser/generators/sql/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.0.0/besser/generators/sql/sql_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.256622 besser-1.0.0/besser/generators/sql/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.0/besser/generators/sql/templates/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.0.0/besser/generators/sql/templates/sql_dialects.sql.j2
--rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.0.0/besser/generators/sql/templates/sql_template.sql.j2
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.258621 besser-1.0.0/besser/generators/sql_alchemy/
--rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.0.0/besser/generators/sql_alchemy/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.0.0/besser/generators/sql_alchemy/sql_alchemy_generator.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.260623 besser-1.0.0/besser/generators/sql_alchemy/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.0/besser/generators/sql_alchemy/templates/__init__.py
--rw-rw-rw-   0        0        0     3632 2024-01-11 16:19:34.000000 besser-1.0.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.263645 besser-1.0.0/besser/utilities/
--rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.0.0/besser/utilities/__init__.py
--rw-rw-rw-   0        0        0     2709 2024-03-08 14:36:21.000000 besser-1.0.0/besser/utilities/image_to_buml.py
--rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.0.0/besser/utilities/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-11 16:18:06.264621 besser-1.0.0/besser.egg-info/
--rw-rw-rw-   0        0        0     3574 2024-03-11 16:18:06.000000 besser-1.0.0/besser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2773 2024-03-11 16:18:06.000000 besser-1.0.0/besser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 16:18:06.000000 besser-1.0.0/besser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      230 2024-03-11 16:18:06.000000 besser-1.0.0/besser.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-11 16:18:06.000000 besser-1.0.0/besser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      242 2024-03-11 12:49:37.000000 besser-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0      659 2024-03-11 16:18:06.267634 besser-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.991981 besser-1.0.1/
+-rw-rw-rw-   0        0        0     3712 2024-04-26 09:30:14.990982 besser-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-04-19 11:55:41.000000 besser-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.902433 besser-1.0.1/besser/
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.908433 besser-1.0.1/besser/BUML/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.0.1/besser/BUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.909433 besser-1.0.1/besser/BUML/metamodel/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/metamodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.911433 besser-1.0.1/besser/BUML/metamodel/gui/
+-rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.0.1/besser/BUML/metamodel/gui/__init__.py
+-rw-rw-rw-   0        0        0    25750 2024-03-08 08:46:02.000000 besser-1.0.1/besser/BUML/metamodel/gui/graphical_ui.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.914433 besser-1.0.1/besser/BUML/metamodel/object/
+-rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.0.1/besser/BUML/metamodel/object/__init__.py
+-rw-rw-rw-   0        0        0    10058 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/metamodel/object/object.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.916456 besser-1.0.1/besser/BUML/metamodel/ocl/
+-rw-rw-rw-   0        0        0       20 2024-03-11 12:02:13.000000 besser-1.0.1/besser/BUML/metamodel/ocl/__init__.py
+-rw-rw-rw-   0        0        0    10785 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/metamodel/ocl/rules.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.919434 besser-1.0.1/besser/BUML/metamodel/structural/
+-rw-rw-rw-   0        0        0       25 2024-03-11 12:02:25.000000 besser-1.0.1/besser/BUML/metamodel/structural/__init__.py
+-rw-rw-rw-   0        0        0    43485 2024-04-19 11:55:28.000000 besser-1.0.1/besser/BUML/metamodel/structural/structural.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.921460 besser-1.0.1/besser/BUML/notations/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.926438 besser-1.0.1/besser/BUML/notations/objectPlantUML/
+-rw-rw-rw-   0        0        0     5938 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODLexer.py
+-rw-rw-rw-   0        0        0     4994 2024-03-07 16:34:33.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODListener.py
+-rw-rw-rw-   0        0        0    25828 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/ODParser.py
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:40:30.000000 besser-1.0.1/besser/BUML/notations/objectPlantUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.939492 besser-1.0.1/besser/BUML/notations/ocl/
+-rw-rw-rw-   0        0        0    23268 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLLexer.py
+-rw-rw-rw-   0        0        0    41633 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLListener.py
+-rw-rw-rw-   0        0        0   212929 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/BOCLParser.py
+-rw-rw-rw-   0        0        0     4732 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/FactoryInstance.py
+-rw-rw-rw-   0        0        0     1080 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/OCLWrapper.py
+-rw-rw-rw-   0        0        0    12723 2024-04-26 08:06:13.000000 besser-1.0.1/besser/BUML/notations/ocl/RootHandler.py
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.0.1/besser/BUML/notations/ocl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.945433 besser-1.0.1/besser/BUML/notations/structuralPlantUML/
+-rw-rw-rw-   0        0        0    10331 2024-01-06 10:27:58.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
+-rw-rw-rw-   0        0        0     6394 2024-01-06 10:27:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
+-rw-rw-rw-   0        0        0    51575 2024-01-06 10:27:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
+-rw-rw-rw-   0        0        0      203 2024-01-04 12:38:28.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/__init__.py
+-rw-rw-rw-   0        0        0     9121 2024-01-15 16:13:03.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
+-rw-rw-rw-   0        0        0     1432 2024-01-15 16:10:59.000000 besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.0.1/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.948449 besser-1.0.1/besser/generators/
+-rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.0.1/besser/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.950435 besser-1.0.1/besser/generators/django/
+-rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/django/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.0.1/besser/generators/django/django_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.953466 besser-1.0.1/besser/generators/django/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/django/templates/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/django/templates/django_fields.py.j2
+-rw-rw-rw-   0        0        0     3213 2023-11-24 11:36:43.000000 besser-1.0.1/besser/generators/django/templates/django_template.py.j2
+-rw-rw-rw-   0        0        0     1166 2024-03-08 16:36:51.000000 besser-1.0.1/besser/generators/generator_interface.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.956461 besser-1.0.1/besser/generators/python_classes/
+-rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.0.1/besser/generators/python_classes/__init__.py
+-rw-rw-rw-   0        0        0     1724 2024-01-15 16:13:59.000000 besser-1.0.1/besser/generators/python_classes/python_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.959452 besser-1.0.1/besser/generators/python_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/python_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.0.1/besser/generators/python_classes/templates/class_parameters.py.j2
+-rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.0.1/besser/generators/python_classes/templates/python_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.962434 besser-1.0.1/besser/generators/rest_api/
+-rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.0.1/besser/generators/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     2720 2024-03-07 13:36:29.000000 besser-1.0.1/besser/generators/rest_api/rest_api_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.964440 besser-1.0.1/besser/generators/rest_api/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.0.1/besser/generators/rest_api/templates/__init__.py
+-rw-rw-rw-   0        0        0     7985 2024-03-07 13:36:29.000000 besser-1.0.1/besser/generators/rest_api/templates/fast_api_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.967455 besser-1.0.1/besser/generators/sql/
+-rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.0.1/besser/generators/sql/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.0.1/besser/generators/sql/sql_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.970451 besser-1.0.1/besser/generators/sql/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/sql/templates/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/sql/templates/sql_dialects.sql.j2
+-rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.0.1/besser/generators/sql/templates/sql_template.sql.j2
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.972453 besser-1.0.1/besser/generators/sql_alchemy/
+-rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.0.1/besser/generators/sql_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.0.1/besser/generators/sql_alchemy/sql_alchemy_generator.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.974475 besser-1.0.1/besser/generators/sql_alchemy/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.0.1/besser/generators/sql_alchemy/templates/__init__.py
+-rw-rw-rw-   0        0        0     3632 2024-01-11 16:19:34.000000 besser-1.0.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.977450 besser-1.0.1/besser/utilities/
+-rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.0.1/besser/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2709 2024-03-08 14:36:21.000000 besser-1.0.1/besser/utilities/image_to_buml.py
+-rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.0.1/besser/utilities/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.989983 besser-1.0.1/besser.egg-info/
+-rw-rw-rw-   0        0        0     3712 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3129 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      230 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-26 09:30:14.000000 besser-1.0.1/besser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      242 2024-03-11 12:49:37.000000 besser-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0      659 2024-04-26 09:30:14.992968 besser-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.978451 besser-1.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.980960 besser-1.0.1/tests/gui/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/gui/__init__.py
+-rw-rw-rw-   0        0        0     2480 2024-03-11 13:08:13.000000 besser-1.0.1/tests/gui/gui_model.py
+-rw-rw-rw-   0        0        0     5271 2024-03-08 09:35:33.000000 besser-1.0.1/tests/gui/test_gui.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.981967 besser-1.0.1/tests/notations/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.984971 besser-1.0.1/tests/object/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/object/__init__.py
+-rw-rw-rw-   0        0        0    10547 2024-04-26 08:06:13.000000 besser-1.0.1/tests/object/library_object.py
+-rw-rw-rw-   0        0        0     3879 2024-03-07 16:31:15.000000 besser-1.0.1/tests/object/test_object_mm.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.986974 besser-1.0.1/tests/ocl/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/ocl/__init__.py
+-rw-rw-rw-   0        0        0     7566 2024-04-26 08:06:13.000000 besser-1.0.1/tests/ocl/test_ocl_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-26 09:30:14.988985 besser-1.0.1/tests/structural/
+-rw-rw-rw-   0        0        0        0 2024-04-26 08:26:18.000000 besser-1.0.1/tests/structural/__init__.py
+-rw-rw-rw-   0        0        0    10194 2024-01-15 16:18:42.000000 besser-1.0.1/tests/structural/test_structural.py
```

### Comparing `besser-1.0.0/PKG-INFO` & `besser-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.0.0
+Version: 1.0.1
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
@@ -54,14 +54,17 @@
     $ python -m build
     $ pip install dist/besser-*.*.*-py3-none-any.whl
 
 You can check the installation of the *besser* package.
 
     $ pip list
 
+## Examples
+If you want to try examples, check out the [BESSER-examples](https://github.com/BESSER-PEARL/BESSER-examples) repository!
+
 ## Contributing
 
 We encourage contributions from the community and any comment is welcome!
 
 If you are interested in contributing to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Code of Conduct
```

### Comparing `besser-1.0.0/README.md` & `besser-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     $ python -m build
     $ pip install dist/besser-*.*.*-py3-none-any.whl
 
 You can check the installation of the *besser* package.
 
     $ pip list
 
+## Examples
+If you want to try examples, check out the [BESSER-examples](https://github.com/BESSER-PEARL/BESSER-examples) repository!
+
 ## Contributing
 
 We encourage contributions from the community and any comment is welcome!
 
 If you are interested in contributing to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Code of Conduct
```

### Comparing `besser-1.0.0/besser/BUML/metamodel/gui/graphical_ui.py` & `besser-1.0.1/besser/BUML/metamodel/gui/graphical_ui.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/metamodel/object/object.py` & `besser-1.0.1/besser/BUML/metamodel/object/object.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.__value = value
 
     @property
     def attribute(self) -> Property:
         """Property: Get the attribute."""
         return self.__attribute
 
-    @value.setter
+    @attribute.setter
     def attribute(self, attribute: Property):
         """Property: Set the attribute."""
         self.__attribute = attribute
 
     def __repr__(self) -> str:
         return f'Attribute Link({self.value}, {self.__attribute})'
```

### Comparing `besser-1.0.0/besser/BUML/metamodel/ocl/rules.py` & `besser-1.0.1/besser/BUML/metamodel/ocl/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,32 @@
 from typing import Any
 from besser.BUML.metamodel.structural import Class, NamedElement, TypedElement, Type, PrimitiveDataType, Property, Constraint
 
 
 class OCLExpression(TypedElement):
     def __init__(self, name: str, type: Type):
         super().__init__(name, type)
+        self._source = None
+        self._referredOperation = None
+
+    @property
+    def source(self) ->Any:
+        return self._source
+    @source.setter
+    def source(self, source)->Any:
+        self._source = source
+    @property
+    def referredOperation(self)->Any:
+        return self._referredOperation
+
+    @referredOperation.setter
+    def referredOperation(self, op):
+        self._referredOperation = op
+
+
 
     def __str__(self) -> str:
         pass
 
 
 # A literal value part of an OCL expression
 class LiteralExpression(OCLExpression):
@@ -79,15 +97,16 @@
     @property
     def arguments(self) -> list[OCLExpression]:
         return self.__arguments
 
     @arguments.setter
     def arguments(self, arguments: list[OCLExpression]):
         self.__arguments = arguments
-
+    def add(self,item):
+        self.arguments.append(item)
     def __str__(self) -> str:
         toRet= ""
         for arg in self.arguments:
             # print(type(arg))
             toRet = toRet+"  \n "+ str(arg)
         return toRet
         # return f'{self.arguments[0]} {self.operation} {self.arguments[1]}'
@@ -99,39 +118,39 @@
 
 
 class IfExp(OCLExpression):
     def __init__(self, name: str, type: Type,ifcond = None, elseExp = None, thenExp = None,):
         # self.ifOwner = null
         super().__init__(name, type)
 
-        self.ifCondition = ifcond
-        self.else_expression = elseExp
-        self.then_expression = thenExp
+        self._ifCondition = None
+        self._else_expression = None
+        self._then_expression = None
 
     @property
-    def get_if_Condition (self):
-        return self.ifCondition
+    def ifCondition (self) -> OCLExpression:
+        return self._ifCondition
 
     @property
-    def get_else_condition(self):
-        return self.else_expression
+    def elseCondition(self) -> OCLExpression:
+        return self._else_expression
     @property
-    def get_then_expression(self):
-        return self.then_expression
+    def thenExpression(self) ->OCLExpression:
+        return self._then_expression
 
-    @property
-    def set_if_Condition (self,if_cond):
-        self.ifCondition = if_cond
+    @ifCondition.setter
+    def ifCondition (self,if_cond):
+        self._ifCondition = if_cond
 
-    @property
-    def set_else_condition(self,else_cond):
-        self.else_expression = else_cond
-    @property
-    def set_then_expression(self, then_expression):
-        self.then_expression = then_expression
+    @elseCondition.setter
+    def elseCondition(self,else_cond):
+        self._else_expression = else_cond
+    @thenExpression.setter
+    def thenExpression(self, then_expression):
+        self._then_expression = then_expression
 class VariableExp(OCLExpression):
     def __init__(self,name: str, type: Type):
         super().__init__(name, type)
         self.name = name
         self.variable = Variable(name,type)
 
     def set_refferred_variable (self,val):
@@ -148,24 +167,24 @@
         super().__init__(name, type)
 
     def set_value(self, val):
         self.representatedParameter = Parameter(val)
     def get_value(self):
         return self.representatedParameter.get_value()
 
-class Property:
-    def __init__(self):
-        self.referringExp = []
-        self.val = None
+# class Property:
+#     def __init__(self):
+#         self.referringExp = []
+#         self.val = None
 
 class TypeExp(OCLExpression):
         def __init__(self,name: str, type: Type):
             super().__init__(name, type)
 
-            self.referedType = Classifier()
+            self.referedType = Classifier(name)
 class Parameter:
     def __init__(self,val):
         self.value =val
 
     def get_value(self):
         return self.value
 
@@ -184,14 +203,16 @@
         super().__init__(name, type=PrimitiveDataType(name="float"), value=value)
 
     def __repr__(self):
         return f'RealLiteralExpression({self.value})'
 
 
 class Classifier:
+    def __init__(self, name= None):
+        self.name = name
     pass
 class CallExp(OCLExpression):
     pass
 class FeatureCallExp(CallExp):
     pass
 class LiteralExp(OCLExpression):
     pass
@@ -259,21 +280,21 @@
 class LetExp(OCLExpression):
     def __init__(self, name: str, type: Type):
         super().__init__(name, type)
         self.OCLExpression = None
         self.variable = None
 class BooleanLiteralExpression(LiteralExpression):
     def __init__(self, name: str, value: bool):
-        super().__init__(name, type=PrimitiveDataType(name="Boolean"), value=value)
+        super().__init__(name, type=PrimitiveDataType(name="bool"), value=value)
 
     def __repr__(self):
         return f'BooleanLiteralExpression({self.value})'
 class StringLiteralExpression(LiteralExpression):
     def __init__(self, name: str, value: str):
-        super().__init__(name, type=PrimitiveDataType(name="String"), value=value)
+        super().__init__(name, type=PrimitiveDataType(name="str"), value=value)
 
     def __repr__(self):
         return f'StringLiteralExpression({self.value})'
 
 class InfixOperator:
     def __init__(self,operator):
         self.operator = operator
@@ -313,15 +334,15 @@
         self.kind = type
         self.collectionItems = []
     def __str__(self):
         toRet= str(self.kind) +": "
         for item in self.collectionItems:
             toRet = toRet + str(item)
         return toRet
-    def add_to_collection_items(self,item):
+    def add(self, item):
         self.collectionItems.append(item)
 
 class CollectionLiteralPart(TypedElement):
     def __init__(self, name):
         super().__init__(name,type = "NP")
```

### Comparing `besser-1.0.0/besser/BUML/metamodel/structural/structural.py` & `besser-1.0.1/besser/BUML/metamodel/structural/structural.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,27 +82,25 @@
     def __init__(self, name: str):
         super().__init__(name)
 
     def __repr__(self):
         return f"DataType({self.name})"
     
 class PrimitiveDataType(DataType):
-    """Class representing an enumeration literal.
+    """Class representing a primitive data type.
 
-    This class is a subclass of NamedElement and is used to represent individual
-    literals within an enumeration.
+    This class is a subclass of DataType and is used to represent primitive data types
+    with a specified name.
 
     Args:
-        name (str): the name of the enumeration literal.
-        owner (DataType): the owner data type of the enumeration literal.
+        name (str): the name of the primitive data type.
 
     Attributes:
-        name (str): Inherited from NamedElement, represents the name of the enumeration literal.
-        owner (DataType): Represents the owner data type of the enumeration literal.
-    """    
+        name (str): Inherited from NamedElement, represents the name of the primitive data type.
+    """
 
     def __init__(self, name: str):
         super().__init__(name)
 
     @NamedElement.name.setter
     def name(self, name: str):
         """
@@ -116,28 +114,28 @@
             raise ValueError("Invalid primitive data type")
         super(PrimitiveDataType, PrimitiveDataType).name.fset(self, name)
     
     def __repr__(self):
         return f"PrimitiveDataType({self.name})"
     
 class EnumerationLiteral(NamedElement):
-    """Class representing a primitive data type.
+    """Class representing an enumeration literal.
 
-    This class is a subclass of DataType and is used to represent primitive data types
-    with a specified name.
+    This class is a subclass of NamedElement and is used to represent individual
+    literals within an enumeration.
 
     Args:
-        name (str): the name of the primitive data type.
-        owner (DataType): the owner data type (Enumeration) of the enumeration literal.
+        name (str): the name of the enumeration literal.
+        owner (DataType): the owner data type of the enumeration literal.
 
     Attributes:
         name (str): Inherited from NamedElement, represents the name of the enumeration literal.
-        owner (DataType): Represents the owner data type (Enumeration) of the enumeration literal.
+        owner (DataType): Represents the owner data type of the enumeration literal.
     """
-    
+
     def __init__(self, name: str, owner: DataType):
         super().__init__(name)
         self.owner: DataType = owner
     
     @property
     def owner(self) -> DataType:
         """Datatype: Get the owner."""
```

### Comparing `besser-1.0.0/besser/BUML/notations/objectPlantUML/ODLexer.py` & `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/objectPlantUML/ODListener.py` & `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/objectPlantUML/ODParser.py` & `besser-1.0.1/besser/BUML/notations/objectPlantUML/ODParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/ocl/OCLsLexer.py` & `besser-1.0.1/besser/BUML/notations/ocl/BOCLLexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,349 +1,355 @@
-# Generated from OCLs.g4 by ANTLR 4.13.1
+# Generated from BOCL.g4 by ANTLR 4.13.1
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
     from typing import TextIO
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     return [
-        4,0,82,660,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
+        4,0,83,672,6,-1,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,
         2,6,7,6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,
         13,7,13,2,14,7,14,2,15,7,15,2,16,7,16,2,17,7,17,2,18,7,18,2,19,7,
         19,2,20,7,20,2,21,7,21,2,22,7,22,2,23,7,23,2,24,7,24,2,25,7,25,2,
         26,7,26,2,27,7,27,2,28,7,28,2,29,7,29,2,30,7,30,2,31,7,31,2,32,7,
         32,2,33,7,33,2,34,7,34,2,35,7,35,2,36,7,36,2,37,7,37,2,38,7,38,2,
         39,7,39,2,40,7,40,2,41,7,41,2,42,7,42,2,43,7,43,2,44,7,44,2,45,7,
         45,2,46,7,46,2,47,7,47,2,48,7,48,2,49,7,49,2,50,7,50,2,51,7,51,2,
         52,7,52,2,53,7,53,2,54,7,54,2,55,7,55,2,56,7,56,2,57,7,57,2,58,7,
         58,2,59,7,59,2,60,7,60,2,61,7,61,2,62,7,62,2,63,7,63,2,64,7,64,2,
         65,7,65,2,66,7,66,2,67,7,67,2,68,7,68,2,69,7,69,2,70,7,70,2,71,7,
         71,2,72,7,72,2,73,7,73,2,74,7,74,2,75,7,75,2,76,7,76,2,77,7,77,2,
-        78,7,78,2,79,7,79,2,80,7,80,2,81,7,81,1,0,1,0,1,0,1,0,1,0,1,0,1,
-        0,1,0,1,1,1,1,1,1,1,1,1,2,1,2,1,2,1,2,1,3,1,3,1,3,1,3,1,3,1,4,1,
-        4,1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,6,1,6,1,6,1,6,1,6,1,
-        6,1,6,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,8,1,8,1,8,1,8,1,8,1,8,1,8,1,
-        8,1,9,1,9,1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,
-        1,10,1,11,4,11,237,8,11,11,11,12,11,238,1,11,1,11,1,12,1,12,1,12,
-        1,13,1,13,1,13,1,14,1,14,1,15,1,15,1,16,1,16,1,17,1,17,1,18,1,18,
-        1,19,1,19,1,20,1,20,1,21,1,21,1,22,1,22,1,23,1,23,1,24,1,24,1,24,
-        1,24,1,24,1,24,1,24,1,24,1,25,1,25,1,25,1,25,1,25,1,25,1,25,1,25,
-        1,26,1,26,1,26,1,26,1,26,1,27,1,27,1,27,1,27,1,27,1,27,1,27,1,28,
-        1,28,1,28,1,29,1,29,1,29,1,29,1,29,1,30,1,30,1,30,1,30,1,30,1,31,
-        1,31,1,31,1,31,1,31,1,31,1,32,1,32,1,32,1,32,1,33,1,33,1,33,1,34,
-        1,34,1,34,1,34,1,35,1,35,1,35,1,36,1,36,1,37,1,37,1,37,1,38,1,38,
-        1,39,1,39,1,39,1,40,1,40,1,41,1,41,1,41,1,41,1,41,1,41,3,41,348,
-        8,41,1,42,1,42,1,42,1,42,1,43,1,43,1,43,1,43,1,43,1,43,1,43,1,43,
-        1,43,1,44,1,44,1,44,1,44,1,44,1,44,1,44,1,44,1,44,1,44,1,44,1,45,
-        1,45,1,46,1,46,1,47,1,47,1,48,1,48,1,49,1,49,1,49,1,49,1,50,1,50,
-        1,50,1,50,1,50,1,50,1,50,1,50,1,51,1,51,1,51,1,51,1,51,1,51,1,51,
-        1,51,1,51,1,51,1,52,1,52,1,52,1,52,1,52,1,52,1,52,1,52,1,52,1,52,
-        1,52,1,52,1,53,1,53,1,53,1,53,1,53,1,53,1,53,1,53,1,53,1,53,1,53,
-        1,53,1,54,1,54,1,54,1,54,1,54,1,54,1,54,1,54,1,54,1,54,1,54,1,54,
-        1,54,1,55,1,55,1,55,1,55,1,55,1,55,1,55,1,55,1,56,1,56,1,56,1,56,
-        1,57,1,57,1,57,1,57,1,57,1,58,1,58,1,58,1,58,1,58,1,58,1,58,1,58,
-        1,58,1,59,1,59,1,59,1,59,1,59,1,59,1,59,1,59,1,59,1,60,1,60,1,60,
-        1,60,1,60,1,60,1,60,1,60,1,60,1,60,1,60,1,60,1,61,1,61,1,61,1,61,
-        1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,62,1,62,1,62,
-        1,62,1,62,1,62,1,62,1,62,1,63,1,63,1,63,1,63,1,63,1,64,1,64,1,64,
-        1,64,1,64,1,64,1,64,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,
-        1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,66,1,66,
-        1,66,1,66,1,66,1,66,1,67,1,67,1,67,1,67,1,67,1,67,1,67,1,68,1,68,
+        78,7,78,2,79,7,79,2,80,7,80,2,81,7,81,2,82,7,82,1,0,1,0,1,1,1,1,
+        1,1,1,1,1,1,1,1,1,1,1,1,1,2,1,2,1,2,1,2,1,3,1,3,1,3,1,3,1,4,1,4,
+        1,4,1,4,1,4,1,5,1,5,1,5,1,5,1,5,1,6,1,6,1,6,1,6,1,6,1,6,1,6,1,7,
+        1,7,1,7,1,7,1,7,1,7,1,7,1,8,1,8,1,8,1,8,1,8,1,8,1,8,1,9,1,9,1,9,
+        1,9,1,9,1,9,1,9,1,9,1,10,1,10,1,10,1,10,1,10,1,10,1,10,1,11,1,11,
+        1,11,1,11,1,11,1,11,1,11,1,11,1,12,4,12,241,8,12,11,12,12,12,242,
+        1,12,1,12,1,13,1,13,1,13,1,14,1,14,1,14,1,15,1,15,1,16,1,16,1,17,
+        1,17,1,18,1,18,1,19,1,19,1,20,1,20,1,21,1,21,1,22,1,22,1,23,1,23,
+        1,24,1,24,1,25,1,25,1,25,1,25,1,25,1,25,1,25,1,25,1,26,1,26,1,26,
+        1,26,1,26,1,26,1,26,1,26,1,27,1,27,1,27,1,27,1,27,1,28,1,28,1,28,
+        1,28,1,28,1,28,1,28,1,29,1,29,1,29,1,30,1,30,1,30,1,30,1,30,1,31,
+        1,31,1,31,1,31,1,31,1,32,1,32,1,32,1,32,1,32,1,32,1,33,1,33,1,33,
+        1,33,1,34,1,34,1,34,1,35,1,35,1,35,1,35,1,36,1,36,1,36,1,37,1,37,
+        1,38,1,38,1,38,1,39,1,39,1,40,1,40,1,40,1,41,1,41,1,42,1,42,1,42,
+        1,42,1,42,1,42,3,42,352,8,42,1,43,1,43,1,43,1,43,1,44,1,44,1,44,
+        1,44,1,44,1,44,1,44,1,44,1,44,1,45,1,45,1,45,1,45,1,45,1,45,1,45,
+        1,45,1,45,1,45,1,45,1,46,1,46,1,47,1,47,1,48,1,48,1,49,1,49,1,50,
+        1,50,1,50,1,50,1,51,1,51,1,51,1,51,1,51,1,51,1,51,1,51,1,52,1,52,
+        1,52,1,52,1,52,1,52,1,52,1,52,1,52,1,52,1,53,1,53,1,53,1,53,1,53,
+        1,53,1,53,1,53,1,53,1,53,1,53,1,53,1,54,1,54,1,54,1,54,1,54,1,54,
+        1,54,1,54,1,54,1,54,1,54,1,54,1,55,1,55,1,55,1,55,1,55,1,55,1,55,
+        1,55,1,55,1,55,1,55,1,55,1,55,1,56,1,56,1,56,1,56,1,56,1,56,1,56,
+        1,56,1,57,1,57,1,57,1,57,1,58,1,58,1,58,1,58,1,58,1,59,1,59,1,59,
+        1,59,1,59,1,59,1,59,1,59,1,59,1,60,1,60,1,60,1,60,1,60,1,60,1,60,
+        1,60,1,60,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,1,61,
+        1,61,1,62,1,62,1,62,1,62,1,62,1,62,1,62,1,62,1,62,1,62,1,62,1,62,
+        1,62,1,62,1,63,1,63,1,63,1,63,1,63,1,63,1,63,1,63,1,64,1,64,1,64,
+        1,64,1,64,1,65,1,65,1,65,1,65,1,65,1,65,1,65,1,66,1,66,1,66,1,66,
+        1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,1,66,
+        1,66,1,66,1,66,1,67,1,67,1,67,1,67,1,67,1,67,1,68,1,68,1,68,1,68,
         1,68,1,68,1,68,1,69,1,69,1,69,1,69,1,69,1,70,1,70,1,70,1,70,1,70,
-        1,70,1,71,1,71,1,71,1,71,1,71,1,72,1,72,1,72,1,72,1,73,1,73,1,73,
-        1,74,1,74,1,74,1,74,1,74,3,74,588,8,74,1,75,1,75,1,75,1,75,1,76,
-        1,76,5,76,596,8,76,10,76,12,76,599,9,76,1,77,4,77,602,8,77,11,77,
-        12,77,603,1,77,1,77,4,77,608,8,77,11,77,12,77,609,3,77,612,8,77,
-        1,78,1,78,1,78,1,78,5,78,618,8,78,10,78,12,78,621,9,78,1,78,1,78,
-        1,79,1,79,1,79,1,79,1,79,1,79,1,79,1,79,1,79,3,79,634,8,79,1,80,
-        1,80,1,80,1,80,5,80,640,8,80,10,80,12,80,643,9,80,1,80,1,80,1,80,
-        1,80,1,80,1,81,1,81,1,81,1,81,5,81,654,8,81,10,81,12,81,657,9,81,
-        1,81,1,81,1,641,0,82,1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,17,9,19,
-        10,21,11,23,12,25,13,27,14,29,15,31,16,33,17,35,18,37,19,39,20,41,
-        21,43,22,45,23,47,24,49,25,51,26,53,27,55,28,57,29,59,30,61,31,63,
-        32,65,33,67,34,69,35,71,36,73,37,75,38,77,39,79,40,81,41,83,42,85,
-        43,87,44,89,45,91,46,93,47,95,48,97,49,99,50,101,51,103,52,105,53,
-        107,54,109,55,111,56,113,57,115,58,117,59,119,60,121,61,123,62,125,
-        63,127,64,129,65,131,66,133,67,135,68,137,69,139,70,141,71,143,72,
-        145,73,147,74,149,75,151,76,153,77,155,78,157,79,159,80,161,81,163,
-        82,1,0,6,3,0,9,10,13,13,32,32,3,0,65,90,95,95,97,122,4,0,48,57,65,
-        90,95,95,97,122,1,0,48,57,2,0,34,34,92,92,2,0,10,10,13,13,671,0,
-        1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,0,0,9,1,0,0,0,0,11,1,
-        0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,0,0,19,1,0,0,0,0,21,1,
-        0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,0,0,29,1,0,0,0,0,31,1,
-        0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,0,0,39,1,0,0,0,0,41,1,
-        0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,0,0,49,1,0,0,0,0,51,1,
-        0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,0,0,59,1,0,0,0,0,61,1,
-        0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,0,0,69,1,0,0,0,0,71,1,
-        0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,0,0,79,1,0,0,0,0,81,1,
-        0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,0,0,89,1,0,0,0,0,91,1,
-        0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,0,0,99,1,0,0,0,0,101,
-        1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,0,0,0,0,109,1,0,0,0,
-        0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,117,1,0,0,0,0,119,1,
-        0,0,0,0,121,1,0,0,0,0,123,1,0,0,0,0,125,1,0,0,0,0,127,1,0,0,0,0,
-        129,1,0,0,0,0,131,1,0,0,0,0,133,1,0,0,0,0,135,1,0,0,0,0,137,1,0,
-        0,0,0,139,1,0,0,0,0,141,1,0,0,0,0,143,1,0,0,0,0,145,1,0,0,0,0,147,
-        1,0,0,0,0,149,1,0,0,0,0,151,1,0,0,0,0,153,1,0,0,0,0,155,1,0,0,0,
-        0,157,1,0,0,0,0,159,1,0,0,0,0,161,1,0,0,0,0,163,1,0,0,0,1,165,1,
-        0,0,0,3,173,1,0,0,0,5,177,1,0,0,0,7,181,1,0,0,0,9,186,1,0,0,0,11,
-        191,1,0,0,0,13,198,1,0,0,0,15,205,1,0,0,0,17,212,1,0,0,0,19,220,
-        1,0,0,0,21,227,1,0,0,0,23,236,1,0,0,0,25,242,1,0,0,0,27,245,1,0,
-        0,0,29,248,1,0,0,0,31,250,1,0,0,0,33,252,1,0,0,0,35,254,1,0,0,0,
-        37,256,1,0,0,0,39,258,1,0,0,0,41,260,1,0,0,0,43,262,1,0,0,0,45,264,
-        1,0,0,0,47,266,1,0,0,0,49,268,1,0,0,0,51,276,1,0,0,0,53,284,1,0,
-        0,0,55,289,1,0,0,0,57,296,1,0,0,0,59,299,1,0,0,0,61,304,1,0,0,0,
-        63,309,1,0,0,0,65,315,1,0,0,0,67,319,1,0,0,0,69,322,1,0,0,0,71,326,
-        1,0,0,0,73,329,1,0,0,0,75,331,1,0,0,0,77,334,1,0,0,0,79,336,1,0,
-        0,0,81,339,1,0,0,0,83,347,1,0,0,0,85,349,1,0,0,0,87,353,1,0,0,0,
-        89,362,1,0,0,0,91,373,1,0,0,0,93,375,1,0,0,0,95,377,1,0,0,0,97,379,
-        1,0,0,0,99,381,1,0,0,0,101,385,1,0,0,0,103,393,1,0,0,0,105,403,1,
-        0,0,0,107,415,1,0,0,0,109,427,1,0,0,0,111,440,1,0,0,0,113,448,1,
-        0,0,0,115,452,1,0,0,0,117,457,1,0,0,0,119,466,1,0,0,0,121,475,1,
-        0,0,0,123,487,1,0,0,0,125,501,1,0,0,0,127,509,1,0,0,0,129,514,1,
-        0,0,0,131,521,1,0,0,0,133,541,1,0,0,0,135,547,1,0,0,0,137,554,1,
-        0,0,0,139,559,1,0,0,0,141,564,1,0,0,0,143,570,1,0,0,0,145,575,1,
-        0,0,0,147,579,1,0,0,0,149,587,1,0,0,0,151,589,1,0,0,0,153,593,1,
-        0,0,0,155,601,1,0,0,0,157,613,1,0,0,0,159,633,1,0,0,0,161,635,1,
-        0,0,0,163,649,1,0,0,0,165,166,5,99,0,0,166,167,5,111,0,0,167,168,
-        5,110,0,0,168,169,5,116,0,0,169,170,5,101,0,0,170,171,5,120,0,0,
-        171,172,5,116,0,0,172,2,1,0,0,0,173,174,5,105,0,0,174,175,5,110,
-        0,0,175,176,5,118,0,0,176,4,1,0,0,0,177,178,5,112,0,0,178,179,5,
-        114,0,0,179,180,5,101,0,0,180,6,1,0,0,0,181,182,5,112,0,0,182,183,
-        5,111,0,0,183,184,5,115,0,0,184,185,5,116,0,0,185,8,1,0,0,0,186,
-        187,5,115,0,0,187,188,5,101,0,0,188,189,5,108,0,0,189,190,5,102,
-        0,0,190,10,1,0,0,0,191,192,5,102,0,0,192,193,5,111,0,0,193,194,5,
-        114,0,0,194,195,5,65,0,0,195,196,5,108,0,0,196,197,5,108,0,0,197,
-        12,1,0,0,0,198,199,5,101,0,0,199,200,5,120,0,0,200,201,5,105,0,0,
-        201,202,5,115,0,0,202,203,5,116,0,0,203,204,5,115,0,0,204,14,1,0,
-        0,0,205,206,5,115,0,0,206,207,5,101,0,0,207,208,5,108,0,0,208,209,
-        5,101,0,0,209,210,5,99,0,0,210,211,5,116,0,0,211,16,1,0,0,0,212,
-        213,5,99,0,0,213,214,5,111,0,0,214,215,5,108,0,0,215,216,5,108,0,
-        0,216,217,5,101,0,0,217,218,5,99,0,0,218,219,5,116,0,0,219,18,1,
-        0,0,0,220,221,5,79,0,0,221,222,5,99,0,0,222,223,5,108,0,0,223,224,
-        5,65,0,0,224,225,5,110,0,0,225,226,5,121,0,0,226,20,1,0,0,0,227,
-        228,5,79,0,0,228,229,5,99,0,0,229,230,5,108,0,0,230,231,5,86,0,0,
-        231,232,5,111,0,0,232,233,5,105,0,0,233,234,5,100,0,0,234,22,1,0,
-        0,0,235,237,7,0,0,0,236,235,1,0,0,0,237,238,1,0,0,0,238,236,1,0,
-        0,0,238,239,1,0,0,0,239,240,1,0,0,0,240,241,6,11,0,0,241,24,1,0,
-        0,0,242,243,5,46,0,0,243,244,5,46,0,0,244,26,1,0,0,0,245,246,5,58,
-        0,0,246,247,5,58,0,0,247,28,1,0,0,0,248,249,5,40,0,0,249,30,1,0,
-        0,0,250,251,5,41,0,0,251,32,1,0,0,0,252,253,5,123,0,0,253,34,1,0,
-        0,0,254,255,5,125,0,0,255,36,1,0,0,0,256,257,5,59,0,0,257,38,1,0,
-        0,0,258,259,5,58,0,0,259,40,1,0,0,0,260,261,5,44,0,0,261,42,1,0,
-        0,0,262,263,5,46,0,0,263,44,1,0,0,0,264,265,5,61,0,0,265,46,1,0,
-        0,0,266,267,5,39,0,0,267,48,1,0,0,0,268,269,5,66,0,0,269,270,5,111,
-        0,0,270,271,5,111,0,0,271,272,5,108,0,0,272,273,5,101,0,0,273,274,
-        5,97,0,0,274,275,5,110,0,0,275,50,1,0,0,0,276,277,5,73,0,0,277,278,
-        5,110,0,0,278,279,5,116,0,0,279,280,5,101,0,0,280,281,5,103,0,0,
-        281,282,5,101,0,0,282,283,5,114,0,0,283,52,1,0,0,0,284,285,5,82,
-        0,0,285,286,5,101,0,0,286,287,5,97,0,0,287,288,5,108,0,0,288,54,
-        1,0,0,0,289,290,5,83,0,0,290,291,5,116,0,0,291,292,5,114,0,0,292,
-        293,5,105,0,0,293,294,5,110,0,0,294,295,5,103,0,0,295,56,1,0,0,0,
-        296,297,5,105,0,0,297,298,5,102,0,0,298,58,1,0,0,0,299,300,5,116,
-        0,0,300,301,5,104,0,0,301,302,5,101,0,0,302,303,5,110,0,0,303,60,
-        1,0,0,0,304,305,5,101,0,0,305,306,5,108,0,0,306,307,5,115,0,0,307,
-        308,5,101,0,0,308,62,1,0,0,0,309,310,5,101,0,0,310,311,5,110,0,0,
-        311,312,5,100,0,0,312,313,5,105,0,0,313,314,5,102,0,0,314,64,1,0,
-        0,0,315,316,5,97,0,0,316,317,5,110,0,0,317,318,5,100,0,0,318,66,
-        1,0,0,0,319,320,5,111,0,0,320,321,5,114,0,0,321,68,1,0,0,0,322,323,
-        5,110,0,0,323,324,5,111,0,0,324,325,5,116,0,0,325,70,1,0,0,0,326,
-        327,5,60,0,0,327,328,5,62,0,0,328,72,1,0,0,0,329,330,5,60,0,0,330,
-        74,1,0,0,0,331,332,5,60,0,0,332,333,5,61,0,0,333,76,1,0,0,0,334,
-        335,5,62,0,0,335,78,1,0,0,0,336,337,5,62,0,0,337,338,5,61,0,0,338,
-        80,1,0,0,0,339,340,5,124,0,0,340,82,1,0,0,0,341,342,5,83,0,0,342,
-        343,5,101,0,0,343,348,5,116,0,0,344,345,5,115,0,0,345,346,5,101,
-        0,0,346,348,5,116,0,0,347,341,1,0,0,0,347,344,1,0,0,0,348,84,1,0,
-        0,0,349,350,5,66,0,0,350,351,5,97,0,0,351,352,5,103,0,0,352,86,1,
-        0,0,0,353,354,5,83,0,0,354,355,5,101,0,0,355,356,5,113,0,0,356,357,
-        5,117,0,0,357,358,5,101,0,0,358,359,5,110,0,0,359,360,5,99,0,0,360,
-        361,5,101,0,0,361,88,1,0,0,0,362,363,5,79,0,0,363,364,5,114,0,0,
-        364,365,5,100,0,0,365,366,5,101,0,0,366,367,5,114,0,0,367,368,5,
-        101,0,0,368,369,5,100,0,0,369,370,5,83,0,0,370,371,5,101,0,0,371,
-        372,5,116,0,0,372,90,1,0,0,0,373,374,5,45,0,0,374,92,1,0,0,0,375,
-        376,5,43,0,0,376,94,1,0,0,0,377,378,5,47,0,0,378,96,1,0,0,0,379,
-        380,5,32,0,0,380,98,1,0,0,0,381,382,5,120,0,0,382,383,5,111,0,0,
-        383,384,5,114,0,0,384,100,1,0,0,0,385,386,5,105,0,0,386,387,5,109,
-        0,0,387,388,5,112,0,0,388,389,5,108,0,0,389,390,5,105,0,0,390,391,
-        5,101,0,0,391,392,5,115,0,0,392,102,1,0,0,0,393,394,5,111,0,0,394,
-        395,5,99,0,0,395,396,5,108,0,0,396,397,5,65,0,0,397,398,5,115,0,
-        0,398,399,5,84,0,0,399,400,5,121,0,0,400,401,5,112,0,0,401,402,5,
-        101,0,0,402,104,1,0,0,0,403,404,5,111,0,0,404,405,5,99,0,0,405,406,
-        5,108,0,0,406,407,5,73,0,0,407,408,5,115,0,0,408,409,5,84,0,0,409,
-        410,5,121,0,0,410,411,5,112,0,0,411,412,5,101,0,0,412,413,5,79,0,
-        0,413,414,5,102,0,0,414,106,1,0,0,0,415,416,5,111,0,0,416,417,5,
-        99,0,0,417,418,5,108,0,0,418,419,5,73,0,0,419,420,5,115,0,0,420,
-        421,5,75,0,0,421,422,5,105,0,0,422,423,5,110,0,0,423,424,5,100,0,
-        0,424,425,5,79,0,0,425,426,5,102,0,0,426,108,1,0,0,0,427,428,5,97,
-        0,0,428,429,5,108,0,0,429,430,5,108,0,0,430,431,5,73,0,0,431,432,
-        5,110,0,0,432,433,5,115,0,0,433,434,5,116,0,0,434,435,5,97,0,0,435,
-        436,5,110,0,0,436,437,5,99,0,0,437,438,5,101,0,0,438,439,5,115,0,
-        0,439,110,1,0,0,0,440,441,5,105,0,0,441,442,5,115,0,0,442,443,5,
-        69,0,0,443,444,5,109,0,0,444,445,5,112,0,0,445,446,5,116,0,0,446,
-        447,5,121,0,0,447,112,1,0,0,0,448,449,5,115,0,0,449,450,5,117,0,
-        0,450,451,5,109,0,0,451,114,1,0,0,0,452,453,5,115,0,0,453,454,5,
-        105,0,0,454,455,5,122,0,0,455,456,5,101,0,0,456,116,1,0,0,0,457,
-        458,5,105,0,0,458,459,5,110,0,0,459,460,5,99,0,0,460,461,5,108,0,
-        0,461,462,5,117,0,0,462,463,5,100,0,0,463,464,5,101,0,0,464,465,
-        5,115,0,0,465,118,1,0,0,0,466,467,5,101,0,0,467,468,5,120,0,0,468,
-        469,5,99,0,0,469,470,5,108,0,0,470,471,5,117,0,0,471,472,5,100,0,
-        0,472,473,5,101,0,0,473,474,5,115,0,0,474,120,1,0,0,0,475,476,5,
-        115,0,0,476,477,5,117,0,0,477,478,5,98,0,0,478,479,5,83,0,0,479,
-        480,5,101,0,0,480,481,5,113,0,0,481,482,5,117,0,0,482,483,5,101,
-        0,0,483,484,5,110,0,0,484,485,5,99,0,0,485,486,5,101,0,0,486,122,
-        1,0,0,0,487,488,5,115,0,0,488,489,5,117,0,0,489,490,5,98,0,0,490,
-        491,5,79,0,0,491,492,5,114,0,0,492,493,5,100,0,0,493,494,5,101,0,
-        0,494,495,5,114,0,0,495,496,5,101,0,0,496,497,5,100,0,0,497,498,
-        5,83,0,0,498,499,5,101,0,0,499,500,5,116,0,0,500,124,1,0,0,0,501,
-        502,5,112,0,0,502,503,5,114,0,0,503,504,5,101,0,0,504,505,5,112,
-        0,0,505,506,5,101,0,0,506,507,5,110,0,0,507,508,5,100,0,0,508,126,
-        1,0,0,0,509,510,5,108,0,0,510,511,5,97,0,0,511,512,5,115,0,0,512,
-        513,5,116,0,0,513,128,1,0,0,0,514,515,5,97,0,0,515,516,5,112,0,0,
-        516,517,5,112,0,0,517,518,5,101,0,0,518,519,5,110,0,0,519,520,5,
-        100,0,0,520,130,1,0,0,0,521,522,5,115,0,0,522,523,5,121,0,0,523,
-        524,5,109,0,0,524,525,5,109,0,0,525,526,5,101,0,0,526,527,5,116,
-        0,0,527,528,5,114,0,0,528,529,5,105,0,0,529,530,5,99,0,0,530,531,
-        5,68,0,0,531,532,5,105,0,0,532,533,5,102,0,0,533,534,5,102,0,0,534,
-        535,5,101,0,0,535,536,5,114,0,0,536,537,5,101,0,0,537,538,5,110,
-        0,0,538,539,5,99,0,0,539,540,5,101,0,0,540,132,1,0,0,0,541,542,5,
-        102,0,0,542,543,5,105,0,0,543,544,5,114,0,0,544,545,5,115,0,0,545,
-        546,5,116,0,0,546,134,1,0,0,0,547,548,5,100,0,0,548,549,5,101,0,
-        0,549,550,5,114,0,0,550,551,5,105,0,0,551,552,5,118,0,0,552,553,
-        5,101,0,0,553,136,1,0,0,0,554,555,5,98,0,0,555,556,5,111,0,0,556,
-        557,5,100,0,0,557,558,5,121,0,0,558,138,1,0,0,0,559,560,5,105,0,
-        0,560,561,5,110,0,0,561,562,5,105,0,0,562,563,5,116,0,0,563,140,
-        1,0,0,0,564,565,5,117,0,0,565,566,5,110,0,0,566,567,5,105,0,0,567,
-        568,5,111,0,0,568,569,5,110,0,0,569,142,1,0,0,0,570,571,5,110,0,
-        0,571,572,5,117,0,0,572,573,5,108,0,0,573,574,5,108,0,0,574,144,
-        1,0,0,0,575,576,5,108,0,0,576,577,5,101,0,0,577,578,5,116,0,0,578,
-        146,1,0,0,0,579,580,5,105,0,0,580,581,5,110,0,0,581,148,1,0,0,0,
-        582,583,5,45,0,0,583,588,5,62,0,0,584,585,5,226,0,0,585,586,5,8224,
-        0,0,586,588,5,8217,0,0,587,582,1,0,0,0,587,584,1,0,0,0,588,150,1,
-        0,0,0,589,590,5,100,0,0,590,591,5,101,0,0,591,592,5,102,0,0,592,
-        152,1,0,0,0,593,597,7,1,0,0,594,596,7,2,0,0,595,594,1,0,0,0,596,
-        599,1,0,0,0,597,595,1,0,0,0,597,598,1,0,0,0,598,154,1,0,0,0,599,
-        597,1,0,0,0,600,602,7,3,0,0,601,600,1,0,0,0,602,603,1,0,0,0,603,
-        601,1,0,0,0,603,604,1,0,0,0,604,611,1,0,0,0,605,607,5,46,0,0,606,
-        608,7,3,0,0,607,606,1,0,0,0,608,609,1,0,0,0,609,607,1,0,0,0,609,
-        610,1,0,0,0,610,612,1,0,0,0,611,605,1,0,0,0,611,612,1,0,0,0,612,
-        156,1,0,0,0,613,619,5,34,0,0,614,618,8,4,0,0,615,616,5,92,0,0,616,
-        618,9,0,0,0,617,614,1,0,0,0,617,615,1,0,0,0,618,621,1,0,0,0,619,
-        617,1,0,0,0,619,620,1,0,0,0,620,622,1,0,0,0,621,619,1,0,0,0,622,
-        623,5,34,0,0,623,158,1,0,0,0,624,625,5,116,0,0,625,626,5,114,0,0,
-        626,627,5,117,0,0,627,634,5,101,0,0,628,629,5,102,0,0,629,630,5,
-        97,0,0,630,631,5,108,0,0,631,632,5,115,0,0,632,634,5,101,0,0,633,
-        624,1,0,0,0,633,628,1,0,0,0,634,160,1,0,0,0,635,636,5,47,0,0,636,
-        637,5,42,0,0,637,641,1,0,0,0,638,640,9,0,0,0,639,638,1,0,0,0,640,
-        643,1,0,0,0,641,642,1,0,0,0,641,639,1,0,0,0,642,644,1,0,0,0,643,
-        641,1,0,0,0,644,645,5,42,0,0,645,646,5,47,0,0,646,647,1,0,0,0,647,
-        648,6,80,0,0,648,162,1,0,0,0,649,650,5,47,0,0,650,651,5,47,0,0,651,
-        655,1,0,0,0,652,654,8,5,0,0,653,652,1,0,0,0,654,657,1,0,0,0,655,
-        653,1,0,0,0,655,656,1,0,0,0,656,658,1,0,0,0,657,655,1,0,0,0,658,
-        659,6,81,0,0,659,164,1,0,0,0,13,0,238,347,587,597,603,609,611,617,
-        619,633,641,655,1,6,0,0
+        1,71,1,71,1,71,1,71,1,71,1,71,1,72,1,72,1,72,1,72,1,72,1,73,1,73,
+        1,73,1,73,1,74,1,74,1,74,1,75,1,75,1,75,1,75,1,75,3,75,592,8,75,
+        1,76,1,76,1,76,1,76,1,77,1,77,5,77,600,8,77,10,77,12,77,603,9,77,
+        1,78,4,78,606,8,78,11,78,12,78,607,1,78,1,78,4,78,612,8,78,11,78,
+        12,78,613,3,78,616,8,78,1,79,1,79,1,79,1,79,5,79,622,8,79,10,79,
+        12,79,625,9,79,1,79,3,79,628,8,79,1,79,1,79,1,79,1,79,1,79,3,79,
+        635,8,79,1,80,1,80,1,80,1,80,1,80,1,80,1,80,1,80,1,80,3,80,646,8,
+        80,1,81,1,81,1,81,1,81,5,81,652,8,81,10,81,12,81,655,9,81,1,81,1,
+        81,1,81,1,81,1,81,1,82,1,82,1,82,1,82,5,82,666,8,82,10,82,12,82,
+        669,9,82,1,82,1,82,1,653,0,83,1,1,3,2,5,3,7,4,9,5,11,6,13,7,15,8,
+        17,9,19,10,21,11,23,12,25,13,27,14,29,15,31,16,33,17,35,18,37,19,
+        39,20,41,21,43,22,45,23,47,24,49,25,51,26,53,27,55,28,57,29,59,30,
+        61,31,63,32,65,33,67,34,69,35,71,36,73,37,75,38,77,39,79,40,81,41,
+        83,42,85,43,87,44,89,45,91,46,93,47,95,48,97,49,99,50,101,51,103,
+        52,105,53,107,54,109,55,111,56,113,57,115,58,117,59,119,60,121,61,
+        123,62,125,63,127,64,129,65,131,66,133,67,135,68,137,69,139,70,141,
+        71,143,72,145,73,147,74,149,75,151,76,153,77,155,78,157,79,159,80,
+        161,81,163,82,165,83,1,0,6,3,0,9,10,13,13,32,32,3,0,65,90,95,95,
+        97,122,4,0,48,57,64,90,95,95,97,122,1,0,48,57,2,0,34,34,92,92,2,
+        0,10,10,13,13,685,0,1,1,0,0,0,0,3,1,0,0,0,0,5,1,0,0,0,0,7,1,0,0,
+        0,0,9,1,0,0,0,0,11,1,0,0,0,0,13,1,0,0,0,0,15,1,0,0,0,0,17,1,0,0,
+        0,0,19,1,0,0,0,0,21,1,0,0,0,0,23,1,0,0,0,0,25,1,0,0,0,0,27,1,0,0,
+        0,0,29,1,0,0,0,0,31,1,0,0,0,0,33,1,0,0,0,0,35,1,0,0,0,0,37,1,0,0,
+        0,0,39,1,0,0,0,0,41,1,0,0,0,0,43,1,0,0,0,0,45,1,0,0,0,0,47,1,0,0,
+        0,0,49,1,0,0,0,0,51,1,0,0,0,0,53,1,0,0,0,0,55,1,0,0,0,0,57,1,0,0,
+        0,0,59,1,0,0,0,0,61,1,0,0,0,0,63,1,0,0,0,0,65,1,0,0,0,0,67,1,0,0,
+        0,0,69,1,0,0,0,0,71,1,0,0,0,0,73,1,0,0,0,0,75,1,0,0,0,0,77,1,0,0,
+        0,0,79,1,0,0,0,0,81,1,0,0,0,0,83,1,0,0,0,0,85,1,0,0,0,0,87,1,0,0,
+        0,0,89,1,0,0,0,0,91,1,0,0,0,0,93,1,0,0,0,0,95,1,0,0,0,0,97,1,0,0,
+        0,0,99,1,0,0,0,0,101,1,0,0,0,0,103,1,0,0,0,0,105,1,0,0,0,0,107,1,
+        0,0,0,0,109,1,0,0,0,0,111,1,0,0,0,0,113,1,0,0,0,0,115,1,0,0,0,0,
+        117,1,0,0,0,0,119,1,0,0,0,0,121,1,0,0,0,0,123,1,0,0,0,0,125,1,0,
+        0,0,0,127,1,0,0,0,0,129,1,0,0,0,0,131,1,0,0,0,0,133,1,0,0,0,0,135,
+        1,0,0,0,0,137,1,0,0,0,0,139,1,0,0,0,0,141,1,0,0,0,0,143,1,0,0,0,
+        0,145,1,0,0,0,0,147,1,0,0,0,0,149,1,0,0,0,0,151,1,0,0,0,0,153,1,
+        0,0,0,0,155,1,0,0,0,0,157,1,0,0,0,0,159,1,0,0,0,0,161,1,0,0,0,0,
+        163,1,0,0,0,0,165,1,0,0,0,1,167,1,0,0,0,3,169,1,0,0,0,5,177,1,0,
+        0,0,7,181,1,0,0,0,9,185,1,0,0,0,11,190,1,0,0,0,13,195,1,0,0,0,15,
+        202,1,0,0,0,17,209,1,0,0,0,19,216,1,0,0,0,21,224,1,0,0,0,23,231,
+        1,0,0,0,25,240,1,0,0,0,27,246,1,0,0,0,29,249,1,0,0,0,31,252,1,0,
+        0,0,33,254,1,0,0,0,35,256,1,0,0,0,37,258,1,0,0,0,39,260,1,0,0,0,
+        41,262,1,0,0,0,43,264,1,0,0,0,45,266,1,0,0,0,47,268,1,0,0,0,49,270,
+        1,0,0,0,51,272,1,0,0,0,53,280,1,0,0,0,55,288,1,0,0,0,57,293,1,0,
+        0,0,59,300,1,0,0,0,61,303,1,0,0,0,63,308,1,0,0,0,65,313,1,0,0,0,
+        67,319,1,0,0,0,69,323,1,0,0,0,71,326,1,0,0,0,73,330,1,0,0,0,75,333,
+        1,0,0,0,77,335,1,0,0,0,79,338,1,0,0,0,81,340,1,0,0,0,83,343,1,0,
+        0,0,85,351,1,0,0,0,87,353,1,0,0,0,89,357,1,0,0,0,91,366,1,0,0,0,
+        93,377,1,0,0,0,95,379,1,0,0,0,97,381,1,0,0,0,99,383,1,0,0,0,101,
+        385,1,0,0,0,103,389,1,0,0,0,105,397,1,0,0,0,107,407,1,0,0,0,109,
+        419,1,0,0,0,111,431,1,0,0,0,113,444,1,0,0,0,115,452,1,0,0,0,117,
+        456,1,0,0,0,119,461,1,0,0,0,121,470,1,0,0,0,123,479,1,0,0,0,125,
+        491,1,0,0,0,127,505,1,0,0,0,129,513,1,0,0,0,131,518,1,0,0,0,133,
+        525,1,0,0,0,135,545,1,0,0,0,137,551,1,0,0,0,139,558,1,0,0,0,141,
+        563,1,0,0,0,143,568,1,0,0,0,145,574,1,0,0,0,147,579,1,0,0,0,149,
+        583,1,0,0,0,151,591,1,0,0,0,153,593,1,0,0,0,155,597,1,0,0,0,157,
+        605,1,0,0,0,159,634,1,0,0,0,161,645,1,0,0,0,163,647,1,0,0,0,165,
+        661,1,0,0,0,167,168,5,42,0,0,168,2,1,0,0,0,169,170,5,99,0,0,170,
+        171,5,111,0,0,171,172,5,110,0,0,172,173,5,116,0,0,173,174,5,101,
+        0,0,174,175,5,120,0,0,175,176,5,116,0,0,176,4,1,0,0,0,177,178,5,
+        105,0,0,178,179,5,110,0,0,179,180,5,118,0,0,180,6,1,0,0,0,181,182,
+        5,112,0,0,182,183,5,114,0,0,183,184,5,101,0,0,184,8,1,0,0,0,185,
+        186,5,112,0,0,186,187,5,111,0,0,187,188,5,115,0,0,188,189,5,116,
+        0,0,189,10,1,0,0,0,190,191,5,115,0,0,191,192,5,101,0,0,192,193,5,
+        108,0,0,193,194,5,102,0,0,194,12,1,0,0,0,195,196,5,102,0,0,196,197,
+        5,111,0,0,197,198,5,114,0,0,198,199,5,65,0,0,199,200,5,108,0,0,200,
+        201,5,108,0,0,201,14,1,0,0,0,202,203,5,101,0,0,203,204,5,120,0,0,
+        204,205,5,105,0,0,205,206,5,115,0,0,206,207,5,116,0,0,207,208,5,
+        115,0,0,208,16,1,0,0,0,209,210,5,115,0,0,210,211,5,101,0,0,211,212,
+        5,108,0,0,212,213,5,101,0,0,213,214,5,99,0,0,214,215,5,116,0,0,215,
+        18,1,0,0,0,216,217,5,99,0,0,217,218,5,111,0,0,218,219,5,108,0,0,
+        219,220,5,108,0,0,220,221,5,101,0,0,221,222,5,99,0,0,222,223,5,116,
+        0,0,223,20,1,0,0,0,224,225,5,79,0,0,225,226,5,99,0,0,226,227,5,108,
+        0,0,227,228,5,65,0,0,228,229,5,110,0,0,229,230,5,121,0,0,230,22,
+        1,0,0,0,231,232,5,79,0,0,232,233,5,99,0,0,233,234,5,108,0,0,234,
+        235,5,86,0,0,235,236,5,111,0,0,236,237,5,105,0,0,237,238,5,100,0,
+        0,238,24,1,0,0,0,239,241,7,0,0,0,240,239,1,0,0,0,241,242,1,0,0,0,
+        242,240,1,0,0,0,242,243,1,0,0,0,243,244,1,0,0,0,244,245,6,12,0,0,
+        245,26,1,0,0,0,246,247,5,46,0,0,247,248,5,46,0,0,248,28,1,0,0,0,
+        249,250,5,58,0,0,250,251,5,58,0,0,251,30,1,0,0,0,252,253,5,40,0,
+        0,253,32,1,0,0,0,254,255,5,41,0,0,255,34,1,0,0,0,256,257,5,123,0,
+        0,257,36,1,0,0,0,258,259,5,125,0,0,259,38,1,0,0,0,260,261,5,59,0,
+        0,261,40,1,0,0,0,262,263,5,58,0,0,263,42,1,0,0,0,264,265,5,44,0,
+        0,265,44,1,0,0,0,266,267,5,46,0,0,267,46,1,0,0,0,268,269,5,61,0,
+        0,269,48,1,0,0,0,270,271,5,39,0,0,271,50,1,0,0,0,272,273,5,66,0,
+        0,273,274,5,111,0,0,274,275,5,111,0,0,275,276,5,108,0,0,276,277,
+        5,101,0,0,277,278,5,97,0,0,278,279,5,110,0,0,279,52,1,0,0,0,280,
+        281,5,73,0,0,281,282,5,110,0,0,282,283,5,116,0,0,283,284,5,101,0,
+        0,284,285,5,103,0,0,285,286,5,101,0,0,286,287,5,114,0,0,287,54,1,
+        0,0,0,288,289,5,82,0,0,289,290,5,101,0,0,290,291,5,97,0,0,291,292,
+        5,108,0,0,292,56,1,0,0,0,293,294,5,83,0,0,294,295,5,116,0,0,295,
+        296,5,114,0,0,296,297,5,105,0,0,297,298,5,110,0,0,298,299,5,103,
+        0,0,299,58,1,0,0,0,300,301,5,105,0,0,301,302,5,102,0,0,302,60,1,
+        0,0,0,303,304,5,116,0,0,304,305,5,104,0,0,305,306,5,101,0,0,306,
+        307,5,110,0,0,307,62,1,0,0,0,308,309,5,101,0,0,309,310,5,108,0,0,
+        310,311,5,115,0,0,311,312,5,101,0,0,312,64,1,0,0,0,313,314,5,101,
+        0,0,314,315,5,110,0,0,315,316,5,100,0,0,316,317,5,105,0,0,317,318,
+        5,102,0,0,318,66,1,0,0,0,319,320,5,97,0,0,320,321,5,110,0,0,321,
+        322,5,100,0,0,322,68,1,0,0,0,323,324,5,111,0,0,324,325,5,114,0,0,
+        325,70,1,0,0,0,326,327,5,110,0,0,327,328,5,111,0,0,328,329,5,116,
+        0,0,329,72,1,0,0,0,330,331,5,60,0,0,331,332,5,62,0,0,332,74,1,0,
+        0,0,333,334,5,60,0,0,334,76,1,0,0,0,335,336,5,60,0,0,336,337,5,61,
+        0,0,337,78,1,0,0,0,338,339,5,62,0,0,339,80,1,0,0,0,340,341,5,62,
+        0,0,341,342,5,61,0,0,342,82,1,0,0,0,343,344,5,124,0,0,344,84,1,0,
+        0,0,345,346,5,83,0,0,346,347,5,101,0,0,347,352,5,116,0,0,348,349,
+        5,115,0,0,349,350,5,101,0,0,350,352,5,116,0,0,351,345,1,0,0,0,351,
+        348,1,0,0,0,352,86,1,0,0,0,353,354,5,66,0,0,354,355,5,97,0,0,355,
+        356,5,103,0,0,356,88,1,0,0,0,357,358,5,83,0,0,358,359,5,101,0,0,
+        359,360,5,113,0,0,360,361,5,117,0,0,361,362,5,101,0,0,362,363,5,
+        110,0,0,363,364,5,99,0,0,364,365,5,101,0,0,365,90,1,0,0,0,366,367,
+        5,79,0,0,367,368,5,114,0,0,368,369,5,100,0,0,369,370,5,101,0,0,370,
+        371,5,114,0,0,371,372,5,101,0,0,372,373,5,100,0,0,373,374,5,83,0,
+        0,374,375,5,101,0,0,375,376,5,116,0,0,376,92,1,0,0,0,377,378,5,45,
+        0,0,378,94,1,0,0,0,379,380,5,43,0,0,380,96,1,0,0,0,381,382,5,47,
+        0,0,382,98,1,0,0,0,383,384,5,32,0,0,384,100,1,0,0,0,385,386,5,120,
+        0,0,386,387,5,111,0,0,387,388,5,114,0,0,388,102,1,0,0,0,389,390,
+        5,105,0,0,390,391,5,109,0,0,391,392,5,112,0,0,392,393,5,108,0,0,
+        393,394,5,105,0,0,394,395,5,101,0,0,395,396,5,115,0,0,396,104,1,
+        0,0,0,397,398,5,111,0,0,398,399,5,99,0,0,399,400,5,108,0,0,400,401,
+        5,65,0,0,401,402,5,115,0,0,402,403,5,84,0,0,403,404,5,121,0,0,404,
+        405,5,112,0,0,405,406,5,101,0,0,406,106,1,0,0,0,407,408,5,111,0,
+        0,408,409,5,99,0,0,409,410,5,108,0,0,410,411,5,73,0,0,411,412,5,
+        115,0,0,412,413,5,84,0,0,413,414,5,121,0,0,414,415,5,112,0,0,415,
+        416,5,101,0,0,416,417,5,79,0,0,417,418,5,102,0,0,418,108,1,0,0,0,
+        419,420,5,111,0,0,420,421,5,99,0,0,421,422,5,108,0,0,422,423,5,73,
+        0,0,423,424,5,115,0,0,424,425,5,75,0,0,425,426,5,105,0,0,426,427,
+        5,110,0,0,427,428,5,100,0,0,428,429,5,79,0,0,429,430,5,102,0,0,430,
+        110,1,0,0,0,431,432,5,97,0,0,432,433,5,108,0,0,433,434,5,108,0,0,
+        434,435,5,73,0,0,435,436,5,110,0,0,436,437,5,115,0,0,437,438,5,116,
+        0,0,438,439,5,97,0,0,439,440,5,110,0,0,440,441,5,99,0,0,441,442,
+        5,101,0,0,442,443,5,115,0,0,443,112,1,0,0,0,444,445,5,105,0,0,445,
+        446,5,115,0,0,446,447,5,69,0,0,447,448,5,109,0,0,448,449,5,112,0,
+        0,449,450,5,116,0,0,450,451,5,121,0,0,451,114,1,0,0,0,452,453,5,
+        115,0,0,453,454,5,117,0,0,454,455,5,109,0,0,455,116,1,0,0,0,456,
+        457,5,115,0,0,457,458,5,105,0,0,458,459,5,122,0,0,459,460,5,101,
+        0,0,460,118,1,0,0,0,461,462,5,105,0,0,462,463,5,110,0,0,463,464,
+        5,99,0,0,464,465,5,108,0,0,465,466,5,117,0,0,466,467,5,100,0,0,467,
+        468,5,101,0,0,468,469,5,115,0,0,469,120,1,0,0,0,470,471,5,101,0,
+        0,471,472,5,120,0,0,472,473,5,99,0,0,473,474,5,108,0,0,474,475,5,
+        117,0,0,475,476,5,100,0,0,476,477,5,101,0,0,477,478,5,115,0,0,478,
+        122,1,0,0,0,479,480,5,115,0,0,480,481,5,117,0,0,481,482,5,98,0,0,
+        482,483,5,83,0,0,483,484,5,101,0,0,484,485,5,113,0,0,485,486,5,117,
+        0,0,486,487,5,101,0,0,487,488,5,110,0,0,488,489,5,99,0,0,489,490,
+        5,101,0,0,490,124,1,0,0,0,491,492,5,115,0,0,492,493,5,117,0,0,493,
+        494,5,98,0,0,494,495,5,79,0,0,495,496,5,114,0,0,496,497,5,100,0,
+        0,497,498,5,101,0,0,498,499,5,114,0,0,499,500,5,101,0,0,500,501,
+        5,100,0,0,501,502,5,83,0,0,502,503,5,101,0,0,503,504,5,116,0,0,504,
+        126,1,0,0,0,505,506,5,112,0,0,506,507,5,114,0,0,507,508,5,101,0,
+        0,508,509,5,112,0,0,509,510,5,101,0,0,510,511,5,110,0,0,511,512,
+        5,100,0,0,512,128,1,0,0,0,513,514,5,108,0,0,514,515,5,97,0,0,515,
+        516,5,115,0,0,516,517,5,116,0,0,517,130,1,0,0,0,518,519,5,97,0,0,
+        519,520,5,112,0,0,520,521,5,112,0,0,521,522,5,101,0,0,522,523,5,
+        110,0,0,523,524,5,100,0,0,524,132,1,0,0,0,525,526,5,115,0,0,526,
+        527,5,121,0,0,527,528,5,109,0,0,528,529,5,109,0,0,529,530,5,101,
+        0,0,530,531,5,116,0,0,531,532,5,114,0,0,532,533,5,105,0,0,533,534,
+        5,99,0,0,534,535,5,68,0,0,535,536,5,105,0,0,536,537,5,102,0,0,537,
+        538,5,102,0,0,538,539,5,101,0,0,539,540,5,114,0,0,540,541,5,101,
+        0,0,541,542,5,110,0,0,542,543,5,99,0,0,543,544,5,101,0,0,544,134,
+        1,0,0,0,545,546,5,102,0,0,546,547,5,105,0,0,547,548,5,114,0,0,548,
+        549,5,115,0,0,549,550,5,116,0,0,550,136,1,0,0,0,551,552,5,100,0,
+        0,552,553,5,101,0,0,553,554,5,114,0,0,554,555,5,105,0,0,555,556,
+        5,118,0,0,556,557,5,101,0,0,557,138,1,0,0,0,558,559,5,98,0,0,559,
+        560,5,111,0,0,560,561,5,100,0,0,561,562,5,121,0,0,562,140,1,0,0,
+        0,563,564,5,105,0,0,564,565,5,110,0,0,565,566,5,105,0,0,566,567,
+        5,116,0,0,567,142,1,0,0,0,568,569,5,117,0,0,569,570,5,110,0,0,570,
+        571,5,105,0,0,571,572,5,111,0,0,572,573,5,110,0,0,573,144,1,0,0,
+        0,574,575,5,110,0,0,575,576,5,117,0,0,576,577,5,108,0,0,577,578,
+        5,108,0,0,578,146,1,0,0,0,579,580,5,108,0,0,580,581,5,101,0,0,581,
+        582,5,116,0,0,582,148,1,0,0,0,583,584,5,105,0,0,584,585,5,110,0,
+        0,585,150,1,0,0,0,586,587,5,45,0,0,587,592,5,62,0,0,588,589,5,226,
+        0,0,589,590,5,8224,0,0,590,592,5,8217,0,0,591,586,1,0,0,0,591,588,
+        1,0,0,0,592,152,1,0,0,0,593,594,5,100,0,0,594,595,5,101,0,0,595,
+        596,5,102,0,0,596,154,1,0,0,0,597,601,7,1,0,0,598,600,7,2,0,0,599,
+        598,1,0,0,0,600,603,1,0,0,0,601,599,1,0,0,0,601,602,1,0,0,0,602,
+        156,1,0,0,0,603,601,1,0,0,0,604,606,7,3,0,0,605,604,1,0,0,0,606,
+        607,1,0,0,0,607,605,1,0,0,0,607,608,1,0,0,0,608,615,1,0,0,0,609,
+        611,5,46,0,0,610,612,7,3,0,0,611,610,1,0,0,0,612,613,1,0,0,0,613,
+        611,1,0,0,0,613,614,1,0,0,0,614,616,1,0,0,0,615,609,1,0,0,0,615,
+        616,1,0,0,0,616,158,1,0,0,0,617,623,5,34,0,0,618,622,8,4,0,0,619,
+        620,5,92,0,0,620,622,9,0,0,0,621,618,1,0,0,0,621,619,1,0,0,0,622,
+        625,1,0,0,0,623,621,1,0,0,0,623,624,1,0,0,0,624,627,1,0,0,0,625,
+        623,1,0,0,0,626,628,3,155,77,0,627,626,1,0,0,0,627,628,1,0,0,0,628,
+        629,1,0,0,0,629,635,5,34,0,0,630,631,3,49,24,0,631,632,3,155,77,
+        0,632,633,3,49,24,0,633,635,1,0,0,0,634,617,1,0,0,0,634,630,1,0,
+        0,0,635,160,1,0,0,0,636,637,5,116,0,0,637,638,5,114,0,0,638,639,
+        5,117,0,0,639,646,5,101,0,0,640,641,5,102,0,0,641,642,5,97,0,0,642,
+        643,5,108,0,0,643,644,5,115,0,0,644,646,5,101,0,0,645,636,1,0,0,
+        0,645,640,1,0,0,0,646,162,1,0,0,0,647,648,5,47,0,0,648,649,5,42,
+        0,0,649,653,1,0,0,0,650,652,9,0,0,0,651,650,1,0,0,0,652,655,1,0,
+        0,0,653,654,1,0,0,0,653,651,1,0,0,0,654,656,1,0,0,0,655,653,1,0,
+        0,0,656,657,5,42,0,0,657,658,5,47,0,0,658,659,1,0,0,0,659,660,6,
+        81,0,0,660,164,1,0,0,0,661,662,5,47,0,0,662,663,5,47,0,0,663,667,
+        1,0,0,0,664,666,8,5,0,0,665,664,1,0,0,0,666,669,1,0,0,0,667,665,
+        1,0,0,0,667,668,1,0,0,0,668,670,1,0,0,0,669,667,1,0,0,0,670,671,
+        6,82,0,0,671,166,1,0,0,0,15,0,242,351,591,601,607,613,615,621,623,
+        627,634,645,653,667,1,6,0,0
     ]
 
-class OCLsLexer(Lexer):
+class BOCLLexer(Lexer):
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
-    CONTEXT = 1
-    INV = 2
-    PRE = 3
-    POST = 4
-    SELF = 5
-    FORALL = 6
-    EXISTS = 7
-    SELECT = 8
-    COLLECT = 9
-    OCLANY = 10
-    OCLVOID = 11
-    WS = 12
-    DoubleDots = 13
-    DoubleCOLON = 14
-    LPAREN = 15
-    RPAREN = 16
-    LBRACE = 17
-    RBRACE = 18
-    SEMI = 19
-    COLON = 20
-    COMMA = 21
-    DOT = 22
-    EQUAL = 23
-    SingleQuote = 24
-    BOOLEAN_TYPE = 25
-    INTEGER_TYPE = 26
-    REAL_TYPE = 27
-    STRING_TYPE = 28
-    IF = 29
-    THEN = 30
-    ELSE = 31
-    ENDIF = 32
-    AND = 33
-    OR = 34
-    NOT = 35
-    NOTEQUAL = 36
-    LT = 37
-    LE = 38
-    GT = 39
-    GE = 40
-    PIPE = 41
-    SET = 42
-    BAG = 43
-    SEQUENCE = 44
-    ORDEREDSET = 45
-    MINUS = 46
-    PLUS = 47
-    Divide = 48
-    EMPTYSTRING = 49
-    XOR = 50
-    IMPLIES = 51
-    OCLASTYPE = 52
-    OCLISTYPEOF = 53
-    OCLISKINDOF = 54
-    ALLINSTANCES = 55
-    ISEMPTY = 56
-    SUM = 57
-    SIZE = 58
-    INCLUDES = 59
-    EXCLUDES = 60
-    SUBSEQUENCE = 61
-    SUBORDEREDSET = 62
-    PREPEND = 63
-    LAST = 64
-    APPEND = 65
-    SYMMETRICDIFFERENCE = 66
-    FIRST = 67
-    DERIVE = 68
-    BODY = 69
-    Init = 70
-    UNION = 71
-    NULL = 72
-    LET = 73
-    IN = 74
-    Arrow = 75
-    Def = 76
-    ID = 77
-    NUMBER = 78
-    STRING_LITERAL = 79
-    BOOLEAN_LITERAL = 80
-    COMMENT = 81
-    LINE_COMMENT = 82
+    T__0 = 1
+    CONTEXT = 2
+    INV = 3
+    PRE = 4
+    POST = 5
+    SELF = 6
+    FORALL = 7
+    EXISTS = 8
+    SELECT = 9
+    COLLECT = 10
+    OCLANY = 11
+    OCLVOID = 12
+    WS = 13
+    DoubleDots = 14
+    DoubleCOLON = 15
+    LPAREN = 16
+    RPAREN = 17
+    LBRACE = 18
+    RBRACE = 19
+    SEMI = 20
+    COLON = 21
+    COMMA = 22
+    DOT = 23
+    EQUAL = 24
+    SingleQuote = 25
+    BOOLEAN_TYPE = 26
+    INTEGER_TYPE = 27
+    REAL_TYPE = 28
+    STRING_TYPE = 29
+    IF = 30
+    THEN = 31
+    ELSE = 32
+    ENDIF = 33
+    AND = 34
+    OR = 35
+    NOT = 36
+    NOTEQUAL = 37
+    LT = 38
+    LE = 39
+    GT = 40
+    GE = 41
+    PIPE = 42
+    SET = 43
+    BAG = 44
+    SEQUENCE = 45
+    ORDEREDSET = 46
+    MINUS = 47
+    PLUS = 48
+    Divide = 49
+    EMPTYSTRING = 50
+    XOR = 51
+    IMPLIES = 52
+    OCLASTYPE = 53
+    OCLISTYPEOF = 54
+    OCLISKINDOF = 55
+    ALLINSTANCES = 56
+    ISEMPTY = 57
+    SUM = 58
+    SIZE = 59
+    INCLUDES = 60
+    EXCLUDES = 61
+    SUBSEQUENCE = 62
+    SUBORDEREDSET = 63
+    PREPEND = 64
+    LAST = 65
+    APPEND = 66
+    SYMMETRICDIFFERENCE = 67
+    FIRST = 68
+    DERIVE = 69
+    BODY = 70
+    Init = 71
+    UNION = 72
+    NULL = 73
+    LET = 74
+    IN = 75
+    Arrow = 76
+    Def = 77
+    ID = 78
+    NUMBER = 79
+    STRING_LITERAL = 80
+    BOOLEAN_LITERAL = 81
+    COMMENT = 82
+    LINE_COMMENT = 83
 
     channelNames = [ u"DEFAULT_TOKEN_CHANNEL", u"HIDDEN" ]
 
     modeNames = [ "DEFAULT_MODE" ]
 
     literalNames = [ "<INVALID>",
-            "'context'", "'inv'", "'pre'", "'post'", "'self'", "'forAll'", 
+            "'*'", "'context'", "'inv'", "'pre'", "'post'", "'self'", "'forAll'", 
             "'exists'", "'select'", "'collect'", "'OclAny'", "'OclVoid'", 
             "'..'", "'::'", "'('", "')'", "'{'", "'}'", "';'", "':'", "','", 
             "'.'", "'='", "'''", "'Boolean'", "'Integer'", "'Real'", "'String'", 
             "'if'", "'then'", "'else'", "'endif'", "'and'", "'or'", "'not'", 
             "'<>'", "'<'", "'<='", "'>'", "'>='", "'|'", "'Bag'", "'Sequence'", 
             "'OrderedSet'", "'-'", "'+'", "'/'", "' '", "'xor'", "'implies'", 
             "'oclAsType'", "'oclIsTypeOf'", "'oclIsKindOf'", "'allInstances'", 
@@ -363,31 +369,31 @@
             "Divide", "EMPTYSTRING", "XOR", "IMPLIES", "OCLASTYPE", "OCLISTYPEOF", 
             "OCLISKINDOF", "ALLINSTANCES", "ISEMPTY", "SUM", "SIZE", "INCLUDES", 
             "EXCLUDES", "SUBSEQUENCE", "SUBORDEREDSET", "PREPEND", "LAST", 
             "APPEND", "SYMMETRICDIFFERENCE", "FIRST", "DERIVE", "BODY", 
             "Init", "UNION", "NULL", "LET", "IN", "Arrow", "Def", "ID", 
             "NUMBER", "STRING_LITERAL", "BOOLEAN_LITERAL", "COMMENT", "LINE_COMMENT" ]
 
-    ruleNames = [ "CONTEXT", "INV", "PRE", "POST", "SELF", "FORALL", "EXISTS", 
-                  "SELECT", "COLLECT", "OCLANY", "OCLVOID", "WS", "DoubleDots", 
-                  "DoubleCOLON", "LPAREN", "RPAREN", "LBRACE", "RBRACE", 
-                  "SEMI", "COLON", "COMMA", "DOT", "EQUAL", "SingleQuote", 
+    ruleNames = [ "T__0", "CONTEXT", "INV", "PRE", "POST", "SELF", "FORALL", 
+                  "EXISTS", "SELECT", "COLLECT", "OCLANY", "OCLVOID", "WS", 
+                  "DoubleDots", "DoubleCOLON", "LPAREN", "RPAREN", "LBRACE", 
+                  "RBRACE", "SEMI", "COLON", "COMMA", "DOT", "EQUAL", "SingleQuote", 
                   "BOOLEAN_TYPE", "INTEGER_TYPE", "REAL_TYPE", "STRING_TYPE", 
                   "IF", "THEN", "ELSE", "ENDIF", "AND", "OR", "NOT", "NOTEQUAL", 
                   "LT", "LE", "GT", "GE", "PIPE", "SET", "BAG", "SEQUENCE", 
                   "ORDEREDSET", "MINUS", "PLUS", "Divide", "EMPTYSTRING", 
                   "XOR", "IMPLIES", "OCLASTYPE", "OCLISTYPEOF", "OCLISKINDOF", 
                   "ALLINSTANCES", "ISEMPTY", "SUM", "SIZE", "INCLUDES", 
                   "EXCLUDES", "SUBSEQUENCE", "SUBORDEREDSET", "PREPEND", 
                   "LAST", "APPEND", "SYMMETRICDIFFERENCE", "FIRST", "DERIVE", 
                   "BODY", "Init", "UNION", "NULL", "LET", "IN", "Arrow", 
                   "Def", "ID", "NUMBER", "STRING_LITERAL", "BOOLEAN_LITERAL", 
                   "COMMENT", "LINE_COMMENT" ]
 
-    grammarFileName = "OCLs.g4"
+    grammarFileName = "BOCL.g4"
 
     def __init__(self, input=None, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = LexerATNSimulator(self, self.atn, self.decisionsToDFA, PredictionContextCache())
         self._actions = None
         self._predicates = None
```

### Comparing `besser-1.0.0/besser/BUML/notations/ocl/OCLsParser.py` & `besser-1.0.1/besser/BUML/notations/ocl/BOCLParser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,546 +1,569 @@
-# Generated from OCLs.g4 by ANTLR 4.13.1
+# Generated from BOCL.g4 by ANTLR 4.13.1
 # encoding: utf-8
 from antlr4 import *
 from io import StringIO
 import sys
 if sys.version_info[1] > 5:
 	from typing import TextIO
 else:
 	from typing.io import TextIO
 
 def serializedATN():
     return [
-        4,1,82,949,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
+        4,1,83,991,2,0,7,0,2,1,7,1,2,2,7,2,2,3,7,3,2,4,7,4,2,5,7,5,2,6,7,
         6,2,7,7,7,2,8,7,8,2,9,7,9,2,10,7,10,2,11,7,11,2,12,7,12,2,13,7,13,
-        1,0,1,0,5,0,31,8,0,10,0,12,0,34,9,0,1,1,1,1,1,1,1,1,3,1,40,8,1,1,
-        1,3,1,43,8,1,1,1,5,1,46,8,1,10,1,12,1,49,9,1,1,1,3,1,52,8,1,1,1,
-        3,1,55,8,1,1,1,3,1,58,8,1,1,1,3,1,61,8,1,1,1,3,1,64,8,1,1,1,3,1,
-        67,8,1,1,1,3,1,70,8,1,1,1,3,1,73,8,1,1,1,3,1,76,8,1,1,1,3,1,79,8,
-        1,1,1,3,1,82,8,1,1,1,3,1,85,8,1,1,2,1,2,3,2,89,8,2,1,2,1,2,1,2,3,
-        2,94,8,2,1,3,1,3,1,3,3,3,99,8,3,1,3,1,3,3,3,103,8,3,1,3,3,3,106,
-        8,3,5,3,108,8,3,10,3,12,3,111,9,3,1,3,1,3,1,3,1,3,1,3,1,3,5,3,119,
-        8,3,10,3,12,3,122,9,3,1,3,1,3,1,3,1,3,3,3,128,8,3,5,3,130,8,3,10,
-        3,12,3,133,9,3,1,3,3,3,136,8,3,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,1,
-        4,3,4,147,8,4,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,
-        5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,3,5,169,8,5,1,6,1,6,1,7,3,7,174,8,
-        7,1,7,1,7,3,7,178,8,7,1,7,1,7,3,7,182,8,7,1,7,1,7,1,7,1,7,1,7,1,
-        7,1,7,1,7,1,7,1,7,1,7,5,7,195,8,7,10,7,12,7,198,9,7,1,7,1,7,1,7,
-        1,7,1,7,1,7,3,7,206,8,7,1,7,1,7,1,7,5,7,211,8,7,10,7,12,7,214,9,
-        7,1,7,1,7,1,7,1,7,1,7,1,7,3,7,222,8,7,1,7,1,7,1,7,5,7,227,8,7,10,
-        7,12,7,230,9,7,1,7,1,7,1,7,1,7,1,7,1,7,3,7,238,8,7,1,7,3,7,241,8,
-        7,1,7,1,7,5,7,245,8,7,10,7,12,7,248,9,7,1,7,1,7,1,7,1,7,1,7,3,7,
-        255,8,7,1,7,5,7,258,8,7,10,7,12,7,261,9,7,1,7,3,7,264,8,7,1,7,1,
-        7,5,7,268,8,7,10,7,12,7,271,9,7,1,7,1,7,1,7,1,7,1,7,3,7,278,8,7,
-        1,7,5,7,281,8,7,10,7,12,7,284,9,7,1,7,3,7,287,8,7,1,7,1,7,5,7,291,
-        8,7,10,7,12,7,294,9,7,1,7,1,7,1,7,1,7,1,7,3,7,301,8,7,1,7,5,7,304,
-        8,7,10,7,12,7,307,9,7,1,7,3,7,310,8,7,1,7,1,7,1,7,1,7,1,7,3,7,317,
-        8,7,1,7,5,7,320,8,7,10,7,12,7,323,9,7,1,7,3,7,326,8,7,1,7,1,7,1,
-        7,1,7,1,7,3,7,333,8,7,1,7,5,7,336,8,7,10,7,12,7,339,9,7,1,7,3,7,
-        342,8,7,1,7,5,7,345,8,7,10,7,12,7,348,9,7,1,7,1,7,5,7,352,8,7,10,
-        7,12,7,355,9,7,1,7,5,7,358,8,7,10,7,12,7,361,9,7,1,7,3,7,364,8,7,
-        1,7,1,7,3,7,368,8,7,1,7,3,7,371,8,7,5,7,373,8,7,10,7,12,7,376,9,
-        7,1,7,5,7,379,8,7,10,7,12,7,382,9,7,1,7,5,7,385,8,7,10,7,12,7,388,
-        9,7,1,7,3,7,391,8,7,1,7,3,7,394,8,7,1,7,5,7,397,8,7,10,7,12,7,400,
-        9,7,1,7,1,7,5,7,404,8,7,10,7,12,7,407,9,7,1,7,5,7,410,8,7,10,7,12,
-        7,413,9,7,1,7,3,7,416,8,7,1,7,1,7,3,7,420,8,7,1,7,3,7,423,8,7,5,
-        7,425,8,7,10,7,12,7,428,9,7,1,7,5,7,431,8,7,10,7,12,7,434,9,7,1,
-        7,5,7,437,8,7,10,7,12,7,440,9,7,1,7,3,7,443,8,7,1,7,3,7,446,8,7,
-        1,7,1,7,4,7,450,8,7,11,7,12,7,451,1,7,1,7,4,7,456,8,7,11,7,12,7,
-        457,1,7,3,7,461,8,7,1,7,3,7,464,8,7,1,7,5,7,467,8,7,10,7,12,7,470,
-        9,7,1,7,1,7,1,7,3,7,475,8,7,1,7,1,7,3,7,479,8,7,1,7,3,7,482,8,7,
-        5,7,484,8,7,10,7,12,7,487,9,7,1,7,1,7,5,7,491,8,7,10,7,12,7,494,
-        9,7,1,7,3,7,497,8,7,1,7,3,7,500,8,7,1,7,5,7,503,8,7,10,7,12,7,506,
-        9,7,1,7,1,7,5,7,510,8,7,10,7,12,7,513,9,7,1,7,5,7,516,8,7,10,7,12,
-        7,519,9,7,1,7,3,7,522,8,7,1,7,1,7,3,7,526,8,7,1,7,3,7,529,8,7,5,
-        7,531,8,7,10,7,12,7,534,9,7,1,7,5,7,537,8,7,10,7,12,7,540,9,7,1,
-        7,5,7,543,8,7,10,7,12,7,546,9,7,1,7,3,7,549,8,7,1,7,1,7,3,7,553,
-        8,7,1,7,5,7,556,8,7,10,7,12,7,559,9,7,1,7,1,7,5,7,563,8,7,10,7,12,
-        7,566,9,7,1,7,5,7,569,8,7,10,7,12,7,572,9,7,1,7,3,7,575,8,7,1,7,
-        1,7,3,7,579,8,7,1,7,3,7,582,8,7,5,7,584,8,7,10,7,12,7,587,9,7,1,
-        7,5,7,590,8,7,10,7,12,7,593,9,7,1,7,5,7,596,8,7,10,7,12,7,599,9,
-        7,1,7,3,7,602,8,7,1,7,3,7,605,8,7,1,7,5,7,608,8,7,10,7,12,7,611,
-        9,7,1,7,1,7,5,7,615,8,7,10,7,12,7,618,9,7,1,7,5,7,621,8,7,10,7,12,
-        7,624,9,7,1,7,3,7,627,8,7,1,7,1,7,3,7,631,8,7,1,7,3,7,634,8,7,5,
-        7,636,8,7,10,7,12,7,639,9,7,1,7,5,7,642,8,7,10,7,12,7,645,9,7,1,
-        7,5,7,648,8,7,10,7,12,7,651,9,7,1,7,3,7,654,8,7,1,7,1,7,1,7,4,7,
-        659,8,7,11,7,12,7,660,1,7,3,7,664,8,7,1,7,1,7,3,7,668,8,7,1,7,3,
-        7,671,8,7,5,7,673,8,7,10,7,12,7,676,9,7,1,7,4,7,679,8,7,11,7,12,
-        7,680,1,7,3,7,684,8,7,1,7,1,7,1,7,1,7,4,7,690,8,7,11,7,12,7,691,
-        1,7,3,7,695,8,7,1,7,1,7,1,7,1,7,3,7,701,8,7,1,7,1,7,3,7,705,8,7,
-        1,7,3,7,708,8,7,5,7,710,8,7,10,7,12,7,713,9,7,1,7,4,7,716,8,7,11,
-        7,12,7,717,1,7,3,7,721,8,7,1,7,3,7,724,8,7,1,7,1,7,1,7,1,7,1,7,3,
-        7,731,8,7,1,7,3,7,734,8,7,4,7,736,8,7,11,7,12,7,737,1,7,1,7,1,7,
-        1,7,3,7,744,8,7,1,7,3,7,747,8,7,1,7,1,7,1,7,1,7,1,7,3,7,754,8,7,
-        1,7,1,7,1,7,1,7,1,7,4,7,761,8,7,11,7,12,7,762,1,7,3,7,766,8,7,1,
-        7,1,7,1,7,1,7,1,7,3,7,773,8,7,1,7,1,7,1,7,1,7,1,7,3,7,780,8,7,1,
-        7,1,7,1,7,1,7,1,7,1,7,3,7,788,8,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,
-        7,1,7,5,7,799,8,7,10,7,12,7,802,9,7,1,7,3,7,805,8,7,1,7,1,7,5,7,
-        809,8,7,10,7,12,7,812,9,7,1,7,3,7,815,8,7,1,7,3,7,818,8,7,1,7,1,
-        7,4,7,822,8,7,11,7,12,7,823,1,7,3,7,827,8,7,1,7,1,7,5,7,831,8,7,
-        10,7,12,7,834,9,7,1,7,5,7,837,8,7,10,7,12,7,840,9,7,1,7,1,7,3,7,
-        844,8,7,1,7,3,7,847,8,7,1,7,1,7,3,7,851,8,7,1,7,1,7,1,7,1,7,3,7,
-        857,8,7,1,7,3,7,860,8,7,1,7,1,7,3,7,864,8,7,1,7,1,7,3,7,868,8,7,
-        1,7,1,7,1,7,3,7,873,8,7,1,7,1,7,3,7,877,8,7,1,7,3,7,880,8,7,1,7,
-        1,7,3,7,884,8,7,1,8,1,8,1,8,5,8,889,8,8,10,8,12,8,892,9,8,1,8,3,
-        8,895,8,8,1,8,1,8,5,8,899,8,8,10,8,12,8,902,9,8,1,8,1,8,1,8,1,8,
-        5,8,908,8,8,10,8,12,8,911,9,8,1,8,3,8,914,8,8,1,9,1,9,1,9,1,10,1,
-        10,1,11,1,11,3,11,923,8,11,1,11,1,11,3,11,927,8,11,1,11,3,11,930,
-        8,11,1,11,3,11,933,8,11,3,11,935,8,11,1,12,1,12,1,12,1,12,1,12,1,
-        12,1,12,1,12,3,12,945,8,12,1,13,1,13,1,13,0,0,14,0,2,4,6,8,10,12,
-        14,16,18,20,22,24,26,0,7,3,0,3,4,68,70,76,76,1,0,2,4,1,0,33,34,1,
-        0,6,9,2,0,35,35,46,46,4,0,23,23,33,34,36,40,46,51,2,0,72,72,78,80,
-        1163,0,28,1,0,0,0,2,35,1,0,0,0,4,86,1,0,0,0,6,135,1,0,0,0,8,146,
-        1,0,0,0,10,168,1,0,0,0,12,170,1,0,0,0,14,883,1,0,0,0,16,894,1,0,
-        0,0,18,915,1,0,0,0,20,918,1,0,0,0,22,934,1,0,0,0,24,944,1,0,0,0,
-        26,946,1,0,0,0,28,32,3,2,1,0,29,31,3,14,7,0,30,29,1,0,0,0,31,34,
-        1,0,0,0,32,30,1,0,0,0,32,33,1,0,0,0,33,1,1,0,0,0,34,32,1,0,0,0,35,
-        36,5,1,0,0,36,39,5,77,0,0,37,38,5,20,0,0,38,40,3,8,4,0,39,37,1,0,
-        0,0,39,40,1,0,0,0,40,42,1,0,0,0,41,43,5,17,0,0,42,41,1,0,0,0,42,
-        43,1,0,0,0,43,47,1,0,0,0,44,46,3,4,2,0,45,44,1,0,0,0,46,49,1,0,0,
-        0,47,45,1,0,0,0,47,48,1,0,0,0,48,51,1,0,0,0,49,47,1,0,0,0,50,52,
-        5,18,0,0,51,50,1,0,0,0,51,52,1,0,0,0,52,54,1,0,0,0,53,55,5,14,0,
-        0,54,53,1,0,0,0,54,55,1,0,0,0,55,57,1,0,0,0,56,58,3,6,3,0,57,56,
-        1,0,0,0,57,58,1,0,0,0,58,60,1,0,0,0,59,61,5,20,0,0,60,59,1,0,0,0,
-        60,61,1,0,0,0,61,63,1,0,0,0,62,64,3,8,4,0,63,62,1,0,0,0,63,64,1,
-        0,0,0,64,66,1,0,0,0,65,67,5,15,0,0,66,65,1,0,0,0,66,67,1,0,0,0,67,
-        69,1,0,0,0,68,70,5,77,0,0,69,68,1,0,0,0,69,70,1,0,0,0,70,72,1,0,
-        0,0,71,73,5,16,0,0,72,71,1,0,0,0,72,73,1,0,0,0,73,75,1,0,0,0,74,
-        76,5,20,0,0,75,74,1,0,0,0,75,76,1,0,0,0,76,78,1,0,0,0,77,79,7,0,
-        0,0,78,77,1,0,0,0,78,79,1,0,0,0,79,81,1,0,0,0,80,82,5,20,0,0,81,
-        80,1,0,0,0,81,82,1,0,0,0,82,84,1,0,0,0,83,85,3,14,7,0,84,83,1,0,
-        0,0,84,85,1,0,0,0,85,3,1,0,0,0,86,88,7,1,0,0,87,89,5,77,0,0,88,87,
-        1,0,0,0,88,89,1,0,0,0,89,90,1,0,0,0,90,91,5,20,0,0,91,93,3,14,7,
-        0,92,94,5,19,0,0,93,92,1,0,0,0,93,94,1,0,0,0,94,5,1,0,0,0,95,96,
-        5,77,0,0,96,109,5,15,0,0,97,99,5,24,0,0,98,97,1,0,0,0,98,99,1,0,
-        0,0,99,100,1,0,0,0,100,102,3,14,7,0,101,103,5,24,0,0,102,101,1,0,
-        0,0,102,103,1,0,0,0,103,105,1,0,0,0,104,106,5,21,0,0,105,104,1,0,
-        0,0,105,106,1,0,0,0,106,108,1,0,0,0,107,98,1,0,0,0,108,111,1,0,0,
-        0,109,107,1,0,0,0,109,110,1,0,0,0,110,112,1,0,0,0,111,109,1,0,0,
-        0,112,136,5,16,0,0,113,114,5,77,0,0,114,120,5,15,0,0,115,116,5,77,
-        0,0,116,117,5,20,0,0,117,119,5,77,0,0,118,115,1,0,0,0,119,122,1,
-        0,0,0,120,118,1,0,0,0,120,121,1,0,0,0,121,123,1,0,0,0,122,120,1,
-        0,0,0,123,136,5,16,0,0,124,131,5,15,0,0,125,127,5,78,0,0,126,128,
-        5,21,0,0,127,126,1,0,0,0,127,128,1,0,0,0,128,130,1,0,0,0,129,125,
-        1,0,0,0,130,133,1,0,0,0,131,129,1,0,0,0,131,132,1,0,0,0,132,134,
-        1,0,0,0,133,131,1,0,0,0,134,136,5,16,0,0,135,95,1,0,0,0,135,113,
-        1,0,0,0,135,124,1,0,0,0,136,7,1,0,0,0,137,147,5,25,0,0,138,147,5,
-        26,0,0,139,147,5,27,0,0,140,147,5,28,0,0,141,147,5,10,0,0,142,147,
-        5,11,0,0,143,147,3,10,5,0,144,147,3,12,6,0,145,147,5,42,0,0,146,
-        137,1,0,0,0,146,138,1,0,0,0,146,139,1,0,0,0,146,140,1,0,0,0,146,
-        141,1,0,0,0,146,142,1,0,0,0,146,143,1,0,0,0,146,144,1,0,0,0,146,
-        145,1,0,0,0,147,9,1,0,0,0,148,149,5,42,0,0,149,150,5,37,0,0,150,
-        151,3,8,4,0,151,152,5,39,0,0,152,169,1,0,0,0,153,154,5,43,0,0,154,
-        155,5,37,0,0,155,156,3,8,4,0,156,157,5,39,0,0,157,169,1,0,0,0,158,
-        159,5,44,0,0,159,160,5,37,0,0,160,161,3,8,4,0,161,162,5,39,0,0,162,
-        169,1,0,0,0,163,164,5,45,0,0,164,165,5,37,0,0,165,166,3,8,4,0,166,
-        167,5,39,0,0,167,169,1,0,0,0,168,148,1,0,0,0,168,153,1,0,0,0,168,
-        158,1,0,0,0,168,163,1,0,0,0,169,11,1,0,0,0,170,171,5,77,0,0,171,
-        13,1,0,0,0,172,174,7,2,0,0,173,172,1,0,0,0,173,174,1,0,0,0,174,175,
-        1,0,0,0,175,177,3,16,8,0,176,178,3,14,7,0,177,176,1,0,0,0,177,178,
-        1,0,0,0,178,884,1,0,0,0,179,181,3,18,9,0,180,182,3,14,7,0,181,180,
-        1,0,0,0,181,182,1,0,0,0,182,884,1,0,0,0,183,184,5,29,0,0,184,185,
-        3,14,7,0,185,186,5,30,0,0,186,187,3,14,7,0,187,188,5,31,0,0,188,
-        189,3,14,7,0,189,190,5,32,0,0,190,884,1,0,0,0,191,196,3,24,12,0,
-        192,193,5,22,0,0,193,195,5,77,0,0,194,192,1,0,0,0,195,198,1,0,0,
-        0,196,194,1,0,0,0,196,197,1,0,0,0,197,199,1,0,0,0,198,196,1,0,0,
-        0,199,200,5,22,0,0,200,201,5,53,0,0,201,202,5,15,0,0,202,203,3,8,
-        4,0,203,205,5,16,0,0,204,206,3,14,7,0,205,204,1,0,0,0,205,206,1,
-        0,0,0,206,884,1,0,0,0,207,212,3,24,12,0,208,209,5,22,0,0,209,211,
-        5,77,0,0,210,208,1,0,0,0,211,214,1,0,0,0,212,210,1,0,0,0,212,213,
-        1,0,0,0,213,215,1,0,0,0,214,212,1,0,0,0,215,216,5,22,0,0,216,217,
-        5,52,0,0,217,218,5,15,0,0,218,219,3,8,4,0,219,221,5,16,0,0,220,222,
-        3,14,7,0,221,220,1,0,0,0,221,222,1,0,0,0,222,884,1,0,0,0,223,228,
-        3,24,12,0,224,225,5,22,0,0,225,227,5,77,0,0,226,224,1,0,0,0,227,
-        230,1,0,0,0,228,226,1,0,0,0,228,229,1,0,0,0,229,231,1,0,0,0,230,
-        228,1,0,0,0,231,232,5,22,0,0,232,233,5,54,0,0,233,234,5,15,0,0,234,
-        235,3,8,4,0,235,237,5,16,0,0,236,238,3,14,7,0,237,236,1,0,0,0,237,
-        238,1,0,0,0,238,884,1,0,0,0,239,241,3,24,12,0,240,239,1,0,0,0,240,
-        241,1,0,0,0,241,246,1,0,0,0,242,243,5,22,0,0,243,245,5,77,0,0,244,
-        242,1,0,0,0,245,248,1,0,0,0,246,244,1,0,0,0,246,247,1,0,0,0,247,
-        249,1,0,0,0,248,246,1,0,0,0,249,250,5,75,0,0,250,251,5,56,0,0,251,
-        252,5,15,0,0,252,254,5,16,0,0,253,255,3,14,7,0,254,253,1,0,0,0,254,
-        255,1,0,0,0,255,259,1,0,0,0,256,258,5,16,0,0,257,256,1,0,0,0,258,
-        261,1,0,0,0,259,257,1,0,0,0,259,260,1,0,0,0,260,884,1,0,0,0,261,
-        259,1,0,0,0,262,264,3,24,12,0,263,262,1,0,0,0,263,264,1,0,0,0,264,
-        269,1,0,0,0,265,266,5,22,0,0,266,268,5,77,0,0,267,265,1,0,0,0,268,
-        271,1,0,0,0,269,267,1,0,0,0,269,270,1,0,0,0,270,272,1,0,0,0,271,
-        269,1,0,0,0,272,273,5,75,0,0,273,274,5,57,0,0,274,275,5,15,0,0,275,
-        277,5,16,0,0,276,278,3,14,7,0,277,276,1,0,0,0,277,278,1,0,0,0,278,
-        282,1,0,0,0,279,281,5,16,0,0,280,279,1,0,0,0,281,284,1,0,0,0,282,
-        280,1,0,0,0,282,283,1,0,0,0,283,884,1,0,0,0,284,282,1,0,0,0,285,
-        287,3,24,12,0,286,285,1,0,0,0,286,287,1,0,0,0,287,292,1,0,0,0,288,
-        289,5,22,0,0,289,291,5,77,0,0,290,288,1,0,0,0,291,294,1,0,0,0,292,
-        290,1,0,0,0,292,293,1,0,0,0,293,295,1,0,0,0,294,292,1,0,0,0,295,
-        296,5,75,0,0,296,297,5,58,0,0,297,298,5,15,0,0,298,300,5,16,0,0,
-        299,301,3,14,7,0,300,299,1,0,0,0,300,301,1,0,0,0,301,305,1,0,0,0,
-        302,304,5,16,0,0,303,302,1,0,0,0,304,307,1,0,0,0,305,303,1,0,0,0,
-        305,306,1,0,0,0,306,884,1,0,0,0,307,305,1,0,0,0,308,310,5,75,0,0,
-        309,308,1,0,0,0,309,310,1,0,0,0,310,311,1,0,0,0,311,312,5,59,0,0,
-        312,313,5,15,0,0,313,314,3,14,7,0,314,316,5,16,0,0,315,317,3,14,
-        7,0,316,315,1,0,0,0,316,317,1,0,0,0,317,321,1,0,0,0,318,320,5,16,
-        0,0,319,318,1,0,0,0,320,323,1,0,0,0,321,319,1,0,0,0,321,322,1,0,
-        0,0,322,884,1,0,0,0,323,321,1,0,0,0,324,326,5,75,0,0,325,324,1,0,
-        0,0,325,326,1,0,0,0,326,327,1,0,0,0,327,328,5,60,0,0,328,329,5,15,
-        0,0,329,330,3,14,7,0,330,332,5,16,0,0,331,333,3,14,7,0,332,331,1,
-        0,0,0,332,333,1,0,0,0,333,337,1,0,0,0,334,336,5,16,0,0,335,334,1,
-        0,0,0,336,339,1,0,0,0,337,335,1,0,0,0,337,338,1,0,0,0,338,884,1,
-        0,0,0,339,337,1,0,0,0,340,342,5,75,0,0,341,340,1,0,0,0,341,342,1,
-        0,0,0,342,346,1,0,0,0,343,345,5,15,0,0,344,343,1,0,0,0,345,348,1,
-        0,0,0,346,344,1,0,0,0,346,347,1,0,0,0,347,349,1,0,0,0,348,346,1,
-        0,0,0,349,353,5,44,0,0,350,352,5,17,0,0,351,350,1,0,0,0,352,355,
-        1,0,0,0,353,351,1,0,0,0,353,354,1,0,0,0,354,359,1,0,0,0,355,353,
-        1,0,0,0,356,358,5,15,0,0,357,356,1,0,0,0,358,361,1,0,0,0,359,357,
-        1,0,0,0,359,360,1,0,0,0,360,374,1,0,0,0,361,359,1,0,0,0,362,364,
-        5,24,0,0,363,362,1,0,0,0,363,364,1,0,0,0,364,365,1,0,0,0,365,367,
-        3,14,7,0,366,368,5,24,0,0,367,366,1,0,0,0,367,368,1,0,0,0,368,370,
-        1,0,0,0,369,371,5,21,0,0,370,369,1,0,0,0,370,371,1,0,0,0,371,373,
-        1,0,0,0,372,363,1,0,0,0,373,376,1,0,0,0,374,372,1,0,0,0,374,375,
-        1,0,0,0,375,380,1,0,0,0,376,374,1,0,0,0,377,379,5,18,0,0,378,377,
-        1,0,0,0,379,382,1,0,0,0,380,378,1,0,0,0,380,381,1,0,0,0,381,386,
-        1,0,0,0,382,380,1,0,0,0,383,385,5,16,0,0,384,383,1,0,0,0,385,388,
-        1,0,0,0,386,384,1,0,0,0,386,387,1,0,0,0,387,390,1,0,0,0,388,386,
-        1,0,0,0,389,391,3,14,7,0,390,389,1,0,0,0,390,391,1,0,0,0,391,884,
-        1,0,0,0,392,394,5,75,0,0,393,392,1,0,0,0,393,394,1,0,0,0,394,398,
-        1,0,0,0,395,397,5,15,0,0,396,395,1,0,0,0,397,400,1,0,0,0,398,396,
-        1,0,0,0,398,399,1,0,0,0,399,401,1,0,0,0,400,398,1,0,0,0,401,405,
-        5,61,0,0,402,404,5,17,0,0,403,402,1,0,0,0,404,407,1,0,0,0,405,403,
-        1,0,0,0,405,406,1,0,0,0,406,411,1,0,0,0,407,405,1,0,0,0,408,410,
-        5,15,0,0,409,408,1,0,0,0,410,413,1,0,0,0,411,409,1,0,0,0,411,412,
-        1,0,0,0,412,426,1,0,0,0,413,411,1,0,0,0,414,416,5,24,0,0,415,414,
-        1,0,0,0,415,416,1,0,0,0,416,417,1,0,0,0,417,419,3,14,7,0,418,420,
-        5,24,0,0,419,418,1,0,0,0,419,420,1,0,0,0,420,422,1,0,0,0,421,423,
-        5,21,0,0,422,421,1,0,0,0,422,423,1,0,0,0,423,425,1,0,0,0,424,415,
-        1,0,0,0,425,428,1,0,0,0,426,424,1,0,0,0,426,427,1,0,0,0,427,432,
-        1,0,0,0,428,426,1,0,0,0,429,431,5,16,0,0,430,429,1,0,0,0,431,434,
-        1,0,0,0,432,430,1,0,0,0,432,433,1,0,0,0,433,438,1,0,0,0,434,432,
-        1,0,0,0,435,437,5,18,0,0,436,435,1,0,0,0,437,440,1,0,0,0,438,436,
-        1,0,0,0,438,439,1,0,0,0,439,442,1,0,0,0,440,438,1,0,0,0,441,443,
-        3,14,7,0,442,441,1,0,0,0,442,443,1,0,0,0,443,884,1,0,0,0,444,446,
-        5,75,0,0,445,444,1,0,0,0,445,446,1,0,0,0,446,447,1,0,0,0,447,449,
-        5,55,0,0,448,450,5,15,0,0,449,448,1,0,0,0,450,451,1,0,0,0,451,449,
-        1,0,0,0,451,452,1,0,0,0,452,453,1,0,0,0,453,455,3,14,7,0,454,456,
-        5,16,0,0,455,454,1,0,0,0,456,457,1,0,0,0,457,455,1,0,0,0,457,458,
-        1,0,0,0,458,460,1,0,0,0,459,461,3,14,7,0,460,459,1,0,0,0,460,461,
-        1,0,0,0,461,884,1,0,0,0,462,464,5,75,0,0,463,462,1,0,0,0,463,464,
-        1,0,0,0,464,468,1,0,0,0,465,467,5,15,0,0,466,465,1,0,0,0,467,470,
-        1,0,0,0,468,466,1,0,0,0,468,469,1,0,0,0,469,471,1,0,0,0,470,468,
-        1,0,0,0,471,472,5,45,0,0,472,485,5,17,0,0,473,475,5,24,0,0,474,473,
-        1,0,0,0,474,475,1,0,0,0,475,476,1,0,0,0,476,478,3,14,7,0,477,479,
-        5,24,0,0,478,477,1,0,0,0,478,479,1,0,0,0,479,481,1,0,0,0,480,482,
-        5,21,0,0,481,480,1,0,0,0,481,482,1,0,0,0,482,484,1,0,0,0,483,474,
-        1,0,0,0,484,487,1,0,0,0,485,483,1,0,0,0,485,486,1,0,0,0,486,488,
-        1,0,0,0,487,485,1,0,0,0,488,492,5,18,0,0,489,491,5,16,0,0,490,489,
-        1,0,0,0,491,494,1,0,0,0,492,490,1,0,0,0,492,493,1,0,0,0,493,496,
-        1,0,0,0,494,492,1,0,0,0,495,497,3,14,7,0,496,495,1,0,0,0,496,497,
-        1,0,0,0,497,884,1,0,0,0,498,500,5,75,0,0,499,498,1,0,0,0,499,500,
-        1,0,0,0,500,504,1,0,0,0,501,503,5,15,0,0,502,501,1,0,0,0,503,506,
-        1,0,0,0,504,502,1,0,0,0,504,505,1,0,0,0,505,507,1,0,0,0,506,504,
-        1,0,0,0,507,511,5,62,0,0,508,510,5,17,0,0,509,508,1,0,0,0,510,513,
-        1,0,0,0,511,509,1,0,0,0,511,512,1,0,0,0,512,517,1,0,0,0,513,511,
-        1,0,0,0,514,516,5,15,0,0,515,514,1,0,0,0,516,519,1,0,0,0,517,515,
-        1,0,0,0,517,518,1,0,0,0,518,532,1,0,0,0,519,517,1,0,0,0,520,522,
-        5,24,0,0,521,520,1,0,0,0,521,522,1,0,0,0,522,523,1,0,0,0,523,525,
-        3,14,7,0,524,526,5,24,0,0,525,524,1,0,0,0,525,526,1,0,0,0,526,528,
-        1,0,0,0,527,529,5,21,0,0,528,527,1,0,0,0,528,529,1,0,0,0,529,531,
-        1,0,0,0,530,521,1,0,0,0,531,534,1,0,0,0,532,530,1,0,0,0,532,533,
-        1,0,0,0,533,538,1,0,0,0,534,532,1,0,0,0,535,537,5,18,0,0,536,535,
-        1,0,0,0,537,540,1,0,0,0,538,536,1,0,0,0,538,539,1,0,0,0,539,544,
-        1,0,0,0,540,538,1,0,0,0,541,543,5,16,0,0,542,541,1,0,0,0,543,546,
-        1,0,0,0,544,542,1,0,0,0,544,545,1,0,0,0,545,548,1,0,0,0,546,544,
-        1,0,0,0,547,549,3,14,7,0,548,547,1,0,0,0,548,549,1,0,0,0,549,550,
-        1,0,0,0,550,884,5,16,0,0,551,553,5,75,0,0,552,551,1,0,0,0,552,553,
-        1,0,0,0,553,557,1,0,0,0,554,556,5,15,0,0,555,554,1,0,0,0,556,559,
-        1,0,0,0,557,555,1,0,0,0,557,558,1,0,0,0,558,560,1,0,0,0,559,557,
-        1,0,0,0,560,564,5,42,0,0,561,563,5,15,0,0,562,561,1,0,0,0,563,566,
-        1,0,0,0,564,562,1,0,0,0,564,565,1,0,0,0,565,570,1,0,0,0,566,564,
-        1,0,0,0,567,569,5,17,0,0,568,567,1,0,0,0,569,572,1,0,0,0,570,568,
-        1,0,0,0,570,571,1,0,0,0,571,585,1,0,0,0,572,570,1,0,0,0,573,575,
-        5,24,0,0,574,573,1,0,0,0,574,575,1,0,0,0,575,576,1,0,0,0,576,578,
-        3,14,7,0,577,579,5,24,0,0,578,577,1,0,0,0,578,579,1,0,0,0,579,581,
-        1,0,0,0,580,582,5,21,0,0,581,580,1,0,0,0,581,582,1,0,0,0,582,584,
-        1,0,0,0,583,574,1,0,0,0,584,587,1,0,0,0,585,583,1,0,0,0,585,586,
-        1,0,0,0,586,591,1,0,0,0,587,585,1,0,0,0,588,590,5,18,0,0,589,588,
-        1,0,0,0,590,593,1,0,0,0,591,589,1,0,0,0,591,592,1,0,0,0,592,597,
-        1,0,0,0,593,591,1,0,0,0,594,596,5,16,0,0,595,594,1,0,0,0,596,599,
-        1,0,0,0,597,595,1,0,0,0,597,598,1,0,0,0,598,601,1,0,0,0,599,597,
-        1,0,0,0,600,602,3,14,7,0,601,600,1,0,0,0,601,602,1,0,0,0,602,884,
-        1,0,0,0,603,605,5,75,0,0,604,603,1,0,0,0,604,605,1,0,0,0,605,609,
-        1,0,0,0,606,608,5,15,0,0,607,606,1,0,0,0,608,611,1,0,0,0,609,607,
-        1,0,0,0,609,610,1,0,0,0,610,612,1,0,0,0,611,609,1,0,0,0,612,616,
-        5,43,0,0,613,615,5,15,0,0,614,613,1,0,0,0,615,618,1,0,0,0,616,614,
-        1,0,0,0,616,617,1,0,0,0,617,622,1,0,0,0,618,616,1,0,0,0,619,621,
-        5,17,0,0,620,619,1,0,0,0,621,624,1,0,0,0,622,620,1,0,0,0,622,623,
-        1,0,0,0,623,637,1,0,0,0,624,622,1,0,0,0,625,627,5,24,0,0,626,625,
-        1,0,0,0,626,627,1,0,0,0,627,628,1,0,0,0,628,630,3,14,7,0,629,631,
-        5,24,0,0,630,629,1,0,0,0,630,631,1,0,0,0,631,633,1,0,0,0,632,634,
-        5,21,0,0,633,632,1,0,0,0,633,634,1,0,0,0,634,636,1,0,0,0,635,626,
-        1,0,0,0,636,639,1,0,0,0,637,635,1,0,0,0,637,638,1,0,0,0,638,643,
-        1,0,0,0,639,637,1,0,0,0,640,642,5,18,0,0,641,640,1,0,0,0,642,645,
-        1,0,0,0,643,641,1,0,0,0,643,644,1,0,0,0,644,649,1,0,0,0,645,643,
-        1,0,0,0,646,648,5,16,0,0,647,646,1,0,0,0,648,651,1,0,0,0,649,647,
-        1,0,0,0,649,650,1,0,0,0,650,653,1,0,0,0,651,649,1,0,0,0,652,654,
-        3,14,7,0,653,652,1,0,0,0,653,654,1,0,0,0,654,884,1,0,0,0,655,656,
-        5,75,0,0,656,658,5,63,0,0,657,659,5,15,0,0,658,657,1,0,0,0,659,660,
-        1,0,0,0,660,658,1,0,0,0,660,661,1,0,0,0,661,674,1,0,0,0,662,664,
-        5,24,0,0,663,662,1,0,0,0,663,664,1,0,0,0,664,665,1,0,0,0,665,667,
-        3,14,7,0,666,668,5,24,0,0,667,666,1,0,0,0,667,668,1,0,0,0,668,670,
-        1,0,0,0,669,671,5,21,0,0,670,669,1,0,0,0,670,671,1,0,0,0,671,673,
-        1,0,0,0,672,663,1,0,0,0,673,676,1,0,0,0,674,672,1,0,0,0,674,675,
-        1,0,0,0,675,678,1,0,0,0,676,674,1,0,0,0,677,679,5,16,0,0,678,677,
-        1,0,0,0,679,680,1,0,0,0,680,678,1,0,0,0,680,681,1,0,0,0,681,683,
-        1,0,0,0,682,684,3,14,7,0,683,682,1,0,0,0,683,684,1,0,0,0,684,884,
-        1,0,0,0,685,686,5,75,0,0,686,687,5,64,0,0,687,689,5,15,0,0,688,690,
-        5,16,0,0,689,688,1,0,0,0,690,691,1,0,0,0,691,689,1,0,0,0,691,692,
-        1,0,0,0,692,694,1,0,0,0,693,695,3,14,7,0,694,693,1,0,0,0,694,695,
-        1,0,0,0,695,884,1,0,0,0,696,697,5,75,0,0,697,698,5,65,0,0,698,711,
-        5,15,0,0,699,701,5,24,0,0,700,699,1,0,0,0,700,701,1,0,0,0,701,702,
-        1,0,0,0,702,704,3,14,7,0,703,705,5,24,0,0,704,703,1,0,0,0,704,705,
-        1,0,0,0,705,707,1,0,0,0,706,708,5,21,0,0,707,706,1,0,0,0,707,708,
-        1,0,0,0,708,710,1,0,0,0,709,700,1,0,0,0,710,713,1,0,0,0,711,709,
-        1,0,0,0,711,712,1,0,0,0,712,715,1,0,0,0,713,711,1,0,0,0,714,716,
-        5,16,0,0,715,714,1,0,0,0,716,717,1,0,0,0,717,715,1,0,0,0,717,718,
-        1,0,0,0,718,720,1,0,0,0,719,721,3,14,7,0,720,719,1,0,0,0,720,721,
-        1,0,0,0,721,884,1,0,0,0,722,724,5,75,0,0,723,722,1,0,0,0,723,724,
-        1,0,0,0,724,725,1,0,0,0,725,726,7,3,0,0,726,735,5,15,0,0,727,730,
-        5,77,0,0,728,729,5,20,0,0,729,731,5,77,0,0,730,728,1,0,0,0,730,731,
-        1,0,0,0,731,733,1,0,0,0,732,734,5,21,0,0,733,732,1,0,0,0,733,734,
-        1,0,0,0,734,736,1,0,0,0,735,727,1,0,0,0,736,737,1,0,0,0,737,735,
-        1,0,0,0,737,738,1,0,0,0,738,739,1,0,0,0,739,740,5,41,0,0,740,741,
-        3,14,7,0,741,743,5,16,0,0,742,744,3,14,7,0,743,742,1,0,0,0,743,744,
-        1,0,0,0,744,884,1,0,0,0,745,747,5,75,0,0,746,745,1,0,0,0,746,747,
-        1,0,0,0,747,748,1,0,0,0,748,749,7,3,0,0,749,750,5,15,0,0,750,751,
-        3,14,7,0,751,753,5,16,0,0,752,754,3,14,7,0,753,752,1,0,0,0,753,754,
-        1,0,0,0,754,884,1,0,0,0,755,756,5,75,0,0,756,757,5,66,0,0,757,758,
-        5,15,0,0,758,760,3,14,7,0,759,761,5,16,0,0,760,759,1,0,0,0,761,762,
-        1,0,0,0,762,760,1,0,0,0,762,763,1,0,0,0,763,765,1,0,0,0,764,766,
-        3,14,7,0,765,764,1,0,0,0,765,766,1,0,0,0,766,884,1,0,0,0,767,768,
-        5,75,0,0,768,769,5,67,0,0,769,770,5,15,0,0,770,772,5,16,0,0,771,
-        773,3,14,7,0,772,771,1,0,0,0,772,773,1,0,0,0,773,884,1,0,0,0,774,
-        775,5,75,0,0,775,776,5,68,0,0,776,777,5,15,0,0,777,779,5,16,0,0,
-        778,780,3,14,7,0,779,778,1,0,0,0,779,780,1,0,0,0,780,884,1,0,0,0,
-        781,782,5,75,0,0,782,783,5,71,0,0,783,784,5,15,0,0,784,785,3,14,
-        7,0,785,787,5,16,0,0,786,788,3,14,7,0,787,786,1,0,0,0,787,788,1,
-        0,0,0,788,884,1,0,0,0,789,790,5,76,0,0,790,791,5,20,0,0,791,884,
-        3,14,7,0,792,793,5,77,0,0,793,794,5,20,0,0,794,795,5,77,0,0,795,
-        796,5,23,0,0,796,884,3,14,7,0,797,799,5,15,0,0,798,797,1,0,0,0,799,
-        802,1,0,0,0,800,798,1,0,0,0,800,801,1,0,0,0,801,804,1,0,0,0,802,
-        800,1,0,0,0,803,805,3,24,12,0,804,803,1,0,0,0,804,805,1,0,0,0,805,
-        810,1,0,0,0,806,807,5,22,0,0,807,809,5,77,0,0,808,806,1,0,0,0,809,
-        812,1,0,0,0,810,808,1,0,0,0,810,811,1,0,0,0,811,814,1,0,0,0,812,
-        810,1,0,0,0,813,815,3,20,10,0,814,813,1,0,0,0,814,815,1,0,0,0,815,
-        817,1,0,0,0,816,818,3,24,12,0,817,816,1,0,0,0,817,818,1,0,0,0,818,
-        821,1,0,0,0,819,820,5,22,0,0,820,822,5,77,0,0,821,819,1,0,0,0,822,
-        823,1,0,0,0,823,821,1,0,0,0,823,824,1,0,0,0,824,826,1,0,0,0,825,
-        827,3,14,7,0,826,825,1,0,0,0,826,827,1,0,0,0,827,884,1,0,0,0,828,
-        832,3,24,12,0,829,831,5,22,0,0,830,829,1,0,0,0,831,834,1,0,0,0,832,
-        830,1,0,0,0,832,833,1,0,0,0,833,838,1,0,0,0,834,832,1,0,0,0,835,
-        837,5,77,0,0,836,835,1,0,0,0,837,840,1,0,0,0,838,836,1,0,0,0,838,
-        839,1,0,0,0,839,841,1,0,0,0,840,838,1,0,0,0,841,843,3,6,3,0,842,
-        844,3,20,10,0,843,842,1,0,0,0,843,844,1,0,0,0,844,846,1,0,0,0,845,
-        847,3,14,7,0,846,845,1,0,0,0,846,847,1,0,0,0,847,884,1,0,0,0,848,
-        850,3,20,10,0,849,851,3,22,11,0,850,849,1,0,0,0,850,851,1,0,0,0,
-        851,884,1,0,0,0,852,853,5,75,0,0,853,884,3,14,7,0,854,856,5,78,0,
-        0,855,857,3,14,7,0,856,855,1,0,0,0,856,857,1,0,0,0,857,884,1,0,0,
-        0,858,860,5,75,0,0,859,858,1,0,0,0,859,860,1,0,0,0,860,861,1,0,0,
-        0,861,863,3,6,3,0,862,864,3,14,7,0,863,862,1,0,0,0,863,864,1,0,0,
-        0,864,884,1,0,0,0,865,867,3,24,12,0,866,868,3,14,7,0,867,866,1,0,
-        0,0,867,868,1,0,0,0,868,884,1,0,0,0,869,870,5,24,0,0,870,872,3,14,
-        7,0,871,873,5,22,0,0,872,871,1,0,0,0,872,873,1,0,0,0,873,874,1,0,
-        0,0,874,876,5,24,0,0,875,877,5,22,0,0,876,875,1,0,0,0,876,877,1,
-        0,0,0,877,879,1,0,0,0,878,880,3,14,7,0,879,878,1,0,0,0,879,880,1,
-        0,0,0,880,884,1,0,0,0,881,882,5,13,0,0,882,884,3,14,7,0,883,173,
-        1,0,0,0,883,179,1,0,0,0,883,183,1,0,0,0,883,191,1,0,0,0,883,207,
-        1,0,0,0,883,223,1,0,0,0,883,240,1,0,0,0,883,263,1,0,0,0,883,286,
-        1,0,0,0,883,309,1,0,0,0,883,325,1,0,0,0,883,341,1,0,0,0,883,393,
-        1,0,0,0,883,445,1,0,0,0,883,463,1,0,0,0,883,499,1,0,0,0,883,552,
-        1,0,0,0,883,604,1,0,0,0,883,655,1,0,0,0,883,685,1,0,0,0,883,696,
-        1,0,0,0,883,723,1,0,0,0,883,746,1,0,0,0,883,755,1,0,0,0,883,767,
-        1,0,0,0,883,774,1,0,0,0,883,781,1,0,0,0,883,789,1,0,0,0,883,792,
-        1,0,0,0,883,800,1,0,0,0,883,828,1,0,0,0,883,848,1,0,0,0,883,852,
-        1,0,0,0,883,854,1,0,0,0,883,859,1,0,0,0,883,865,1,0,0,0,883,869,
-        1,0,0,0,883,881,1,0,0,0,884,15,1,0,0,0,885,890,3,24,12,0,886,887,
-        5,22,0,0,887,889,5,77,0,0,888,886,1,0,0,0,889,892,1,0,0,0,890,888,
-        1,0,0,0,890,891,1,0,0,0,891,895,1,0,0,0,892,890,1,0,0,0,893,895,
-        5,78,0,0,894,885,1,0,0,0,894,893,1,0,0,0,895,900,1,0,0,0,896,897,
-        5,22,0,0,897,899,5,77,0,0,898,896,1,0,0,0,899,902,1,0,0,0,900,898,
-        1,0,0,0,900,901,1,0,0,0,901,903,1,0,0,0,902,900,1,0,0,0,903,913,
-        3,20,10,0,904,909,3,24,12,0,905,906,5,22,0,0,906,908,5,77,0,0,907,
-        905,1,0,0,0,908,911,1,0,0,0,909,907,1,0,0,0,909,910,1,0,0,0,910,
-        914,1,0,0,0,911,909,1,0,0,0,912,914,5,78,0,0,913,904,1,0,0,0,913,
-        912,1,0,0,0,914,17,1,0,0,0,915,916,7,4,0,0,916,917,3,14,7,0,917,
-        19,1,0,0,0,918,919,7,5,0,0,919,21,1,0,0,0,920,935,5,78,0,0,921,923,
-        5,24,0,0,922,921,1,0,0,0,922,923,1,0,0,0,923,924,1,0,0,0,924,926,
-        5,77,0,0,925,927,5,15,0,0,926,925,1,0,0,0,926,927,1,0,0,0,927,929,
-        1,0,0,0,928,930,5,16,0,0,929,928,1,0,0,0,929,930,1,0,0,0,930,932,
-        1,0,0,0,931,933,5,24,0,0,932,931,1,0,0,0,932,933,1,0,0,0,933,935,
-        1,0,0,0,934,920,1,0,0,0,934,922,1,0,0,0,935,23,1,0,0,0,936,945,3,
-        26,13,0,937,945,5,5,0,0,938,945,3,6,3,0,939,940,5,15,0,0,940,941,
-        3,14,7,0,941,942,5,16,0,0,942,945,1,0,0,0,943,945,5,77,0,0,944,936,
-        1,0,0,0,944,937,1,0,0,0,944,938,1,0,0,0,944,939,1,0,0,0,944,943,
-        1,0,0,0,945,25,1,0,0,0,946,947,7,6,0,0,947,27,1,0,0,0,180,32,39,
-        42,47,51,54,57,60,63,66,69,72,75,78,81,84,88,93,98,102,105,109,120,
-        127,131,135,146,168,173,177,181,196,205,212,221,228,237,240,246,
-        254,259,263,269,277,282,286,292,300,305,309,316,321,325,332,337,
-        341,346,353,359,363,367,370,374,380,386,390,393,398,405,411,415,
-        419,422,426,432,438,442,445,451,457,460,463,468,474,478,481,485,
-        492,496,499,504,511,517,521,525,528,532,538,544,548,552,557,564,
-        570,574,578,581,585,591,597,601,604,609,616,622,626,630,633,637,
-        643,649,653,660,663,667,670,674,680,683,691,694,700,704,707,711,
-        717,720,723,730,733,737,743,746,753,762,765,772,779,787,800,804,
-        810,814,817,823,826,832,838,843,846,850,856,859,863,867,872,876,
-        879,883,890,894,900,909,913,922,926,929,932,934,944
+        2,14,7,14,2,15,7,15,1,0,1,0,5,0,35,8,0,10,0,12,0,38,9,0,1,1,1,1,
+        1,1,1,1,3,1,44,8,1,1,1,3,1,47,8,1,1,1,5,1,50,8,1,10,1,12,1,53,9,
+        1,1,1,3,1,56,8,1,1,1,3,1,59,8,1,1,1,3,1,62,8,1,1,1,3,1,65,8,1,1,
+        1,3,1,68,8,1,1,1,3,1,71,8,1,1,1,3,1,74,8,1,1,1,3,1,77,8,1,1,1,3,
+        1,80,8,1,1,1,3,1,83,8,1,1,1,3,1,86,8,1,1,1,3,1,89,8,1,1,2,1,2,3,
+        2,93,8,2,1,2,1,2,1,2,3,2,98,8,2,1,3,1,3,1,3,3,3,103,8,3,1,3,1,3,
+        3,3,107,8,3,1,3,3,3,110,8,3,5,3,112,8,3,10,3,12,3,115,9,3,1,3,1,
+        3,1,3,1,3,1,3,1,3,5,3,123,8,3,10,3,12,3,126,9,3,1,3,1,3,1,3,1,3,
+        3,3,132,8,3,5,3,134,8,3,10,3,12,3,137,9,3,1,3,3,3,140,8,3,1,4,1,
+        4,1,4,1,4,1,4,1,4,1,4,1,4,1,4,3,4,151,8,4,1,5,1,5,1,5,1,5,1,5,1,
+        5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,1,5,3,5,173,
+        8,5,1,6,1,6,1,7,3,7,178,8,7,1,7,1,7,3,7,182,8,7,1,7,1,7,3,7,186,
+        8,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,3,7,196,8,7,1,7,1,7,1,7,5,7,
+        201,8,7,10,7,12,7,204,9,7,1,7,1,7,1,7,1,7,1,7,1,7,3,7,212,8,7,1,
+        7,1,7,1,7,5,7,217,8,7,10,7,12,7,220,9,7,1,7,1,7,1,7,1,7,1,7,1,7,
+        3,7,228,8,7,1,7,1,7,1,7,5,7,233,8,7,10,7,12,7,236,9,7,1,7,1,7,1,
+        7,1,7,1,7,1,7,3,7,244,8,7,1,7,3,7,247,8,7,1,7,1,7,5,7,251,8,7,10,
+        7,12,7,254,9,7,1,7,1,7,1,7,1,7,1,7,3,7,261,8,7,1,7,5,7,264,8,7,10,
+        7,12,7,267,9,7,1,7,3,7,270,8,7,1,7,1,7,5,7,274,8,7,10,7,12,7,277,
+        9,7,1,7,1,7,1,7,1,7,1,7,3,7,284,8,7,1,7,3,7,287,8,7,1,7,5,7,290,
+        8,7,10,7,12,7,293,9,7,1,7,3,7,296,8,7,1,7,1,7,5,7,300,8,7,10,7,12,
+        7,303,9,7,1,7,1,7,1,7,1,7,1,7,3,7,310,8,7,1,7,3,7,313,8,7,1,7,5,
+        7,316,8,7,10,7,12,7,319,9,7,1,7,3,7,322,8,7,1,7,1,7,1,7,1,7,1,7,
+        3,7,329,8,7,1,7,5,7,332,8,7,10,7,12,7,335,9,7,1,7,3,7,338,8,7,1,
+        7,1,7,1,7,1,7,1,7,3,7,345,8,7,1,7,5,7,348,8,7,10,7,12,7,351,9,7,
+        1,7,3,7,354,8,7,1,7,5,7,357,8,7,10,7,12,7,360,9,7,1,7,1,7,5,7,364,
+        8,7,10,7,12,7,367,9,7,1,7,5,7,370,8,7,10,7,12,7,373,9,7,1,7,3,7,
+        376,8,7,1,7,1,7,3,7,380,8,7,1,7,3,7,383,8,7,5,7,385,8,7,10,7,12,
+        7,388,9,7,1,7,5,7,391,8,7,10,7,12,7,394,9,7,1,7,5,7,397,8,7,10,7,
+        12,7,400,9,7,1,7,3,7,403,8,7,1,7,3,7,406,8,7,1,7,5,7,409,8,7,10,
+        7,12,7,412,9,7,1,7,1,7,5,7,416,8,7,10,7,12,7,419,9,7,1,7,5,7,422,
+        8,7,10,7,12,7,425,9,7,1,7,3,7,428,8,7,1,7,1,7,3,7,432,8,7,1,7,3,
+        7,435,8,7,5,7,437,8,7,10,7,12,7,440,9,7,1,7,5,7,443,8,7,10,7,12,
+        7,446,9,7,1,7,5,7,449,8,7,10,7,12,7,452,9,7,1,7,3,7,455,8,7,1,7,
+        3,7,458,8,7,1,7,1,7,4,7,462,8,7,11,7,12,7,463,1,7,3,7,467,8,7,1,
+        7,4,7,470,8,7,11,7,12,7,471,1,7,3,7,475,8,7,1,7,3,7,478,8,7,1,7,
+        5,7,481,8,7,10,7,12,7,484,9,7,1,7,1,7,1,7,3,7,489,8,7,1,7,1,7,3,
+        7,493,8,7,1,7,3,7,496,8,7,5,7,498,8,7,10,7,12,7,501,9,7,1,7,1,7,
+        5,7,505,8,7,10,7,12,7,508,9,7,1,7,3,7,511,8,7,1,7,3,7,514,8,7,1,
+        7,5,7,517,8,7,10,7,12,7,520,9,7,1,7,1,7,5,7,524,8,7,10,7,12,7,527,
+        9,7,1,7,5,7,530,8,7,10,7,12,7,533,9,7,1,7,3,7,536,8,7,1,7,1,7,3,
+        7,540,8,7,1,7,3,7,543,8,7,5,7,545,8,7,10,7,12,7,548,9,7,1,7,5,7,
+        551,8,7,10,7,12,7,554,9,7,1,7,5,7,557,8,7,10,7,12,7,560,9,7,1,7,
+        3,7,563,8,7,1,7,1,7,3,7,567,8,7,1,7,5,7,570,8,7,10,7,12,7,573,9,
+        7,1,7,1,7,5,7,577,8,7,10,7,12,7,580,9,7,1,7,5,7,583,8,7,10,7,12,
+        7,586,9,7,1,7,3,7,589,8,7,1,7,1,7,3,7,593,8,7,1,7,3,7,596,8,7,5,
+        7,598,8,7,10,7,12,7,601,9,7,1,7,5,7,604,8,7,10,7,12,7,607,9,7,1,
+        7,5,7,610,8,7,10,7,12,7,613,9,7,1,7,3,7,616,8,7,1,7,3,7,619,8,7,
+        1,7,5,7,622,8,7,10,7,12,7,625,9,7,1,7,1,7,5,7,629,8,7,10,7,12,7,
+        632,9,7,1,7,5,7,635,8,7,10,7,12,7,638,9,7,1,7,3,7,641,8,7,1,7,1,
+        7,3,7,645,8,7,1,7,3,7,648,8,7,5,7,650,8,7,10,7,12,7,653,9,7,1,7,
+        5,7,656,8,7,10,7,12,7,659,9,7,1,7,5,7,662,8,7,10,7,12,7,665,9,7,
+        1,7,3,7,668,8,7,1,7,1,7,1,7,4,7,673,8,7,11,7,12,7,674,1,7,3,7,678,
+        8,7,1,7,1,7,3,7,682,8,7,1,7,3,7,685,8,7,5,7,687,8,7,10,7,12,7,690,
+        9,7,1,7,4,7,693,8,7,11,7,12,7,694,1,7,3,7,698,8,7,1,7,1,7,1,7,1,
+        7,4,7,704,8,7,11,7,12,7,705,1,7,3,7,709,8,7,1,7,1,7,1,7,1,7,3,7,
+        715,8,7,1,7,1,7,3,7,719,8,7,1,7,3,7,722,8,7,5,7,724,8,7,10,7,12,
+        7,727,9,7,1,7,4,7,730,8,7,11,7,12,7,731,1,7,3,7,735,8,7,1,7,3,7,
+        738,8,7,1,7,1,7,1,7,1,7,1,7,3,7,745,8,7,1,7,3,7,748,8,7,4,7,750,
+        8,7,11,7,12,7,751,1,7,1,7,1,7,1,7,3,7,758,8,7,1,7,3,7,761,8,7,1,
+        7,1,7,1,7,1,7,1,7,3,7,768,8,7,1,7,1,7,1,7,1,7,1,7,4,7,775,8,7,11,
+        7,12,7,776,1,7,3,7,780,8,7,1,7,1,7,1,7,1,7,1,7,3,7,787,8,7,1,7,1,
+        7,1,7,1,7,1,7,3,7,794,8,7,1,7,1,7,1,7,1,7,1,7,1,7,3,7,802,8,7,1,
+        7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,1,7,5,7,813,8,7,10,7,12,7,816,9,7,
+        1,7,3,7,819,8,7,1,7,1,7,5,7,823,8,7,10,7,12,7,826,9,7,1,7,3,7,829,
+        8,7,1,7,3,7,832,8,7,1,7,1,7,4,7,836,8,7,11,7,12,7,837,1,7,3,7,841,
+        8,7,1,7,1,7,5,7,845,8,7,10,7,12,7,848,9,7,1,7,5,7,851,8,7,10,7,12,
+        7,854,9,7,1,7,1,7,3,7,858,8,7,1,7,3,7,861,8,7,1,7,1,7,1,7,1,7,3,
+        7,867,8,7,1,7,3,7,870,8,7,1,7,1,7,3,7,874,8,7,1,7,1,7,1,7,3,7,879,
+        8,7,1,7,1,7,3,7,883,8,7,1,7,3,7,886,8,7,1,7,1,7,1,7,3,7,891,8,7,
+        1,7,3,7,894,8,7,1,7,3,7,897,8,7,1,7,1,7,1,7,1,7,3,7,903,8,7,1,7,
+        1,7,3,7,907,8,7,3,7,909,8,7,1,8,3,8,912,8,8,1,8,1,8,1,9,1,9,1,9,
+        1,9,5,9,920,8,9,10,9,12,9,923,9,9,1,9,3,9,926,8,9,1,10,1,10,1,10,
+        5,10,931,8,10,10,10,12,10,934,9,10,1,10,3,10,937,8,10,1,10,1,10,
+        5,10,941,8,10,10,10,12,10,944,9,10,1,10,1,10,1,10,1,10,5,10,950,
+        8,10,10,10,12,10,953,9,10,1,10,3,10,956,8,10,1,11,1,11,1,11,1,12,
+        1,12,1,13,1,13,3,13,965,8,13,1,13,1,13,3,13,969,8,13,1,13,3,13,972,
+        8,13,1,13,3,13,975,8,13,3,13,977,8,13,1,14,1,14,1,14,1,14,1,14,1,
+        14,1,14,1,14,3,14,987,8,14,1,15,1,15,1,15,0,0,16,0,2,4,6,8,10,12,
+        14,16,18,20,22,24,26,28,30,0,7,3,0,4,5,69,71,77,77,1,0,3,5,1,0,34,
+        35,1,0,7,10,3,0,1,1,36,36,47,49,5,0,1,1,24,24,34,35,37,41,47,52,
+        2,0,73,73,79,81,1217,0,32,1,0,0,0,2,39,1,0,0,0,4,90,1,0,0,0,6,139,
+        1,0,0,0,8,150,1,0,0,0,10,172,1,0,0,0,12,174,1,0,0,0,14,908,1,0,0,
+        0,16,911,1,0,0,0,18,915,1,0,0,0,20,936,1,0,0,0,22,957,1,0,0,0,24,
+        960,1,0,0,0,26,976,1,0,0,0,28,986,1,0,0,0,30,988,1,0,0,0,32,36,3,
+        2,1,0,33,35,3,14,7,0,34,33,1,0,0,0,35,38,1,0,0,0,36,34,1,0,0,0,36,
+        37,1,0,0,0,37,1,1,0,0,0,38,36,1,0,0,0,39,40,5,2,0,0,40,43,5,78,0,
+        0,41,42,5,21,0,0,42,44,3,8,4,0,43,41,1,0,0,0,43,44,1,0,0,0,44,46,
+        1,0,0,0,45,47,5,18,0,0,46,45,1,0,0,0,46,47,1,0,0,0,47,51,1,0,0,0,
+        48,50,3,4,2,0,49,48,1,0,0,0,50,53,1,0,0,0,51,49,1,0,0,0,51,52,1,
+        0,0,0,52,55,1,0,0,0,53,51,1,0,0,0,54,56,5,19,0,0,55,54,1,0,0,0,55,
+        56,1,0,0,0,56,58,1,0,0,0,57,59,5,15,0,0,58,57,1,0,0,0,58,59,1,0,
+        0,0,59,61,1,0,0,0,60,62,3,6,3,0,61,60,1,0,0,0,61,62,1,0,0,0,62,64,
+        1,0,0,0,63,65,5,21,0,0,64,63,1,0,0,0,64,65,1,0,0,0,65,67,1,0,0,0,
+        66,68,3,8,4,0,67,66,1,0,0,0,67,68,1,0,0,0,68,70,1,0,0,0,69,71,5,
+        16,0,0,70,69,1,0,0,0,70,71,1,0,0,0,71,73,1,0,0,0,72,74,5,78,0,0,
+        73,72,1,0,0,0,73,74,1,0,0,0,74,76,1,0,0,0,75,77,5,17,0,0,76,75,1,
+        0,0,0,76,77,1,0,0,0,77,79,1,0,0,0,78,80,5,21,0,0,79,78,1,0,0,0,79,
+        80,1,0,0,0,80,82,1,0,0,0,81,83,7,0,0,0,82,81,1,0,0,0,82,83,1,0,0,
+        0,83,85,1,0,0,0,84,86,5,21,0,0,85,84,1,0,0,0,85,86,1,0,0,0,86,88,
+        1,0,0,0,87,89,3,14,7,0,88,87,1,0,0,0,88,89,1,0,0,0,89,3,1,0,0,0,
+        90,92,7,1,0,0,91,93,5,78,0,0,92,91,1,0,0,0,92,93,1,0,0,0,93,94,1,
+        0,0,0,94,95,5,21,0,0,95,97,3,14,7,0,96,98,5,20,0,0,97,96,1,0,0,0,
+        97,98,1,0,0,0,98,5,1,0,0,0,99,100,5,78,0,0,100,113,5,16,0,0,101,
+        103,5,25,0,0,102,101,1,0,0,0,102,103,1,0,0,0,103,104,1,0,0,0,104,
+        106,3,14,7,0,105,107,5,25,0,0,106,105,1,0,0,0,106,107,1,0,0,0,107,
+        109,1,0,0,0,108,110,5,22,0,0,109,108,1,0,0,0,109,110,1,0,0,0,110,
+        112,1,0,0,0,111,102,1,0,0,0,112,115,1,0,0,0,113,111,1,0,0,0,113,
+        114,1,0,0,0,114,116,1,0,0,0,115,113,1,0,0,0,116,140,5,17,0,0,117,
+        118,5,78,0,0,118,124,5,16,0,0,119,120,5,78,0,0,120,121,5,21,0,0,
+        121,123,5,78,0,0,122,119,1,0,0,0,123,126,1,0,0,0,124,122,1,0,0,0,
+        124,125,1,0,0,0,125,127,1,0,0,0,126,124,1,0,0,0,127,140,5,17,0,0,
+        128,135,5,16,0,0,129,131,5,79,0,0,130,132,5,22,0,0,131,130,1,0,0,
+        0,131,132,1,0,0,0,132,134,1,0,0,0,133,129,1,0,0,0,134,137,1,0,0,
+        0,135,133,1,0,0,0,135,136,1,0,0,0,136,138,1,0,0,0,137,135,1,0,0,
+        0,138,140,5,17,0,0,139,99,1,0,0,0,139,117,1,0,0,0,139,128,1,0,0,
+        0,140,7,1,0,0,0,141,151,5,26,0,0,142,151,5,27,0,0,143,151,5,28,0,
+        0,144,151,5,29,0,0,145,151,5,11,0,0,146,151,5,12,0,0,147,151,3,10,
+        5,0,148,151,3,12,6,0,149,151,5,43,0,0,150,141,1,0,0,0,150,142,1,
+        0,0,0,150,143,1,0,0,0,150,144,1,0,0,0,150,145,1,0,0,0,150,146,1,
+        0,0,0,150,147,1,0,0,0,150,148,1,0,0,0,150,149,1,0,0,0,151,9,1,0,
+        0,0,152,153,5,43,0,0,153,154,5,38,0,0,154,155,3,8,4,0,155,156,5,
+        40,0,0,156,173,1,0,0,0,157,158,5,44,0,0,158,159,5,38,0,0,159,160,
+        3,8,4,0,160,161,5,40,0,0,161,173,1,0,0,0,162,163,5,45,0,0,163,164,
+        5,38,0,0,164,165,3,8,4,0,165,166,5,40,0,0,166,173,1,0,0,0,167,168,
+        5,46,0,0,168,169,5,38,0,0,169,170,3,8,4,0,170,171,5,40,0,0,171,173,
+        1,0,0,0,172,152,1,0,0,0,172,157,1,0,0,0,172,162,1,0,0,0,172,167,
+        1,0,0,0,173,11,1,0,0,0,174,175,5,78,0,0,175,13,1,0,0,0,176,178,7,
+        2,0,0,177,176,1,0,0,0,177,178,1,0,0,0,178,179,1,0,0,0,179,181,3,
+        20,10,0,180,182,3,14,7,0,181,180,1,0,0,0,181,182,1,0,0,0,182,909,
+        1,0,0,0,183,185,3,22,11,0,184,186,3,14,7,0,185,184,1,0,0,0,185,186,
+        1,0,0,0,186,909,1,0,0,0,187,188,5,30,0,0,188,909,3,14,7,0,189,190,
+        5,31,0,0,190,909,3,14,7,0,191,192,5,32,0,0,192,909,3,14,7,0,193,
+        195,5,33,0,0,194,196,3,14,7,0,195,194,1,0,0,0,195,196,1,0,0,0,196,
+        909,1,0,0,0,197,202,3,28,14,0,198,199,5,23,0,0,199,201,5,78,0,0,
+        200,198,1,0,0,0,201,204,1,0,0,0,202,200,1,0,0,0,202,203,1,0,0,0,
+        203,205,1,0,0,0,204,202,1,0,0,0,205,206,5,23,0,0,206,207,5,54,0,
+        0,207,208,5,16,0,0,208,209,3,8,4,0,209,211,5,17,0,0,210,212,3,14,
+        7,0,211,210,1,0,0,0,211,212,1,0,0,0,212,909,1,0,0,0,213,218,3,28,
+        14,0,214,215,5,23,0,0,215,217,5,78,0,0,216,214,1,0,0,0,217,220,1,
+        0,0,0,218,216,1,0,0,0,218,219,1,0,0,0,219,221,1,0,0,0,220,218,1,
+        0,0,0,221,222,5,23,0,0,222,223,5,53,0,0,223,224,5,16,0,0,224,225,
+        3,8,4,0,225,227,5,17,0,0,226,228,3,14,7,0,227,226,1,0,0,0,227,228,
+        1,0,0,0,228,909,1,0,0,0,229,234,3,28,14,0,230,231,5,23,0,0,231,233,
+        5,78,0,0,232,230,1,0,0,0,233,236,1,0,0,0,234,232,1,0,0,0,234,235,
+        1,0,0,0,235,237,1,0,0,0,236,234,1,0,0,0,237,238,5,23,0,0,238,239,
+        5,55,0,0,239,240,5,16,0,0,240,241,3,8,4,0,241,243,5,17,0,0,242,244,
+        3,14,7,0,243,242,1,0,0,0,243,244,1,0,0,0,244,909,1,0,0,0,245,247,
+        3,28,14,0,246,245,1,0,0,0,246,247,1,0,0,0,247,252,1,0,0,0,248,249,
+        5,23,0,0,249,251,5,78,0,0,250,248,1,0,0,0,251,254,1,0,0,0,252,250,
+        1,0,0,0,252,253,1,0,0,0,253,255,1,0,0,0,254,252,1,0,0,0,255,256,
+        5,76,0,0,256,257,5,57,0,0,257,258,5,16,0,0,258,260,5,17,0,0,259,
+        261,3,14,7,0,260,259,1,0,0,0,260,261,1,0,0,0,261,265,1,0,0,0,262,
+        264,5,17,0,0,263,262,1,0,0,0,264,267,1,0,0,0,265,263,1,0,0,0,265,
+        266,1,0,0,0,266,909,1,0,0,0,267,265,1,0,0,0,268,270,3,28,14,0,269,
+        268,1,0,0,0,269,270,1,0,0,0,270,275,1,0,0,0,271,272,5,23,0,0,272,
+        274,5,78,0,0,273,271,1,0,0,0,274,277,1,0,0,0,275,273,1,0,0,0,275,
+        276,1,0,0,0,276,278,1,0,0,0,277,275,1,0,0,0,278,279,5,76,0,0,279,
+        280,5,58,0,0,280,281,5,16,0,0,281,283,5,17,0,0,282,284,3,18,9,0,
+        283,282,1,0,0,0,283,284,1,0,0,0,284,286,1,0,0,0,285,287,3,14,7,0,
+        286,285,1,0,0,0,286,287,1,0,0,0,287,291,1,0,0,0,288,290,5,17,0,0,
+        289,288,1,0,0,0,290,293,1,0,0,0,291,289,1,0,0,0,291,292,1,0,0,0,
+        292,909,1,0,0,0,293,291,1,0,0,0,294,296,3,28,14,0,295,294,1,0,0,
+        0,295,296,1,0,0,0,296,301,1,0,0,0,297,298,5,23,0,0,298,300,5,78,
+        0,0,299,297,1,0,0,0,300,303,1,0,0,0,301,299,1,0,0,0,301,302,1,0,
+        0,0,302,304,1,0,0,0,303,301,1,0,0,0,304,305,5,76,0,0,305,306,5,59,
+        0,0,306,307,5,16,0,0,307,309,5,17,0,0,308,310,3,18,9,0,309,308,1,
+        0,0,0,309,310,1,0,0,0,310,312,1,0,0,0,311,313,3,14,7,0,312,311,1,
+        0,0,0,312,313,1,0,0,0,313,317,1,0,0,0,314,316,5,17,0,0,315,314,1,
+        0,0,0,316,319,1,0,0,0,317,315,1,0,0,0,317,318,1,0,0,0,318,909,1,
+        0,0,0,319,317,1,0,0,0,320,322,5,76,0,0,321,320,1,0,0,0,321,322,1,
+        0,0,0,322,323,1,0,0,0,323,324,5,60,0,0,324,325,5,16,0,0,325,326,
+        3,14,7,0,326,328,5,17,0,0,327,329,3,14,7,0,328,327,1,0,0,0,328,329,
+        1,0,0,0,329,333,1,0,0,0,330,332,5,17,0,0,331,330,1,0,0,0,332,335,
+        1,0,0,0,333,331,1,0,0,0,333,334,1,0,0,0,334,909,1,0,0,0,335,333,
+        1,0,0,0,336,338,5,76,0,0,337,336,1,0,0,0,337,338,1,0,0,0,338,339,
+        1,0,0,0,339,340,5,61,0,0,340,341,5,16,0,0,341,342,3,14,7,0,342,344,
+        5,17,0,0,343,345,3,14,7,0,344,343,1,0,0,0,344,345,1,0,0,0,345,349,
+        1,0,0,0,346,348,5,17,0,0,347,346,1,0,0,0,348,351,1,0,0,0,349,347,
+        1,0,0,0,349,350,1,0,0,0,350,909,1,0,0,0,351,349,1,0,0,0,352,354,
+        5,76,0,0,353,352,1,0,0,0,353,354,1,0,0,0,354,358,1,0,0,0,355,357,
+        5,16,0,0,356,355,1,0,0,0,357,360,1,0,0,0,358,356,1,0,0,0,358,359,
+        1,0,0,0,359,361,1,0,0,0,360,358,1,0,0,0,361,365,5,45,0,0,362,364,
+        5,18,0,0,363,362,1,0,0,0,364,367,1,0,0,0,365,363,1,0,0,0,365,366,
+        1,0,0,0,366,371,1,0,0,0,367,365,1,0,0,0,368,370,5,16,0,0,369,368,
+        1,0,0,0,370,373,1,0,0,0,371,369,1,0,0,0,371,372,1,0,0,0,372,386,
+        1,0,0,0,373,371,1,0,0,0,374,376,5,25,0,0,375,374,1,0,0,0,375,376,
+        1,0,0,0,376,377,1,0,0,0,377,379,3,14,7,0,378,380,5,25,0,0,379,378,
+        1,0,0,0,379,380,1,0,0,0,380,382,1,0,0,0,381,383,5,22,0,0,382,381,
+        1,0,0,0,382,383,1,0,0,0,383,385,1,0,0,0,384,375,1,0,0,0,385,388,
+        1,0,0,0,386,384,1,0,0,0,386,387,1,0,0,0,387,392,1,0,0,0,388,386,
+        1,0,0,0,389,391,5,19,0,0,390,389,1,0,0,0,391,394,1,0,0,0,392,390,
+        1,0,0,0,392,393,1,0,0,0,393,398,1,0,0,0,394,392,1,0,0,0,395,397,
+        5,17,0,0,396,395,1,0,0,0,397,400,1,0,0,0,398,396,1,0,0,0,398,399,
+        1,0,0,0,399,402,1,0,0,0,400,398,1,0,0,0,401,403,3,14,7,0,402,401,
+        1,0,0,0,402,403,1,0,0,0,403,909,1,0,0,0,404,406,5,76,0,0,405,404,
+        1,0,0,0,405,406,1,0,0,0,406,410,1,0,0,0,407,409,5,16,0,0,408,407,
+        1,0,0,0,409,412,1,0,0,0,410,408,1,0,0,0,410,411,1,0,0,0,411,413,
+        1,0,0,0,412,410,1,0,0,0,413,417,5,62,0,0,414,416,5,18,0,0,415,414,
+        1,0,0,0,416,419,1,0,0,0,417,415,1,0,0,0,417,418,1,0,0,0,418,423,
+        1,0,0,0,419,417,1,0,0,0,420,422,5,16,0,0,421,420,1,0,0,0,422,425,
+        1,0,0,0,423,421,1,0,0,0,423,424,1,0,0,0,424,438,1,0,0,0,425,423,
+        1,0,0,0,426,428,5,25,0,0,427,426,1,0,0,0,427,428,1,0,0,0,428,429,
+        1,0,0,0,429,431,3,14,7,0,430,432,5,25,0,0,431,430,1,0,0,0,431,432,
+        1,0,0,0,432,434,1,0,0,0,433,435,5,22,0,0,434,433,1,0,0,0,434,435,
+        1,0,0,0,435,437,1,0,0,0,436,427,1,0,0,0,437,440,1,0,0,0,438,436,
+        1,0,0,0,438,439,1,0,0,0,439,444,1,0,0,0,440,438,1,0,0,0,441,443,
+        5,17,0,0,442,441,1,0,0,0,443,446,1,0,0,0,444,442,1,0,0,0,444,445,
+        1,0,0,0,445,450,1,0,0,0,446,444,1,0,0,0,447,449,5,19,0,0,448,447,
+        1,0,0,0,449,452,1,0,0,0,450,448,1,0,0,0,450,451,1,0,0,0,451,454,
+        1,0,0,0,452,450,1,0,0,0,453,455,3,14,7,0,454,453,1,0,0,0,454,455,
+        1,0,0,0,455,909,1,0,0,0,456,458,5,76,0,0,457,456,1,0,0,0,457,458,
+        1,0,0,0,458,459,1,0,0,0,459,461,5,56,0,0,460,462,5,16,0,0,461,460,
+        1,0,0,0,462,463,1,0,0,0,463,461,1,0,0,0,463,464,1,0,0,0,464,466,
+        1,0,0,0,465,467,3,14,7,0,466,465,1,0,0,0,466,467,1,0,0,0,467,469,
+        1,0,0,0,468,470,5,17,0,0,469,468,1,0,0,0,470,471,1,0,0,0,471,469,
+        1,0,0,0,471,472,1,0,0,0,472,474,1,0,0,0,473,475,3,14,7,0,474,473,
+        1,0,0,0,474,475,1,0,0,0,475,909,1,0,0,0,476,478,5,76,0,0,477,476,
+        1,0,0,0,477,478,1,0,0,0,478,482,1,0,0,0,479,481,5,16,0,0,480,479,
+        1,0,0,0,481,484,1,0,0,0,482,480,1,0,0,0,482,483,1,0,0,0,483,485,
+        1,0,0,0,484,482,1,0,0,0,485,486,5,46,0,0,486,499,5,18,0,0,487,489,
+        5,25,0,0,488,487,1,0,0,0,488,489,1,0,0,0,489,490,1,0,0,0,490,492,
+        3,14,7,0,491,493,5,25,0,0,492,491,1,0,0,0,492,493,1,0,0,0,493,495,
+        1,0,0,0,494,496,5,22,0,0,495,494,1,0,0,0,495,496,1,0,0,0,496,498,
+        1,0,0,0,497,488,1,0,0,0,498,501,1,0,0,0,499,497,1,0,0,0,499,500,
+        1,0,0,0,500,502,1,0,0,0,501,499,1,0,0,0,502,506,5,19,0,0,503,505,
+        5,17,0,0,504,503,1,0,0,0,505,508,1,0,0,0,506,504,1,0,0,0,506,507,
+        1,0,0,0,507,510,1,0,0,0,508,506,1,0,0,0,509,511,3,14,7,0,510,509,
+        1,0,0,0,510,511,1,0,0,0,511,909,1,0,0,0,512,514,5,76,0,0,513,512,
+        1,0,0,0,513,514,1,0,0,0,514,518,1,0,0,0,515,517,5,16,0,0,516,515,
+        1,0,0,0,517,520,1,0,0,0,518,516,1,0,0,0,518,519,1,0,0,0,519,521,
+        1,0,0,0,520,518,1,0,0,0,521,525,5,63,0,0,522,524,5,18,0,0,523,522,
+        1,0,0,0,524,527,1,0,0,0,525,523,1,0,0,0,525,526,1,0,0,0,526,531,
+        1,0,0,0,527,525,1,0,0,0,528,530,5,16,0,0,529,528,1,0,0,0,530,533,
+        1,0,0,0,531,529,1,0,0,0,531,532,1,0,0,0,532,546,1,0,0,0,533,531,
+        1,0,0,0,534,536,5,25,0,0,535,534,1,0,0,0,535,536,1,0,0,0,536,537,
+        1,0,0,0,537,539,3,14,7,0,538,540,5,25,0,0,539,538,1,0,0,0,539,540,
+        1,0,0,0,540,542,1,0,0,0,541,543,5,22,0,0,542,541,1,0,0,0,542,543,
+        1,0,0,0,543,545,1,0,0,0,544,535,1,0,0,0,545,548,1,0,0,0,546,544,
+        1,0,0,0,546,547,1,0,0,0,547,552,1,0,0,0,548,546,1,0,0,0,549,551,
+        5,19,0,0,550,549,1,0,0,0,551,554,1,0,0,0,552,550,1,0,0,0,552,553,
+        1,0,0,0,553,558,1,0,0,0,554,552,1,0,0,0,555,557,5,17,0,0,556,555,
+        1,0,0,0,557,560,1,0,0,0,558,556,1,0,0,0,558,559,1,0,0,0,559,562,
+        1,0,0,0,560,558,1,0,0,0,561,563,3,14,7,0,562,561,1,0,0,0,562,563,
+        1,0,0,0,563,564,1,0,0,0,564,909,5,17,0,0,565,567,5,76,0,0,566,565,
+        1,0,0,0,566,567,1,0,0,0,567,571,1,0,0,0,568,570,5,16,0,0,569,568,
+        1,0,0,0,570,573,1,0,0,0,571,569,1,0,0,0,571,572,1,0,0,0,572,574,
+        1,0,0,0,573,571,1,0,0,0,574,578,5,43,0,0,575,577,5,16,0,0,576,575,
+        1,0,0,0,577,580,1,0,0,0,578,576,1,0,0,0,578,579,1,0,0,0,579,584,
+        1,0,0,0,580,578,1,0,0,0,581,583,5,18,0,0,582,581,1,0,0,0,583,586,
+        1,0,0,0,584,582,1,0,0,0,584,585,1,0,0,0,585,599,1,0,0,0,586,584,
+        1,0,0,0,587,589,5,25,0,0,588,587,1,0,0,0,588,589,1,0,0,0,589,590,
+        1,0,0,0,590,592,3,14,7,0,591,593,5,25,0,0,592,591,1,0,0,0,592,593,
+        1,0,0,0,593,595,1,0,0,0,594,596,5,22,0,0,595,594,1,0,0,0,595,596,
+        1,0,0,0,596,598,1,0,0,0,597,588,1,0,0,0,598,601,1,0,0,0,599,597,
+        1,0,0,0,599,600,1,0,0,0,600,605,1,0,0,0,601,599,1,0,0,0,602,604,
+        5,19,0,0,603,602,1,0,0,0,604,607,1,0,0,0,605,603,1,0,0,0,605,606,
+        1,0,0,0,606,611,1,0,0,0,607,605,1,0,0,0,608,610,5,17,0,0,609,608,
+        1,0,0,0,610,613,1,0,0,0,611,609,1,0,0,0,611,612,1,0,0,0,612,615,
+        1,0,0,0,613,611,1,0,0,0,614,616,3,14,7,0,615,614,1,0,0,0,615,616,
+        1,0,0,0,616,909,1,0,0,0,617,619,5,76,0,0,618,617,1,0,0,0,618,619,
+        1,0,0,0,619,623,1,0,0,0,620,622,5,16,0,0,621,620,1,0,0,0,622,625,
+        1,0,0,0,623,621,1,0,0,0,623,624,1,0,0,0,624,626,1,0,0,0,625,623,
+        1,0,0,0,626,630,5,44,0,0,627,629,5,16,0,0,628,627,1,0,0,0,629,632,
+        1,0,0,0,630,628,1,0,0,0,630,631,1,0,0,0,631,636,1,0,0,0,632,630,
+        1,0,0,0,633,635,5,18,0,0,634,633,1,0,0,0,635,638,1,0,0,0,636,634,
+        1,0,0,0,636,637,1,0,0,0,637,651,1,0,0,0,638,636,1,0,0,0,639,641,
+        5,25,0,0,640,639,1,0,0,0,640,641,1,0,0,0,641,642,1,0,0,0,642,644,
+        3,14,7,0,643,645,5,25,0,0,644,643,1,0,0,0,644,645,1,0,0,0,645,647,
+        1,0,0,0,646,648,5,22,0,0,647,646,1,0,0,0,647,648,1,0,0,0,648,650,
+        1,0,0,0,649,640,1,0,0,0,650,653,1,0,0,0,651,649,1,0,0,0,651,652,
+        1,0,0,0,652,657,1,0,0,0,653,651,1,0,0,0,654,656,5,19,0,0,655,654,
+        1,0,0,0,656,659,1,0,0,0,657,655,1,0,0,0,657,658,1,0,0,0,658,663,
+        1,0,0,0,659,657,1,0,0,0,660,662,5,17,0,0,661,660,1,0,0,0,662,665,
+        1,0,0,0,663,661,1,0,0,0,663,664,1,0,0,0,664,667,1,0,0,0,665,663,
+        1,0,0,0,666,668,3,14,7,0,667,666,1,0,0,0,667,668,1,0,0,0,668,909,
+        1,0,0,0,669,670,5,76,0,0,670,672,5,64,0,0,671,673,5,16,0,0,672,671,
+        1,0,0,0,673,674,1,0,0,0,674,672,1,0,0,0,674,675,1,0,0,0,675,688,
+        1,0,0,0,676,678,5,25,0,0,677,676,1,0,0,0,677,678,1,0,0,0,678,679,
+        1,0,0,0,679,681,3,14,7,0,680,682,5,25,0,0,681,680,1,0,0,0,681,682,
+        1,0,0,0,682,684,1,0,0,0,683,685,5,22,0,0,684,683,1,0,0,0,684,685,
+        1,0,0,0,685,687,1,0,0,0,686,677,1,0,0,0,687,690,1,0,0,0,688,686,
+        1,0,0,0,688,689,1,0,0,0,689,692,1,0,0,0,690,688,1,0,0,0,691,693,
+        5,17,0,0,692,691,1,0,0,0,693,694,1,0,0,0,694,692,1,0,0,0,694,695,
+        1,0,0,0,695,697,1,0,0,0,696,698,3,14,7,0,697,696,1,0,0,0,697,698,
+        1,0,0,0,698,909,1,0,0,0,699,700,5,76,0,0,700,701,5,65,0,0,701,703,
+        5,16,0,0,702,704,5,17,0,0,703,702,1,0,0,0,704,705,1,0,0,0,705,703,
+        1,0,0,0,705,706,1,0,0,0,706,708,1,0,0,0,707,709,3,14,7,0,708,707,
+        1,0,0,0,708,709,1,0,0,0,709,909,1,0,0,0,710,711,5,76,0,0,711,712,
+        5,66,0,0,712,725,5,16,0,0,713,715,5,25,0,0,714,713,1,0,0,0,714,715,
+        1,0,0,0,715,716,1,0,0,0,716,718,3,14,7,0,717,719,5,25,0,0,718,717,
+        1,0,0,0,718,719,1,0,0,0,719,721,1,0,0,0,720,722,5,22,0,0,721,720,
+        1,0,0,0,721,722,1,0,0,0,722,724,1,0,0,0,723,714,1,0,0,0,724,727,
+        1,0,0,0,725,723,1,0,0,0,725,726,1,0,0,0,726,729,1,0,0,0,727,725,
+        1,0,0,0,728,730,5,17,0,0,729,728,1,0,0,0,730,731,1,0,0,0,731,729,
+        1,0,0,0,731,732,1,0,0,0,732,734,1,0,0,0,733,735,3,14,7,0,734,733,
+        1,0,0,0,734,735,1,0,0,0,735,909,1,0,0,0,736,738,5,76,0,0,737,736,
+        1,0,0,0,737,738,1,0,0,0,738,739,1,0,0,0,739,740,7,3,0,0,740,749,
+        5,16,0,0,741,744,5,78,0,0,742,743,5,21,0,0,743,745,5,78,0,0,744,
+        742,1,0,0,0,744,745,1,0,0,0,745,747,1,0,0,0,746,748,5,22,0,0,747,
+        746,1,0,0,0,747,748,1,0,0,0,748,750,1,0,0,0,749,741,1,0,0,0,750,
+        751,1,0,0,0,751,749,1,0,0,0,751,752,1,0,0,0,752,753,1,0,0,0,753,
+        754,5,42,0,0,754,755,3,14,7,0,755,757,5,17,0,0,756,758,3,16,8,0,
+        757,756,1,0,0,0,757,758,1,0,0,0,758,909,1,0,0,0,759,761,5,76,0,0,
+        760,759,1,0,0,0,760,761,1,0,0,0,761,762,1,0,0,0,762,763,7,3,0,0,
+        763,764,5,16,0,0,764,765,3,14,7,0,765,767,5,17,0,0,766,768,3,16,
+        8,0,767,766,1,0,0,0,767,768,1,0,0,0,768,909,1,0,0,0,769,770,5,76,
+        0,0,770,771,5,67,0,0,771,772,5,16,0,0,772,774,3,14,7,0,773,775,5,
+        17,0,0,774,773,1,0,0,0,775,776,1,0,0,0,776,774,1,0,0,0,776,777,1,
+        0,0,0,777,779,1,0,0,0,778,780,3,14,7,0,779,778,1,0,0,0,779,780,1,
+        0,0,0,780,909,1,0,0,0,781,782,5,76,0,0,782,783,5,68,0,0,783,784,
+        5,16,0,0,784,786,5,17,0,0,785,787,3,14,7,0,786,785,1,0,0,0,786,787,
+        1,0,0,0,787,909,1,0,0,0,788,789,5,76,0,0,789,790,5,69,0,0,790,791,
+        5,16,0,0,791,793,5,17,0,0,792,794,3,14,7,0,793,792,1,0,0,0,793,794,
+        1,0,0,0,794,909,1,0,0,0,795,796,5,76,0,0,796,797,5,72,0,0,797,798,
+        5,16,0,0,798,799,3,14,7,0,799,801,5,17,0,0,800,802,3,14,7,0,801,
+        800,1,0,0,0,801,802,1,0,0,0,802,909,1,0,0,0,803,804,5,77,0,0,804,
+        805,5,21,0,0,805,909,3,14,7,0,806,807,5,78,0,0,807,808,5,21,0,0,
+        808,809,5,78,0,0,809,810,5,24,0,0,810,909,3,14,7,0,811,813,5,16,
+        0,0,812,811,1,0,0,0,813,816,1,0,0,0,814,812,1,0,0,0,814,815,1,0,
+        0,0,815,818,1,0,0,0,816,814,1,0,0,0,817,819,3,28,14,0,818,817,1,
+        0,0,0,818,819,1,0,0,0,819,824,1,0,0,0,820,821,5,23,0,0,821,823,5,
+        78,0,0,822,820,1,0,0,0,823,826,1,0,0,0,824,822,1,0,0,0,824,825,1,
+        0,0,0,825,828,1,0,0,0,826,824,1,0,0,0,827,829,3,24,12,0,828,827,
+        1,0,0,0,828,829,1,0,0,0,829,831,1,0,0,0,830,832,3,28,14,0,831,830,
+        1,0,0,0,831,832,1,0,0,0,832,835,1,0,0,0,833,834,5,23,0,0,834,836,
+        5,78,0,0,835,833,1,0,0,0,836,837,1,0,0,0,837,835,1,0,0,0,837,838,
+        1,0,0,0,838,840,1,0,0,0,839,841,3,14,7,0,840,839,1,0,0,0,840,841,
+        1,0,0,0,841,909,1,0,0,0,842,846,3,28,14,0,843,845,5,23,0,0,844,843,
+        1,0,0,0,845,848,1,0,0,0,846,844,1,0,0,0,846,847,1,0,0,0,847,852,
+        1,0,0,0,848,846,1,0,0,0,849,851,5,78,0,0,850,849,1,0,0,0,851,854,
+        1,0,0,0,852,850,1,0,0,0,852,853,1,0,0,0,853,855,1,0,0,0,854,852,
+        1,0,0,0,855,857,3,6,3,0,856,858,3,24,12,0,857,856,1,0,0,0,857,858,
+        1,0,0,0,858,860,1,0,0,0,859,861,3,14,7,0,860,859,1,0,0,0,860,861,
+        1,0,0,0,861,909,1,0,0,0,862,863,5,76,0,0,863,909,3,14,7,0,864,866,
+        5,79,0,0,865,867,3,14,7,0,866,865,1,0,0,0,866,867,1,0,0,0,867,909,
+        1,0,0,0,868,870,5,76,0,0,869,868,1,0,0,0,869,870,1,0,0,0,870,871,
+        1,0,0,0,871,873,3,6,3,0,872,874,3,14,7,0,873,872,1,0,0,0,873,874,
+        1,0,0,0,874,909,1,0,0,0,875,876,5,25,0,0,876,878,3,14,7,0,877,879,
+        5,23,0,0,878,877,1,0,0,0,878,879,1,0,0,0,879,880,1,0,0,0,880,882,
+        5,25,0,0,881,883,5,23,0,0,882,881,1,0,0,0,882,883,1,0,0,0,883,885,
+        1,0,0,0,884,886,3,14,7,0,885,884,1,0,0,0,885,886,1,0,0,0,886,909,
+        1,0,0,0,887,888,5,14,0,0,888,909,3,14,7,0,889,891,5,34,0,0,890,889,
+        1,0,0,0,890,891,1,0,0,0,891,893,1,0,0,0,892,894,5,35,0,0,893,892,
+        1,0,0,0,893,894,1,0,0,0,894,896,1,0,0,0,895,897,5,78,0,0,896,895,
+        1,0,0,0,896,897,1,0,0,0,897,898,1,0,0,0,898,899,5,15,0,0,899,909,
+        3,14,7,0,900,902,3,24,12,0,901,903,3,26,13,0,902,901,1,0,0,0,902,
+        903,1,0,0,0,903,909,1,0,0,0,904,906,3,28,14,0,905,907,3,14,7,0,906,
+        905,1,0,0,0,906,907,1,0,0,0,907,909,1,0,0,0,908,177,1,0,0,0,908,
+        183,1,0,0,0,908,187,1,0,0,0,908,189,1,0,0,0,908,191,1,0,0,0,908,
+        193,1,0,0,0,908,197,1,0,0,0,908,213,1,0,0,0,908,229,1,0,0,0,908,
+        246,1,0,0,0,908,269,1,0,0,0,908,295,1,0,0,0,908,321,1,0,0,0,908,
+        337,1,0,0,0,908,353,1,0,0,0,908,405,1,0,0,0,908,457,1,0,0,0,908,
+        477,1,0,0,0,908,513,1,0,0,0,908,566,1,0,0,0,908,618,1,0,0,0,908,
+        669,1,0,0,0,908,699,1,0,0,0,908,710,1,0,0,0,908,737,1,0,0,0,908,
+        760,1,0,0,0,908,769,1,0,0,0,908,781,1,0,0,0,908,788,1,0,0,0,908,
+        795,1,0,0,0,908,803,1,0,0,0,908,806,1,0,0,0,908,814,1,0,0,0,908,
+        842,1,0,0,0,908,862,1,0,0,0,908,864,1,0,0,0,908,869,1,0,0,0,908,
+        875,1,0,0,0,908,887,1,0,0,0,908,890,1,0,0,0,908,900,1,0,0,0,908,
+        904,1,0,0,0,909,15,1,0,0,0,910,912,7,2,0,0,911,910,1,0,0,0,911,912,
+        1,0,0,0,912,913,1,0,0,0,913,914,3,14,7,0,914,17,1,0,0,0,915,925,
+        3,24,12,0,916,921,3,28,14,0,917,918,5,23,0,0,918,920,5,78,0,0,919,
+        917,1,0,0,0,920,923,1,0,0,0,921,919,1,0,0,0,921,922,1,0,0,0,922,
+        926,1,0,0,0,923,921,1,0,0,0,924,926,5,79,0,0,925,916,1,0,0,0,925,
+        924,1,0,0,0,926,19,1,0,0,0,927,932,3,28,14,0,928,929,5,23,0,0,929,
+        931,5,78,0,0,930,928,1,0,0,0,931,934,1,0,0,0,932,930,1,0,0,0,932,
+        933,1,0,0,0,933,937,1,0,0,0,934,932,1,0,0,0,935,937,5,79,0,0,936,
+        927,1,0,0,0,936,935,1,0,0,0,937,942,1,0,0,0,938,939,5,23,0,0,939,
+        941,5,78,0,0,940,938,1,0,0,0,941,944,1,0,0,0,942,940,1,0,0,0,942,
+        943,1,0,0,0,943,945,1,0,0,0,944,942,1,0,0,0,945,955,3,24,12,0,946,
+        951,3,28,14,0,947,948,5,23,0,0,948,950,5,78,0,0,949,947,1,0,0,0,
+        950,953,1,0,0,0,951,949,1,0,0,0,951,952,1,0,0,0,952,956,1,0,0,0,
+        953,951,1,0,0,0,954,956,5,79,0,0,955,946,1,0,0,0,955,954,1,0,0,0,
+        956,21,1,0,0,0,957,958,7,4,0,0,958,959,3,14,7,0,959,23,1,0,0,0,960,
+        961,7,5,0,0,961,25,1,0,0,0,962,977,5,79,0,0,963,965,5,25,0,0,964,
+        963,1,0,0,0,964,965,1,0,0,0,965,966,1,0,0,0,966,968,5,78,0,0,967,
+        969,5,16,0,0,968,967,1,0,0,0,968,969,1,0,0,0,969,971,1,0,0,0,970,
+        972,5,17,0,0,971,970,1,0,0,0,971,972,1,0,0,0,972,974,1,0,0,0,973,
+        975,5,25,0,0,974,973,1,0,0,0,974,975,1,0,0,0,975,977,1,0,0,0,976,
+        962,1,0,0,0,976,964,1,0,0,0,977,27,1,0,0,0,978,987,3,30,15,0,979,
+        987,5,6,0,0,980,987,3,6,3,0,981,982,5,16,0,0,982,983,3,14,7,0,983,
+        984,5,17,0,0,984,987,1,0,0,0,985,987,5,78,0,0,986,978,1,0,0,0,986,
+        979,1,0,0,0,986,980,1,0,0,0,986,981,1,0,0,0,986,985,1,0,0,0,987,
+        29,1,0,0,0,988,989,7,6,0,0,989,31,1,0,0,0,190,36,43,46,51,55,58,
+        61,64,67,70,73,76,79,82,85,88,92,97,102,106,109,113,124,131,135,
+        139,150,172,177,181,185,195,202,211,218,227,234,243,246,252,260,
+        265,269,275,283,286,291,295,301,309,312,317,321,328,333,337,344,
+        349,353,358,365,371,375,379,382,386,392,398,402,405,410,417,423,
+        427,431,434,438,444,450,454,457,463,466,471,474,477,482,488,492,
+        495,499,506,510,513,518,525,531,535,539,542,546,552,558,562,566,
+        571,578,584,588,592,595,599,605,611,615,618,623,630,636,640,644,
+        647,651,657,663,667,674,677,681,684,688,694,697,705,708,714,718,
+        721,725,731,734,737,744,747,751,757,760,767,776,779,786,793,801,
+        814,818,824,828,831,837,840,846,852,857,860,866,869,873,878,882,
+        885,890,893,896,902,906,908,911,921,925,932,936,942,951,955,964,
+        968,971,974,976,986
     ]
 
-class OCLsParser ( Parser ):
+class BOCLParser ( Parser ):
 
-    grammarFileName = "OCLs.g4"
+    grammarFileName = "BOCL.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
 
     decisionsToDFA = [ DFA(ds, i) for i, ds in enumerate(atn.decisionToState) ]
 
     sharedContextCache = PredictionContextCache()
 
-    literalNames = [ "<INVALID>", "'context'", "'inv'", "'pre'", "'post'", 
-                     "'self'", "'forAll'", "'exists'", "'select'", "'collect'", 
-                     "'OclAny'", "'OclVoid'", "<INVALID>", "'..'", "'::'", 
-                     "'('", "')'", "'{'", "'}'", "';'", "':'", "','", "'.'", 
-                     "'='", "'''", "'Boolean'", "'Integer'", "'Real'", "'String'", 
-                     "'if'", "'then'", "'else'", "'endif'", "'and'", "'or'", 
-                     "'not'", "'<>'", "'<'", "'<='", "'>'", "'>='", "'|'", 
-                     "<INVALID>", "'Bag'", "'Sequence'", "'OrderedSet'", 
-                     "'-'", "'+'", "'/'", "' '", "'xor'", "'implies'", "'oclAsType'", 
-                     "'oclIsTypeOf'", "'oclIsKindOf'", "'allInstances'", 
-                     "'isEmpty'", "'sum'", "'size'", "'includes'", "'excludes'", 
-                     "'subSequence'", "'subOrderedSet'", "'prepend'", "'last'", 
-                     "'append'", "'symmetricDifference'", "'first'", "'derive'", 
-                     "'body'", "'init'", "'union'", "'null'", "'let'", "'in'", 
-                     "<INVALID>", "'def'" ]
-
-    symbolicNames = [ "<INVALID>", "CONTEXT", "INV", "PRE", "POST", "SELF", 
-                      "FORALL", "EXISTS", "SELECT", "COLLECT", "OCLANY", 
-                      "OCLVOID", "WS", "DoubleDots", "DoubleCOLON", "LPAREN", 
-                      "RPAREN", "LBRACE", "RBRACE", "SEMI", "COLON", "COMMA", 
-                      "DOT", "EQUAL", "SingleQuote", "BOOLEAN_TYPE", "INTEGER_TYPE", 
-                      "REAL_TYPE", "STRING_TYPE", "IF", "THEN", "ELSE", 
-                      "ENDIF", "AND", "OR", "NOT", "NOTEQUAL", "LT", "LE", 
-                      "GT", "GE", "PIPE", "SET", "BAG", "SEQUENCE", "ORDEREDSET", 
-                      "MINUS", "PLUS", "Divide", "EMPTYSTRING", "XOR", "IMPLIES", 
-                      "OCLASTYPE", "OCLISTYPEOF", "OCLISKINDOF", "ALLINSTANCES", 
-                      "ISEMPTY", "SUM", "SIZE", "INCLUDES", "EXCLUDES", 
-                      "SUBSEQUENCE", "SUBORDEREDSET", "PREPEND", "LAST", 
-                      "APPEND", "SYMMETRICDIFFERENCE", "FIRST", "DERIVE", 
-                      "BODY", "Init", "UNION", "NULL", "LET", "IN", "Arrow", 
-                      "Def", "ID", "NUMBER", "STRING_LITERAL", "BOOLEAN_LITERAL", 
-                      "COMMENT", "LINE_COMMENT" ]
+    literalNames = [ "<INVALID>", "'*'", "'context'", "'inv'", "'pre'", 
+                     "'post'", "'self'", "'forAll'", "'exists'", "'select'", 
+                     "'collect'", "'OclAny'", "'OclVoid'", "<INVALID>", 
+                     "'..'", "'::'", "'('", "')'", "'{'", "'}'", "';'", 
+                     "':'", "','", "'.'", "'='", "'''", "'Boolean'", "'Integer'", 
+                     "'Real'", "'String'", "'if'", "'then'", "'else'", "'endif'", 
+                     "'and'", "'or'", "'not'", "'<>'", "'<'", "'<='", "'>'", 
+                     "'>='", "'|'", "<INVALID>", "'Bag'", "'Sequence'", 
+                     "'OrderedSet'", "'-'", "'+'", "'/'", "' '", "'xor'", 
+                     "'implies'", "'oclAsType'", "'oclIsTypeOf'", "'oclIsKindOf'", 
+                     "'allInstances'", "'isEmpty'", "'sum'", "'size'", "'includes'", 
+                     "'excludes'", "'subSequence'", "'subOrderedSet'", "'prepend'", 
+                     "'last'", "'append'", "'symmetricDifference'", "'first'", 
+                     "'derive'", "'body'", "'init'", "'union'", "'null'", 
+                     "'let'", "'in'", "<INVALID>", "'def'" ]
+
+    symbolicNames = [ "<INVALID>", "<INVALID>", "CONTEXT", "INV", "PRE", 
+                      "POST", "SELF", "FORALL", "EXISTS", "SELECT", "COLLECT", 
+                      "OCLANY", "OCLVOID", "WS", "DoubleDots", "DoubleCOLON", 
+                      "LPAREN", "RPAREN", "LBRACE", "RBRACE", "SEMI", "COLON", 
+                      "COMMA", "DOT", "EQUAL", "SingleQuote", "BOOLEAN_TYPE", 
+                      "INTEGER_TYPE", "REAL_TYPE", "STRING_TYPE", "IF", 
+                      "THEN", "ELSE", "ENDIF", "AND", "OR", "NOT", "NOTEQUAL", 
+                      "LT", "LE", "GT", "GE", "PIPE", "SET", "BAG", "SEQUENCE", 
+                      "ORDEREDSET", "MINUS", "PLUS", "Divide", "EMPTYSTRING", 
+                      "XOR", "IMPLIES", "OCLASTYPE", "OCLISTYPEOF", "OCLISKINDOF", 
+                      "ALLINSTANCES", "ISEMPTY", "SUM", "SIZE", "INCLUDES", 
+                      "EXCLUDES", "SUBSEQUENCE", "SUBORDEREDSET", "PREPEND", 
+                      "LAST", "APPEND", "SYMMETRICDIFFERENCE", "FIRST", 
+                      "DERIVE", "BODY", "Init", "UNION", "NULL", "LET", 
+                      "IN", "Arrow", "Def", "ID", "NUMBER", "STRING_LITERAL", 
+                      "BOOLEAN_LITERAL", "COMMENT", "LINE_COMMENT" ]
 
     RULE_oclFile = 0
     RULE_contextDeclaration = 1
     RULE_constraint = 2
     RULE_functionCall = 3
     RULE_type = 4
     RULE_collectionType = 5
     RULE_userDefinedType = 6
     RULE_expression = 7
-    RULE_binaryExpression = 8
-    RULE_unaryExpression = 9
-    RULE_operator = 10
-    RULE_numberORUserDefined = 11
-    RULE_primaryExpression = 12
-    RULE_literal = 13
+    RULE_endExpression = 8
+    RULE_binaryFunctionCall = 9
+    RULE_binaryExpression = 10
+    RULE_unaryExpression = 11
+    RULE_operator = 12
+    RULE_numberORUserDefined = 13
+    RULE_primaryExpression = 14
+    RULE_literal = 15
 
     ruleNames =  [ "oclFile", "contextDeclaration", "constraint", "functionCall", 
                    "type", "collectionType", "userDefinedType", "expression", 
-                   "binaryExpression", "unaryExpression", "operator", "numberORUserDefined", 
+                   "endExpression", "binaryFunctionCall", "binaryExpression", 
+                   "unaryExpression", "operator", "numberORUserDefined", 
                    "primaryExpression", "literal" ]
 
     EOF = Token.EOF
-    CONTEXT=1
-    INV=2
-    PRE=3
-    POST=4
-    SELF=5
-    FORALL=6
-    EXISTS=7
-    SELECT=8
-    COLLECT=9
-    OCLANY=10
-    OCLVOID=11
-    WS=12
-    DoubleDots=13
-    DoubleCOLON=14
-    LPAREN=15
-    RPAREN=16
-    LBRACE=17
-    RBRACE=18
-    SEMI=19
-    COLON=20
-    COMMA=21
-    DOT=22
-    EQUAL=23
-    SingleQuote=24
-    BOOLEAN_TYPE=25
-    INTEGER_TYPE=26
-    REAL_TYPE=27
-    STRING_TYPE=28
-    IF=29
-    THEN=30
-    ELSE=31
-    ENDIF=32
-    AND=33
-    OR=34
-    NOT=35
-    NOTEQUAL=36
-    LT=37
-    LE=38
-    GT=39
-    GE=40
-    PIPE=41
-    SET=42
-    BAG=43
-    SEQUENCE=44
-    ORDEREDSET=45
-    MINUS=46
-    PLUS=47
-    Divide=48
-    EMPTYSTRING=49
-    XOR=50
-    IMPLIES=51
-    OCLASTYPE=52
-    OCLISTYPEOF=53
-    OCLISKINDOF=54
-    ALLINSTANCES=55
-    ISEMPTY=56
-    SUM=57
-    SIZE=58
-    INCLUDES=59
-    EXCLUDES=60
-    SUBSEQUENCE=61
-    SUBORDEREDSET=62
-    PREPEND=63
-    LAST=64
-    APPEND=65
-    SYMMETRICDIFFERENCE=66
-    FIRST=67
-    DERIVE=68
-    BODY=69
-    Init=70
-    UNION=71
-    NULL=72
-    LET=73
-    IN=74
-    Arrow=75
-    Def=76
-    ID=77
-    NUMBER=78
-    STRING_LITERAL=79
-    BOOLEAN_LITERAL=80
-    COMMENT=81
-    LINE_COMMENT=82
+    T__0=1
+    CONTEXT=2
+    INV=3
+    PRE=4
+    POST=5
+    SELF=6
+    FORALL=7
+    EXISTS=8
+    SELECT=9
+    COLLECT=10
+    OCLANY=11
+    OCLVOID=12
+    WS=13
+    DoubleDots=14
+    DoubleCOLON=15
+    LPAREN=16
+    RPAREN=17
+    LBRACE=18
+    RBRACE=19
+    SEMI=20
+    COLON=21
+    COMMA=22
+    DOT=23
+    EQUAL=24
+    SingleQuote=25
+    BOOLEAN_TYPE=26
+    INTEGER_TYPE=27
+    REAL_TYPE=28
+    STRING_TYPE=29
+    IF=30
+    THEN=31
+    ELSE=32
+    ENDIF=33
+    AND=34
+    OR=35
+    NOT=36
+    NOTEQUAL=37
+    LT=38
+    LE=39
+    GT=40
+    GE=41
+    PIPE=42
+    SET=43
+    BAG=44
+    SEQUENCE=45
+    ORDEREDSET=46
+    MINUS=47
+    PLUS=48
+    Divide=49
+    EMPTYSTRING=50
+    XOR=51
+    IMPLIES=52
+    OCLASTYPE=53
+    OCLISTYPEOF=54
+    OCLISKINDOF=55
+    ALLINSTANCES=56
+    ISEMPTY=57
+    SUM=58
+    SIZE=59
+    INCLUDES=60
+    EXCLUDES=61
+    SUBSEQUENCE=62
+    SUBORDEREDSET=63
+    PREPEND=64
+    LAST=65
+    APPEND=66
+    SYMMETRICDIFFERENCE=67
+    FIRST=68
+    DERIVE=69
+    BODY=70
+    Init=71
+    UNION=72
+    NULL=73
+    LET=74
+    IN=75
+    Arrow=76
+    Def=77
+    ID=78
+    NUMBER=79
+    STRING_LITERAL=80
+    BOOLEAN_LITERAL=81
+    COMMENT=82
+    LINE_COMMENT=83
 
     def __init__(self, input:TokenStream, output:TextIO = sys.stdout):
         super().__init__(input, output)
         self.checkVersion("4.13.1")
         self._interp = ParserATNSimulator(self, self.atn, self.decisionsToDFA, self.sharedContextCache)
         self._predicates = None
 
@@ -551,54 +574,54 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def contextDeclaration(self):
-            return self.getTypedRuleContext(OCLsParser.ContextDeclarationContext,0)
+            return self.getTypedRuleContext(BOCLParser.ContextDeclarationContext,0)
 
 
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_oclFile
+            return BOCLParser.RULE_oclFile
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOclFile" ):
                 listener.enterOclFile(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOclFile" ):
                 listener.exitOclFile(self)
 
 
 
 
     def oclFile(self):
 
-        localctx = OCLsParser.OclFileContext(self, self._ctx, self.state)
+        localctx = BOCLParser.OclFileContext(self, self._ctx, self.state)
         self.enterRule(localctx, 0, self.RULE_oclFile)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 28
-            self.contextDeclaration()
             self.state = 32
+            self.contextDeclaration()
+            self.state = 36
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                self.state = 29
+            while (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                self.state = 33
                 self.expression()
-                self.state = 34
+                self.state = 38
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -612,230 +635,230 @@
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_contextDeclaration
+            return BOCLParser.RULE_contextDeclaration
 
      
         def copyFrom(self, ctx:ParserRuleContext):
             super().copyFrom(ctx)
 
 
 
     class ContextExpContext(ContextDeclarationContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ContextDeclarationContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ContextDeclarationContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def CONTEXT(self):
-            return self.getToken(OCLsParser.CONTEXT, 0)
+            return self.getToken(BOCLParser.CONTEXT, 0)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def COLON(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COLON)
+                return self.getTokens(BOCLParser.COLON)
             else:
-                return self.getToken(OCLsParser.COLON, i)
+                return self.getToken(BOCLParser.COLON, i)
         def type_(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.TypeContext)
+                return self.getTypedRuleContexts(BOCLParser.TypeContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.TypeContext,i)
+                return self.getTypedRuleContext(BOCLParser.TypeContext,i)
 
         def LBRACE(self):
-            return self.getToken(OCLsParser.LBRACE, 0)
+            return self.getToken(BOCLParser.LBRACE, 0)
         def constraint(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ConstraintContext)
+                return self.getTypedRuleContexts(BOCLParser.ConstraintContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ConstraintContext,i)
+                return self.getTypedRuleContext(BOCLParser.ConstraintContext,i)
 
         def RBRACE(self):
-            return self.getToken(OCLsParser.RBRACE, 0)
+            return self.getToken(BOCLParser.RBRACE, 0)
         def DoubleCOLON(self):
-            return self.getToken(OCLsParser.DoubleCOLON, 0)
+            return self.getToken(BOCLParser.DoubleCOLON, 0)
         def functionCall(self):
-            return self.getTypedRuleContext(OCLsParser.FunctionCallContext,0)
+            return self.getTypedRuleContext(BOCLParser.FunctionCallContext,0)
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
         def DERIVE(self):
-            return self.getToken(OCLsParser.DERIVE, 0)
+            return self.getToken(BOCLParser.DERIVE, 0)
         def BODY(self):
-            return self.getToken(OCLsParser.BODY, 0)
+            return self.getToken(BOCLParser.BODY, 0)
         def Init(self):
-            return self.getToken(OCLsParser.Init, 0)
+            return self.getToken(BOCLParser.Init, 0)
         def PRE(self):
-            return self.getToken(OCLsParser.PRE, 0)
+            return self.getToken(BOCLParser.PRE, 0)
         def POST(self):
-            return self.getToken(OCLsParser.POST, 0)
+            return self.getToken(BOCLParser.POST, 0)
         def Def(self):
-            return self.getToken(OCLsParser.Def, 0)
+            return self.getToken(BOCLParser.Def, 0)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterContextExp" ):
                 listener.enterContextExp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitContextExp" ):
                 listener.exitContextExp(self)
 
 
 
     def contextDeclaration(self):
 
-        localctx = OCLsParser.ContextDeclarationContext(self, self._ctx, self.state)
+        localctx = BOCLParser.ContextDeclarationContext(self, self._ctx, self.state)
         self.enterRule(localctx, 2, self.RULE_contextDeclaration)
         self._la = 0 # Token type
         try:
-            localctx = OCLsParser.ContextExpContext(self, localctx)
+            localctx = BOCLParser.ContextExpContext(self, localctx)
             self.enterOuterAlt(localctx, 1)
-            self.state = 35
-            self.match(OCLsParser.CONTEXT)
-            self.state = 36
-            self.match(OCLsParser.ID)
             self.state = 39
+            self.match(BOCLParser.CONTEXT)
+            self.state = 40
+            self.match(BOCLParser.ID)
+            self.state = 43
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,1,self._ctx)
             if la_ == 1:
-                self.state = 37
-                self.match(OCLsParser.COLON)
-                self.state = 38
+                self.state = 41
+                self.match(BOCLParser.COLON)
+                self.state = 42
                 self.type_()
 
 
-            self.state = 42
+            self.state = 46
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==17:
-                self.state = 41
-                self.match(OCLsParser.LBRACE)
+            if _la==18:
+                self.state = 45
+                self.match(BOCLParser.LBRACE)
 
 
-            self.state = 47
+            self.state = 51
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input,3,self._ctx)
             while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                 if _alt==1:
-                    self.state = 44
+                    self.state = 48
                     self.constraint() 
-                self.state = 49
+                self.state = 53
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input,3,self._ctx)
 
-            self.state = 51
+            self.state = 55
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==18:
-                self.state = 50
-                self.match(OCLsParser.RBRACE)
+            if _la==19:
+                self.state = 54
+                self.match(BOCLParser.RBRACE)
 
 
-            self.state = 54
+            self.state = 58
             self._errHandler.sync(self)
-            _la = self._input.LA(1)
-            if _la==14:
-                self.state = 53
-                self.match(OCLsParser.DoubleCOLON)
+            la_ = self._interp.adaptivePredict(self._input,5,self._ctx)
+            if la_ == 1:
+                self.state = 57
+                self.match(BOCLParser.DoubleCOLON)
 
 
-            self.state = 57
+            self.state = 61
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,6,self._ctx)
             if la_ == 1:
-                self.state = 56
+                self.state = 60
                 self.functionCall()
 
 
-            self.state = 60
+            self.state = 64
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,7,self._ctx)
             if la_ == 1:
-                self.state = 59
-                self.match(OCLsParser.COLON)
+                self.state = 63
+                self.match(BOCLParser.COLON)
 
 
-            self.state = 63
+            self.state = 67
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,8,self._ctx)
             if la_ == 1:
-                self.state = 62
+                self.state = 66
                 self.type_()
 
 
-            self.state = 66
+            self.state = 70
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,9,self._ctx)
             if la_ == 1:
-                self.state = 65
-                self.match(OCLsParser.LPAREN)
+                self.state = 69
+                self.match(BOCLParser.LPAREN)
 
 
-            self.state = 69
+            self.state = 73
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,10,self._ctx)
             if la_ == 1:
-                self.state = 68
-                self.match(OCLsParser.ID)
+                self.state = 72
+                self.match(BOCLParser.ID)
 
 
-            self.state = 72
+            self.state = 76
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==16:
-                self.state = 71
-                self.match(OCLsParser.RPAREN)
+            if _la==17:
+                self.state = 75
+                self.match(BOCLParser.RPAREN)
 
 
-            self.state = 75
+            self.state = 79
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,12,self._ctx)
             if la_ == 1:
-                self.state = 74
-                self.match(OCLsParser.COLON)
+                self.state = 78
+                self.match(BOCLParser.COLON)
 
 
-            self.state = 78
+            self.state = 82
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,13,self._ctx)
             if la_ == 1:
-                self.state = 77
+                self.state = 81
                 _la = self._input.LA(1)
-                if not(_la==3 or _la==4 or ((((_la - 68)) & ~0x3f) == 0 and ((1 << (_la - 68)) & 263) != 0)):
+                if not(_la==4 or _la==5 or ((((_la - 69)) & ~0x3f) == 0 and ((1 << (_la - 69)) & 263) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
 
 
-            self.state = 81
+            self.state = 85
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==20:
-                self.state = 80
-                self.match(OCLsParser.COLON)
+            if _la==21:
+                self.state = 84
+                self.match(BOCLParser.COLON)
 
 
-            self.state = 84
+            self.state = 88
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,15,self._ctx)
             if la_ == 1:
-                self.state = 83
+                self.state = 87
                 self.expression()
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -848,81 +871,81 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def COLON(self):
-            return self.getToken(OCLsParser.COLON, 0)
+            return self.getToken(BOCLParser.COLON, 0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def INV(self):
-            return self.getToken(OCLsParser.INV, 0)
+            return self.getToken(BOCLParser.INV, 0)
 
         def PRE(self):
-            return self.getToken(OCLsParser.PRE, 0)
+            return self.getToken(BOCLParser.PRE, 0)
 
         def POST(self):
-            return self.getToken(OCLsParser.POST, 0)
+            return self.getToken(BOCLParser.POST, 0)
 
         def ID(self):
-            return self.getToken(OCLsParser.ID, 0)
+            return self.getToken(BOCLParser.ID, 0)
 
         def SEMI(self):
-            return self.getToken(OCLsParser.SEMI, 0)
+            return self.getToken(BOCLParser.SEMI, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_constraint
+            return BOCLParser.RULE_constraint
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterConstraint" ):
                 listener.enterConstraint(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitConstraint" ):
                 listener.exitConstraint(self)
 
 
 
 
     def constraint(self):
 
-        localctx = OCLsParser.ConstraintContext(self, self._ctx, self.state)
+        localctx = BOCLParser.ConstraintContext(self, self._ctx, self.state)
         self.enterRule(localctx, 4, self.RULE_constraint)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 86
+            self.state = 90
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 28) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 56) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
-            self.state = 88
+            self.state = 92
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==77:
-                self.state = 87
-                self.match(OCLsParser.ID)
+            if _la==78:
+                self.state = 91
+                self.match(BOCLParser.ID)
 
 
-            self.state = 90
-            self.match(OCLsParser.COLON)
-            self.state = 91
+            self.state = 94
+            self.match(BOCLParser.COLON)
+            self.state = 95
             self.expression()
-            self.state = 93
+            self.state = 97
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            if _la==19:
-                self.state = 92
-                self.match(OCLsParser.SEMI)
+            if _la==20:
+                self.state = 96
+                self.match(BOCLParser.SEMI)
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -935,170 +958,170 @@
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
 
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
 
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
 
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def COLON(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COLON)
+                return self.getTokens(BOCLParser.COLON)
             else:
-                return self.getToken(OCLsParser.COLON, i)
+                return self.getToken(BOCLParser.COLON, i)
 
         def NUMBER(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.NUMBER)
+                return self.getTokens(BOCLParser.NUMBER)
             else:
-                return self.getToken(OCLsParser.NUMBER, i)
+                return self.getToken(BOCLParser.NUMBER, i)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_functionCall
+            return BOCLParser.RULE_functionCall
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterFunctionCall" ):
                 listener.enterFunctionCall(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitFunctionCall" ):
                 listener.exitFunctionCall(self)
 
 
 
 
     def functionCall(self):
 
-        localctx = OCLsParser.FunctionCallContext(self, self._ctx, self.state)
+        localctx = BOCLParser.FunctionCallContext(self, self._ctx, self.state)
         self.enterRule(localctx, 6, self.RULE_functionCall)
         self._la = 0 # Token type
         try:
-            self.state = 135
+            self.state = 139
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,25,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 95
-                self.match(OCLsParser.ID)
-                self.state = 96
-                self.match(OCLsParser.LPAREN)
-                self.state = 109
+                self.state = 99
+                self.match(BOCLParser.ID)
+                self.state = 100
+                self.match(BOCLParser.LPAREN)
+                self.state = 113
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                    self.state = 98
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 102
                     self._errHandler.sync(self)
                     la_ = self._interp.adaptivePredict(self._input,18,self._ctx)
                     if la_ == 1:
-                        self.state = 97
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 101
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 100
+                    self.state = 104
                     self.expression()
-                    self.state = 102
+                    self.state = 106
                     self._errHandler.sync(self)
                     la_ = self._interp.adaptivePredict(self._input,19,self._ctx)
                     if la_ == 1:
-                        self.state = 101
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 105
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 105
+                    self.state = 109
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 104
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 108
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 111
+                    self.state = 115
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 112
-                self.match(OCLsParser.RPAREN)
+                self.state = 116
+                self.match(BOCLParser.RPAREN)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 113
-                self.match(OCLsParser.ID)
-                self.state = 114
-                self.match(OCLsParser.LPAREN)
-                self.state = 120
+                self.state = 117
+                self.match(BOCLParser.ID)
+                self.state = 118
+                self.match(BOCLParser.LPAREN)
+                self.state = 124
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==77:
-                    self.state = 115
-                    self.match(OCLsParser.ID)
-                    self.state = 116
-                    self.match(OCLsParser.COLON)
-                    self.state = 117
-                    self.match(OCLsParser.ID)
-                    self.state = 122
+                while _la==78:
+                    self.state = 119
+                    self.match(BOCLParser.ID)
+                    self.state = 120
+                    self.match(BOCLParser.COLON)
+                    self.state = 121
+                    self.match(BOCLParser.ID)
+                    self.state = 126
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 123
-                self.match(OCLsParser.RPAREN)
+                self.state = 127
+                self.match(BOCLParser.RPAREN)
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 124
-                self.match(OCLsParser.LPAREN)
-                self.state = 131
+                self.state = 128
+                self.match(BOCLParser.LPAREN)
+                self.state = 135
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==78:
-                    self.state = 125
-                    self.match(OCLsParser.NUMBER)
-                    self.state = 127
+                while _la==79:
+                    self.state = 129
+                    self.match(BOCLParser.NUMBER)
+                    self.state = 131
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 126
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 130
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 133
+                    self.state = 137
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 134
-                self.match(OCLsParser.RPAREN)
+                self.state = 138
+                self.match(BOCLParser.RPAREN)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1111,116 +1134,116 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def BOOLEAN_TYPE(self):
-            return self.getToken(OCLsParser.BOOLEAN_TYPE, 0)
+            return self.getToken(BOCLParser.BOOLEAN_TYPE, 0)
 
         def INTEGER_TYPE(self):
-            return self.getToken(OCLsParser.INTEGER_TYPE, 0)
+            return self.getToken(BOCLParser.INTEGER_TYPE, 0)
 
         def REAL_TYPE(self):
-            return self.getToken(OCLsParser.REAL_TYPE, 0)
+            return self.getToken(BOCLParser.REAL_TYPE, 0)
 
         def STRING_TYPE(self):
-            return self.getToken(OCLsParser.STRING_TYPE, 0)
+            return self.getToken(BOCLParser.STRING_TYPE, 0)
 
         def OCLANY(self):
-            return self.getToken(OCLsParser.OCLANY, 0)
+            return self.getToken(BOCLParser.OCLANY, 0)
 
         def OCLVOID(self):
-            return self.getToken(OCLsParser.OCLVOID, 0)
+            return self.getToken(BOCLParser.OCLVOID, 0)
 
         def collectionType(self):
-            return self.getTypedRuleContext(OCLsParser.CollectionTypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.CollectionTypeContext,0)
 
 
         def userDefinedType(self):
-            return self.getTypedRuleContext(OCLsParser.UserDefinedTypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.UserDefinedTypeContext,0)
 
 
         def SET(self):
-            return self.getToken(OCLsParser.SET, 0)
+            return self.getToken(BOCLParser.SET, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_type
+            return BOCLParser.RULE_type
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterType" ):
                 listener.enterType(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitType" ):
                 listener.exitType(self)
 
 
 
 
     def type_(self):
 
-        localctx = OCLsParser.TypeContext(self, self._ctx, self.state)
+        localctx = BOCLParser.TypeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 8, self.RULE_type)
         try:
-            self.state = 146
+            self.state = 150
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input,26,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 137
-                self.match(OCLsParser.BOOLEAN_TYPE)
+                self.state = 141
+                self.match(BOCLParser.BOOLEAN_TYPE)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 138
-                self.match(OCLsParser.INTEGER_TYPE)
+                self.state = 142
+                self.match(BOCLParser.INTEGER_TYPE)
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 139
-                self.match(OCLsParser.REAL_TYPE)
+                self.state = 143
+                self.match(BOCLParser.REAL_TYPE)
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 140
-                self.match(OCLsParser.STRING_TYPE)
+                self.state = 144
+                self.match(BOCLParser.STRING_TYPE)
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 141
-                self.match(OCLsParser.OCLANY)
+                self.state = 145
+                self.match(BOCLParser.OCLANY)
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 142
-                self.match(OCLsParser.OCLVOID)
+                self.state = 146
+                self.match(BOCLParser.OCLVOID)
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 143
+                self.state = 147
                 self.collectionType()
                 pass
 
             elif la_ == 8:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 144
+                self.state = 148
                 self.userDefinedType()
                 pass
 
             elif la_ == 9:
                 self.enterOuterAlt(localctx, 9)
-                self.state = 145
-                self.match(OCLsParser.SET)
+                self.state = 149
+                self.match(BOCLParser.SET)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -1233,100 +1256,100 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def SET(self):
-            return self.getToken(OCLsParser.SET, 0)
+            return self.getToken(BOCLParser.SET, 0)
 
         def LT(self):
-            return self.getToken(OCLsParser.LT, 0)
+            return self.getToken(BOCLParser.LT, 0)
 
         def type_(self):
-            return self.getTypedRuleContext(OCLsParser.TypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.TypeContext,0)
 
 
         def GT(self):
-            return self.getToken(OCLsParser.GT, 0)
+            return self.getToken(BOCLParser.GT, 0)
 
         def BAG(self):
-            return self.getToken(OCLsParser.BAG, 0)
+            return self.getToken(BOCLParser.BAG, 0)
 
         def SEQUENCE(self):
-            return self.getToken(OCLsParser.SEQUENCE, 0)
+            return self.getToken(BOCLParser.SEQUENCE, 0)
 
         def ORDEREDSET(self):
-            return self.getToken(OCLsParser.ORDEREDSET, 0)
+            return self.getToken(BOCLParser.ORDEREDSET, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_collectionType
+            return BOCLParser.RULE_collectionType
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterCollectionType" ):
                 listener.enterCollectionType(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCollectionType" ):
                 listener.exitCollectionType(self)
 
 
 
 
     def collectionType(self):
 
-        localctx = OCLsParser.CollectionTypeContext(self, self._ctx, self.state)
+        localctx = BOCLParser.CollectionTypeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 10, self.RULE_collectionType)
         try:
-            self.state = 168
+            self.state = 172
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [42]:
+            if token in [43]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 148
-                self.match(OCLsParser.SET)
-                self.state = 149
-                self.match(OCLsParser.LT)
-                self.state = 150
-                self.type_()
-                self.state = 151
-                self.match(OCLsParser.GT)
-                pass
-            elif token in [43]:
-                self.enterOuterAlt(localctx, 2)
+                self.state = 152
+                self.match(BOCLParser.SET)
                 self.state = 153
-                self.match(OCLsParser.BAG)
+                self.match(BOCLParser.LT)
                 self.state = 154
-                self.match(OCLsParser.LT)
-                self.state = 155
                 self.type_()
-                self.state = 156
-                self.match(OCLsParser.GT)
+                self.state = 155
+                self.match(BOCLParser.GT)
                 pass
             elif token in [44]:
-                self.enterOuterAlt(localctx, 3)
+                self.enterOuterAlt(localctx, 2)
+                self.state = 157
+                self.match(BOCLParser.BAG)
                 self.state = 158
-                self.match(OCLsParser.SEQUENCE)
+                self.match(BOCLParser.LT)
                 self.state = 159
-                self.match(OCLsParser.LT)
-                self.state = 160
                 self.type_()
-                self.state = 161
-                self.match(OCLsParser.GT)
+                self.state = 160
+                self.match(BOCLParser.GT)
                 pass
             elif token in [45]:
-                self.enterOuterAlt(localctx, 4)
+                self.enterOuterAlt(localctx, 3)
+                self.state = 162
+                self.match(BOCLParser.SEQUENCE)
                 self.state = 163
-                self.match(OCLsParser.ORDEREDSET)
+                self.match(BOCLParser.LT)
                 self.state = 164
-                self.match(OCLsParser.LT)
+                self.type_()
                 self.state = 165
+                self.match(BOCLParser.GT)
+                pass
+            elif token in [46]:
+                self.enterOuterAlt(localctx, 4)
+                self.state = 167
+                self.match(BOCLParser.ORDEREDSET)
+                self.state = 168
+                self.match(BOCLParser.LT)
+                self.state = 169
                 self.type_()
-                self.state = 166
-                self.match(OCLsParser.GT)
+                self.state = 170
+                self.match(BOCLParser.GT)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -1340,38 +1363,38 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def ID(self):
-            return self.getToken(OCLsParser.ID, 0)
+            return self.getToken(BOCLParser.ID, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_userDefinedType
+            return BOCLParser.RULE_userDefinedType
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterUserDefinedType" ):
                 listener.enterUserDefinedType(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitUserDefinedType" ):
                 listener.exitUserDefinedType(self)
 
 
 
 
     def userDefinedType(self):
 
-        localctx = OCLsParser.UserDefinedTypeContext(self, self._ctx, self.state)
+        localctx = BOCLParser.UserDefinedTypeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 12, self.RULE_userDefinedType)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 170
-            self.match(OCLsParser.ID)
+            self.state = 174
+            self.match(BOCLParser.ID)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
@@ -1382,3164 +1405,3479 @@
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_expression
+            return BOCLParser.RULE_expression
 
      
         def copyFrom(self, ctx:ParserRuleContext):
             super().copyFrom(ctx)
 
 
 
+    class ElseExpContext(ExpressionContext):
+
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
+            super().__init__(parser)
+            self.copyFrom(ctx)
+
+        def ELSE(self):
+            return self.getToken(BOCLParser.ELSE, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterElseExp" ):
+                listener.enterElseExp(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitElseExp" ):
+                listener.exitElseExp(self)
+
+
     class ArrowexpContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterArrowexp" ):
                 listener.enterArrowexp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitArrowexp" ):
                 listener.exitArrowexp(self)
 
 
     class COLLECTIONContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def PIPE(self):
-            return self.getToken(OCLsParser.PIPE, 0)
-        def expression(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
-            else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+            return self.getToken(BOCLParser.PIPE, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def FORALL(self):
-            return self.getToken(OCLsParser.FORALL, 0)
+            return self.getToken(BOCLParser.FORALL, 0)
         def EXISTS(self):
-            return self.getToken(OCLsParser.EXISTS, 0)
+            return self.getToken(BOCLParser.EXISTS, 0)
         def SELECT(self):
-            return self.getToken(OCLsParser.SELECT, 0)
+            return self.getToken(BOCLParser.SELECT, 0)
         def COLLECT(self):
-            return self.getToken(OCLsParser.COLLECT, 0)
+            return self.getToken(BOCLParser.COLLECT, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
+        def endExpression(self):
+            return self.getTypedRuleContext(BOCLParser.EndExpressionContext,0)
+
         def COLON(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COLON)
+                return self.getTokens(BOCLParser.COLON)
             else:
-                return self.getToken(OCLsParser.COLON, i)
+                return self.getToken(BOCLParser.COLON, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterCOLLECTION" ):
                 listener.enterCOLLECTION(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCOLLECTION" ):
                 listener.exitCOLLECTION(self)
 
 
     class SETContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def SET(self):
-            return self.getToken(OCLsParser.SET, 0)
+            return self.getToken(BOCLParser.SET, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def LBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LBRACE)
+                return self.getTokens(BOCLParser.LBRACE)
             else:
-                return self.getToken(OCLsParser.LBRACE, i)
+                return self.getToken(BOCLParser.LBRACE, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RBRACE)
+                return self.getTokens(BOCLParser.RBRACE)
             else:
-                return self.getToken(OCLsParser.RBRACE, i)
+                return self.getToken(BOCLParser.RBRACE, i)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSET" ):
                 listener.enterSET(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSET" ):
                 listener.exitSET(self)
 
 
     class DefIDAssignmentexpressionContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def COLON(self):
-            return self.getToken(OCLsParser.COLON, 0)
+            return self.getToken(BOCLParser.COLON, 0)
         def EQUAL(self):
-            return self.getToken(OCLsParser.EQUAL, 0)
+            return self.getToken(BOCLParser.EQUAL, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterDefIDAssignmentexpression" ):
                 listener.enterDefIDAssignmentexpression(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDefIDAssignmentexpression" ):
                 listener.exitDefIDAssignmentexpression(self)
 
 
     class PredefinedfunctionCallContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def functionCall(self):
-            return self.getTypedRuleContext(OCLsParser.FunctionCallContext,0)
+            return self.getTypedRuleContext(BOCLParser.FunctionCallContext,0)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPredefinedfunctionCall" ):
                 listener.enterPredefinedfunctionCall(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitPredefinedfunctionCall" ):
                 listener.exitPredefinedfunctionCall(self)
 
 
     class UnaryContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def unaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.UnaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.UnaryExpressionContext,0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterUnary" ):
                 listener.enterUnary(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitUnary" ):
                 listener.exitUnary(self)
 
 
     class INCLUDESContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def INCLUDES(self):
-            return self.getToken(OCLsParser.INCLUDES, 0)
+            return self.getToken(BOCLParser.INCLUDES, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterINCLUDES" ):
                 listener.enterINCLUDES(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitINCLUDES" ):
                 listener.exitINCLUDES(self)
 
 
+    class ThenExpContext(ExpressionContext):
+
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
+            super().__init__(parser)
+            self.copyFrom(ctx)
+
+        def THEN(self):
+            return self.getToken(BOCLParser.THEN, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterThenExp" ):
+                listener.enterThenExp(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitThenExp" ):
+                listener.exitThenExp(self)
+
+
     class SUBORDEREDSETContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def SUBORDEREDSET(self):
-            return self.getToken(OCLsParser.SUBORDEREDSET, 0)
+            return self.getToken(BOCLParser.SUBORDEREDSET, 0)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def LBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LBRACE)
+                return self.getTokens(BOCLParser.LBRACE)
             else:
-                return self.getToken(OCLsParser.LBRACE, i)
+                return self.getToken(BOCLParser.LBRACE, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RBRACE)
+                return self.getTokens(BOCLParser.RBRACE)
             else:
-                return self.getToken(OCLsParser.RBRACE, i)
+                return self.getToken(BOCLParser.RBRACE, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSUBORDEREDSET" ):
                 listener.enterSUBORDEREDSET(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSUBORDEREDSET" ):
                 listener.exitSUBORDEREDSET(self)
 
 
     class PrimaryExpContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def primaryExpression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.PrimaryExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.PrimaryExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,i)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def operator(self):
-            return self.getTypedRuleContext(OCLsParser.OperatorContext,0)
+            return self.getTypedRuleContext(BOCLParser.OperatorContext,0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPrimaryExp" ):
                 listener.enterPrimaryExp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitPrimaryExp" ):
                 listener.exitPrimaryExp(self)
 
 
     class OCLISKINDOFContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def OCLISKINDOF(self):
-            return self.getToken(OCLsParser.OCLISKINDOF, 0)
+            return self.getToken(BOCLParser.OCLISKINDOF, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def type_(self):
-            return self.getTypedRuleContext(OCLsParser.TypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.TypeContext,0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOCLISKINDOF" ):
                 listener.enterOCLISKINDOF(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOCLISKINDOF" ):
                 listener.exitOCLISKINDOF(self)
 
 
     class NumberContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def NUMBER(self):
-            return self.getToken(OCLsParser.NUMBER, 0)
+            return self.getToken(BOCLParser.NUMBER, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterNumber" ):
                 listener.enterNumber(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitNumber" ):
                 listener.exitNumber(self)
 
 
+    class DoubleCOLONsContext(ExpressionContext):
+
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
+            super().__init__(parser)
+            self.copyFrom(ctx)
+
+        def DoubleCOLON(self):
+            return self.getToken(BOCLParser.DoubleCOLON, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+        def AND(self):
+            return self.getToken(BOCLParser.AND, 0)
+        def OR(self):
+            return self.getToken(BOCLParser.OR, 0)
+        def ID(self):
+            return self.getToken(BOCLParser.ID, 0)
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterDoubleCOLONs" ):
+                listener.enterDoubleCOLONs(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitDoubleCOLONs" ):
+                listener.exitDoubleCOLONs(self)
+
+
     class SYMMETRICDIFFERENCEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def SYMMETRICDIFFERENCE(self):
-            return self.getToken(OCLsParser.SYMMETRICDIFFERENCE, 0)
+            return self.getToken(BOCLParser.SYMMETRICDIFFERENCE, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSYMMETRICDIFFERENCE" ):
                 listener.enterSYMMETRICDIFFERENCE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSYMMETRICDIFFERENCE" ):
                 listener.exitSYMMETRICDIFFERENCE(self)
 
 
     class SEQUENCEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def SEQUENCE(self):
-            return self.getToken(OCLsParser.SEQUENCE, 0)
+            return self.getToken(BOCLParser.SEQUENCE, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def LBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LBRACE)
+                return self.getTokens(BOCLParser.LBRACE)
             else:
-                return self.getToken(OCLsParser.LBRACE, i)
+                return self.getToken(BOCLParser.LBRACE, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RBRACE)
+                return self.getTokens(BOCLParser.RBRACE)
             else:
-                return self.getToken(OCLsParser.RBRACE, i)
+                return self.getToken(BOCLParser.RBRACE, i)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSEQUENCE" ):
                 listener.enterSEQUENCE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSEQUENCE" ):
                 listener.exitSEQUENCE(self)
 
 
     class ORDEREDSETContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def ORDEREDSET(self):
-            return self.getToken(OCLsParser.ORDEREDSET, 0)
+            return self.getToken(BOCLParser.ORDEREDSET, 0)
         def LBRACE(self):
-            return self.getToken(OCLsParser.LBRACE, 0)
+            return self.getToken(BOCLParser.LBRACE, 0)
         def RBRACE(self):
-            return self.getToken(OCLsParser.RBRACE, 0)
+            return self.getToken(BOCLParser.RBRACE, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterORDEREDSET" ):
                 listener.enterORDEREDSET(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitORDEREDSET" ):
                 listener.exitORDEREDSET(self)
 
 
     class DoubleDotsContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def DoubleDots(self):
-            return self.getToken(OCLsParser.DoubleDots, 0)
+            return self.getToken(BOCLParser.DoubleDots, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterDoubleDots" ):
                 listener.enterDoubleDots(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDoubleDots" ):
                 listener.exitDoubleDots(self)
 
 
     class EXCLUDESContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def EXCLUDES(self):
-            return self.getToken(OCLsParser.EXCLUDES, 0)
+            return self.getToken(BOCLParser.EXCLUDES, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterEXCLUDES" ):
                 listener.enterEXCLUDES(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitEXCLUDES" ):
                 listener.exitEXCLUDES(self)
 
 
     class DERIVEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def DERIVE(self):
-            return self.getToken(OCLsParser.DERIVE, 0)
+            return self.getToken(BOCLParser.DERIVE, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterDERIVE" ):
                 listener.enterDERIVE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDERIVE" ):
                 listener.exitDERIVE(self)
 
 
     class IDContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterID" ):
                 listener.enterID(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitID" ):
                 listener.exitID(self)
 
 
     class ALLINSTANCESContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def ALLINSTANCES(self):
-            return self.getToken(OCLsParser.ALLINSTANCES, 0)
-        def expression(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
-            else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
-
+            return self.getToken(BOCLParser.ALLINSTANCES, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
+            else:
+                return self.getToken(BOCLParser.LPAREN, i)
+        def expression(self, i:int=None):
+            if i is None:
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
+
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterALLINSTANCES" ):
                 listener.enterALLINSTANCES(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitALLINSTANCES" ):
                 listener.exitALLINSTANCES(self)
 
 
-    class IfContext(ExpressionContext):
-
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
-            super().__init__(parser)
-            self.copyFrom(ctx)
-
-        def IF(self):
-            return self.getToken(OCLsParser.IF, 0)
-        def expression(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
-            else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
-
-        def THEN(self):
-            return self.getToken(OCLsParser.THEN, 0)
-        def ELSE(self):
-            return self.getToken(OCLsParser.ELSE, 0)
-        def ENDIF(self):
-            return self.getToken(OCLsParser.ENDIF, 0)
-
-        def enterRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "enterIf" ):
-                listener.enterIf(self)
-
-        def exitRule(self, listener:ParseTreeListener):
-            if hasattr( listener, "exitIf" ):
-                listener.exitIf(self)
-
-
     class OpContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def operator(self):
-            return self.getTypedRuleContext(OCLsParser.OperatorContext,0)
+            return self.getTypedRuleContext(BOCLParser.OperatorContext,0)
 
         def numberORUserDefined(self):
-            return self.getTypedRuleContext(OCLsParser.NumberORUserDefinedContext,0)
+            return self.getTypedRuleContext(BOCLParser.NumberORUserDefinedContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOp" ):
                 listener.enterOp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOp" ):
                 listener.exitOp(self)
 
 
     class SUBSEQUENCEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def SUBSEQUENCE(self):
-            return self.getToken(OCLsParser.SUBSEQUENCE, 0)
+            return self.getToken(BOCLParser.SUBSEQUENCE, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def LBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LBRACE)
+                return self.getTokens(BOCLParser.LBRACE)
             else:
-                return self.getToken(OCLsParser.LBRACE, i)
+                return self.getToken(BOCLParser.LBRACE, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def RBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RBRACE)
+                return self.getTokens(BOCLParser.RBRACE)
             else:
-                return self.getToken(OCLsParser.RBRACE, i)
+                return self.getToken(BOCLParser.RBRACE, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSUBSEQUENCE" ):
                 listener.enterSUBSEQUENCE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSUBSEQUENCE" ):
                 listener.exitSUBSEQUENCE(self)
 
 
     class SIZEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def SIZE(self):
-            return self.getToken(OCLsParser.SIZE, 0)
+            return self.getToken(BOCLParser.SIZE, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
+        def binaryFunctionCall(self):
+            return self.getTypedRuleContext(BOCLParser.BinaryFunctionCallContext,0)
+
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSIZE" ):
                 listener.enterSIZE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSIZE" ):
                 listener.exitSIZE(self)
 
 
     class SingleQuoteExpContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSingleQuoteExp" ):
                 listener.enterSingleQuoteExp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSingleQuoteExp" ):
                 listener.exitSingleQuoteExp(self)
 
 
     class BAGContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def BAG(self):
-            return self.getToken(OCLsParser.BAG, 0)
+            return self.getToken(BOCLParser.BAG, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def LBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LBRACE)
+                return self.getTokens(BOCLParser.LBRACE)
             else:
-                return self.getToken(OCLsParser.LBRACE, i)
+                return self.getToken(BOCLParser.LBRACE, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RBRACE(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RBRACE)
+                return self.getTokens(BOCLParser.RBRACE)
             else:
-                return self.getToken(OCLsParser.RBRACE, i)
+                return self.getToken(BOCLParser.RBRACE, i)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterBAG" ):
                 listener.enterBAG(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitBAG" ):
                 listener.exitBAG(self)
 
 
     class OCLISTYPEOFContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def OCLISTYPEOF(self):
-            return self.getToken(OCLsParser.OCLISTYPEOF, 0)
+            return self.getToken(BOCLParser.OCLISTYPEOF, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def type_(self):
-            return self.getTypedRuleContext(OCLsParser.TypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.TypeContext,0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOCLISTYPEOF" ):
                 listener.enterOCLISTYPEOF(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOCLISTYPEOF" ):
                 listener.exitOCLISTYPEOF(self)
 
 
     class SUMContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def SUM(self):
-            return self.getToken(OCLsParser.SUM, 0)
+            return self.getToken(BOCLParser.SUM, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
+        def binaryFunctionCall(self):
+            return self.getTypedRuleContext(BOCLParser.BinaryFunctionCallContext,0)
+
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterSUM" ):
                 listener.enterSUM(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitSUM" ):
                 listener.exitSUM(self)
 
 
     class FIRSTContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def FIRST(self):
-            return self.getToken(OCLsParser.FIRST, 0)
+            return self.getToken(BOCLParser.FIRST, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterFIRST" ):
                 listener.enterFIRST(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitFIRST" ):
                 listener.exitFIRST(self)
 
 
     class APPENDContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def APPEND(self):
-            return self.getToken(OCLsParser.APPEND, 0)
+            return self.getToken(BOCLParser.APPEND, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterAPPEND" ):
                 listener.enterAPPEND(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitAPPEND" ):
                 listener.exitAPPEND(self)
 
 
     class OCLASTYPEContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def OCLASTYPE(self):
-            return self.getToken(OCLsParser.OCLASTYPE, 0)
+            return self.getToken(BOCLParser.OCLASTYPE, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def type_(self):
-            return self.getTypedRuleContext(OCLsParser.TypeContext,0)
+            return self.getTypedRuleContext(BOCLParser.TypeContext,0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOCLASTYPE" ):
                 listener.enterOCLASTYPE(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOCLASTYPE" ):
                 listener.exitOCLASTYPE(self)
 
 
     class CollectionExpressionVariableContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
-        def expression(self, i:int=None):
-            if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
-            else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+            return self.getToken(BOCLParser.LPAREN, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
         def FORALL(self):
-            return self.getToken(OCLsParser.FORALL, 0)
+            return self.getToken(BOCLParser.FORALL, 0)
         def EXISTS(self):
-            return self.getToken(OCLsParser.EXISTS, 0)
+            return self.getToken(BOCLParser.EXISTS, 0)
         def SELECT(self):
-            return self.getToken(OCLsParser.SELECT, 0)
+            return self.getToken(BOCLParser.SELECT, 0)
         def COLLECT(self):
-            return self.getToken(OCLsParser.COLLECT, 0)
+            return self.getToken(BOCLParser.COLLECT, 0)
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
+        def endExpression(self):
+            return self.getTypedRuleContext(BOCLParser.EndExpressionContext,0)
+
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterCollectionExpressionVariable" ):
                 listener.enterCollectionExpressionVariable(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitCollectionExpressionVariable" ):
                 listener.exitCollectionExpressionVariable(self)
 
 
     class LASTContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def LAST(self):
-            return self.getToken(OCLsParser.LAST, 0)
+            return self.getToken(BOCLParser.LAST, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterLAST" ):
                 listener.enterLAST(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitLAST" ):
                 listener.exitLAST(self)
 
 
     class BinaryContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def binaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.BinaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.BinaryExpressionContext,0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
         def AND(self):
-            return self.getToken(OCLsParser.AND, 0)
+            return self.getToken(BOCLParser.AND, 0)
         def OR(self):
-            return self.getToken(OCLsParser.OR, 0)
+            return self.getToken(BOCLParser.OR, 0)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterBinary" ):
                 listener.enterBinary(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitBinary" ):
                 listener.exitBinary(self)
 
 
+    class IfExpContext(ExpressionContext):
+
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
+            super().__init__(parser)
+            self.copyFrom(ctx)
+
+        def IF(self):
+            return self.getToken(BOCLParser.IF, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterIfExp" ):
+                listener.enterIfExp(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitIfExp" ):
+                listener.exitIfExp(self)
+
+
+    class EndIfExpContext(ExpressionContext):
+
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
+            super().__init__(parser)
+            self.copyFrom(ctx)
+
+        def ENDIF(self):
+            return self.getToken(BOCLParser.ENDIF, 0)
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterEndIfExp" ):
+                listener.enterEndIfExp(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitEndIfExp" ):
+                listener.exitEndIfExp(self)
+
+
     class ISEMPTYContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def ISEMPTY(self):
-            return self.getToken(OCLsParser.ISEMPTY, 0)
+            return self.getToken(BOCLParser.ISEMPTY, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterISEMPTY" ):
                 listener.enterISEMPTY(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitISEMPTY" ):
                 listener.exitISEMPTY(self)
 
 
     class DefExpContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Def(self):
-            return self.getToken(OCLsParser.Def, 0)
+            return self.getToken(BOCLParser.Def, 0)
         def COLON(self):
-            return self.getToken(OCLsParser.COLON, 0)
+            return self.getToken(BOCLParser.COLON, 0)
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterDefExp" ):
                 listener.enterDefExp(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitDefExp" ):
                 listener.exitDefExp(self)
 
 
     class FuncCallContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def primaryExpression(self):
-            return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
 
         def functionCall(self):
-            return self.getTypedRuleContext(OCLsParser.FunctionCallContext,0)
+            return self.getTypedRuleContext(BOCLParser.FunctionCallContext,0)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
         def operator(self):
-            return self.getTypedRuleContext(OCLsParser.OperatorContext,0)
+            return self.getTypedRuleContext(BOCLParser.OperatorContext,0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterFuncCall" ):
                 listener.enterFuncCall(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitFuncCall" ):
                 listener.exitFuncCall(self)
 
 
     class UNIONContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def UNION(self):
-            return self.getToken(OCLsParser.UNION, 0)
+            return self.getToken(BOCLParser.UNION, 0)
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterUNION" ):
                 listener.enterUNION(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitUNION" ):
                 listener.exitUNION(self)
 
 
     class PREPENDContext(ExpressionContext):
 
-        def __init__(self, parser, ctx:ParserRuleContext): # actually a OCLsParser.ExpressionContext
+        def __init__(self, parser, ctx:ParserRuleContext): # actually a BOCLParser.ExpressionContext
             super().__init__(parser)
             self.copyFrom(ctx)
 
         def Arrow(self):
-            return self.getToken(OCLsParser.Arrow, 0)
+            return self.getToken(BOCLParser.Arrow, 0)
         def PREPEND(self):
-            return self.getToken(OCLsParser.PREPEND, 0)
+            return self.getToken(BOCLParser.PREPEND, 0)
         def LPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.LPAREN)
+                return self.getTokens(BOCLParser.LPAREN)
             else:
-                return self.getToken(OCLsParser.LPAREN, i)
+                return self.getToken(BOCLParser.LPAREN, i)
         def expression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.ExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.ExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.ExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.ExpressionContext,i)
 
         def RPAREN(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.RPAREN)
+                return self.getTokens(BOCLParser.RPAREN)
             else:
-                return self.getToken(OCLsParser.RPAREN, i)
+                return self.getToken(BOCLParser.RPAREN, i)
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
         def COMMA(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.COMMA)
+                return self.getTokens(BOCLParser.COMMA)
             else:
-                return self.getToken(OCLsParser.COMMA, i)
+                return self.getToken(BOCLParser.COMMA, i)
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPREPEND" ):
                 listener.enterPREPEND(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitPREPEND" ):
                 listener.exitPREPEND(self)
 
 
 
     def expression(self):
 
-        localctx = OCLsParser.ExpressionContext(self, self._ctx, self.state)
+        localctx = BOCLParser.ExpressionContext(self, self._ctx, self.state)
         self.enterRule(localctx, 14, self.RULE_expression)
         self._la = 0 # Token type
         try:
-            self.state = 883
+            self.state = 908
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,168,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,175,self._ctx)
             if la_ == 1:
-                localctx = OCLsParser.BinaryContext(self, localctx)
+                localctx = BOCLParser.BinaryContext(self, localctx)
                 self.enterOuterAlt(localctx, 1)
-                self.state = 173
+                self.state = 177
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==33 or _la==34:
-                    self.state = 172
+                if _la==34 or _la==35:
+                    self.state = 176
                     _la = self._input.LA(1)
-                    if not(_la==33 or _la==34):
+                    if not(_la==34 or _la==35):
                         self._errHandler.recoverInline(self)
                     else:
                         self._errHandler.reportMatch(self)
                         self.consume()
 
 
-                self.state = 175
+                self.state = 179
                 self.binaryExpression()
-                self.state = 177
+                self.state = 181
                 self._errHandler.sync(self)
                 la_ = self._interp.adaptivePredict(self._input,29,self._ctx)
                 if la_ == 1:
-                    self.state = 176
+                    self.state = 180
                     self.expression()
 
 
                 pass
 
             elif la_ == 2:
-                localctx = OCLsParser.UnaryContext(self, localctx)
+                localctx = BOCLParser.UnaryContext(self, localctx)
                 self.enterOuterAlt(localctx, 2)
-                self.state = 179
+                self.state = 183
                 self.unaryExpression()
-                self.state = 181
+                self.state = 185
                 self._errHandler.sync(self)
                 la_ = self._interp.adaptivePredict(self._input,30,self._ctx)
                 if la_ == 1:
-                    self.state = 180
+                    self.state = 184
                     self.expression()
 
 
                 pass
 
             elif la_ == 3:
-                localctx = OCLsParser.IfContext(self, localctx)
+                localctx = BOCLParser.IfExpContext(self, localctx)
                 self.enterOuterAlt(localctx, 3)
-                self.state = 183
-                self.match(OCLsParser.IF)
-                self.state = 184
-                self.expression()
-                self.state = 185
-                self.match(OCLsParser.THEN)
-                self.state = 186
-                self.expression()
                 self.state = 187
-                self.match(OCLsParser.ELSE)
+                self.match(BOCLParser.IF)
                 self.state = 188
                 self.expression()
-                self.state = 189
-                self.match(OCLsParser.ENDIF)
                 pass
 
             elif la_ == 4:
-                localctx = OCLsParser.OCLISTYPEOFContext(self, localctx)
+                localctx = BOCLParser.ThenExpContext(self, localctx)
                 self.enterOuterAlt(localctx, 4)
+                self.state = 189
+                self.match(BOCLParser.THEN)
+                self.state = 190
+                self.expression()
+                pass
+
+            elif la_ == 5:
+                localctx = BOCLParser.ElseExpContext(self, localctx)
+                self.enterOuterAlt(localctx, 5)
                 self.state = 191
+                self.match(BOCLParser.ELSE)
+                self.state = 192
+                self.expression()
+                pass
+
+            elif la_ == 6:
+                localctx = BOCLParser.EndIfExpContext(self, localctx)
+                self.enterOuterAlt(localctx, 6)
+                self.state = 193
+                self.match(BOCLParser.ENDIF)
+                self.state = 195
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,31,self._ctx)
+                if la_ == 1:
+                    self.state = 194
+                    self.expression()
+
+
+                pass
+
+            elif la_ == 7:
+                localctx = BOCLParser.OCLISTYPEOFContext(self, localctx)
+                self.enterOuterAlt(localctx, 7)
+                self.state = 197
                 self.primaryExpression()
-                self.state = 196
+                self.state = 202
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,31,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,32,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 192
-                        self.match(OCLsParser.DOT)
-                        self.state = 193
-                        self.match(OCLsParser.ID) 
-                    self.state = 198
-                    self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,31,self._ctx)
-
-                self.state = 199
-                self.match(OCLsParser.DOT)
-                self.state = 200
-                self.match(OCLsParser.OCLISTYPEOF)
-                self.state = 201
-                self.match(OCLsParser.LPAREN)
-                self.state = 202
-                self.type_()
-                self.state = 203
-                self.match(OCLsParser.RPAREN)
+                        self.state = 198
+                        self.match(BOCLParser.DOT)
+                        self.state = 199
+                        self.match(BOCLParser.ID) 
+                    self.state = 204
+                    self._errHandler.sync(self)
+                    _alt = self._interp.adaptivePredict(self._input,32,self._ctx)
+
                 self.state = 205
+                self.match(BOCLParser.DOT)
+                self.state = 206
+                self.match(BOCLParser.OCLISTYPEOF)
+                self.state = 207
+                self.match(BOCLParser.LPAREN)
+                self.state = 208
+                self.type_()
+                self.state = 209
+                self.match(BOCLParser.RPAREN)
+                self.state = 211
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,32,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,33,self._ctx)
                 if la_ == 1:
-                    self.state = 204
+                    self.state = 210
                     self.expression()
 
 
                 pass
 
-            elif la_ == 5:
-                localctx = OCLsParser.OCLASTYPEContext(self, localctx)
-                self.enterOuterAlt(localctx, 5)
-                self.state = 207
+            elif la_ == 8:
+                localctx = BOCLParser.OCLASTYPEContext(self, localctx)
+                self.enterOuterAlt(localctx, 8)
+                self.state = 213
                 self.primaryExpression()
-                self.state = 212
+                self.state = 218
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,33,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,34,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 208
-                        self.match(OCLsParser.DOT)
-                        self.state = 209
-                        self.match(OCLsParser.ID) 
-                    self.state = 214
-                    self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,33,self._ctx)
-
-                self.state = 215
-                self.match(OCLsParser.DOT)
-                self.state = 216
-                self.match(OCLsParser.OCLASTYPE)
-                self.state = 217
-                self.match(OCLsParser.LPAREN)
-                self.state = 218
-                self.type_()
-                self.state = 219
-                self.match(OCLsParser.RPAREN)
+                        self.state = 214
+                        self.match(BOCLParser.DOT)
+                        self.state = 215
+                        self.match(BOCLParser.ID) 
+                    self.state = 220
+                    self._errHandler.sync(self)
+                    _alt = self._interp.adaptivePredict(self._input,34,self._ctx)
+
                 self.state = 221
+                self.match(BOCLParser.DOT)
+                self.state = 222
+                self.match(BOCLParser.OCLASTYPE)
+                self.state = 223
+                self.match(BOCLParser.LPAREN)
+                self.state = 224
+                self.type_()
+                self.state = 225
+                self.match(BOCLParser.RPAREN)
+                self.state = 227
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,34,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,35,self._ctx)
                 if la_ == 1:
-                    self.state = 220
+                    self.state = 226
                     self.expression()
 
 
                 pass
 
-            elif la_ == 6:
-                localctx = OCLsParser.OCLISKINDOFContext(self, localctx)
-                self.enterOuterAlt(localctx, 6)
-                self.state = 223
+            elif la_ == 9:
+                localctx = BOCLParser.OCLISKINDOFContext(self, localctx)
+                self.enterOuterAlt(localctx, 9)
+                self.state = 229
                 self.primaryExpression()
-                self.state = 228
+                self.state = 234
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,35,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,36,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 224
-                        self.match(OCLsParser.DOT)
-                        self.state = 225
-                        self.match(OCLsParser.ID) 
-                    self.state = 230
-                    self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,35,self._ctx)
-
-                self.state = 231
-                self.match(OCLsParser.DOT)
-                self.state = 232
-                self.match(OCLsParser.OCLISKINDOF)
-                self.state = 233
-                self.match(OCLsParser.LPAREN)
-                self.state = 234
-                self.type_()
-                self.state = 235
-                self.match(OCLsParser.RPAREN)
+                        self.state = 230
+                        self.match(BOCLParser.DOT)
+                        self.state = 231
+                        self.match(BOCLParser.ID) 
+                    self.state = 236
+                    self._errHandler.sync(self)
+                    _alt = self._interp.adaptivePredict(self._input,36,self._ctx)
+
                 self.state = 237
+                self.match(BOCLParser.DOT)
+                self.state = 238
+                self.match(BOCLParser.OCLISKINDOF)
+                self.state = 239
+                self.match(BOCLParser.LPAREN)
+                self.state = 240
+                self.type_()
+                self.state = 241
+                self.match(BOCLParser.RPAREN)
+                self.state = 243
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,36,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,37,self._ctx)
                 if la_ == 1:
-                    self.state = 236
+                    self.state = 242
                     self.expression()
 
 
                 pass
 
-            elif la_ == 7:
-                localctx = OCLsParser.ISEMPTYContext(self, localctx)
-                self.enterOuterAlt(localctx, 7)
-                self.state = 240
+            elif la_ == 10:
+                localctx = BOCLParser.ISEMPTYContext(self, localctx)
+                self.enterOuterAlt(localctx, 10)
+                self.state = 246
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==5 or _la==15 or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 481) != 0):
-                    self.state = 239
+                if _la==6 or _la==16 or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 481) != 0):
+                    self.state = 245
                     self.primaryExpression()
 
 
-                self.state = 246
+                self.state = 252
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==22:
-                    self.state = 242
-                    self.match(OCLsParser.DOT)
-                    self.state = 243
-                    self.match(OCLsParser.ID)
+                while _la==23:
                     self.state = 248
+                    self.match(BOCLParser.DOT)
+                    self.state = 249
+                    self.match(BOCLParser.ID)
+                    self.state = 254
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 249
-                self.match(OCLsParser.Arrow)
-                self.state = 250
-                self.match(OCLsParser.ISEMPTY)
-                self.state = 251
-                self.match(OCLsParser.LPAREN)
-                self.state = 252
-                self.match(OCLsParser.RPAREN)
-                self.state = 254
+                self.state = 255
+                self.match(BOCLParser.Arrow)
+                self.state = 256
+                self.match(BOCLParser.ISEMPTY)
+                self.state = 257
+                self.match(BOCLParser.LPAREN)
+                self.state = 258
+                self.match(BOCLParser.RPAREN)
+                self.state = 260
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,39,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,40,self._ctx)
                 if la_ == 1:
-                    self.state = 253
+                    self.state = 259
                     self.expression()
 
 
-                self.state = 259
+                self.state = 265
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,40,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 256
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 261
+                        self.state = 262
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 267
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,40,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,41,self._ctx)
 
                 pass
 
-            elif la_ == 8:
-                localctx = OCLsParser.SUMContext(self, localctx)
-                self.enterOuterAlt(localctx, 8)
-                self.state = 263
+            elif la_ == 11:
+                localctx = BOCLParser.SUMContext(self, localctx)
+                self.enterOuterAlt(localctx, 11)
+                self.state = 269
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==5 or _la==15 or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 481) != 0):
-                    self.state = 262
+                if _la==6 or _la==16 or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 481) != 0):
+                    self.state = 268
                     self.primaryExpression()
 
 
-                self.state = 269
+                self.state = 275
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==22:
-                    self.state = 265
-                    self.match(OCLsParser.DOT)
-                    self.state = 266
-                    self.match(OCLsParser.ID)
+                while _la==23:
                     self.state = 271
+                    self.match(BOCLParser.DOT)
+                    self.state = 272
+                    self.match(BOCLParser.ID)
+                    self.state = 277
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 272
-                self.match(OCLsParser.Arrow)
-                self.state = 273
-                self.match(OCLsParser.SUM)
-                self.state = 274
-                self.match(OCLsParser.LPAREN)
-                self.state = 275
-                self.match(OCLsParser.RPAREN)
-                self.state = 277
+                self.state = 278
+                self.match(BOCLParser.Arrow)
+                self.state = 279
+                self.match(BOCLParser.SUM)
+                self.state = 280
+                self.match(BOCLParser.LPAREN)
+                self.state = 281
+                self.match(BOCLParser.RPAREN)
+                self.state = 283
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,44,self._ctx)
+                if la_ == 1:
+                    self.state = 282
+                    self.binaryFunctionCall()
+
+
+                self.state = 286
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,43,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,45,self._ctx)
                 if la_ == 1:
-                    self.state = 276
+                    self.state = 285
                     self.expression()
 
 
-                self.state = 282
+                self.state = 291
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 279
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 284
+                        self.state = 288
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 293
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,44,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,46,self._ctx)
 
                 pass
 
-            elif la_ == 9:
-                localctx = OCLsParser.SIZEContext(self, localctx)
-                self.enterOuterAlt(localctx, 9)
-                self.state = 286
+            elif la_ == 12:
+                localctx = BOCLParser.SIZEContext(self, localctx)
+                self.enterOuterAlt(localctx, 12)
+                self.state = 295
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==5 or _la==15 or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 481) != 0):
-                    self.state = 285
+                if _la==6 or _la==16 or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 481) != 0):
+                    self.state = 294
                     self.primaryExpression()
 
 
-                self.state = 292
+                self.state = 301
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==22:
-                    self.state = 288
-                    self.match(OCLsParser.DOT)
-                    self.state = 289
-                    self.match(OCLsParser.ID)
-                    self.state = 294
+                while _la==23:
+                    self.state = 297
+                    self.match(BOCLParser.DOT)
+                    self.state = 298
+                    self.match(BOCLParser.ID)
+                    self.state = 303
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 295
-                self.match(OCLsParser.Arrow)
-                self.state = 296
-                self.match(OCLsParser.SIZE)
-                self.state = 297
-                self.match(OCLsParser.LPAREN)
-                self.state = 298
-                self.match(OCLsParser.RPAREN)
-                self.state = 300
+                self.state = 304
+                self.match(BOCLParser.Arrow)
+                self.state = 305
+                self.match(BOCLParser.SIZE)
+                self.state = 306
+                self.match(BOCLParser.LPAREN)
+                self.state = 307
+                self.match(BOCLParser.RPAREN)
+                self.state = 309
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,49,self._ctx)
+                if la_ == 1:
+                    self.state = 308
+                    self.binaryFunctionCall()
+
+
+                self.state = 312
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,47,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,50,self._ctx)
                 if la_ == 1:
-                    self.state = 299
+                    self.state = 311
                     self.expression()
 
 
-                self.state = 305
+                self.state = 317
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 302
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 307
+                        self.state = 314
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 319
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,48,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
 
                 pass
 
-            elif la_ == 10:
-                localctx = OCLsParser.INCLUDESContext(self, localctx)
-                self.enterOuterAlt(localctx, 10)
-                self.state = 309
+            elif la_ == 13:
+                localctx = BOCLParser.INCLUDESContext(self, localctx)
+                self.enterOuterAlt(localctx, 13)
+                self.state = 321
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 308
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 320
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 311
-                self.match(OCLsParser.INCLUDES)
-                self.state = 312
-                self.match(OCLsParser.LPAREN)
-                self.state = 313
+                self.state = 323
+                self.match(BOCLParser.INCLUDES)
+                self.state = 324
+                self.match(BOCLParser.LPAREN)
+                self.state = 325
                 self.expression()
-                self.state = 314
-                self.match(OCLsParser.RPAREN)
-                self.state = 316
+                self.state = 326
+                self.match(BOCLParser.RPAREN)
+                self.state = 328
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,50,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,53,self._ctx)
                 if la_ == 1:
-                    self.state = 315
+                    self.state = 327
                     self.expression()
 
 
-                self.state = 321
+                self.state = 333
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,54,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 318
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 323
+                        self.state = 330
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 335
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,51,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,54,self._ctx)
 
                 pass
 
-            elif la_ == 11:
-                localctx = OCLsParser.EXCLUDESContext(self, localctx)
-                self.enterOuterAlt(localctx, 11)
-                self.state = 325
+            elif la_ == 14:
+                localctx = BOCLParser.EXCLUDESContext(self, localctx)
+                self.enterOuterAlt(localctx, 14)
+                self.state = 337
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 324
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 336
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 327
-                self.match(OCLsParser.EXCLUDES)
-                self.state = 328
-                self.match(OCLsParser.LPAREN)
-                self.state = 329
+                self.state = 339
+                self.match(BOCLParser.EXCLUDES)
+                self.state = 340
+                self.match(BOCLParser.LPAREN)
+                self.state = 341
                 self.expression()
-                self.state = 330
-                self.match(OCLsParser.RPAREN)
-                self.state = 332
+                self.state = 342
+                self.match(BOCLParser.RPAREN)
+                self.state = 344
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,53,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,56,self._ctx)
                 if la_ == 1:
-                    self.state = 331
+                    self.state = 343
                     self.expression()
 
 
-                self.state = 337
+                self.state = 349
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,54,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,57,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 334
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 339
+                        self.state = 346
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 351
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,54,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,57,self._ctx)
 
                 pass
 
-            elif la_ == 12:
-                localctx = OCLsParser.SEQUENCEContext(self, localctx)
-                self.enterOuterAlt(localctx, 12)
-                self.state = 341
+            elif la_ == 15:
+                localctx = BOCLParser.SEQUENCEContext(self, localctx)
+                self.enterOuterAlt(localctx, 15)
+                self.state = 353
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 340
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 352
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 346
+                self.state = 358
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 343
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 348
+                while _la==16:
+                    self.state = 355
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 360
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 349
-                self.match(OCLsParser.SEQUENCE)
-                self.state = 353
+                self.state = 361
+                self.match(BOCLParser.SEQUENCE)
+                self.state = 365
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==17:
-                    self.state = 350
-                    self.match(OCLsParser.LBRACE)
-                    self.state = 355
+                while _la==18:
+                    self.state = 362
+                    self.match(BOCLParser.LBRACE)
+                    self.state = 367
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 359
+                self.state = 371
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,58,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,61,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 356
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 361
+                        self.state = 368
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 373
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,58,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,61,self._ctx)
 
-                self.state = 374
+                self.state = 386
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,62,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,65,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 363
+                        self.state = 375
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,59,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,62,self._ctx)
                         if la_ == 1:
-                            self.state = 362
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 374
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 365
+                        self.state = 377
                         self.expression()
-                        self.state = 367
+                        self.state = 379
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,60,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,63,self._ctx)
                         if la_ == 1:
-                            self.state = 366
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 378
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 370
+                        self.state = 382
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,61,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,64,self._ctx)
                         if la_ == 1:
-                            self.state = 369
-                            self.match(OCLsParser.COMMA)
+                            self.state = 381
+                            self.match(BOCLParser.COMMA)
 
                  
-                    self.state = 376
+                    self.state = 388
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,62,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,65,self._ctx)
 
-                self.state = 380
+                self.state = 392
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,63,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,66,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 377
-                        self.match(OCLsParser.RBRACE) 
-                    self.state = 382
+                        self.state = 389
+                        self.match(BOCLParser.RBRACE) 
+                    self.state = 394
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,63,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,66,self._ctx)
 
-                self.state = 386
+                self.state = 398
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,64,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,67,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 383
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 388
+                        self.state = 395
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 400
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,64,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,67,self._ctx)
 
-                self.state = 390
+                self.state = 402
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,65,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,68,self._ctx)
                 if la_ == 1:
-                    self.state = 389
+                    self.state = 401
                     self.expression()
 
 
                 pass
 
-            elif la_ == 13:
-                localctx = OCLsParser.SUBSEQUENCEContext(self, localctx)
-                self.enterOuterAlt(localctx, 13)
-                self.state = 393
+            elif la_ == 16:
+                localctx = BOCLParser.SUBSEQUENCEContext(self, localctx)
+                self.enterOuterAlt(localctx, 16)
+                self.state = 405
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 392
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 404
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 398
+                self.state = 410
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 395
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 400
+                while _la==16:
+                    self.state = 407
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 412
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 401
-                self.match(OCLsParser.SUBSEQUENCE)
-                self.state = 405
+                self.state = 413
+                self.match(BOCLParser.SUBSEQUENCE)
+                self.state = 417
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==17:
-                    self.state = 402
-                    self.match(OCLsParser.LBRACE)
-                    self.state = 407
+                while _la==18:
+                    self.state = 414
+                    self.match(BOCLParser.LBRACE)
+                    self.state = 419
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 411
+                self.state = 423
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,69,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,72,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 408
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 413
+                        self.state = 420
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 425
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,69,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,72,self._ctx)
 
-                self.state = 426
+                self.state = 438
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,73,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,76,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 415
+                        self.state = 427
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,70,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,73,self._ctx)
                         if la_ == 1:
-                            self.state = 414
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 426
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 417
+                        self.state = 429
                         self.expression()
-                        self.state = 419
+                        self.state = 431
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,71,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,74,self._ctx)
                         if la_ == 1:
-                            self.state = 418
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 430
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 422
+                        self.state = 434
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,72,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,75,self._ctx)
                         if la_ == 1:
-                            self.state = 421
-                            self.match(OCLsParser.COMMA)
+                            self.state = 433
+                            self.match(BOCLParser.COMMA)
 
                  
-                    self.state = 428
+                    self.state = 440
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,73,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,76,self._ctx)
 
-                self.state = 432
+                self.state = 444
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,74,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,77,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 429
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 434
+                        self.state = 441
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 446
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,74,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,77,self._ctx)
 
-                self.state = 438
+                self.state = 450
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,75,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,78,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 435
-                        self.match(OCLsParser.RBRACE) 
-                    self.state = 440
+                        self.state = 447
+                        self.match(BOCLParser.RBRACE) 
+                    self.state = 452
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,75,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,78,self._ctx)
 
-                self.state = 442
+                self.state = 454
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,76,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,79,self._ctx)
                 if la_ == 1:
-                    self.state = 441
+                    self.state = 453
                     self.expression()
 
 
                 pass
 
-            elif la_ == 14:
-                localctx = OCLsParser.ALLINSTANCESContext(self, localctx)
-                self.enterOuterAlt(localctx, 14)
-                self.state = 445
+            elif la_ == 17:
+                localctx = BOCLParser.ALLINSTANCESContext(self, localctx)
+                self.enterOuterAlt(localctx, 17)
+                self.state = 457
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 444
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 456
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 447
-                self.match(OCLsParser.ALLINSTANCES)
-                self.state = 449 
+                self.state = 459
+                self.match(BOCLParser.ALLINSTANCES)
+                self.state = 461 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 448
-                        self.match(OCLsParser.LPAREN)
+                        self.state = 460
+                        self.match(BOCLParser.LPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 451 
+                    self.state = 463 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,78,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,81,self._ctx)
 
-                self.state = 453
-                self.expression()
-                self.state = 455 
+                self.state = 466
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 465
+                    self.expression()
+
+
+                self.state = 469 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 454
-                        self.match(OCLsParser.RPAREN)
+                        self.state = 468
+                        self.match(BOCLParser.RPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 457 
+                    self.state = 471 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,79,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,83,self._ctx)
 
-                self.state = 460
+                self.state = 474
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,80,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,84,self._ctx)
                 if la_ == 1:
-                    self.state = 459
+                    self.state = 473
                     self.expression()
 
 
                 pass
 
-            elif la_ == 15:
-                localctx = OCLsParser.ORDEREDSETContext(self, localctx)
-                self.enterOuterAlt(localctx, 15)
-                self.state = 463
+            elif la_ == 18:
+                localctx = BOCLParser.ORDEREDSETContext(self, localctx)
+                self.enterOuterAlt(localctx, 18)
+                self.state = 477
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 462
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 476
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 468
+                self.state = 482
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 465
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 470
+                while _la==16:
+                    self.state = 479
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 484
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 471
-                self.match(OCLsParser.ORDEREDSET)
-                self.state = 472
-                self.match(OCLsParser.LBRACE)
                 self.state = 485
+                self.match(BOCLParser.ORDEREDSET)
+                self.state = 486
+                self.match(BOCLParser.LBRACE)
+                self.state = 499
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                    self.state = 474
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 488
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,83,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,87,self._ctx)
                     if la_ == 1:
-                        self.state = 473
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 487
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 476
+                    self.state = 490
                     self.expression()
-                    self.state = 478
+                    self.state = 492
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,84,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,88,self._ctx)
                     if la_ == 1:
-                        self.state = 477
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 491
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 481
+                    self.state = 495
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 480
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 494
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 487
+                    self.state = 501
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 488
-                self.match(OCLsParser.RBRACE)
-                self.state = 492
+                self.state = 502
+                self.match(BOCLParser.RBRACE)
+                self.state = 506
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,87,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,91,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 489
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 494
+                        self.state = 503
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 508
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,87,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,91,self._ctx)
 
-                self.state = 496
+                self.state = 510
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,88,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,92,self._ctx)
                 if la_ == 1:
-                    self.state = 495
+                    self.state = 509
                     self.expression()
 
 
                 pass
 
-            elif la_ == 16:
-                localctx = OCLsParser.SUBORDEREDSETContext(self, localctx)
-                self.enterOuterAlt(localctx, 16)
-                self.state = 499
+            elif la_ == 19:
+                localctx = BOCLParser.SUBORDEREDSETContext(self, localctx)
+                self.enterOuterAlt(localctx, 19)
+                self.state = 513
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 498
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 512
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 504
+                self.state = 518
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 501
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 506
+                while _la==16:
+                    self.state = 515
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 520
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 507
-                self.match(OCLsParser.SUBORDEREDSET)
-                self.state = 511
+                self.state = 521
+                self.match(BOCLParser.SUBORDEREDSET)
+                self.state = 525
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==17:
-                    self.state = 508
-                    self.match(OCLsParser.LBRACE)
-                    self.state = 513
+                while _la==18:
+                    self.state = 522
+                    self.match(BOCLParser.LBRACE)
+                    self.state = 527
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 517
+                self.state = 531
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,92,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,96,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 514
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 519
+                        self.state = 528
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 533
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,92,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,96,self._ctx)
 
-                self.state = 532
+                self.state = 546
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,96,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,100,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 521
+                        self.state = 535
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,93,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,97,self._ctx)
                         if la_ == 1:
-                            self.state = 520
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 534
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 523
+                        self.state = 537
                         self.expression()
-                        self.state = 525
+                        self.state = 539
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,94,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,98,self._ctx)
                         if la_ == 1:
-                            self.state = 524
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 538
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 528
+                        self.state = 542
                         self._errHandler.sync(self)
                         _la = self._input.LA(1)
-                        if _la==21:
-                            self.state = 527
-                            self.match(OCLsParser.COMMA)
+                        if _la==22:
+                            self.state = 541
+                            self.match(BOCLParser.COMMA)
 
                  
-                    self.state = 534
+                    self.state = 548
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,96,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,100,self._ctx)
 
-                self.state = 538
+                self.state = 552
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==18:
-                    self.state = 535
-                    self.match(OCLsParser.RBRACE)
-                    self.state = 540
+                while _la==19:
+                    self.state = 549
+                    self.match(BOCLParser.RBRACE)
+                    self.state = 554
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 544
+                self.state = 558
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,98,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,102,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 541
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 546
+                        self.state = 555
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 560
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,98,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,102,self._ctx)
 
-                self.state = 548
+                self.state = 562
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                    self.state = 547
+                if (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 561
                     self.expression()
 
 
-                self.state = 550
-                self.match(OCLsParser.RPAREN)
+                self.state = 564
+                self.match(BOCLParser.RPAREN)
                 pass
 
-            elif la_ == 17:
-                localctx = OCLsParser.SETContext(self, localctx)
-                self.enterOuterAlt(localctx, 17)
-                self.state = 552
+            elif la_ == 20:
+                localctx = BOCLParser.SETContext(self, localctx)
+                self.enterOuterAlt(localctx, 20)
+                self.state = 566
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 551
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 565
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 557
+                self.state = 571
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 554
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 559
+                while _la==16:
+                    self.state = 568
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 573
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 560
-                self.match(OCLsParser.SET)
-                self.state = 564
+                self.state = 574
+                self.match(BOCLParser.SET)
+                self.state = 578
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,102,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,106,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 561
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 566
+                        self.state = 575
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 580
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,102,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,106,self._ctx)
 
-                self.state = 570
+                self.state = 584
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==17:
-                    self.state = 567
-                    self.match(OCLsParser.LBRACE)
-                    self.state = 572
+                while _la==18:
+                    self.state = 581
+                    self.match(BOCLParser.LBRACE)
+                    self.state = 586
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 585
+                self.state = 599
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,107,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,111,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 574
+                        self.state = 588
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,104,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,108,self._ctx)
                         if la_ == 1:
-                            self.state = 573
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 587
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 576
+                        self.state = 590
                         self.expression()
-                        self.state = 578
+                        self.state = 592
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,105,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,109,self._ctx)
                         if la_ == 1:
-                            self.state = 577
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 591
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 581
+                        self.state = 595
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,106,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,110,self._ctx)
                         if la_ == 1:
-                            self.state = 580
-                            self.match(OCLsParser.COMMA)
+                            self.state = 594
+                            self.match(BOCLParser.COMMA)
 
                  
-                    self.state = 587
+                    self.state = 601
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,107,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,111,self._ctx)
 
-                self.state = 591
+                self.state = 605
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,108,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,112,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 588
-                        self.match(OCLsParser.RBRACE) 
-                    self.state = 593
+                        self.state = 602
+                        self.match(BOCLParser.RBRACE) 
+                    self.state = 607
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,108,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,112,self._ctx)
 
-                self.state = 597
+                self.state = 611
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,109,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,113,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 594
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 599
+                        self.state = 608
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 613
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,109,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,113,self._ctx)
 
-                self.state = 601
+                self.state = 615
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,110,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,114,self._ctx)
                 if la_ == 1:
-                    self.state = 600
+                    self.state = 614
                     self.expression()
 
 
                 pass
 
-            elif la_ == 18:
-                localctx = OCLsParser.BAGContext(self, localctx)
-                self.enterOuterAlt(localctx, 18)
-                self.state = 604
+            elif la_ == 21:
+                localctx = BOCLParser.BAGContext(self, localctx)
+                self.enterOuterAlt(localctx, 21)
+                self.state = 618
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 603
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 617
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 609
+                self.state = 623
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==15:
-                    self.state = 606
-                    self.match(OCLsParser.LPAREN)
-                    self.state = 611
+                while _la==16:
+                    self.state = 620
+                    self.match(BOCLParser.LPAREN)
+                    self.state = 625
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 612
-                self.match(OCLsParser.BAG)
-                self.state = 616
+                self.state = 626
+                self.match(BOCLParser.BAG)
+                self.state = 630
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,113,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,117,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 613
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 618
+                        self.state = 627
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 632
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,113,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,117,self._ctx)
 
-                self.state = 622
+                self.state = 636
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==17:
-                    self.state = 619
-                    self.match(OCLsParser.LBRACE)
-                    self.state = 624
+                while _la==18:
+                    self.state = 633
+                    self.match(BOCLParser.LBRACE)
+                    self.state = 638
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 637
+                self.state = 651
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,118,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,122,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 626
+                        self.state = 640
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,115,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,119,self._ctx)
                         if la_ == 1:
-                            self.state = 625
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 639
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 628
+                        self.state = 642
                         self.expression()
-                        self.state = 630
+                        self.state = 644
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,116,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,120,self._ctx)
                         if la_ == 1:
-                            self.state = 629
-                            self.match(OCLsParser.SingleQuote)
+                            self.state = 643
+                            self.match(BOCLParser.SingleQuote)
 
 
-                        self.state = 633
+                        self.state = 647
                         self._errHandler.sync(self)
-                        la_ = self._interp.adaptivePredict(self._input,117,self._ctx)
+                        la_ = self._interp.adaptivePredict(self._input,121,self._ctx)
                         if la_ == 1:
-                            self.state = 632
-                            self.match(OCLsParser.COMMA)
+                            self.state = 646
+                            self.match(BOCLParser.COMMA)
 
                  
-                    self.state = 639
+                    self.state = 653
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,118,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,122,self._ctx)
 
-                self.state = 643
+                self.state = 657
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,119,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,123,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 640
-                        self.match(OCLsParser.RBRACE) 
-                    self.state = 645
+                        self.state = 654
+                        self.match(BOCLParser.RBRACE) 
+                    self.state = 659
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,119,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,123,self._ctx)
 
-                self.state = 649
+                self.state = 663
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,120,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,124,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 646
-                        self.match(OCLsParser.RPAREN) 
-                    self.state = 651
+                        self.state = 660
+                        self.match(BOCLParser.RPAREN) 
+                    self.state = 665
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,120,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,124,self._ctx)
 
-                self.state = 653
+                self.state = 667
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,121,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,125,self._ctx)
                 if la_ == 1:
-                    self.state = 652
+                    self.state = 666
                     self.expression()
 
 
                 pass
 
-            elif la_ == 19:
-                localctx = OCLsParser.PREPENDContext(self, localctx)
-                self.enterOuterAlt(localctx, 19)
-                self.state = 655
-                self.match(OCLsParser.Arrow)
-                self.state = 656
-                self.match(OCLsParser.PREPEND)
-                self.state = 658 
+            elif la_ == 22:
+                localctx = BOCLParser.PREPENDContext(self, localctx)
+                self.enterOuterAlt(localctx, 22)
+                self.state = 669
+                self.match(BOCLParser.Arrow)
+                self.state = 670
+                self.match(BOCLParser.PREPEND)
+                self.state = 672 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 657
-                        self.match(OCLsParser.LPAREN)
+                        self.state = 671
+                        self.match(BOCLParser.LPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 660 
+                    self.state = 674 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,122,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,126,self._ctx)
 
-                self.state = 674
+                self.state = 688
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                    self.state = 663
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 677
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,123,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,127,self._ctx)
                     if la_ == 1:
-                        self.state = 662
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 676
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 665
+                    self.state = 679
                     self.expression()
-                    self.state = 667
+                    self.state = 681
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,124,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,128,self._ctx)
                     if la_ == 1:
-                        self.state = 666
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 680
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 670
+                    self.state = 684
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 669
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 683
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 676
+                    self.state = 690
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 678 
+                self.state = 692 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 677
-                        self.match(OCLsParser.RPAREN)
+                        self.state = 691
+                        self.match(BOCLParser.RPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 680 
+                    self.state = 694 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,127,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,131,self._ctx)
 
-                self.state = 683
+                self.state = 697
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,128,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,132,self._ctx)
                 if la_ == 1:
-                    self.state = 682
+                    self.state = 696
                     self.expression()
 
 
                 pass
 
-            elif la_ == 20:
-                localctx = OCLsParser.LASTContext(self, localctx)
-                self.enterOuterAlt(localctx, 20)
-                self.state = 685
-                self.match(OCLsParser.Arrow)
-                self.state = 686
-                self.match(OCLsParser.LAST)
-                self.state = 687
-                self.match(OCLsParser.LPAREN)
-                self.state = 689 
+            elif la_ == 23:
+                localctx = BOCLParser.LASTContext(self, localctx)
+                self.enterOuterAlt(localctx, 23)
+                self.state = 699
+                self.match(BOCLParser.Arrow)
+                self.state = 700
+                self.match(BOCLParser.LAST)
+                self.state = 701
+                self.match(BOCLParser.LPAREN)
+                self.state = 703 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 688
-                        self.match(OCLsParser.RPAREN)
+                        self.state = 702
+                        self.match(BOCLParser.RPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 691 
+                    self.state = 705 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,129,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,133,self._ctx)
 
-                self.state = 694
+                self.state = 708
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,130,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,134,self._ctx)
                 if la_ == 1:
-                    self.state = 693
+                    self.state = 707
                     self.expression()
 
 
                 pass
 
-            elif la_ == 21:
-                localctx = OCLsParser.APPENDContext(self, localctx)
-                self.enterOuterAlt(localctx, 21)
-                self.state = 696
-                self.match(OCLsParser.Arrow)
-                self.state = 697
-                self.match(OCLsParser.APPEND)
-                self.state = 698
-                self.match(OCLsParser.LPAREN)
+            elif la_ == 24:
+                localctx = BOCLParser.APPENDContext(self, localctx)
+                self.enterOuterAlt(localctx, 24)
+                self.state = 710
+                self.match(BOCLParser.Arrow)
                 self.state = 711
+                self.match(BOCLParser.APPEND)
+                self.state = 712
+                self.match(BOCLParser.LPAREN)
+                self.state = 725
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while (((_la) & ~0x3f) == 0 and ((1 << _la) & 8687441474150769632) != 0) or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 505) != 0):
-                    self.state = 700
+                while (((_la) & ~0x3f) == 0 and ((1 << _la) & -1071861110375594046) != 0) or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 505) != 0):
+                    self.state = 714
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,131,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,135,self._ctx)
                     if la_ == 1:
-                        self.state = 699
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 713
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 702
+                    self.state = 716
                     self.expression()
-                    self.state = 704
+                    self.state = 718
                     self._errHandler.sync(self)
-                    la_ = self._interp.adaptivePredict(self._input,132,self._ctx)
+                    la_ = self._interp.adaptivePredict(self._input,136,self._ctx)
                     if la_ == 1:
-                        self.state = 703
-                        self.match(OCLsParser.SingleQuote)
+                        self.state = 717
+                        self.match(BOCLParser.SingleQuote)
 
 
-                    self.state = 707
+                    self.state = 721
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 706
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 720
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 713
+                    self.state = 727
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 715 
+                self.state = 729 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 714
-                        self.match(OCLsParser.RPAREN)
+                        self.state = 728
+                        self.match(BOCLParser.RPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 717 
+                    self.state = 731 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,135,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,139,self._ctx)
 
-                self.state = 720
+                self.state = 734
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,136,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,140,self._ctx)
                 if la_ == 1:
-                    self.state = 719
+                    self.state = 733
                     self.expression()
 
 
                 pass
 
-            elif la_ == 22:
-                localctx = OCLsParser.COLLECTIONContext(self, localctx)
-                self.enterOuterAlt(localctx, 22)
-                self.state = 723
+            elif la_ == 25:
+                localctx = BOCLParser.COLLECTIONContext(self, localctx)
+                self.enterOuterAlt(localctx, 25)
+                self.state = 737
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 722
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 736
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 725
+                self.state = 739
                 _la = self._input.LA(1)
-                if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 960) != 0)):
+                if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1920) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 726
-                self.match(OCLsParser.LPAREN)
-                self.state = 735 
+                self.state = 740
+                self.match(BOCLParser.LPAREN)
+                self.state = 749 
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while True:
-                    self.state = 727
-                    self.match(OCLsParser.ID)
-                    self.state = 730
+                    self.state = 741
+                    self.match(BOCLParser.ID)
+                    self.state = 744
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==20:
-                        self.state = 728
-                        self.match(OCLsParser.COLON)
-                        self.state = 729
-                        self.match(OCLsParser.ID)
+                    if _la==21:
+                        self.state = 742
+                        self.match(BOCLParser.COLON)
+                        self.state = 743
+                        self.match(BOCLParser.ID)
 
 
-                    self.state = 733
+                    self.state = 747
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if _la==21:
-                        self.state = 732
-                        self.match(OCLsParser.COMMA)
+                    if _la==22:
+                        self.state = 746
+                        self.match(BOCLParser.COMMA)
 
 
-                    self.state = 737 
+                    self.state = 751 
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
-                    if not (_la==77):
+                    if not (_la==78):
                         break
 
-                self.state = 739
-                self.match(OCLsParser.PIPE)
-                self.state = 740
+                self.state = 753
+                self.match(BOCLParser.PIPE)
+                self.state = 754
                 self.expression()
-                self.state = 741
-                self.match(OCLsParser.RPAREN)
-                self.state = 743
+                self.state = 755
+                self.match(BOCLParser.RPAREN)
+                self.state = 757
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,141,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,145,self._ctx)
                 if la_ == 1:
-                    self.state = 742
-                    self.expression()
+                    self.state = 756
+                    self.endExpression()
 
 
                 pass
 
-            elif la_ == 23:
-                localctx = OCLsParser.CollectionExpressionVariableContext(self, localctx)
-                self.enterOuterAlt(localctx, 23)
-                self.state = 746
+            elif la_ == 26:
+                localctx = BOCLParser.CollectionExpressionVariableContext(self, localctx)
+                self.enterOuterAlt(localctx, 26)
+                self.state = 760
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 745
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 759
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 748
+                self.state = 762
                 _la = self._input.LA(1)
-                if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 960) != 0)):
+                if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 1920) != 0)):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 749
-                self.match(OCLsParser.LPAREN)
-                self.state = 750
+                self.state = 763
+                self.match(BOCLParser.LPAREN)
+                self.state = 764
                 self.expression()
-                self.state = 751
-                self.match(OCLsParser.RPAREN)
-                self.state = 753
+                self.state = 765
+                self.match(BOCLParser.RPAREN)
+                self.state = 767
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,143,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,147,self._ctx)
                 if la_ == 1:
-                    self.state = 752
-                    self.expression()
+                    self.state = 766
+                    self.endExpression()
 
 
                 pass
 
-            elif la_ == 24:
-                localctx = OCLsParser.SYMMETRICDIFFERENCEContext(self, localctx)
-                self.enterOuterAlt(localctx, 24)
-                self.state = 755
-                self.match(OCLsParser.Arrow)
-                self.state = 756
-                self.match(OCLsParser.SYMMETRICDIFFERENCE)
-                self.state = 757
-                self.match(OCLsParser.LPAREN)
-                self.state = 758
+            elif la_ == 27:
+                localctx = BOCLParser.SYMMETRICDIFFERENCEContext(self, localctx)
+                self.enterOuterAlt(localctx, 27)
+                self.state = 769
+                self.match(BOCLParser.Arrow)
+                self.state = 770
+                self.match(BOCLParser.SYMMETRICDIFFERENCE)
+                self.state = 771
+                self.match(BOCLParser.LPAREN)
+                self.state = 772
                 self.expression()
-                self.state = 760 
+                self.state = 774 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 759
-                        self.match(OCLsParser.RPAREN)
+                        self.state = 773
+                        self.match(BOCLParser.RPAREN)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 762 
+                    self.state = 776 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,144,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,148,self._ctx)
 
-                self.state = 765
+                self.state = 779
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,145,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,149,self._ctx)
                 if la_ == 1:
-                    self.state = 764
+                    self.state = 778
                     self.expression()
 
 
                 pass
 
-            elif la_ == 25:
-                localctx = OCLsParser.FIRSTContext(self, localctx)
-                self.enterOuterAlt(localctx, 25)
-                self.state = 767
-                self.match(OCLsParser.Arrow)
-                self.state = 768
-                self.match(OCLsParser.FIRST)
-                self.state = 769
-                self.match(OCLsParser.LPAREN)
-                self.state = 770
-                self.match(OCLsParser.RPAREN)
-                self.state = 772
+            elif la_ == 28:
+                localctx = BOCLParser.FIRSTContext(self, localctx)
+                self.enterOuterAlt(localctx, 28)
+                self.state = 781
+                self.match(BOCLParser.Arrow)
+                self.state = 782
+                self.match(BOCLParser.FIRST)
+                self.state = 783
+                self.match(BOCLParser.LPAREN)
+                self.state = 784
+                self.match(BOCLParser.RPAREN)
+                self.state = 786
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,146,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,150,self._ctx)
                 if la_ == 1:
-                    self.state = 771
+                    self.state = 785
                     self.expression()
 
 
                 pass
 
-            elif la_ == 26:
-                localctx = OCLsParser.DERIVEContext(self, localctx)
-                self.enterOuterAlt(localctx, 26)
-                self.state = 774
-                self.match(OCLsParser.Arrow)
-                self.state = 775
-                self.match(OCLsParser.DERIVE)
-                self.state = 776
-                self.match(OCLsParser.LPAREN)
-                self.state = 777
-                self.match(OCLsParser.RPAREN)
-                self.state = 779
+            elif la_ == 29:
+                localctx = BOCLParser.DERIVEContext(self, localctx)
+                self.enterOuterAlt(localctx, 29)
+                self.state = 788
+                self.match(BOCLParser.Arrow)
+                self.state = 789
+                self.match(BOCLParser.DERIVE)
+                self.state = 790
+                self.match(BOCLParser.LPAREN)
+                self.state = 791
+                self.match(BOCLParser.RPAREN)
+                self.state = 793
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,147,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,151,self._ctx)
                 if la_ == 1:
-                    self.state = 778
+                    self.state = 792
                     self.expression()
 
 
                 pass
 
-            elif la_ == 27:
-                localctx = OCLsParser.UNIONContext(self, localctx)
-                self.enterOuterAlt(localctx, 27)
-                self.state = 781
-                self.match(OCLsParser.Arrow)
-                self.state = 782
-                self.match(OCLsParser.UNION)
-                self.state = 783
-                self.match(OCLsParser.LPAREN)
-                self.state = 784
+            elif la_ == 30:
+                localctx = BOCLParser.UNIONContext(self, localctx)
+                self.enterOuterAlt(localctx, 30)
+                self.state = 795
+                self.match(BOCLParser.Arrow)
+                self.state = 796
+                self.match(BOCLParser.UNION)
+                self.state = 797
+                self.match(BOCLParser.LPAREN)
+                self.state = 798
                 self.expression()
-                self.state = 785
-                self.match(OCLsParser.RPAREN)
-                self.state = 787
+                self.state = 799
+                self.match(BOCLParser.RPAREN)
+                self.state = 801
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,148,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,152,self._ctx)
                 if la_ == 1:
-                    self.state = 786
+                    self.state = 800
                     self.expression()
 
 
                 pass
 
-            elif la_ == 28:
-                localctx = OCLsParser.DefExpContext(self, localctx)
-                self.enterOuterAlt(localctx, 28)
-                self.state = 789
-                self.match(OCLsParser.Def)
-                self.state = 790
-                self.match(OCLsParser.COLON)
-                self.state = 791
+            elif la_ == 31:
+                localctx = BOCLParser.DefExpContext(self, localctx)
+                self.enterOuterAlt(localctx, 31)
+                self.state = 803
+                self.match(BOCLParser.Def)
+                self.state = 804
+                self.match(BOCLParser.COLON)
+                self.state = 805
                 self.expression()
                 pass
 
-            elif la_ == 29:
-                localctx = OCLsParser.DefIDAssignmentexpressionContext(self, localctx)
-                self.enterOuterAlt(localctx, 29)
-                self.state = 792
-                self.match(OCLsParser.ID)
-                self.state = 793
-                self.match(OCLsParser.COLON)
-                self.state = 794
-                self.match(OCLsParser.ID)
-                self.state = 795
-                self.match(OCLsParser.EQUAL)
-                self.state = 796
+            elif la_ == 32:
+                localctx = BOCLParser.DefIDAssignmentexpressionContext(self, localctx)
+                self.enterOuterAlt(localctx, 32)
+                self.state = 806
+                self.match(BOCLParser.ID)
+                self.state = 807
+                self.match(BOCLParser.COLON)
+                self.state = 808
+                self.match(BOCLParser.ID)
+                self.state = 809
+                self.match(BOCLParser.EQUAL)
+                self.state = 810
                 self.expression()
                 pass
 
-            elif la_ == 30:
-                localctx = OCLsParser.PrimaryExpContext(self, localctx)
-                self.enterOuterAlt(localctx, 30)
-                self.state = 800
+            elif la_ == 33:
+                localctx = BOCLParser.PrimaryExpContext(self, localctx)
+                self.enterOuterAlt(localctx, 33)
+                self.state = 814
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,149,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,153,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 797
-                        self.match(OCLsParser.LPAREN) 
-                    self.state = 802
+                        self.state = 811
+                        self.match(BOCLParser.LPAREN) 
+                    self.state = 816
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,149,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,153,self._ctx)
 
-                self.state = 804
+                self.state = 818
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,150,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,154,self._ctx)
                 if la_ == 1:
-                    self.state = 803
+                    self.state = 817
                     self.primaryExpression()
 
 
-                self.state = 810
+                self.state = 824
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,151,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,155,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 806
-                        self.match(OCLsParser.DOT)
-                        self.state = 807
-                        self.match(OCLsParser.ID) 
-                    self.state = 812
+                        self.state = 820
+                        self.match(BOCLParser.DOT)
+                        self.state = 821
+                        self.match(BOCLParser.ID) 
+                    self.state = 826
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,151,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,155,self._ctx)
 
-                self.state = 814
+                self.state = 828
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if (((_la) & ~0x3f) == 0 and ((1 << _la) & 4435386965164032) != 0):
-                    self.state = 813
+                if (((_la) & ~0x3f) == 0 and ((1 << _la) & 8870773930328066) != 0):
+                    self.state = 827
                     self.operator()
 
 
-                self.state = 817
+                self.state = 831
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==5 or _la==15 or ((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 481) != 0):
-                    self.state = 816
+                if _la==6 or _la==16 or ((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 481) != 0):
+                    self.state = 830
                     self.primaryExpression()
 
 
-                self.state = 821 
+                self.state = 835 
                 self._errHandler.sync(self)
                 _alt = 1
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 819
-                        self.match(OCLsParser.DOT)
-                        self.state = 820
-                        self.match(OCLsParser.ID)
+                        self.state = 833
+                        self.match(BOCLParser.DOT)
+                        self.state = 834
+                        self.match(BOCLParser.ID)
 
                     else:
                         raise NoViableAltException(self)
-                    self.state = 823 
+                    self.state = 837 
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,154,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,158,self._ctx)
 
-                self.state = 826
+                self.state = 840
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,155,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,159,self._ctx)
                 if la_ == 1:
-                    self.state = 825
+                    self.state = 839
                     self.expression()
 
 
                 pass
 
-            elif la_ == 31:
-                localctx = OCLsParser.FuncCallContext(self, localctx)
-                self.enterOuterAlt(localctx, 31)
-                self.state = 828
+            elif la_ == 34:
+                localctx = BOCLParser.FuncCallContext(self, localctx)
+                self.enterOuterAlt(localctx, 34)
+                self.state = 842
                 self.primaryExpression()
-                self.state = 832
+                self.state = 846
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                while _la==22:
-                    self.state = 829
-                    self.match(OCLsParser.DOT)
-                    self.state = 834
+                while _la==23:
+                    self.state = 843
+                    self.match(BOCLParser.DOT)
+                    self.state = 848
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 838
+                self.state = 852
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,157,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,161,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 835
-                        self.match(OCLsParser.ID) 
-                    self.state = 840
+                        self.state = 849
+                        self.match(BOCLParser.ID) 
+                    self.state = 854
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,157,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,161,self._ctx)
 
-                self.state = 841
+                self.state = 855
                 self.functionCall()
-                self.state = 843
+                self.state = 857
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,158,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,162,self._ctx)
                 if la_ == 1:
-                    self.state = 842
+                    self.state = 856
                     self.operator()
 
 
-                self.state = 846
+                self.state = 860
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,159,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,163,self._ctx)
                 if la_ == 1:
-                    self.state = 845
+                    self.state = 859
                     self.expression()
 
 
                 pass
 
-            elif la_ == 32:
-                localctx = OCLsParser.OpContext(self, localctx)
-                self.enterOuterAlt(localctx, 32)
-                self.state = 848
-                self.operator()
-                self.state = 850
-                self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,160,self._ctx)
-                if la_ == 1:
-                    self.state = 849
-                    self.numberORUserDefined()
-
-
-                pass
-
-            elif la_ == 33:
-                localctx = OCLsParser.ArrowexpContext(self, localctx)
-                self.enterOuterAlt(localctx, 33)
-                self.state = 852
-                self.match(OCLsParser.Arrow)
-                self.state = 853
+            elif la_ == 35:
+                localctx = BOCLParser.ArrowexpContext(self, localctx)
+                self.enterOuterAlt(localctx, 35)
+                self.state = 862
+                self.match(BOCLParser.Arrow)
+                self.state = 863
                 self.expression()
                 pass
 
-            elif la_ == 34:
-                localctx = OCLsParser.NumberContext(self, localctx)
-                self.enterOuterAlt(localctx, 34)
-                self.state = 854
-                self.match(OCLsParser.NUMBER)
-                self.state = 856
+            elif la_ == 36:
+                localctx = BOCLParser.NumberContext(self, localctx)
+                self.enterOuterAlt(localctx, 36)
+                self.state = 864
+                self.match(BOCLParser.NUMBER)
+                self.state = 866
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,161,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,164,self._ctx)
                 if la_ == 1:
-                    self.state = 855
+                    self.state = 865
                     self.expression()
 
 
                 pass
 
-            elif la_ == 35:
-                localctx = OCLsParser.PredefinedfunctionCallContext(self, localctx)
-                self.enterOuterAlt(localctx, 35)
-                self.state = 859
+            elif la_ == 37:
+                localctx = BOCLParser.PredefinedfunctionCallContext(self, localctx)
+                self.enterOuterAlt(localctx, 37)
+                self.state = 869
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==75:
-                    self.state = 858
-                    self.match(OCLsParser.Arrow)
+                if _la==76:
+                    self.state = 868
+                    self.match(BOCLParser.Arrow)
 
 
-                self.state = 861
+                self.state = 871
                 self.functionCall()
-                self.state = 863
+                self.state = 873
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,163,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,166,self._ctx)
                 if la_ == 1:
-                    self.state = 862
+                    self.state = 872
                     self.expression()
 
 
                 pass
 
-            elif la_ == 36:
-                localctx = OCLsParser.IDContext(self, localctx)
-                self.enterOuterAlt(localctx, 36)
-                self.state = 865
-                self.primaryExpression()
-                self.state = 867
+            elif la_ == 38:
+                localctx = BOCLParser.SingleQuoteExpContext(self, localctx)
+                self.enterOuterAlt(localctx, 38)
+                self.state = 875
+                self.match(BOCLParser.SingleQuote)
+                self.state = 876
+                self.expression()
+                self.state = 878
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,164,self._ctx)
+                _la = self._input.LA(1)
+                if _la==23:
+                    self.state = 877
+                    self.match(BOCLParser.DOT)
+
+
+                self.state = 880
+                self.match(BOCLParser.SingleQuote)
+                self.state = 882
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,168,self._ctx)
+                if la_ == 1:
+                    self.state = 881
+                    self.match(BOCLParser.DOT)
+
+
+                self.state = 885
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,169,self._ctx)
                 if la_ == 1:
-                    self.state = 866
+                    self.state = 884
                     self.expression()
 
 
                 pass
 
-            elif la_ == 37:
-                localctx = OCLsParser.SingleQuoteExpContext(self, localctx)
-                self.enterOuterAlt(localctx, 37)
-                self.state = 869
-                self.match(OCLsParser.SingleQuote)
-                self.state = 870
+            elif la_ == 39:
+                localctx = BOCLParser.DoubleDotsContext(self, localctx)
+                self.enterOuterAlt(localctx, 39)
+                self.state = 887
+                self.match(BOCLParser.DoubleDots)
+                self.state = 888
                 self.expression()
-                self.state = 872
+                pass
+
+            elif la_ == 40:
+                localctx = BOCLParser.DoubleCOLONsContext(self, localctx)
+                self.enterOuterAlt(localctx, 40)
+                self.state = 890
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==22:
-                    self.state = 871
-                    self.match(OCLsParser.DOT)
+                if _la==34:
+                    self.state = 889
+                    self.match(BOCLParser.AND)
 
 
-                self.state = 874
-                self.match(OCLsParser.SingleQuote)
-                self.state = 876
+                self.state = 893
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,166,self._ctx)
+                _la = self._input.LA(1)
+                if _la==35:
+                    self.state = 892
+                    self.match(BOCLParser.OR)
+
+
+                self.state = 896
+                self._errHandler.sync(self)
+                _la = self._input.LA(1)
+                if _la==78:
+                    self.state = 895
+                    self.match(BOCLParser.ID)
+
+
+                self.state = 898
+                self.match(BOCLParser.DoubleCOLON)
+                self.state = 899
+                self.expression()
+                pass
+
+            elif la_ == 41:
+                localctx = BOCLParser.OpContext(self, localctx)
+                self.enterOuterAlt(localctx, 41)
+                self.state = 900
+                self.operator()
+                self.state = 902
+                self._errHandler.sync(self)
+                la_ = self._interp.adaptivePredict(self._input,173,self._ctx)
                 if la_ == 1:
-                    self.state = 875
-                    self.match(OCLsParser.DOT)
+                    self.state = 901
+                    self.numberORUserDefined()
+
 
+                pass
 
-                self.state = 879
+            elif la_ == 42:
+                localctx = BOCLParser.IDContext(self, localctx)
+                self.enterOuterAlt(localctx, 42)
+                self.state = 904
+                self.primaryExpression()
+                self.state = 906
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,167,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,174,self._ctx)
                 if la_ == 1:
-                    self.state = 878
+                    self.state = 905
                     self.expression()
 
 
                 pass
 
-            elif la_ == 38:
-                localctx = OCLsParser.DoubleDotsContext(self, localctx)
-                self.enterOuterAlt(localctx, 38)
-                self.state = 881
-                self.match(OCLsParser.DoubleDots)
-                self.state = 882
-                self.expression()
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class EndExpressionContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def expression(self):
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
+
+
+        def AND(self):
+            return self.getToken(BOCLParser.AND, 0)
+
+        def OR(self):
+            return self.getToken(BOCLParser.OR, 0)
+
+        def getRuleIndex(self):
+            return BOCLParser.RULE_endExpression
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterEndExpression" ):
+                listener.enterEndExpression(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitEndExpression" ):
+                listener.exitEndExpression(self)
+
+
+
+
+    def endExpression(self):
+
+        localctx = BOCLParser.EndExpressionContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 16, self.RULE_endExpression)
+        self._la = 0 # Token type
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 911
+            self._errHandler.sync(self)
+            la_ = self._interp.adaptivePredict(self._input,176,self._ctx)
+            if la_ == 1:
+                self.state = 910
+                _la = self._input.LA(1)
+                if not(_la==34 or _la==35):
+                    self._errHandler.recoverInline(self)
+                else:
+                    self._errHandler.reportMatch(self)
+                    self.consume()
+
+
+            self.state = 913
+            self.expression()
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+
+    class BinaryFunctionCallContext(ParserRuleContext):
+        __slots__ = 'parser'
+
+        def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def operator(self):
+            return self.getTypedRuleContext(BOCLParser.OperatorContext,0)
+
+
+        def NUMBER(self):
+            return self.getToken(BOCLParser.NUMBER, 0)
+
+        def primaryExpression(self):
+            return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,0)
+
+
+        def DOT(self, i:int=None):
+            if i is None:
+                return self.getTokens(BOCLParser.DOT)
+            else:
+                return self.getToken(BOCLParser.DOT, i)
+
+        def ID(self, i:int=None):
+            if i is None:
+                return self.getTokens(BOCLParser.ID)
+            else:
+                return self.getToken(BOCLParser.ID, i)
+
+        def getRuleIndex(self):
+            return BOCLParser.RULE_binaryFunctionCall
+
+        def enterRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "enterBinaryFunctionCall" ):
+                listener.enterBinaryFunctionCall(self)
+
+        def exitRule(self, listener:ParseTreeListener):
+            if hasattr( listener, "exitBinaryFunctionCall" ):
+                listener.exitBinaryFunctionCall(self)
+
+
+
+
+    def binaryFunctionCall(self):
+
+        localctx = BOCLParser.BinaryFunctionCallContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 18, self.RULE_binaryFunctionCall)
+        try:
+            self.enterOuterAlt(localctx, 1)
+            self.state = 915
+            self.operator()
+            self.state = 925
+            self._errHandler.sync(self)
+            la_ = self._interp.adaptivePredict(self._input,178,self._ctx)
+            if la_ == 1:
+                self.state = 916
+                self.primaryExpression()
+                self.state = 921
+                self._errHandler.sync(self)
+                _alt = self._interp.adaptivePredict(self._input,177,self._ctx)
+                while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
+                    if _alt==1:
+                        self.state = 917
+                        self.match(BOCLParser.DOT)
+                        self.state = 918
+                        self.match(BOCLParser.ID) 
+                    self.state = 923
+                    self._errHandler.sync(self)
+                    _alt = self._interp.adaptivePredict(self._input,177,self._ctx)
+
+                pass
+
+            elif la_ == 2:
+                self.state = 924
+                self.match(BOCLParser.NUMBER)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4552,128 +4890,128 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def operator(self):
-            return self.getTypedRuleContext(OCLsParser.OperatorContext,0)
+            return self.getTypedRuleContext(BOCLParser.OperatorContext,0)
 
 
         def NUMBER(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.NUMBER)
+                return self.getTokens(BOCLParser.NUMBER)
             else:
-                return self.getToken(OCLsParser.NUMBER, i)
+                return self.getToken(BOCLParser.NUMBER, i)
 
         def DOT(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.DOT)
+                return self.getTokens(BOCLParser.DOT)
             else:
-                return self.getToken(OCLsParser.DOT, i)
+                return self.getToken(BOCLParser.DOT, i)
 
         def ID(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.ID)
+                return self.getTokens(BOCLParser.ID)
             else:
-                return self.getToken(OCLsParser.ID, i)
+                return self.getToken(BOCLParser.ID, i)
 
         def primaryExpression(self, i:int=None):
             if i is None:
-                return self.getTypedRuleContexts(OCLsParser.PrimaryExpressionContext)
+                return self.getTypedRuleContexts(BOCLParser.PrimaryExpressionContext)
             else:
-                return self.getTypedRuleContext(OCLsParser.PrimaryExpressionContext,i)
+                return self.getTypedRuleContext(BOCLParser.PrimaryExpressionContext,i)
 
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_binaryExpression
+            return BOCLParser.RULE_binaryExpression
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterBinaryExpression" ):
                 listener.enterBinaryExpression(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitBinaryExpression" ):
                 listener.exitBinaryExpression(self)
 
 
 
 
     def binaryExpression(self):
 
-        localctx = OCLsParser.BinaryExpressionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 16, self.RULE_binaryExpression)
+        localctx = BOCLParser.BinaryExpressionContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 20, self.RULE_binaryExpression)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 894
+            self.state = 936
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,170,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,180,self._ctx)
             if la_ == 1:
-                self.state = 885
+                self.state = 927
                 self.primaryExpression()
-                self.state = 890
+                self.state = 932
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,169,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,179,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 886
-                        self.match(OCLsParser.DOT)
-                        self.state = 887
-                        self.match(OCLsParser.ID) 
-                    self.state = 892
+                        self.state = 928
+                        self.match(BOCLParser.DOT)
+                        self.state = 929
+                        self.match(BOCLParser.ID) 
+                    self.state = 934
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,169,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,179,self._ctx)
 
                 pass
 
             elif la_ == 2:
-                self.state = 893
-                self.match(OCLsParser.NUMBER)
+                self.state = 935
+                self.match(BOCLParser.NUMBER)
                 pass
 
 
-            self.state = 900
+            self.state = 942
             self._errHandler.sync(self)
             _la = self._input.LA(1)
-            while _la==22:
-                self.state = 896
-                self.match(OCLsParser.DOT)
-                self.state = 897
-                self.match(OCLsParser.ID)
-                self.state = 902
+            while _la==23:
+                self.state = 938
+                self.match(BOCLParser.DOT)
+                self.state = 939
+                self.match(BOCLParser.ID)
+                self.state = 944
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 903
+            self.state = 945
             self.operator()
-            self.state = 913
+            self.state = 955
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,173,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,183,self._ctx)
             if la_ == 1:
-                self.state = 904
+                self.state = 946
                 self.primaryExpression()
-                self.state = 909
+                self.state = 951
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input,172,self._ctx)
+                _alt = self._interp.adaptivePredict(self._input,182,self._ctx)
                 while _alt!=2 and _alt!=ATN.INVALID_ALT_NUMBER:
                     if _alt==1:
-                        self.state = 905
-                        self.match(OCLsParser.DOT)
-                        self.state = 906
-                        self.match(OCLsParser.ID) 
-                    self.state = 911
+                        self.state = 947
+                        self.match(BOCLParser.DOT)
+                        self.state = 948
+                        self.match(BOCLParser.ID) 
+                    self.state = 953
                     self._errHandler.sync(self)
-                    _alt = self._interp.adaptivePredict(self._input,172,self._ctx)
+                    _alt = self._interp.adaptivePredict(self._input,182,self._ctx)
 
                 pass
 
             elif la_ == 2:
-                self.state = 912
-                self.match(OCLsParser.NUMBER)
+                self.state = 954
+                self.match(BOCLParser.NUMBER)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4686,52 +5024,58 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def NOT(self):
-            return self.getToken(OCLsParser.NOT, 0)
+            return self.getToken(BOCLParser.NOT, 0)
 
         def MINUS(self):
-            return self.getToken(OCLsParser.MINUS, 0)
+            return self.getToken(BOCLParser.MINUS, 0)
+
+        def PLUS(self):
+            return self.getToken(BOCLParser.PLUS, 0)
+
+        def Divide(self):
+            return self.getToken(BOCLParser.Divide, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_unaryExpression
+            return BOCLParser.RULE_unaryExpression
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterUnaryExpression" ):
                 listener.enterUnaryExpression(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitUnaryExpression" ):
                 listener.exitUnaryExpression(self)
 
 
 
 
     def unaryExpression(self):
 
-        localctx = OCLsParser.UnaryExpressionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 18, self.RULE_unaryExpression)
+        localctx = BOCLParser.UnaryExpressionContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 22, self.RULE_unaryExpression)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 915
+            self.state = 957
             _la = self._input.LA(1)
-            if not(_la==35 or _la==46):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 985231137964034) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
-            self.state = 916
+            self.state = 958
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4742,79 +5086,79 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def EQUAL(self):
-            return self.getToken(OCLsParser.EQUAL, 0)
+            return self.getToken(BOCLParser.EQUAL, 0)
 
         def NOTEQUAL(self):
-            return self.getToken(OCLsParser.NOTEQUAL, 0)
+            return self.getToken(BOCLParser.NOTEQUAL, 0)
 
         def LT(self):
-            return self.getToken(OCLsParser.LT, 0)
+            return self.getToken(BOCLParser.LT, 0)
 
         def LE(self):
-            return self.getToken(OCLsParser.LE, 0)
+            return self.getToken(BOCLParser.LE, 0)
 
         def GT(self):
-            return self.getToken(OCLsParser.GT, 0)
+            return self.getToken(BOCLParser.GT, 0)
 
         def GE(self):
-            return self.getToken(OCLsParser.GE, 0)
+            return self.getToken(BOCLParser.GE, 0)
 
         def PLUS(self):
-            return self.getToken(OCLsParser.PLUS, 0)
+            return self.getToken(BOCLParser.PLUS, 0)
 
         def MINUS(self):
-            return self.getToken(OCLsParser.MINUS, 0)
+            return self.getToken(BOCLParser.MINUS, 0)
 
         def EMPTYSTRING(self):
-            return self.getToken(OCLsParser.EMPTYSTRING, 0)
+            return self.getToken(BOCLParser.EMPTYSTRING, 0)
 
         def Divide(self):
-            return self.getToken(OCLsParser.Divide, 0)
+            return self.getToken(BOCLParser.Divide, 0)
 
         def AND(self):
-            return self.getToken(OCLsParser.AND, 0)
+            return self.getToken(BOCLParser.AND, 0)
 
         def OR(self):
-            return self.getToken(OCLsParser.OR, 0)
+            return self.getToken(BOCLParser.OR, 0)
 
         def XOR(self):
-            return self.getToken(OCLsParser.XOR, 0)
+            return self.getToken(BOCLParser.XOR, 0)
 
         def IMPLIES(self):
-            return self.getToken(OCLsParser.IMPLIES, 0)
+            return self.getToken(BOCLParser.IMPLIES, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_operator
+            return BOCLParser.RULE_operator
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterOperator" ):
                 listener.enterOperator(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitOperator" ):
                 listener.exitOperator(self)
 
 
 
 
     def operator(self):
 
-        localctx = OCLsParser.OperatorContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 20, self.RULE_operator)
+        localctx = BOCLParser.OperatorContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 24, self.RULE_operator)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 918
+            self.state = 960
             _la = self._input.LA(1)
-            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 4435386965164032) != 0)):
+            if not((((_la) & ~0x3f) == 0 and ((1 << _la) & 8870773930328066) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
@@ -4828,93 +5172,93 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def NUMBER(self):
-            return self.getToken(OCLsParser.NUMBER, 0)
+            return self.getToken(BOCLParser.NUMBER, 0)
 
         def ID(self):
-            return self.getToken(OCLsParser.ID, 0)
+            return self.getToken(BOCLParser.ID, 0)
 
         def SingleQuote(self, i:int=None):
             if i is None:
-                return self.getTokens(OCLsParser.SingleQuote)
+                return self.getTokens(BOCLParser.SingleQuote)
             else:
-                return self.getToken(OCLsParser.SingleQuote, i)
+                return self.getToken(BOCLParser.SingleQuote, i)
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_numberORUserDefined
+            return BOCLParser.RULE_numberORUserDefined
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterNumberORUserDefined" ):
                 listener.enterNumberORUserDefined(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitNumberORUserDefined" ):
                 listener.exitNumberORUserDefined(self)
 
 
 
 
     def numberORUserDefined(self):
 
-        localctx = OCLsParser.NumberORUserDefinedContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 22, self.RULE_numberORUserDefined)
+        localctx = BOCLParser.NumberORUserDefinedContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 26, self.RULE_numberORUserDefined)
         self._la = 0 # Token type
         try:
-            self.state = 934
+            self.state = 976
             self._errHandler.sync(self)
             token = self._input.LA(1)
-            if token in [78]:
+            if token in [79]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 920
-                self.match(OCLsParser.NUMBER)
+                self.state = 962
+                self.match(BOCLParser.NUMBER)
                 pass
-            elif token in [24, 77]:
+            elif token in [25, 78]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 922
+                self.state = 964
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
-                if _la==24:
-                    self.state = 921
-                    self.match(OCLsParser.SingleQuote)
+                if _la==25:
+                    self.state = 963
+                    self.match(BOCLParser.SingleQuote)
 
 
-                self.state = 924
-                self.match(OCLsParser.ID)
-                self.state = 926
+                self.state = 966
+                self.match(BOCLParser.ID)
+                self.state = 968
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,175,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,185,self._ctx)
                 if la_ == 1:
-                    self.state = 925
-                    self.match(OCLsParser.LPAREN)
+                    self.state = 967
+                    self.match(BOCLParser.LPAREN)
 
 
-                self.state = 929
+                self.state = 971
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,176,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,186,self._ctx)
                 if la_ == 1:
-                    self.state = 928
-                    self.match(OCLsParser.RPAREN)
+                    self.state = 970
+                    self.match(BOCLParser.RPAREN)
 
 
-                self.state = 932
+                self.state = 974
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input,177,self._ctx)
+                la_ = self._interp.adaptivePredict(self._input,187,self._ctx)
                 if la_ == 1:
-                    self.state = 931
-                    self.match(OCLsParser.SingleQuote)
+                    self.state = 973
+                    self.match(BOCLParser.SingleQuote)
 
 
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
@@ -4930,91 +5274,91 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def literal(self):
-            return self.getTypedRuleContext(OCLsParser.LiteralContext,0)
+            return self.getTypedRuleContext(BOCLParser.LiteralContext,0)
 
 
         def SELF(self):
-            return self.getToken(OCLsParser.SELF, 0)
+            return self.getToken(BOCLParser.SELF, 0)
 
         def functionCall(self):
-            return self.getTypedRuleContext(OCLsParser.FunctionCallContext,0)
+            return self.getTypedRuleContext(BOCLParser.FunctionCallContext,0)
 
 
         def LPAREN(self):
-            return self.getToken(OCLsParser.LPAREN, 0)
+            return self.getToken(BOCLParser.LPAREN, 0)
 
         def expression(self):
-            return self.getTypedRuleContext(OCLsParser.ExpressionContext,0)
+            return self.getTypedRuleContext(BOCLParser.ExpressionContext,0)
 
 
         def RPAREN(self):
-            return self.getToken(OCLsParser.RPAREN, 0)
+            return self.getToken(BOCLParser.RPAREN, 0)
 
         def ID(self):
-            return self.getToken(OCLsParser.ID, 0)
+            return self.getToken(BOCLParser.ID, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_primaryExpression
+            return BOCLParser.RULE_primaryExpression
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterPrimaryExpression" ):
                 listener.enterPrimaryExpression(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitPrimaryExpression" ):
                 listener.exitPrimaryExpression(self)
 
 
 
 
     def primaryExpression(self):
 
-        localctx = OCLsParser.PrimaryExpressionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 24, self.RULE_primaryExpression)
+        localctx = BOCLParser.PrimaryExpressionContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 28, self.RULE_primaryExpression)
         try:
-            self.state = 944
+            self.state = 986
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input,179,self._ctx)
+            la_ = self._interp.adaptivePredict(self._input,189,self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 936
+                self.state = 978
                 self.literal()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 937
-                self.match(OCLsParser.SELF)
+                self.state = 979
+                self.match(BOCLParser.SELF)
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 938
+                self.state = 980
                 self.functionCall()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 939
-                self.match(OCLsParser.LPAREN)
-                self.state = 940
+                self.state = 981
+                self.match(BOCLParser.LPAREN)
+                self.state = 982
                 self.expression()
-                self.state = 941
-                self.match(OCLsParser.RPAREN)
+                self.state = 983
+                self.match(BOCLParser.RPAREN)
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 943
-                self.match(OCLsParser.ID)
+                self.state = 985
+                self.match(BOCLParser.ID)
                 pass
 
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5027,49 +5371,49 @@
         __slots__ = 'parser'
 
         def __init__(self, parser, parent:ParserRuleContext=None, invokingState:int=-1):
             super().__init__(parent, invokingState)
             self.parser = parser
 
         def NUMBER(self):
-            return self.getToken(OCLsParser.NUMBER, 0)
+            return self.getToken(BOCLParser.NUMBER, 0)
 
         def STRING_LITERAL(self):
-            return self.getToken(OCLsParser.STRING_LITERAL, 0)
+            return self.getToken(BOCLParser.STRING_LITERAL, 0)
 
         def BOOLEAN_LITERAL(self):
-            return self.getToken(OCLsParser.BOOLEAN_LITERAL, 0)
+            return self.getToken(BOCLParser.BOOLEAN_LITERAL, 0)
 
         def NULL(self):
-            return self.getToken(OCLsParser.NULL, 0)
+            return self.getToken(BOCLParser.NULL, 0)
 
         def getRuleIndex(self):
-            return OCLsParser.RULE_literal
+            return BOCLParser.RULE_literal
 
         def enterRule(self, listener:ParseTreeListener):
             if hasattr( listener, "enterLiteral" ):
                 listener.enterLiteral(self)
 
         def exitRule(self, listener:ParseTreeListener):
             if hasattr( listener, "exitLiteral" ):
                 listener.exitLiteral(self)
 
 
 
 
     def literal(self):
 
-        localctx = OCLsParser.LiteralContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 26, self.RULE_literal)
+        localctx = BOCLParser.LiteralContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 30, self.RULE_literal)
         self._la = 0 # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 946
+            self.state = 988
             _la = self._input.LA(1)
-            if not(((((_la - 72)) & ~0x3f) == 0 and ((1 << (_la - 72)) & 449) != 0)):
+            if not(((((_la - 73)) & ~0x3f) == 0 and ((1 << (_la - 73)) & 449) != 0)):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
```

### Comparing `besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py` & `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py` & `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py` & `besser-1.0.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py` & `besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py` & `besser-1.0.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/django/django_generator.py` & `besser-1.0.1/besser/generators/django/django_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/django/templates/django_fields.py.j2` & `besser-1.0.1/besser/generators/django/templates/django_fields.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/django/templates/django_template.py.j2` & `besser-1.0.1/besser/generators/django/templates/django_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/generator_interface.py` & `besser-1.0.1/besser/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/python_classes/python_classes_generator.py` & `besser-1.0.1/besser/generators/python_classes/python_classes_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/python_classes/templates/class_parameters.py.j2` & `besser-1.0.1/besser/generators/python_classes/templates/class_parameters.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/python_classes/templates/python_classes_template.py.j2` & `besser-1.0.1/besser/generators/python_classes/templates/python_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/rest_api/rest_api_generator.py` & `besser-1.0.1/besser/generators/rest_api/rest_api_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/rest_api/templates/fast_api_template.py.j2` & `besser-1.0.1/besser/generators/rest_api/templates/fast_api_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/sql/sql_generator.py` & `besser-1.0.1/besser/generators/sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/sql/templates/sql_dialects.sql.j2` & `besser-1.0.1/besser/generators/sql/templates/sql_dialects.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/sql/templates/sql_template.sql.j2` & `besser-1.0.1/besser/generators/sql/templates/sql_template.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/sql_alchemy/sql_alchemy_generator.py` & `besser-1.0.1/besser/generators/sql_alchemy/sql_alchemy_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2` & `besser-1.0.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/utilities/image_to_buml.py` & `besser-1.0.1/besser/utilities/image_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser/utilities/utils.py` & `besser-1.0.1/besser/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `besser-1.0.0/besser.egg-info/PKG-INFO` & `besser-1.0.1/besser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.0.0
+Version: 1.0.1
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
@@ -54,14 +54,17 @@
     $ python -m build
     $ pip install dist/besser-*.*.*-py3-none-any.whl
 
 You can check the installation of the *besser* package.
 
     $ pip list
 
+## Examples
+If you want to try examples, check out the [BESSER-examples](https://github.com/BESSER-PEARL/BESSER-examples) repository!
+
 ## Contributing
 
 We encourage contributions from the community and any comment is welcome!
 
 If you are interested in contributing to this project, please read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 
 ## Code of Conduct
```

### Comparing `besser-1.0.0/besser.egg-info/SOURCES.txt` & `besser-1.0.1/besser.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,19 @@
 besser/BUML/metamodel/structural/__init__.py
 besser/BUML/metamodel/structural/structural.py
 besser/BUML/notations/__init__.py
 besser/BUML/notations/objectPlantUML/ODLexer.py
 besser/BUML/notations/objectPlantUML/ODListener.py
 besser/BUML/notations/objectPlantUML/ODParser.py
 besser/BUML/notations/objectPlantUML/__init__.py
+besser/BUML/notations/ocl/BOCLLexer.py
+besser/BUML/notations/ocl/BOCLListener.py
+besser/BUML/notations/ocl/BOCLParser.py
 besser/BUML/notations/ocl/FactoryInstance.py
-besser/BUML/notations/ocl/OCLsLexer.py
-besser/BUML/notations/ocl/OCLsListener.py
-besser/BUML/notations/ocl/OCLsParser.py
+besser/BUML/notations/ocl/OCLWrapper.py
 besser/BUML/notations/ocl/RootHandler.py
 besser/BUML/notations/ocl/__init__.py
 besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
 besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
 besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
 besser/BUML/notations/structuralPlantUML/__init__.py
 besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
@@ -58,8 +59,20 @@
 besser/generators/sql/templates/sql_template.sql.j2
 besser/generators/sql_alchemy/__init__.py
 besser/generators/sql_alchemy/sql_alchemy_generator.py
 besser/generators/sql_alchemy/templates/__init__.py
 besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
 besser/utilities/__init__.py
 besser/utilities/image_to_buml.py
-besser/utilities/utils.py
+besser/utilities/utils.py
+tests/__init__.py
+tests/gui/__init__.py
+tests/gui/gui_model.py
+tests/gui/test_gui.py
+tests/notations/__init__.py
+tests/object/__init__.py
+tests/object/library_object.py
+tests/object/test_object_mm.py
+tests/ocl/__init__.py
+tests/ocl/test_ocl_parser.py
+tests/structural/__init__.py
+tests/structural/test_structural.py
```

### Comparing `besser-1.0.0/setup.cfg` & `besser-1.0.1/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 720d 0a76 6572 7369   = besser..versi
-00000020: 6f6e 203d 2031 2e30 2e30 0d0a 6175 7468  on = 1.0.0..auth
+00000020: 6f6e 203d 2031 2e30 2e31 0d0a 6175 7468  on = 1.0.1..auth
 00000030: 6f72 203d 204c 7578 656d 626f 7572 6720  or = Luxembourg 
 00000040: 496e 7374 6974 7574 6520 6f66 2053 6369  Institute of Sci
 00000050: 656e 6365 2061 6e64 2054 6563 686e 6f6c  ence and Technol
 00000060: 6f67 790d 0a64 6573 6372 6970 7469 6f6e  ogy..description
 00000070: 203d 2042 4553 5345 520d 0a6c 6f6e 675f   = BESSER..long_
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000090: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
```

