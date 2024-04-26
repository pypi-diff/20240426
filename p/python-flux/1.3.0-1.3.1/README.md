# Comparing `tmp/python_flux-1.3.0.tar.gz` & `tmp/python_flux-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.3.0.tar", max compression
+gzip compressed data, was "python_flux-1.3.1.tar", max compression
```

## Comparing `python_flux-1.3.0.tar` & `python_flux-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     8248 2024-04-25 01:56:27.648550 python_flux-1.3.0/README.rst
--rw-r--r--   0        0        0      741 2024-04-25 04:02:34.745676 python_flux-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.3.0/python_flux/__init__.py
--rw-r--r--   0        0        0    23050 2024-04-25 04:02:14.645860 python_flux-1.3.0/python_flux/flux.py
--rw-r--r--   0        0        0      759 2024-04-22 18:08:07.620526 python_flux-1.3.0/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1921 2024-04-25 03:44:04.154407 python_flux-1.3.0/python_flux/producers.py
--rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.3.0/python_flux/subscribers.py
--rw-r--r--   0        0        0     8979 1970-01-01 00:00:00.000000 python_flux-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     8872 2024-04-26 12:27:05.738836 python_flux-1.3.1/README.rst
+-rw-r--r--   0        0        0      741 2024-04-26 12:27:05.272758 python_flux-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.3.1/python_flux/__init__.py
+-rw-r--r--   0        0        0    23514 2024-04-26 12:27:05.273713 python_flux-1.3.1/python_flux/flux.py
+-rw-r--r--   0        0        0      759 2024-04-25 04:03:40.583703 python_flux-1.3.1/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1921 2024-04-25 04:03:40.584710 python_flux-1.3.1/python_flux/producers.py
+-rw-r--r--   0        0        0     1641 2024-04-18 05:35:27.173689 python_flux-1.3.1/python_flux/subscribers.py
+-rw-r--r--   0        0        0     9603 1970-01-01 00:00:00.000000 python_flux-1.3.1/PKG-INFO
```

### Comparing `python_flux-1.3.0/README.rst` & `python_flux-1.3.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,215 +1,257 @@
 python-flux
 ===========
 
 Esta librería implementa una interfaz de programación similar a la brindada por el proyecto **WebFlux** de spring.
 
-La interfaz implementada es similar a la siguiente: `Flux <https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Flux.html>`_
+La interfaz implementada es similar a la siguiente:
+`Flux <https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Flux.html>`_
 
 
 filter(predicate, on_mismatch)
 ------------------------------
 
 Permite filtrar un flujo permitiendo continuar a aquellos valores que cumplen con el predicado que se indica.
 
 Si no se cumple el predicado opcionalmente se puede indicar una función que dado el valor y el contexto actual retorna el valor que se enviará al flujo.
 
+**Parámetros:**
+
 -  **predicate**: función(valor, contexto) que retorna un booleano
 
 -  **on_mismatch**: función(valor, contexto) que retorna un valor alternativo al testeado originalmente
 
 
 map(map_function)
 -----------------
 
 Permite modificar el valor de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y se substituirá en el mismo por lo obtenido de la función.
 
+**Parámetros:**
+
 -  **map_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
 map_if(predicate, map_function)
 -------------------------------
 Evalúa el predicado, si este es verdadero mapea el valor actual con la función de mapeo.
 
+**Parámetros:**
+
 - **predicate**: función(valor, contexto) predicado que se evalúa.
 
 - **map_function**: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
 
 
 map_context(map_context_function)
 ---------------------------------
 
 Permite modificar el contexto de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y retornará un nuevo contexto que sustituirá al actual
 
+**Parámetros:**
+
 -  **map_context_function**: función(valor, contexto) desde donde se obtendrá el contexto a subsituir.
 
 
 flat_map(flatmap_function)
 --------------------------
 
 Permite sustituir el valor de un flujo por elementos de otro flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo original y retornará un flujo cuyos elementos se usarán como nuevo origen del flujo de datos.
 
+**Parámetros:**
+
 -  **flatmap_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
 do_on_next(on_next)
 -------------------
 
 Ejecuta para cada elemento del flujo una acción de forma asincrónica.
 No afecta a los valores del flujo.
 
+**Parámetros:**
+
 -  **on_next**: función(valor, contexto) que se ejecutará para cada valor del flujo
 
 -  **on_error**: función(ex, contexto) se ejecuta en caso de error
 
 - **exec_async**: Booleano que indica si las funciones se ejecutarán de forma asíncrona
 
 
 delay_ms(delay_ms, predicate=fu.default_predicate)
 --------------------------------------------------
 
 Retrasa en delay milisegundos la ejecución de paso del flujo. Esto marca el tiempo en que se procesarán sus elementos.
 
