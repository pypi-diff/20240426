# Comparing `tmp/pyDolarVenezuela-1.4.2.tar.gz` & `tmp/pydolarvenezuela-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDolarVenezuela-1.4.2.tar", last modified: Tue Apr  2 20:34:22 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.4.3.tar", last modified: Thu Apr 25 23:19:00 2024, max compression
```

## Comparing `pyDolarVenezuela-1.4.2.tar` & `pydolarvenezuela-1.4.3.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:22.011117 pyDolarVenezuela-1.4.2/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pyDolarVenezuela-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     6232 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     3863 2024-04-02 19:50:04.000000 pyDolarVenezuela-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.874999 pyDolarVenezuela-1.4.2/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2453 2024-04-02 19:51:59.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.926782 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.926782 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/__init__.py
--rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.975021 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     1420 2024-04-02 19:36:45.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/dpedidos.py
--rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/ivenezuela.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-02 20:34:21.991657 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     6232 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      765 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-02 20:34:21.000000 pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2024-04-02 19:51:54.000000 pyDolarVenezuela-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 20:34:22.011117 pyDolarVenezuela-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1472 2024-04-02 19:51:50.000000 pyDolarVenezuela-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.245956 pydolarvenezuela-1.4.3/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     7276 2024-04-25 23:19:00.229489 pydolarvenezuela-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4885 2024-04-25 23:08:28.000000 pydolarvenezuela-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.946504 pydolarvenezuela-1.4.3/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2562 2024-04-25 21:35:52.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.979889 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.979889 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:18:59.996426 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      612 2024-04-25 22:15:03.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.013061 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      159 2024-04-25 21:35:09.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      802 2023-11-22 00:44:52.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2023-11-23 16:38:28.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/network.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.196006 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     3516 2024-04-25 22:29:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2159 2024-04-02 19:39:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     2529 2024-04-02 19:27:15.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     1842 2024-04-02 19:27:50.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/dpedidos.py
+-rw-rw-rw-   0        0        0     3002 2024-04-02 19:28:10.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     4136 2024-04-02 19:28:30.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/ivenezuela.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.213218 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     1201 2023-10-17 03:57:15.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-25 23:19:00.229489 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7276 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-25 23:18:59.000000 pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-25 23:09:11.000000 pydolarvenezuela-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 23:19:00.245956 pydolarvenezuela-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-25 23:09:18.000000 pydolarvenezuela-1.4.3/setup.py
```

### Comparing `pyDolarVenezuela-1.4.2/LICENSE` & `pydolarvenezuela-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/PKG-INFO` & `pydolarvenezuela-1.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.2
+Version: 1.4.3
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -38,14 +38,15 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: curl_cffi
 Requires-Dist: beautifulsoup4
 Requires-Dist: babel
 Requires-Dist: pytz
 Requires-Dist: colorama
