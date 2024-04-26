# Comparing `tmp/ecuapassdocs-0.72.tar.gz` & `tmp/ecuapassdocs-0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecuapassdocs-0.72.tar", last modified: Sun Apr 21 20:13:51 2024, max compression
+gzip compressed data, was "ecuapassdocs-0.73.tar", last modified: Thu Apr 25 21:09:08 2024, max compression
```

## Comparing `ecuapassdocs-0.72.tar` & `ecuapassdocs-0.73.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.752394 ecuapassdocs-0.72/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-21 20:13:51.752394 ecuapassdocs-0.72/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)      335 2024-01-18 22:56:29.000000 ecuapassdocs-0.72/README.md
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.668391 ecuapassdocs-0.72/ecuapassdocs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.676391 ecuapassdocs-0.72/ecuapassdocs/info/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3203 2024-04-14 23:07:17.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_data.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    16144 2024-04-19 16:41:25.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_extractor.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     3852 2024-04-11 20:12:42.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_feedback.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     8759 2024-04-18 18:03:46.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    22728 2024-04-19 16:44:38.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2728 2024-04-12 15:44:03.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_declaracion.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    25562 2024-04-12 15:14:37.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1850 2024-04-12 15:43:23.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1709 2024-04-12 15:43:35.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     5488 2024-04-18 05:29:13.000000 ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/info/old-utils.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.72/ecuapassdocs/info/resourceloader.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.676391 ecuapassdocs-0.72/ecuapassdocs/resources/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.688391 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/documentos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/empresa.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/monedas.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/out.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/sustancias.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.688391 ecuapassdocs-0.72/ecuapassdocs/resources/data_declaracion/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_declaracion/__init__.py
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.696392 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/derivado.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/distritos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/meses.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/paises.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/sectores.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.724393 ecuapassdocs-0.72/ecuapassdocs/resources/docs/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    15528 2024-04-01 17:21:22.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/join.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
--rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
--rw-rw-r--   0 lg        (1000) lg        (1000)    18425 2024-03-30 18:30:32.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
--rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.72/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.752394 ecuapassdocs-0.72/ecuapassdocs/resources/images/
--rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/__init__.py
--rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-colombia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-ecuador.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-white-bot.ico
--rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-cartaporte-vacia.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
--rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-scroll-up.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
--rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
--rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
--rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.72/ecuapassdocs/resources/images/image-windows-WindowButtons.png
-drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-21 20:13:51.672391 ecuapassdocs-0.72/ecuapassdocs.egg-info/
--rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-21 20:13:51.000000 ecuapassdocs-0.72/ecuapassdocs.egg-info/PKG-INFO
--rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-04-21 20:13:51.000000 ecuapassdocs-0.72/ecuapassdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-04-21 20:13:51.000000 ecuapassdocs-0.72/ecuapassdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-04-21 20:13:51.000000 ecuapassdocs-0.72/ecuapassdocs.egg-info/requires.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-04-21 20:13:51.000000 ecuapassdocs-0.72/ecuapassdocs.egg-info/top_level.txt
--rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-04-21 20:13:51.752394 ecuapassdocs-0.72/setup.cfg
--rw-rw-r--   0 lg        (1000) lg        (1000)     1249 2024-04-21 20:13:49.000000 ecuapassdocs-0.72/setup.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.310192 ecuapassdocs-0.73/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-25 21:09:08.310192 ecuapassdocs-0.73/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)       40 2024-04-22 18:48:50.000000 ecuapassdocs-0.73/README.md
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.230190 ecuapassdocs-0.73/ecuapassdocs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.238191 ecuapassdocs-0.73/ecuapassdocs/info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3202 2024-04-25 03:25:15.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_data.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    16144 2024-04-19 16:41:25.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_extractor.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4546 2024-04-23 23:21:48.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_feedback.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     8726 2024-04-25 20:33:15.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    22728 2024-04-19 16:44:38.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     9140 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1481 2024-04-12 15:49:22.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2728 2024-04-12 15:44:03.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1729 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     4601 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_declaracion.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    25562 2024-04-12 15:14:37.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1330 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1850 2024-04-12 15:43:23.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1709 2024-04-12 15:43:35.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1654 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     5488 2024-04-18 05:29:13.000000 ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    12459 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/info/old-utils.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1463 2024-03-17 23:52:12.000000 ecuapassdocs-0.73/ecuapassdocs/info/resourceloader.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.238191 ecuapassdocs-0.73/ecuapassdocs/resources/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.246191 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-02-19 04:05:45.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-09-26 04:28:29.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      976 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      195 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/condiciones_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      108 2023-10-19 03:53:25.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_cebaf.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      369 2023-10-19 03:53:25.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_huaquillas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      109 2023-10-19 03:53:25.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_loja.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      293 2023-10-19 03:53:25.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_quito.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 20:00:30.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-09-26 04:28:51.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      100 2023-09-26 04:29:01.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/documentos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       76 2023-10-16 19:53:52.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/empresa.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-09-26 04:28:56.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/monedas.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      575 2023-11-07 19:28:46.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/out.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-09-26 04:29:13.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1971 2023-10-16 19:53:44.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/paises_todos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      124 2023-09-26 04:05:06.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      924 2023-09-26 04:28:24.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/sustancias.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.250191 ecuapassdocs-0.73/ecuapassdocs/resources/data_declaracion/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_declaracion/__init__.py
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.274191 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-01-10 20:24:00.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1818 2023-10-16 13:31:38.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      554 2023-10-16 13:31:38.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      280 2023-10-16 13:31:38.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      721 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      899 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     3686 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1630 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1569 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       44 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/condiciones_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       15 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/derivado.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      106 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/distritos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       79 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/empresas_transporte.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 19:53:29.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/meses.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       56 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/paises.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      127 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/procedimientos.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       70 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/sectores.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      105 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_carga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      103 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_documento.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)    14648 2023-11-19 21:59:18.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      532 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      104 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_moneda.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       42 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_sexo.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1422 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)      164 2023-10-16 13:31:39.000000 ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_vehiculo.txt
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.298192 ecuapassdocs-0.73/ecuapassdocs/resources/docs/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18165 2024-03-26 00:09:58.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:08:52.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   185152 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    15528 2024-04-01 17:21:22.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6076 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)   102275 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   184038 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10893 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   281667 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   339751 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   361834 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    96924 2024-03-26 01:01:53.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/join.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)    74532 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf
+-rw-rw-r--   0 lg        (1000) lg        (1000)   130529 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg
+-rw-rw-r--   0 lg        (1000) lg        (1000)    18425 2024-03-30 18:30:32.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto_input_parameters.json
+-rw-rw-r--   0 lg        (1000) lg        (1000)   346795 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    95521 2024-03-26 00:59:47.000000 ecuapassdocs-0.73/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.310192 ecuapassdocs-0.73/ecuapassdocs/resources/images/
+-rw-rw-r--   0 lg        (1000) lg        (1000)        0 2024-03-15 14:44:02.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/__init__.py
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2379 2023-11-16 17:04:17.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-colombia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     2164 2023-11-16 17:08:35.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-ecuador.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1449 2023-09-13 02:19:14.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-white-bot.ico
+-rw-rw-r--   0 lg        (1000) lg        (1000)   128273 2023-09-04 20:18:38.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    29117 2023-09-12 15:32:21.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-cartaporte-vacia.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    43614 2023-10-22 22:14:16.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-declaracion-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)   134943 2023-10-06 23:29:34.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)      297 2023-10-21 21:41:16.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-scroll-up.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)     1906 2023-08-13 18:09:07.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1727 2023-10-22 22:15:41.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1346 2023-10-21 20:53:42.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)    10993 2023-11-23 18:07:54.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1270 2023-11-23 18:09:48.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png
+-rw-rw-rw-   0 lg        (1000) lg        (1000)      418 2023-08-13 18:52:28.000000 ecuapassdocs-0.73/ecuapassdocs/resources/images/image-windows-WindowButtons.png
+drwxrwxr-x   0 lg        (1000) lg        (1000)        0 2024-04-25 21:09:08.230190 ecuapassdocs-0.73/ecuapassdocs.egg-info/
+-rw-rw-r--   0 lg        (1000) lg        (1000)      348 2024-04-25 21:09:08.000000 ecuapassdocs-0.73/ecuapassdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 lg        (1000) lg        (1000)     6030 2024-04-25 21:09:08.000000 ecuapassdocs-0.73/ecuapassdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)        1 2024-04-25 21:09:08.000000 ecuapassdocs-0.73/ecuapassdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       46 2024-04-25 21:09:08.000000 ecuapassdocs-0.73/ecuapassdocs.egg-info/requires.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       13 2024-04-25 21:09:08.000000 ecuapassdocs-0.73/ecuapassdocs.egg-info/top_level.txt
+-rw-rw-r--   0 lg        (1000) lg        (1000)       38 2024-04-25 21:09:08.314192 ecuapassdocs-0.73/setup.cfg
+-rw-rw-r--   0 lg        (1000) lg        (1000)     1296 2024-04-25 21:09:05.000000 ecuapassdocs-0.73/setup.py
```

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_data.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 class EcuData:
 	temporalDir = None
 
 	empresas = { 
 		"BYZA": {
 			'id'     : "BYZA",
 			"nombre" : "Grupo BYZA S.A.S.",
-			"direccion": "Av. Coral y los Álamos",
+			"direccion": "Av. Coral y los Alamos",
 			"idTipo" : "RUC", 
 			"idNumero" : "0400201414001",
 			"modelCartaportes": "Model_02_Cartaportes_NTA_BYZA",
 			"modelManifiestos": "Manifiestos_NTA_BYZA_Template",
 			#"modelManifiestos": "Model_Manifiestos_NTA_BYZA_4",
 			"modelDeclaraciones": None,
 			"MRN": None,
```

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_extractor.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_extractor.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_feedback.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_feedback.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 """
 
 import os
 from datetime import datetime
 
 from azure.storage.blob import BlobServiceClient, BlobClient, ContainerClient
 
+from .ecuapass_utils import Utils
+
 class EcuFeedback:
 	#----------------------------------------------------------------
 	#-- Get the blob client to write to Azure blob
 	#----------------------------------------------------------------
 	def getBlobClient (text_blob_name):
 		# Azure Blob Storage container name
 		container_name = "blobfeedback"
 
 		# Azure Storage account connection string
-		connection_string = "DefaultEndpointsProtocol=https;AccountName=lgformsstorage;AccountKey=BHsWkVaWQYStRq8FOpoIl0jI39W+WFvrSJmxesr0euIEJe+qkSi0LoTM0HZfyOn2XbYfnHir7CD8+ASt6ZJnwg==;EndpointSuffix=core.windows.net"
+		#connection_string = os.environ.get ("AZR_BLOB_CONN_STR")
+		connection_string ="DefaultEndpointsProtocol=https;AccountName=lgformsstorage;AccountKey=BHsWkVaWQYStRq8FOpoIl0jI39W+WFvrSJmxesr0euIEJe+qkSi0LoTM0HZfyOn2XbYfnHir7CD8+ASt6ZJnwg==;EndpointSuffix=core.windows.net"
+		Utils.printx ("Connection string:", connection_string)
 
 		# Initialize the BlobServiceClient
 		blob_service_client = BlobServiceClient.from_connection_string (connection_string)
 
 		# Create a container (if it doesn't exist)
 		container_client = blob_service_client.get_container_client (container_name)
 		blob_client = container_client.get_blob_client (text_blob_name)
@@ -33,48 +37,60 @@
 	#----------------------------------------------------------------
 	def sendLog (empresa, filename):
 		logMessage = f"LOG_{empresa}_{filename.split ('.')[0]}"
 		print ("Sending log: ", logMessage)
 		try:
 			blob_client    = EcuFeedback.getBlobClient (f"{logMessage}")
 			blob_client.upload_blob ("", overwrite=True)
-		except:
+		except: 
 			print (f"No se pudo enviar el log'")
 
 	#----------------------------------------------------------------
 	# Send a file to blob
 	#----------------------------------------------------------------
 	def sendFile (empresa, docFilepath):
 		# Upload PDF file as a blob
 		filename    = os.path.basename (docFilepath)
 		logFilename = f"LOG_{empresa}_{filename}"
 		print ("Sending log file: ", logFilename)
+		EcuFeedback.sendFileAsBytes (docFilepath, logFilename)
+#		if docFilepath != None and os.path.exists (docFilepath):
+#			pdf_blob_client = EcuFeedback.getBlobClient (logFilename)
+#			with open(docFilepath, "rb") as pdf_file:
+#				pdf_blob_client.upload_blob (pdf_file, overwrite=True)
+
+	def sendFileAsBytes (docFilepath, logFilename):
 		if docFilepath != None and os.path.exists (docFilepath):
 			pdf_blob_client = EcuFeedback.getBlobClient (logFilename)
 			with open(docFilepath, "rb") as pdf_file:
 				pdf_blob_client.upload_blob (pdf_file, overwrite=True)
 
 	#----------------------------------------------------------------
 	# Send message and file from GUI 
 	#----------------------------------------------------------------
 	def sendFeedback (zipFilepath, docFilepath):
 		try:
 			print ("Enviando retroalimentación: ", zipFilepath) 
 			# Upload text as a blob
-			feedbackText = EcuFeedback.getTextFromZipFile (zipFilepath)
-			fileSufix    = EcuFeedback.getCurrentDateTimeString ()
+			filename    = os.path.basename (docFilepath)
+			logFilename = f"LOG_{filename}"
+			EcuFeedback.sendFileAsBytes (zipFilepath, logFilename)
+
+			#feedbackText = EcuFeedback.getTextFromZipFile (zipFilepath)
+			#print ("--feedbackText: ", feedbackText)
+			#fileSufix    = EcuFeedback.getCurrentDateTimeString ()
 
-			blob_client  = EcuFeedback.getBlobClient (f"feedback-{fileSufix}.txt")
-			blob_client.upload_blob (feedbackText, overwrite=True)
+			#blob_client  = EcuFeedback.getBlobClient (f"feedback-{fileSufix}.txt")
+			#blob_client.upload_blob (feedbackText, overwrite=True)
 
-			EcuFeedback.sendPdfFile (docFilepath)	
+			#EcuFeedback.sendPdfFile (docFilepath)	
 
 			return (f"Retroalimentación en la nube: Documento {docFilepath}")
 		except:
-			print (f"No se pudo enviar retroalimentación")
+			Utils.printException (f"No se pudo enviar retroalimentación")
 
 		return None
 
 	#----------------------------------------------------------------
 	# Get the text as zip file from GUI
 	#----------------------------------------------------------------
 	def getTextFromZipFile (zip_file_path):
```

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 		self.docType        = docType
 		self.fieldsJsonFile = fieldsJsonFile
 		self.runningDir     = runningDir
 
 		self.empresa        = self.getEmpresaInfo ()   # Overwritten per 'empresa'
 		self.nombreEmpresa  = self.empresa ["id"]
 
-		print (f"-- docType: '{self.docType}'")
 		if self.docType == "CARTAPORTE":
 			self.inputsParametersFile = "cartaporte_input_parameters.json"
 		elif self.docType == "MANIFIESTO":
 			self.inputsParametersFile = "manifiesto_input_parameters.json"
 		elif self.docType == "DECLARACION":
 			self.inputsParametersFile = "declaracion_input_parameters.json"
 		else:
@@ -139,15 +138,15 @@
 	#-----------------------------------------------------------
 	def cleanWaterMark (self, text):
 		if self.empresa ['id'] == "NTA":
 			w1, w2, w3, w4 = "N\.T\.A\.", "CIA\.", "LTDA.", "N\.I\.A\."
 			expression = rf'(?:{w1}\s+{w2}\s+{w3}|{w2}\s+{w3}\s+{w1}|{w3}\s+{w1}\s+{w2}|{w4}\s+{w2}\s+{w3}|{w2}\s+{w3}\s+{w4}|{w3}\s+{w4}\s+{w2}|{w1}\s+{w2}\s+{w3}|{w2}\s+{w3}\s+{w1}|{w3}\s+{w1}\s+{w2}|{w4}\s+{w2}\s+{w3}|{w2}\s+{w3}\s+{w4}|{w3}\s+{w4}\s+{w2})'
 
 		elif self.empresa ['id'] == 'BYZA':
-			expression = r"By\s*za\s*soluciones\s*(que\s*)*facilitan\s*tu\s*vida"
+			expression = r"(Byza)|(By\s*za\s*soluciones\s*(que\s*)*facilitan\s*tu\s*vida)"
 		else:
 			return text
 
 		pattern = re.compile (expression)
 		text = re.sub (pattern, '', text)
 
 		return text.strip()
```

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_cartaporte_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_declaracion.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_declaracion.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_BOTERO.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_BYZA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_NTA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_info_manifiesto_SYTSA.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/ecuapass_utils.py` & `ecuapassdocs-0.73/ecuapassdocs/info/ecuapass_utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/old-utils.py` & `ecuapassdocs-0.73/ecuapassdocs/info/old-utils.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/info/resourceloader.py` & `ecuapassdocs-0.73/ecuapassdocs/info/resourceloader.py`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/condiciones_pago.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/depositos_tulcan.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/out.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/out.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/paises_todos.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/paises_todos.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/sustancias.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/sustancias.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_cartaportes/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/aduanas_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_bolivia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_colombia.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/ciudades_peru.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_embalaje.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_incoterm.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/data_manifiestos/tipos_unidadcarga.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-contrato-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte-vacia-SILOG-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/cartaporte_input_parameters.json` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/cartaporte_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/ciudades-paises-colombia-ecuador.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion-vacia-NTA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion-vacia-NTA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/declaracion_input_parameters.json` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/declaracion_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-declaracion-vacia-NTA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/image-manifiesto-vacio-NTA-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/join.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/join.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto-vacio-NTA-BYZA.svg`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/manifiesto_input_parameters.json` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/manifiesto_input_parameters.json`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/old-image-cartaporte-vacia-SILOG-BYZA.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf` & `ecuapassdocs-0.73/ecuapassdocs/resources/docs/org-cartaporte-vacia-SILOG-BYZA.pdf`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-colombia.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-colombia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-ecuador.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-ecuador.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/icon-white-bot.ico` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/icon-white-bot.ico`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-cartaporte-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-cartaporte-vacia.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-cartaporte-vacia.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-declaracion-ecuapass.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-declaracion-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-manifiesto-ecuapass.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-CartaporteCarretera.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-DeclaracionTransito.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-ManifiestoTerrestre.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto-full.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png` & `ecuapassdocs-0.73/ecuapassdocs/resources/images/image-text-blue-TERRESTRE-manifiesto.png`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/ecuapassdocs.egg-info/SOURCES.txt` & `ecuapassdocs-0.73/ecuapassdocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecuapassdocs-0.72/setup.py` & `ecuapassdocs-0.73/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ecuapassdocs',  # Package name
-    version='0.72',  # Package version
+    version='0.73',  # Package version
     url="https://github.com/lgarreta/ecuapassdocs",
     author='Luis Garreta',
     author_email='lgarreta@gmail.com',
     description='Utils for creating PDFs, loading resources and extracting info from fields in ECUAPASS docs: cartaportes, manifiestos, declaraciones',
     packages=find_packages(),  # Automatically finds packages within the directory
 	include_package_data=True, 
 	package_data={"ecuapassdocs": ["resources/images/*", 
@@ -17,14 +17,15 @@
 	# List any dependencies here
     install_requires = [
 		"PyPDF2==3.0.1",
 		"reportlab==4.0.8",
 		"Pillow==10.1.0"
 	], 
 	logs = {
+		"0.73" : "Improved Byza's clean watermarks",
 		"0.72" : "Improved infos: embalaje",
 		"0.71" : "Improved assignation of vehicle type in Manifiestos",
 		"0.70" : "Added creation of ECUAPASSDOCS fields. Added numero to parameters",
 		"0.63" : "Added creation of CODEBIN fields",
 		"0.60" : "Changed resource names from 'data-XXX' to data_XXX'"
 		},
 )
```