+**Parámetros:**
+
 -  **delay_ms**: Delay en milisegundos que se retrasará el procesamiento de los elementos del flujo
 
 -  **predicate**: Si es verdadero se aplica el delay establecido
 
 
 parallel(pool_size=5, metric_function=None)
 -------------------------------------------
 Consume elementos de un flujo en paralelo.
 Utiliza tantos hilos como se haya configurado en pool_size.
 Si se indica, con cada elemento procesado invoca a la función metric_function pasándole un mapa con la siguiente
 información:
+
 - pool_size: Tamaño del pool
-used_pool: Cantidad de hilos utilizados
-avg_used_pool: Promedio de hilos utilizados
-avg_task_time: Promedio de tiempo de ejecución de la obtención de elementos en paralelo
-rate_s: Tasa de procesamiento
+
+- used_pool: Cantidad de hilos utilizados
+
+- avg_used_pool: Promedio de hilos utilizados
+
+- avg_task_time: Promedio de tiempo de ejecución de la obtención de elementos en paralelo
+
+- rate_s: Tasa de procesamiento
+
+**Parámetros:**
 
 - **pool_size**: Pool de hilos a utilizar
-- **metric_function**: función(metrics) Esta es una función que si se setea recibe con cada elemento procesado  un bloque de métricas sobre la ejecución paralela
 
+- **metric_function**: función(metrics, context) Esta es una función que si se setea recibe con cada elemento procesado un bloque de métricas sobre la ejecución paralela
 
 
-take(n)
--------
+take_if(n, predicate=None)
+--------------------------
 
-Corta la ejecución del flujo luego de procesar n elementos.
+Corta la ejecución del flujo luego de procesar n elementos que cumplen con la condición indicada.
+Si no se indica una función de predicado se cortará la ejecución al procesar n elementos.
 
+**Parámetros:**
 -  **n**: Cantidad de elementos procesados antes de cortar el flujo
-
+-  **predicate**: función(value, context) Si esta función retorna verdadero ese elemento es tomado en cuenta
 
 take_until_seconds(n)
 ---------------------
 
 Corta la ejecución del flujo luego de n segundos de procesamiento.
 
 La ejecución se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior al configurado.
 
+**Parámetros:**
+
 -  **n**: Cantidad de segundos que el stream procesa elementos.
 
 chunks(n)
 ---------
 
 Emite un valor construido como una lista de como máximo n valores obtenidos del flujo padre.
 
 Si algún valor mientras se construye el chunk da error se emiten los elementos recolectados y luego se propaga el error.
 
+**Parámetros:**
+
 - ***n***: Cantidad de elementos recolectados antes de emitir el evento de lista.
 
 
 log(build_log_message, build_error_message, level)
 --------------------------------------------------
 
 Recibe una función(valor, contexto) que retorna un mensaje de texto que será logueado con el nivel de log indicado en level.
 
 El logueo se hace de forma asincrónica y no afecta al flujo.
 
+**Parámetros:**
+
 -  **build_log_message**: Función que dado un valor y contexto retorna un mensaje a loguear
 
 -  **build_error_message**: Función que dada una excepción y el contexto retorna el mensaje a loguear como ERROR
 
 -  **level**: Nivel de logueo que se usará
 
 
 on_error_resume(resume=fu.default_error_resume, exceptions=[Exception])
 -----------------------------------------------------------------------
 En caso de error, este paso ejecuta la función resume que debe retornar un valor a partir del error recibido por parámetro.
 
+**Parámetros:**
+
 -  **resume**: función(ex, contexto) Debe retornar el valor a sustituir en el flujo.
 
 -  **exceptions**: Lista de excepciones para los que se aplica la función resume.
 
 
 on_error_retry(retries=3, delay_ms=lambda i: 0, exceptions=[Exception])
 -----------------------------------------------------------------------
 
 En caso de error, este paso intenta ejecutar nuevamente el flujo **retries** cantidad de veces.
 
 Esto lo hace sólo para las excepciones indicadas por **exceptions** y los reintentos tienen un delay dado por la función **delay_ms** que recibe el número de reintento que es y espera obtener los ms de delay que se deben aplicar.
 
+**Parámetros:**
+
 -  **retries**: Cantidad de reintentos a aplicar
 
 -  **delay_ms**: función(int) que retorna dado el número de reintento en el que se está cuantos: ms de delay se deben aplicar.
 
 -  **exceptions**: Lista de excepciones para los que se aplica el método resume.
 
 
 subscribe(context, skip_error)
 ------------------------------
 
 Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán los valores del flujo.
 
