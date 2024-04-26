# Comparing `tmp/brickbundles-0.7.3-py3-none-any.whl.zip` & `tmp/brickbundles-0.7.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 111922 bytes, number of entries: 281
+Zip file size: 111923 bytes, number of entries: 281
 -rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Actuator.brick
 -rw-r--r--  2.0 unx     1363 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/CombustionEngine.brick
 -rw-r--r--  2.0 unx      742 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Differential.brick
 -rw-r--r--  2.0 unx     3717 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/EmpiricalTorqueConverter.brick
 -rw-r--r--  2.0 unx      133 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/Gear.brick
 -rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/HingeActuator.brick
 -rw-r--r--  2.0 unx      246 b- defN 80-Jan-01 00:00 brickbundles/DriveTrain/PrismaticActuator.brick
@@ -273,11 +273,11 @@
 -rw-r--r--  2.0 unx      234 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick
 -rw-r--r--  2.0 unx       90 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Geometry.brick
 -rw-r--r--  2.0 unx       39 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/Sphere.brick
 -rw-r--r--  2.0 unx       96 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Geometries/TriMeshGeometry.brick
 -rw-r--r--  2.0 unx       10 b- defN 80-Jan-01 00:00 brickbundles/Visuals/Materials/Material.brick
 -rw-r--r--  2.0 unx       72 b- defN 80-Jan-01 00:00 brickbundles/Visuals/config.brick
 -rw-r--r--  2.0 unx     1346 b- defN 80-Jan-01 00:00 brickbundles/__init__.py
--rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.7.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.7.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx    31267 b- defN 16-Jan-01 00:00 brickbundles-0.7.3.dist-info/RECORD
-281 files, 135268 bytes uncompressed, 59296 bytes compressed:  56.2%
+-rw-r--r--  2.0 unx     1066 b- defN 80-Jan-01 00:00 brickbundles-0.7.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 brickbundles-0.7.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx    31267 b- defN 16-Jan-01 00:00 brickbundles-0.7.4.dist-info/RECORD
+281 files, 135268 bytes uncompressed, 59297 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -828,17 +828,17 @@
 
 Filename: brickbundles/Visuals/config.brick
 Comment: 
 
 Filename: brickbundles/__init__.py
 Comment: 
 
-Filename: brickbundles-0.7.3.dist-info/METADATA
+Filename: brickbundles-0.7.4.dist-info/METADATA
 Comment: 
 
-Filename: brickbundles-0.7.3.dist-info/WHEEL
+Filename: brickbundles-0.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: brickbundles-0.7.3.dist-info/RECORD
+Filename: brickbundles-0.7.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `brickbundles-0.7.3.dist-info/METADATA` & `brickbundles-0.7.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BrickBundles
-Version: 0.7.3
+Version: 0.7.4
 Summary: Brick Bundles package, i.e. all Brick sourcefiles and convenience access method in a package
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `brickbundles-0.7.3.dist-info/RECORD` & `brickbundles-0.7.4.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -272,10 +272,10 @@
 brickbundles/Visuals/Geometries/ExternalTriMeshGeometry.brick,sha256=0cEEaVuE72vhJvAv6J1guVo6yZVOCf7Q4gFP9KvElGQ,234
 brickbundles/Visuals/Geometries/Geometry.brick,sha256=-tiwTgsHtKnrPvaPO6kj5LG_gfF0csLAxdJUXJJzywg,90
 brickbundles/Visuals/Geometries/Sphere.brick,sha256=K3DerE_AE6EnHc_2GmT1e9sYrCMUosmUlTXIcqYapBg,39
 brickbundles/Visuals/Geometries/TriMeshGeometry.brick,sha256=qctdVQYflyKPuuX6HK8QvTgRbKNYlI5JAB82UNmKTZs,96
 brickbundles/Visuals/Materials/Material.brick,sha256=hVvFGaQhcFJblZ1R0SLDhWjIY6lSKC84i9hBwmA3sq8,10
 brickbundles/Visuals/config.brick,sha256=Z7y-m-8BN9N4V0OvqKp8BKivcspo8_-IpA2xA5xvf80,72
 brickbundles/__init__.py,sha256=VC7H2Q-oD1kqfe06eBZdgPlW8tC1kzBRQXWHkOIYk24,1346
-brickbundles-0.7.3.dist-info/METADATA,sha256=kJh2k2Icl2o5ZhqC8a8Luz0aha5TFlUnwNit4u9YhKw,1066
-brickbundles-0.7.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-brickbundles-0.7.3.dist-info/RECORD,,
+brickbundles-0.7.4.dist-info/METADATA,sha256=NZLZqspM1aKkhs8_AHzONUMgkfZAek-ZmE0r49oOcdY,1066
+brickbundles-0.7.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+brickbundles-0.7.4.dist-info/RECORD,,
```