+Requires-Dist: redis
 
 ![Portada pyDolarVenezuela](https://github.com/fcoagz/pydolarvenezuela/blob/main/static/pyDolarVenezuela.jpg?raw=true)
 
 pyDolarVenezuela es una librería de Python que te brinda la posibilidad de obtener los valores del dólar en distintos monitores en Venezuela, así como las tasas de cambio proporcionadas por el Banco Central de Venezuela. Esta librería consulta diversas páginas web que ofrecen información actualizada sobre el valor del dólar:
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
@@ -69,21 +70,52 @@
 ```python
 from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
+pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
+
+```python
+from pyDolarVenezuela import Monitor, Redis
+from pyDolarVenezuela.models.pages import BCV, CriptoDolar, ExchangeMonitor
+
+# Defecto
+db = Redis(
+    host='localhost',
+    port=6379
+)
+
+monitor = Monitor(CriptoDolar, 'USD', db=db)
+
+```
+Si prefieres utilizar [Redis Cloud](https://app.redislabs.com/) en lugar de una instancia local de `Redis`, puedes hacerlo cambiando el host y el puerto cuando creas la instancia de `Redis`.
+
+```python
+db = Redis(
+    host='redis-cloud-host',
+    port='redis-cloud-port',
+    password='*************'
+)
+```
+
+```
+Aunque Redis puede funcionar en Windows, no es una versión oficial. Para un entorno de producción estable, se recomienda instalar Redis en Linux o utilizar Redis Cloud.
+```
+
+
 El parámetro `currency` de la clase `Monitor` por defecto tiene el valor: `USD`, verifique que la página de la que desea obtener los datos pueda expresar precios en `EUR`.
 
 ```python
 print(ExchangeMonitor.currencies)
 
 >> ['usd', 'eur']
 ```
+
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
```

### Comparing `pyDolarVenezuela-1.4.2/README.md` & `pydolarvenezuela-1.4.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,21 +24,52 @@
 ```python
 from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
+pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
+
+```python
+from pyDolarVenezuela import Monitor, Redis
+from pyDolarVenezuela.models.pages import BCV, CriptoDolar, ExchangeMonitor
+
+# Defecto
+db = Redis(
+    host='localhost',
+    port=6379
+)
+
+monitor = Monitor(CriptoDolar, 'USD', db=db)
+
+```
+Si prefieres utilizar [Redis Cloud](https://app.redislabs.com/) en lugar de una instancia local de `Redis`, puedes hacerlo cambiando el host y el puerto cuando creas la instancia de `Redis`.
+
+```python
+db = Redis(
+    host='redis-cloud-host',
+    port='redis-cloud-port',
+    password='*************'
+)
+```
+
+```
+Aunque Redis puede funcionar en Windows, no es una versión oficial. Para un entorno de producción estable, se recomienda instalar Redis en Linux o utilizar Redis Cloud.
+```
+
+
 El parámetro `currency` de la clase `Monitor` por defecto tiene el valor: `USD`, verifique que la página de la que desea obtener los datos pueda expresar precios en `EUR`.
 
 ```python
 print(ExchangeMonitor.currencies)
 
 >> ['usd', 'eur']
 ```
+
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
```

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import Literal
 from colorama import Fore
 
 from . import network
-from .pages import Monitor as Page
+from .models.pages import Monitor as Page
+from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
 version = '1.4.2'
 
 class CheckVersion:
     check = True
@@ -17,15 +18,15 @@
             response = network.get("https://pypi.org/pypi/pydolarvenezuela/json")
             latest_version = json.loads(response)["info"]["version"]
 
             if version != latest_version:
                 print(f"{Fore.GREEN}New version: {latest_version}.{Fore.RESET} {Fore.RED}Current version {version}.{Fore.RESET} write the following command: pip install --upgrade pyDolarVenezuela\n")
 
 class Monitor:
-    def __init__(self, provider: Page, currency: Literal['USD', 'EUR'] = 'USD') -> None:
+    def __init__(self, provider: Page, currency: Literal['USD', 'EUR'] = 'USD', db: Redis = None) -> None:
         """
         La clase `Monitor` proporciona funcionalidades para consultar los precios de diversos monitores en Venezuela.
 
         Parámetros:
         - `provider`: La página de la que se accederán los datos.
         - `currency`: La moneda en la que se expresarán los precios. Puede ser `USD` o `EUR`. Por defecto es `USD`.
         """
@@ -33,24 +34,26 @@
         if CheckVersion.check:
             CheckVersion._check_dependence_version()
         if not isinstance(provider, Page):
             raise TypeError("The parameter must be an object of type Monitor.")
         
         self.provider = provider
         self.currency = currency.lower()
+        self.db       = db
     
     def get_value_monitors(self, monitor_code: str = None, name_property: Literal['title', 'price', 'last_update'] = None, prettify: bool = False):
         """
         El método `get_value_monitors` permite acceder a los datos extraídos de los monitores.
 
         Parámetros:
         - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
         - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
         - `prettify`: Si es True, muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
         """ 
         return select_monitor(
             self.provider,
+            db=self.db,
             currency=self.currency,
             monitor_code=monitor_code,
             name_property=name_property,
             prettify=prettify
         )
```

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/models/pages.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/criptodolar.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/dpedidos.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/dpedidos.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/provider/ivenezuela.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/provider/ivenezuela.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.4.3/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.4.2
+Version: 1.4.3
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -38,14 +38,15 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: curl_cffi
 Requires-Dist: beautifulsoup4
 Requires-Dist: babel
 Requires-Dist: pytz
 Requires-Dist: colorama
+Requires-Dist: redis
 
 ![Portada pyDolarVenezuela](https://github.com/fcoagz/pydolarvenezuela/blob/main/static/pyDolarVenezuela.jpg?raw=true)
 
 pyDolarVenezuela es una librería de Python que te brinda la posibilidad de obtener los valores del dólar en distintos monitores en Venezuela, así como las tasas de cambio proporcionadas por el Banco Central de Venezuela. Esta librería consulta diversas páginas web que ofrecen información actualizada sobre el valor del dólar:
 
 | Página Web | URL | Estado
 |------------|-------------|-------------|
@@ -69,21 +70,52 @@
 ```python
 from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
 from pyDolarVenezuela import Monitor
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 ```
 
+pyDolarVenezuela utiliza [Redis](https://github.com/redis/redis-py), un motor de base de datos en memoria, para almacenar y procesar datos. Esto nos ayuda para calcular el cambio, el porcentaje, el color y el símbolo, y se devuelven los datos actualizados.
+
+```python
+from pyDolarVenezuela import Monitor, Redis
+from pyDolarVenezuela.models.pages import BCV, CriptoDolar, ExchangeMonitor
+
+# Defecto
+db = Redis(
+    host='localhost',
+    port=6379
+)
+
+monitor = Monitor(CriptoDolar, 'USD', db=db)
+
+```
+Si prefieres utilizar [Redis Cloud](https://app.redislabs.com/) en lugar de una instancia local de `Redis`, puedes hacerlo cambiando el host y el puerto cuando creas la instancia de `Redis`.
+
+```python
+db = Redis(
+    host='redis-cloud-host',
+    port='redis-cloud-port',
+    password='*************'
+)
+```
+
+```
+Aunque Redis puede funcionar en Windows, no es una versión oficial. Para un entorno de producción estable, se recomienda instalar Redis en Linux o utilizar Redis Cloud.
+```
+
+
 El parámetro `currency` de la clase `Monitor` por defecto tiene el valor: `USD`, verifique que la página de la que desea obtener los datos pueda expresar precios en `EUR`.
 
 ```python
 print(ExchangeMonitor.currencies)
 
 >> ['usd', 'eur']
 ```
+
 El método `get_value_monitors` se utiliza después de crear una instancia del objeto Monitor y permite el acceso a los datos almacenados en el diccionario. Los siguientes parámetros serían los siguientes:
 
 - `monitor_code`: El código del monitor del cual se desea obtener información. Por defecto es `None`.
 - `name_property`: El nombre de la propiedad específica del diccionario de la información del monitor extraído que se desea obtener. Por defecto es `None`.
 - `prettify`: Muestra los precios en formato de moneda con el símbolo de Bolívares. Por defecto es `False`.
 
 ```python
```

### Comparing `pyDolarVenezuela-1.4.2/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.4.3/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 pyDolarVenezuela/__init__.py
 pyDolarVenezuela/network.py
-pyDolarVenezuela/pages.py
 pyDolarVenezuela/utils.py
 pyDolarVenezuela.egg-info/PKG-INFO
 pyDolarVenezuela.egg-info/SOURCES.txt
 pyDolarVenezuela.egg-info/dependency_links.txt
 pyDolarVenezuela.egg-info/requires.txt
 pyDolarVenezuela.egg-info/top_level.txt
 pyDolarVenezuela/assets/__init__.py
 pyDolarVenezuela/assets/icons/__init__.py
+pyDolarVenezuela/data/__init__.py
+pyDolarVenezuela/data/redis.py
+pyDolarVenezuela/models/__init__.py
+pyDolarVenezuela/models/database.py
+pyDolarVenezuela/models/pages.py
 pyDolarVenezuela/provider/__init__.py
 pyDolarVenezuela/provider/bcv.py
 pyDolarVenezuela/provider/criptodolar.py
 pyDolarVenezuela/provider/dpedidos.py
 pyDolarVenezuela/provider/exchangemonitor.py
 pyDolarVenezuela/provider/ivenezuela.py
 pyDolarVenezuela/tools/__init__.py
```

### Comparing `pyDolarVenezuela-1.4.2/pyproject.toml` & `pydolarvenezuela-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.4.2"
+version = "1.4.3"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
+  "redis",
 ]
 requires-python = ">=3.9"
 authors = [
   {name = "Francisco Griman", email = "grihardware@gmail.com"}
 ]
 description = "Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV."
 readme = "README.md"
```

### Comparing `pyDolarVenezuela-1.4.2/setup.py` & `pydolarvenezuela-1.4.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.4.2'
+VERSION = '1.4.3'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
@@ -16,15 +16,16 @@
 
 INSTALL_REQUIRES = [
       'requests',
       'curl_cffi',
       'beautifulsoup4',
       'babel',
       'colorama',
-      'pytz'
+      'pytz',
+      'redis'
       ]
 
 CLASSIFIERS = [
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