+**Parámetros:**
+
 -  **skip_error**: Ignora errores al obtener los valores desde el flujo
 
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Objeto iterable
 
 
 foreach(on_success=fu.default_success, on_error=fu.default_error, context={})
 -----------------------------------------------------------------------------
 
 Itera sobre los elementos del flujo e invoca a funciones **on_success** y on_error dependiendo el estado del flujo.
 
+**Parámetros:**
+
 -  **on_success**: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
 
 -  **on_error**: función(ex, valor, contexto) se invoca si hay un error en el flujo. Esto no corta el procesamiento a menos que se lance una excepción en el método
 
 -  **on_finish**: función(contexto) se invoca cuando el flujo finaliza
 
 -  **context**: Contexto inicial para el flujo
 
 
 to_list(context={}, skip_error=True)
 ------------------------------------
 
 Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
 
+**Parámetros:**
+
 -  **context**: contexto inicial para el flujo
 
 -  **skip_error**: Ignora errores al obtener los valores desde el flujo
 
 -  **return**: Lista de elementos
 
 
 collect(init=lambda c: {}, reduce=lambda v, a: a, context={})
 -------------------------------------------------------------
 
 Permite resumir en un sólo objeto el procesamiento de todos los elementos del flujo.
 
 Se inicializa un acumulador a través de la función init(contexto) y luego para cada elemento del flujo se invoca la función reduce(valor, acumulador) que procesa el valor y retorna un nuevo valor del acumulador.
 
+**Parámetros:**
+
 -  **init**: función(contexto) Retorna valor inicial del acumulador
 
 -  **reduce**: funcón(valor, acumulador) Dados el nuevo valor y el acumulador retorna un nuevo valor de acumulador.
 
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Acumulador
```

### Comparing `python_flux-1.3.0/pyproject.toml` & `python_flux-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.3.0"
+version = "1.3.1"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `python_flux-1.3.0/python_flux/flux.py` & `python_flux-1.3.1/python_flux/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import threading
-import traceback
 import types
 import time
 from datetime import timedelta, datetime
 from functools import partial
 from jsonmerge import merge
 from python_flux.flux_utilis import FluxUtils as fu
 from python_flux.subscribers import SSubscribe
@@ -90,21 +89,22 @@
         Si algún valor mientras se construye el chunk da error se emiten los elementos recolectados
         y luego se propaga el error.
 
         :param n: Cantidad de elementos recolectados antes de emitir el evento de lista.
         """
         return FChunks(n, self)
 
-    def take(self, n):
+    def take(self, n, predicate=None):
         """
         Corta la ejecución del flujo luego de n elementos procesados.
 
         :param n: Cantidad de elementos procesados antes de cortar el flujo
+        :param predicate: función(value, context) Si esta función retorna verdadero ese elemento es tomado en cuenta
         """
-        return FTake(n, self)
+        return FTake(n, predicate, self)
 
     def take_until_seconds(self, n):
         """
         Corta la ejecución del flujo luego de n segundos de procesamiento.
         La ejecición se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior
         al configurado.
 
@@ -291,22 +291,32 @@
                 return value, e, ctx
             return v, e, ctx
 
         return value, e, ctx
 
 
 class FTake(Stream):
-    def __init__(self, count, flux):
+    def __init__(self, count, predicate, flux):
         super().__init__(flux)
         self.count = count
+        self.predicate = predicate
         self.idx = 0
 
     def next(self, context):
         value, e, ctx = super(FTake, self).next(context)
-        self.idx = self.idx + 1
+        if e is not None:
+            return value, e, ctx
+        if self.predicate is not None:
+            valid, e = fu.try_or(partial(self.predicate), value, ctx)
+        else:
+            valid = False
+        if e is not None:
+            return value, e, ctx
+        if valid:
+            self.idx = self.idx + 1
         if self.idx <= self.count:
             return value, e, ctx
         else:
             return value, StopIteration(), ctx
 
 
 class FTakeDuringTimeDelta(Stream):
```

### Comparing `python_flux-1.3.0/python_flux/flux_utilis.py` & `python_flux-1.3.1/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.0/python_flux/producers.py` & `python_flux-1.3.1/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.0/python_flux/subscribers.py` & `python_flux-1.3.1/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.3.0/PKG-INFO` & `python_flux-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.3.0
+Version: 1.3.1
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -17,217 +17,259 @@
 Description-Content-Type: text/x-rst
 
 python-flux
 ===========
 
 Esta librería implementa una interfaz de programación similar a la brindada por el proyecto **WebFlux** de spring.
 
