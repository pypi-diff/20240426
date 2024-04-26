# Comparing `tmp/edupils-0.1.8.tar.gz` & `tmp/edupils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edupils-0.1.8.tar", last modified: Fri Feb 16 21:34:49 2024, max compression
+gzip compressed data, was "edupils-0.1.9.tar", last modified: Sun Feb 18 22:04:22 2024, max compression
```

## Comparing `edupils-0.1.8.tar` & `edupils-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-16 21:34:41.000000 edupils-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-16 21:34:49.531599 edupils-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-16 21:34:41.000000 edupils-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.527599 edupils-0.1.8/edupils/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/constantes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/edupils/desafios/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desafios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desafios/gude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8614 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desafios/labirinto.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desafios/turtle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/edupils/desenho/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desenho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desenho/desenho.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/desenho/painel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/edupils/imagem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/imagem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/imagem/image_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/edupils/sons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/sons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-16 21:34:41.000000 edupils-0.1.8/edupils/sons/audio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 21:34:49.531599 edupils-0.1.8/edupils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-16 21:34:49.000000 edupils-0.1.8/edupils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-16 21:34:49.000000 edupils-0.1.8/edupils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 21:34:49.000000 edupils-0.1.8/edupils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-16 21:34:49.000000 edupils-0.1.8/edupils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 21:34:49.531599 edupils-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-16 21:34:41.000000 edupils-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-18 22:04:14.000000 edupils-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-18 22:04:22.784056 edupils-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-18 22:04:14.000000 edupils-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.780055 edupils-0.1.9/edupils/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/constantes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/edupils/desafios/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desafios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desafios/gude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desafios/labirinto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desafios/turtle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/edupils/desenho/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desenho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desenho/desenho.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/desenho/painel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/edupils/imagem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/imagem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/imagem/image_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/edupils/sons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/sons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-18 22:04:14.000000 edupils-0.1.9/edupils/sons/audio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 22:04:22.784056 edupils-0.1.9/edupils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-18 22:04:22.000000 edupils-0.1.9/edupils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-18 22:04:22.000000 edupils-0.1.9/edupils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 22:04:22.000000 edupils-0.1.9/edupils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-18 22:04:22.000000 edupils-0.1.9/edupils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 22:04:22.784056 edupils-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-18 22:04:14.000000 edupils-0.1.9/setup.py
```

### Comparing `edupils-0.1.8/LICENSE` & `edupils-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edupils-0.1.8/edupils/constantes.py` & `edupils-0.1.9/edupils/constantes.py`

 * *Files identical despite different names*

### Comparing `edupils-0.1.8/edupils/desafios/labirinto.py` & `edupils-0.1.9/edupils/desafios/labirinto.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,17 @@
                         j * largura_do_tile, 
                         i * largura_do_tile, 
                         largura_do_tile, 
                         largura_do_tile, 
                         camada, 
                         cor_preenchimento=constantes.COR_ESCURA
                     )
+
+    def get_labirinto(self):
+        return self.labirinto, self.paredes
     
 
 class Jogador(ABC):
     DIRECOES = {
         'cima': (-1, 0),
         'baixo': (1, 0),
         'direita': (0, 1),
```

### Comparing `edupils-0.1.8/edupils/desenho/desenho.py` & `edupils-0.1.9/edupils/desenho/desenho.py`

 * *Files identical despite different names*

### Comparing `edupils-0.1.8/edupils/desenho/painel.py` & `edupils-0.1.9/edupils/desenho/painel.py`

 * *Files identical despite different names*

### Comparing `edupils-0.1.8/setup.py` & `edupils-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your requirements.txt file
 with open('requirements.txt') as f:
     required_packages = f.read().splitlines()
 
 setup(
     name='edupils',
-    version='0.1.8',
+    version='0.1.9',
     author='Georges Spyrides',
     author_email='georgesmss@gmail.com',
     packages=find_packages(),
     install_requires=required_packages,
     url='https://github.com/georgesms/edupils',
     license='MIT',
     description='A collection of educational tools for Python',
```

