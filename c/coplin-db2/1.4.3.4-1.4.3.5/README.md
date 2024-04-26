# Comparing `tmp/coplin_db2-1.4.3.4.tar.gz` & `tmp/coplin_db2-1.4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coplin_db2-1.4.3.4.tar", last modified: Thu Mar  7 12:03:32 2024, max compression
+gzip compressed data, was "coplin_db2-1.4.3.5.tar", last modified: Fri Apr 26 14:43:01 2024, max compression
```

## Comparing `coplin_db2-1.4.3.4.tar` & `coplin_db2-1.4.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-07 12:02:44.000000 coplin_db2-1.4.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-03-07 12:02:44.000000 coplin_db2-1.4.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/coplin_db2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-07 12:03:32.000000 coplin_db2-1.4.3.4/coplin_db2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-07 12:03:32.000000 coplin_db2-1.4.3.4/coplin_db2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:03:32.000000 coplin_db2-1.4.3.4/coplin_db2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-07 12:03:32.000000 coplin_db2-1.4.3.4/coplin_db2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-07 12:03:32.000000 coplin_db2-1.4.3.4/coplin_db2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/db2/
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-03-07 12:02:44.000000 coplin_db2-1.4.3.4/db2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/db2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-07 12:02:44.000000 coplin_db2-1.4.3.4/db2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:03:32.113051 coplin_db2-1.4.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-07 12:02:44.000000 coplin_db2-1.4.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-26 14:42:12.000000 coplin_db2-1.4.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-26 14:42:12.000000 coplin_db2-1.4.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/coplin_db2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-26 14:43:01.000000 coplin_db2-1.4.3.5/coplin_db2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-26 14:43:01.000000 coplin_db2-1.4.3.5/coplin_db2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 14:43:01.000000 coplin_db2-1.4.3.5/coplin_db2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-26 14:43:01.000000 coplin_db2-1.4.3.5/coplin_db2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-26 14:43:01.000000 coplin_db2-1.4.3.5/coplin_db2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/db2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12309 2024-04-26 14:42:12.000000 coplin_db2-1.4.3.5/db2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/db2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-26 14:42:12.000000 coplin_db2-1.4.3.5/db2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 14:43:01.227615 coplin_db2-1.4.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-26 14:42:12.000000 coplin_db2-1.4.3.5/setup.py
```

### Comparing `coplin_db2-1.4.3.4/LICENSE` & `coplin_db2-1.4.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `coplin_db2-1.4.3.4/PKG-INFO` & `coplin_db2-1.4.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coplin_db2
-Version: 1.4.3.4
+Version: 1.4.3.5
 Summary: Um módulo de conveniência para manipulação de bancos de dados IBM DB2 em Python.
 Home-page: https://github.com/COPLIN-UFSM/db2
 Author: Henry Cagnini
 Author-email: henry.cagnini@ufsm.br
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `coplin_db2-1.4.3.4/README.md` & `coplin_db2-1.4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `coplin_db2-1.4.3.4/coplin_db2.egg-info/PKG-INFO` & `coplin_db2-1.4.3.5/coplin_db2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coplin_db2
-Version: 1.4.3.4
+Version: 1.4.3.5
 Summary: Um módulo de conveniência para manipulação de bancos de dados IBM DB2 em Python.
 Home-page: https://github.com/COPLIN-UFSM/db2
 Author: Henry Cagnini
 Author-email: henry.cagnini@ufsm.br
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `coplin_db2-1.4.3.4/db2/__init__.py` & `coplin_db2-1.4.3.5/db2/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -237,14 +237,38 @@
         row_str = ', '.join(row_values)
 
         insert_sql = f"""INSERT INTO {table_name} ({column_names_str}) VALUES ({row_str});"""
 
         success = self.modify(insert_sql)
         return success
 
+    def update(self, table_name: str, where: dict, values: dict) -> bool:
+        """
+        Atualiza os valores de uma tupla (apresentada como um dicionário) em uma tabela.
+
+        :param table_name: Nome da tabela onde os dados serão atualizados.
+        :param where: Dicionário com a cláusula WHERE. As chaves do dicionário são os nomes das colunas, e seus valores
+            os valores da tupla a ser atualizada.
+        :param values: Valores a serem atualizados na tabela do banco de dados.
+        :return: Um booleano denotando se a operação de atualização foi bem sucedida
+        """
+
+        where_column_names, where_row_values = self.__collect__(where)
+
+        column_names, row_values = self.__collect__(values)
+        insert_str = ', '.join([f'{k} = {v}' for k, v in zip(column_names, row_values)])
+        where_str = ' AND '.join(f'{k} = {v}' for k, v in zip(where_column_names, where_row_values))
+
+        update_sql = f"""
+        UPDATE {table_name} SET {insert_str} WHERE {where_str} 
+        """
+
+        success = self.modify(update_sql)
+        return success
+
     def generic_update(self, table_name: str, where: dict, sqlite_row: dict) -> bool:
         """
         Atualiza os valores de uma tupla (apresentada como um dicionário) em uma tabela.
 
         :param table_name: Nome da tabela onde os dados serão atualizados.
         :param where: Dicionário com a cláusula WHERE. As chaves do dicionário são os nomes das colunas, e seus valores
             os valores da tupla a ser atualizada.
```

### Comparing `coplin_db2-1.4.3.4/db2/utils/__init__.py` & `coplin_db2-1.4.3.5/db2/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coplin_db2-1.4.3.4/setup.py` & `coplin_db2-1.4.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = Path(__file__).parent
 
 with open(os.path.join(this_directory, 'README.md'), 'r', encoding='utf-8') as read_file:
     long_description = read_file.read()
 
 setup(
     name='coplin_db2',
-    version='1.4.3.4',
+    version='1.4.3.5',
     url='https://github.com/COPLIN-UFSM/db2',
     author='Henry Cagnini',
     author_email='henry.cagnini@ufsm.br',
     description='Um módulo de conveniência para manipulação de bancos de dados IBM DB2 em Python.',
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=['db2', 'db2.utils'],
```