-La interfaz implementada es similar a la siguiente: `Flux <https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Flux.html>`_
+La interfaz implementada es similar a la siguiente:
+`Flux <https://projectreactor.io/docs/core/release/api/reactor/core/publisher/Flux.html>`_
 
 
 filter(predicate, on_mismatch)
 ------------------------------
 
 Permite filtrar un flujo permitiendo continuar a aquellos valores que cumplen con el predicado que se indica.
 
 Si no se cumple el predicado opcionalmente se puede indicar una función que dado el valor y el contexto actual retorna el valor que se enviará al flujo.
 
+**Parámetros:**
+
 -  **predicate**: función(valor, contexto) que retorna un booleano
 
 -  **on_mismatch**: función(valor, contexto) que retorna un valor alternativo al testeado originalmente
 
 
 map(map_function)
 -----------------
 
 Permite modificar el valor de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y se substituirá en el mismo por lo obtenido de la función.
 
+**Parámetros:**
+
 -  **map_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
 map_if(predicate, map_function)
 -------------------------------
 Evalúa el predicado, si este es verdadero mapea el valor actual con la función de mapeo.
 
+**Parámetros:**
+
 - **predicate**: función(valor, contexto) predicado que se evalúa.
 
 - **map_function**: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
 
 
 map_context(map_context_function)
 ---------------------------------
 
 Permite modificar el contexto de un flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y retornará un nuevo contexto que sustituirá al actual
 
+**Parámetros:**
+
 -  **map_context_function**: función(valor, contexto) desde donde se obtendrá el contexto a subsituir.
 
 
 flat_map(flatmap_function)
 --------------------------
 
 Permite sustituir el valor de un flujo por elementos de otro flujo.
 
 Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo original y retornará un flujo cuyos elementos se usarán como nuevo origen del flujo de datos.
 
+**Parámetros:**
+
 -  **flatmap_function**: función(valor, contexto) desde donde se obtendrá el valor a sustituir.
 
 
 do_on_next(on_next)
 -------------------
 
 Ejecuta para cada elemento del flujo una acción de forma asincrónica.
 No afecta a los valores del flujo.
 
+**Parámetros:**
+
 -  **on_next**: función(valor, contexto) que se ejecutará para cada valor del flujo
 
 -  **on_error**: función(ex, contexto) se ejecuta en caso de error
 
 - **exec_async**: Booleano que indica si las funciones se ejecutarán de forma asíncrona
 
 
 delay_ms(delay_ms, predicate=fu.default_predicate)
 --------------------------------------------------
 
 Retrasa en delay milisegundos la ejecución de paso del flujo. Esto marca el tiempo en que se procesarán sus elementos.
 
+**Parámetros:**
+
 -  **delay_ms**: Delay en milisegundos que se retrasará el procesamiento de los elementos del flujo
 
 -  **predicate**: Si es verdadero se aplica el delay establecido
 
 
 parallel(pool_size=5, metric_function=None)
 -------------------------------------------
 Consume elementos de un flujo en paralelo.
 Utiliza tantos hilos como se haya configurado en pool_size.
 Si se indica, con cada elemento procesado invoca a la función metric_function pasándole un mapa con la siguiente
 información:
+
 - pool_size: Tamaño del pool
-used_pool: Cantidad de hilos utilizados
-avg_used_pool: Promedio de hilos utilizados
-avg_task_time: Promedio de tiempo de ejecución de la obtención de elementos en paralelo
-rate_s: Tasa de procesamiento
+
+- used_pool: Cantidad de hilos utilizados
+
+- avg_used_pool: Promedio de hilos utilizados
+
+- avg_task_time: Promedio de tiempo de ejecución de la obtención de elementos en paralelo
+
+- rate_s: Tasa de procesamiento
+
+**Parámetros:**
 
 - **pool_size**: Pool de hilos a utilizar
-- **metric_function**: función(metrics) Esta es una función que si se setea recibe con cada elemento procesado  un bloque de métricas sobre la ejecución paralela
 
+- **metric_function**: función(metrics, context) Esta es una función que si se setea recibe con cada elemento procesado un bloque de métricas sobre la ejecución paralela
 
 
-take(n)
--------
+take_if(n, predicate=None)
+--------------------------
 
-Corta la ejecución del flujo luego de procesar n elementos.
+Corta la ejecución del flujo luego de procesar n elementos que cumplen con la condición indicada.
+Si no se indica una función de predicado se cortará la ejecución al procesar n elementos.
 
+**Parámetros:**
 -  **n**: Cantidad de elementos procesados antes de cortar el flujo
