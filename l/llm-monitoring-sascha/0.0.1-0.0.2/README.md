# Comparing `tmp/llm_monitoring_sascha-0.0.1.tar.gz` & `tmp/llm_monitoring_sascha-0.0.2.tar.gz`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4049 bytes, number of entries: 7
+Zip file size: 4046 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     2113 b- defN 24-Apr-25 14:07 monitoring/__init__.py
 -rw-r--r--  2.0 unx     4629 b- defN 24-Apr-26 07:28 monitoring/client.py
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-26 08:10 llm_monitoring_sascha-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      549 b- defN 24-Apr-26 08:10 llm_monitoring_sascha-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 08:10 llm_monitoring_sascha-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-26 08:10 llm_monitoring_sascha-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      608 b- defN 24-Apr-26 08:10 llm_monitoring_sascha-0.0.1.dist-info/RECORD
-7 files, 8010 bytes uncompressed, 2953 bytes compressed:  63.1%
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-26 08:11 llm_monitoring_sascha-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      549 b- defN 24-Apr-26 08:11 llm_monitoring_sascha-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 08:11 llm_monitoring_sascha-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-26 08:11 llm_monitoring_sascha-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      608 b- defN 24-Apr-26 08:11 llm_monitoring_sascha-0.0.2.dist-info/RECORD
+7 files, 8010 bytes uncompressed, 2950 bytes compressed:  63.2%
```

## zipnote «TEMP»/diffoscope_h4ltvoak_/tmpnaold0qn_.zip

```diff
@@ -1,22 +1,22 @@
 Filename: monitoring/__init__.py
 Comment: 
 
 Filename: monitoring/client.py
 Comment: 
 
-Filename: llm_monitoring_sascha-0.0.1.dist-info/LICENSE
+Filename: llm_monitoring_sascha-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: llm_monitoring_sascha-0.0.1.dist-info/METADATA
+Filename: llm_monitoring_sascha-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: llm_monitoring_sascha-0.0.1.dist-info/WHEEL
+Filename: llm_monitoring_sascha-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: llm_monitoring_sascha-0.0.1.dist-info/top_level.txt
+Filename: llm_monitoring_sascha-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: llm_monitoring_sascha-0.0.1.dist-info/RECORD
+Filename: llm_monitoring_sascha-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `llm_monitoring_sascha-0.0.1.dist-info/METADATA` & `llm_monitoring_sascha-0.0.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm_monitoring_sascha
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Sascha Heyer <mail@saschaheyer.de>, Sascha Heyer <sascha@doit.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `llm_monitoring_sascha-0.0.1.dist-info/RECORD` & `llm_monitoring_sascha-0.0.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 monitoring/__init__.py,sha256=mtuV3IBnBa0qVuolb8AwlIc3FcwOWP1eWUHGL6kkw5s,2113
 monitoring/client.py,sha256=Vmo3J44mnbI0B3tyk4Ej4uLBNSum7sxp2xkulmgQHOU,4629
-llm_monitoring_sascha-0.0.1.dist-info/LICENSE,sha256=P8LbZeJRLLSAfoDFsIwTh1b7J-mtfv_IzBcu9fO7WDo,8
-llm_monitoring_sascha-0.0.1.dist-info/METADATA,sha256=1dMLdKXa4JBWzj4IlF1OuoNC4dElir_jBXm3EjLY60s,549
-llm_monitoring_sascha-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-llm_monitoring_sascha-0.0.1.dist-info/top_level.txt,sha256=QGBmMzom9uTYMO5A1ffaCw3pFZGGuDe6dpZ2Y-VZoQc,11
-llm_monitoring_sascha-0.0.1.dist-info/RECORD,,
+llm_monitoring_sascha-0.0.2.dist-info/LICENSE,sha256=P8LbZeJRLLSAfoDFsIwTh1b7J-mtfv_IzBcu9fO7WDo,8
+llm_monitoring_sascha-0.0.2.dist-info/METADATA,sha256=OOjVi4DvjtA9RMq3_pBpzHSYUBDQzGe3-M5f_dt1Iv4,549
+llm_monitoring_sascha-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+llm_monitoring_sascha-0.0.2.dist-info/top_level.txt,sha256=QGBmMzom9uTYMO5A1ffaCw3pFZGGuDe6dpZ2Y-VZoQc,11
+llm_monitoring_sascha-0.0.2.dist-info/RECORD,,
```