-
+-  **predicate**: función(value, context) Si esta función retorna verdadero ese elemento es tomado en cuenta
 
 take_until_seconds(n)
 ---------------------
 
 Corta la ejecución del flujo luego de n segundos de procesamiento.
 
 La ejecución se cortará si al momento de evaluar este paso el tiempo transcurrido fue superior al configurado.
 
+**Parámetros:**
+
 -  **n**: Cantidad de segundos que el stream procesa elementos.
 
 chunks(n)
 ---------
 
 Emite un valor construido como una lista de como máximo n valores obtenidos del flujo padre.
 
 Si algún valor mientras se construye el chunk da error se emiten los elementos recolectados y luego se propaga el error.
 
+**Parámetros:**
+
 - ***n***: Cantidad de elementos recolectados antes de emitir el evento de lista.
 
 
 log(build_log_message, build_error_message, level)
 --------------------------------------------------
 
 Recibe una función(valor, contexto) que retorna un mensaje de texto que será logueado con el nivel de log indicado en level.
 
 El logueo se hace de forma asincrónica y no afecta al flujo.
 
+**Parámetros:**
+
 -  **build_log_message**: Función que dado un valor y contexto retorna un mensaje a loguear
 
 -  **build_error_message**: Función que dada una excepción y el contexto retorna el mensaje a loguear como ERROR
 
 -  **level**: Nivel de logueo que se usará
 
 
 on_error_resume(resume=fu.default_error_resume, exceptions=[Exception])
 -----------------------------------------------------------------------
 En caso de error, este paso ejecuta la función resume que debe retornar un valor a partir del error recibido por parámetro.
 
+**Parámetros:**
+
 -  **resume**: función(ex, contexto) Debe retornar el valor a sustituir en el flujo.
 
 -  **exceptions**: Lista de excepciones para los que se aplica la función resume.
 
 
 on_error_retry(retries=3, delay_ms=lambda i: 0, exceptions=[Exception])
 -----------------------------------------------------------------------
 
 En caso de error, este paso intenta ejecutar nuevamente el flujo **retries** cantidad de veces.
 
 Esto lo hace sólo para las excepciones indicadas por **exceptions** y los reintentos tienen un delay dado por la función **delay_ms** que recibe el número de reintento que es y espera obtener los ms de delay que se deben aplicar.
 
+**Parámetros:**
+
 -  **retries**: Cantidad de reintentos a aplicar
 
 -  **delay_ms**: función(int) que retorna dado el número de reintento en el que se está cuantos: ms de delay se deben aplicar.
 
 -  **exceptions**: Lista de excepciones para los que se aplica el método resume.
 
 
 subscribe(context, skip_error)
 ------------------------------
 
 Crea un objeto iterable a partir del flujo. Si se itera sobre este objeto se obtendrán los valores del flujo.
 
+**Parámetros:**
+
 -  **skip_error**: Ignora errores al obtener los valores desde el flujo
 
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Objeto iterable
 
 
 foreach(on_success=fu.default_success, on_error=fu.default_error, context={})
 -----------------------------------------------------------------------------
 
 Itera sobre los elementos del flujo e invoca a funciones **on_success** y on_error dependiendo el estado del flujo.
 
+**Parámetros:**
+
 -  **on_success**: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
 
 -  **on_error**: función(ex, valor, contexto) se invoca si hay un error en el flujo. Esto no corta el procesamiento a menos que se lance una excepción en el método
 
 -  **on_finish**: función(contexto) se invoca cuando el flujo finaliza
 
 -  **context**: Contexto inicial para el flujo
 
 
 to_list(context={}, skip_error=True)
 ------------------------------------
 
 Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
 
+**Parámetros:**
+
 -  **context**: contexto inicial para el flujo
 
 -  **skip_error**: Ignora errores al obtener los valores desde el flujo
 
 -  **return**: Lista de elementos
 
 
 collect(init=lambda c: {}, reduce=lambda v, a: a, context={})
 -------------------------------------------------------------
 
 Permite resumir en un sólo objeto el procesamiento de todos los elementos del flujo.
 
 Se inicializa un acumulador a través de la función init(contexto) y luego para cada elemento del flujo se invoca la función reduce(valor, acumulador) que procesa el valor y retorna un nuevo valor del acumulador.
 
+**Parámetros:**
+
 -  **init**: función(contexto) Retorna valor inicial del acumulador
 
 -  **reduce**: funcón(valor, acumulador) Dados el nuevo valor y el acumulador retorna un nuevo valor de acumulador.
 
 -  **context**: Contexto inicial para el flujo
 
 -  **return**: Acumulador
```

