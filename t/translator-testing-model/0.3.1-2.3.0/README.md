# Comparing `tmp/translator_testing_model-0.3.1.tar.gz` & `tmp/translator_testing_model-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_testing_model-0.3.1.tar", max compression
+gzip compressed data, was "translator_testing_model-2.3.0.tar", max compression
```

## Comparing `translator_testing_model-0.3.1.tar` & `translator_testing_model-2.3.0.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0     1080 2024-04-26 00:45:08.508252 translator_testing_model-0.3.1/LICENSE
--rw-r--r--   0        0        0     2135 2024-04-26 00:45:08.508252 translator_testing_model-0.3.1/README.md
--rw-r--r--   0        0        0    18763 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/excel/translator_testing_model.xlsx
--rw-r--r--   0        0        0     7159 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/graphql/translator_testing_model.graphql
--rw-r--r--   0        0        0    11318 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/jsonld/translator_testing_model.context.jsonld
--rw-r--r--   0        0        0    99618 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/jsonld/translator_testing_model.jsonld
--rw-r--r--   0        0        0    74600 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/jsonschema/translator_testing_model.schema.json
--rw-r--r--   0        0        0    84288 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/owl/translator_testing_model.owl.ttl
--rw-r--r--   0        0        0      277 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/prefixmap/translator_testing_model.yaml
--rw-r--r--   0        0        0     9632 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/protobuf/translator_testing_model.proto
--rw-r--r--   0        0        0    60704 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/shacl/translator_testing_model.shacl.ttl
--rw-r--r--   0        0        0    15590 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/shex/translator_testing_model.shex
--rw-r--r--   0        0        0    50812 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/project/sqlschema/translator_testing_model.sql
--rw-r--r--   0        0        0     1010 2024-04-26 00:45:21.596446 translator_testing_model-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      709 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/src/data/examples/Bad-AcceptanceTestAsset-001.yaml
--rw-r--r--   0        0        0      496 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/src/data/examples/Bad-AcceptanceTestCase-001.yaml
--rw-r--r--   0        0        0      337 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/src/data/examples/Bad-TestAsset-001.yaml
--rw-r--r--   0        0        0      508 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/src/data/examples/Bad-TestCaseSpecification-001.yaml
--rw-r--r--   0        0        0      873 2024-04-26 00:45:08.512252 translator_testing_model-0.3.1/src/data/examples/Bad-TestEntity-001.yaml
--rw-r--r--   0        0        0      860 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not
--rw-r--r--   0        0        0      554 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Bad-TestMetadata-001.yaml
--rw-r--r--   0        0        0      636 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Bad-TestSuite-001.yaml
--rw-r--r--   0        0        0      964 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-AcceptanceTestAsset-001.yaml
--rw-r--r--   0        0        0      829 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-AcceptanceTestCase-001.yaml
--rw-r--r--   0        0        0      363 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestAsset-001.json
--rw-r--r--   0        0        0     1627 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestAsset-001.yaml
--rw-r--r--   0        0        0      585 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestCase-001.json
--rw-r--r--   0        0        0     1786 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestCase-001.yaml
--rw-r--r--   0        0        0      529 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestCaseSpecification-001.yaml
--rw-r--r--   0        0        0      826 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestEntity-Complete.yaml
--rw-r--r--   0        0        0      144 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestEntity-Missing_Description_OK.yaml
--rw-r--r--   0        0        0      133 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestEntity-Missing_Name_OK.yaml
--rw-r--r--   0        0        0      506 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestMetadata-001.yaml
--rw-r--r--   0        0        0      637 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/Good-TestSuite-001.yaml
--rw-r--r--   0        0        0      828 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/data/examples/SampleTestAssetList.json
--rw-r--r--   0        0        0      243 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/translator_testing_model/README.md
--rw-r--r--   0        0        0     3313 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/translator_testing_model/adaptor/test_case_generator.py
--rw-r--r--   0        0        0     2299 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/translator_testing_model/adaptor/testrunner.py
--rw-r--r--   0        0        0      220 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/translator_testing_model/datamodel/README.md
--rw-r--r--   0        0        0    43778 2024-04-26 00:45:08.516252 translator_testing_model-0.3.1/src/translator_testing_model/datamodel/pydanticmodel.py
--rw-r--r--   0        0        0    70308 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/datamodel/translator_testing_model.py
--rw-r--r--   0        0        0      124 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/schema/README.md
--rw-r--r--   0        0        0    29634 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/schema/translator_testing_model.yaml
--rw-r--r--   0        0        0     3038 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/scripts/GitHub_issue_parser.py
--rw-r--r--   0        0        0    15228 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/scripts/generate_suite_for_demo.py
--rw-r--r--   0        0        0     3536 2024-04-26 00:45:08.520252 translator_testing_model-0.3.1/src/translator_testing_model/scripts/test_suite_generator.py
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 translator_testing_model-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-03-18 19:40:32.656137 translator_testing_model-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2191 2024-03-18 19:40:32.656137 translator_testing_model-2.3.0/README.md
+-rw-r--r--   0        0        0    21223 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/excel/translator_testing_model.xlsx
+-rw-r--r--   0        0        0     8135 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/graphql/translator_testing_model.graphql
+-rw-r--r--   0        0        0     6223 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonld/translator_testing_model.context.jsonld
+-rw-r--r--   0        0        0    99507 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonld/translator_testing_model.jsonld
+-rw-r--r--   0        0        0    79264 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/jsonschema/translator_testing_model.schema.json
+-rw-r--r--   0        0        0    81158 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/owl/translator_testing_model.owl.ttl
+-rw-r--r--   0        0        0      228 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/prefixmap/translator_testing_model.yaml
+-rw-r--r--   0        0        0    10811 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/protobuf/translator_testing_model.proto
+-rw-r--r--   0        0        0    68537 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/shacl/translator_testing_model.shacl.ttl
+-rw-r--r--   0        0        0     9703 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/shex/translator_testing_model.shex
+-rw-r--r--   0        0        0    14640 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/project/sqlschema/translator_testing_model.sql
+-rw-r--r--   0        0        0      992 2024-03-18 19:40:56.772001 translator_testing_model-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      709 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml
+-rw-r--r--   0        0        0      496 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestCase-001.yaml
+-rw-r--r--   0        0        0      332 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-001.yaml
+-rw-r--r--   0        0        0      390 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-002.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-003.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-004.yaml
+-rw-r--r--   0        0        0      391 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-005.yaml
+-rw-r--r--   0        0        0      399 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestAsset-006.yaml
+-rw-r--r--   0        0        0     1405 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestCase-001.yaml
+-rw-r--r--   0        0        0      508 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestCaseSpecification-001.yaml
+-rw-r--r--   0        0        0      829 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-001.yaml
+-rw-r--r--   0        0        0      816 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not
+-rw-r--r--   0        0        0      554 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestMetadata-001.yaml
+-rw-r--r--   0        0        0      636 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Bad-TestSuite-001.yaml
+-rw-r--r--   0        0        0      959 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml
+-rw-r--r--   0        0        0      829 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml
+-rw-r--r--   0        0        0      358 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.json
+-rw-r--r--   0        0        0     1642 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.yaml
+-rw-r--r--   0        0        0      585 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.json
+-rw-r--r--   0        0        0     1786 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.yaml
+-rw-r--r--   0        0        0      529 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml
+-rw-r--r--   0        0        0      782 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Complete.yaml
+-rw-r--r--   0        0        0      144 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Missing_Description_OK.yaml
+-rw-r--r--   0        0        0      133 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Missing_Name_OK.yaml
+-rw-r--r--   0        0        0      506 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestMetadata-001.yaml
+-rw-r--r--   0        0        0      637 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/Good-TestSuite-001.yaml
+-rw-r--r--   0        0        0      828 2024-03-18 19:40:32.660137 translator_testing_model-2.3.0/src/data/examples/SampleTestAssetList.json
+-rw-r--r--   0        0        0      243 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/README.md
+-rw-r--r--   0        0        0     3313 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/adaptor/test_case_generator.py
+-rw-r--r--   0        0        0     2299 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/adaptor/testrunner.py
+-rw-r--r--   0        0        0      270 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/README.md
+-rw-r--r--   0        0        0    47412 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel.py
+-rw-r--r--   0        0        0    47105 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py
+-rw-r--r--   0        0        0    70932 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/datamodel/translator_testing_model.py
+-rw-r--r--   0        0        0      124 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/schema/README.md
+-rw-r--r--   0        0        0    27461 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/schema/translator_testing_model.yaml
+-rw-r--r--   0        0        0     3038 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py
+-rw-r--r--   0        0        0    12807 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py
+-rw-r--r--   0        0        0     3536 2024-03-18 19:40:32.664137 translator_testing_model-2.3.0/src/translator_testing_model/scripts/test_suite_generator.py
+-rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 translator_testing_model-2.3.0/PKG-INFO
```

### Comparing `translator_testing_model-0.3.1/LICENSE` & `translator_testing_model-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/README.md` & `translator_testing_model-2.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 * [project/](project/) - project files (do not edit these)
 * [src/](src/translator_testing_model/README.md) - source files (edit these)
   * [translator testing model specification](src/translator_testing_model/README.md)
     * [schema](src/translator_testing_model/schema/translator_testing_model.yaml) -- LinkML schema
       (edit this)
     * [datamodel](src/translator_testing_model/datamodel/README.md) -- generated
       Python datamodels
-      * [Pydantic](src/translator_testing_model/datamodel/pydanticmodel.py) - this is a version 2 model.
+      * [Pydantic V1](src/translator_testing_model/datamodel/pydanticmodel.py)
+      * [Pydantic V2](src/translator_testing_model/datamodel/pydanticmodel_v2.py)
       * [Python Dataclasses](src/translator_testing_model/datamodel/translator_testing_model.py)
 * [tests/](tests/test_data.py) - Python tests
 
 ## Developer Documentation
 
 <details>
 The project uses [Poetry](https://python-poetry.org/) to manage its dependencies. Install Poetry then:
```

### Comparing `translator_testing_model-0.3.1/project/excel/translator_testing_model.xlsx` & `translator_testing_model-2.3.0/project/excel/translator_testing_model.xlsx`

 * *Files 23% similar despite different names*

```diff
@@ -1,1173 +1,1327 @@
-00000000: 504b 0304 1400 0000 0800 d585 9958 465a  PK...........XFZ
+00000000: 504b 0304 1400 0000 0800 5263 7258 465a  PK........RcrXFZ
 00000010: c10c 8200 0000 b100 0000 1000 0000 646f  ..............do
 00000020: 6350 726f 7073 2f61 7070 2e78 6d6c 4d8e  cProps/app.xmlM.
 00000030: 4d0b c230 1044 ff4a e9dd 6e55 f020 3120  M..0.D.J..nU. 1 
 00000040: d4a3 e0c9 7b48 3736 9064 4376 85fc 7c53  ....{H76.dCv..|S
 00000050: c18f db3c de30 8cba 15ca 58c4 2377 3586  ...<.0....X.#w5.
 00000060: c4a7 7e11 c947 00b6 0b46 c343 d3a9 1947  ..~..G...F.C...G
 00000070: 251a 6958 1e40 ce79 8b13 d967 c424 b01b  %.iX.@.y...g.$..
 00000080: c703 6015 4c33 ce9b fc1d ecb5 3ae7 1cbc  ..`.L3......:...
 00000090: 35e2 29e9 abb7 8598 9c74 976a 3128 f897  5.)......t.j1(..
 000000a0: 6bf3 8e85 d7bc 1fb6 6ff9 6105 bf93 fa05  k.......o.a.....
-000000b0: 504b 0304 1400 0000 0800 d585 9958 eb1e  PK...........X..
-000000c0: 5f40 ee00 0000 cb01 0000 1100 0000 646f  _@............do
+000000b0: 504b 0304 1400 0000 0800 5263 7258 6a72  PK........RcrXjr
+000000c0: 2c18 ed00 0000 cb01 0000 1100 0000 646f  ,.............do
 000000d0: 6350 726f 7073 2f63 6f72 652e 786d 6c95  cProps/core.xml.
-000000e0: 91c1 4ec3 300c 865f 65ca bd75 9b96 0945  ..N.0.._e..u...E
-000000f0: 592f 204e 2021 3109 c42d 4abc ada2 49a3  Y/ N !1..-J...I.
-00000100: c4a8 dddb 9396 ad1b 820b c7f8 fffc d956  ...............V
-00000110: a4f6 42f7 019f 43ef 3150 8b71 35da ce45  ..B...C.1P.q5..E
-00000120: a1fd 861d 88bc 0088 fa80 56c5 3c11 2e85  ..........V.<...
-00000130: bb3e 5845 e919 f6e0 95fe 507b 045e 146b  .>XE......P{.^.k
-00000140: b048 ca28 5230 0933 bf18 d949 69f4 a2f4  .H.(R0.3...Ii...
-00000150: 9fa1 9b05 4603 7668 d151 8432 2fe1 c212  ....F.vh.Q.2/...
-00000160: 061b ff6c 9893 851c 63bb 50c3 30e4 4335  ...l....c.P.0.C5
-00000170: 7369 a312 de9e 1e5f e6e5 b3d6 4552 4e23  si....._....ERN#
-00000180: 6ba4 d142 0754 d487 66ba c81f c74e c255  k..B.T..f....N.U
-00000190: 519e 667f 17d0 acd2 0441 478f 1b76 4e5e  Q.f......AG..vN^
-000001a0: abbb fbed 036b 78c1 ebac a833 7eb3 e595  .....kx....3~...
-000001b0: a8d7 a2ba 7d9f 5c3f fa2f 42db 9b76 d7fe  ....}.\?./B..v..
-000001c0: cf58 5757 c6b3 a091 f0eb df9a 2f50 4b03  .XWW......../PK.
-000001d0: 0414 0000 0008 00d5 8599 5899 5c9c 2310  ..........X.\.#.
-000001e0: 0600 009c 2700 0013 0000 0078 6c2f 7468  ....'......xl/th
-000001f0: 656d 652f 7468 656d 6531 2e78 6d6c ed5a  eme/theme1.xml.Z
-00000200: 5b73 da38 147e efaf d078 67f6 6d0b c636  [s.8.~...xg.m..6
-00000210: 81b6 b413 7369 76db b499 84ed 4e1f 8511  ....siv.....N...
-00000220: 588d 6c79 6491 847f bf47 3610 cb96 0ded  X.lyd....G6.....
-00000230: 924d ba9b 3c04 2ce9 fbce 4547 e7e8 3879  .M..<.,...EG..8y
-00000240: f3ee 2e62 e886 8894 f278 60d9 2fdb d6bb  ...b.....x`./...
-00000250: b72f dee0 5732 2411 4130 19a7 aff0 c00a  ./..W2$.A0......
-00000260: a54c 5eb5 5a69 00c3 387d c913 12c3 dc82  .L^.Zi..8}......
-00000270: 8b08 4b78 14cb d65c e05b 1a2f 23d6 eab4  ..Kx...\.[./#...
-00000280: dbdd 5684 696c a118 4764 607d 5e2c 6840  ..V.il..Gd`}^,h@
-00000290: d054 515a 6f5f 20b4 e51f 33f8 15cb 548d  .TQZo_ ...3...T.
-000002a0: 65a3 0113 5741 26b9 88b4 f2f9 6cc5 fcda  e...WA&.....l...
-000002b0: de3e 65cf e93a 1d32 816e 301b 5820 7fce  .>e..:.2.n0.X ..
-000002c0: 6fa7 e44e 5a88 e154 c2c4 c06a 673f 566b  o..NZ..T...jg?Vk
-000002d0: c7d1 d248 8082 c97d 9405 ba49 f6a3 d315  ...H...}...I....
-000002e0: 0832 0d3b 3a9d 58ce 767c f6c4 ed9f 8cca  .2.;:.X.v|......
-000002f0: da74 346d 1ae0 e3f1 7838 b6cb d28b 701c  .t4m....x8....p.
-00000300: 04e0 51bb 9ec2 9df4 6cbf a441 09b4 a369  ..Q.....l..A...i
-00000310: d064 d8f6 daae 91a6 aa8d 534f d3f7 7ddf  .d........SO..}.
-00000320: eb9b 689c 0a8d 5b4f d36b 77dd d38e 89c6  ..h...[O.kw.....
-00000330: add0 780d bef1 4f87 c3ae 89c6 abd0 74eb  ..x...O.......t.
-00000340: 6926 27fd ae6b a4e9 1668 4246 e3eb 7a12  i&'..k...hBF..z.
-00000350: 15b5 e540 d320 0058 7076 d6cc d203 965e  ...@. .Xpv.....^
-00000360: 29fa 7594 1ad9 1dbb dd41 5cf0 58ee 3989  ).u......A\.X.9.
-00000370: 11fe c6c5 04d6 69d2 1996 3446 729d 9005  ......i...4Fr...
-00000380: 0e00 37c4 d14c 507c af41 b68a e0c2 92d2  ..7..LP|.A......
-00000390: 5c90 d6cf 29b5 501a 089a c881 f547 8221  \...).P......G.!
-000003a0: c5dc affd f597 bbc9 a433 7a9d 7d3a ce6b  .........3z.}:.k
-000003b0: 947f 69ab 01a7 edbb 9bcf 93fc 73e8 e49f  ..i.........s...
-000003c0: a793 d74d 42ce 70bc 2c09 f1fb 235b 6187  ...MB.p.,...#[a.
-000003d0: 276e 3b13 723a 1c67 427c cff6 f691 a525  'n;.r:.gB|.....%
-000003e0: 32cf eff9 0aeb 4e3c 671f 5696 b05d cfcf  2.....N<g.V..]..
-000003f0: e49e 8c72 23bb ddf6 587d f64f 476e 23d7  ...r#...X}.OGn#.
-00000400: a9c0 b322 d794 4624 459f c82d bae4 1138  ..."..F$E..-...8
-00000410: b549 0d32 133f 089d 8698 6a50 1c02 a409  .I.2.?....jP....
-00000420: 3196 a186 f8b4 c6ac 11e0 137d b7be 08c8  1..........}....
-00000430: df8d 88f7 ab6f 9a3d 57a1 5849 da84 f810  .....o.=W.XI....
-00000440: 461a e29c 73e6 73d1 6cfb 07a5 46d1 f655  F...s.s.l...F..U
-00000450: bcdc a397 5815 0197 18df 34aa 352c c5d6  ....X.....4.5,..
-00000460: 7895 c0f1 ad9c 3c1d 1312 cd94 0b06 4186  x.....<.......A.
-00000470: 9724 2612 a939 7e4d 4813 fe2b a5da fe9c  .$&..9~MH..+....
-00000480: d340 f094 2f24 fa4a 918f 69b3 23a7 7426  .@../$.J..i.#.t&
-00000490: cde8 331a c146 af1b 7587 68d2 3c7a fe05  ..3..F..u.h.<z..
-000004a0: f99c 350a 1c91 1b1d 0267 1bb3 4621 8469  ..5......g..F!.i
-000004b0: bbf0 1eaf 248e 9aad c211 2b42 3e62 1936  ....$.....+B>b.6
-000004c0: 1a72 b516 81b6 71a9 8460 5a12 c6d1 784e  .r....q..`Z...xN
-000004d0: d2b4 11fc 59ac 3593 3e60 c8ec cd91 75ce  ....Y.5.>`....u.
-000004e0: d691 0e11 925e 3742 3e62 ce8b 9011 bf1e  .....^7B>b......
-000004f0: 8638 4a9a eda2 7158 04fd 9e5e c349 c1e8  .8J...qX...^.I..
-00000500: 82cb 66fd b87e 86d5 336c 2c8e f747 d417  ..f..~..3l,..G..
-00000510: 4ae4 0f26 a73f e932 3407 a39a 5909 bd84  J..&.?.24...Y...
-00000520: 566a 9faa 8734 3ea8 1e32 0a05 f1b9 1e3e  Vj...4>..2.....>
-00000530: e57a 780a 3796 c6bc 50ae 827b 01ff d1da  .zx.7...P..{....
-00000540: 37c2 abf8 82c0 397f 2e7d cfa5 efb9 f43d  7.....9..}.....=
-00000550: a1d2 b737 237d 67c1 d38b 5bde 466e 5bc4  ...7#}g...[.Fn[.
-00000560: fbae 31da d734 2e28 6357 72cd c8c7 54af  ..1..4.(cWr...T.
-00000570: 9329 d839 9fc0 ecfd 683e 9ef1 edfa d924  .).9....h>.....$
-00000580: 84af 9a59 2d23 1690 4b81 b341 24b8 fc8b  ...Y-#..K..A$...
-00000590: caf0 2ac4 09e8 645b 2509 cb54 d365 378a  ..*...d[%..T.e7.
-000005a0: 129e 421b 6ee9 53f5 4a95 d7e5 afb9 28b8  ..B.n.S.J.....(.
-000005b0: 3c5b e4e9 afa1 743e 2ccf f93c 5fe7 b4cd  <[....t>,..<_...
-000005c0: 0b33 43b7 724b eab6 94be b526 384a f4b1  .3C.rK.....&8J..
-000005d0: cc70 4e1e cb0c 3b67 3c92 1db6 77a0 1d35  .pN...;g<...w..5
-000005e0: fbf6 5d76 e423 a530 5397 43b8 1a42 be03  ..]v.#.0S.C..B..
-000005f0: 6dba 9ddc 3a38 9e98 91b9 0ad3 5290 6fc3  m...:8......R.o.
-00000600: f9e9 c578 1ae2 39d9 04b9 7d98 576d e7d8  ...x..9...}.Wm..
-00000610: d1d1 fbe7 c151 b0a3 ef3c 961d c788 f2a2  .....Q...<......
-00000620: 21ee a186 98cf c343 8779 7b5f 9867 95c6  !......C.y{_.g..
-00000630: 5034 146d 6cac 242c 46b7 60b8 d7f1 2c14  P4.ml.$,F.`...,.
-00000640: e064 602d a007 83af 5102 f252 5560 315b  .d`-....Q..RU`1[
-00000650: c603 2b90 a27c 4c8c 45e8 70e7 975c 5fe3  ..+..|L.E.p..\_.
-00000660: d192 e3db a665 b56e af29 7719 6d22 5239  .....e.n.)w.m"R9
-00000670: c269 9813 67ab cade 65b1 c155 1dcf 555b  .i..g...e..U..U[
-00000680: f2b0 be6a 3db4 154e cffe 59ad c89f 0c11  ...j=..N..Y.....
-00000690: 4e16 0b12 4863 9417 a64a a2f3 1953 bee7  N...Hc...J...S..
-000006a0: 2b49 c455 38bf 4533 b612 9718 bce3 e6c7  +I.U8.E3........
-000006b0: 714e 53b8 1276 b60f 0232 b9bb 39a9 7a65  qNS..v...2..9.ze
-000006c0: 3167 a6f2 df2d 0c09 2c5b 8859 12e2 4d5d  1g...-..,[.Y..M]
-000006d0: edd5 e79b 9cae 7a22 76fa 9777 c160 f2fd  ......z"v..w.`..
-000006e0: 70c9 470f e53b e75f f45d 43ae 7ef6 dde3  p.G..;._.]C.~...
-000006f0: fa6e 933b 484c 9c79 c511 0174 4502 2395  .n.;HL.y...tE.#.
-00000700: 1c06 1617 32e4 50ee 9290 0613 01cd 94c9  ....2.P.........
-00000710: 44f0 0282 64a6 1c80 98fa 0bbd f20c b929  D...d..........)
-00000720: 15ce ad3e 397f 452c 8386 4e5e d225 1214  ...>9.E,..N^.%..
-00000730: 8ab0 0c05 2117 72e3 efef 936a 778c d7fa  ....!.r....jw...
-00000740: 2c81 6d84 5432 64d5 17ca 4389 c13d 3372  ,.m.T2d...C..=3r
-00000750: 43d8 5425 f3ae da26 0b85 dbe2 54cd bb1a  C.T%...&....T...
-00000760: be26 604b c37a 6e9d 2d27 ffdb 5ed4 3db4  .&`K.zn.-'..^.=.
-00000770: 173d 46f3 a399 e01e b387 739b 7ab8 c245  .=F.......s.z..E
-00000780: acff 58d6 1ef9 32df 3970 db3a de03 5ee6  ..X...2.9p.:..^.
-00000790: 132c 43a4 7ec1 7d8a 8a80 11ab 62be baaf  .,C.~.}.....b...
-000007a0: 4ff9 259c 3bb4 7bf1 8120 9bfc d6db a4f6  O.%.;.{.. ......
-000007b0: dde0 0c7c d4ab 5aa5 642b 113f 4b07 7c1f  ...|..Z.d+.?K.|.
-000007c0: 9206 638c 5bf4 345f 8f14 62ad a6b1 adc6  ..c.[.4_..b.....
-000007d0: da31 0c79 8058 f30c a166 38df 8745 9a1a  .1.y.X...f8..E..
-000007e0: 33d5 8bac 398d 0a6f 41d5 40e5 3fdb d40d  3...9..oA.@.?...
-000007f0: 68f6 0d34 1c91 055e 3199 b636 a3e4 4e0a  h..4...^1..6..N.
-00000800: 3cdc feef 0db0 c2c4 8ee1 ed8b bf01 504b  <.............PK
-00000810: 0304 1400 0000 0800 d585 9958 0f95 4d33  ...........X..M3
-00000820: 4801 0000 4902 0000 1800 0000 786c 2f77  H...I.......xl/w
-00000830: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00000840: 2e78 6d6c 7552 db4e c330 0cfd 952a 1fb0  .xmluR.N.0...*..
-00000850: 7448 5c34 b595 d810 8207 a469 13f0 9cb5  tH\4.......i....
-00000860: 6e1b 2d89 4be2 aef0 f738 ed6e 3cf0 14fb  n.-.K....8.n<...
-00000870: c4e7 f8d8 4936 a0df 8716 8092 6f6b 5cc8  ....I6......ok\.
-00000880: 454b d42d a40c 650b 5685 1976 e0f8 a646  EK.-..e.V..v...F
-00000890: 6f15 71ea 1b19 3a0f aa1a 49d6 c89b 34bd  o.q...:...I...4.
-000008a0: 9356 6927 8a6c c4d6 bec8 b027 a31d ac7d  .Vi'.l.....'...}
-000008b0: 127a 6b95 ff59 82c1 2117 7371 0236 ba69  .zk..Y..!.sq.6.i
-000008c0: 6904 6491 75aa 812d d07b c704 4ee5 59a7  i.d.u..-.{..N.Y.
-000008d0: d216 5cd0 e812 0f75 2e1e e78b e5c4 182b  ..\....u.......+
-000008e0: 3e34 0ce1 2a4e e230 3bc4 7d4c 5eab 5ca4  >4..*N.0;.}L^.\.
-000008f0: d113 1828 294a 283e 0eb0 0263 a212 3bf9  ...()J(>...c..;.
-00000900: 3a8a 8a4b d3c8 bc8e 4ff2 cfe3 fc6c 6fa7  :..K....O....lo.
-00000910: 02ac d07c ea8a da5c 3c88 a482 5af5 8636  ...|...\<...Z..6
-00000920: 38bc c071 a6db 8bc5 2745 aac8 3c0e 898f  8..q....'E..<...
-00000930: c316 5919 83d8 920b b58b 4bda 9267 5c73  ..Y.......K..g\s
-00000940: 272a 3ae5 9505 029f 4962 1b11 94e5 91b4  '*:.....Ib......
-00000950: fc8f 7450 a687 bf04 c91d 4f63 4c16 e28a  ..tP......OcL...
-00000960: df94 6fb4 0b89 819a 85d2 d93d 1bf5 93e7  ..o........=....
-00000970: 2921 ecc6 27d9 2111 da31 6cf9 a9c1 c702  )!..'.!..1l.....
-00000980: beaf 11e9 9cc4 9d9d 7f4f f10b 504b 0304  .........O..PK..
-00000990: 1400 0000 0800 d585 9958 0f95 4d33 4801  .........X..M3H.
-000009a0: 0000 4902 0000 1800 0000 786c 2f77 6f72  ..I.......xl/wor
-000009b0: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
-000009c0: 6d6c 7552 db4e c330 0cfd 952a 1fb0 7448  mluR.N.0...*..tH
-000009d0: 5c34 b595 d810 8207 a469 13f0 9cb5 6e1b  \4.......i....n.
-000009e0: 2d89 4be2 aef0 f738 ed6e 3cf0 14fb c4e7  -.K....8.n<.....
-000009f0: f8d8 4936 a0df 8716 8092 6f6b 5cc8 454b  ..I6......ok\.EK
-00000a00: d42d a40c 650b 5685 1976 e0f8 a646 6f15  .-..e.V..v...Fo.
-00000a10: 71ea 1b19 3a0f aa1a 49d6 c89b 34bd 9356  q...:...I...4..V
-00000a20: 6927 8a6c c4d6 bec8 b027 a31d ac7d 127a  i'.l.....'...}.z
-00000a30: 6b95 ff59 82c1 2117 7371 0236 ba69 6904  k..Y..!.sq.6.ii.
-00000a40: 6491 75aa 812d d07b c704 4ee5 59a7 d216  d.u..-.{..N.Y...
-00000a50: 5cd0 e812 0f75 2e1e e78b e5c4 182b 3e34  \....u.......+>4
-00000a60: 0ce1 2a4e e230 3bc4 7d4c 5eab 5ca4 d113  ..*N.0;.}L^.\...
-00000a70: 1828 294a 283e 0eb0 0263 a212 3bf9 3a8a  .()J(>...c..;.:.
-00000a80: 8a4b d3c8 bc8e 4ff2 cfe3 fc6c 6fa7 02ac  .K....O....lo...
-00000a90: d07c ea8a da5c 3c88 a482 5af5 8636 38bc  .|...\<...Z..68.
-00000aa0: c071 a6db 8bc5 2745 aac8 3c0e 898f c316  .q....'E..<.....
-00000ab0: 5919 83d8 920b b58b 4bda 9267 5c73 272a  Y.......K..g\s'*
-00000ac0: 3ae5 9505 029f 4962 1b11 94e5 91b4 fc8f  :.....Ib........
-00000ad0: 7450 a687 bf04 c91d 4f63 4c16 e28a df94  tP......OcL.....
-00000ae0: 6fb4 0b89 819a 85d2 d93d 1bf5 93e7 2921  o........=....)!
-00000af0: ecc6 27d9 2111 da31 6cf9 a9c1 c702 beaf  ..'.!..1l.......
-00000b00: 11e9 9cc4 9d9d 7f4f f10b 504b 0304 1400  .......O..PK....
-00000b10: 0000 0800 d585 9958 6464 8808 5c02 0000  .......Xdd..\...
-00000b20: db05 0000 1800 0000 786c 2f77 6f72 6b73  ........xl/works
-00000b30: 6865 6574 732f 7368 6565 7433 2e78 6d6c  heets/sheet3.xml
-00000b40: bd54 6d6f da40 0cfe 2b28 9f51 0368 7d11  .Tmo.@..+(.Q.h}.
-00000b50: 0a91 7829 0569 685d a1dd c7ca 2486 dcb8  ..x).ih]....$...
-00000b60: 9cb3 3ba7 d9fe fd7c 494b bb2a f071 5fc8  ..;....|IK.*.q_.
-00000b70: f939 3f3e 3fc6 7654 913d b80c 913b bf73  .9?>?.vT.=...;.s
-00000b80: 6ddc 28c8 988b 6118 ba24 c31c dc05 1568  m.(...a..$.....h
-00000b90: e466 4736 0716 d3ee 4357 5884 b426 e53a  .fG6....CWX..&.:
-00000ba0: 1cf4 7a57 610e ca04 7154 63f7 368e a864  ..zWa...qTc.6..d
-00000bb0: ad0c dedb 8e2b f31c ec9f 096a aa46 413f  .....+.....j.FA?
-00000bc0: 7803 1ed4 3ee3 1a08 e3a8 803d ae91 1f0b  x...>......=....
-00000bd0: 2188 191e e3a4 2a47 e314 998e c5dd 2818  !.....*G......(.
-00000be0: f787 cb86 517b 3c29 acdc 8773 c78b d912  ....Q{<)...s....
-00000bf0: 1dbc b14c 4741 cfe7 841a 13f6 2140 3e2f  ...LGA......!@>/
-00000c00: 3845 ad7d 24c9 e4d7 6bd0 e0fd 51cf fc78  8E.}$...k...Q..x
-00000c10: 7e0b 3faf f54b 7a5b 7038 25fd 43a5 9c8d  ~.?..Kz[p8%.C...
-00000c20: 829b a093 e20e 4acd 0f54 2df0 55d3 e57b  ......J..T-.U..{
-00000c30: 8a33 6088 234b 55c7 7ab1 7194 f883 7f52  .3`.#KU.z.q....R
-00000c40: 1c95 f145 5ab3 155c c94b 1c33 3a7e 7654  ...EZ..\.K.3:~vT
-00000c50: da04 a390 2511 0f87 c92b 6d72 9626 62d0  ....%....+mr.&b.
-00000c60: a269 654e cf32 69fb 13eb dab4 3067 6799  .ieN.2i.....0gg.
-00000c70: 600c 31f8 eaba 16ee ed29 ae4a 5bbc e7a7  `.1......).J[...
-00000c80: bc0d e46d 99dd 9df2 4fd1 2556 153e ab16  ...m....O.%V.>..
-00000c90: dae2 a420 d8b7 8958 9e2f 7a69 0cda 6787  ... ...X./zi..g.
-00000ca0: ccca 7ce6 87f2 bfbf 3553 d308 a9fc 3e81  ..|.....5S....>.
-00000cb0: 5669 53b3 4e42 a591 e083 e0f3 d5b1 3907  ViS.NB........9.
-00000cc0: c371 bff7 e5e6 f2fa 4a1a 36a3 6a66 a998  .q......J.6.jf..
-00000cd0: 5165 7c73 d7c0 d214 25af d039 99a1 2378  Qe|s....%..9..#x
-00000ce0: 6b2d d98f 2068 99bf 8906 73a8 678e ff14  k-.. h....s.g...
-00000cf0: 826b e558 5ef6 b35d 6ae8 c7c1 7a75 db5d  .k.X^..]j...zu.]
-00000d00: af1e 1fe6 dd3b c58b 72fb e8d0 ce11 d32d  .....;..r......-
-00000d10: 2487 ee66 3cdd 7427 d260 d90a ac98 168c  $..f<.t'.`......
-00000d20: d3c0 6437 0879 7723 d5f0 1abf 5252 0b08  ..d7.yw#....RR..
-00000d30: a2f0 1837 0aff 1577 4aec 7430 9cfe 3fb1  ...7...wJ.t0..?.
-00000d40: e324 c182 4106 c6e7 de28 93cd 74a8 adef  .$..A....(..t...
-00000d50: 2518 56be b55f 9aeb b578 a660 53f7 9e76  %.V.._...x.`S..v
-00000d60: 8d7f 33b8 a0c2 1fcf 2bfe 04b8 66e9 4925  ..3.....+...f.I%
-00000d70: f74a fa40 e34e daa0 7771 2dab c336 5ba4  .J.@.N..wq-..6[.
-00000d80: 3198 8a5a c396 9829 af8f 992c 5fb4 de41  1..Z...)...,_..A
-00000d90: ee77 447c 34fc 163b eef3 f82f 504b 0304  .wD|4..;.../PK..
-00000da0: 1400 0000 0800 d585 9958 1837 6c2c be02  .........X.7l,..
-00000db0: 0000 7808 0000 1800 0000 786c 2f77 6f72  ..x.......xl/wor
-00000dc0: 6b73 6865 6574 732f 7368 6565 7434 2e78  ksheets/sheet4.x
-00000dd0: 6d6c bd96 db72 da30 1086 5fc5 e36b 2606  ml...r.0.._..k&.
-00000de0: a639 0c63 3c93 84a4 4903 2dcd 815e 32c2  .9.c<...I.-..^2.
-00000df0: 5e8c 0659 eb48 eb38 79fb ae4c 2069 c682  ^..Y.H.8y..L i..
-00000e00: bb5e 21ad f549 fbaf 56bb c435 9ab5 5d01  .^!..I..V..5..].
-00000e10: 50f0 5a28 6d87 e18a a81c 4491 4d57 5008  P.Z(m.....D.MWP.
-00000e20: 7b84 2568 feb2 4453 08e2 a9c9 235b 1a10  {.%h..DS....#[..
-00000e30: 5903 152a ea77 bb27 5121 a40e 93b8 b14d  Y..*.w.'Q!.....M
-00000e40: 4d12 6345 4a6a 989a c056 4521 ccdb 0528  M.cEJj...VE!...(
-00000e50: ac87 612f dc1a ee65 bea2 c610 2571 2972  ..a/...e....%q)r
-00000e60: 7800 7a2a 19e0 69b4 db27 9305 682b 5107  x.z*..i..'..h+Q.
-00000e70: 0696 c3f0 bc37 986d 8866 c54c 426d 3f8d  .....7.m.f.LBm?.
-00000e80: 0327 6681 b876 93db 6c18 769d 4fa0 2025  .'f..v..l.v.O. %
-00000e90: b785 e09f 17b8 04a5 dc4e ecc9 f3fb a6e1  .........N......
-00000ea0: c7a1 8efc 3cde 6e7f dde8 67f7 16c2 c225  ....<.n...g....%
-00000eb0: aa3f 32a3 d530 3c0b 830c 96a2 5274 8ff5  .?2..0<.....Rt..
-00000ec0: 0dbc 6b3a fe70 7124 4824 b1c1 3a30 4e6c  ..k:.pq$H$..:0Nl
-00000ed0: 12a7 6ee0 8ee4 8552 bb20 3d90 61bb e493  ..n....R. =.a...
-00000ee0: 2891 baac 682e b338 22f6 c2d9 a2f4 9db9  (...h..8".......
-00000ef0: d8cf 6851 400b 75b9 9f4a 0541 8ee6 ad85  ..hQ@.u..J.A....
-00000f00: 1cf9 48be fd4c 3ab0 ddcf abc3 9cc7 d76b  ..H..L:........k
-00000f10: 1fc9 d9e4 0dcb f703 90e7 ac9b 03d8 9ec0  ................
-00000f20: dcfa 5061 2da6 52b8 5c6b c17e f8b0 e74a  ..Pa-.R.\k.~...J
-00000f30: 28b9 9460 6c0b 75e7 a3e0 b5e4 b486 6cbe  (..`l.u.......l.
-00000f40: 71b8 051d fb50 02cb c1b4 b66a 0bcc c447  q....P.....j...G
-00000f50: 592e 079a 643a b7f0 0246 525b 687e fab3  Y...d:...FR[h~..
-00000f60: 6dfe d26b 017e f980 9a5f e97c adb1 6e0b  m..k.~..._.|..n.
-00000f70: e574 af32 7ed4 6040 a76d ea7e ef25 0b20  .t.2~.`@.m.~.%. 
-00000f80: 91f1 836d 01ef bdca da92 f2c1 b7da 938d  ...m............
-00000f90: 8fbe f519 d8d4 c8d2 9352 4f5e 3522 6f4b  .........RO^5"oK
-00000fa0: a6d9 feb8 555a 83e1 eb25 92fa 2b1f 7109  ....UZ...%..+.q.
-00000fb0: dbd6 c54d 4d73 819a 71e6 664d c2db 20c5  ...MMs..q.fM.. .
-00000fc0: 4af3 e6fd f0eb a76d 9d1d f707 e35e f7db  J......m.....^..
-00000fd0: d9f1 e909 d7de 15d6 2383 e588 6fd8 d5e9  ........#...o...
-00000fe0: c670 eb6a d204 ace5 76b0 335e 1983 e6b3  .p.j....v.3^....
-00000ff0: 5128 6e25 174a e875 d33e e8ad 64bb 9296  Q(n%.J.u.>..d...
-00001000: f864 d7a6 2a25 7a49 988a ca82 0d34 5240  .d..*%zI.....4R@
-00001010: dcae c876 1e27 77d3 cef6 5d07 8418 e4c0  ...v.'w...].....
-00001020: 8265 da49 5193 e10e d694 2727 a6e3 9a1f  .e.IQ.....''....
-00001030: 4f54 6050 81ed 7cbc 9830 8e76 67c4 d1bf  OT`P..|..0.vg...
-00001040: 427d c227 fdc1 e4ff 09bf e126 d419 63dd  B}.'.......&..c.
-00001050: f989 745e 968a 652c d401 bfbf 18ec a623  ..t^..e,.......#
-00001060: 4f84 c925 dfac 8225 5f6c f7e8 94fb 9ad9  O..%...%_l......
-00001070: b4b8 cd84 b06c 3c59 2011 16cd 70c5 ff0c  .....l<Y ...p...
-00001080: c0b8 05fc 7d89 48bb 896b b1bb 3f1b c95f  ....}.H..k..?.._
-00001090: 504b 0304 1400 0000 0800 d585 9958 4cb5  PK...........XL.
-000010a0: afc5 9403 0000 910d 0000 1800 0000 786c  ..............xl
-000010b0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-000010c0: 7435 2e78 6d6c bd57 db6e db38 10fd 1541  t5.xml.W.n.8...A
-000010d0: cf42 651b dbb4 3064 0376 aede 36dd 6cd2  .Be...0d.v..6.l.
-000010e0: 3add 7d11 6871 2c73 4391 2a39 b292 bfdf  :.}.hq,sC.*9....
-000010f0: a114 2769 40c6 401e fc24 5e74 8687 c3e1  ..'i@.@..$^t....
-00001100: 9961 d66a 7367 3700 18dd 5752 d949 bc41  .a.jsg7...WR.I.A
-00001110: acc7 696a 8b0d 54cc 7ed0 3528 9a59 6b53  ..ij..T.~.5(.YkS
-00001120: 31a4 ae29 535b 1b60 bc03 5532 1d0d 0647  1..)S[.`..U2...G
-00001130: 69c5 848a a759 3776 65a6 996e 500a 0557  i....Y7ve..nP..W
-00001140: 26b2 4d55 31f3 3007 a9db 493c 8c77 03d7  &.MU1.0...I<.w..
-00001150: a2dc 6037 904e b39a 9570 03f8 a326 0075  ..`7.N...p...&.u
-00001160: d327 3b5c 54a0 acd0 2a32 b09e c4b3 e178  .';\T...*2.....x
-00001170: 76d6 43ba 5f96 025a fba2 1db9 ddac b4be  v.C._..Z........
-00001180: 739d 059f c403 470a 2414 e86c 30fa 6ce1  s.....G.$..l0.l.
-00001190: 18a4 74a6 88ca af47 abf1 f3aa 0ef9 b2bd  ..t....G........
-000011a0: 337f d639 80f8 ad98 8563 2d6f 05c7 cd24  3..9.....c-o...$
-000011b0: fe1c 471c d6ac 9178 addb 0b78 dcd4 c767  ..G....x...x...g
-000011c0: 8a27 0cd9 3433 ba8d 8cdb ed34 2b5c c32d  .'..43.....4+\.-
-000011d0: 493f 0ae5 bc74 8386 c605 ad84 d3aa b198  I?...t..........
-000011e0: d7cc da9c 3384 2c45 e2e2 66d2 e211 39df  ....3.,E..f...9.
-000011f0: 8f04 b515 462b f21c 7a0c 1c87 0cd8 4210  ....F+..z.....B.
-00001200: 42ac 4591 ff6a c03a 8f79 e027 4138 1aa1  B.E..j.:.y.'A8..
-00001210: 4a5a 1ccd 8307 771a c271 61fa e3f1 80ce  JZ....w..qa.....
-00001220: 4220 a66c 0b26 17aa 8b4b 9917 5a15 50fb  B .l.&...K..Z.P.
-00001230: b67b 1e32 01f7 35ad 0b3c 3760 e9f8 3cd0  .{.2..5..<7`..<.
-00001240: 8b10 1475 9d4b d882 f480 1621 10f9 d43c  ...u.K.....!...<
-00001250: e44a 73df a9fe 1942 298d 603d 802f 2180  .Js....B).`=./!.
-00001260: 5075 83b9 e01e ccd7 b731 8a55 3e6a 976f  Pu.......1.U>j.o
-00001270: a30a 0ad3 527b 8ffc 5b08 49fa c185 03fa  ....R{..[.I.....
-00001280: 79fe b51f 17e0 7a15 4292 1e05 ddf2 f71e  y.....z.B.......
-00001290: 5060 adeb 3db0 371c 7313 0c6b 6b75 2158  P`..=.7.s..kku!X
-000012a0: e036 7c0f 8716 9374 6fc1 f822 e5c7 de0b  .6|....to.."....
-000012b0: d013 f640 97c1 0b40 f290 0b6b 1b9f 636e  ...@...@...k..cn
-000012c0: 830a 4109 8504 a6c8 2ddd 1d23 d0e7 9a9f  ..A.....-..#....
-000012d0: e168 cbb7 430f e09f 10a0 2599 cfef 946e  .h..C.....%....n
-000012e0: 7dae fcf7 cd9d 5156 0003 a428 1ee4 2c28  }.....QV...(..,(
-000012f0: dd1d b402 64a4 dccc 870c 4ab7 372c 6741  ....d.....J.7,gA
-00001300: a10e 04e4 2c28 cd1c 6c61 441d 08ab 5950  ....,(..laD...YP
-00001310: 9a91 95be 889a 0565 b9f7 5ea3 1469 b305  .......e..^..i..
-00001320: 444a 08af 0ca4 9409 77e9 b54f 8dce 5b4b  DJ......w..O..[K
-00001330: 8a5f de85 bd8d 0add 2832 7e14 bf9e daa5  ._......(2~.....
-00001340: ebf9 683c 1f0e fef8 fcf1 d311 a5f0 8d6e  ..h<...........n
-00001350: 4f8c ae4f e89c 5dba ef06 164e 992e c15a  O..O..]....N...Z
-00001360: 2a2b 9e06 4f8d d1e6 e520 9354 92cc 2553  *+..O.... .T..%S
-00001370: 775d 1982 0f35 8d4b 6191 5676 69a5 916c  w]...5.Ka.Vvi..l
-00001380: 388d 396c 9342 246e 6749 6d34 8fb3 f469  8.9l.B$ngIm4...i
-00001390: 324b 7f67 1862 7c3a 1a9f 1e8e b150 05d5  2K.g.b|:.....P..
-000013a0: 6716 78c2 e1b1 f51e d2e7 a3f1 f941 49cb  g.x..........AI.
-000013b0: 8643 5e6a cd13 b8ef 3b2b f62e e68b d178  .C^j....;+.....x
-000013c0: 7138 e6b6 59fd 473a 9ae8 eef3 1ebe cbd1  q8..Y.G:........
-000013d0: 7879 38be 056b 2cd8 880a 8b08 293a d026  xy8..k,.....):.&
-000013e0: df2f bf5c 25bb 7415 a1d6 5109 7483 4591  ./.\%.t...Q.t.E.
-000013f0: 5059 8586 4afb 2eeb badb 99b8 5701 7564  PY..J.......W.ud
-00001400: 64b4 049b 3c27 82f7 6cfc 7634 be3d dcc6  d...<'..l.v4.=..
-00001410: 2fa8 384f beea 36f9 a671 56d7 92b6 b192  /.8O..6..qV.....
-00001420: 7b78 bf1a b0fd 53e5 9299 5290 5449 5893  {x....S...R.TIX.
-00001430: 520d 3e7c a27a dff4 a57f dfa1 02b1 63b2  R.>|.z........c.
-00001440: d288 baea 9a1b 7a32 8171 3fd0 fc5a 5359  ......z2.q?..ZSY
-00001450: b7eb b8a7 c7d3 2b6c fa3f 504b 0304 1400  ......+l.?PK....
-00001460: 0000 0800 d585 9958 1837 6c2c be02 0000  .......X.7l,....
-00001470: 7808 0000 1800 0000 786c 2f77 6f72 6b73  x.......xl/works
-00001480: 6865 6574 732f 7368 6565 7436 2e78 6d6c  heets/sheet6.xml
-00001490: bd96 db72 da30 1086 5fc5 e36b 2606 a639  ...r.0.._..k&..9
-000014a0: 0c63 3c93 84a4 4903 2dcd 815e 32c2 5e8c  .c<...I.-..^2.^.
-000014b0: 0659 eb48 eb38 79fb ae4c 2069 c682 bb5e  .Y.H.8y..L i...^
-000014c0: 21ad f549 fbaf 56bb c435 9ab5 5d01 50f0  !..I..V..5..].P.
-000014d0: 5a28 6d87 e18a a81c 4491 4d57 5008 7b84  Z(m.....D.MWP.{.
-000014e0: 2568 feb2 4453 08e2 a9c9 235b 1a10 5903  %h..DS....#[..Y.
-000014f0: 152a ea77 bb27 5121 a40e 93b8 b14d 4d12  .*.w.'Q!.....MM.
-00001500: 6345 4a6a 989a c056 4521 ccdb 0528 ac87  cEJj...VE!...(..
-00001510: 612f dc1a ee65 bea2 c610 2571 2972 7800  a/...e....%q)rx.
-00001520: 7a2a 19e0 69b4 db27 9305 682b 5107 0696  z*..i..'..h+Q...
-00001530: c3f0 bc37 986d 8866 c54c 426d 3f8d 0327  ...7.m.f.LBm?..'
-00001540: 6681 b876 93db 6c18 769d 4fa0 2025 b785  f..v..l.v.O. %..
-00001550: e09f 17b8 04a5 dc4e ecc9 f3fb a6e1 c7a1  .......N........
-00001560: 8efc 3cde 6e7f dde8 67f7 16c2 c225 aa3f  ..<.n...g....%.?
-00001570: 32a3 d530 3c0b 830c 96a2 5274 8ff5 0dbc  2..0<.....Rt....
-00001580: 6b3a fe70 7124 4824 b1c1 3a30 4e6c 12a7  k:.pq$H$..:0Nl..
-00001590: 6ee0 8ee4 8552 bb20 3d90 61bb e493 2891  n....R. =.a...(.
-000015a0: baac 682e b338 22f6 c2d9 a2f4 9db9 d8cf  ..h..8".........
-000015b0: 6851 400b 75b9 9f4a 0541 8ee6 ad85 1cf9  hQ@.u..J.A......
-000015c0: 48be fd4c 3ab0 ddcf abc3 9cc7 d76b 1fc9  H..L:........k..
-000015d0: d9e4 0dcb f703 90e7 ac9b 03d8 9ec0 dcfa  ................
-000015e0: 5061 2da6 52b8 5c6b c17e f8b0 e74a 28b9  Pa-.R.\k.~...J(.
-000015f0: 9460 6c0b 75e7 a3e0 b5e4 b486 6cbe 71b8  .`l.u.......l.q.
-00001600: 051d fb50 02cb c1b4 b66a 0bcc c447 592e  ...P.....j...GY.
-00001610: 079a 643a b7f0 0246 525b 687e fab3 6dfe  ..d:...FR[h~..m.
-00001620: d26b 017e f980 9a5f e97c adb1 6e0b e574  .k.~..._.|..n..t
-00001630: af32 7ed4 6040 a76d ea7e ef25 0b20 91f1  .2~.`@.m.~.%. ..
-00001640: 836d 01ef bdca da92 f2c1 b7da 938d 8fbe  .m..............
-00001650: f519 d8d4 c8d2 9352 4f5e 3522 6f4b a6d9  .......RO^5"oK..
-00001660: feb8 555a 83e1 eb25 92fa 2b1f 7109 dbd6  ..UZ...%..+.q...
-00001670: c54d 4d73 819a 71e6 664d c2db 20c5 4af3  .MMs..q.fM.. .J.
-00001680: e6fd f0eb a76d 9d1d f707 e35e f7db d9f1  .....m.....^....
-00001690: e909 d7de 15d6 2383 e588 6fd8 d5e9 c670  ......#...o....p
-000016a0: eb6a d204 ace5 76b0 335e 1983 e6b3 5128  .j....v.3^....Q(
-000016b0: 6e25 174a e875 d33e e8ad 64bb 9296 f864  n%.J.u.>..d....d
-000016c0: d7a6 2a25 7a49 988a ca82 0d34 5240 dcae  ..*%zI.....4R@..
-000016d0: c876 1e27 77d3 cef6 5d07 8418 e4c0 8265  .v.'w...]......e
-000016e0: da49 5193 e10e d694 2727 a6e3 9a1f 4f54  .IQ.....''....OT
-000016f0: 6050 81ed 7cbc 9830 8e76 67c4 d1bf 427d  `P..|..0.vg...B}
-00001700: c227 fdc1 e4ff 09bf e126 d419 63dd f989  .'.......&..c...
-00001710: 745e 968a 652c d401 bfbf 18ec a623 4f84  t^..e,.......#O.
-00001720: c925 dfac 8225 5f6c f7e8 94fb 9ad9 b4b8  .%...%_l........
-00001730: cd84 b06c 3c59 2011 16cd 70c5 ff0c c0b8  ...l<Y ...p.....
-00001740: 05fc 7d89 48bb 896b b1bb 3f1b c95f 504b  ..}.H..k..?.._PK
-00001750: 0304 1400 0000 0800 d585 9958 146c abe1  ...........X.l..
-00001760: 6801 0000 e802 0000 1800 0000 786c 2f77  h...........xl/w
-00001770: 6f72 6b73 6865 6574 732f 7368 6565 7437  orksheets/sheet7
-00001780: 2e78 6d6c 7552 db6e 8330 0cfd 1594 0f58  .xmluR.n.0.....X
-00001790: e8a4 5d54 01d2 7a99 b687 4955 ab6d 8f55  ..]T..z...IU.m.U
-000017a0: 0a06 a2e6 c21c 33b6 bf5f 02bd 692a 4fd8  ......3.._..i*O.
-000017b0: ce39 c7f6 c149 6771 ef6a 008a 7eb4 322e  .9...Igq.j..~.2.
-000017c0: 6535 5133 e5dc e535 68e1 6e6c 03c6 bf94  e5Q3...5h.nl....
-000017d0: 16b5 209f 62c5 5d83 208a 9ea4 15bf 8de3  .. .b.]. .......
-000017e0: 7bae 8534 2c4b fada 0ab3 c4b6 a4a4 8115  {..4,K..........
-000017f0: 46ae d55a e0ef 0c94 ed52 3661 c7c2 5a56  F..Z.....R6a..ZV
-00001800: 35f5 059e 258d a860 03f4 de78 824f f949  5...%..`...x.O.I
-00001810: a790 1a8c 93d6 4408 65ca 9e26 d3e5 c0e8  ......D.e..&....
-00001820: 111f 123a 7711 4761 999d b5fb 90bc 1629  ...:w.Ga.......)
-00001830: 8bc3 4ca0 20a7 2021 fce7 1be6 a054 50f2  ..L. . !.....TP.
-00001840: 937c 1d44 d9b9 6960 5ec6 47f9 e77e 7f3f  .|.D..i`^.G..~.?
-00001850: de4e 3898 5bf5 290b aa53 f6c8 a202 4ad1  .N8.[.)..S....J.
-00001860: 2a5a dbee 050e 3bdd 9d47 5c08 1259 82b6  *Z....;..G\..Y..
-00001870: 8b30 2c9b 2579 0842 4b0f 9426 98b4 21f4  .0,.%y.BK..&..!.
-00001880: 75e9 3b51 268b 8493 ef1f 329e 1fd0 b331  u.;Q&.....2....1
-00001890: b411 1aae e0e7 63f8 025c 8eb2 0966 5ca1  ......c..\...f\.
-000018a0: 2dc6 6824 2a77 05bf 1cc5 83a3 2db6 c600  -.h$*w......-...
-000018b0: 6e1d 1049 f39f cfbd 2147 9707 87c2 05bc  n..I....!G......
-000018c0: 09ac a471 9182 d2eb c637 0fde 471c 2c1d  ...q.....7..G.,.
-000018d0: 12b2 4d7f 313b 4b64 751f d6fe 1201 03c0  ..M.1;Kdu.......
-000018e0: bf97 d6d2 2909 bff4 74dc d91f 504b 0304  ....)...t...PK..
-000018f0: 1400 0000 0800 d585 9958 90c3 86f2 7c03  .........X....|.
-00001900: 0000 900b 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00001910: 6b73 6865 6574 732f 7368 6565 7438 2e78  ksheets/sheet8.x
-00001920: 6d6c bd56 5173 da38 10fe 2b8c 9fd5 9a30  ml.VQs.8..+....0
-00001930: d7b4 c300 3349 8026 7725 4d03 691f 3d42  ....3I.&w%M.i.=B
-00001940: 5eb0 0e59 7257 eb00 fffe 5676 4272 193b  ^..YrW....VvBr.;
-00001950: 99e6 8117 9056 fa56 fbc9 bb9f 76b0 75b8  .....V.V....v.u.
-00001960: f119 0075 76b9 b17e 1865 4445 3f8e bdca  ...uv..~.eDE?...
-00001970: 2097 fea3 2bc0 f2ca ca61 2e89 a7b8 8e7d   ...+....a.....}
-00001980: 8120 d30a 949b b8d7 ed9e c6b9 d436 1a0d  . ...........6..
-00001990: 2adb 0d8e 06ae 24a3 2ddc 60c7 9779 2e71  *.....$.-.`..y.q
-000019a0: 7f0e c66d 87d1 49f4 68b8 d5eb 8c2a 433c  ...m..I.h....*C<
-000019b0: 1a14 720d 73a0 bb82 013c 8d0f 7e52 9d83  ..r.s....<..~R..
-000019c0: f5da d90e c26a 189d 9df4 e735 a2da f153  .....j.....5...S
-000019d0: c3d6 3f1b 7702 99a5 739b 30b9 4a87 5137  ..?.w...s.0.J.Q7
-000019e0: c404 0614 0517 92ff eee1 028c 099e 3892  ..............8.
-000019f0: df0f 4ea3 a743 03f2 f9f8 d1fd b4e2 cfe1  ..N..C..........
-00001a00: 2da5 870b 677e e994 b261 f425 eaa4 b092  -...g~...a.%....
-00001a10: a5a1 5bb7 bd84 074e 9f9e 421c 4b92 a301  ..[....N..B.K...
-00001a20: ba6d 0703 d9d1 4085 4138 9237 6a1b 2e69  .m....@.A8.7j..i
-00001a30: 4ec8 76cd 27d1 e877 09b8 4f68 5fc0 2026  N.v.'..w..Oh_. &
-00001a40: 8e23 5863 f580 3a6f 4311 784a a4f7 40be  .#Xc..:oC.xJ..@.
-00001a50: 0176 d106 e3cf a89c 4d75 b89c 26e0 b8f5  .v......Mu..&...
-00001a60: 3c94 854e 08f2 c248 6a8a 74f2 6aa4 8aaf  <..N...Hj.t.j...
-00001a70: 3071 cb7f a1fa 1e0d f0e9 db70 ef4a 544d  0q.........p.JTM
-00001a80: d8af 6f63 9977 aa15 479e 5899 37f9 b8fc  ..oc.w..G.X.7...
-00001a90: 131f 3a6d f070 f5b6 076d 8b92 9ad1 7fb7  ..:m.p...m......
-00001aa0: a787 347a a501 9b3e d73f 6da8 faa4 10ec  ..4z...>.?m.....
-00001ab0: dae1 be01 f9ad 0dc9 65fc 0674 d606 552e  ........e..t..U.
-00001ac0: 2f9c 05db 9892 d7af 5e0f d8fb 06cc f756  /.......^......V
-00001ad0: 7a4d 5778 d3b6 bbe5 93ff 68db 9f82 57a8  zMWx......h...W.
-00001ae0: 8b50 230d b0db 5622 72dd 447c fe2a 712c  .P#...V"r.D|.*q,
-00001af0: ad05 4cb8 8e49 db97 f898 45e4 5199 6a55  ..L..I....E.Q.jU
-00001b00: 49f9 f727 2704 ff87 0aee 2857 5a76 7e1a  I..''.....(WZv~.
-00001b10: bd5c 3a28 5daf 7f76 d2fd ebcb a7cf a7ac  .\:(]..v........
-00001b20: 7e99 db8e d115 63b7 b541 292b c355 4895  ~.....c..A)+.UH.
-00001b30: 1978 cf82 7c30 4e10 1d3e 374a c362 7e6e  .x..|0N..>7J.b~n
-00001b40: a4dd 5402 1ee4 6a18 19ed 894f 0e0f 4569  ..T...j....O..Ei
-00001b50: e4c9 2822 7e25 c847 83f8 601a c4ff 8fab  ..("~%.G..`.....
-00001b60: 2dce 71af 3f3e 5e9c 9c10 463b e41c f7a2  -.q.?>^...F;....
-00001b70: 8e59 5086 0049 e60a 9162 b94e 6a6b 8212  .YP..I...b.Njk..
-00001b80: 2149 b507 2edf 6ae1 03b9 0f6b b0f0 1e8e  !I....j....k....
-00001b90: 935e 7f72 3c8e 674a 4141 d22a 5870 a289  .^.r<.gJAA.*Xp..
-00001ba0: 73b0 2ae3 5778 53cd 7e94 d292 2619 d4b8  s.*.WxS.~...&...
-00001bb0: 32cc 7967 2a31 f54f 6157 f6ef 162e 5d11  2.yg*1.OaW....].
-00001bc0: 86ef 613c edf5 a7c7 633c 9f4d c47c 7677  ..a<....c<.M.|vw
-00001bd0: 3b15 5f35 5d96 cb3b 0f38 0548 9752 6dc4  ;._5]..;.8.H.Rm.
-00001be0: e2ec 6251 5fc2 8c2f 412c 505a cf4f 99c3  ..bQ_../A,PZ.O..
-00001bf0: 05c8 5c04 82a1 c2be 3955 1178 0fd9 59af  ..\.....9U.x..Y.
-00001c00: 3f3b 620a a317 12e5 4ec0 8e9f 641b 98ec  ?;b.....N...d...
-00001c10: 85ce 0b74 f72c 2461 89e5 db8a 2581 28ad  ...t.,$a....%.(.
-00001c20: 0785 4002 69b7 59f7 8456 c079 af98 b62f  ..@.i.Y..V.y.../
-00001c30: dc06 44ee 0c30 4e10 ec28 d736 c095 cb52  ..D..0N..(.6...R
-00001c40: 11fa c0fa d123 3618 2397 a164 c239 dc43  .....#6.#..d.9.C
-00001c50: d8ba c37a 57b1 5ff7 fad7 c7bb a914 ee85  ...zW._.........
-00001c60: d222 c8ad 609a e9eb 11bf 30f8 ba53 e59c  ."..`.....0..S..
-00001c70: 596b d65b 032b 96db eec7 cfdc ef61 ddfa  Yk.[.+.......a..
-00001c80: d513 7245 15c3 d211 b9bc 1a66 dc31 0386  ..rE.......f.1..
-00001c90: 0dbc be72 8e0e 93d0 7a1e 9af0 d17f 504b  ...r....z.....PK
-00001ca0: 0304 1400 0000 0800 d585 9958 90c3 86f2  ...........X....
-00001cb0: 7c03 0000 900b 0000 1800 0000 786c 2f77  |...........xl/w
-00001cc0: 6f72 6b73 6865 6574 732f 7368 6565 7439  orksheets/sheet9
-00001cd0: 2e78 6d6c bd56 5173 da38 10fe 2b8c 9fd5  .xml.VQs.8..+...
-00001ce0: 9a30 d7b4 c300 3349 8026 7725 4d03 691f  .0....3I.&w%M.i.
-00001cf0: 3d42 5eb0 0e59 7257 eb00 fffe 5676 4272  =B^..YrW....VvBr
-00001d00: 193b 99e6 8117 9056 fa56 fbc9 bb9f 76b0  .;.....V.V....v.
-00001d10: 75b8 f119 0075 76b9 b17e 1865 4445 3f8e  u....uv..~.eDE?.
-00001d20: bdca 2097 fea3 2bc0 f2ca ca61 2e89 a7b8  .. ...+....a....
-00001d30: 8e7d 8120 d30a 949b b8d7 ed9e c6b9 d436  .}. ...........6
-00001d40: 1a0d 2adb 0d8e 06ae 24a3 2ddc 60c7 9779  ..*.....$.-.`..y
-00001d50: 2e71 7f0e c66d 87d1 49f4 68b8 d5eb 8c2a  .q...m..I.h....*
-00001d60: 433c 1a14 720d 73a0 bb82 013c 8d0f 7e52  C<..r.s....<..~R
-00001d70: 9d83 f5da d90e c26a 189d 9df4 e735 a2da  .......j.....5..
-00001d80: f153 c3d6 3f1b 7702 99a5 739b 30b9 4a87  .S..?.w...s.0.J.
-00001d90: 5137 c404 0614 0517 92ff eee1 028c 099e  Q7..............
-00001da0: 3892 df0f 4ea3 a743 03f2 f9f8 d1fd b4e2  8...N..C........
-00001db0: cfe1 2da5 870b 677e e994 b261 f425 eaa4  ..-...g~...a.%..
-00001dc0: b092 a5a1 5bb7 bd84 074e 9f9e 421c 4b92  ....[....N..B.K.
-00001dd0: a301 ba6d 0703 d9d1 4085 4138 9237 6a1b  ...m....@.A8.7j.
-00001de0: 2e69 4ec8 76cd 27d1 e877 09b8 4f68 5fc0  .iN.v.'..w..Oh_.
-00001df0: 2026 8e23 5863 f580 3a6f 4311 784a a4f7   &.#Xc..:oC.xJ..
-00001e00: 40be 0176 d106 e3cf a89c 4d75 b89c 26e0  @..v......Mu..&.
-00001e10: b8f5 3c94 854e 08f2 c248 6a8a 74f2 6aa4  ..<..N...Hj.t.j.
-00001e20: 8aaf 3071 cb7f a1fa 1e0d f0e9 db70 ef4a  ..0q.........p.J
-00001e30: 544d d8af 6f63 9977 aa15 479e 5899 37f9  TM..oc.w..G.X.7.
-00001e40: b8fc 131f 3a6d f070 f5b6 076d 8b92 9ad1  ....:m.p...m....
-00001e50: 7fb7 a787 347a a501 9b3e d73f 6da8 faa4  ....4z...>.?m...
-00001e60: 10ec dae1 be01 f9ad 0dc9 65fc 0674 d606  ..........e..t..
-00001e70: 552e 2f9c 05db 9892 d7af 5e0f d8fb 06cc  U./.......^.....
-00001e80: f756 7a4d 5778 d3b6 bbe5 93ff 68db 9f82  .VzMWx......h...
-00001e90: 57a8 8b50 230d b0db 5622 72dd 447c fe2a  W..P#...V"r.D|.*
-00001ea0: 712c ad05 4cb8 8e49 db97 f898 45e4 5199  q,..L..I....E.Q.
-00001eb0: 6a55 49f9 f727 2704 ff87 0aee 2857 5a76  jUI..''.....(WZv
-00001ec0: 7e1a bd5c 3a28 5daf 7f76 d2fd ebcb a7cf  ~..\:(]..v......
-00001ed0: a7ac 7e99 db8e d115 63b7 b541 292b c355  ..~.....c..A)+.U
-00001ee0: 4895 1978 cf82 7c30 4e10 1d3e 374a c362  H..x..|0N..>7J.b
-00001ef0: 7e6e a4dd 5402 1ee4 6a18 19ed 894f 0e0f  ~n..T...j....O..
-00001f00: 4569 e4c9 2822 7e25 c847 83f8 601a c4ff  Ei..("~%.G..`...
-00001f10: 8fab 2dce 71af 3f3e 5e9c 9c10 463b e41c  ..-.q.?>^...F;..
-00001f20: f7a2 8e59 5086 0049 e60a 9162 b94e 6a6b  ...YP..I...b.Njk
-00001f30: 8212 2149 b507 2edf 6ae1 03b9 0f6b b0f0  ..!I....j....k..
-00001f40: 1e8e 935e 7f72 3c8e 674a 4141 d22a 5870  ...^.r<.gJAA.*Xp
-00001f50: a289 73b0 2ae3 5778 53cd 7e94 d292 2619  ..s.*.WxS.~...&.
-00001f60: d4b8 32cc 7967 2a31 f54f 6157 f6ef 162e  ..2.yg*1.OaW....
-00001f70: 5d11 86ef 613c edf5 a7c7 633c 9f4d c47c  ]...a<....c<.M.|
-00001f80: 7677 3b15 5f35 5d96 cb3b 0f38 0548 9752  vw;._5]..;.8.H.R
-00001f90: 6dc4 e2ec 6251 5fc2 8c2f 412c 505a cf4f  m...bQ_../A,PZ.O
-00001fa0: 99c3 05c8 5c04 82a1 c2be 3955 1178 0fd9  ....\.....9U.x..
-00001fb0: 59af 3f3b 620a a317 12e5 4ec0 8e9f 641b  Y.?;b.....N...d.
-00001fc0: 98ec 85ce 0b74 f72c 2461 89e5 db8a 2581  .....t.,$a....%.
-00001fd0: 28ad 0785 4002 69b7 59f7 8456 c079 af98  (...@.i.Y..V.y..
-00001fe0: b62f dc06 44ee 0c30 4e10 ec28 d736 c095  ./..D..0N..(.6..
-00001ff0: cb52 11fa c0fa d123 3618 2397 a164 c239  .R.....#6.#..d.9
-00002000: dc43 d8ba c37a 57b1 5ff7 fad7 c7bb a914  .C...zW._.......
-00002010: ee85 d222 c8ad 609a e9eb 11bf 30f8 ba53  ..."..`.....0..S
-00002020: e59c 596b d65b 032b 96db eec7 cfdc ef61  ..Yk.[.+.......a
-00002030: ddfa d513 7245 15c3 d211 b9bc 1a66 dc31  ....rE.......f.1
-00002040: 0386 0dbc be72 8e0e 93d0 7a1e 9af0 d17f  .....r....z.....
-00002050: 504b 0304 1400 0000 0800 d585 9958 90c3  PK...........X..
-00002060: 86f2 7c03 0000 900b 0000 1900 0000 786c  ..|...........xl
-00002070: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-00002080: 7431 302e 786d 6cbd 5651 73da 3810 fe2b  t10.xml.VQs.8..+
-00002090: 8c9f d59a 30d7 b4c3 0033 4980 2677 254d  ....0....3I.&w%M
-000020a0: 0369 1f3d 425e b00e 5972 57eb 00ff fe56  .i.=B^..YrW....V
-000020b0: 7642 7219 3b99 e681 1790 56fa 56fb c9bb  vBr.;.....V.V...
-000020c0: 9f76 b075 b8f1 1900 7576 b9b1 7e18 6544  .v.u....uv..~.eD
-000020d0: 453f 8ebd ca20 97fe a32b c0f2 caca 612e  E?... ...+....a.
-000020e0: 89a7 b88e 7d81 20d3 0a94 9bb8 d7ed 9ec6  ....}. .........
-000020f0: b9d4 361a 0d2a db0d 8e06 ae24 a32d dc60  ..6..*.....$.-.`
-00002100: c797 792e 717f 0ec6 6d87 d149 f468 b8d5  ..y.q...m..I.h..
-00002110: eb8c 2a43 3c1a 1472 0d73 a0bb 8201 3c8d  ..*C<..r.s....<.
-00002120: 0f7e 529d 83f5 dad9 0ec2 6a18 9d9d f4e7  .~R.......j.....
-00002130: 35a2 daf1 53c3 d63f 1b77 0299 a573 9b30  5...S..?.w...s.0
-00002140: b94a 8751 37c4 0406 1405 1792 ffee e102  .J.Q7...........
-00002150: 8c09 9e38 92df 0f4e a3a7 4303 f2f9 f8d1  ...8...N..C.....
-00002160: fdb4 e2cf e12d a587 0b67 7ee9 94b2 61f4  .....-...g~...a.
-00002170: 25ea a4b0 92a5 a15b b7bd 8407 4e9f 9e42  %......[....N..B
-00002180: 1c4b 92a3 01ba 6d07 03d9 d140 8541 3892  .K....m....@.A8.
-00002190: 376a 1b2e 694e c876 cd27 d1e8 7709 b84f  7j..iN.v.'..w..O
-000021a0: 685f c020 268e 2358 63f5 803a 6f43 1178  h_. &.#Xc..:oC.x
-000021b0: 4aa4 f740 be01 76d1 06e3 cfa8 9c4d 75b8  J..@..v......Mu.
-000021c0: 9c26 e0b8 f53c 9485 4e08 f2c2 486a 8a74  .&...<..N...Hj.t
-000021d0: f26a a48a af30 71cb 7fa1 fa1e 0df0 e9db  .j...0q.........
-000021e0: 70ef 4a54 4dd8 af6f 6399 77aa 1547 9e58  p.JTM..oc.w..G.X
-000021f0: 9937 f9b8 fc13 1f3a 6df0 70f5 b607 6d8b  .7.....:m.p...m.
-00002200: 929a d17f b7a7 8734 7aa5 019b 3ed7 3f6d  .......4z...>.?m
-00002210: a8fa a410 ecda e1be 01f9 ad0d c965 fc06  .............e..
-00002220: 74d6 0655 2e2f 9c05 db98 92d7 af5e 0fd8  t..U./.......^..
-00002230: fb06 ccf7 567a 4d57 78d3 b6bb e593 ff68  ....VzMWx......h
-00002240: db9f 8257 a88b 5023 0db0 db56 2272 dd44  ...W..P#...V"r.D
-00002250: 7cfe 2a71 2cad 054c b88e 49db 97f8 9845  |.*q,..L..I....E
-00002260: e451 996a 5549 f9f7 2727 04ff 870a ee28  .Q.jUI..''.....(
-00002270: 575a 767e 1abd 5c3a 285d af7f 76d2 fdeb  WZv~..\:(]..v...
-00002280: cba7 cfa7 ac7e 99db 8ed1 1563 b7b5 4129  .....~.....c..A)
-00002290: 2bc3 5548 9519 78cf 827c 304e 101d 3e37  +.UH..x..|0N..>7
-000022a0: 4ac3 627e 6ea4 dd54 021e e46a 1819 ed89  J.b~n..T...j....
-000022b0: 4f0e 0f45 69e4 c928 227e 25c8 4783 f860  O..Ei..("~%.G..`
-000022c0: 1ac4 ff8f ab2d ce71 af3f 3e5e 9c9c 1046  .....-.q.?>^...F
-000022d0: 3be4 1cf7 a28e 5950 8600 49e6 0a91 62b9  ;.....YP..I...b.
-000022e0: 4e6a 6b82 1221 49b5 072e df6a e103 b90f  Njk..!I....j....
-000022f0: 6bb0 f01e 8e93 5e7f 723c 8e67 4a41 41d2  k.....^.r<.gJAA.
-00002300: 2a58 70a2 8973 b02a e357 7853 cd7e 94d2  *Xp..s.*.WxS.~..
-00002310: 9226 19d4 b832 cc79 672a 31f5 4f61 57f6  .&...2.yg*1.OaW.
-00002320: ef16 2e5d 1186 ef61 3ced f5a7 c763 3c9f  ...]...a<....c<.
-00002330: 4dc4 7c76 773b 155f 355d 96cb 3b0f 3805  M.|vw;._5]..;.8.
-00002340: 4897 526d c4e2 ec62 515f c28c 2f41 2c50  H.Rm...bQ_../A,P
-00002350: 5acf 4f99 c305 c85c 0482 a1c2 be39 5511  Z.O....\.....9U.
-00002360: 780f d959 af3f 3b62 0aa3 1712 e54e c08e  x..Y.?;b.....N..
-00002370: 9f64 1b98 ec85 ce0b 74f7 2c24 6189 e5db  .d......t.,$a...
-00002380: 8a25 8128 ad07 8540 0269 b759 f784 56c0  .%.(...@.i.Y..V.
-00002390: 79af 98b6 2fdc 0644 ee0c 304e 10ec 28d7  y.../..D..0N..(.
-000023a0: 36c0 95cb 5211 fac0 fad1 2336 1823 97a1  6...R.....#6.#..
-000023b0: 64c2 39dc 43d8 bac3 7a57 b15f f7fa d7c7  d.9.C...zW._....
-000023c0: bba9 14ee 85d2 22c8 ad60 9ae9 eb11 bf30  ......"..`.....0
-000023d0: f8ba 53e5 9c59 6bd6 5b03 2b96 dbee c7cf  ..S..Yk.[.+.....
-000023e0: dcef 61dd fad5 1372 4515 c3d2 11b9 bc1a  ..a....rE.......
-000023f0: 66dc 3103 860d bcbe 728e 0e93 d07a 1e9a  f.1.....r....z..
-00002400: f0d1 7f50 4b03 0414 0000 0008 00d5 8599  ...PK...........
-00002410: 5832 eb97 58f4 0100 0047 0400 0019 0000  X2..X....G......
-00002420: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00002430: 6865 6574 3131 2e78 6d6c 8d54 db6e db30  heet11.xml.T.n.0
-00002440: 0cfd 1543 cf45 9514 eb05 816d a049 daae  ...C.E.....m.I..
-00002450: c3b2 15cd 9661 4f81 62d3 b110 59f4 247a  .....aO.b...Y.$z
-00002460: 5eff 7e94 9da4 e996 0c7b b278 7478 488a  ^.~......{.xtxH.
-00002470: a4e3 16dd c697 0014 fdaa 8cf5 8928 89ea  .............(..
-00002480: 9194 3e2b a152 fe1c 6bb0 7c53 a0ab 14b1  ..>+.R..k.|S....
-00002490: e9d6 d2d7 0e54 de39 5546 5e0c 0657 b252  .....T.9UF^..W.R
-000024a0: da8a 34ee b027 97c6 d890 d116 9e5c e49b  ..4..'.......\..
-000024b0: aa52 ee65 0c06 db44 0cc5 0e78 d6eb 923a  .R.e...D...x...:
-000024c0: 40a6 71ad d630 07fa 5ab3 039b 72af 93eb  @.q..0..Z...r...
-000024d0: 0aac d768 2307 4522 6e87 a387 dea3 632c  ...h#.E"n.....c,
-000024e0: 34b4 fee0 1c85 6256 889b 603c e689 1884  4.....bV..`<....
-000024f0: 9cc0 4046 4142 f1e7 274c c098 a0c4 99fc  ..@FAB..'L......
-00002500: d88a 8ad7 a0c1 f3f0 bc93 bfef eae7 f456  ...............V
-00002510: cac3 04cd 379d 5399 881b 11e5 50a8 c6d0  ....7.S.....P...
-00002520: 33b6 ef61 5bd3 e56b 8a53 452a 8d1d b691  3..a[..k.SE*....
-00002530: 0bc5 a671 160e 2124 13b5 0d8f 3427 c7b8  ...q..!$....4'..
-00002540: e648 9412 785a e6ec b32c b481 a5c1 4c11  .H..xZ...,....L.
-00002550: ba58 12e7 1418 32db 2a8c ff53 a1ef db11  .X....2.*..S....
-00002560: 81c9 2901 9d1f 614f 4fb1 adaa e008 ffee  ..)...aOO.......
-00002570: 143f 079f 395d 877e 1c71 bb3f 5995 5afb  .?..9].~.q.?Y.Z.
-00002580: 23fc 877f be82 6bac 05b7 f440 a4ed 9ffe  #.....k....@....
-00002590: 927b b26b 74df a4f0 680b 6534 7f39 3b1f  .{.kt...h.e4.9;.
-000025a0: 65d8 58ea 9bf6 f66a 3738 e38b d178 3878  e.X....j78...x8x
-000025b0: 7773 797d c5c3 5462 3b75 584f b1b5 61f0  wsy}..Tb;uXO..a.
-000025c0: 3ae0 d1d6 0dcd c07b 9eef 3d78 e71c ba43  :......{..=x...C
-000025d0: 5019 de8d b151 76d3 ed03 bdd4 8c1b ed89  P....Qv.........
-000025e0: 2387 fe35 460d 53f1 65be 38fb 7e3b fb78  #..5F.S.e.8.~;.x
-000025f0: f661 fef9 9388 e5fe 2696 6fd3 fb0b f0fd  .a......&.o.....
-00002600: 82cd 945b 6bae cb40 c165 0dce af79 4c5d  ...[k..@.e...yL]
-00002610: 3fb1 bd41 5877 09ac 9008 abee 58f2 a283  ?..AXw......X...
-00002620: 0b04 be2f 1069 6f84 8dd9 ff3b d2df 504b  .../.io....;..PK
-00002630: 0304 1400 0000 0800 d585 9958 6565 3fda  ...........Xee?.
-00002640: 0d02 0000 c104 0000 1900 0000 786c 2f77  ............xl/w
-00002650: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002660: 322e 786d 6c7d 546d 6fe2 300c fe2b 553e  2.xml}Tmo.0..+U>
-00002670: a305 a6db 8b50 a934 602f 4887 346d daee  .....P.4`/H.4m..
-00002680: 230a a94b 23d2 244b dceb eddf 9fd3 0263  #..K#.$K.......c
-00002690: 7785 4f8d 9ff8 b1fd 3876 d3c6 fa6d 2801  w.O.....8v...m(.
-000026a0: 30f9 5369 1326 ac44 7463 ce83 2ca1 12e1  0.Si.&.Dtc..,...
-000026b0: c23a 3074 5358 5f09 24d3 6f78 701e 44de  .:0tSX_.$.oxp.D.
-000026c0: 922a cd2f 87c3 6b5e 0965 5896 b6d8 b3cf  .*./..k^.eX.....
-000026d0: 525b a356 069e 7d12 eaaa 12fe 730a da36  R[.V..}.....s..6
-000026e0: 1336 627b e045 6d4a 6c01 9ea5 4e6c e015  .6b{.EmJl...Nl..
-000026f0: f0cd 1181 4c7e 8893 ab0a 4c50 d624 1e8a  ....L~....LP.$..
-00002700: 09bb 1b8d 171d a3f5 7857 d084 a373 12c5  ........xW...s..
-00002710: acad dd46 6391 4fd8 30d6 041a 24c6 1082  ...Fc.O.0...$...
-00002720: 3ebf 6106 5ac7 4854 c9c7 2e28 fb4a 1a99  >.a.Z.HT...(.J..
-00002730: c7e7 7df8 8756 3f95 b716 0166 56ff 5239  ..}..V?....fV.R9
-00002740: 9613 76cb 921c 0a51 6b7c b1cd 13ec 345d  ..v....Qk|....4]
-00002750: 7d95 3817 28b2 d4db 26f1 516c 96ca 7888  }.8.(...&.Ql..x.
-00002760: 29c9 5199 d8a4 57f4 842b ca84 1942 c055  ).Q...W..+...B.U
-00002770: 0528 72e2 a51c a994 78c1 e58e 383d 4b74  .(r.....x...8=Kt
-00002780: e083 357d bcd9 599e 244d a187 353f cb0a  ..5}..Y.$M..5?..
-00002790: b542 5805 0752 154a 8ad8 e29e 18f7 a762  .BX..R.J.......b
-000027a0: a8bc c7fb e194 b711 15f4 f83f 9ef2 cf21  ...........?...!
-000027b0: 48af dc89 a29e 4e0a 139b be46 2cce 36c2  H.....N....F,.6.
-000027c0: d7c6 805f 0540 54e6 5f3e a7b7 df0f 5437  ..._.@T._>....T7
-000027d0: 0cf1 69df 8556 79db b290 485b 1bec 86e3  ..i..Vy...H[....
-000027e0: fbd5 7e40 a797 e3e9 68f8 e3f6 eae6 9a86  ..~@....h.......
-000027f0: b6b4 cddc 5b37 b78d 8903 de02 0be3 6a5c  ....[7........j\
-00002800: 4208 b447 07f0 de7b eb8f 41a1 6907 a75a  B..G...{..A.i..Z
-00002810: 986d bb77 f8e9 08d7 2a20 658e fb5d 6b31  .m.w....* e..]k1
-00002820: cad8 9dd6 8319 e9a4 27d5 839f b44c 6f6e  ........'....Lon
-00002830: b004 590a 439e 4ab2 941f 7c53 febd e0ff  ..Y.C.J...|S....
-00002840: 80d0 adf6 52f8 8d22 a51a 0a12 3abc b8a1  ....R.."....:...
-00002850: 05f1 ddae 7406 5ad7 96b4 b688 b66a 8f25  ....t.Z......j.%
-00002860: fd62 c047 07ba 2fac c583 1177 f5f0 d7ca  .b.G../....w....
-00002870: fe02 504b 0304 1400 0000 0800 d585 9958  ..PK...........X
-00002880: 6565 3fda 0d02 0000 c104 0000 1900 0000  ee?.............
-00002890: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000028a0: 6565 7431 332e 786d 6c7d 546d 6fe2 300c  eet13.xml}Tmo.0.
-000028b0: fe2b 553e a305 a6db 8b50 a934 602f 4887  .+U>.....P.4`/H.
-000028c0: 346d daee 230a a94b 23d2 244b dceb eddf  4m..#..K#.$K....
-000028d0: 9fd3 0263 7785 4f8d 9ff8 b1fd 3876 d3c6  ...cw.O.....8v..
-000028e0: fa6d 2801 30f9 5369 1326 ac44 7463 ce83  .m(.0.Si.&.Dtc..
-000028f0: 2ca1 12e1 c23a 3074 5358 5f09 24d3 6f78  ,....:0tSX_.$.ox
-00002900: 701e 44de 922a cd2f 87c3 6b5e 0965 5896  p.D..*./..k^.eX.
-00002910: b6d8 b3cf 525b a356 069e 7d12 eaaa 12fe  ....R[.V..}.....
-00002920: 730a da36 1336 627b e045 6d4a 6c01 9ea5  s..6.6b{.EmJl...
-00002930: 4e6c e015 f0cd 1181 4c7e 8893 ab0a 4c50  Nl......L~....LP
-00002940: d624 1e8a 09bb 1b8d 171d a3f5 7857 d084  .$..........xW..
-00002950: a373 12c5 acad dd46 6391 4fd8 30d6 041a  .s.....Fc.O.0...
-00002960: 24c6 1082 3ebf 6106 5ac7 4854 c9c7 2e28  $...>.a.Z.HT...(
-00002970: fb4a 1a99 c7e7 7df8 8756 3f95 b716 0166  .J....}..V?....f
-00002980: 56ff 5239 9613 76cb 921c 0a51 6b7c b1cd  V.R9..v....Qk|..
-00002990: 13ec 345d 7d95 3817 28b2 d4db 26f1 516c  ..4]}.8.(...&.Ql
-000029a0: 96ca 7888 29c9 5199 d8a4 57f4 842b ca84  ..x.).Q...W..+..
-000029b0: 1942 c055 0528 72e2 a51c a994 78c1 e58e  .B.U.(r.....x...
-000029c0: 383d 4b74 e083 357d bcd9 599e 244d a187  8=Kt..5}..Y.$M..
-000029d0: 353f cb0a b542 5805 0752 154a 8ad8 e29e  5?...BX..R.J....
-000029e0: 18f7 a762 a8bc c7fb e194 b711 15f4 f83f  ...b...........?
-000029f0: 9ef2 cf21 48af dc89 a29e 4e0a 139b be46  ...!H.....N....F
-00002a00: 2cce 36c2 d7c6 805f 0540 54e6 5f3e a7b7  ,.6...._.@T._>..
-00002a10: df0f 5437 0cf1 69df 8556 79db b290 485b  ..T7..i..Vy...H[
-00002a20: 1bec 86e3 fbd5 7e40 a797 e3e9 68f8 e3f6  ......~@....h...
-00002a30: eae6 9a86 b6b4 cddc 5b37 b78d 8903 de02  ........[7......
-00002a40: 0be3 6a5c 4208 b447 07f0 de7b eb8f 41a1  ..j\B..G...{..A.
-00002a50: 6907 a75a 986d bb77 f8e9 08d7 2a20 658e  i..Z.m.w....* e.
-00002a60: fb5d 6b31 cad8 9dd6 8319 e9a4 27d5 839f  .]k1........'...
-00002a70: b44c 6f6e b004 590a 439e 4ab2 941f 7c53  .Lon..Y.C.J...|S
-00002a80: febd e0ff 80d0 adf6 52f8 8d22 a51a 0a12  ........R.."....
-00002a90: 3abc b8a1 05f1 ddae 7406 5ad7 96b4 b688  :.......t.Z.....
-00002aa0: b66a 8f25 fd62 c047 07ba 2fac c583 1177  .j.%.b.G../....w
-00002ab0: f5f0 d7ca fe02 504b 0304 1400 0000 0800  ......PK........
-00002ac0: d585 9958 953b a42f 1101 0000 c801 0000  ...X.;./........
-00002ad0: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-00002ae0: 732f 7368 6565 7431 342e 786d 6c4d 51cb  s/sheet14.xmlMQ.
-00002af0: 6ec3 2010 fc15 8b0f 084e a53e 14d9 96d2  n. ......N.>....
-00002b00: 5455 7ba8 14a5 6a7b c6f1 da46 0196 c2ba  TU{...j{...F....
-00002b10: 6eff be80 6327 2776 7677 8619 2846 7427  n...c''vvw..(Ft'
-00002b20: df03 50f6 ab95 f125 eb89 ec86 737f ec41  ..P....%....s..A
-00002b30: 0bbf 420b 264c 5a74 5a50 80ae e3de 3a10  ..B.&LZtZP....:.
-00002b40: 4d22 69c5 6ff2 fc8e 6b21 0dab 8ad4 dbbb  M"i.o...k!......
-00002b50: aac0 8194 34b0 7799 1fb4 16ee ef11 148e  ....4.w.........
-00002b60: 255b b3b9 7190 5d4f a9c1 abc2 8a0e de81  %[..q.]O........
-00002b70: 3e6c 2004 c817 9d46 6a30 5ea2 c91c b425  >l ....Fj0^....%
-00002b80: dbae 37db 8991 363e 258c feaa ce62 981a  ..7...6>%....b..
-00002b90: f114 c16b 53b2 3c7a 0205 478a 1222 1c3f  ...kS.<z..G..".?
-00002ba0: b003 a5a2 5270 f27d 1665 974b 23f3 ba9e  ....Rp.}.e.K#...
-00002bb0: e59f 53fe 60af 161e 76a8 be64 437d c91e  ..S.`...v..dC}..
-00002bc0: 58d6 402b 0645 071c 5fe0 9ce9 f662 f149  X.@+.E.._....b.I
-00002bd0: 9098 13be 09d7 49e3 3305 6dd8 ca57 f761  ......I.3.m..W.a
-00002be0: cf4d 9409 10da f422 3512 a14e 651f 5e1a  .M....."5..Ne.^.
-00002bf0: 5c5c 08f3 1691 1610 2d2f 9f57 fd03 504b  \\......-/.W..PK
-00002c00: 0304 1400 0000 0800 d585 9958 6565 3fda  ...........Xee?.
-00002c10: 0d02 0000 c104 0000 1900 0000 786c 2f77  ............xl/w
-00002c20: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00002c30: 352e 786d 6c7d 546d 6fe2 300c fe2b 553e  5.xml}Tmo.0..+U>
-00002c40: a305 a6db 8b50 a934 602f 4887 346d daee  .....P.4`/H.4m..
-00002c50: 230a a94b 23d2 244b dceb eddf 9fd3 0263  #..K#.$K.......c
-00002c60: 7785 4f8d 9ff8 b1fd 3876 d3c6 fa6d 2801  w.O.....8v...m(.
-00002c70: 30f9 5369 1326 ac44 7463 ce83 2ca1 12e1  0.Si.&.Dtc..,...
-00002c80: c23a 3074 5358 5f09 24d3 6f78 701e 44de  .:0tSX_.$.oxp.D.
-00002c90: 922a cd2f 87c3 6b5e 0965 5896 b6d8 b3cf  .*./..k^.eX.....
-00002ca0: 525b a356 069e 7d12 eaaa 12fe 730a da36  R[.V..}.....s..6
-00002cb0: 1336 627b e045 6d4a 6c01 9ea5 4e6c e015  .6b{.EmJl...Nl..
-00002cc0: f0cd 1181 4c7e 8893 ab0a 4c50 d624 1e8a  ....L~....LP.$..
-00002cd0: 09bb 1b8d 171d a3f5 7857 d084 a373 12c5  ........xW...s..
-00002ce0: acad dd46 6391 4fd8 30d6 041a 24c6 1082  ...Fc.O.0...$...
-00002cf0: 3ebf 6106 5ac7 4854 c9c7 2e28 fb4a 1a99  >.a.Z.HT...(.J..
-00002d00: c7e7 7df8 8756 3f95 b716 0166 56ff 5239  ..}..V?....fV.R9
-00002d10: 9613 76cb 921c 0a51 6b7c b1cd 13ec 345d  ..v....Qk|....4]
-00002d20: 7d95 3817 28b2 d4db 26f1 516c 96ca 7888  }.8.(...&.Ql..x.
-00002d30: 29c9 5199 d8a4 57f4 842b ca84 1942 c055  ).Q...W..+...B.U
-00002d40: 0528 72e2 a51c a994 78c1 e58e 383d 4b74  .(r.....x...8=Kt
-00002d50: e083 357d bcd9 599e 244d a187 353f cb0a  ..5}..Y.$M..5?..
-00002d60: b542 5805 0752 154a 8ad8 e29e 18f7 a762  .BX..R.J.......b
-00002d70: a8bc c7fb e194 b711 15f4 f83f 9ef2 cf21  ...........?...!
-00002d80: 48af dc89 a29e 4e0a 139b be46 2cce 36c2  H.....N....F,.6.
-00002d90: d7c6 805f 0540 54e6 5f3e a7b7 df0f 5437  ..._.@T._>....T7
-00002da0: 0cf1 69df 8556 79db b290 485b 1bec 86e3  ..i..Vy...H[....
-00002db0: fbd5 7e40 a797 e3e9 68f8 e3f6 eae6 9a86  ..~@....h.......
-00002dc0: b6b4 cddc 5b37 b78d 8903 de02 0be3 6a5c  ....[7........j\
-00002dd0: 4208 b447 07f0 de7b eb8f 41a1 6907 a75a  B..G...{..A.i..Z
-00002de0: 986d bb77 f8e9 08d7 2a20 658e fb5d 6b31  .m.w....* e..]k1
-00002df0: cad8 9dd6 8319 e9a4 27d5 839f b44c 6f6e  ........'....Lon
-00002e00: b004 590a 439e 4ab2 941f 7c53 febd e0ff  ..Y.C.J...|S....
-00002e10: 80d0 adf6 52f8 8d22 a51a 0a12 3abc b8a1  ....R.."....:...
-00002e20: 05f1 ddae 7406 5ad7 96b4 b688 b66a 8f25  ....t.Z......j.%
-00002e30: fd62 c047 07ba 2fac c583 1177 f5f0 d7ca  .b.G../....w....
-00002e40: fe02 504b 0304 1400 0000 0800 d585 9958  ..PK...........X
-00002e50: 6565 3fda 0d02 0000 c104 0000 1900 0000  ee?.............
-00002e60: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00002e70: 6565 7431 362e 786d 6c7d 546d 6fe2 300c  eet16.xml}Tmo.0.
-00002e80: fe2b 553e a305 a6db 8b50 a934 602f 4887  .+U>.....P.4`/H.
-00002e90: 346d daee 230a a94b 23d2 244b dceb eddf  4m..#..K#.$K....
-00002ea0: 9fd3 0263 7785 4f8d 9ff8 b1fd 3876 d3c6  ...cw.O.....8v..
-00002eb0: fa6d 2801 30f9 5369 1326 ac44 7463 ce83  .m(.0.Si.&.Dtc..
-00002ec0: 2ca1 12e1 c23a 3074 5358 5f09 24d3 6f78  ,....:0tSX_.$.ox
-00002ed0: 701e 44de 922a cd2f 87c3 6b5e 0965 5896  p.D..*./..k^.eX.
-00002ee0: b6d8 b3cf 525b a356 069e 7d12 eaaa 12fe  ....R[.V..}.....
-00002ef0: 730a da36 1336 627b e045 6d4a 6c01 9ea5  s..6.6b{.EmJl...
-00002f00: 4e6c e015 f0cd 1181 4c7e 8893 ab0a 4c50  Nl......L~....LP
-00002f10: d624 1e8a 09bb 1b8d 171d a3f5 7857 d084  .$..........xW..
-00002f20: a373 12c5 acad dd46 6391 4fd8 30d6 041a  .s.....Fc.O.0...
-00002f30: 24c6 1082 3ebf 6106 5ac7 4854 c9c7 2e28  $...>.a.Z.HT...(
-00002f40: fb4a 1a99 c7e7 7df8 8756 3f95 b716 0166  .J....}..V?....f
-00002f50: 56ff 5239 9613 76cb 921c 0a51 6b7c b1cd  V.R9..v....Qk|..
-00002f60: 13ec 345d 7d95 3817 28b2 d4db 26f1 516c  ..4]}.8.(...&.Ql
-00002f70: 96ca 7888 29c9 5199 d8a4 57f4 842b ca84  ..x.).Q...W..+..
-00002f80: 1942 c055 0528 72e2 a51c a994 78c1 e58e  .B.U.(r.....x...
-00002f90: 383d 4b74 e083 357d bcd9 599e 244d a187  8=Kt..5}..Y.$M..
-00002fa0: 353f cb0a b542 5805 0752 154a 8ad8 e29e  5?...BX..R.J....
-00002fb0: 18f7 a762 a8bc c7fb e194 b711 15f4 f83f  ...b...........?
-00002fc0: 9ef2 cf21 48af dc89 a29e 4e0a 139b be46  ...!H.....N....F
-00002fd0: 2cce 36c2 d7c6 805f 0540 54e6 5f3e a7b7  ,.6...._.@T._>..
-00002fe0: df0f 5437 0cf1 69df 8556 79db b290 485b  ..T7..i..Vy...H[
-00002ff0: 1bec 86e3 fbd5 7e40 a797 e3e9 68f8 e3f6  ......~@....h...
-00003000: eae6 9a86 b6b4 cddc 5b37 b78d 8903 de02  ........[7......
-00003010: 0be3 6a5c 4208 b447 07f0 de7b eb8f 41a1  ..j\B..G...{..A.
-00003020: 6907 a75a 986d bb77 f8e9 08d7 2a20 658e  i..Z.m.w....* e.
-00003030: fb5d 6b31 cad8 9dd6 8319 e9a4 27d5 839f  .]k1........'...
-00003040: b44c 6f6e b004 590a 439e 4ab2 941f 7c53  .Lon..Y.C.J...|S
-00003050: febd e0ff 80d0 adf6 52f8 8d22 a51a 0a12  ........R.."....
-00003060: 3abc b8a1 05f1 ddae 7406 5ad7 96b4 b688  :.......t.Z.....
-00003070: b66a 8f25 fd62 c047 07ba 2fac c583 1177  .j.%.b.G../....w
-00003080: f5f0 d7ca fe02 504b 0304 1400 0000 0800  ......PK........
-00003090: d585 9958 2bcd 4145 fa01 0000 7604 0000  ...X+.AE....v...
-000030a0: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
-000030b0: 732f 7368 6565 7431 372e 786d 6c85 546d  s/sheet17.xml.Tm
-000030c0: 8fda 300c fe2b 553f 4f17 38ed 5e84 4a25  ..0..+U?O.8.^.J%
-000030d0: a030 d076 12ba 6ab7 8f28 b486 46a4 49e7  .0.v..j..(..F.I.
-000030e0: b8eb eedf cf69 81e3 b672 fbd2 c44f fcd8  .....i...r...O..
-000030f0: 8f1b 3b51 63f1 e00a 000a 7e97 dab8 7158  ..;Qc.....~...qX
-00003100: 1055 2321 5c56 4029 dd8d adc0 f0c9 ce62  .U#!\V@).......b
-00003110: 2989 4ddc 0b57 21c8 bc25 955a dc0e 06f7  ).M..W!..%.Z....
-00003120: a294 ca84 71d4 626b 8c23 5b93 5606 d618  ....q.bk.#[.V...
-00003130: b8ba 2c25 be4e 41db 661c 0ec3 13f0 acf6  ..,%.NA.f.......
-00003140: 05b5 8088 a34a ee21 05fa 5e31 814d 718e  .....J.!..^1.Mq.
-00003150: 93ab 128c 53d6 0408 bb71 3819 8e96 1da3  ....S....q8.....
-00003160: f578 51d0 b88b 7de0 8bd9 5a7b f0c6 2a1f  .xQ...}...Z{..*.
-00003170: 8703 af09 3464 e443 485e 7ec1 0cb4 f691  ....4d.CH^~.....
-00003180: 58c9 cf63 d0f0 2da9 675e ee4f e117 6dfd  X..c..-.g^.O..m.
-00003190: 2c6f 2b1d ccac fea1 722a c6e1 6318 e4b0  ,o+.....r*..c...
-000031a0: 93b5 a667 db2c e158 d3dd 9bc4 4492 8c23  ...g.,.X....D..#
-000031b0: b44d 80be d838 cafc c6a7 6447 65fc 4f4a  .M...8....dGe.OJ
-000031c0: 0919 579c 8962 0247 1b57 2b82 8dca 2341  ..W..b.G.W+...#A
-000031d0: 2cc5 1f88 ec48 9c7e 48cc 585b 0f69 f65f  ,....H.~H.X[.i._
-000031e0: d206 c171 0d3d dce4 1ab7 57de fc9a b791  ...q.=....W.....
-000031f0: 659f b2c5 35ff 1c5c 86aa f2d7 d643 fb72  e...5..\.....C.r
-00003200: b520 b977 3dfe cb0f 7f00 d6c6 006e 1c10  . .w=........n..
-00003210: 29f3 375f f0d5 9dfa a1bb cb9c bf2f 522b  ).7_........./R+
-00003220: 5e59 9d0b 325b 1bea eef6 fdd1 a9bf 66b7  ^Y..2[........f.
-00003230: a3d9 70f0 f9f1 eee1 9e7b aeb0 4d82 b64a  ..p......{..M..J
-00003240: 6c63 7c7f b6c0 ca54 353d 8173 3c06 6770  lc|....T5=.s<.gp
-00003250: 8e68 f112 949a 4768 aaa5 39b4 6343 af15  .h....Gh..9.cC..
-00003260: e35a 39e2 cc7e 3c6b 2d87 71b8 9ea4 e93c  .Z9..~<k-.q....<
-00003270: f9b4 98ac bef1 927e 5dad d7f3 248c c4d9  .......~]...$...
-00003280: 2312 ef65 fe03 b86e 1e9f 24ee 15d7 a761  #..e...n..$....a
-00003290: c7e5 0d6e 1eb8 abb1 6bf0 ce20 5bb5 42b6  ...n....k.. [.B.
-000032a0: 96c8 96ed b6e0 7701 d03b f0f9 ce5a 3a1b  ......w..;...Z:.
-000032b0: 7ec0 ce4f 4dfc 0750 4b03 0414 0000 0008  ~..OM..PK.......
-000032c0: 00d5 8599 5865 2fbe fe7e 0200 0081 0600  ....Xe/..~......
-000032d0: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-000032e0: 7473 2f73 6865 6574 3138 2e78 6d6c bd55  ts/sheet18.xml.U
-000032f0: db6e db30 0cfd 95c0 cf46 9d04 eb05 8163  .n.0.....F.....c
-00003300: a069 dab5 5b0b 0c2d d63d 068a cdc4 4224  .i..[..-.=....B$
-00003310: 51a3 984b ff7e 94d3 a65d 61b7 7bda 8b2d  Q..K.~...]a.{..-
-00003320: 1ef1 5087 3445 e75b a455 a801 b8b7 b3c6  ..P.4E.[.U......
-00003330: 8571 5233 fb51 9685 b206 abc2 117a 70b2  .qR3.Q.......zp.
-00003340: b340 b28a c5a4 6516 3c81 aa1a 9235 d9b0  .@....e.<....5..
-00003350: df3f c9ac d22e 29f2 06fb 4145 8e6b 36da  .?....)...AE.k6.
-00003360: c10f ea85 b5b5 8a9e 2660 703b 4e06 c90b  ........&`p;N...
-00003370: 70af 9735 3740 56e4 5e2d e101 f8a7 1782  p..57@V.^-......
-00003380: 98d9 214e a52d b8a0 d1f5 0816 e3e4 7c30  ..!N.-........|0
-00003390: badd 331a 8f47 0ddb f066 dd8b c9cc 1157  ..3..G...f.....W
-000033a0: d1b8 a9c6 493f 6a02 0325 c710 4a5e 1bb8  ....I?j..%..J^..
-000033b0: 0063 6224 51f2 fb39 68f2 7a68 64be 5dbf  .cb$Q..9h.zhd.].
-000033c0: 84bf 6af2 1779 7315 e002 cd2f 5d71 3d4e  ..j..ys..../]q=N
-000033d0: ce92 5e05 0bb5 367c 8fdb 6b78 cee9 f855  ..^...6|..kx...U
-000033e0: e254 b12a 72c2 6d8f 62b2 455e c645 3c52  .T.*r.m.b.E^.E<R
-000033f0: 1cb5 8b45 7a60 125c cb49 5c94 683d 3a70  ...Ez`.\.I\.h=:p
-00003400: 1cf2 8c45 4744 b3f2 9935 e962 3104 9e81  ...EGD...5.b1...
-00003410: dbb4 702e 3ee4 d0da 39a0 9953 165a b8d3  ..p.>...9..S.Z..
-00003420: cfb8 33af 48a8 0cd4 26f7 f213 b9ac 5943  ..3.H...&.....YC
-00003430: 1bf1 ea43 6229 1f60 4610 a4e6 6de4 af9d  ...Cb).`F...m...
-00003440: 6469 a5c0 cafa 16d2 7517 4957 2dde 375d  di......u.IW-.7]
-00003450: de1d 75fc d6e5 5f41 2849 fbd8 9c2d b4ef  ..u..._A(I...-..
-00003460: 9d99 a865 5be6 b7ff f2a9 0330 6bf7 9e9f  ...e[......0k...
-00003470: 4983 be74 fdbe 632b 793e 2aa3 e52d ea42  I..t..c+y>*..-.B
-00003480: afc4 b593 e0c3 e4fd d6e1 160d 47e7 83fe  ............G...
-00003490: 97b3 e3d3 13b9 5935 6ea7 847e 8a5b 176f  ......Y5n..~.[.o
-000034a0: 6103 dc38 bfe6 3b08 412e fb01 bc24 427a  a..8..;.A....$Bz
-000034b0: 0b2a 2383 6262 945b 35c3 819f bce0 4607  .*#.bb.[5.....F.
-000034c0: 9693 e310 5a1b 3528 1245 2195 dedb a5b0  ....Z.5(.E!.....
-000034d0: f3e2 ab18 e929 d5d6 136e 24bb b8b5 4472  .....)...n$...Dr
-000034e0: e99c 215d bb00 2501 a7c4 bbd5 7298 ea12  ..!]..%.....r...
-000034f0: 20a4 a5b2 69f0 b882 d4a2 01e1 a50c 3bb6   ...i.........;.
-00003500: da45 7a89 7595 c6c1 2783 aed2 250b 608c  .Ez.u...'...%.`.
-00003510: 9a23 edcf 2951 4ad9 8c94 90e4 d941 549e  .#..)QJ......AT.
-00003520: fd5d 99ae 4a4d 86a3 c9ff ab54 059b b4d4  .]..JM.....T....
-00003530: 69ec 8154 d2ac 3e56 fc0e 08fb d17c a768  i..T..>V.....|.h
-00003540: a9a5 090c 2ca4 07fa 47a7 32e0 683f ebf6  ....,...G.2.h?..
-00003550: 06a3 6f34 cc91 196d b3ac e517 0114 1d64  ..o4...m.......d
-00003560: 7f81 c807 23ce dac3 5fa7 f803 504b 0304  ....#..._...PK..
-00003570: 1400 0000 0800 d585 9958 e1b4 af0f 7901  .........X....y.
-00003580: 0000 4f03 0000 1900 0000 786c 2f77 6f72  ..O.......xl/wor
-00003590: 6b73 6865 6574 732f 7368 6565 7431 392e  ksheets/sheet19.
-000035a0: 786d 6c7d 53c9 4ec3 3010 fd95 c81f 5017  xml}S.N.0.....P.
-000035b0: 2416 a124 1294 f580 845a 01c7 ca4d 2689  $..$.....Z...M&.
-000035c0: 552f 613c 25f0 f78c d385 0a25 9c32 337e  U/a<%......%.23~
-000035d0: efcd 9ab4 f3b8 0e0d 0025 5fd6 b890 8986  .........%_.....
-000035e0: a8bd 9232 140d 5815 26be 05c7 2f95 47ab  ...2..X.&.../.G.
-000035f0: 885d ac65 6811 54d9 93ac 91a7 d3e9 b9b4  .].eh.T.........
-00003600: 4a3b 91a7 7dec 05f3 d46f c868 072f 9884  J;..}....o.h./..
-00003610: 8db5 0abf 6fc0 f82e 1327 621f 98eb baa1  ....o....'b.....
-00003620: 3e20 f3b4 5535 2c80 5e5b 26b0 2b0f 3aa5  > ..U5,.^[&.+.:.
-00003630: b6e0 82f6 2e41 a832 717d 72f5 b065 f488  .....A.2q}r..e..
-00003640: 370d 5d38 b293 d8cc cafb 7574 9eca 4c4c  7.]8......ut..LL
-00003650: 634d 60a0 a028 a1f8 f309 3330 262a 7125  cM`..(....30&*q%
-00003660: 1f3b 51f1 9b34 328f edbd fc7d df3f 97b7  .;Q..42....}.?..
-00003670: 5201 66de bceb 929a 4c5c 8aa4 844a 6d0c  R.f.....L\...Jm.
-00003680: cd7d f708 bb9e ce7e 4bbc 55a4 f214 7d97  .}.....~K.U...}.
-00003690: 606c 364f 8b68 c494 0cd4 2e0e 6941 c871  `l6O.h......iA.q
-000036a0: cd99 2827 08b4 2c38 c552 97a9 24ae 24c6  ..('..,8.R..$.$.
-000036b0: 65b1 e3dd 8cf1 da75 1880 cfc6 e083 e2b7  e......u........
-000036c0: 6368 a72c 0ce0 efc6 f025 8402 751b 673e  ch.,.....%..u.g>
-000036d0: 40bb 1fed 5dd5 434d 3cfc 3b2b dc38 07b8  @...].CM<.;+.8..
-000036e0: 0c40 a4dd 5fbe e4b9 ef97 b95d 443c b467  .@.._......]D<.g
-000036f0: 85b5 7621 3150 b1ee 7472 c1eb c2ed e6b6  ..v!1P..tr......
-00003700: 0ef9 b63f cc95 27f2 b637 1b3e 78c0 08e0  ...?..'..7.>x...
-00003710: f7ca 7b3a 38f1 720e ff50 fe03 504b 0304  ..{:8.r..P..PK..
-00003720: 1400 0000 0800 d585 9958 25f9 f458 ac01  .........X%..X..
-00003730: 0000 4d04 0000 1900 0000 786c 2f77 6f72  ..M.......xl/wor
-00003740: 6b73 6865 6574 732f 7368 6565 7432 302e  ksheets/sheet20.
-00003750: 786d 6c7d 946d 4fdc 300c c7bf 4ad5 0f40  xml}.mO.0...J..@
-00003760: 8e49 7b10 6a2b 8d63 0c36 2621 10db cb53  .I{.j+.c.6&!...S
-00003770: ae75 dbe8 9238 735c cabe fd92 de03 684a  .u...8s\......hJ
-00003780: f6aa b6f3 ff39 7664 b79a 9176 7e04 e0e2  .....9vd...v~...
-00003790: c568 ebeb 7264 7617 42f8 7604 23fd 193a  .h..rdv.B.v.#..:
-000037a0: b0e1 a447 3292 834b 83f0 8e40 760b 64b4  ...G2..K...@v.d.
-000037b0: 78b7 5a7d 1046 2a5b 36d5 12bb a7a6 c289  x.Z}.F*[6.......
-000037c0: b5b2 704f 859f 8c91 f4e7 1234 ce75 795e  ..pO.......4.uy^
-000037d0: 1e03 0f6a 1879 0988 a672 7280 47e0 2717  ...j.y...rr.G.'.
-000037e0: 80e0 8a53 9e4e 19b0 5ea1 2d08 faba fc7c  ...S.N..^.-....|
-000037f0: 7e71 b727 16c5 4f05 b37f 6317 b199 2de2  ~q.'..O...c...-.
-00003800: 2e3a b75d 5dae 624d a0a1 e598 4286 cf33  .:.]].bM....B..3
-00003810: ac41 eb98 2954 f2fb 90b4 7cbd 3492 6fed  .A..)T....|.4.o.
-00003820: 63fa eba5 ff50 de56 7a58 a3fe a53a 1eeb  c....P.VzX...:..
-00003830: f253 5974 d0cb 49f3 03ce 3770 e8e9 fd6b  .SYt..I...7p...k
-00003840: 8957 9265 5311 ce05 c566 9baa 8d46 bc32  .W.eS....f...F.2
-00003850: 0895 8d8f f4c8 14e2 2adc c48d 9304 9637  ........*......7
-00003860: 6e57 090e 65c4 a068 0fd0 650e 3240 0374  nW..e..h..e.2@.t
-00003870: 6968 9d83 24c9 01c9 2690 abff 202f 09fd  ih..$...&... /..
-00003880: 979c 7eb2 1e5a 024e 30d7 3966 cb90 907f  ..~..Z.N0.9f....
-00003890: cdc9 9571 84cf ca0e 09e8 260b 7509 f56d  ...q......&.u..m
-000038a0: 4e6d a549 95f4 2da7 efc0 b7a4 5c9c b804  Nm.I..-.....\...
-000038b0: f63d 87b1 1c7c 427f 97d5 83e7 0d4d d602  .=...|B......M..
-000038c0: 6d3c 3087 37f8 8717 61ea 8ea3 bc1f c3b8  m<0.7...a.......
-000038d0: 663f 240d cafa 4243 1ff2 aece 3e86 61a5  f?$...BC....>.a.
-000038e0: fddc ee1d 46b7 ace5 1699 d12c e618 d61d  ....F......,....
-000038f0: 280a c279 8fc8 2727 eecd e90f d2fc 0550  (..y..''.......P
-00003900: 4b03 0414 0000 0008 00d5 8599 58d2 05f1  K...........X...
-00003910: 4652 0200 0047 0a00 000d 0000 0078 6c2f  FR...G.......xl/
-00003920: 7374 796c 6573 2e78 6d6c dd56 db8a db30  styles.xml.V...0
-00003930: 10fd 15e3 0fa8 9398 9ab8 2479 a821 5068  ..........$y.!Ph
-00003940: cbc2 ee43 5fe5 584e 04ba b8b2 bc24 fdfa  ...C_.XN.....$..
-00003950: 6a24 e7b6 9be3 52fa 569b e099 393a 3367  j$....R.V...9:3g
-00003960: a431 ceaa 7727 c99f 0f9c bbe4 a8a4 eed7  .1..w'..........
-00003970: e9c1 b9ee 5396 f5bb 0357 acff 603a ae3d  ....S....W..`:.=
-00003980: d21a ab98 f3ae dd67 7d67 396b 7a22 2999  .......g}g9kz").
-00003990: 2d66 b322 534c e874 b3d2 83da 2ad7 273b  -f."SL.t....*.';
-000039a0: 3368 b74e 6769 926d 56ad d1d7 d03c 8d01  3h.Ngi.mV....<..
-000039b0: bf96 299e bc32 b94e 2b26 456d 455c cc94  ..)..2.N+&EmE\..
-000039c0: 90a7 185f 84c8 ce48 6313 e7d5 70a2 53a8  ..._...Hc...p.S.
-000039d0: ff15 17cc 4797 a48e b994 d0c6 8668 16cb  ....G........h..
-000039e0: 8447 ef13 0b29 2f2a 1669 0c6c 561d 738e  .G...)/*.i.lV.s.
-000039f0: 5bbd f54e 2485 e87b 6cb4 5f4e 9d57 b1b7  [..N$..{l._N.W..
-00003a00: ec34 5f7c 4c6f 18e1 e1cb d4c6 36dc deb5  .4_|Lo......6...
-00003a10: 1b43 9b95 e4ad 2386 15fb 4330 9ce9 e851  .C....#...C0...Q
-00003a20: 1be7 8c22 ab11 6c6f 348b 4ace b4d1 f0b9  ..."..lo4.J.....
-00003a30: 775c ca67 3aaf 1fed 5d81 639b c48d ffd2  w\.g:...].c.....
-00003a40: 843d a78e cfa6 5735 9a31 cde8 5081 db74  .=....W5.1..P..t
-00003a50: 31f9 bfe7 edc4 ab71 9f07 df90 0efe cfc1  1......q........
-00003a60: 38fe 6479 2b8e c13f b66f 045c 6a07 2577  8.dy+..?.o.\j.%w
-00003a70: e52f d184 4665 9d7e a711 9437 39ea 4148  ./..Fe.~...79.AH
-00003a80: 27f4 e81d 44d3 70fd be3b 9fdf b1da 0ff9  '...D.p..;......
-00003a90: 5d01 bfaa e12d 1ba4 7bb9 80eb f46a 7fe3  ]....-..{....j..
-00003aa0: 8d18 5479 59f5 448d 8dab aef6 573a ca79  ..TyY.D.....W:.y
-00003ab0: 719d 535f 4ce8 861f 7953 8dae ddd7 c14c  q.S_L...yS.....L
-00003ac0: bce1 cb8e 5760 bc85 b6e1 0210 6445 1040  ....W`......dE.@
-00003ad0: 04c2 5a50 0664 451e acf5 3ff6 b5c4 7d45  ..ZP.dE...?...}E
-00003ae0: 102a 5c3e 8696 98b5 c4ac c87b 0855 e186  .*\>.......{.U..
-00003af0: b500 abf4 1768 b92c f3bc 28e0 f656 d563  .....h.,..(..V.c
-00003b00: 1915 dcc3 a2a0 1f48 0815 1207 d6a2 6a7f  .......H......j.
-00003b10: bbf3 1303 3031 367f 980d 78ca 9363 035b  ....016...x..c.[
-00003b20: 9e18 51d8 f2c4 ce13 04f6 9038 6509 0600  ..Q........8e...
-00003b30: d622 0e3c 1438 5124 02d4 a251 03ac 3ca7  .".<.8Q$...Q..<.
-00003b40: 7386 0ae1 6b3e 0195 2584 6848 c1f4 1605  s...k>..%.hH....
-00003b50: daa8 826e 705e f025 caf3 b204 1081 4046  ...np^.%......@F
-00003b60: 9e43 885e d809 08ca 2021 10ca f3f8 217d  .C.^.... !....!}
-00003b70: f33d cbce dfb9 ecfa d771 f31b 504b 0304  .=.......q..PK..
-00003b80: 1400 0000 0800 d585 9958 b747 eb8a c000  .........X.G....
-00003b90: 0000 1602 0000 0b00 0000 5f72 656c 732f  .........._rels/
-00003ba0: 2e72 656c 739d 924b 6e02 310c 40af 1265  .rels..Kn.1.@..e
-00003bb0: 5f4c a9c4 0231 acd8 b043 880b b889 e7a3  _L...1...C......
-00003bc0: 99c4 9163 c4f4 f68d d8c0 2068 114b ff9e  ...c...... h.K..
-00003bd0: 9e2d af0f 34a0 761c 73db a56c c630 c45c  .-..4.v.s..l.0.\
-00003be0: d956 35ad 00b2 6b29 609e 71a2 582a 354b  .V5...k)`.q.X*5K
-00003bf0: 402d a134 90d0 f5d8 102c e6f3 25c8 2dc3  @-.4.....,..%.-.
-00003c00: 6ed6 b74c 73fc 49f4 0a91 ebba 73b4 6577  n..Ls.I.....s.ew
-00003c10: 0a14 f501 f8ae c39a 234a 435a d971 8033  ........#JCZ.q.3
-00003c20: 4bff cddc cf0a d49a 9daf acec fca7 35f0  K.............5.
-00003c30: a6cc f3f5 2090 a247 4570 2cf4 91a4 4c8b  .... ..GEp,...L.
-00003c40: 7694 af3e 9edd bea4 f3a5 6362 b478 dfe8  v..>......cb.x..
-00003c50: fff3 d0a8 143d f9bf 9d30 a589 d2d7 4509  .....=...0....E.
-00003c60: 266f b0f9 0550 4b03 0414 0000 0008 00d5  &o...PK.........
-00003c70: 8599 58b1 db15 1a3c 0200 00a2 0700 000f  ..X....<........
-00003c80: 0000 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
-00003c90: 6d6c 8d95 ed6e 9b30 1486 6f05 7101 03d2  ml...n.0..o.q...
-00003ca0: 266d a352 a94b bab5 da47 b250 f5bf 631f  &m.R.K...G.P..c.
-00003cb0: 8215 6323 fbd0 6cbd fad9 a074 2466 de7e  ..c#..l....t$f.~
-00003cc0: 818f adc7 efb1 1ef0 ed41 e9fd 56a9 7df4  .........A..V.}.
-00003cd0: b316 d2cc 751e 5788 cd3c 490c ada0 26e6  ....u.W..<I...&.
-00003ce0: 836a 40da b952 e99a a01d ea5d a2ca 9253  .j@..R.....]...S
-00003cf0: 582a dad6 2031 99a4 e92c d120 0872 254d  X*.. 1...,. .r%M
-00003d00: c51b 13f7 b4ff 6199 4603 61a6 02c0 5af4  ......a.F.a...Z.
-00003d10: a89a 7019 dfdd 1e93 ad75 940c 470a 81ba  ..p......u..G...
-00003d20: 9d5c d555 5e38 1ccc 9f05 6e18 bd72 c3b7  .\.U^8....n..r..
-00003d30: 5c70 fc95 c7dd bb80 38aa b9e4 357f 0396  \p......8...5...
-00003d40: c769 1c99 4a1d 1e95 e66f 4a22 1105 d54a  .i..J....oJ"...J
-00003d50: 883c cefa 8917 d0c8 a957 2e5c cc67 b235  .<.......W.\.g.5
-00003d60: 5d05 c976 e37a cee3 596a 8125 d706 bb15  ]..v.z..Yj.%....
-00003d70: 1d9f d890 af60 17f7 a316 d527 2e10 f492  .....`.....'....
-00003d80: 207c d6aa 6db8 dc75 18db 4632 e8a3 3b8a   |..m..u..F2..;.
-00003d90: e333 92a4 863c 7e06 830f 126d 3b6b a26d  .3...<~....m;k.m
-00003da0: c562 5c20 bbe0 89f5 e1d0 5207 adea 39b7  .b\ ......R...9.
-00003db0: 13fa 89f5 fc21 eb47 4b04 2ff9 0961 1220  .....!.GK./..a. 
-00003dc0: 4c3c 824b f30d 9030 8264 00b9 0840 2e46  L<.K...0.d...@.F
-00003dd0: 21f7 c600 0e08 9701 c2a5 47b8 a714 1a24  !.........G....$
-00003de0: 92c2 186b 1a60 4d47 d33c b01d 2c4f 5b9a  ...k.`MG.<..,O[.
-00003df0: 0520 330f b2d6 4095 64dc c939 805c 0520  . 3...@.d..9.\. 
-00003e00: 57a3 4916 c4c0 0070 1d00 5cff e358 ce50  W.I....p..\..X.P
-00003e10: 3701 d4cd 982a 4e3a d289 ecc3 b234 245e  7....*N:.....4$^
-00003e20: 3ada 5ad1 7284 a201 6a15 a4e4 eca4 b2a0  :.Z.r...j.......
-00003e30: c9be caef c021 23e4 72e6 cb7c 7a5c 1e2d  .....!#.r..|z\.-
-00003e40: 2475 e65b fd11 24ad 6aa2 f7a3 b090 df99  $u.[..$.j.......
-00003e50: 2f78 6163 31a2 9959 a8ba 11fc af19 43aa  /xac1..Y......C.
-00003e60: 67be eb2b 098f aa19 2585 7ccf 7ce1 8f4e  g..+....%.|.|..N
-00003e70: 6cc0 b462 f8f1 6521 e7b3 71e9 37ad 2cc0  l..b..e!..q.7.,.
-00003e80: 9833 2342 ee67 befc 0eb4 6ab1 694f d284  .3#B.g....j.iO..
-00003e90: accf 7ced bb34 5d4b eb2f c5c9 4f65 1232  ..|..4]K./..Oe.2
-00003ea0: 7ed2 1b9f 1c7f e00c 4a2e 817d b74c e326  ~.......J..}.L.&
-00003eb0: ec75 42ed 5de6 1ebd a897 53b7 79d9 0ab1  .uB.].....S.y...
-00003ec0: b0b5 95fc aa08 7bbf 118e d7d9 dd6f 504b  ......{......oPK
-00003ed0: 0304 1400 0000 0800 d585 9958 6741 6968  ...........XgAih
-00003ee0: 2101 0000 e90c 0000 1a00 0000 786c 2f5f  !...........xl/_
-00003ef0: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
-00003f00: 6c2e 7265 6c73 cdd7 cf8e 8230 10c7 f157  l.rels.....0...W
-00003f10: 217d 00cb 5445 dd88 a7bd 7835 be40 83c3  !}..TE....x5.@..
-00003f20: 9f08 94b4 dda8 6fbf 440e f8db ec61 2f66  ......o.D....a/f
-00003f30: e744 a684 e17b fa10 f627 6e6d 6c5c 1fea  .D...{...'nml\..
-00003f40: 6608 c9bd 6bfb 90ab 3ac6 e143 eb50 d4dc  f...k...:..C.P..
-00003f50: d9b0 7003 f7e3 9dd2 f9ce c671 f495 1e6c  ..p........q...l
-00003f60: 71b5 156b 93a6 99f6 af3b d461 ffba 3339  q..k.....;.a..39
-00003f70: 3f06 fecb 4657 964d c19f aef8 eab8 8fbf  ?...FW.M........
-00003f80: 2cd6 37e7 afa1 668e 2a39 5b5f 71cc 95be  ,.7...f.*9[_q...
-00003f90: b7f3 71d0 cf0b 2dc6 cd2a 395e 72e5 8f17  ..q...-..*9^r...
-00003fa0: 5289 feef 2203 4546 40d1 128a 9602 8a56  R...".EF@......V
-00003fb0: 50b4 1250 b486 a2b5 80a2 0c8a 3201 451b  P..P........2.E.
-00003fc0: 28da 0828 da42 d156 40d1 0e8a 7602 8a28  (..(.B.V@...v..(
-00003fd0: 4522 5309 4d3f d896 e036 21dc 2441 6e42  E"S.M?...6!.$AnB
-00003fe0: ba49 82dd 8478 9304 bd09 f926 097e 1302  .I...x.....&.~..
-00003ff0: 4e12 0427 249c 2418 4e88 3849 509c 9071  N..'$.$.N.8IP..q
-00004000: 92e0 b841 c7cd 5b1d 0ff1 d172 9883 a619  ...A..[....r....
-00004010: 03de 8a76 1c9f e5f9 fdcf 713a c44f 8799  ...v......q:.O..
-00004020: 98d6 f067 73f8 0650 4b03 0414 0000 0008  ...gs..PK.......
-00004030: 00d5 8599 5852 4472 5562 0100 000d 0e00  ....XRDrUb......
-00004040: 0013 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
-00004050: 7065 735d 2e78 6d6c cd97 dd4e c240 1085  pes].xml...N.@..
-00004060: 5fa5 e92d a1cb a2e2 4f80 1bf5 56b9 f005  _..-....O...V...
-00004070: d676 4a37 ec5f 7616 84b7 775a 8444 8322  .vJ7._v...wZ.D."
-00004080: c1c4 b9e9 a6dd 9973 bedd 494e d2f1 cb26  .......s..IN...&
-00004090: 0066 6b6b 1c4e f226 a570 2704 960d 5885  .fkk.N.&.p'...X.
-000040a0: 850f e068 a7f6 d1aa 44af 712e 822a 176a  ...h....D.q..*.j
-000040b0: 0e62 3818 8c44 e95d 0297 faa9 d5c8 a7e3  .b8..D.]........
-000040c0: 07a8 d5d2 a4ec 714d 9f51 7b37 c923 18cc  ......qM.Q{7.#..
-000040d0: b3fb 6d61 eb35 c955 0846 972a d1be 58b9  ..ma.5.U.F.*..X.
-000040e0: ea8b 4bff c3a1 a0ce ae06 1b1d b047 0579  ..K..........G.y
-000040f0: 260e 5a74 5bdf 3aec 1a9f 5710 a3ae 209b  &.Zt[.:...W... .
-00004100: a998 9e94 a532 b136 02d3 c600 163f 6b1c  .....2.6.....?k.
-00004110: a0f4 75ad 4ba8 7cb9 b4d4 5260 88a0 2a6c  ..u.K.|...R`..*l
-00004120: 0092 35c5 56b4 77c4 3ad1 25c3 f629 cf06  ..5.V.w.:.%..)..
-00004130: e864 7e74 a4d2 59f4 0169 6a11 4ef7 db8d  .d~t..Y..ij.N...
-00004140: a5ed ee07 1282 98f4 9143 ee2d 49fb ec13  .........C.-I...
-00004150: 423b f10a aadf 9ad3 0dbf f9b8 e866 82a2  B;...........f..
-00004160: 5bce bfe6 cf73 deeb 9f0a 32e4 0272 c105  [....s....2..r..
-00004170: e492 0bc8 1517 9011 1790 6b2e 2037 5c40  ..........k. 7\@
-00004180: 6eb9 80c8 011b 1236 d92a d984 ab64 93ae  n......6.*...d..
-00004190: 924d bc4a 36f9 2ad9 04ac 6493 b092 4dc4  .M.J6.*...d...M.
-000041a0: 4a36 193b fcd7 8c7d f57e f1d7 7f27 ed5a  J6.;...}.~...'.Z
-000041b0: 58a5 dd1e 4074 7f81 d377 504b 0102 1403  X...@t...wPK....
-000041c0: 1400 0000 0800 d585 9958 465a c10c 8200  .........XFZ....
-000041d0: 0000 b100 0000 1000 0000 0000 0000 0000  ................
-000041e0: 0000 8001 0000 0000 646f 6350 726f 7073  ........docProps
-000041f0: 2f61 7070 2e78 6d6c 504b 0102 1403 1400  /app.xmlPK......
-00004200: 0000 0800 d585 9958 eb1e 5f40 ee00 0000  .......X.._@....
-00004210: cb01 0000 1100 0000 0000 0000 0000 0000  ................
-00004220: 8001 b000 0000 646f 6350 726f 7073 2f63  ......docProps/c
-00004230: 6f72 652e 786d 6c50 4b01 0214 0314 0000  ore.xmlPK.......
-00004240: 0008 00d5 8599 5899 5c9c 2310 0600 009c  ......X.\.#.....
-00004250: 2700 0013 0000 0000 0000 0000 0000 0080  '...............
-00004260: 01cd 0100 0078 6c2f 7468 656d 652f 7468  .....xl/theme/th
-00004270: 656d 6531 2e78 6d6c 504b 0102 1403 1400  eme1.xmlPK......
-00004280: 0000 0800 d585 9958 0f95 4d33 4801 0000  .......X..M3H...
-00004290: 4902 0000 1800 0000 0000 0000 0000 0000  I...............
-000042a0: 8081 0e08 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000042b0: 6574 732f 7368 6565 7431 2e78 6d6c 504b  ets/sheet1.xmlPK
-000042c0: 0102 1403 1400 0000 0800 d585 9958 0f95  .............X..
-000042d0: 4d33 4801 0000 4902 0000 1800 0000 0000  M3H...I.........
-000042e0: 0000 0000 0000 8081 8c09 0000 786c 2f77  ............xl/w
-000042f0: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
-00004300: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-00004310: d585 9958 6464 8808 5c02 0000 db05 0000  ...Xdd..\.......
-00004320: 1800 0000 0000 0000 0000 0000 8081 0a0b  ................
-00004330: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00004340: 7368 6565 7433 2e78 6d6c 504b 0102 1403  sheet3.xmlPK....
-00004350: 1400 0000 0800 d585 9958 1837 6c2c be02  .........X.7l,..
-00004360: 0000 7808 0000 1800 0000 0000 0000 0000  ..x.............
-00004370: 0000 8081 9c0d 0000 786c 2f77 6f72 6b73  ........xl/works
-00004380: 6865 6574 732f 7368 6565 7434 2e78 6d6c  heets/sheet4.xml
-00004390: 504b 0102 1403 1400 0000 0800 d585 9958  PK.............X
-000043a0: 4cb5 afc5 9403 0000 910d 0000 1800 0000  L...............
-000043b0: 0000 0000 0000 0000 8081 9010 0000 786c  ..............xl
-000043c0: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
-000043d0: 7435 2e78 6d6c 504b 0102 1403 1400 0000  t5.xmlPK........
-000043e0: 0800 d585 9958 1837 6c2c be02 0000 7808  .....X.7l,....x.
-000043f0: 0000 1800 0000 0000 0000 0000 0000 8081  ................
-00004400: 5a14 0000 786c 2f77 6f72 6b73 6865 6574  Z...xl/worksheet
-00004410: 732f 7368 6565 7436 2e78 6d6c 504b 0102  s/sheet6.xmlPK..
-00004420: 1403 1400 0000 0800 d585 9958 146c abe1  ...........X.l..
-00004430: 6801 0000 e802 0000 1800 0000 0000 0000  h...............
-00004440: 0000 0000 8081 4e17 0000 786c 2f77 6f72  ......N...xl/wor
-00004450: 6b73 6865 6574 732f 7368 6565 7437 2e78  ksheets/sheet7.x
-00004460: 6d6c 504b 0102 1403 1400 0000 0800 d585  mlPK............
-00004470: 9958 90c3 86f2 7c03 0000 900b 0000 1800  .X....|.........
-00004480: 0000 0000 0000 0000 0000 8081 ec18 0000  ................
-00004490: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-000044a0: 6565 7438 2e78 6d6c 504b 0102 1403 1400  eet8.xmlPK......
-000044b0: 0000 0800 d585 9958 90c3 86f2 7c03 0000  .......X....|...
-000044c0: 900b 0000 1800 0000 0000 0000 0000 0000  ................
-000044d0: 8081 9e1c 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
-000044e0: 6574 732f 7368 6565 7439 2e78 6d6c 504b  ets/sheet9.xmlPK
-000044f0: 0102 1403 1400 0000 0800 d585 9958 90c3  .............X..
-00004500: 86f2 7c03 0000 900b 0000 1900 0000 0000  ..|.............
-00004510: 0000 0000 0000 8081 5020 0000 786c 2f77  ........P ..xl/w
-00004520: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
-00004530: 302e 786d 6c50 4b01 0214 0314 0000 0008  0.xmlPK.........
-00004540: 00d5 8599 5832 eb97 58f4 0100 0047 0400  ....X2..X....G..
-00004550: 0019 0000 0000 0000 0000 0000 0080 8103  ................
-00004560: 2400 0078 6c2f 776f 726b 7368 6565 7473  $..xl/worksheets
-00004570: 2f73 6865 6574 3131 2e78 6d6c 504b 0102  /sheet11.xmlPK..
-00004580: 1403 1400 0000 0800 d585 9958 6565 3fda  ...........Xee?.
-00004590: 0d02 0000 c104 0000 1900 0000 0000 0000  ................
-000045a0: 0000 0000 8081 2e26 0000 786c 2f77 6f72  .......&..xl/wor
-000045b0: 6b73 6865 6574 732f 7368 6565 7431 322e  ksheets/sheet12.
-000045c0: 786d 6c50 4b01 0214 0314 0000 0008 00d5  xmlPK...........
-000045d0: 8599 5865 653f da0d 0200 00c1 0400 0019  ..Xee?..........
-000045e0: 0000 0000 0000 0000 0000 0080 8172 2800  .............r(.
-000045f0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00004600: 6865 6574 3133 2e78 6d6c 504b 0102 1403  heet13.xmlPK....
-00004610: 1400 0000 0800 d585 9958 953b a42f 1101  .........X.;./..
-00004620: 0000 c801 0000 1900 0000 0000 0000 0000  ................
-00004630: 0000 8081 b62a 0000 786c 2f77 6f72 6b73  .....*..xl/works
-00004640: 6865 6574 732f 7368 6565 7431 342e 786d  heets/sheet14.xm
-00004650: 6c50 4b01 0214 0314 0000 0008 00d5 8599  lPK.............
-00004660: 5865 653f da0d 0200 00c1 0400 0019 0000  Xee?............
-00004670: 0000 0000 0000 0000 0080 81fe 2b00 0078  ............+..x
-00004680: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
-00004690: 6574 3135 2e78 6d6c 504b 0102 1403 1400  et15.xmlPK......
-000046a0: 0000 0800 d585 9958 6565 3fda 0d02 0000  .......Xee?.....
-000046b0: c104 0000 1900 0000 0000 0000 0000 0000  ................
-000046c0: 8081 422e 0000 786c 2f77 6f72 6b73 6865  ..B...xl/workshe
-000046d0: 6574 732f 7368 6565 7431 362e 786d 6c50  ets/sheet16.xmlP
-000046e0: 4b01 0214 0314 0000 0008 00d5 8599 582b  K.............X+
-000046f0: cd41 45fa 0100 0076 0400 0019 0000 0000  .AE....v........
-00004700: 0000 0000 0000 0080 8186 3000 0078 6c2f  ..........0..xl/
-00004710: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00004720: 3137 2e78 6d6c 504b 0102 1403 1400 0000  17.xmlPK........
-00004730: 0800 d585 9958 652f befe 7e02 0000 8106  .....Xe/..~.....
-00004740: 0000 1900 0000 0000 0000 0000 0000 8081  ................
-00004750: b732 0000 786c 2f77 6f72 6b73 6865 6574  .2..xl/worksheet
-00004760: 732f 7368 6565 7431 382e 786d 6c50 4b01  s/sheet18.xmlPK.
-00004770: 0214 0314 0000 0008 00d5 8599 58e1 b4af  ............X...
-00004780: 0f79 0100 004f 0300 0019 0000 0000 0000  .y...O..........
-00004790: 0000 0000 0080 816c 3500 0078 6c2f 776f  .......l5..xl/wo
-000047a0: 726b 7368 6565 7473 2f73 6865 6574 3139  rksheets/sheet19
-000047b0: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
-000047c0: d585 9958 25f9 f458 ac01 0000 4d04 0000  ...X%..X....M...
-000047d0: 1900 0000 0000 0000 0000 0000 8081 1c37  ...............7
-000047e0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-000047f0: 7368 6565 7432 302e 786d 6c50 4b01 0214  sheet20.xmlPK...
-00004800: 0314 0000 0008 00d5 8599 58d2 05f1 4652  ..........X...FR
-00004810: 0200 0047 0a00 000d 0000 0000 0000 0000  ...G............
-00004820: 0000 0080 01ff 3800 0078 6c2f 7374 796c  ......8..xl/styl
-00004830: 6573 2e78 6d6c 504b 0102 1403 1400 0000  es.xmlPK........
-00004840: 0800 d585 9958 b747 eb8a c000 0000 1602  .....X.G........
-00004850: 0000 0b00 0000 0000 0000 0000 0000 8001  ................
-00004860: 7c3b 0000 5f72 656c 732f 2e72 656c 7350  |;.._rels/.relsP
-00004870: 4b01 0214 0314 0000 0008 00d5 8599 58b1  K.............X.
-00004880: db15 1a3c 0200 00a2 0700 000f 0000 0000  ...<............
-00004890: 0000 0000 0000 0080 0165 3c00 0078 6c2f  .........e<..xl/
-000048a0: 776f 726b 626f 6f6b 2e78 6d6c 504b 0102  workbook.xmlPK..
-000048b0: 1403 1400 0000 0800 d585 9958 6741 6968  ...........XgAih
-000048c0: 2101 0000 e90c 0000 1a00 0000 0000 0000  !...............
-000048d0: 0000 0000 8001 ce3e 0000 786c 2f5f 7265  .......>..xl/_re
-000048e0: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
-000048f0: 7265 6c73 504b 0102 1403 1400 0000 0800  relsPK..........
-00004900: d585 9958 5244 7255 6201 0000 0d0e 0000  ...XRDrUb.......
-00004910: 1300 0000 0000 0000 0000 0000 8001 2740  ..............'@
-00004920: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
-00004930: 5d2e 786d 6c50 4b05 0600 0000 001c 001c  ].xmlPK.........
-00004940: 007b 0700 00ba 4100 0000 00              .{....A....
+000000e0: 91c1 4ec3 300c 865f 65ea bd75 d3a0 0aa2  ..N.0.._e..u....
+000000f0: ac17 1027 9090 9804 e216 25de 16ad 49a3  ...'......%...I.
+00000100: c4a8 dddb d396 ad1b 820b c7f8 fffc d956  ...............V
+00000110: a40e 4277 115f 6217 3092 c5b4 1a5c eb93  ..Bw._b.0....\..
+00000120: d061 9ded 8982 0048 7a8f 4ea5 6224 fc18  .a.....Hz.N.b$..
+00000130: 6ebb e814 8dcf b883 a0f4 41ed 10aa b2ac  n.........A.....
+00000140: c121 29a3 48c1 24cc c362 cc4e 4aa3 1765  .!).H.$..b.NJ..e
+00000150: f88c ed2c 301a b045 879e 12b0 82c1 8525  ...,0..E.......%
+00000160: 8c2e fdd9 3027 0b39 24bb 507d df17 3d9f  ....0'.9$.P}..=.
+00000170: b971 2306 efcf 4faf f3f2 b9f5 8994 d798  .q#...O.........
+00000180: 35d2 68a1 232a ea62 335d 148e 432b e1aa  5.h.#*.b3]..C+..
+00000190: 284f b3bf 0b68 56e3 0441 c780 ebec 9cbc  (O...hV..A......
+000001a0: f1fb 87cd 63d6 5465 7593 973c 67b7 1b76  ....c.Teu..<g..v
+000001b0: 27aa 5a70 fe31 b97e f45f 84ae 3376 6bff  '.Zp.1.~._..3vk.
+000001c0: 69ac af8c 6741 23e1 d7bf 355f 504b 0304  i...gA#...5_PK..
+000001d0: 1400 0000 0800 5263 7258 995c 9c23 1006  ......RcrX.\.#..
+000001e0: 0000 9c27 0000 1300 0000 786c 2f74 6865  ...'......xl/the
+000001f0: 6d65 2f74 6865 6d65 312e 786d 6ced 5a5b  me/theme1.xml.Z[
+00000200: 73da 3814 7eef afd0 7867 f66d 0bc6 3681  s.8.~...xg.m..6.
+00000210: b6b4 1373 6976 dbb4 9984 ed4e 1f85 1158  ...siv.....N...X
+00000220: 8d6c 7964 9184 7fbf 4736 10cb 960d ed92  .lyd....G6......
+00000230: 4dba 9b3c 042c e9fb ce45 47e7 e838 79f3  M..<.,...EG..8y.
+00000240: ee2e 62e8 8688 94f2 7860 d92f dbd6 bbb7  ..b.....x`./....
+00000250: 2fde e057 3224 1141 3019 a7af f0c0 0aa5  /..W2$.A0.......
+00000260: 4c5e b55a 6900 c338 7dc9 1312 c3dc 828b  L^.Zi..8}.......
+00000270: 084b 7814 cbd6 5ce0 5b1a 2f23 d6ea b4db  .Kx...\.[./#....
+00000280: dd56 8469 6ca1 1847 6460 7d5e 2c68 40d0  .V.il..Gd`}^,h@.
+00000290: 5451 5a6f 5f20 b4e5 1f33 f815 cb54 8d65  TQZo_ ...3...T.e
+000002a0: a301 1357 4126 b988 b4f2 f96c c5fc dade  ...WA&.....l....
+000002b0: 3e65 cfe9 3a1d 3281 6e30 1b58 207f ce6f  >e..:.2.n0.X ..o
+000002c0: a7e4 4e5a 88e1 54c2 c4c0 6a67 3f56 6bc7  ..NZ..T...jg?Vk.
+000002d0: d1d2 4880 82c9 7d94 05ba 49f6 a3d3 1508  ..H...}...I.....
+000002e0: 320d 3b3a 9d58 ce76 7cf6 c4ed 9f8c cada  2.;:.X.v|.......
+000002f0: 7434 6d1a e0e3 f178 38b6 cbd2 8b70 1c04  t4m....x8....p..
+00000300: e051 bb9e c29d f46c bfa4 4109 b4a3 69d0  .Q.....l..A...i.
+00000310: 64d8 f6da ae91 a6aa 8d53 4fd3 f77d dfeb  d........SO..}..
+00000320: 9b68 9c0a 8d5b 4fd3 6b77 ddd3 8e89 c6ad  .h...[O.kw......
+00000330: d078 0dbe f14f 87c3 ae89 c6ab d074 eb69  .x...O.......t.i
+00000340: 2627 fdae 6ba4 e916 6842 46e3 eb7a 1215  &'..k...hBF..z..
+00000350: b5e5 40d3 2000 5870 76d6 ccd2 0396 5e29  ..@. .Xpv.....^)
+00000360: fa75 941a d91d bbdd 415c f058 ee39 8911  .u......A\.X.9..
+00000370: fec6 c504 d669 d219 9634 4672 9d90 050e  .....i...4Fr....
+00000380: 0037 c4d1 4c50 7caf 41b6 8ae0 c292 d25c  .7..LP|.A......\
+00000390: 90d6 cf29 b550 1a08 9ac8 81f5 4782 21c5  ...).P......G.!.
+000003a0: dcaf fdf5 97bb c9a4 337a 9d7d 3ace 6b94  ........3z.}:.k.
+000003b0: 7f69 ab01 a7ed bb9b cf93 fc73 e8e4 9fa7  .i.........s....
+000003c0: 93d7 4d42 ce70 bc2c 09f1 fb23 5b61 8727  ..MB.p.,...#[a.'
+000003d0: 6e3b 1372 3a1c 6742 7ccf f6f6 91a5 2532  n;.r:.gB|.....%2
+000003e0: cfef f90a eb4e 3c67 1f56 96b0 5dcf cfe4  .....N<g.V..]...
+000003f0: 9e8c 7223 bbdd f658 7df6 4f47 6e23 d7a9  ..r#...X}.OGn#..
+00000400: c0b3 22d7 9446 2445 9fc8 2dba e411 38b5  .."..F$E..-...8.
+00000410: 490d 3213 3f08 9d86 986a 501c 02a4 0931  I.2.?....jP....1
+00000420: 96a1 86f8 b4c6 ac11 e013 7db7 be08 c8df  ..........}.....
+00000430: 8d88 f7ab 6f9a 3d57 a158 49da 84f8 1046  ....o.=W.XI....F
+00000440: 1ae2 9c73 e673 d16c fb07 a546 d1f6 55bc  ...s.s.l...F..U.
+00000450: dca3 9758 1501 9718 df34 aa35 2cc5 d678  ...X.....4.5,..x
+00000460: 95c0 f1ad 9c3c 1d13 12cd 940b 0641 8697  .....<.......A..
+00000470: 2426 12a9 397e 4d48 13fe 2ba5 dafe 9cd3  $&..9~MH..+.....
+00000480: 40f0 942f 24fa 4a91 8f69 b323 a774 26cd  @../$.J..i.#.t&.
+00000490: e833 1ac1 46af 1b75 8768 d23c 7afe 05f9  .3..F..u.h.<z...
+000004a0: 9c35 0a1c 911b 1d02 671b b346 2184 69bb  .5......g..F!.i.
+000004b0: f01e af24 8e9a adc2 112b 423e 6219 361a  ...$.....+B>b.6.
+000004c0: 72b5 1681 b671 a984 605a 12c6 d178 4ed2  r....q..`Z...xN.
+000004d0: b411 fc59 ac35 933e 60c8 eccd 9175 ced6  ...Y.5.>`....u..
+000004e0: 910e 1192 5e37 423e 62ce 8b90 11bf 1e86  ....^7B>b.......
+000004f0: 384a 9aed a271 5804 fd9e 5ec3 49c1 e882  8J...qX...^.I...
+00000500: cb66 fdb8 7e86 d533 6c2c 8ef7 47d4 174a  .f..~..3l,..G..J
+00000510: e40f 26a7 3fe9 3234 07a3 9a59 09bd 8456  ..&.?.24...Y...V
+00000520: 6a9f aa87 343e a81e 320a 05f1 b91e 3ee5  j...4>..2.....>.
+00000530: 7a78 0a37 96c6 bc50 ae82 7b01 ffd1 da37  zx.7...P..{....7
+00000540: c2ab f882 c039 7f2e 7dcf a5ef b9f4 3da1  .....9..}.....=.
+00000550: d2b7 3723 7d67 c1d3 8b5b de46 6e5b c4fb  ..7#}g...[.Fn[..
+00000560: ae31 dad7 342e 2863 5772 cdc8 c754 af93  .1..4.(cWr...T..
+00000570: 29d8 399f c0ec fd68 3e9e f1ed fad9 2484  ).9....h>.....$.
+00000580: af9a 592d 2316 904b 81b3 4124 b8fc 8bca  ..Y-#..K..A$....
+00000590: f02a c409 e864 5b25 09cb 54d3 6537 8a12  .*...d[%..T.e7..
+000005a0: 9e42 1b6e e953 f54a 95d7 e5af b928 b83c  .B.n.S.J.....(.<
+000005b0: 5be4 e9af a174 3e2c cff9 3c5f e7b4 cd0b  [....t>,..<_....
+000005c0: 3343 b772 4bea b694 beb5 2638 4af4 b1cc  3C.rK.....&8J...
+000005d0: 704e 1ecb 0c3b 673c 921d b677 a01d 35fb  pN...;g<...w..5.
+000005e0: f65d 76e4 23a5 3053 9743 b81a 42be 036d  .]v.#.0S.C..B..m
+000005f0: ba9d dc3a 389e 9891 b90a d352 906f c3f9  ...:8......R.o..
+00000600: e9c5 781a e239 d904 b97d 9857 6de7 d8d1  ..x..9...}.Wm...
+00000610: d1fb e7c1 51b0 a3ef 3c96 1dc7 88f2 a221  ....Q...<......!
+00000620: eea1 8698 cfc3 4387 797b 5f98 6795 c650  ......C.y{_.g..P
+00000630: 3414 6d6c ac24 2c46 b760 b8d7 f12c 14e0  4.ml.$,F.`...,..
+00000640: 6460 2da0 0783 af51 02f2 5255 6031 5bc6  d`-....Q..RU`1[.
+00000650: 032b 90a2 7c4c 8c45 e870 e797 5c5f e3d1  .+..|L.E.p..\_..
+00000660: 92e3 dba6 65b5 6eaf 2977 196d 2252 39c2  ....e.n.)w.m"R9.
+00000670: 6998 1367 abca de65 b1c1 551d cf55 5bf2  i..g...e..U..U[.
+00000680: b0be 6a3d b415 4ecf fe59 adc8 9f0c 114e  ..j=..N..Y.....N
+00000690: 160b 1248 6394 17a6 4aa2 f319 53be e72b  ...Hc...J...S..+
+000006a0: 49c4 5538 bf45 33b6 1297 18bc e3e6 c771  I.U8.E3........q
+000006b0: 4e53 b812 76b6 0f02 32b9 bb39 a97a 6531  NS..v...2..9.ze1
+000006c0: 67a6 f2df 2d0c 092c 5b88 5912 e24d 5ded  g...-..,[.Y..M].
+000006d0: d5e7 9b9c ae7a 2276 fa97 77c1 60f2 fd70  .....z"v..w.`..p
+000006e0: c947 0fe5 3be7 5ff4 5d43 ae7e f6dd e3fa  .G..;._.]C.~....
+000006f0: 6e93 3b48 4c9c 79c5 1101 7445 0223 951c  n.;HL.y...tE.#..
+00000700: 0616 1732 e450 ee92 9006 1301 cd94 c944  ...2.P.........D
+00000710: f002 8264 a61c 8098 fa0b bdf2 0cb9 2915  ...d..........).
+00000720: cead 3e39 7f45 2c83 864e 5ed2 2512 148a  ..>9.E,..N^.%...
+00000730: b00c 0521 1772 e3ef ef93 6a77 8cd7 fa2c  ...!.r....jw...,
+00000740: 816d 8454 3264 d517 ca43 89c1 3d33 7243  .m.T2d...C..=3rC
+00000750: d854 25f3 aeda 260b 85db e254 cdbb 1abe  .T%...&....T....
+00000760: 2660 4bc3 7a6e 9d2d 27ff db5e d43d b417  &`K.zn.-'..^.=..
+00000770: 3d46 f3a3 99e0 1eb3 8773 9b7a b8c2 45ac  =F.......s.z..E.
+00000780: ff58 d61e f932 df39 70db 3ade 035e e613  .X...2.9p.:..^..
+00000790: 2c43 a47e c17d 8a8a 8011 ab62 beba af4f  ,C.~.}.....b...O
+000007a0: f925 9c3b b47b f181 209b fcd6 dba4 f6dd  .%.;.{.. .......
+000007b0: e00c 7cd4 ab5a a564 2b11 3f4b 077c 1f92  ..|..Z.d+.?K.|..
+000007c0: 0663 8c5b f434 5f8f 1462 ada6 b1ad c6da  .c.[.4_..b......
+000007d0: 310c 7980 58f3 0ca1 6638 df87 459a 1a33  1.y.X...f8..E..3
+000007e0: d58b ac39 8d0a 6f41 d540 e53f dbd4 0d68  ...9..oA.@.?...h
+000007f0: f60d 341c 9105 5e31 99b6 36a3 e44e 0a3c  ..4...^1..6..N.<
+00000800: dcfe ef0d b0c2 c48e e1ed 8bbf 0150 4b03  .............PK.
+00000810: 0414 0000 0008 0052 6372 580f 954d 3348  .......RcrX..M3H
+00000820: 0100 0049 0200 0018 0000 0078 6c2f 776f  ...I.......xl/wo
+00000830: 726b 7368 6565 7473 2f73 6865 6574 312e  rksheets/sheet1.
+00000840: 786d 6c75 52db 4ec3 300c fd95 2a1f b074  xmluR.N.0...*..t
+00000850: 485c 34b5 95d8 1082 07a4 6913 f09c b56e  H\4.......i....n
+00000860: 1b2d 894b e2ae f0f7 38ed 6e3c f014 fbc4  .-.K....8.n<....
+00000870: e7f8 d849 36a0 df87 1680 926f 6b5c c845  ...I6......ok\.E
+00000880: 4bd4 2da4 0c65 0b56 8519 76e0 f8a6 466f  K.-..e.V..v...Fo
+00000890: 1571 ea1b 193a 0faa 1a49 d6c8 9b34 bd93  .q...:...I...4..
+000008a0: 5669 278a 6cc4 d6be c8b0 27a3 1dac 7d12  Vi'.l.....'...}.
+000008b0: 7a6b 95ff 5982 c121 1773 7102 36ba 6969  zk..Y..!.sq.6.ii
+000008c0: 0464 9175 aa81 2dd0 7bc7 044e e559 a7d2  .d.u..-.{..N.Y..
+000008d0: 165c d0e8 120f 752e 1ee7 8be5 c418 2b3e  .\....u.......+>
+000008e0: 340c e12a 4ee2 303b c47d 4c5e ab5c a4d1  4..*N.0;.}L^.\..
+000008f0: 1318 2829 4a28 3e0e b002 63a2 123b f93a  ..()J(>...c..;.:
+00000900: 8a8a 4bd3 c8bc 8e4f f2cf e3fc 6c6f a702  ..K....O....lo..
+00000910: acd0 7cea 8ada 5c3c 88a4 825a f586 3638  ..|...\<...Z..68
+00000920: bcc0 71a6 db8b c527 45aa c83c 0e89 8fc3  ..q....'E..<....
+00000930: 1659 1983 d892 0bb5 8b4b da92 675c 7327  .Y.......K..g\s'
+00000940: 2a3a e595 0502 9f49 621b 1194 e591 b4fc  *:.....Ib.......
+00000950: 8f74 50a6 87bf 04c9 1d4f 634c 16e2 8adf  .tP......OcL....
+00000960: 946f b40b 8981 9a85 d2d9 3d1b f593 e729  .o........=....)
+00000970: 21ec c627 d921 11da 316c f9a9 c1c7 02be  !..'.!..1l......
+00000980: af11 e99c c49d 9d7f 4ff1 0b50 4b03 0414  ........O..PK...
+00000990: 0000 0008 0052 6372 580f 954d 3348 0100  .....RcrX..M3H..
+000009a0: 0049 0200 0018 0000 0078 6c2f 776f 726b  .I.......xl/work
+000009b0: 7368 6565 7473 2f73 6865 6574 322e 786d  sheets/sheet2.xm
+000009c0: 6c75 52db 4ec3 300c fd95 2a1f b074 485c  luR.N.0...*..tH\
+000009d0: 34b5 95d8 1082 07a4 6913 f09c b56e 1b2d  4.......i....n.-
+000009e0: 894b e2ae f0f7 38ed 6e3c f014 fbc4 e7f8  .K....8.n<......
+000009f0: d849 36a0 df87 1680 926f 6b5c c845 4bd4  .I6......ok\.EK.
+00000a00: 2da4 0c65 0b56 8519 76e0 f8a6 466f 1571  -..e.V..v...Fo.q
+00000a10: ea1b 193a 0faa 1a49 d6c8 9b34 bd93 5669  ...:...I...4..Vi
+00000a20: 278a 6cc4 d6be c8b0 27a3 1dac 7d12 7a6b  '.l.....'...}.zk
+00000a30: 95ff 5982 c121 1773 7102 36ba 6969 0464  ..Y..!.sq.6.ii.d
+00000a40: 9175 aa81 2dd0 7bc7 044e e559 a7d2 165c  .u..-.{..N.Y...\
+00000a50: d0e8 120f 752e 1ee7 8be5 c418 2b3e 340c  ....u.......+>4.
+00000a60: e12a 4ee2 303b c47d 4c5e ab5c a4d1 1318  .*N.0;.}L^.\....
+00000a70: 2829 4a28 3e0e b002 63a2 123b f93a 8a8a  ()J(>...c..;.:..
+00000a80: 4bd3 c8bc 8e4f f2cf e3fc 6c6f a702 acd0  K....O....lo....
+00000a90: 7cea 8ada 5c3c 88a4 825a f586 3638 bcc0  |...\<...Z..68..
+00000aa0: 71a6 db8b c527 45aa c83c 0e89 8fc3 1659  q....'E..<.....Y
+00000ab0: 1983 d892 0bb5 8b4b da92 675c 7327 2a3a  .......K..g\s'*:
+00000ac0: e595 0502 9f49 621b 1194 e591 b4fc 8f74  .....Ib........t
+00000ad0: 50a6 87bf 04c9 1d4f 634c 16e2 8adf 946f  P......OcL.....o
+00000ae0: b40b 8981 9a85 d2d9 3d1b f593 e729 21ec  ........=....)!.
+00000af0: c627 d921 11da 316c f9a9 c1c7 02be af11  .'.!..1l........
+00000b00: e99c c49d 9d7f 4ff1 0b50 4b03 0414 0000  ......O..PK.....
+00000b10: 0008 0052 6372 58b1 1155 4740 0200 0078  ...RcrX..UG@...x
+00000b20: 0500 0018 0000 0078 6c2f 776f 726b 7368  .......xl/worksh
+00000b30: 6565 7473 2f73 6865 6574 332e 786d 6cbd  eets/sheet3.xml.
+00000b40: 54db 6edb 300c fd15 c3cf 419d 04eb 0581  T.n.0.....A.....
+00000b50: 6320 97a6 29b0 005d 9376 8f03 6333 b116  c ..)..].v..c3..
+00000b60: 59f4 24ba 5eff 7e94 9da6 1724 79dc 8b2d  Y.$.^.~....$y..-
+00000b70: 1ef1 503c 12c9 b826 bb73 3922 077f 0b6d  ..P<...&.s9"...m
+00000b80: dc30 cc99 cb41 14b9 34c7 02dc 0595 6864  .0...A..4.....hd
+00000b90: 6743 b600 16d3 6e23 575a 84ac 2115 3aea  gC....n#WZ..!.:.
+00000ba0: 77bb 5751 01ca 8449 dc60 0f36 89a9 62ad  w.WQ...I.`.6..b.
+00000bb0: 0c3e d8c0 5545 01f6 758c 9aea 61d8 0bdf  .>..UE..u...a...
+00000bc0: 8047 b5cd b901 a224 2e61 8b4b e4a7 5208  .G.....$.a.K..R.
+00000bd0: 6246 8738 992a d038 4526 b0b8 1986 a3de  bF.8.*.8E&......
+00000be0: 60de 321a 8f67 85b5 fbb0 0ebc 9835 d1ce  `.2..g.......5..
+00000bf0: 1bf7 d930 ecfa 9c50 63ca 3e04 c8ef 0527  ...0...Pc.>....'
+00000c00: a8b5 8f24 99fc d907 0ddf 0ff5 cc8f ebb7  ...$............
+00000c10: f0b3 46bf a4b7 0687 13d2 3f55 c6f9 30bc  ..F.......?U..0.
+00000c20: 0983 0c37 5069 7ea4 7a8e 7b4d 97ef 294e  ...7Pi~.z.{M..)N
+00000c30: 8121 892d d581 f562 9338 f50b 7fa4 382a  .!.-...b.8....8*
+00000c40: e32f 69c9 5670 2527 71c2 e8f8 97a3 caa6  ./i.Vp%'q.......
+00000c50: 1847 2c89 7838 4af7 b4f1 599a 8841 8be6  .G,.x8J...Y..A..
+00000c60: 2873 7296 49eb dfd8 dccd 11e6 f42c 138c  (sr.I........,..
+00000c70: 2106 7fbb ee08 f7f6 1457 6547 bc67 a7bc  !........WeG.g..
+00000c80: 0d14 c732 bb3b e59f a14b ad2a 7d56 4768  ...2.;...K.*}VGh
+00000c90: f393 8260 fb45 4424 eff6 560c ed43 66f2  ...`.ED$..V..Cf.
+00000ca0: 7d06 adb2 5673 9052 6524 583f fcba 7528  }...Vs.Re$X?..u(
+00000cb0: aefe 60d4 eb7e bbb9 bcbe 9282 cba9 9e5a  ..`..~.........Z
+00000cc0: 2aa7 541b 5f9c 0d70 6fca 8a17 e89c f4c0  *.T._..po.......
+00000cd0: 01bc b596 ec47 10b4 f4cf 5883 d935 3dc3  .....G....X..5=.
+00000ce0: afa5 e05a 3996 937d 6f56 1a7a 49b8 5cdc  ...Z9..}oV.zI.\.
+00000cf0: 7696 8ba7 c759 e74e f1bc 5a3f 39b4 33c4  v....Y.N..Z?9.3.
+00000d00: 6c0d e9ae b31a 4d56 9db1 1448 be00 2ba6  l.....MV...H..+.
+00000d10: 05e3 3430 d915 42d1 59c9 737a 8ddf 296d  ..40..B.Y.sz..)m
+00000d20: 0484 7174 881b 479f c59d 123b e90f 26ff  ..qt..G....;..&.
+00000d30: 4fec 284d b164 9082 f7b9 b7ca 64b2 ec1a  O.(M.d......d...
+00000d40: eb47 0586 952f cd97 66fb bc9c 2f80 6b27  .G.../..f.../.k'
+00000d50: 925c d356 c923 6bdc c81b 772f aea5 af6d  .\.V.#k...w/...m
+00000d60: dbe2 adc1 5436 09ae 8999 8a66 99cb 6444  ....T6.....f..dD
+00000d70: eb1d 647f 43c4 07c3 8f98 c3b0 4dfe 0150  ..d.C.......M..P
+00000d80: 4b03 0414 0000 0008 0052 6372 5825 817d  K........RcrX%.}
+00000d90: dbbf 0200 0073 0800 0018 0000 0078 6c2f  .....s.......xl/
+00000da0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00000db0: 342e 786d 6cbd 96db 72da 3010 865f c5e3  4.xml...r.0.._..
+00000dc0: 6b26 06a6 390c 633c 9384 a449 032d cd81  k&..9.c<...I.-..
+00000dd0: 5e32 c25e 8c06 59eb 48eb 3879 fbae 4c20  ^2.^..Y.H.8y..L 
+00000de0: 69c6 82bb 5e21 adf5 49fb af56 bbc4 359a  i...^!..I..V..5.
+00000df0: b55d 0150 f05a 286d 87e1 8aa8 1c44 914d  .].P.Z(m.....D.M
+00000e00: 5750 087b 8425 68fe b244 5308 e2a9 c923  WP.{.%h..DS....#
+00000e10: 5b1a 1059 0315 2aea 77bb 2751 21a4 0e93  [..Y..*.w.'Q!...
+00000e20: b8b1 4d4d 1263 454a 6a98 9ac0 5645 21cc  ..MM.cEJj...VE!.
+00000e30: db05 28ac 8761 2fdc 1aee 65be a2c6 1025  ..(..a/...e....%
+00000e40: 7129 7278 007a 2a19 e069 b4db 2793 0568  q)rx.z*..i..'..h
+00000e50: 2b51 0706 96c3 f0bc 3798 6d88 66c5 4c42  +Q......7.m.f.LB
+00000e60: 6d3f 8d03 2766 81b8 7693 db6c 1876 9d4f  m?..'f..v..l.v.O
+00000e70: a020 25b7 85e0 9f17 b804 a5dc 4eec c9f3  . %.........N...
+00000e80: fba6 e1c7 a18e fc3c de6e 7fdd e867 f716  .......<.n...g..
+00000e90: c2c2 25aa 3f32 a3d5 303c 0b83 0c96 a252  ..%.?2..0<.....R
+00000ea0: 748f f50d bc6b 3afe 7071 2448 24b1 c13a  t....k:.pq$H$..:
+00000eb0: 304e 6c12 a76e e08e e485 52bb 203d 9061  0Nl..n....R. =.a
+00000ec0: bbe4 9328 91ba ac68 2eb3 3822 f6c2 d9a2  ...(...h..8"....
+00000ed0: f49d b9d8 cf68 5140 0b75 b99f 4a05 418e  .....hQ@.u..J.A.
+00000ee0: e6ad 851c f948 befd 4c3a b0dd cfab c39c  .....H..L:......
+00000ef0: c7d7 6b1f c9d9 e40d cbf7 0390 e7ac 9b03  ..k.............
+00000f00: d89e c0dc fa50 612d a652 b85c 6bc1 7ef8  .....Pa-.R.\k.~.
+00000f10: b0e7 4a28 b994 606c 0b75 e7a3 e0b5 e4b4  ..J(..`l.u......
+00000f20: 866c be71 b805 1dfb 5002 cbc1 b4b6 6a0b  .l.q....P.....j.
+00000f30: ccc4 4759 2e07 9a64 3ab7 f002 4652 5b68  ..GY...d:...FR[h
+00000f40: 7efa b36d fed2 6b01 7ef9 809a 5fe9 7cad  ~..m..k.~..._.|.
+00000f50: b16e 0be5 74af 327e d460 40a7 6dea 7efb  .n..t.2~.`@.m.~.
+00000f60: 4853 690d 86b5 1149 9db7 ddc4 fdde 430b  HSi....I......C.
+00000f70: 2091 f15b 6f01 1fbc 4169 cbe7 47df 6a4f   ..[o...Ai..G.jO
+00000f80: 223f f9d6 6760 5323 4b4f 36ce bc6a c457  "?..g`S#KO6..j.W
+00000f90: f511 57af 6d49 dc94 3327 74c6 499b 35b9  ..W.mI..3't.I.5.
+00000fa0: 6e83 142b cd9b f5c3 af9f b625 76dc 1f8c  n..+.......%v...
+00000fb0: 7bdd 6f67 c7a7 275c 7657 588f 0c96 23be  {.og..'\vWX...#.
+00000fc0: 5c57 a21b c3ad 2b47 13b0 963b c1ce 7865  \W....+G...;..xe
+00000fd0: 0c9a cf46 a1b8 8b5c 28a1 d74d e7a0 b792  ...F...\(..M....
+00000fe0: ed4a 5ae2 935d 87aa 94e8 2561 2a2a 0b36  .JZ..]....%a**.6
+00000ff0: d048 0171 a722 db79 9cdc 4d3b db27 1d10  .H.q.".y..M;.'..
+00001000: 6290 035f b74c 3b29 6a32 dcbc 9aca e4c4  b.._.L;)j2......
+00001010: 745c dfe3 890a 0c2a b09d 8fc7 12c6 d1ee  t\.....*........
+00001020: 8c38 fa57 a84f f8a4 3f98 fc3f e137 dc7f  .8.W.O..?..?.7..
+00001030: 3a63 ac3b 3f91 cecb 52b1 8c85 3ae0 f717  :c.;?...R...:...
+00001040: 83dd 34e3 8930 b9e4 9b55 b0e4 8bed 1e9d  ..4..0...U......
+00001050: 724b 339b eeb6 9910 968d 270b 24c2 a219  rK3.......'.$...
+00001060: aef8 4f01 18b7 80bf 2f11 6937 71dd 75f7  ..O...../.i7q.u.
+00001070: 3f23 f90b 504b 0304 1400 0000 0800 5263  ?#..PK........Rc
+00001080: 7258 b356 a83b 9203 0000 8c0d 0000 1800  rX.V.;..........
+00001090: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+000010a0: 7368 6565 7435 2e78 6d6c bd57 db6e db38  sheet5.xml.W.n.8
+000010b0: 10fd 1541 cf42 651b dbb4 3064 0376 aede  ...A.Be...0d.v..
+000010c0: 36dd 6cd2 3add 7d11 6872 6c73 4391 2a39  6.l.:.}.hrlsC.*9
+000010d0: b292 bfdf a11c 2769 40c6 401e fc24 5e74  ......'i@.@..$^t
+000010e0: 8687 c3e1 9961 d11a 7be7 d600 98dc 574a  .....a..{.....WJ
+000010f0: bb51 ba46 ac87 79ee f81a 2ae6 3e98 1a34  .Q.F..y...*.>..4
+00001100: cd2c 8dad 1852 d7ae 7257 5b60 a203 552a  .,...R..rW[`..U*
+00001110: 1ff4 7a47 79c5 a44e c745 3776 65c7 8569  ..zGy..N.E7ve..i
+00001120: 5049 0d57 3671 4d55 31fb 3005 65da 51da  PI.W6qMU1.0.e.Q.
+00001130: 4f77 03d7 72b5 c66e 201f 1735 5bc1 0de0  Ow..r..n ..5[...
+00001140: 8f9a 00d4 cd9f ec08 5981 76d2 e8c4 c272  ........Y.v....r
+00001150: 944e fac3 c9d9 16d2 fd32 97d0 ba17 edc4  .N.......2......
+00001160: ef66 61cc 9def ccc4 28ed 7952 a080 a3b7  .fa.....(.yR....
+00001170: c1e8 b381 6350 ca9b 222a bf1e ada6 cfab  ....cP.."*......
+00001180: 7ae4 cbf6 cefc 59e7 00e2 b760 0e8e 8dba  z.....Y....`....
+00001190: 9502 d7a3 f473 9a08 58b2 46e1 b569 2fe0  .....s..X.F..i/.
+000011a0: 7153 1f9f 299e 3064 e3c2 9a36 b17e b7e3  qS..).0d...6.~..
+000011b0: 82fb 865f 927e 94da 7be9 062d 8d4b 5a09  ..._.~..{..-.KZ.
+000011c0: c755 e3b0 ac99 73a5 6008 458e c4c5 cfe4  .U....s.`.E.....
+000011d0: fc11 39dd 8f04 bd91 d668 f21c 060c 1cc7  ..9......h......
+000011e0: 0c38 2e09 2197 9297 bf1a 70de 6301 f849  .8..!.....p.c..I
+000011f0: 148e 56ea 152d 8ef6 2180 3b8d e184 b4db  ..V..-..!.;.....
+00001200: e309 80ce 6220 a65d 0bb6 94ba 8b4b 5572  ....b .].....KUr
+00001210: a339 d4a1 ed9e c74c c07d 4deb 8228 2d38  .9.....L.}M..(-8
+00001220: 3abe 00f4 2206 4553 970a 36a0 02a0 590c  :...".ES..6...Y.
+00001230: 443e b50f a536 2274 aa7f c650 da20 b800  D>...6"t...P. ..
+00001240: e04b 0c20 75dd 6029 4500 f3f5 6d8c 6655  .K. u.`)E...m.fU
+00001250: 88da e5db 284e 61ba 32c1 23ff 1643 927e  ....(Na.2.#..C.~
+00001260: 08e9 8161 9e7f edc7 45b8 5ec5 90a4 4751  ...a....E.^...GQ
+00001270: b7fc bd07 1459 eb7a 0fec 0dc7 dc44 c3da  .....Y.z.....D..
+00001280: 39c3 258b dc86 eff1 d062 8aee 2dd8 50a4  9.%......b..-.P.
+00001290: fcd8 7b01 b684 03d0 79f4 0290 3c94 d2b9  ..{.....y...<...
+000012a0: 26e4 98db a842 5042 2181 e1a5 a3bb 6325  &....BPB!.....c%
+000012b0: 865c f333 1e6d e5a6 1f00 fc13 03b4 24f3  .\.3.m........$.
+000012c0: e59d 366d c895 ffbe b933 ca0a 6081 1425  ..6m.....3..`..%
+000012d0: 809c 44a5 db36 5a93 2639 4024 210c 1dc5  ..D..6Z.&9@$!...
+000012e0: 242a dedd b215 2023 d567 2164 54b5 8321  $*.... #.g!dT..!
+000012f0: 3d89 aa74 2498 2771 7906 c7ad ac23 2139  =..t$.'qy....#!9
+00001300: 892a 34b2 d72e c829 09ee 32eb 362b facd  .*4....)..2.6+..
+00001310: ce29 7445 17f1 2ee1 a6d1 64ec 287d 3db5  .)tE......d.(}=.
+00001320: cbd4 d3c1 70da effd f1f9 e3a7 23ca de6b  ....p.......#..k
+00001330: d39e 5853 9fd0 11fb 4cdf 0dcc bc28 5d82  ..XS....L....(].
+00001340: 7354 513c 0d9e 5a6b eccb 41a6 a81a 992a  sTQ<..Zk..A....*
+00001350: a6ef ba0a 041f 6a1a 57d2 21ad ec33 4aa3  ......j.W.!..3J.
+00001360: 587f 9c0a d864 5c66 fe6c b2da 1a91 16f9  X....d\f.l......
+00001370: d364 91ff ce30 c6f8 7430 3c3d 1c63 a939  .d...0..t0<=.c.9
+00001380: 9566 0e44 26e0 b1f5 1ed2 e783 e1f9 4149  .f.D&.........AI
+00001390: ab46 40b9 3246 6470 bfed 2cd8 bb98 cf06  .F@.2Fdp..,.....
+000013a0: c3d9 e198 bb66 f11f 4968 66ba cf7b f8ce  .....f..Ihf..{..
+000013b0: 07c3 f9e1 f872 d638 7009 d514 0952 74a0  .....r.8p....Rt.
+000013c0: cbbe 5f7e b9ca 7699 2a41 6392 1590 8849  .._~..v.*Ac....I
+000013d0: 9e51 4585 96aa fa2e e1fa db99 f907 0175  .QE............u
+000013e0: 5462 8d02 973d e780 f76c fc76 30bc 3ddc  Tb...=...l.v0.=.
+000013f0: c62f a82e cfbe 9a36 fb66 7052 d78a b6b1  ./.....6.fpR....
+00001400: 507b 78bf 1a70 db57 ca25 b32b 4952 a560  P{x..p.W.%.+IR.`
+00001410: 494a d5fb f089 4a7d bbad fab7 1daa 0d3b  IJ....J}.......;
+00001420: 260b 8368 aaae b9a6 d712 58ff 03cd 2f0d  &..h......X.../.
+00001430: 5574 bb8e 7f75 3c3d c0c6 ff03 504b 0304  Ut...u<=....PK..
+00001440: 1400 0000 0800 5263 7258 2581 7ddb bf02  ......RcrX%.}...
+00001450: 0000 7308 0000 1800 0000 786c 2f77 6f72  ..s.......xl/wor
+00001460: 6b73 6865 6574 732f 7368 6565 7436 2e78  ksheets/sheet6.x
+00001470: 6d6c bd96 db72 da30 1086 5fc5 e36b 2606  ml...r.0.._..k&.
+00001480: a639 0c63 3c93 84a4 4903 2dcd 815e 32c2  .9.c<...I.-..^2.
+00001490: 5e8c 0659 eb48 eb38 79fb ae4c 2069 c682  ^..Y.H.8y..L i..
+000014a0: bb5e 21ad f549 fbaf 56bb c435 9ab5 5d01  .^!..I..V..5..].
+000014b0: 50f0 5a28 6d87 e18a a81c 4491 4d57 5008  P.Z(m.....D.MWP.
+000014c0: 7b84 2568 feb2 4453 08e2 a9c9 235b 1a10  {.%h..DS....#[..
+000014d0: 5903 152a ea77 bb27 5121 a40e 93b8 b14d  Y..*.w.'Q!.....M
+000014e0: 4d12 6345 4a6a 989a c056 4521 ccdb 0528  M.cEJj...VE!...(
+000014f0: ac87 612f dc1a ee65 bea2 c610 2571 2972  ..a/...e....%q)r
+00001500: 7800 7a2a 19e0 69b4 db27 9305 682b 5107  x.z*..i..'..h+Q.
+00001510: 0696 c3f0 bc37 986d 8866 c54c 426d 3f8d  .....7.m.f.LBm?.
+00001520: 0327 6681 b876 93db 6c18 769d 4fa0 2025  .'f..v..l.v.O. %
+00001530: b785 e09f 17b8 04a5 dc4e ecc9 f3fb a6e1  .........N......
+00001540: c7a1 8efc 3cde 6e7f dde8 67f7 16c2 c225  ....<.n...g....%
+00001550: aa3f 32a3 d530 3c0b 830c 96a2 5274 8ff5  .?2..0<.....Rt..
+00001560: 0dbc 6b3a fe70 7124 4824 b1c1 3a30 4e6c  ..k:.pq$H$..:0Nl
+00001570: 12a7 6ee0 8ee4 8552 bb20 3d90 61bb e493  ..n....R. =.a...
+00001580: 2891 baac 682e b338 22f6 c2d9 a2f4 9db9  (...h..8".......
+00001590: d8cf 6851 400b 75b9 9f4a 0541 8ee6 ad85  ..hQ@.u..J.A....
+000015a0: 1cf9 48be fd4c 3ab0 ddcf abc3 9cc7 d76b  ..H..L:........k
+000015b0: 1fc9 d9e4 0dcb f703 90e7 ac9b 03d8 9ec0  ................
+000015c0: dcfa 5061 2da6 52b8 5c6b c17e f8b0 e74a  ..Pa-.R.\k.~...J
+000015d0: 28b9 9460 6c0b 75e7 a3e0 b5e4 b486 6cbe  (..`l.u.......l.
+000015e0: 71b8 051d fb50 02cb c1b4 b66a 0bcc c447  q....P.....j...G
+000015f0: 592e 079a 643a b7f0 0246 525b 687e fab3  Y...d:...FR[h~..
+00001600: 6dfe d26b 017e f980 9a5f e97c adb1 6e0b  m..k.~..._.|..n.
+00001610: e574 af32 7ed4 6040 a76d ea7e fb48 5369  .t.2~.`@.m.~.HSi
+00001620: 0d86 b511 499d b7dd c4fd de43 0b20 91f1  ....I......C. ..
+00001630: 5b6f 011f bc41 69cb e747 df6a 4f22 3ff9  [o...Ai..G.jO"?.
+00001640: d667 6053 234b 4f36 cebc 6ac4 57f5 1157  .g`S#KO6..j.W..W
+00001650: af6d 49dc 9433 2774 c649 9b35 b96e 8314  .mI..3't.I.5.n..
+00001660: 2bcd 9bf5 c3af 9fb6 2576 dc1f 8c7b dd6f  +.......%v...{.o
+00001670: 67c7 a727 5c76 5758 8f0c 9623 be5c 57a2  g..'\vWX...#.\W.
+00001680: 1bc3 ad2b 4713 b096 3bc1 ce78 650c 9acf  ...+G...;..xe...
+00001690: 46a1 b88b 5c28 a1d7 4de7 a0b7 92ed 4a5a  F...\(..M.....JZ
+000016a0: e293 5d87 aa94 e825 612a 2a0b 36d0 4801  ..]....%a**.6.H.
+000016b0: 71a7 22db 799c dc4d 3bdb 271d 1062 9003  q.".y..M;.'..b..
+000016c0: 5fb7 4c3b 296a 32dc bc9a cae4 c474 5cdf  _.L;)j2......t\.
+000016d0: e389 0a0c 2ab0 9d8f c712 c6d1 ee8c 38fa  ....*.........8.
+000016e0: 57a8 4ff8 a43f 98fc 3fe1 37dc 7f3a 63ac  W.O..?..?.7..:c.
+000016f0: 3b3f 91ce cb52 b18c 853a e0f7 1783 dd34  ;?...R...:.....4
+00001700: e389 30b9 e49b 55b0 e48b ed1e 9d72 4b33  ..0...U......rK3
+00001710: 9bee b699 1096 8d27 0b24 c2a2 19ae f84f  .......'.$.....O
+00001720: 0118 b780 bf2f 1169 3771 dd75 f73f 23f9  ...../.i7q.u.?#.
+00001730: 0b50 4b03 0414 0000 0008 0052 6372 5864  .PK........RcrXd
+00001740: 2f60 5f58 0100 00a8 0200 0018 0000 0078  /`_X...........x
+00001750: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00001760: 6574 372e 786d 6c75 52db 4ec3 300c fd95  et7.xmluR.N.0...
+00001770: 2a1f b074 485c 34b5 95d8 2604 0f48 d326  *..tH\4...&..H.&
+00001780: e039 6bdd 365a 1297 c4a3 f0f7 38ed 2e20  .9k.6Z......8.. 
+00001790: 6d4f b19d 738e 7d9c 643d fa5d 6801 28f9  mO..s.}.d=.]h.(.
+000017a0: b6c6 855c b444 dd4c ca50 b660 5598 6007  ...\.D.L.P.`U.`.
+000017b0: 8e6f 6af4 5611 a7be 91a1 f3a0 aa81 648d  .oj.V.........d.
+000017c0: bc49 d33b 6995 76a2 c886 daca 1719 eec9  .I.;i.v.........
+000017d0: 6807 2b9f 84bd b5ca ffcc c160 9f8b a938  h.+........`...8
+000017e0: 16d6 ba69 6928 c822 eb54 031b a0b7 8e09  ...ii(.".T......
+000017f0: 9cca 934e a52d b8a0 d125 1eea 5c3c 4e67  ...N.-...%..\<Ng
+00001800: cb91 3120 de35 f4e1 4f9c 4433 5bc4 5d4c  ..1 .5..O.D3[.]L
+00001810: 5eaa 5ca4 7126 3050 5294 507c 7cc1 028c  ^.\.q&0PR.P||...
+00001820: 894a 3cc9 e741 549c 9b46 e6df f828 ff34  .J<..AT..F...(.4
+00001830: f8e7 f1b6 2ac0 02cd 87ae a8cd c583 482a  ....*.........H*
+00001840: a8d5 ded0 1afb 6738 78ba 3d8f b854 a48a  ......g8x.=..T..
+00001850: cc63 9ff8 68b6 c8ca 18c4 960c d42e 2e69  .c..h..........i
+00001860: 439e eb9a 3b51 a1ab 4c12 f78f 992c 0fe8  C...;Q..L....,..
+00001870: f935 b453 162e e017 d7f0 1584 d2eb 2e2e  .5.S............
+00001880: e302 6d79 8d46 aa09 fff1 920d 1db7 343a  ..my.F........4:
+00001890: 8c2f f8aa 7ca3 5d48 0cd4 ac93 4eee 790f  ./..|.]H....N.y.
+000018a0: 7e5c c998 1076 c38b 6f91 08ed 10b6 fc93  ~\...v..o.......
+000018b0: c047 00df d788 744a e293 9c3e 67f1 0b50  .G....tJ...>g..P
+000018c0: 4b03 0414 0000 0008 0052 6372 5855 85c6  K........RcrXU..
+000018d0: 84f8 0200 003f 0a00 0018 0000 0078 6c2f  .....?.......xl/
+000018e0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+000018f0: 382e 786d 6cbd 56db 72da 3010 fd15 c6cf  8.xml.V.r.0.....
+00001900: 4e0c 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e  N.Ls..0.........
+00001910: 212f 5845 961c 691d 9abf efca 2424 cdd8  !/XE..i.....$$..
+00001920: 61ca 032f 20ad 7476 cf91 b4eb 0db7 da6c  a../ .tv.......l
+00001930: 6c02 80b5 3fa9 54b6 ed25 8859 2b08 2c4f  l...?.T..%.Y+.,O
+00001940: 2065 f65c 67a0 6865 a54d ca90 a666 1dd8   e.\g.he.M...f..
+00001950: cc00 8b0b 502a 8366 bd7e 19a4 4c28 af13  ....P*.f.~..L(..
+00001960: 16b6 99e9 843a 4729 14cc 4ccd e669 cacc  .....:G)..L..i..
+00001970: 730f a4de b6bd 86f7 6ab8 13eb 040b 43d0  s.......j.....C.
+00001980: 0933 b686 39e0 7d46 009a 067b 3fb1 4841  .3..9.}F...{?.HA
+00001990: 59a1 55cd c0aa ed75 1bad d90e 51ec 7810  Y.U....u....Q.x.
+000019a0: b0b5 efc6 3527 66a9 f5c6 4d6e e2b6 5777  ....5'f...Mn..Ww
+000019b0: 9c40 0247 e782 d1df 13f4 414a e789 983c  .@.G......AJ...<
+000019c0: be38 f5de 823a e4fb f1ab fb51 a19f e82d  .8...:.....Q...-
+000019d0: 9985 be96 bf44 8c49 dbbb f66a 31ac 582e  .....D.I...j1.X.
+000019e0: f14e 6f27 f0a2 e9e2 8de2 8021 eb84 466f  .No'.......!..Fo
+000019f0: 6bc6 89ed 84dc 0d5c 48da 2894 3ba4 391a  k......\H.(.;.9.
+00001a00: b20b 8a84 1d04 8b11 a8a7 3040 62e1 6c01  ..........0@b.l.
+00001a10: 7fc1 f4aa 308f 3998 e708 9f33 2841 f53f  ....0.9....3(A.?
+00001a20: 8dc4 ac05 b425 b041 158c ae9e 6b15 0b77  .....%.A....k..w
+00001a30: a065 c061 653c c332 1121 a499 6458 c674  .e.ae<.2.!..dX.t
+00001a40: 5485 e43a cdb4 0255 4a74 fca9 3e4e 9715  T..:...UJt..>N..
+00001a50: e9e5 6f28 6ebe 043e 390c b73a 37bc 0c7b  ..o(n..>9..:7..{
+00001a60: 7318 4ba7 150b 4e7a 23c5 d232 1f5f ffc7  s.K...Nz#..2._..
+00001a70: 8788 4b3c 7c3b ec41 a82c c772 f4ed 61b4  ..K<|;.A.,.r..a.
+00001a80: c995 0213 d143 41a1 d665 7730 ad72 521a  .....CA..ew0.rR.
+00001a90: f27b d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b  .{...#.Q.?.....K
+00001aa0: 2c81 cd2a 95b1 8f22 024a cfd7 9cdf e56b  ,..*...".J.....k
+00001ab0: 4cbf 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7  L..L..w...u.....
+00001ac0: 7169 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a  qi_C..n........J
+00001ad0: a2b7 03a3 b381 de2a 5783 0ac3 8dbb 8429  .......*W......)
+00001ae0: 584b a56e 6f1c 1aa3 cd7b 2393 5426 7b92  XK.no....{#.T&{.
+00001af0: a94d 511a 5d52 b73d 292c 5264 5782 73c9  .MQ.]R.=),RdW.s.
+00001b00: 1a1d 2f86 279f 0bdf dd91 9f19 1d7b 61b0  ../.'........{a.
+00001b10: 5f0c 837f 1956 31ee 355b bdd3 3146 fa62  _....V1.5[..1F.b
+00001b20: a03d 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c  .=.......'=A)..l
+00001b30: b3fe 8eb3 8f89 0188 129d f9b1 c9d7 d1ce  ................
+00001b40: 1a19 6620 8a85 054a 9162 e10c f5d9 1a14  ..f ...J.b......
+00001b50: 1ca3 71d4 6c8d 4ea7 f118 86e3 666b 7c3a  ..q.l.N.....fk|:
+00001b60: 865d ce21 43a6 382c dc13 ef81 e209 f50c  .].!C.8,........
+00001b70: 9b62 f633 670a 0532 57d1 9de1 1839 9366  .b.3g..2W....9.f
+00001b80: 6b72 3a39 f3e9 d09f 4fef ef46 fe58 e024  kr:9....O..F.X.$
+00001b90: 5fde 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2  _.[0#.x..._t....
+00001ba0: 2929 f417 8629 4b5f 486d 16c0 52df 0974  ))...)K_Hm..R..t
+00001bb0: 25e9 56f3 42c0 e762 3f18 ecae b122 bf6b  %.V.B..b?....".k
+00001bc0: 4145 4cc2 8a6a 58fd fc8a da13 b3eb 5476  AEL..jX.......Tv
+00001bd0: 13d4 5941 7fa9 1175 5a0c 136a f0c0 b80d  ..YA...uZ..j....
+00001be0: b4be d21a f713 d729 ed7b c6ce 5f50 4b03  .......).{.._PK.
+00001bf0: 0414 0000 0008 0052 6372 5855 85c6 84f8  .......RcrXU....
+00001c00: 0200 003f 0a00 0018 0000 0078 6c2f 776f  ...?.......xl/wo
+00001c10: 726b 7368 6565 7473 2f73 6865 6574 392e  rksheets/sheet9.
+00001c20: 786d 6cbd 56db 72da 3010 fd15 c6cf 4e0c  xml.V.r.0.....N.
+00001c30: 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e 212f  Ls..0.........!/
+00001c40: 5845 961c 691d 9abf efca 2424 cdd8 61ca  XE..i.....$$..a.
+00001c50: 032f 20ad 7476 cf91 b4eb 0db7 da6c 6c02  ./ .tv.......ll.
+00001c60: 80b5 3fa9 54b6 ed25 8859 2b08 2c4f 2065  ..?.T..%.Y+.,O e
+00001c70: f65c 67a0 6865 a54d ca90 a666 1dd8 cc00  .\g.he.M...f....
+00001c80: 8b0b 502a 8366 bd7e 19a4 4c28 af13 16b6  ..P*.f.~..L(....
+00001c90: 99e9 843a 4729 14cc 4ccd e669 cacc 730f  ...:G)..L..i..s.
+00001ca0: a4de b6bd 86f7 6ab8 13eb 040b 43d0 0933  ......j.....C..3
+00001cb0: b686 39e0 7d46 009a 067b 3fb1 4841 59a1  ..9.}F...{?.HAY.
+00001cc0: 55cd c0aa ed75 1bad d90e 51ec 7810 b0b5  U....u....Q.x...
+00001cd0: efc6 3527 66a9 f5c6 4d6e e2b6 5777 9c40  ..5'f...Mn..Ww.@
+00001ce0: 0247 e782 d1df 13f4 414a e789 983c be38  .G......AJ...<.8
+00001cf0: f5de 823a e4fb f1ab fb51 a19f e82d 9985  ...:.....Q...-..
+00001d00: be96 bf44 8c49 dbbb f66a 31ac 582e f14e  ...D.I...j1.X..N
+00001d10: 6f27 f0a2 e9e2 8de2 8021 eb84 466f 6bc6  o'.......!..Fok.
+00001d20: 89ed 84dc 0d5c 48da 2894 3ba4 391a b20b  .....\H.(.;.9...
+00001d30: 8a84 1d04 8b11 a8a7 3040 62e1 6c01 7fc1  ........0@b.l...
+00001d40: f4aa 308f 3998 e708 9f33 2841 f53f 8dc4  ..0.9....3(A.?..
+00001d50: ac05 b425 b041 158c ae9e 6b15 0b77 a065  ...%.A....k..w.e
+00001d60: c061 653c c332 1121 a499 6458 c674 5485  .ae<.2.!..dX.tT.
+00001d70: e43a cdb4 0255 4a74 fca9 3e4e 9715 e9e5  .:...UJt..>N....
+00001d80: 6f28 6ebe 043e 390c b73a 37bc 0c7b 7318  o(n..>9..:7..{s.
+00001d90: 4ba7 150b 4e7a 23c5 d232 1f5f ffc7 8788  K...Nz#..2._....
+00001da0: 4b3c 7c3b ec41 a82c c772 f4ed 61b4 c995  K<|;.A.,.r..a...
+00001db0: 0213 d143 41a1 d665 7730 ad72 521a f27b  ...CA..ew0.rR..{
+00001dc0: d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b 2c81  ...#.Q.?.....K,.
+00001dd0: cd2a 95b1 8f22 024a cfd7 9cdf e56b 4cbf  .*...".J.....kL.
+00001de0: 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7 7169  .L..w...u.....qi
+00001df0: 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a a2b7  _C..n........J..
+00001e00: 03a3 b381 de2a 5783 0ac3 8dbb 8429 584b  .....*W......)XK
+00001e10: a56e 6f1c 1aa3 cd7b 2393 5426 7b92 a94d  .no....{#.T&{..M
+00001e20: 511a 5d52 b73d 292c 5264 5782 73c9 1a1d  Q.]R.=),RdW.s...
+00001e30: 2f86 279f 0bdf dd91 9f19 1d7b 61b0 5f0c  /.'........{a._.
+00001e40: 837f 1956 31ee 355b bdd3 3146 fa62 a03d  ...V1.5[..1F.b.=
+00001e50: 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c b3fe  .......'=A)..l..
+00001e60: 8eb3 8f89 0188 129d f9b1 c9d7 d1ce 1a19  ................
+00001e70: 6620 8a85 054a 9162 e10c f5d9 1a14 1ca3  f ...J.b........
+00001e80: 71d4 6c8d 4ea7 f118 86e3 666b 7c3a 865d  q.l.N.....fk|:.]
+00001e90: ce21 43a6 382c dc13 ef81 e209 f50c 9b62  .!C.8,.........b
+00001ea0: f633 670a 0532 57d1 9de1 1839 9366 6b72  .3g..2W....9.fkr
+00001eb0: 3a39 f3e9 d09f 4fef ef46 fe58 e024 5fde  :9....O..F.X.$_.
+00001ec0: 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2 2929  [0#.x..._t....))
+00001ed0: f417 8629 4b5f 486d 16c0 52df 0974 25e9  ...)K_Hm..R..t%.
+00001ee0: 56f3 42c0 e762 3f18 ecae b122 bf6b 4145  V.B..b?....".kAE
+00001ef0: 4cc2 8a6a 58fd fc8a da13 b3eb 5476 13d4  L..jX.......Tv..
+00001f00: 5941 7fa9 1175 5a0c 136a f0c0 b80d b4be  YA...uZ..j......
+00001f10: d21a f713 d729 ed7b c6ce 5f50 4b03 0414  .....).{.._PK...
+00001f20: 0000 0008 0052 6372 5855 85c6 84f8 0200  .....RcrXU......
+00001f30: 003f 0a00 0019 0000 0078 6c2f 776f 726b  .?.......xl/work
+00001f40: 7368 6565 7473 2f73 6865 6574 3130 2e78  sheets/sheet10.x
+00001f50: 6d6c bd56 db72 da30 10fd 15c6 cf4e 0c4c  ml.V.r.0.....N.L
+00001f60: 7319 c630 c39d b4a1 a581 a48f 1e21 2f58  s..0.........!/X
+00001f70: 4596 1c69 1d9a bfef ca24 24cd d861 ca03  E..i.....$$..a..
+00001f80: 2f20 ad74 76cf 91b4 eb0d b7da 6c6c 0280  / .tv.......ll..
+00001f90: b53f a954 b6ed 2588 592b 082c 4f20 65f6  .?.T..%.Y+.,O e.
+00001fa0: 5c67 a068 65a5 4dca 90a6 661d d8cc 008b  \g.he.M...f.....
+00001fb0: 0b50 2a83 66bd 7e19 a44c 28af 1316 b699  .P*.f.~..L(.....
+00001fc0: e984 3a47 2914 cc4c cde6 69ca cc73 0fa4  ..:G)..L..i..s..
+00001fd0: deb6 bd86 f76a b813 eb04 0b43 d009 33b6  .....j.....C..3.
+00001fe0: 8639 e07d 4600 9a06 7b3f b148 4159 a155  .9.}F...{?.HAY.U
+00001ff0: cdc0 aaed 751b add9 0e51 ec78 10b0 b5ef  ....u....Q.x....
+00002000: c635 2766 a9f5 c64d 6ee2 b657 779c 4002  .5'f...Mn..Ww.@.
+00002010: 47e7 82d1 df13 f441 4ae7 8998 3cbe 38f5  G......AJ...<.8.
+00002020: de82 3ae4 fbf1 abfb 51a1 9fe8 2d99 85be  ..:.....Q...-...
+00002030: 96bf 448c 49db bbf6 6a31 ac58 2ef1 4e6f  ..D.I...j1.X..No
+00002040: 27f0 a2e9 e28d e280 21eb 8446 6f6b c689  '.......!..Fok..
+00002050: ed84 dc0d 5c48 da28 943b a439 1ab2 0b8a  ....\H.(.;.9....
+00002060: 841d 048b 11a8 a730 4062 e16c 017f c1f4  .......0@b.l....
+00002070: aa30 8f39 98e7 089f 3328 41f5 3f8d c4ac  .0.9....3(A.?...
+00002080: 05b4 25b0 4115 8cae 9e6b 150b 77a0 65c0  ..%.A....k..w.e.
+00002090: 6165 3cc3 3211 21a4 9964 58c6 7454 85e4  ae<.2.!..dX.tT..
+000020a0: 3acd b402 554a 74fc a93e 4e97 15e9 e56f  :...UJt..>N....o
+000020b0: 286e be04 3e39 0cb7 3a37 bc0c 7b73 184b  (n..>9..:7..{s.K
+000020c0: a715 0b4e 7a23 c5d2 321f 5fff c787 884b  ...Nz#..2._....K
+000020d0: 3c7c 3bec 41a8 2cc7 72f4 ed61 b4c9 9502  <|;.A.,.r..a....
+000020e0: 13d1 4341 a1d6 6577 30ad 7252 1af2 7bd5  ..CA..ew0.rR..{.
+000020f0: ee8a 23fa 51b5 3f06 cb8d c8dc 4b2c 81cd  ..#.Q.?.....K,..
+00002100: 2a95 b18f 2202 4acf d79c dfe5 6b4c bf0f  *...".J.....kL..
+00002110: 4c0a fa77 efbc c675 aec8 d9a5 f771 695f  L..w...u.....qi_
+00002120: 439a ad6e a3fe e5fa e2ea 92ea 4aa2 b703  C..n........J...
+00002130: a3b3 81de 2a57 830a c38d bb84 2958 4ba5  ....*W......)XK.
+00002140: 6e6f 1c1a a3cd 7b23 9354 267b 92a9 4d51  no....{#.T&{..MQ
+00002150: 1a5d 52b7 3d29 2c52 6457 8273 c91a 1d2f  .]R.=),RdW.s.../
+00002160: 8627 9f0b dfdd 919f 191d 7b61 b05f 0c83  .'........{a._..
+00002170: 7f19 5631 ee35 5bbd d331 46fa 62a0 3d86  ..V1.5[..1F.b.=.
+00002180: e7b0 d91a 9e8e 273d 4129 b4a1 6cb3 fe8e  ......'=A)..l...
+00002190: b38f 8901 8812 9df9 b1c9 d7d1 ce1a 1966  ...............f
+000021a0: 208a 8505 4a91 62e1 0cf5 d91a 141c a371   ...J.b........q
+000021b0: d46c 8d4e a7f1 1886 e366 6b7c 3a86 5dce  .l.N.....fk|:.].
+000021c0: 2143 a638 2cdc 13ef 81e2 09f5 0c9b 62f6  !C.8,.........b.
+000021d0: 3367 0a05 3257 d19d e118 3993 666b 723a  3g..2W....9.fkr:
+000021e0: 39f3 e9d0 9f4f efef 46fe 58e0 245f de5b  9....O..F.X.$_.[
+000021f0: 3023 8078 c9f8 c65f 74fb 8b9d c229 29f4  0#.x..._t....)).
+00002200: 1786 294b 5f48 6d16 c052 df09 7425 e956  ..)K_Hm..R..t%.V
+00002210: f342 c0e7 623f 18ec aeb1 22bf 6b41 454c  .B..b?....".kAEL
+00002220: c28a 6a58 fdfc 8ada 13b3 eb54 7613 d459  ..jX.......Tv..Y
+00002230: 417f a911 755a 0c13 6af0 c0b8 0db4 bed2  A...uZ..j.......
+00002240: 1af7 13d7 29ed 7bc6 ce5f 504b 0304 1400  ....).{.._PK....
+00002250: 0000 0800 5263 7258 3013 165e 0d03 0000  ....RcrX0..^....
+00002260: b30a 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+00002270: 6865 6574 732f 7368 6565 7431 312e 786d  heets/sheet11.xm
+00002280: 6cbd 5651 53db 300c fe2b bd3c 67a4 f406  l.VQS.0..+.<g...
+00002290: e37a 69ef a005 5a46 3728 657b ccb9 8eda  .zi...ZF7(e{....
+000022a0: 7875 accc 56e8 f8f7 9353 288c 4bca 8d87  xu..V....S(.K...
+000022b0: beb4 b6ec 4ffa 3e5b 5614 afd1 ae5c 0640  ....O.>[V....\.@
+000022c0: ad3f b936 ae17 6444 4537 8a9c cc20 17ee  .?.6..dDE7... ..
+000022d0: 000b 30bc b240 9b0b e2a9 5d46 aeb0 20d2  ..0..@....]F.. .
+000022e0: 0a94 eba8 d36e 1f47 b950 26e8 c795 edc6  .....n.G.P&.....
+000022f0: f663 2c49 2b03 37b6 e5ca 3c17 f6f1 0c34  .c,I+.7...<....4
+00002300: ae7b c161 f06c 98aa 6546 9521 eac7 8558  .{.a.l..eF.!...X
+00002310: c21d d07d c100 9e46 5b3f a9ca c138 85a6  ...}...F[?...8..
+00002320: 6561 d10b 4e0f bbd3 0da2 daf1 43c1 dabd  ea..N.......C...
+00002330: 1ab7 bc98 39e2 ca4f c669 2f68 7b4e a041  ....9..O.i/h{N.A
+00002340: 9277 21f8 ef01 06a0 b5f7 c44c 7e3f 390d  .w!........L~?9.
+00002350: 5e82 7ae4 ebf1 b3fb 8b4a 3fd3 9b0b 0703  ^.z......J?.....
+00002360: d43f 554a 592f 3809 5a29 2c44 a969 8aeb  .?UJY/8.Z),D.i..
+00002370: 113c 693a 7aa1 3814 24fa b1c5 75cb 7ab1  .<i:z.8.$...u.z.
+00002380: fd58 fa81 0fc9 1b95 f187 7447 96ed 8a23  .X........tG...#
+00002390: 519f ac28 54f2 00d6 6b8e 2362 2a7e 2192  Q..(T...k.#b*~!.
+000023a0: 4fc0 b326 e05c 219b 563b a083 c698 e028  O..&.\!.V;.....(
+000023b0: 01f3 5083 1936 617e 9760 1f13 7a2c a006  ..P..6a~.`..z,..
+000023c0: 75be 3392 700e c8d5 c02e 9a60 9c6e 124d  u.3.p......`.n.M
+000023d0: aafc 25d6 012f 779f 2641 5e68 4175 4c47  ..%../w.&A^hAuLG
+000023e0: 4d48 8979 8106 4c2d d1f1 4e7d 9213 24c1  MH.y..L-..N}..$.
+000023f0: f92f a8b2 ad06 7ef5 3edc 6169 651d f6eb  ./....~.>.aie...
+00002400: fb58 3ead 5449 d69b 1891 d7f9 b8fe 1f1f  .X>.TI..........
+00002410: 2aad f130 79df 8332 4549 f5e8 6fef a36d  *..0y..2EI..o..m
+00002420: 690c d884 1385 9459 d6dd c1f7 2627 b521  i......Y....&'.!
+00002430: 6f9a 7637 1cd1 6dd3 fe14 9cb4 aaa0 fa27  o.v7..m........'
+00002440: 366d 5426 de8a 88b8 243c d799 4d8d 48f9  6mT&....$<..M.H.
+00002450: f787 d08a ff7d 9eb7 2496 869d 1d07 6f97  .....}..$.....o.
+00002460: 9eeb d6a0 d31d 1cb6 3f9f 1c7d 39e6 5a96  ........?..}9.Z.
+00002470: e17a 68b1 18e2 daf8 ba57 19c6 fe12 26e0  .zh......W....&.
+00002480: 1c97 d7ad f1dc 5ab4 af8d 4273 693e d3c2  ......Z...Bsi>..
+00002490: acaa 72ec 1f75 2fd0 ca11 47f6 65bf d4e2  ..r..u/...G.e...
+000024a0: b01f a4f0 104a 15fa 3b0a 0b8b 6910 47db  .....J..;...i.G.
+000024b0: c538 fa97 6113 e361 a73b dc1f 63e2 af14  .8..a..a.;..c...
+000024c0: b98f f0bc ec74 2ff7 c793 5350 2bb4 fcda  .....t/...SP+...
+000024d0: 5cb8 e11c 5266 0192 0c8b 30b5 e532 d958  \...Rf....0..2.X
+000024e0: 132b 2c24 a972 c04f a45a f844 f869 0906  .+,$.r.O.Z.D.i..
+000024f0: 3ea2 71d4 e98e f6a7 f123 0cc7 9dee 787f  >.q......#....x.
+00002500: 0c4f a584 8284 9130 f329 7e06 4666 dca7  .O.....0.)~.Ff..
+00002510: acaa d96d 290c 2912 bea2 7bc3 47e4 5c75  ...m).)...{.G.\u
+00002520: ba57 fb93 7337 390f ef26 f7d3 8bf0 52d1  .W..s79..&....R.
+00002530: a89c df3b b017 00e9 5cc8 5538 3b1d cc36  ...;....\.U8;..6
+00002540: 0a27 ac30 9c59 611c 7f21 d1ce 40e4 a117  .'.0.Ya..!..@...
+00002550: e84b d235 ca4a c06e b16f 0c6e d3cc b1df  .K.5.J.n.o.n....
+00002560: a5e2 22a6 61c1 35ac 7df0 855b 22bb e98e  ..".a.5.}..["...
+00002570: 3613 c2a2 a23f 4722 ccab 61c6 4d25 58bf  6....?G"..a.M%X.
+00002580: 81d7 1788 b49d f8ee 6cdb a7f6 ff02 504b  ........l.....PK
+00002590: 0304 1400 0000 0800 5263 7258 5585 c684  ........RcrXU...
+000025a0: f802 0000 3f0a 0000 1900 0000 786c 2f77  ....?.......xl/w
+000025b0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+000025c0: 322e 786d 6cbd 56db 72da 3010 fd15 c6cf  2.xml.V.r.0.....
+000025d0: 4e0c 4c73 19c6 30c3 9db4 a1a5 81a4 8f1e  N.Ls..0.........
+000025e0: 212f 5845 961c 691d 9abf efca 2424 cdd8  !/XE..i.....$$..
+000025f0: 61ca 032f 20ad 7476 cf91 b4eb 0db7 da6c  a../ .tv.......l
+00002600: 6c02 80b5 3fa9 54b6 ed25 8859 2b08 2c4f  l...?.T..%.Y+.,O
+00002610: 2065 f65c 67a0 6865 a54d ca90 a666 1dd8   e.\g.he.M...f..
+00002620: cc00 8b0b 502a 8366 bd7e 19a4 4c28 af13  ....P*.f.~..L(..
+00002630: 16b6 99e9 843a 4729 14cc 4ccd e669 cacc  .....:G)..L..i..
+00002640: 730f a4de b6bd 86f7 6ab8 13eb 040b 43d0  s.......j.....C.
+00002650: 0933 b686 39e0 7d46 009a 067b 3fb1 4841  .3..9.}F...{?.HA
+00002660: 59a1 55cd c0aa ed75 1bad d90e 51ec 7810  Y.U....u....Q.x.
+00002670: b0b5 efc6 3527 66a9 f5c6 4d6e e2b6 5777  ....5'f...Mn..Ww
+00002680: 9c40 0247 e782 d1df 13f4 414a e789 983c  .@.G......AJ...<
+00002690: be38 f5de 823a e4fb f1ab fb51 a19f e82d  .8...:.....Q...-
+000026a0: 9985 be96 bf44 8c49 dbbb f66a 31ac 582e  .....D.I...j1.X.
+000026b0: f14e 6f27 f0a2 e9e2 8de2 8021 eb84 466f  .No'.......!..Fo
+000026c0: 6bc6 89ed 84dc 0d5c 48da 2894 3ba4 391a  k......\H.(.;.9.
+000026d0: b20b 8a84 1d04 8b11 a8a7 3040 62e1 6c01  ..........0@b.l.
+000026e0: 7fc1 f4aa 308f 3998 e708 9f33 2841 f53f  ....0.9....3(A.?
+000026f0: 8dc4 ac05 b425 b041 158c ae9e 6b15 0b77  .....%.A....k..w
+00002700: a065 c061 653c c332 1121 a499 6458 c674  .e.ae<.2.!..dX.t
+00002710: 5485 e43a cdb4 0255 4a74 fca9 3e4e 9715  T..:...UJt..>N..
+00002720: e9e5 6f28 6ebe 043e 390c b73a 37bc 0c7b  ..o(n..>9..:7..{
+00002730: 7318 4ba7 150b 4e7a 23c5 d232 1f5f ffc7  s.K...Nz#..2._..
+00002740: 8788 4b3c 7c3b ec41 a82c c772 f4ed 61b4  ..K<|;.A.,.r..a.
+00002750: c995 0213 d143 41a1 d665 7730 ad72 521a  .....CA..ew0.rR.
+00002760: f27b d5ee 8a23 fa51 b53f 06cb 8dc8 dc4b  .{...#.Q.?.....K
+00002770: 2c81 cd2a 95b1 8f22 024a cfd7 9cdf e56b  ,..*...".J.....k
+00002780: 4cbf 0f4c 0afa 77ef bcc6 75ae c8d9 a5f7  L..L..w...u.....
+00002790: 7169 5f43 9aad 6ea3 fee5 fae2 ea92 ea4a  qi_C..n........J
+000027a0: a2b7 03a3 b381 de2a 5783 0ac3 8dbb 8429  .......*W......)
+000027b0: 584b a56e 6f1c 1aa3 cd7b 2393 5426 7b92  XK.no....{#.T&{.
+000027c0: a94d 511a 5d52 b73d 292c 5264 5782 73c9  .MQ.]R.=),RdW.s.
+000027d0: 1a1d 2f86 279f 0bdf dd91 9f19 1d7b 61b0  ../.'........{a.
+000027e0: 5f0c 837f 1956 31ee 355b bdd3 3146 fa62  _....V1.5[..1F.b
+000027f0: a03d 86e7 b0d9 1a9e 8e27 3d41 29b4 a16c  .=.......'=A)..l
+00002800: b3fe 8eb3 8f89 0188 129d f9b1 c9d7 d1ce  ................
+00002810: 1a19 6620 8a85 054a 9162 e10c f5d9 1a14  ..f ...J.b......
+00002820: 1ca3 71d4 6c8d 4ea7 f118 86e3 666b 7c3a  ..q.l.N.....fk|:
+00002830: 865d ce21 43a6 382c dc13 ef81 e209 f50c  .].!C.8,........
+00002840: 9b62 f633 670a 0532 57d1 9de1 1839 9366  .b.3g..2W....9.f
+00002850: 6b72 3a39 f3e9 d09f 4fef ef46 fe58 e024  kr:9....O..F.X.$
+00002860: 5fde 5b30 2380 78c9 f8c6 5f74 fb8b 9dc2  _.[0#.x..._t....
+00002870: 2929 f417 8629 4b5f 486d 16c0 52df 0974  ))...)K_Hm..R..t
+00002880: 25e9 56f3 42c0 e762 3f18 ecae b122 bf6b  %.V.B..b?....".k
+00002890: 4145 4cc2 8a6a 58fd fc8a da13 b3eb 5476  AEL..jX.......Tv
+000028a0: 13d4 5941 7fa9 1175 5a0c 136a f0c0 b80d  ..YA...uZ..j....
+000028b0: b4be d21a f713 d729 ed7b c6ce 5f50 4b03  .......).{.._PK.
+000028c0: 0414 0000 0008 0052 6372 5855 85c6 84f8  .......RcrXU....
+000028d0: 0200 003f 0a00 0019 0000 0078 6c2f 776f  ...?.......xl/wo
+000028e0: 726b 7368 6565 7473 2f73 6865 6574 3133  rksheets/sheet13
+000028f0: 2e78 6d6c bd56 db72 da30 10fd 15c6 cf4e  .xml.V.r.0.....N
+00002900: 0c4c 7319 c630 c39d b4a1 a581 a48f 1e21  .Ls..0.........!
+00002910: 2f58 4596 1c69 1d9a bfef ca24 24cd d861  /XE..i.....$$..a
+00002920: ca03 2f20 ad74 76cf 91b4 eb0d b7da 6c6c  ../ .tv.......ll
+00002930: 0280 b53f a954 b6ed 2588 592b 082c 4f20  ...?.T..%.Y+.,O 
+00002940: 65f6 5c67 a068 65a5 4dca 90a6 661d d8cc  e.\g.he.M...f...
+00002950: 008b 0b50 2a83 66bd 7e19 a44c 28af 1316  ...P*.f.~..L(...
+00002960: b699 e984 3a47 2914 cc4c cde6 69ca cc73  ....:G)..L..i..s
+00002970: 0fa4 deb6 bd86 f76a b813 eb04 0b43 d009  .......j.....C..
+00002980: 33b6 8639 e07d 4600 9a06 7b3f b148 4159  3..9.}F...{?.HAY
+00002990: a155 cdc0 aaed 751b add9 0e51 ec78 10b0  .U....u....Q.x..
+000029a0: b5ef c635 2766 a9f5 c64d 6ee2 b657 779c  ...5'f...Mn..Ww.
+000029b0: 4002 47e7 82d1 df13 f441 4ae7 8998 3cbe  @.G......AJ...<.
+000029c0: 38f5 de82 3ae4 fbf1 abfb 51a1 9fe8 2d99  8...:.....Q...-.
+000029d0: 85be 96bf 448c 49db bbf6 6a31 ac58 2ef1  ....D.I...j1.X..
+000029e0: 4e6f 27f0 a2e9 e28d e280 21eb 8446 6f6b  No'.......!..Fok
+000029f0: c689 ed84 dc0d 5c48 da28 943b a439 1ab2  ......\H.(.;.9..
+00002a00: 0b8a 841d 048b 11a8 a730 4062 e16c 017f  .........0@b.l..
+00002a10: c1f4 aa30 8f39 98e7 089f 3328 41f5 3f8d  ...0.9....3(A.?.
+00002a20: c4ac 05b4 25b0 4115 8cae 9e6b 150b 77a0  ....%.A....k..w.
+00002a30: 65c0 6165 3cc3 3211 21a4 9964 58c6 7454  e.ae<.2.!..dX.tT
+00002a40: 85e4 3acd b402 554a 74fc a93e 4e97 15e9  ..:...UJt..>N...
+00002a50: e56f 286e be04 3e39 0cb7 3a37 bc0c 7b73  .o(n..>9..:7..{s
+00002a60: 184b a715 0b4e 7a23 c5d2 321f 5fff c787  .K...Nz#..2._...
+00002a70: 884b 3c7c 3bec 41a8 2cc7 72f4 ed61 b4c9  .K<|;.A.,.r..a..
+00002a80: 9502 13d1 4341 a1d6 6577 30ad 7252 1af2  ....CA..ew0.rR..
+00002a90: 7bd5 ee8a 23fa 51b5 3f06 cb8d c8dc 4b2c  {...#.Q.?.....K,
+00002aa0: 81cd 2a95 b18f 2202 4acf d79c dfe5 6b4c  ..*...".J.....kL
+00002ab0: bf0f 4c0a fa77 efbc c675 aec8 d9a5 f771  ..L..w...u.....q
+00002ac0: 695f 439a ad6e a3fe e5fa e2ea 92ea 4aa2  i_C..n........J.
+00002ad0: b703 a3b3 81de 2a57 830a c38d bb84 2958  ......*W......)X
+00002ae0: 4ba5 6e6f 1c1a a3cd 7b23 9354 267b 92a9  K.no....{#.T&{..
+00002af0: 4d51 1a5d 52b7 3d29 2c52 6457 8273 c91a  MQ.]R.=),RdW.s..
+00002b00: 1d2f 8627 9f0b dfdd 919f 191d 7b61 b05f  ./.'........{a._
+00002b10: 0c83 7f19 5631 ee35 5bbd d331 46fa 62a0  ....V1.5[..1F.b.
+00002b20: 3d86 e7b0 d91a 9e8e 273d 4129 b4a1 6cb3  =.......'=A)..l.
+00002b30: fe8e b38f 8901 8812 9df9 b1c9 d7d1 ce1a  ................
+00002b40: 1966 208a 8505 4a91 62e1 0cf5 d91a 141c  .f ...J.b.......
+00002b50: a371 d46c 8d4e a7f1 1886 e366 6b7c 3a86  .q.l.N.....fk|:.
+00002b60: 5dce 2143 a638 2cdc 13ef 81e2 09f5 0c9b  ].!C.8,.........
+00002b70: 62f6 3367 0a05 3257 d19d e118 3993 666b  b.3g..2W....9.fk
+00002b80: 723a 39f3 e9d0 9f4f efef 46fe 58e0 245f  r:9....O..F.X.$_
+00002b90: de5b 3023 8078 c9f8 c65f 74fb 8b9d c229  .[0#.x..._t....)
+00002ba0: 29f4 1786 294b 5f48 6d16 c052 df09 7425  )...)K_Hm..R..t%
+00002bb0: e956 f342 c0e7 623f 18ec aeb1 22bf 6b41  .V.B..b?....".kA
+00002bc0: 454c c28a 6a58 fdfc 8ada 13b3 eb54 7613  EL..jX.......Tv.
+00002bd0: d459 417f a911 755a 0c13 6af0 c0b8 0db4  .YA...uZ..j.....
+00002be0: bed2 1af7 13d7 29ed 7bc6 ce5f 504b 0304  ......).{.._PK..
+00002bf0: 1400 0000 0800 5263 7258 2359 55fc e301  ......RcrX#YU...
+00002c00: 0000 0704 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
+00002c10: 6b73 6865 6574 732f 7368 6565 7431 342e  ksheets/sheet14.
+00002c20: 786d 6c8d 536d 6fda 3010 fe2b 913f 5735  xml.Smo.0..+.?W5
+00002c30: 54eb 8b50 12a9 40d1 3a8d ad2a 1bd3 3e21  T..P..@.:..*..>!
+00002c40: 935c 8885 e3cb eccb b2fe fb9d 13a0 a081  .\..............
+00002c50: b44f be7b fcdc e37b 73dc a2db fa12 80a2  .O.{...{s.......
+00002c60: 3f95 b13e 1125 513d 92d2 6725 54ca 5f63  ?..>.%Q=..g%T._c
+00002c70: 0d96 6f0a 7495 2276 dd46 fada 81ca bba0  ..o.t."v.F......
+00002c80: cac8 9bc1 e04e 564a 5b91 c61d f6e2 d218  .....NVJ[.......
+00002c90: 1b32 dac2 8b8b 7c53 55ca bd8d c160 9b88  .2....|SU....`..
+00002ca0: a1d8 03af 7a53 5207 c834 aed5 0616 40df  ....zSR..4....@.
+00002cb0: 6b0e 6057 1e74 725d 81f5 1a6d e4a0 48c4  k.`W.tr]...m..H.
+00002cc0: e370 34eb 233a c652 43eb 8fec 2814 b346  .p4.#:.RC...(..F
+00002cd0: dc06 e739 4fc4 20e4 0406 320a 128a 8fdf  ...9O. ...2.....
+00002ce0: 3001 6382 1267 f26b 272a de1f 0d91 c7f6  0.c..g.k'*......
+00002cf0: 5e7e d6d5 cfe9 ad95 8709 9a1f 3aa7 3211  ^~..........:.2.
+00002d00: 0f22 caa1 508d a157 6c3f c2ae a6db f714  ."..P..Wl?......
+00002d10: a78a 541a 3b6c 2317 8a4d e32c 18e1 4926  ..T.;l#..M.,..I&
+00002d20: 6a1b 9ab4 20c7 b8e6 9728 25f0 b4ca 3966  j... ....(%...9f
+00002d30: 5568 032b 8399 2274 b124 ce29 3064 b653  Uh.+.."t.$.)0d.S
+00002d40: 18ff a742 3fb7 3302 934b 023a 3fc3 9e5e  ...B?.3..K.:?..^
+00002d50: 625b 55c1 19fe d325 7e0e 3e73 ba0e f338  b[U....%~.>s...8
+00002d60: 1336 bb58 95da f853 bee4 9eee 07d5 3739  .6.X...S......79
+00002d70: 14bd 5446 f3c9 ea3e cab0 b1d4 37fd f46a  ..TF...>....7..j
+00002d80: 3ff8 f1cd 683c 1c7c 78b8 bdbf e365 28b1  ?...h<.|x....e(.
+00002d90: 9d3a aca7 d8da b038 1df0 6ceb 86e6 e03d  .:.....8..l....=
+00002da0: efe7 017c 720e dd31 a80c eff6 d828 bbed  ...|r..1.....(..
+00002db0: f699 de6a c68d f6c4 2f87 fe37 460d 53f1  ...j..../..7F.S.
+00002dc0: 6db1 bcfa f938 ff7c f569 f1f5 8b88 e5e1  m....8.|.i......
+00002dd0: 2696 a7e9 fd03 f8fe 83cc 95db 68ae cb40  &...........h..@
+00002de0: c165 0dae ef79 cd5c bf71 bd43 5877 09ac  .e...y.\.q.CXw..
+00002df0: 9108 abce 2cf9 a382 0b04 be2f 10e9 e084  ....,....../....
+00002e00: 8d3f fcfd f42f 504b 0304 1400 0000 0800  .?.../PK........
+00002e10: 5263 7258 bc72 e0e6 ff01 0000 8104 0000  RcrX.r..........
+00002e20: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00002e30: 732f 7368 6565 7431 352e 786d 6c7d 54db  s/sheet15.xml}T.
+00002e40: 6edb 300c fd15 43cf 4195 14eb 0581 63a0  n.0...C.A.....c.
+00002e50: 49da a5c0 0214 2dda 3d16 8a4c c742 749b  I.....-.=..L.Bt.
+00002e60: 44cf ebdf 8fb2 9334 dd92 3c59 3ce2 2179  D......4..<Y<.!y
+00002e70: 44d2 79eb c226 d600 98fd 31da c609 ab11  D.y..&....1.....
+00002e80: fd98 f328 6b30 225e 380f 966e 2a17 8c40  ...(k0"^8..n*..@
+00002e90: 32c3 9a47 1f40 941d c968 7e39 1c5e 7323  2..G.@...h~9.^s#
+00002ea0: 9465 45de 614f a1c8 5d83 5a59 780a 596c  .eE.aO..].ZYx.Yl
+00002eb0: 8c11 e163 0ada b513 3662 3be0 59ad 6bec  ...c....6b;.Y.k.
+00002ec0: 005e e45e ace1 05f0 d513 814c be8f 532a  .^.^.......L..S*
+00002ed0: 0336 2a67 b300 d584 dd8d c68b 9ed1 79bc  .6*g..........y.
+00002ee0: 2968 e3c1 394b 6256 ce6d 92f1 584e d830  )h..9KbV.m..XN.0
+00002ef0: d504 1a24 a610 823e bf61 065a a748 54c9  ...$...>.a.Z.HT.
+00002f00: af6d 50f6 9934 310f cfbb f00f 9d7e 2a6f  .mP..41......~*o
+00002f10: 2522 cc9c fea9 4aac 27ec 9665 2554 a2d1  %"....J.'..e%T..
+00002f20: f8ec da05 6c35 5d7d 9638 1728 8a3c b836  ....l5]}.8.(.<.6
+00002f30: 0b49 6c91 cb74 4829 c951 d9f4 482f 1808  .Il..tH).Q..H/..
+00002f40: 5794 090b 8488 ef06 5094 c4cb 3952 29e9  W.......P...9R).
+00002f50: 82cb 2d71 7a96 e821 4467 8ff1 6667 7992  ..-qz..!Dg..fgy.
+00002f60: 34c5 23ac f959 566c 14c2 7bf4 2055 a5a4  4.#..YVl..{. U..
+00002f70: 484f 7c24 c6fd a918 aa3c e2fd 70ca db0a  HO|$.....<..p...
+00002f80: 0347 fcbf 9ff2 2f21 caa0 fc89 a216 2785  .G..../!......'.
+00002f90: 89f5 3f0f c1a9 77bb 81e8 9b99 5af3 26b4  ..?...w.....Z.&.
+00002fa0: 2a3b c931 93ae b1d8 37f7 ebd5 6ec0 a697  *;.1....7...n...
+00002fb0: e3e9 68f8 edf6 eae6 9a86 ae76 ed3c 383f  ..h........v.<8?
+00002fc0: 77ad 4d03 da01 8fd6 37b8 8418 690f f6e0  w.M.....7...i...
+00002fd0: 7d08 2e1c 8242 d30e 4db5 b09b 6e6f f0c3  }....B..M...no..
+00002fe0: 13ae 5544 ca9c f6b3 d162 54b0 3bad 0733  ..UD.....bT.;..3
+00002ff0: d245 2dd1 831f b40c af7e b004 590b 4b9e  .E-......~..Y.K.
+00003000: 4ab2 9cef 7d73 feb5 e0ff 80d8 afe6 5284  J...}s........R.
+00003010: b522 a51a 2a12 3abc b8a1 010f fdac f706  ."..*.:.........
+00003020: 3adf 95b4 7288 ce74 c79a 7e11 1092 03dd  :...r..t..~.....
+00003030: 57ce e1de 48bb b6ff eb14 7f01 504b 0304  W...H.......PK..
+00003040: 1400 0000 0800 5263 7258 bc72 e0e6 ff01  ......RcrX.r....
+00003050: 0000 8104 0000 1900 0000 786c 2f77 6f72  ..........xl/wor
+00003060: 6b73 6865 6574 732f 7368 6565 7431 362e  ksheets/sheet16.
+00003070: 786d 6c7d 54db 6edb 300c fd15 43cf 4195  xml}T.n.0...C.A.
+00003080: 14eb 0581 63a0 49da a5c0 0214 2dda 3d16  ....c.I.....-.=.
+00003090: 8a4c c742 749b 44cf ebdf 8fb2 9334 dd92  .L.Bt.D......4..
+000030a0: 3c59 3ce2 2179 44d2 79eb c226 d600 98fd  <Y<.!yD.y..&....
+000030b0: 31da c609 ab11 fd98 f328 6b30 225e 380f  1........(k0"^8.
+000030c0: 966e 2a17 8c40 32c3 9a47 1f40 941d c968  .n*..@2..G.@...h
+000030d0: 7e39 1c5e 7323 9465 45de 614f a1c8 5d83  ~9.^s#.eE.aO..].
+000030e0: 5a59 780a 596c 8c11 e163 0ada b513 3662  ZYx.Yl...c....6b
+000030f0: 3be0 59ad 6bec 005e e45e ace1 05f0 d513  ;.Y.k..^.^......
+00003100: 814c be8f 532a 0336 2a67 b300 d584 dd8d  .L..S*.6*g......
+00003110: c68b 9ed1 79bc 2968 e3c1 394b 6256 ce6d  ....y.)h..9KbV.m
+00003120: 92f1 584e d830 d504 1a24 a610 823e bf61  ..XN.0...$...>.a
+00003130: 065a a748 54c9 af6d 50f6 9934 310f cfbb  .Z.HT..mP..41...
+00003140: f00f 9d7e 2a6f 2522 cc9c fea9 4aac 27ec  ...~*o%"....J.'.
+00003150: 9665 2554 a2d1 f8ec da05 6c35 5d7d 9638  .e%T......l5]}.8
+00003160: 1728 8a3c b836 0b49 6c91 cb74 4829 c951  .(.<.6.Il..tH).Q
+00003170: d9f4 482f 1808 5794 090b 8488 ef06 5094  ..H/..W.......P.
+00003180: c4cb 3952 29e9 82cb 2d71 7a96 e821 4467  ..9R)...-qz..!Dg
+00003190: 8ff1 6667 7992 34c5 23ac f959 566c 14c2  ..fgy.4.#..YVl..
+000031a0: 7bf4 2055 a5a4 484f 7c24 c6fd a918 aa3c  {. U..HO|$.....<
+000031b0: e2fd 70ca db0a 0347 fcbf 9ff2 2f21 caa0  ..p....G..../!..
+000031c0: fc89 a216 2785 89f5 3f0f c1a9 77bb 81e8  ....'...?...w...
+000031d0: 9b99 5af3 26b4 2a3b c931 93ae b1d8 37f7  ..Z.&.*;.1....7.
+000031e0: ebd5 6ec0 a697 e3e9 68f8 edf6 eae6 9a86  ..n.....h.......
+000031f0: ae76 ed3c 383f 77ad 4d03 da01 8fd6 37b8  .v.<8?w.M.....7.
+00003200: 8418 690f f6e0 7d08 2e1c 8242 d30e 4db5  ..i...}....B..M.
+00003210: b09b 6e6f f0c3 13ae 5544 ca9c f6b3 d162  ..no....UD.....b
+00003220: 54b0 3bad 0733 d245 2dd1 831f b40c af7e  T.;..3.E-......~
+00003230: b004 590b 4b9e 4ab2 9cef 7d73 feb5 e0ff  ..Y.K.J...}s....
+00003240: 80d8 afe6 5284 b522 a51a 2a12 3abc b8a1  ....R.."..*.:...
+00003250: 010f fdac f706 3adf 95b4 7288 ce74 c79a  ......:...r..t..
+00003260: 7e11 1092 03dd 57ce e1de 48bb b6ff eb14  ~.....W...H.....
+00003270: 7f01 504b 0304 1400 0000 0800 5263 7258  ..PK........RcrX
+00003280: 953b a42f 1101 0000 c801 0000 1900 0000  .;./............
+00003290: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+000032a0: 6565 7431 372e 786d 6c4d 51cb 6ec3 2010  eet17.xmlMQ.n. .
+000032b0: fc15 8b0f 084e a53e 14d9 96d2 5455 7ba8  .....N.>....TU{.
+000032c0: 14a5 6a7b c6f1 da46 0196 c2ba 6eff be80  ..j{...F....n...
+000032d0: 6327 2776 7677 8619 2846 7427 df03 50f6  c''vvw..(Ft'..P.
+000032e0: ab95 f125 eb89 ec86 737f ec41 0bbf 420b  ...%....s..A..B.
+000032f0: 264c 5a74 5a50 80ae e3de 3a10 4d22 69c5  &LZtZP....:.M"i.
+00003300: 6ff2 fc8e 6b21 0dab 8ad4 dbbb aac0 8194  o...k!..........
+00003310: 34b0 7799 1fb4 16ee ef11 148e 255b b3b9  4.w.........%[..
+00003320: 7190 5d4f a9c1 abc2 8a0e de81 3e6c 2004  q.]O........>l .
+00003330: c817 9d46 6a30 5ea2 c91c b425 dbae 37db  ...Fj0^....%..7.
+00003340: 8991 363e 258c feaa ce62 981a f114 c16b  ..6>%....b.....k
+00003350: 53b2 3c7a 0205 478a 1222 1c3f b003 a5a2  S.<z..G..".?....
+00003360: 5270 f27d 1665 974b 23f3 ba9e e59f 53fe  Rp.}.e.K#.....S.
+00003370: 60af 161e 76a8 be64 437d c91e 58d6 402b  `...v..dC}..X.@+
+00003380: 0645 071c 5fe0 9ce9 f662 f149 9098 13be  .E.._....b.I....
+00003390: 09d7 49e3 3305 6dd8 ca57 f761 cf4d 9409  ..I.3.m..W.a.M..
+000033a0: 10da f422 3512 a14e 651f 5e1a 5c5c 08f3  ..."5..Ne.^.\\..
+000033b0: 1691 1610 2d2f 9f57 fd03 504b 0304 1400  ....-/.W..PK....
+000033c0: 0000 0800 5263 7258 bc72 e0e6 ff01 0000  ....RcrX.r......
+000033d0: 8104 0000 1900 0000 786c 2f77 6f72 6b73  ........xl/works
+000033e0: 6865 6574 732f 7368 6565 7431 382e 786d  heets/sheet18.xm
+000033f0: 6c7d 54db 6edb 300c fd15 43cf 4195 14eb  l}T.n.0...C.A...
+00003400: 0581 63a0 49da a5c0 0214 2dda 3d16 8a4c  ..c.I.....-.=..L
+00003410: c742 749b 44cf ebdf 8fb2 9334 dd92 3c59  .Bt.D......4..<Y
+00003420: 3ce2 2179 44d2 79eb c226 d600 98fd 31da  <.!yD.y..&....1.
+00003430: c609 ab11 fd98 f328 6b30 225e 380f 966e  .......(k0"^8..n
+00003440: 2a17 8c40 32c3 9a47 1f40 941d c968 7e39  *..@2..G.@...h~9
+00003450: 1c5e 7323 9465 45de 614f a1c8 5d83 5a59  .^s#.eE.aO..].ZY
+00003460: 780a 596c 8c11 e163 0ada b513 3662 3be0  x.Yl...c....6b;.
+00003470: 59ad 6bec 005e e45e ace1 05f0 d513 814c  Y.k..^.^.......L
+00003480: be8f 532a 0336 2a67 b300 d584 dd8d c68b  ..S*.6*g........
+00003490: 9ed1 79bc 2968 e3c1 394b 6256 ce6d 92f1  ..y.)h..9KbV.m..
+000034a0: 584e d830 d504 1a24 a610 823e bf61 065a  XN.0...$...>.a.Z
+000034b0: a748 54c9 af6d 50f6 9934 310f cfbb f00f  .HT..mP..41.....
+000034c0: 9d7e 2a6f 2522 cc9c fea9 4aac 27ec 9665  .~*o%"....J.'..e
+000034d0: 2554 a2d1 f8ec da05 6c35 5d7d 9638 1728  %T......l5]}.8.(
+000034e0: 8a3c b836 0b49 6c91 cb74 4829 c951 d9f4  .<.6.Il..tH).Q..
+000034f0: 482f 1808 5794 090b 8488 ef06 5094 c4cb  H/..W.......P...
+00003500: 3952 29e9 82cb 2d71 7a96 e821 4467 8ff1  9R)...-qz..!Dg..
+00003510: 6667 7992 34c5 23ac f959 566c 14c2 7bf4  fgy.4.#..YVl..{.
+00003520: 2055 a5a4 484f 7c24 c6fd a918 aa3c e2fd   U..HO|$.....<..
+00003530: 70ca db0a 0347 fcbf 9ff2 2f21 caa0 fc89  p....G..../!....
+00003540: a216 2785 89f5 3f0f c1a9 77bb 81e8 9b99  ..'...?...w.....
+00003550: 5af3 26b4 2a3b c931 93ae b1d8 37f7 ebd5  Z.&.*;.1....7...
+00003560: 6ec0 a697 e3e9 68f8 edf6 eae6 9a86 ae76  n.....h........v
+00003570: ed3c 383f 77ad 4d03 da01 8fd6 37b8 8418  .<8?w.M.....7...
+00003580: 690f f6e0 7d08 2e1c 8242 d30e 4db5 b09b  i...}....B..M...
+00003590: 6e6f f0c3 13ae 5544 ca9c f6b3 d162 54b0  no....UD.....bT.
+000035a0: 3bad 0733 d245 2dd1 831f b40c af7e b004  ;..3.E-......~..
+000035b0: 590b 4b9e 4ab2 9cef 7d73 feb5 e0ff 80d8  Y.K.J...}s......
+000035c0: afe6 5284 b522 a51a 2a12 3abc b8a1 010f  ..R.."..*.:.....
+000035d0: fdac f706 3adf 95b4 7288 ce74 c79a 7e11  ....:...r..t..~.
+000035e0: 1092 03dd 57ce e1de 48bb b6ff eb14 7f01  ....W...H.......
+000035f0: 504b 0304 1400 0000 0800 5263 7258 bc72  PK........RcrX.r
+00003600: e0e6 ff01 0000 8104 0000 1900 0000 786c  ..............xl
+00003610: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00003620: 7431 392e 786d 6c7d 54db 6edb 300c fd15  t19.xml}T.n.0...
+00003630: 43cf 4195 14eb 0581 63a0 49da a5c0 0214  C.A.....c.I.....
+00003640: 2dda 3d16 8a4c c742 749b 44cf ebdf 8fb2  -.=..L.Bt.D.....
+00003650: 9334 dd92 3c59 3ce2 2179 44d2 79eb c226  .4..<Y<.!yD.y..&
+00003660: d600 98fd 31da c609 ab11 fd98 f328 6b30  ....1........(k0
+00003670: 225e 380f 966e 2a17 8c40 32c3 9a47 1f40  "^8..n*..@2..G.@
+00003680: 941d c968 7e39 1c5e 7323 9465 45de 614f  ...h~9.^s#.eE.aO
+00003690: a1c8 5d83 5a59 780a 596c 8c11 e163 0ada  ..].ZYx.Yl...c..
+000036a0: b513 3662 3be0 59ad 6bec 005e e45e ace1  ..6b;.Y.k..^.^..
+000036b0: 05f0 d513 814c be8f 532a 0336 2a67 b300  .....L..S*.6*g..
+000036c0: d584 dd8d c68b 9ed1 79bc 2968 e3c1 394b  ........y.)h..9K
+000036d0: 6256 ce6d 92f1 584e d830 d504 1a24 a610  bV.m..XN.0...$..
+000036e0: 823e bf61 065a a748 54c9 af6d 50f6 9934  .>.a.Z.HT..mP..4
+000036f0: 310f cfbb f00f 9d7e 2a6f 2522 cc9c fea9  1......~*o%"....
+00003700: 4aac 27ec 9665 2554 a2d1 f8ec da05 6c35  J.'..e%T......l5
+00003710: 5d7d 9638 1728 8a3c b836 0b49 6c91 cb74  ]}.8.(.<.6.Il..t
+00003720: 4829 c951 d9f4 482f 1808 5794 090b 8488  H).Q..H/..W.....
+00003730: ef06 5094 c4cb 3952 29e9 82cb 2d71 7a96  ..P...9R)...-qz.
+00003740: e821 4467 8ff1 6667 7992 34c5 23ac f959  .!Dg..fgy.4.#..Y
+00003750: 566c 14c2 7bf4 2055 a5a4 484f 7c24 c6fd  Vl..{. U..HO|$..
+00003760: a918 aa3c e2fd 70ca db0a 0347 fcbf 9ff2  ...<..p....G....
+00003770: 2f21 caa0 fc89 a216 2785 89f5 3f0f c1a9  /!......'...?...
+00003780: 77bb 81e8 9b99 5af3 26b4 2a3b c931 93ae  w.....Z.&.*;.1..
+00003790: b1d8 37f7 ebd5 6ec0 a697 e3e9 68f8 edf6  ..7...n.....h...
+000037a0: eae6 9a86 ae76 ed3c 383f 77ad 4d03 da01  .....v.<8?w.M...
+000037b0: 8fd6 37b8 8418 690f f6e0 7d08 2e1c 8242  ..7...i...}....B
+000037c0: d30e 4db5 b09b 6e6f f0c3 13ae 5544 ca9c  ..M...no....UD..
+000037d0: f6b3 d162 54b0 3bad 0733 d245 2dd1 831f  ...bT.;..3.E-...
+000037e0: b40c af7e b004 590b 4b9e 4ab2 9cef 7d73  ...~..Y.K.J...}s
+000037f0: feb5 e0ff 80d8 afe6 5284 b522 a51a 2a12  ........R.."..*.
+00003800: 3abc b8a1 010f fdac f706 3adf 95b4 7288  :.........:...r.
+00003810: ce74 c79a 7e11 1092 03dd 57ce e1de 48bb  .t..~.....W...H.
+00003820: b6ff eb14 7f01 504b 0304 1400 0000 0800  ......PK........
+00003830: 5263 7258 4f5c d595 6901 0000 e702 0000  RcrXO\..i.......
+00003840: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+00003850: 732f 7368 6565 7432 302e 786d 6c75 52d9  s/sheet20.xmluR.
+00003860: 4ec3 400c fc95 683f 806d 9138 5425 91e8  N.@...h?.m.8T%..
+00003870: 81e0 01a9 6a05 3c56 dbc4 4956 dd23 785d  ....j.<V..IV.#x]
+00003880: 027f 8f37 3d85 daa7 d8de 99b1 3d71 da79  ...7=.......=q.y
+00003890: dc84 0680 921f 6b5c c844 43d4 8ea4 0c45  ......k\.DC....E
+000038a0: 0356 851b df82 e397 caa3 55c4 29d6 32b4  .V........U.).2.
+000038b0: 08aa ec49 d6c8 dbc1 e05e 5aa5 9dc8 d3be  ...I.....^Z.....
+000038c0: 36c7 3cf5 5b32 dac1 1c93 b0b5 56e1 ef18  6.<.[2......V...
+000038d0: 8cef 3231 1487 c242 d70d f505 99a7 adaa  ..21...B........
+000038e0: 6109 f4de 3281 5379 d429 b505 17b4 7709  a...2.Sy.)....w.
+000038f0: 4295 89a7 e168 b663 f488 0f0d 5d38 8b93  B....h.c....]8..
+00003900: b8cc dafb 4d4c 5ecb 4c0c e24c 60a0 a028  ....ML^.L..L`..(
+00003910: a1f8 f30d 1330 262a f124 5f7b 5171 6a1a  .....0&*.$_{Qqj.
+00003920: 99e7 f141 feb9 df9f c75b ab00 136f 3e75  ...A.....[...o>u
+00003930: 494d 261e 4552 42a5 b686 16be 7b81 fd4e  IM&.ERB.....{..N
+00003940: 77a7 11a7 8a54 9ea2 ef12 8ccb e669 1183  w....T.......i..
+00003950: d892 81da 4593 9684 5cd7 dc89 7282 402b  ....E...\...r.@+
+00003960: dcba 55ab 5059 20c0 904a e281 e2b3 2cf6  ..U.PY ..J....,.
+00003970: f4f1 35ba 2e2f a027 d7d0 8e3b 5cc0 4faf  ..5../.'...;\.O.
+00003980: e14b 0805 ea36 7a79 8136 bbba 93aa ff2d  .K...6zy.6.....-
+00003990: 21d9 8f83 c93b 83e2 01bc 29ac b50b 8981  !....;....).....
+000039a0: 8a75 0637 0f6c 23ee 1cdd 25e4 dbfe 60d6  .u.7.l#...%...`.
+000039b0: 9ec8 db3e 6cf8 1001 2380 df2b efe9 98c4  ...>l...#..+....
+000039c0: 3f7a bced fc0f 504b 0304 1400 0000 0800  ?z....PK........
+000039d0: 5263 7258 7d51 27cc ea01 0000 4504 0000  RcrX}Q'.....E...
+000039e0: 1900 0000 786c 2f77 6f72 6b73 6865 6574  ....xl/worksheet
+000039f0: 732f 7368 6565 7432 312e 786d 6c85 544d  s/sheet21.xml.TM
+00003a00: 6fdb 300c fd2b 86ce 4395 14eb 0702 c7c0  o.0..+..C.......
+00003a10: 92b4 5d0f 058a 166b 8f81 62d3 b110 59d2  ..]....k..b...Y.
+00003a20: 447a 5eff fd28 3949 132c d92e 36f9 c447  Dz^..(9I.,..6..G
+00003a30: 3d9a a4f3 de85 0d36 0094 fd6e 8dc5 a968  =......6...n...h
+00003a40: 88fc 444a 2c1b 6815 5e38 0f96 4f6a 175a  ..DJ,.h.^8..Oj.Z
+00003a50: 45ec 86b5 441f 4055 89d4 1a79 391a 5dcb  E...D.@U...y9.].
+00003a60: 5669 2b8a 3c61 cfa1 c85d 4746 5b78 0e19  Vi+.<a...]GF[x..
+00003a70: 766d abc2 c70c 8ceb a762 2c76 c08b 5e37  vm.......b,v..^7
+00003a80: 9400 59e4 5ead e115 e887 6702 bb72 9fa7  ..Y.^.....g..r..
+00003a90: d22d 58d4 ce66 01ea a9f8 369e 3c0c 8c14  .-X..f....6.<...
+00003aa0: f1a6 a1c7 033b 8bc5 ac9c db44 e7b1 9a8a  .....;.....D....
+00003ab0: 51d4 0406 4a8a 2914 bf7e c11c 8c89 9958  Q...J.)..~.....X
+00003ac0: c9cf 6d52 f179 6964 1eda bbf4 f7a9 7e96  ..mR.yid......~.
+00003ad0: b752 0873 67de 7545 cd54 dc8a ac82 5a75  .R.sg.uE.T....Zu
+00003ae0: 865e 5cff 1db6 355d 7d4a 5c28 5245 1e5c  .^\...5]}J\(RE.\
+00003af0: 9f85 586c 9197 d188 5772 a0b6 f123 bd52  ..Xl....Wr...#.R
+00003b00: 605c f34d 5410 202d b1d3 044b 5de5 9258  `\.MT. -...K]..X
+00003b10: 4a3c 90e5 9638 fb27 b164 6d27 48f3 ff92  J<...8.'.dm'H...
+00003b20: 9601 906b 38c1 5d9c e39e 9477 772e daaa  ...k8.]....ww...
+00003b30: f694 b2fb 73f1 1560 19b4 8f6d 3b41 7b38  ....s..`...m;A{8
+00003b40: 5b90 5ae3 71bc e44f bfeb e7d0 8b8a 9f6f  [.Z.q..O.......o
+00003b50: ca68 7e73 76cc 4ad7 591a 7a73 7cb4 9b8f  .h~sv.J.Y.zs|...
+00003b60: f9e5 643e 1e7d bdbd bab9 e699 695c bf08  ..d>.}......i\..
+00003b70: ce2f 5c6f e37c 25e0 d1fa 8e9e 0091 c778  ./\o.|%........x
+00003b80: 0fde 85e0 c221 a80c afc0 cc28 bb49 634f  .....!.....(.IcO
+00003b90: 1f9e 71a3 91f8 e6b8 5e9d 51e3 42a4 9e78  ..q.....^.Q.B..x
+00003ba0: 8508 d597 64d7 4a9b 9d8d 1bed 3d54 2297  ....d.J.....=T".
+00003bb0: 7b42 2e8f 55ff 05e0 b05e 4f2a ac35 976b  {B..U....^O*.5.k
+00003bc0: a0e6 6a47 1737 3ca4 6198 d7c1 21e7 93ae  ..jG.7<.a...!...
+00003bd0: 9523 726d 321b 5e73 0831 80cf 6be7 68ef  .#rm2.^s.1..k.h.
+00003be0: c47d d9ff 398a 3f50 4b03 0414 0000 0008  .}..9.?PK.......
+00003bf0: 0052 6372 58d4 5695 de87 0100 008f 0300  .RcrX.V.........
+00003c00: 0019 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00003c10: 7473 2f73 6865 6574 3232 2e78 6d6c 7d93  ts/sheet22.xml}.
+00003c20: db4e c330 0c86 5fa5 ca03 900d 8983 a6b6  .N.0.._.........
+00003c30: 128c c3b8 409a 8680 cb29 6bdd 3622 87e2  ....@....)k.6"..
+00003c40: 7814 de1e a73b 8050 cb55 6dc7 9fe3 3f76  x....;.P.Um...?v
+00003c50: d3ce e35b 6800 28f9 b4c6 854c 3444 ed4c  ...[h.(....L4D.L
+00003c60: ca50 3460 5538 f12d 383e a93c 5a45 ec62  .P4`U8.-8>.<ZE.b
+00003c70: 2d43 8ba0 ca1e b246 9e4e 26e7 d22a ed44  -C.....F.N&..*.D
+00003c80: 9ef6 b125 e6a9 df92 d10e 9698 84ad b50a  ...%............
+00003c90: bfae c1f8 2e13 5371 08ac 74dd 501f 9079  ......Sq..t.P..y
+00003ca0: daaa 1a9e 809e 5b06 d895 c73a a5b6 e082  ......[....:....
+00003cb0: f62e 41a8 3271 359d 2d76 449f f1a2 a10b  ..A.2q5.-vD.....
+00003cc0: bfec 248a d978 ff16 9d87 3213 93d8 1318  ..$..x....2.....
+00003cd0: 2828 9650 fcf9 8039 1813 2b71 27ef fba2  ((.P...9..+q'...
+00003ce0: e2e7 d248 feb6 0fe5 ef7a fddc de46 0598  ...H.....z...F..
+00003cf0: 7bf3 aa4b 6a32 7129 9212 2ab5 35b4 f2dd  {..Kj2q)..*.5...
+00003d00: 02f6 9ace 7e5a bc51 a4f2 147d 9760 149b  ....~Z.Q...}.`..
+00003d10: a745 34e2 959c a85d 7ca4 2742 8e6b be89  .E4....]|.'B.k..
+00003d20: 7282 406b dc3a 07b8 76ca 422a 89bb 8967  r.@k.:..v.B*...g
+00003d30: b2d8 b3d7 ffb2 e048 9386 3000 ceff 050b  .......H..0.....
+00003d40: d6b5 4608 2c65 08be 1985 7942 8194 6d07  ..F.,e....yB..m.
+00003d50: a0db 3148 9703 d977 63d9 230f 713f 965f  ..1H...wc.#.q?._
+00003d60: 4228 50b7 71e6 03d8 6254 89aa ff28 973c  B(P.q...bT...(.<
+00003d70: b7c3 32ec 0619 17f5 5161 ad5d 480c 545c  ..2.....Qa.]H.T\
+00003d80: 6772 72c1 e3c6 dde4 770e f9b6 5fec 8d27  grr.....w..._..'
+00003d90: f2b6 371b fe61 0063 029f 57de d3d1 899b  ..7..a.c..W.....
+00003da0: 77fc 07f3 6f50 4b03 0414 0000 0008 0052  w...oPK........R
+00003db0: 6372 58c4 ce01 8a6c 0100 000f 0300 0019  crX....l........
+00003dc0: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
+00003dd0: 2f73 6865 6574 3233 2e78 6d6c 7553 db6e  /sheet23.xmluS.n
+00003de0: 8330 0cfd 1594 0f58 e8a4 5d54 01d2 daae  .0.....X..]T....
+00003df0: da1e 2655 adb6 3d56 2918 889a 0b4b dcb1  ..&U..=V)....K..
+00003e00: fdfd 1ce8 4d13 3c61 3be7 1cfb 3821 69ad  ....M.<a;...8!i.
+00003e10: dbfb 1a00 a31f ad8c 4f59 8dd8 4c39 f779  ........OY..L9.y
+00003e20: 0d5a f81b db80 a193 d23a 2d90 5257 71df  .Z.......:-.RWq.
+00003e30: 3810 4547 d28a dfc6 f13d d742 1a96 255d  8.EG.....=.B..%]
+00003e40: 6de5 b2c4 1e50 4903 2b17 f983 d6c2 fdce  m....PI.+.......
+00003e50: 40d9 3665 1376 2aac 6555 6357 e059 d288  @.6e.v*.eUcW.Y..
+00003e60: 0a36 80ef 0d11 28e5 679d 426a 305e 5a13  .6....(.g.Bj0^Z.
+00003e70: 3928 53f6 3499 2e7b 4687 f890 d0fa ab38  9(S.4..{F......8
+00003e80: 0a66 76d6 ee43 f25a a42c 0e33 8182 1c83  .fv..C.Z.,.3....
+00003e90: 84a0 cf37 cc41 a9a0 4493 7c1d 45d9 a569  ...7.A..D.|.E..i
+00003ea0: 605e c727 f965 e79f c6db 090f 73ab 3e65  `^.'.e......s.>e
+00003eb0: 8175 ca1e 5954 4029 0e0a d7b6 7d81 a3a7  .u..YT@)....}...
+00003ec0: bbcb 880b 8122 4b9c 6d23 17cc 6649 1e82  ....."K.m#..fI..
+00003ed0: d092 80d2 8425 6dd0 515d 5227 cc10 3c6e  .....%m.Q]R'..<n
+00003ee0: 736a b195 45c2 9126 0975 9e1f 79b3 315e  sj..E..&.u..y.1^
+00003ef0: b3f7 03f0 f918 7c50 7c31 8636 42c3 00fe  ......|P|1.6B...
+00003f00: 790c 5f80 cf9d 6cc2 ce07 68cb 51ef a2fa  y._...l...h.Q...
+00003f10: 6782 d3de 4e97 d12f 323c 9437 e12a 697c  g...N../2<.7.*i|
+00003f20: a4a0 249d f8e6 81d6 edfa cdf7 09da a67b  ..$............{
+00003f30: 583b 8b68 7517 d6f4 60c1 0500 9d97 d6e2  X;.hu...`.......
+00003f40: 3909 377f fe07 b23f 504b 0304 1400 0000  9.7....?PK......
+00003f50: 0800 5263 7258 1b56 7ebc 9c01 0000 0d04  ..RcrX.V~.......
+00003f60: 0000 1900 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00003f70: 6574 732f 7368 6565 7432 342e 786d 6c7d  ets/sheet24.xml}
+00003f80: 94db 6adc 3010 865f c5e8 01a2 4da1 0782  ..j.0.._....M...
+00003f90: 6d68 364d 9386 4248 687a 59b4 f6d8 162b  mh6M..BHhzY....+
+00003fa0: 69d4 d16c 9cbe 7d25 ef21 2948 bdf2 ccf8  i..l..}%.!)H....
+00003fb0: ff46 33e6 97eb 1969 1b26 00ae 5eac 71a1  .F3....i.&..^.q.
+00003fc0: 1113 b3bf 9032 7413 5815 ced0 838b 6f06  .....2t.X.....o.
+00003fd0: 24ab 38a6 34ca e009 54bf 40d6 c877 abd5  $.8.4...T.@..w..
+00003fe0: 0769 9576 a2ad 97da 3db5 35ee d868 07f7  .i.v....=.5..h..
+00003ff0: 5485 9db5 8afe 5c82 c1b9 11e7 e258 78d0  T.....\......Xx.
+00004000: e3c4 4b41 b6b5 5723 3c02 fff0 1188 a93c  ..KA..W#<......<
+00004010: f5e9 b505 1734 ba8a 6068 c4e7 f38b bb3d  .....4..`h.....=
+00004020: b128 9e34 cce1 4d5c a565 3688 db94 dcf6  .(.4..M\.e6.....
+00004030: 8d58 a599 c040 c7a9 858a 8f67 5883 31a9  .X...@.....gX.1.
+00004040: 539c e4f7 a1a9 783d 3491 6fe3 63fb eb65  S.....x=4.o.c..e
+00004050: ff38 de46 0558 a3f9 a97b 9e1a f149 543d  .8.F.X...{...IT=
+00004060: 0c6a 67f8 01e7 1b38 ecf4 fe75 c42b c5aa  .jg....8...u.+..
+00004070: ad09 e78a d2b2 6ddd a520 1d19 85da a58f  ......m.. ......
+00004080: f4c8 14eb 3a9e c4ad 5704 8e7f f96d 2d39  ....:...W....m-9
+00004090: 8e91 8ab2 3b40 9725 c802 8dd0 e7a1 7509  ....;@.%......u.
+000040a0: 52a4 4624 9741 aefe 83bc 64f4 5f4a fa9d  R.F$.A....d._J..
+000040b0: 0bd0 1170 86b9 2e31 1b86 8cfc 6b49 aead  ...p...1....kI..
+000040c0: 277c d66e cc40 3745 a8cf a86f 4b6a a76c  '|.n.@7E...oKj.l
+000040d0: 6ea4 6f25 7d0f a123 ed93 e332 d85d 0963  n.o%}..#...2.].c
+000040e0: 3586 7ff5 32ba e668 c5bd 8dd2 35f9 ae68  5...2..h....5..h
+000040f0: d42e 5406 86d8 6775 f631 9a8d f6be db27  ..T...gu.1.....'
+00004100: 8c7e b956 1b64 46bb 8453 bcae 4049 10df  .~.V.dF..S..@I..
+00004110: 0f88 7c4a 92ef 4f7f 80f6 2f50 4b03 0414  ..|J..O.../PK...
+00004120: 0000 0008 0052 6372 58d2 05f1 4652 0200  .....RcrX...FR..
+00004130: 0047 0a00 000d 0000 0078 6c2f 7374 796c  .G.......xl/styl
+00004140: 6573 2e78 6d6c dd56 db8a db30 10fd 15e3  es.xml.V...0....
+00004150: 0fa8 9398 9ab8 2479 a821 5068 cbc2 ee43  ......$y.!Ph...C
+00004160: 5fe5 584e 04ba b8b2 bc24 fdfa 6a24 e7b6  _.XN.....$..j$..
+00004170: 9be3 52fa 569b e099 393a 3367 a431 ceaa  ..R.V...9:3g.1..
+00004180: 7727 c99f 0f9c bbe4 a8a4 eed7 e9c1 b9ee  w'..............
+00004190: 5396 f5bb 0357 acff 603a ae3d d21a ab98  S....W..`:.=....
+000041a0: f3ae dd67 7d67 396b 7a22 2999 2d66 b322  ...g}g9kz").-f."
+000041b0: 534c e874 b3d2 83da 2ad7 273b 3368 b74e  SL.t....*.';3h.N
+000041c0: 6769 926d 56ad d1d7 d03c 8d01 bf96 299e  gi.mV....<....).
+000041d0: bc32 b94e 2b26 456d 455c cc94 90a7 185f  .2.N+&EmE\....._
+000041e0: 84c8 ce48 6313 e7d5 70a2 53a8 ff15 17cc  ...Hc...p.S.....
+000041f0: 4797 a48e b994 d0c6 8668 16cb 8447 ef13  G........h...G..
+00004200: 0b29 2f2a 1669 0c6c 561d 738e 5bbd f54e  .)/*.i.lV.s.[..N
+00004210: 2485 e87b 6cb4 5f4e 9d57 b1b7 ec34 5f7c  $..{l._N.W...4_|
+00004220: 4c6f 18e1 e1cb d4c6 36dc deb5 1b43 9b95  Lo......6....C..
+00004230: e4ad 2386 15fb 4330 9ce9 e851 1be7 8c22  ..#...C0...Q..."
+00004240: ab11 6c6f 348b 4ace b4d1 f0b9 775c ca67  ..lo4.J.....w\.g
+00004250: 3aaf 1fed 5d81 639b c48d ffd2 843d a78e  :...].c......=..
+00004260: cfa6 5735 9a31 cde8 5081 db74 31f9 bfe7  ..W5.1..P..t1...
+00004270: edc4 ab71 9f07 df90 0efe cfc1 38fe 6479  ...q........8.dy
+00004280: 2b8e c13f b66f 045c 6a07 2577 e52f d184  +..?.o.\j.%w./..
+00004290: 4665 9d7e a711 9437 39ea 4148 27f4 e81d  Fe.~...79.AH'...
+000042a0: 44d3 70fd be3b 9fdf b1da 0ff9 5d01 bfaa  D.p..;......]...
+000042b0: e12d 1ba4 7bb9 80eb f46a 7fe3 8d18 5479  .-..{....j....Ty
+000042c0: 59f5 448d 8dab aef6 573a ca79 719d 535f  Y.D.....W:.yq.S_
+000042d0: 4ce8 861f 7953 8dae ddd7 c14c bce1 cb8e  L...yS.....L....
+000042e0: 5760 bc85 b6e1 0210 6445 1040 04c2 5a50  W`......dE.@..ZP
+000042f0: 0664 451e acf5 3ff6 b5c4 7d45 102a 5c3e  .dE...?...}E.*\>
+00004300: 8696 98b5 c4ac c87b 0855 e186 b500 abf4  .......{.U......
+00004310: 1768 b92c f3bc 28e0 f656 d563 1915 dcc3  .h.,..(..V.c....
+00004320: a2a0 1f48 0815 1207 d6a2 6a7f bbf3 1303  ...H......j.....
+00004330: 3031 367f 980d 78ca 9363 035b 9e18 51d8  016...x..c.[..Q.
+00004340: f2c4 ce13 04f6 9038 6509 0600 d622 0e3c  .......8e....".<
+00004350: 1438 5124 02d4 a251 03ac 3ca7 7386 0ae1  .8Q$...Q..<.s...
+00004360: 6b3e 0195 2584 6848 c1f4 1605 daa8 826e  k>..%.hH.......n
+00004370: 705e f025 caf3 b204 1081 4046 9e43 885e  p^.%......@F.C.^
+00004380: d809 08ca 2021 10ca f3f8 217d f33d cbce  .... !....!}.=..
+00004390: dfb9 ecfa d771 f31b 504b 0304 1400 0000  .....q..PK......
+000043a0: 0800 5263 7258 b747 eb8a c000 0000 1602  ..RcrX.G........
+000043b0: 0000 0b00 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+000043c0: 739d 924b 6e02 310c 40af 1265 5f4c a9c4  s..Kn.1.@..e_L..
+000043d0: 0231 acd8 b043 880b b889 e7a3 99c4 9163  .1...C.........c
+000043e0: c4f4 f68d d8c0 2068 114b ff9e 9e2d af0f  ...... h.K...-..
+000043f0: 34a0 761c 73db a56c c630 c45c d956 35ad  4.v.s..l.0.\.V5.
+00004400: 00b2 6b29 609e 71a2 582a 354b 402d a134  ..k)`.q.X*5K@-.4
+00004410: 90d0 f5d8 102c e6f3 25c8 2dc3 6ed6 b74c  .....,..%.-.n..L
+00004420: 73fc 49f4 0a91 ebba 73b4 6577 0a14 f501  s.I.....s.ew....
+00004430: f8ae c39a 234a 435a d971 8033 4bff cddc  ....#JCZ.q.3K...
+00004440: cf0a d49a 9daf acec fca7 35f0 a6cc f3f5  ..........5.....
+00004450: 2090 a247 4570 2cf4 91a4 4c8b 7694 af3e   ..GEp,...L.v..>
+00004460: 9edd bea4 f3a5 6362 b478 dfe8 fff3 d0a8  ......cb.x......
+00004470: 143d f9bf 9d30 a589 d2d7 4509 266f b0f9  .=...0....E.&o..
+00004480: 0550 4b03 0414 0000 0008 0052 6372 5821  .PK........RcrX!
+00004490: 0fd9 4c7b 0200 00e5 0800 000f 0000 0078  ..L{...........x
+000044a0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 8d96  l/workbook.xml..
+000044b0: 6d4f db30 1080 ff4a 951f b034 8196 1751  mO.0...J...4...Q
+000044c0: 24d6 3240 6cb4 2388 ef57 e7d2 9c70 ecc8  $.2@l.#..W...p..
+000044d0: 76e8 c6af 9f9d 5048 ebcc dba7 d467 ebe9  v.....PH.....g..
+000044e0: 5dfc 9c9d 8bad 542f 6b29 5f46 bf2a 2ef4  ].....T/k)_F.*..
+000044f0: b99a 45a5 31f5 791c 6b56 6205 fa8b ac51  ..E.1.y.kVb....Q
+00004500: d8b9 42aa 0a8c 1daa 4d2c 8b82 182e 246b  ..B.....M,....$k
+00004510: 2a14 264e c7e3 69ac 9083 2129 7449 b58e  *.&N..i...!)tI..
+00004520: 3ada ffb0 74ad 1072 5d22 9a8a 77a8 0a48  :...t..r]"..w..H
+00004530: 4497 17bb cc56 6a14 f747 d220 73ff e4a2  D....Vj..G. s...
+00004540: 2ef2 4cb8 d59f 0bdc 70f4 4a9a d6c4 c9fc  ..L.....p.J.....
+00004550: 9e45 ed6f 8ed1 a822 4115 bd61 3e8b c6d1  .E.o..."A..a>...
+00004560: 4897 727b 2b15 bd49 6180 674c 49ce 6751  H.r{+..Ia.gLI.gQ
+00004570: d24d 3ca3 32c4 bc70 e6d2 7c82 b56e 2306  .M<.2..p..|..n#.
+00004580: d68f aee6 5934 1d5b 6041 4a9b 7645 cb07  ....Y4.[`AJ.vE..
+00004590: 9be4 2bda c5dd a831 f21b 7183 6a01 066f  ..+....1..q.j..o
+000045a0: 946c 6a12 9b16 63cb 887b 75b4 af62 f71c  .lj...c..{u..b..
+000045b0: 09a8 7016 3da1 36d7 c2d8 7256 a06c c462  ..p.=.6...rV.l.b
+000045c0: 5c42 76c1 5dde 2567 2cb5 57aa 3a27 3ba1  \Bv.].%g,.W.:';.
+000045d0: eef2 8edf 67fd 6c80 5341 7b84 3440 483d  ....g.l.SA{.4@H=
+000045e0: 82cb e607 1ac8 c140 0f72 1480 1c0d 42ae  .......@.r....B.
+000045f0: b446 d323 1c07 08c7 1ee1 8a31 ac0d 0886  .F.#.......1....
+00004600: 43ac 4980 3519 cce6 3adf e062 bfa4 6900  C.I.5...:..b..i.
+00004610: 32f5 202b 854c 8a9c 9c9c 3dc8 4900 7232  2. +.L....=.I.r2
+00004620: 98c9 1c34 f600 a701 c0e9 3f5e cb01 ea2c  ...4......?^...,
+00004630: 803a 1b52 c549 07ad c83e 2c19 87c4 1b7b  .:.R.I...>,....{
+00004640: b8b9 ac6a 4e7f c92c 095a ec6b 7c2f e496  ...jN..,.Z.k|/..
+00004650: a3dd b21b 0575 f900 afb4 69cf 9f21 7448  .....u....i..!tH
+00004660: efc4 f77b 29f0 56d6 43a0 90e2 c9b0 e359  ...{).V.C......Y
+00004670: 4306 b31a 99ed 3906 076a 2421 e313 5ff9  C.....9..j$!.._.
+00004680: 0f60 9f11 323d f155 dff7 c3a3 8594 4f7c  .`..2=.U......O|
+00004690: e7bf a260 6505 ea65 1016 523f f1dd cf6c  ...`e..e..R?...l
+000046a0: 5a39 a85c ef9b e261 430d 91f8 1df1 b99f  Z9.\...aC.......
+000046b0: 1e29 d40f 89df 108e f1d8 0881 6a2e 4541  .)..........j.EA
+000046c0: 9b46 1dee 681a ea89 d4ef 899d 658f a81b  .F..h.......e...
+000046d0: de3f bfd2 503f a47e 3fbc a796 a1d6 0719  .?..P?.~?.......
+000046e0: 050f f7e1 d37d d998 bad9 cb26 647e 3a6c  .....}.....&d~:l
+000046f0: 7e57 d2ea 3edb 3b97 d390 f269 a77c bcbb  ~W..>.;....i.|..
+00004700: 0373 2c48 60fe 6099 da4d d81b 99d9 cf01  .s,H`.`..M......
+00004710: f7e8 1afb 78e2 76a9 6838 9fdb d852 7c97  ....x.v.h8...R|.
+00004720: 907f 5caa bb2f 82cb 3f50 4b03 0414 0000  ..\../..?PK.....
+00004730: 0008 0052 6372 5872 967e 9137 0100 0039  ...RcrXr.~.7...9
+00004740: 0f00 001a 0000 0078 6c2f 5f72 656c 732f  .......xl/_rels/
+00004750: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
+00004760: 73cd d741 8e82 3014 c6f1 ab90 1ec0 f2aa  s..A..0.........
+00004770: a24e c495 1bb7 132f d0e0 1388 4049 dbc9  .N...../....@I..
+00004780: e8ed 87c8 023f 328b d998 792b d212 1eff  .....?2...y+....
+00004790: 45f3 0bec 3fb9 b1b1 765d a8ea 3e24 f7b6  E...?...v]..>$..
+000047a0: e942 aeaa 18fb 0fad 4351 716b c3c2 f5dc  .B......CQqk....
+000047b0: 0d77 aece b736 0e4b 5fea de16 375b b236  .w...6.K_...7[.6
+000047c0: 699a 69ff 3a43 1df6 af33 93f3 a3e7 bf4c  i.i.:C...3.....L
+000047d0: 74d7 6b5d f0d1 155f 2d77 f197 c1fa dbf9  t.k]..._-w......
+000047e0: 5ba8 98a3 4ace d697 1c73 a5ef cdb4 1df4  [...J....s......
+000047f0: f342 8b61 b24a 4e97 5cf9 d385 54a2 ffbb  .B.a.JN.\...T...
+00004800: c840 9111 50b4 84a2 a580 a215 14ad 0414  .@..P...........
+00004810: ada1 682d a028 83a2 4c40 d106 8a36 028a  ..h-.(..L@...6..
+00004820: b650 b415 50b4 83a2 9d80 224a 91c8 5442  .P..P....."J..TB
+00004830: d38c 6d09 6e13 c24d 12e4 26a4 9b24 d84d  ..m.n..M..&..$.M
+00004840: 8837 49d0 9b90 6f92 e037 21e0 2441 7042  .7I...o..7!.$ApB
+00004850: c249 82e1 8488 9304 c509 1927 098e 1b74  .I.........'...t
+00004860: dc48 70dc a0e3 4682 e366 f601 2ec1 7183  .Hp...F..f....q.
+00004870: 8e1b 098e 1b74 dcbc d5f1 101f 0d87 2968  .....t........)h
+00004880: 5c63 c05b d18e c3b3 3cbd ffb9 1c37 6747  \c.[....<....7gG
+00004890: 7864 5ac3 9ff2 e107 504b 0304 1400 0000  xdZ.....PK......
+000048a0: 0800 5263 7258 8b1a e4a4 7101 0000 3510  ..RcrX....q...5.
+000048b0: 0000 1300 0000 5b43 6f6e 7465 6e74 5f54  ......[Content_T
+000048c0: 7970 6573 5d2e 786d 6ccd 98cb 6ec2 3010  ypes].xml...n.0.
+000048d0: 457f 25ca 1611 63b7 a50f 019b b6db 9645  E.%...c........E
+000048e0: 7fc0 4d26 c4c2 2f79 0c85 bfaf 130a 522b  ..M&../y......R+
+000048f0: ca43 54ea 6c62 259e b9f7 c623 1d29 19bd  .CT.lb%....#.)..
+00004900: ad3d 60b6 32da e238 6f62 f40f 8c61 d980  .=`.2..8ob...a..
+00004910: 9158 380f 36ed d42e 1819 d36d 9831 2fcb  .X8.6......m.1/.
+00004920: b99c 0113 83c1 9095 ce46 b0b1 1f5b 8d7c  .........F...[.|
+00004930: 327a 825a 2e74 cc9e 57e9 312a 67c7 7900  2z.Z.t..W.1*g.y.
+00004940: 8d79 f6b8 296c bdc6 b9f4 5eab 52c6 b4cf  .y..)l....^.R...
+00004950: 96b6 fae1 d2ff 7228 5267 5783 8df2 d84b  ......r(RgW....K
+00004960: 0579 c6f6 5a74 5bbf 3a6c 1b5f 9710 82aa  .y..Zt[.:l._....
+00004970: 209b ca10 5fa4 4965 6ca5 19c6 b506 2c0e   ..._.Iel.....,.
+00004980: 6bec 49e9 ea5a 9550 b972 6152 4b81 3e80  k.I..Z.P.raRK.>.
+00004990: acb0 0188 4617 1bd1 de11 eb98 0e19 3657  ....F.........6W
+000049a0: 7e71 804e e6a0 632a 9d06 e731 4d2d c0f9  ~q.N..c*...1M-..
+000049b0: 7edb b1b4 dd7d 9f84 2044 75e4 2577 9649  ~....}.. Du.%w.I
+000049c0: fbe2 3784 76e2 1554 a79a a713 fe70 61de  ..7.v..T.....pa.
+000049d0: cd04 59b7 5c7e ccdf e7bc d33f 3788 a012  ..Y.\~.....?7...
+000049e0: e48a 4a90 6b2a 416e a804 1952 0972 4b25  ..J.k*An...R.rK%
+000049f0: c81d 9520 f754 82f0 0199 2464 d8ca c9c0  ... .T....$d....
+00004a00: 9593 a12b 2783 574e 86af 9c0c 6039 19c2  ...+'.WN....`9..
+00004a10: 7232 88e5 6418 2bc8 3056 9061 ac20 c358  r2..d.+.0V.a. .X
+00004a20: 4186 b1e2 5f19 fbee dcfc afbf 62db b530  A..._.......b..0
+00004a30: 52d9 5d00 d6fd 2d98 7c02 504b 0102 1403  R.]...-.|.PK....
+00004a40: 1400 0000 0800 5263 7258 465a c10c 8200  ......RcrXFZ....
+00004a50: 0000 b100 0000 1000 0000 0000 0000 0000  ................
+00004a60: 0000 8001 0000 0000 646f 6350 726f 7073  ........docProps
+00004a70: 2f61 7070 2e78 6d6c 504b 0102 1403 1400  /app.xmlPK......
+00004a80: 0000 0800 5263 7258 6a72 2c18 ed00 0000  ....RcrXjr,.....
+00004a90: cb01 0000 1100 0000 0000 0000 0000 0000  ................
+00004aa0: 8001 b000 0000 646f 6350 726f 7073 2f63  ......docProps/c
+00004ab0: 6f72 652e 786d 6c50 4b01 0214 0314 0000  ore.xmlPK.......
+00004ac0: 0008 0052 6372 5899 5c9c 2310 0600 009c  ...RcrX.\.#.....
+00004ad0: 2700 0013 0000 0000 0000 0000 0000 0080  '...............
+00004ae0: 01cc 0100 0078 6c2f 7468 656d 652f 7468  .....xl/theme/th
+00004af0: 656d 6531 2e78 6d6c 504b 0102 1403 1400  eme1.xmlPK......
+00004b00: 0000 0800 5263 7258 0f95 4d33 4801 0000  ....RcrX..M3H...
+00004b10: 4902 0000 1800 0000 0000 0000 0000 0000  I...............
+00004b20: 8081 0d08 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00004b30: 6574 732f 7368 6565 7431 2e78 6d6c 504b  ets/sheet1.xmlPK
+00004b40: 0102 1403 1400 0000 0800 5263 7258 0f95  ..........RcrX..
+00004b50: 4d33 4801 0000 4902 0000 1800 0000 0000  M3H...I.........
+00004b60: 0000 0000 0000 8081 8b09 0000 786c 2f77  ............xl/w
+00004b70: 6f72 6b73 6865 6574 732f 7368 6565 7432  orksheets/sheet2
+00004b80: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00004b90: 5263 7258 b111 5547 4002 0000 7805 0000  RcrX..UG@...x...
+00004ba0: 1800 0000 0000 0000 0000 0000 8081 090b  ................
+00004bb0: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00004bc0: 7368 6565 7433 2e78 6d6c 504b 0102 1403  sheet3.xmlPK....
+00004bd0: 1400 0000 0800 5263 7258 2581 7ddb bf02  ......RcrX%.}...
+00004be0: 0000 7308 0000 1800 0000 0000 0000 0000  ..s.............
+00004bf0: 0000 8081 7f0d 0000 786c 2f77 6f72 6b73  ........xl/works
+00004c00: 6865 6574 732f 7368 6565 7434 2e78 6d6c  heets/sheet4.xml
+00004c10: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+00004c20: b356 a83b 9203 0000 8c0d 0000 1800 0000  .V.;............
+00004c30: 0000 0000 0000 0000 8081 7410 0000 786c  ..........t...xl
+00004c40: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00004c50: 7435 2e78 6d6c 504b 0102 1403 1400 0000  t5.xmlPK........
+00004c60: 0800 5263 7258 2581 7ddb bf02 0000 7308  ..RcrX%.}.....s.
+00004c70: 0000 1800 0000 0000 0000 0000 0000 8081  ................
+00004c80: 3c14 0000 786c 2f77 6f72 6b73 6865 6574  <...xl/worksheet
+00004c90: 732f 7368 6565 7436 2e78 6d6c 504b 0102  s/sheet6.xmlPK..
+00004ca0: 1403 1400 0000 0800 5263 7258 642f 605f  ........RcrXd/`_
+00004cb0: 5801 0000 a802 0000 1800 0000 0000 0000  X...............
+00004cc0: 0000 0000 8081 3117 0000 786c 2f77 6f72  ......1...xl/wor
+00004cd0: 6b73 6865 6574 732f 7368 6565 7437 2e78  ksheets/sheet7.x
+00004ce0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+00004cf0: 7258 5585 c684 f802 0000 3f0a 0000 1800  rXU.......?.....
+00004d00: 0000 0000 0000 0000 0000 8081 bf18 0000  ................
+00004d10: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00004d20: 6565 7438 2e78 6d6c 504b 0102 1403 1400  eet8.xmlPK......
+00004d30: 0000 0800 5263 7258 5585 c684 f802 0000  ....RcrXU.......
+00004d40: 3f0a 0000 1800 0000 0000 0000 0000 0000  ?...............
+00004d50: 8081 ed1b 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00004d60: 6574 732f 7368 6565 7439 2e78 6d6c 504b  ets/sheet9.xmlPK
+00004d70: 0102 1403 1400 0000 0800 5263 7258 5585  ..........RcrXU.
+00004d80: c684 f802 0000 3f0a 0000 1900 0000 0000  ......?.........
+00004d90: 0000 0000 0000 8081 1b1f 0000 786c 2f77  ............xl/w
+00004da0: 6f72 6b73 6865 6574 732f 7368 6565 7431  orksheets/sheet1
+00004db0: 302e 786d 6c50 4b01 0214 0314 0000 0008  0.xmlPK.........
+00004dc0: 0052 6372 5830 1316 5e0d 0300 00b3 0a00  .RcrX0..^.......
+00004dd0: 0019 0000 0000 0000 0000 0000 0080 814a  ...............J
+00004de0: 2200 0078 6c2f 776f 726b 7368 6565 7473  "..xl/worksheets
+00004df0: 2f73 6865 6574 3131 2e78 6d6c 504b 0102  /sheet11.xmlPK..
+00004e00: 1403 1400 0000 0800 5263 7258 5585 c684  ........RcrXU...
+00004e10: f802 0000 3f0a 0000 1900 0000 0000 0000  ....?...........
+00004e20: 0000 0000 8081 8e25 0000 786c 2f77 6f72  .......%..xl/wor
+00004e30: 6b73 6865 6574 732f 7368 6565 7431 322e  ksheets/sheet12.
+00004e40: 786d 6c50 4b01 0214 0314 0000 0008 0052  xmlPK..........R
+00004e50: 6372 5855 85c6 84f8 0200 003f 0a00 0019  crXU.......?....
+00004e60: 0000 0000 0000 0000 0000 0080 81bd 2800  ..............(.
+00004e70: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00004e80: 6865 6574 3133 2e78 6d6c 504b 0102 1403  heet13.xmlPK....
+00004e90: 1400 0000 0800 5263 7258 2359 55fc e301  ......RcrX#YU...
+00004ea0: 0000 0704 0000 1900 0000 0000 0000 0000  ................
+00004eb0: 0000 8081 ec2b 0000 786c 2f77 6f72 6b73  .....+..xl/works
+00004ec0: 6865 6574 732f 7368 6565 7431 342e 786d  heets/sheet14.xm
+00004ed0: 6c50 4b01 0214 0314 0000 0008 0052 6372  lPK..........Rcr
+00004ee0: 58bc 72e0 e6ff 0100 0081 0400 0019 0000  X.r.............
+00004ef0: 0000 0000 0000 0000 0080 8106 2e00 0078  ...............x
+00004f00: 6c2f 776f 726b 7368 6565 7473 2f73 6865  l/worksheets/she
+00004f10: 6574 3135 2e78 6d6c 504b 0102 1403 1400  et15.xmlPK......
+00004f20: 0000 0800 5263 7258 bc72 e0e6 ff01 0000  ....RcrX.r......
+00004f30: 8104 0000 1900 0000 0000 0000 0000 0000  ................
+00004f40: 8081 3c30 0000 786c 2f77 6f72 6b73 6865  ..<0..xl/workshe
+00004f50: 6574 732f 7368 6565 7431 362e 786d 6c50  ets/sheet16.xmlP
+00004f60: 4b01 0214 0314 0000 0008 0052 6372 5895  K..........RcrX.
+00004f70: 3ba4 2f11 0100 00c8 0100 0019 0000 0000  ;./.............
+00004f80: 0000 0000 0000 0080 8172 3200 0078 6c2f  .........r2..xl/
+00004f90: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
+00004fa0: 3137 2e78 6d6c 504b 0102 1403 1400 0000  17.xmlPK........
+00004fb0: 0800 5263 7258 bc72 e0e6 ff01 0000 8104  ..RcrX.r........
+00004fc0: 0000 1900 0000 0000 0000 0000 0000 8081  ................
+00004fd0: ba33 0000 786c 2f77 6f72 6b73 6865 6574  .3..xl/worksheet
+00004fe0: 732f 7368 6565 7431 382e 786d 6c50 4b01  s/sheet18.xmlPK.
+00004ff0: 0214 0314 0000 0008 0052 6372 58bc 72e0  .........RcrX.r.
+00005000: e6ff 0100 0081 0400 0019 0000 0000 0000  ................
+00005010: 0000 0000 0080 81f0 3500 0078 6c2f 776f  ........5..xl/wo
+00005020: 726b 7368 6565 7473 2f73 6865 6574 3139  rksheets/sheet19
+00005030: 2e78 6d6c 504b 0102 1403 1400 0000 0800  .xmlPK..........
+00005040: 5263 7258 4f5c d595 6901 0000 e702 0000  RcrXO\..i.......
+00005050: 1900 0000 0000 0000 0000 0000 8081 2638  ..............&8
+00005060: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00005070: 7368 6565 7432 302e 786d 6c50 4b01 0214  sheet20.xmlPK...
+00005080: 0314 0000 0008 0052 6372 587d 5127 ccea  .......RcrX}Q'..
+00005090: 0100 0045 0400 0019 0000 0000 0000 0000  ...E............
+000050a0: 0000 0080 81c6 3900 0078 6c2f 776f 726b  ......9..xl/work
+000050b0: 7368 6565 7473 2f73 6865 6574 3231 2e78  sheets/sheet21.x
+000050c0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+000050d0: 7258 d456 95de 8701 0000 8f03 0000 1900  rX.V............
+000050e0: 0000 0000 0000 0000 0000 8081 e73b 0000  .............;..
+000050f0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00005100: 6565 7432 322e 786d 6c50 4b01 0214 0314  eet22.xmlPK.....
+00005110: 0000 0008 0052 6372 58c4 ce01 8a6c 0100  .....RcrX....l..
+00005120: 000f 0300 0019 0000 0000 0000 0000 0000  ................
+00005130: 0080 81a5 3d00 0078 6c2f 776f 726b 7368  ....=..xl/worksh
+00005140: 6565 7473 2f73 6865 6574 3233 2e78 6d6c  eets/sheet23.xml
+00005150: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+00005160: 1b56 7ebc 9c01 0000 0d04 0000 1900 0000  .V~.............
+00005170: 0000 0000 0000 0000 8081 483f 0000 786c  ..........H?..xl
+00005180: 2f77 6f72 6b73 6865 6574 732f 7368 6565  /worksheets/shee
+00005190: 7432 342e 786d 6c50 4b01 0214 0314 0000  t24.xmlPK.......
+000051a0: 0008 0052 6372 58d2 05f1 4652 0200 0047  ...RcrX...FR...G
+000051b0: 0a00 000d 0000 0000 0000 0000 0000 0080  ................
+000051c0: 011b 4100 0078 6c2f 7374 796c 6573 2e78  ..A..xl/styles.x
+000051d0: 6d6c 504b 0102 1403 1400 0000 0800 5263  mlPK..........Rc
+000051e0: 7258 b747 eb8a c000 0000 1602 0000 0b00  rX.G............
+000051f0: 0000 0000 0000 0000 0000 8001 9843 0000  .............C..
+00005200: 5f72 656c 732f 2e72 656c 7350 4b01 0214  _rels/.relsPK...
+00005210: 0314 0000 0008 0052 6372 5821 0fd9 4c7b  .......RcrX!..L{
+00005220: 0200 00e5 0800 000f 0000 0000 0000 0000  ................
+00005230: 0000 0080 0181 4400 0078 6c2f 776f 726b  ......D..xl/work
+00005240: 626f 6f6b 2e78 6d6c 504b 0102 1403 1400  book.xmlPK......
+00005250: 0000 0800 5263 7258 7296 7e91 3701 0000  ....RcrXr.~.7...
+00005260: 390f 0000 1a00 0000 0000 0000 0000 0000  9...............
+00005270: 8001 2947 0000 786c 2f5f 7265 6c73 2f77  ..)G..xl/_rels/w
+00005280: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
+00005290: 504b 0102 1403 1400 0000 0800 5263 7258  PK..........RcrX
+000052a0: 8b1a e4a4 7101 0000 3510 0000 1300 0000  ....q...5.......
+000052b0: 0000 0000 0000 0000 8001 9848 0000 5b43  ...........H..[C
+000052c0: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+000052d0: 6c50 4b05 0600 0000 0020 0020 0097 0800  lPK...... . ....
+000052e0: 003a 4a00 0000 00                        .:J....
```

### Comparing `translator_testing_model-0.3.1/project/graphql/translator_testing_model.graphql` & `translator_testing_model-2.3.0/project/graphql/translator_testing_model.graphql`

 * *Files 26% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     qualifiers: [Qualifier]
     expectedOutput: String
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
-    testMetadata: TestMetadata
+    runnerSettings: [String]!
+    testMetadata: TestMetadata!
     id: Uriorcurie!
     tags: [String]
-    testRunnerSettings: [String]
     mustPassDate: Date
     mustPassEnvironment: TestEnvEnum
     scientificQuestion: String
     stringEntry: String
     direction: DirectionEnum
     answerInformalConcept: String
     expectedResult: ExpectedResultsEnum
@@ -35,108 +35,160 @@
   }
 
 type AcceptanceTestCase
   {
     id: Uriorcurie!
     name: String
     description: String
-    testRunnerSettings: [String]
+    testEnv: TestEnvEnum
     queryType: QueryTypeEnum
     preconditions: [Precondition]
     trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
     testCaseObjective: TestObjectiveEnum
     testCaseSource: TestSourceEnum
     testCasePredicateName: String
     testCasePredicateId: String
     testCaseInputId: Uriorcurie
-    qualifiers: [Qualifier]
-    inputCategory: ConceptCategory
-    outputCategory: ConceptCategory
-    components: [ComponentEnum]
-    testEnv: TestEnvEnum
+    testCaseRunnerSettings: [String]!
     tags: [String]
     testAssets: [AcceptanceTestAsset]!
   }
 
 type AcceptanceTestSuite
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
-    testMetadata: TestMetadata
+    testMetadata: TestMetadata!
     testPersona: TestPersonaEnum
     testCases: [TestCase]
     testSuiteSpecification: TestSuiteSpecification
   }
 
 type BenchmarkTestSuite
   {
   }
 
+type ComplianceTestCase
+  {
+    id: Uriorcurie!
+    name: String
+    description: String
+    testEnv: TestEnvEnum
+    queryType: QueryTypeEnum
+    testAssets: [TestAsset]!
+    preconditions: [Precondition]
+    trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
+    testCaseObjective: TestObjectiveEnum
+    testCaseSource: TestSourceEnum
+    testCasePredicateName: String
+    testCasePredicateId: String
+    testCaseInputId: Uriorcurie
+    testCaseRunnerSettings: [String]!
+    tags: [String]
+    trapiVersion: String
+    biolinkVersion: String
+  }
+
+type KnowledgeGraphNavigationTestCase
+  {
+    id: Uriorcurie!
+    name: String
+    description: String
+    testEnv: TestEnvEnum
+    queryType: QueryTypeEnum
+    testAssets: [TestAsset]!
+    preconditions: [Precondition]
+    trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
+    testCaseObjective: TestObjectiveEnum
+    testCaseSource: TestSourceEnum
+    testCasePredicateName: String
+    testCasePredicateId: String
+    testCaseInputId: Uriorcurie
+    testCaseRunnerSettings: [String]!
+    tags: [String]
+  }
+
+type OneHopTestCase
+  {
+    id: Uriorcurie!
+    name: String
+    description: String
+    testEnv: TestEnvEnum
+    queryType: QueryTypeEnum
+    testAssets: [TestAsset]!
+    preconditions: [Precondition]
+    trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
+    testCaseObjective: TestObjectiveEnum
+    testCaseSource: TestSourceEnum
+    testCasePredicateName: String
+    testCasePredicateId: String
+    testCaseInputId: Uriorcurie
+    testCaseRunnerSettings: [String]!
+    tags: [String]
+  }
+
 type OneHopTestSuite
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
-    testMetadata: TestMetadata
+    testMetadata: TestMetadata!
     testPersona: TestPersonaEnum
     testCases: [TestCase]
     testSuiteSpecification: TestSuiteSpecification
   }
 
 type Precondition
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
   }
 
 type Qualifier
   {
     parameter: String
     value: String
   }
 
 type QuantitativeTestCase
   {
     id: Uriorcurie!
     name: String
     description: String
-    testRunnerSettings: [String]
+    testEnv: TestEnvEnum
     queryType: QueryTypeEnum
     testAssets: [TestAsset]!
     preconditions: [Precondition]
     trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
     testCaseObjective: TestObjectiveEnum
     testCaseSource: TestSourceEnum
     testCasePredicateName: String
     testCasePredicateId: String
     testCaseInputId: Uriorcurie
-    qualifiers: [Qualifier]
-    inputCategory: ConceptCategory
-    outputCategory: ConceptCategory
-    components: [ComponentEnum]
-    testEnv: TestEnvEnum
+    testCaseRunnerSettings: [String]!
     tags: [String]
   }
 
 type StandardsComplianceTestSuite
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
-    testMetadata: TestMetadata
+    testMetadata: TestMetadata!
     testPersona: TestPersonaEnum
     testCases: [TestCase]
     testSuiteSpecification: TestSuiteSpecification
   }
 
 type TestAsset
   {
@@ -154,50 +206,46 @@
     qualifiers: [Qualifier]
     expectedOutput: String
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
-    testMetadata: TestMetadata
+    runnerSettings: [String]!
+    testMetadata: TestMetadata!
     id: Uriorcurie!
     tags: [String]
-    testRunnerSettings: [String]
   }
 
 type TestCase
   {
     id: Uriorcurie!
     name: String
     description: String
-    testRunnerSettings: [String]
+    testEnv: TestEnvEnum
     queryType: QueryTypeEnum
     testAssets: [TestAsset]!
     preconditions: [Precondition]
     trapiTemplate: TrapiTemplateEnum
+    components: [ComponentEnum]
     testCaseObjective: TestObjectiveEnum
     testCaseSource: TestSourceEnum
     testCasePredicateName: String
     testCasePredicateId: String
     testCaseInputId: Uriorcurie
-    qualifiers: [Qualifier]
-    inputCategory: ConceptCategory
-    outputCategory: ConceptCategory
-    components: [ComponentEnum]
-    testEnv: TestEnvEnum
+    testCaseRunnerSettings: [String]!
     tags: [String]
   }
 
 type TestCaseResult
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
     testSuiteId: Uriorcurie
     testCase: TestCase
     testCaseResult: TestCaseResultEnum
   }
 
 type TestEdgeData
   {
@@ -215,108 +263,107 @@
     qualifiers: [Qualifier]
     expectedOutput: String
     testIssue: TestIssueEnum
     semanticSeverity: SemanticSeverityEnum
     inV1: Boolean
     wellKnown: Boolean
     testReference: Uriorcurie
-    testMetadata: TestMetadata
+    runnerSettings: [String]!
+    testMetadata: TestMetadata!
     id: Uriorcurie!
     tags: [String]
-    testRunnerSettings: [String]
   }
 
 interface TestEntity
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
   }
 
 type TestEntityParameter
   {
     parameter: String
     value: String
   }
 
 type TestMetadata
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
     testSource: TestSourceEnum
     testReference: Uriorcurie
     testObjective: TestObjectiveEnum
     testAnnotations: [TestEntityParameter]
   }
 
 type TestOutput
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
     testCaseId: String
     pks: [TestResultPKSet]
   }
 
 type TestResultPKSet
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
     parentPk: String
     mergedPk: String
     aragorn: String
     arax: String
     unsecret: String
     bte: String
     improving: String
   }
 
+type TestRunnerConfiguration
+  {
+    id: Uriorcurie!
+    name: String
+    description: String
+    testRunParameters: [TestEntityParameter]
+    tags: [String]
+  }
+
 type TestRunSession
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
-    components: [ComponentEnum]
-    testEnv: TestEnvEnum
     testRunnerName: String
-    testRunParameters: [TestEntityParameter]
     testEntities: [TestEntity]
     testCaseResults: [TestCaseResult]
     timestamp: Datetime
   }
 
 type TestSuite
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
-    testMetadata: TestMetadata
+    testMetadata: TestMetadata!
     testPersona: TestPersonaEnum
     testCases: [TestCase]
     testSuiteSpecification: TestSuiteSpecification
   }
 
 type TestSuiteSpecification
   {
     id: Uriorcurie!
     name: String
     description: String
     tags: [String]
-    testRunnerSettings: [String]
     testDataFileLocator: Uriorcurie
     testDataFileFormat: FileFormatEnum
   }
```

### Comparing `translator_testing_model-0.3.1/project/jsonld/translator_testing_model.context.jsonld` & `translator_testing_model-2.3.0/project/jsonld/translator_testing_model.context.jsonld`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.816131498470948%*

 * *Differences: {"'@context'": "{'association': {delete: ['@id']}, 'biolink_predicate': {delete: ['@id']}, "*

 * *               "'biolink_qualified_predicate': {delete: ['@id']}, 'components': {delete: ['@id']}, "*

 * *               "'direction': {delete: ['@id']}, 'expected_result': {delete: ['@id']}, 'in_v1': "*

 * *               "{delete: ['@id']}, 'input_category': {delete: ['@id']}, 'input_id': {delete: "*

 * *               "['@id']}, 'must_pass_date': {delete: ['@id']}, 'must_pass_environment': {delete: "*

 * *               "['@id']}, ' […]*

```diff
@@ -1,451 +1,255 @@
 {
     "@context": {
         "@vocab": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/",
-        "AcceptanceTestAsset": {
-            "@id": "AcceptanceTestAsset"
-        },
-        "AcceptanceTestCase": {
-            "@id": "AcceptanceTestCase"
-        },
-        "AcceptanceTestSuite": {
-            "@id": "AcceptanceTestSuite"
-        },
-        "BenchmarkTestSuite": {
-            "@id": "BenchmarkTestSuite"
-        },
-        "OneHopTestSuite": {
-            "@id": "OneHopTestSuite"
-        },
-        "Precondition": {
-            "@id": "Precondition"
-        },
-        "Qualifier": {
-            "@id": "Qualifier"
-        },
-        "QuantitativeTestCase": {
-            "@id": "QuantitativeTestCase"
-        },
-        "StandardsComplianceTestSuite": {
-            "@id": "StandardsComplianceTestSuite"
-        },
-        "TestAsset": {
-            "@id": "TestAsset"
-        },
-        "TestCase": {
-            "@id": "TestCase"
-        },
-        "TestCaseResult": {
-            "@id": "TestCaseResult"
-        },
-        "TestEdgeData": {
-            "@id": "TestEdgeData"
-        },
-        "TestEntity": {
-            "@id": "TestEntity"
-        },
-        "TestEntityParameter": {
-            "@id": "TestEntityParameter"
-        },
-        "TestMetadata": {
-            "@id": "TestMetadata"
-        },
-        "TestOutput": {
-            "@id": "TestOutput"
-        },
-        "TestResultPKSet": {
-            "@id": "TestResultPKSet"
-        },
-        "TestRunSession": {
-            "@id": "TestRunSession"
-        },
-        "TestSuite": {
-            "@id": "TestSuite"
-        },
-        "TestSuiteSpecification": {
-            "@id": "TestSuiteSpecification"
-        },
-        "answer_informal_concept": {
-            "@id": "answer_informal_concept"
-        },
-        "aragorn": {
-            "@id": "aragorn"
-        },
-        "arax": {
-            "@id": "arax"
-        },
         "association": {
-            "@id": "association",
             "@type": "@id"
         },
         "biolink": "https://w3id.org/biolink/",
-        "biolink_object_aspect_qualifier": {
-            "@id": "biolink_object_aspect_qualifier"
-        },
-        "biolink_object_direction_qualifier": {
-            "@id": "biolink_object_direction_qualifier"
-        },
         "biolink_predicate": {
-            "@id": "biolink_predicate",
             "@type": "@id"
         },
         "biolink_qualified_predicate": {
-            "@id": "biolink_qualified_predicate",
             "@type": "@id"
         },
-        "biolink_subject_aspect_qualifier": {
-            "@id": "biolink_subject_aspect_qualifier"
-        },
-        "biolink_subject_direction_qualifier": {
-            "@id": "biolink_subject_direction_qualifier"
-        },
-        "biolink_version": {
-            "@id": "biolink_version"
-        },
-        "bte": {
-            "@id": "bte"
-        },
         "components": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "components"
+            }
         },
         "description": {
             "@id": "schema:description"
         },
         "direction": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "direction"
+            }
         },
         "example": "https://example.org/",
-        "expected_output": {
-            "@id": "expected_output"
-        },
         "expected_result": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "expected_result"
+            }
         },
         "id": "@id",
-        "improving": {
-            "@id": "improving"
-        },
         "in_v1": {
-            "@id": "in_v1",
             "@type": "xsd:boolean"
         },
-        "infores": "https://w3id.org/biolink/vocab/",
         "input_category": {
-            "@id": "input_category",
             "@type": "@id"
         },
         "input_id": {
-            "@id": "input_id",
             "@type": "@id"
         },
-        "input_name": {
-            "@id": "input_name"
-        },
         "linkml": "https://w3id.org/linkml/",
-        "merged_pk": {
-            "@id": "merged_pk"
-        },
         "must_pass_date": {
-            "@id": "must_pass_date",
             "@type": "xsd:date"
         },
         "must_pass_environment": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "must_pass_environment"
+            }
         },
         "name": {
             "@id": "schema:name"
         },
-        "notes": {
-            "@id": "notes"
-        },
         "output_category": {
-            "@id": "output_category",
             "@type": "@id"
         },
         "output_id": {
-            "@id": "output_id",
             "@type": "@id"
         },
-        "output_name": {
-            "@id": "output_name"
-        },
-        "parameter": {
-            "@id": "parameter"
-        },
-        "parent_pk": {
-            "@id": "parent_pk"
-        },
         "pks": {
-            "@id": "pks",
             "@type": "@id"
         },
         "preconditions": {
-            "@id": "preconditions",
             "@type": "@id"
         },
         "predicate_id": {
-            "@id": "predicate_id",
             "@type": "@id"
         },
-        "predicate_name": {
-            "@id": "predicate_name"
-        },
         "qualifiers": {
-            "@id": "qualifiers",
             "@type": "@id"
         },
         "query_node": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "query_node"
+            }
         },
         "query_type": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "query_type"
+            }
         },
         "results": {
-            "@id": "results",
             "@type": "@id"
         },
         "schema": "http://schema.org/",
-        "scientific_question": {
-            "@id": "scientific_question"
-        },
         "semantic_severity": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "semantic_severity"
+            }
         },
         "skos": "http://www.w3.org/2004/02/skos/core#",
-        "string_entry": {
-            "@id": "string_entry"
-        },
         "tags": {
             "@id": "schema:additionalType"
         },
         "test_annotations": {
-            "@id": "test_annotations",
             "@type": "@id"
         },
         "test_assets": {
-            "@id": "test_assets",
             "@type": "@id"
         },
         "test_case": {
-            "@id": "test_case",
             "@type": "@id"
         },
-        "test_case_id": {
-            "@id": "test_case_id"
-        },
         "test_case_input_id": {
-            "@id": "test_case_input_id",
             "@type": "@id"
         },
         "test_case_objective": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_case_objective"
-        },
-        "test_case_predicate_id": {
-            "@id": "test_case_predicate_id"
-        },
-        "test_case_predicate_name": {
-            "@id": "test_case_predicate_name"
+            }
         },
         "test_case_result": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_case_result"
+            }
         },
         "test_case_results": {
-            "@id": "test_case_results",
             "@type": "@id"
         },
         "test_case_source": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_case_source"
+            }
         },
         "test_cases": {
-            "@id": "test_cases",
             "@type": "@id"
         },
         "test_data_file_format": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_data_file_format"
+            }
         },
         "test_data_file_locator": {
-            "@id": "test_data_file_locator",
             "@type": "@id"
         },
         "test_entities": {
-            "@id": "test_entities",
             "@type": "@id"
         },
         "test_entity_parameters": {
-            "@id": "test_entity_parameters",
             "@type": "@id"
         },
         "test_env": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_env"
+            }
         },
         "test_issue": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_issue"
+            }
         },
         "test_metadata": {
-            "@id": "test_metadata",
             "@type": "@id"
         },
         "test_objective": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_objective"
+            }
         },
         "test_persona": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_persona"
+            }
         },
         "test_reference": {
-            "@id": "test_reference",
             "@type": "@id"
         },
         "test_run_parameters": {
-            "@id": "test_run_parameters",
             "@type": "@id"
         },
-        "test_runner_name": {
-            "@id": "test_runner_name"
-        },
-        "test_runner_settings": {
-            "@id": "test_runner_settings"
-        },
         "test_source": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "test_source"
+            }
         },
         "test_suite_id": {
-            "@id": "test_suite_id",
             "@type": "@id"
         },
         "test_suite_specification": {
-            "@id": "test_suite_specification",
             "@type": "@id"
         },
         "timestamp": {
-            "@id": "timestamp",
             "@type": "xsd:dateTime"
         },
         "top_level": {
-            "@id": "top_level",
             "@type": "xsd:integer"
         },
         "trapi_template": {
             "@context": {
                 "@vocab": "@null",
                 "description": "skos:prefLabel",
                 "meaning": "@id",
                 "text": "skos:notation"
-            },
-            "@id": "trapi_template"
-        },
-        "trapi_version": {
-            "@id": "trapi_version"
+            }
         },
         "ttm": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/",
-        "unsecret": {
-            "@id": "unsecret"
-        },
-        "value": {
-            "@id": "value"
-        },
         "well_known": {
-            "@id": "well_known",
             "@type": "xsd:boolean"
         }
     },
     "comments": {
         "description": "Auto generated by LinkML jsonld context generator",
-        "generation_date": "2024-04-25T16:46:29",
+        "generation_date": "2024-03-18T12:26:22",
         "source": "translator_testing_model.yaml"
     }
 }
```

### Comparing `translator_testing_model-0.3.1/project/jsonld/translator_testing_model.jsonld` & `translator_testing_model-2.3.0/project/jsonld/translator_testing_model.jsonld`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9226326234972497%*

 * *Differences: {"'classes'": "{2: {'slots': {delete: [4]}}, 3: {'slots': {delete: [4]}}, 4: {'slots': {insert: "*

 * *              "[(18, 'TestAsset_runner_settings')], delete: [21]}}, 5: {'slots': {insert: [(18, "*

 * *              "'TestAsset_runner_settings')], delete: [21]}}, 6: {'slots': {insert: [(18, "*

 * *              "'TestAsset_runner_settings')], delete: [21]}}, 7: {'slots': {delete: [4]}}, 8: "*

 * *              "{'slots': {insert: [(3, 'test_env'), (8, 'components'), (14, "*

 * *              "'test_case_runner_settings')], dele […]*

```diff
@@ -43,16 +43,15 @@
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "TestEntity",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
-                "tags",
-                "test_runner_settings"
+                "tags"
             ],
             "tree_root": true
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestMetadata",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestMetadata",
@@ -62,15 +61,14 @@
             "name": "TestMetadata",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_source",
                 "test_reference",
                 "test_objective",
                 "test_annotations"
             ]
         },
         {
@@ -97,18 +95,18 @@
                 "qualifiers",
                 "expected_output",
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
+                "TestAsset_runner_settings",
                 "test_metadata",
                 "TestAsset_id",
-                "TestAsset_tags",
-                "TestAsset_test_runner_settings"
+                "TestAsset_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/AcceptanceTestAsset",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/AcceptanceTestAsset",
             "description": "Model derived from Jenn's test asset design and Shervin's runner JSON here as an example.",
@@ -131,18 +129,18 @@
                 "qualifiers",
                 "expected_output",
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
+                "TestAsset_runner_settings",
                 "test_metadata",
                 "TestAsset_id",
                 "TestAsset_tags",
-                "TestAsset_test_runner_settings",
                 "must_pass_date",
                 "must_pass_environment",
                 "scientific_question",
                 "string_entry",
                 "direction",
                 "answer_informal_concept",
                 "expected_result",
@@ -175,18 +173,18 @@
                 "qualifiers",
                 "expected_output",
                 "test_issue",
                 "semantic_severity",
                 "in_v1",
                 "well_known",
                 "test_reference",
+                "TestAsset_runner_settings",
                 "test_metadata",
                 "TestAsset_id",
-                "TestAsset_tags",
-                "TestAsset_test_runner_settings"
+                "TestAsset_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/Precondition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/Precondition",
             "description": "Represents a precondition for a TestCase",
@@ -194,16 +192,15 @@
             "is_a": "TestEntity",
             "name": "Precondition",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
-                "tags",
-                "test_runner_settings"
+                "tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCase",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCase",
             "description": "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition.",
@@ -211,29 +208,26 @@
             "is_a": "TestEntity",
             "name": "TestCase",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
-                "test_runner_settings",
+                "test_env",
                 "query_type",
                 "TestCase_test_assets",
                 "preconditions",
                 "trapi_template",
+                "components",
                 "test_case_objective",
                 "test_case_source",
                 "test_case_predicate_name",
                 "test_case_predicate_id",
                 "test_case_input_id",
-                "qualifiers",
-                "input_category",
-                "output_category",
-                "components",
-                "test_env",
+                "test_case_runner_settings",
                 "TestCase_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/AcceptanceTestCase",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/AcceptanceTestCase",
@@ -242,28 +236,25 @@
             "is_a": "TestCase",
             "name": "AcceptanceTestCase",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
-                "test_runner_settings",
+                "test_env",
                 "query_type",
                 "preconditions",
                 "trapi_template",
+                "components",
                 "test_case_objective",
                 "test_case_source",
                 "test_case_predicate_name",
                 "test_case_predicate_id",
                 "test_case_input_id",
-                "qualifiers",
-                "input_category",
-                "output_category",
-                "components",
-                "test_env",
+                "test_case_runner_settings",
                 "TestCase_tags",
                 "AcceptanceTestCase_test_assets"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/QuantitativeTestCase",
@@ -273,29 +264,112 @@
             "is_a": "TestCase",
             "name": "QuantitativeTestCase",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
-                "test_runner_settings",
+                "test_env",
                 "query_type",
                 "TestCase_test_assets",
                 "preconditions",
                 "trapi_template",
+                "components",
                 "test_case_objective",
                 "test_case_source",
                 "test_case_predicate_name",
                 "test_case_predicate_id",
                 "test_case_input_id",
-                "qualifiers",
-                "input_category",
-                "output_category",
+                "test_case_runner_settings",
+                "TestCase_tags"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/ComplianceTestCase",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/ComplianceTestCase",
+            "description": "TRAPI and Biolink Model standards compliance test",
+            "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
+            "is_a": "TestCase",
+            "name": "ComplianceTestCase",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "name",
+                "description",
+                "test_env",
+                "query_type",
+                "TestCase_test_assets",
+                "preconditions",
+                "trapi_template",
                 "components",
+                "test_case_objective",
+                "test_case_source",
+                "test_case_predicate_name",
+                "test_case_predicate_id",
+                "test_case_input_id",
+                "test_case_runner_settings",
+                "TestCase_tags",
+                "trapi_version",
+                "biolink_version"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/KnowledgeGraphNavigationTestCase",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/KnowledgeGraphNavigationTestCase",
+            "description": "Knowledge Graph navigation integration test",
+            "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
+            "is_a": "TestCase",
+            "name": "KnowledgeGraphNavigationTestCase",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "name",
+                "description",
+                "test_env",
+                "query_type",
+                "TestCase_test_assets",
+                "preconditions",
+                "trapi_template",
+                "components",
+                "test_case_objective",
+                "test_case_source",
+                "test_case_predicate_name",
+                "test_case_predicate_id",
+                "test_case_input_id",
+                "test_case_runner_settings",
+                "TestCase_tags"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
+            "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/OneHopTestCase",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/OneHopTestCase",
+            "description": "'One Hop' Knowledge Graph navigation integration test",
+            "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
+            "is_a": "KnowledgeGraphNavigationTestCase",
+            "name": "OneHopTestCase",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "name",
+                "description",
                 "test_env",
+                "query_type",
+                "TestCase_test_assets",
+                "preconditions",
+                "trapi_template",
+                "components",
+                "test_case_objective",
+                "test_case_source",
+                "test_case_predicate_name",
+                "test_case_predicate_id",
+                "test_case_input_id",
+                "test_case_runner_settings",
                 "TestCase_tags"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSuiteSpecification",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSuiteSpecification",
@@ -305,15 +379,14 @@
             "name": "TestSuiteSpecification",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_data_file_locator",
                 "test_data_file_format"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSuite",
@@ -324,15 +397,14 @@
             "name": "TestSuite",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_metadata",
                 "test_persona",
                 "test_cases",
                 "test_suite_specification"
             ]
         },
         {
@@ -344,15 +416,14 @@
             "name": "AcceptanceTestSuite",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_metadata",
                 "test_persona",
                 "test_cases",
                 "test_suite_specification"
             ]
         },
         {
@@ -374,15 +445,14 @@
             "name": "StandardsComplianceTestSuite",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_metadata",
                 "test_persona",
                 "test_cases",
                 "test_suite_specification"
             ]
         },
         {
@@ -395,60 +465,71 @@
             "name": "OneHopTestSuite",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_metadata",
                 "test_persona",
                 "test_cases",
                 "test_suite_specification"
             ]
         },
         {
             "@type": "ClassDefinition",
+            "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestRunnerConfiguration",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestRunnerConfiguration",
+            "description": "General configuration parameters and test data input  for a single invocation of a TestRunner.",
+            "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
+            "is_a": "TestEntity",
+            "name": "TestRunnerConfiguration",
+            "slot_usage": {},
+            "slots": [
+                "id",
+                "name",
+                "description",
+                "test_run_parameters",
+                "TestRunnerConfiguration_tags"
+            ]
+        },
+        {
+            "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResult",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResult",
             "description": "The outcome of a TestRunner run of one specific TestCase.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "is_a": "TestEntity",
             "name": "TestCaseResult",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_suite_id",
                 "test_case",
                 "test_case_result"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestRunSession",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestRunSession",
-            "description": "Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite).",
+            "description": "A single invocation of a TestRunner.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "is_a": "TestEntity",
             "name": "TestRunSession",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
-                "components",
-                "test_env",
                 "test_runner_name",
-                "TestRunSession_test_run_parameters",
                 "TestRunSession_test_entities",
                 "test_case_results",
                 "timestamp"
             ]
         },
         {
             "@type": "ClassDefinition",
@@ -460,15 +541,14 @@
             "name": "TestOutput",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "test_case_id",
                 "pks"
             ]
         },
         {
             "@type": "ClassDefinition",
             "class_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestResultPKSet",
@@ -479,15 +559,14 @@
             "name": "TestResultPKSet",
             "slot_usage": {},
             "slots": [
                 "id",
                 "name",
                 "description",
                 "tags",
-                "test_runner_settings",
                 "parent_pk",
                 "merged_pk",
                 "aragorn",
                 "arax",
                 "unsecret",
                 "bte",
                 "improving"
@@ -546,22 +625,14 @@
                 {
                     "description": "Semantic benchmarking",
                     "text": "BenchmarkTest"
                 },
                 {
                     "description": "Quantitative test",
                     "text": "QuantitativeTest"
-                },
-                {
-                    "description": "Release-specific TRAPI and Biolink Model (\"reasoner-validator\") compliance validation",
-                    "text": "StandardsValidationTest"
-                },
-                {
-                    "description": "Knowledge graph \"One Hop\" query navigation integrity",
-                    "text": "OneHopTest"
                 }
             ]
         },
         {
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum",
             "description": "Testing environments within which a TestSuite is run by a TestRunner scheduled by the TestHarness.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
@@ -748,101 +819,20 @@
             ]
         },
         {
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/ComponentEnum",
             "description": "Translator components are identified by their InfoRes identifiers.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "ComponentEnum",
-            "permissible_values": [
-                {
-                    "description": "Automatic Relay Service component of Translator",
-                    "meaning": "infores:ncats-ars",
-                    "text": "ars"
-                },
-                {
-                    "description": "ARAX Translator Reasoner",
-                    "meaning": "infores:arax",
-                    "text": "arax"
-                },
-                {
-                    "description": "A Translator Reasoner API for the Explanatory Agent",
-                    "meaning": "infores:explanatory-agent",
-                    "text": "explanatory"
-                },
-                {
-                    "description": "imProving Agent OpenAPI TRAPI Specification",
-                    "meaning": "infores:improving-agent",
-                    "text": "improving"
-                },
-                {
-                    "description": "Performs a query operation which compiles data from numerous ranking agent services.",
-                    "meaning": "infores:aragorn",
-                    "text": "aragorn"
-                },
-                {
-                    "description": "BioThings Explorer",
-                    "meaning": "infores:biothings-explorer",
-                    "text": "bte"
-                },
-                {
-                    "description": "Unsecret Agent OpenAPI for NCATS Biomedical Translator Reasoners",
-                    "meaning": "infores:unsecret-agent",
-                    "text": "unsecret"
-                },
-                {
-                    "description": "TRAPI endpoint for the NCATS Biomedical Translator KP called RTX KG2",
-                    "meaning": "infores:rtx-kg2",
-                    "text": "rtxkg2"
-                },
-                {
-                    "description": "ICEES (Integrated Clinical and Environmental Exposures Service)",
-                    "meaning": "infores:icees-kg",
-                    "text": "icees"
-                },
-                {
-                    "description": "Causal Activity Model KP",
-                    "meaning": "infores:cam-kp",
-                    "text": "cam"
-                },
-                {
-                    "description": "SPOKE KP - an NIH NCATS Knowledge Provider to expose UCSFs SPOKE",
-                    "meaning": "infores:spoke",
-                    "text": "spoke"
-                },
-                {
-                    "description": "Molecular Data Provider for NCATS Biomedical Translator Reasoners",
-                    "meaning": "infores:molepro",
-                    "text": "molepro"
-                },
-                {
-                    "description": "Text Mining KP",
-                    "meaning": "infores:textmining-kp",
-                    "text": "textmining"
-                },
-                {
-                    "description": "Columbia Open Health Data (COHD)",
-                    "meaning": "infores:cohd",
-                    "text": "cohd"
-                },
-                {
-                    "description": "OpenPredict API",
-                    "meaning": "infores:openpredict",
-                    "text": "openpredict"
-                },
-                {
-                    "description": "Translator Knowledge Collaboratory API",
-                    "meaning": "infores:knowledge-collaboratory",
-                    "text": "collaboratory"
-                },
-                {
-                    "description": "Connections Hypothesis Provider API",
-                    "meaning": "infores:connections-hypothesis",
-                    "text": "connections"
-                }
-            ]
+            "reachable_from": {
+                "source_nodes": [
+                    "biolink:infores"
+                ],
+                "source_ontology": "biolink"
+            }
         },
         {
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum",
             "description": "User persona context of a given test.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "TestPersonaEnum",
             "permissible_values": [
@@ -865,29 +855,26 @@
         },
         {
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "TestCaseResultEnum",
             "permissible_values": [
                 {
-                    "description": "test case result indicating success.",
-                    "text": "PASSED"
+                    "text": "test_passed"
                 },
                 {
-                    "description": "test case result indicating failure.",
-                    "text": "FAILED"
+                    "text": "test_failed"
                 },
                 {
-                    "description": "test case result indicating that the specified test was not run.",
-                    "text": "SKIPPED"
+                    "text": "test_skipped"
                 }
             ]
         }
     ],
-    "generation_date": "2024-04-25T16:46:29",
+    "generation_date": "2024-03-18T12:26:22",
     "id": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
     "imports": [
         "linkml:types"
     ],
     "license": "MIT",
     "metamodel_version": "1.7.0",
     "name": "Translator-Testing-Model",
@@ -901,18 +888,14 @@
             "prefix_reference": "https://w3id.org/linkml/"
         },
         {
             "prefix_prefix": "biolink",
             "prefix_reference": "https://w3id.org/biolink/"
         },
         {
-            "prefix_prefix": "infores",
-            "prefix_reference": "https://w3id.org/biolink/vocab/"
-        },
-        {
             "prefix_prefix": "schema",
             "prefix_reference": "http://schema.org/"
         },
         {
             "prefix_prefix": "example",
             "prefix_reference": "https://example.org/"
         }
@@ -1067,15 +1050,15 @@
             "owner": "TestEntityParameter",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/value"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_entity_parameters",
-            "description": "One or more 'tag = value' parameters documenting target characteristics of a TestEntity.",
+            "description": "One or more parameters documenting target characteristics of a TestEntity.",
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "inlined": true,
             "inlined_as_list": true,
             "multivalued": true,
             "name": "test_entity_parameters",
             "range": "TestEntityParameter",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_entity_parameters"
@@ -1189,28 +1172,28 @@
             "owner": "TestAsset",
             "range": "uriorcurie",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_reference"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_objective",
-            "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)",
+            "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)",
             "domain_of": [
                 "TestMetadata"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "test_objective",
             "owner": "TestMetadata",
             "range": "TestObjectiveEnum",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_objective"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_case_objective",
-            "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)",
+            "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)",
             "domain_of": [
                 "TestCase"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "test_case_objective",
             "owner": "TestCase",
             "range": "TestObjectiveEnum",
@@ -1327,20 +1310,19 @@
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "SubjectCategory"
             ],
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/input_category",
             "domain_of": [
-                "TestAsset",
-                "TestCase"
+                "TestAsset"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "input_category",
-            "owner": "TestCase",
+            "owner": "TestAsset",
             "range": "concept_category",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/input_category"
         },
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "Predicate"
@@ -1460,20 +1442,19 @@
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "ObjectCategory"
             ],
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/output_category",
             "domain_of": [
-                "TestAsset",
-                "TestCase"
+                "TestAsset"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "output_category",
-            "owner": "TestCase",
+            "owner": "TestAsset",
             "range": "concept_category",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/output_category"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/association",
             "description": "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement",
@@ -1487,23 +1468,22 @@
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/association"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/qualifiers",
             "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
             "domain_of": [
-                "TestAsset",
-                "TestCase"
+                "TestAsset"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "inlined": true,
             "inlined_as_list": true,
             "multivalued": true,
             "name": "qualifiers",
-            "owner": "TestCase",
+            "owner": "TestAsset",
             "range": "Qualifier",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/qualifiers"
         },
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "Expected Output"
@@ -1579,25 +1559,44 @@
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/well_known"
         },
         {
             "@type": "SlotDefinition",
             "aliases": [
                 "Settings"
             ],
-            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_runner_settings",
-            "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/runner_settings",
+            "description": "Settings for the test harness for TestAsset",
             "domain_of": [
-                "TestEntity"
+                "TestAsset"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "multivalued": true,
-            "name": "test_runner_settings",
-            "owner": "TestEntity",
+            "name": "runner_settings",
+            "owner": "TestAsset",
+            "range": "string",
+            "required": true,
+            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/runner_settings"
+        },
+        {
+            "@type": "SlotDefinition",
+            "aliases": [
+                "Settings"
+            ],
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_case_runner_settings",
+            "description": "Settings for the test harness for TestCase",
+            "domain_of": [
+                "TestCase"
+            ],
+            "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
+            "multivalued": true,
+            "name": "test_case_runner_settings",
+            "owner": "TestCase",
             "range": "string",
-            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_runner_settings"
+            "required": true,
+            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_case_runner_settings"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/must_pass_date",
             "description": "The date by which this test must pass",
             "domain_of": [
                 "AcceptanceTestAsset"
@@ -1788,20 +1787,19 @@
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/notes"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_env",
             "description": "Deployment environment within which the associated TestSuite is run.",
             "domain_of": [
-                "TestCase",
-                "TestRunSession"
+                "TestCase"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "test_env",
-            "owner": "TestRunSession",
+            "owner": "TestCase",
             "range": "TestEnvEnum",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_env"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/query_type",
             "description": "Type of TestCase query.",
@@ -1858,39 +1856,46 @@
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/trapi_template"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/components",
             "description": "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.",
             "domain_of": [
-                "TestCase",
-                "TestRunSession"
+                "TestCase"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "multivalued": true,
             "name": "components",
-            "owner": "TestRunSession",
+            "owner": "TestCase",
             "range": "ComponentEnum",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/components"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/trapi_version",
             "description": "TRAPI version (SemVer string)",
+            "domain_of": [
+                "ComplianceTestCase"
+            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "trapi_version",
+            "owner": "ComplianceTestCase",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/trapi_version"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_version",
             "description": "Biolink Model release (SemVer string)",
+            "domain_of": [
+                "ComplianceTestCase"
+            ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "name": "biolink_version",
+            "owner": "ComplianceTestCase",
             "range": "string",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/biolink_version"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_data_file_locator",
             "description": "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)",
@@ -1925,14 +1930,15 @@
                 "TestSuite"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "inlined": true,
             "name": "test_metadata",
             "owner": "TestSuite",
             "range": "TestMetadata",
+            "required": true,
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_metadata"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_persona",
             "description": "A Test persona describes the user or operational context of a given test.",
             "domain_of": [
@@ -1972,25 +1978,25 @@
             "owner": "TestSuite",
             "range": "TestSuiteSpecification",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_suite_specification"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_run_parameters",
-            "description": "TestRunSession parameters informing a TestHarness about the global characteristics of TestRunner processing tests.",
+            "description": "Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run.",
             "domain_of": [
-                "TestRunSession"
+                "TestRunnerConfiguration"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "inlined": true,
             "inlined_as_list": true,
             "is_a": "test_entity_parameters",
             "multivalued": true,
             "name": "test_run_parameters",
-            "owner": "TestRunSession",
+            "owner": "TestRunnerConfiguration",
             "range": "TestEntityParameter",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_run_parameters"
         },
         {
             "@type": "SlotDefinition",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_suite_id",
             "description": "CURIE id of a TestSuite registered in the system.",
@@ -2155,33 +2161,34 @@
             "owner": "TestAsset",
             "range": "string",
             "slot_uri": "http://schema.org/additionalType",
             "usage_slot_name": "tags"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "test_runner_settings",
+            "alias": "runner_settings",
             "aliases": [
                 "Settings"
             ],
-            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_runner_settings",
-            "description": "Scalar settings for the TestRunner, e.g. \"inferred\"",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/runner_settings",
+            "description": "Settings for the test harness, e.g. \"inferred\"",
             "domain": "TestAsset",
             "domain_of": [
                 "TestAsset"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
-            "is_a": "test_runner_settings",
+            "is_a": "runner_settings",
             "is_usage_slot": true,
             "multivalued": true,
-            "name": "TestAsset_test_runner_settings",
+            "name": "TestAsset_runner_settings",
             "owner": "TestAsset",
             "range": "string",
-            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_runner_settings",
-            "usage_slot_name": "test_runner_settings"
+            "required": true,
+            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/runner_settings",
+            "usage_slot_name": "runner_settings"
         },
         {
             "@type": "SlotDefinition",
             "alias": "test_assets",
             "aliases": [
                 "Block List"
             ],
@@ -2246,38 +2253,39 @@
             "range": "AcceptanceTestAsset",
             "required": true,
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_assets",
             "usage_slot_name": "test_assets"
         },
         {
             "@type": "SlotDefinition",
-            "alias": "test_run_parameters",
-            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_run_parameters",
-            "description": "Different TestRunners could expect additional global test configuration parameters, like the applicable TRAPI version (\"trapi_version\") or Biolink Model versions (\"biolink_version\").",
-            "domain": "TestRunSession",
+            "alias": "tags",
+            "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/tags",
+            "description": "One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration.",
+            "domain": "TestRunnerConfiguration",
             "domain_of": [
-                "TestRunSession"
+                "TestRunnerConfiguration"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
-            "inlined": true,
-            "inlined_as_list": true,
-            "is_a": "test_run_parameters",
+            "is_a": "tags",
             "is_usage_slot": true,
+            "mappings": [
+                "http://schema.org/additionalType"
+            ],
             "multivalued": true,
-            "name": "TestRunSession_test_run_parameters",
-            "owner": "TestRunSession",
-            "range": "TestEntityParameter",
-            "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_run_parameters",
-            "usage_slot_name": "test_run_parameters"
+            "name": "TestRunnerConfiguration_tags",
+            "owner": "TestRunnerConfiguration",
+            "range": "string",
+            "slot_uri": "http://schema.org/additionalType",
+            "usage_slot_name": "tags"
         },
         {
             "@type": "SlotDefinition",
             "alias": "test_entities",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_entities",
-            "description": "Different TestRunners could expect specific kinds of TestEntity as an input.  These 'test_entities' are one or more instances of TestAsset, TestCase or (preferably?) TestSuite.",
+            "description": "Different TestRunners may expect specific kinds of TestEntity as input. These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite.",
             "domain": "TestRunSession",
             "domain_of": [
                 "TestRunSession"
             ],
             "from_schema": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
             "inlined": true,
             "is_a": "test_entities",
@@ -2287,16 +2295,16 @@
             "owner": "TestRunSession",
             "range": "TestEntity",
             "slot_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/test_entities",
             "usage_slot_name": "test_entities"
         }
     ],
     "source_file": "translator_testing_model.yaml",
-    "source_file_date": "2024-04-25T16:35:26",
-    "source_file_size": 29634,
+    "source_file_date": "2024-03-18T12:26:09",
+    "source_file_size": 27461,
     "title": "Translator Testing Data Model",
     "types": [
         {
             "@type": "TypeDefinition",
             "base": "URIorCURIE",
             "definition_uri": "https://w3id.org/TranslatorSRI/TranslatorTestingModel/CategoryType",
             "description": "A primitive type in which the value denotes a class within the biolink model. The value must be a URI or a CURIE within the 'biolink' namespace.",
```

### Comparing `translator_testing_model-0.3.1/project/jsonschema/translator_testing_model.schema.json` & `translator_testing_model-2.3.0/project/jsonschema/translator_testing_model.schema.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9304734930143298%*

 * *Differences: {"'$defs'": "{'AcceptanceTestAsset': {'properties': {'runner_settings': "*

 * *            'OrderedDict([(\'description\', \'Settings for the test harness, e.g. "inferred"\'), '*

 * *            "('items', OrderedDict([('type', 'string')])), ('type', 'array')]), delete: "*

 * *            "['test_runner_settings']}, 'required': {insert: [(0, 'runner_settings'), (1, "*

 * *            "'test_metadata')]}}, 'AcceptanceTestCase': {'properties': {'test_case_objective': "*

 * *            "{'description': 'Testing objective behind speci […]*

```diff
@@ -82,14 +82,21 @@
                     },
                     "type": "array"
                 },
                 "query_node": {
                     "$ref": "#/$defs/NodeEnum",
                     "description": "The node of the (templated) TRAPI query to replace"
                 },
+                "runner_settings": {
+                    "description": "Settings for the test harness, e.g. \"inferred\"",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "scientific_question": {
                     "description": "The full human-readable scientific question a SME would ask, which is encoded into the test asset.",
                     "type": "string"
                 },
                 "semantic_severity": {
                     "$ref": "#/$defs/SemanticSeverityEnum"
                 },
@@ -111,30 +118,25 @@
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_reference": {
                     "description": "Document URL where original test source particulars are registered (e.g. Github repo)",
                     "type": "string"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar settings for the TestRunner, e.g. \"inferred\"",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "top_level": {
                     "description": "The answer must return in these many results",
                     "type": "integer"
                 },
                 "well_known": {
                     "type": "boolean"
                 }
             },
             "required": [
+                "runner_settings",
+                "test_metadata",
                 "id"
             ],
             "title": "AcceptanceTestAsset",
             "type": "object"
         },
         "AcceptanceTestCase": {
             "additionalProperties": false,
@@ -151,37 +153,24 @@
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "id": {
                     "description": "A unique identifier for a Test Entity",
                     "type": "string"
                 },
-                "input_category": {
-                    "type": "string"
-                },
                 "name": {
                     "description": "A human-readable name for a Test Entity",
                     "type": "string"
                 },
-                "output_category": {
-                    "type": "string"
-                },
                 "preconditions": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "qualifiers": {
-                    "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
-                    "items": {
-                        "$ref": "#/$defs/Qualifier"
-                    },
-                    "type": "array"
-                },
                 "query_type": {
                     "$ref": "#/$defs/QueryTypeEnum",
                     "description": "Type of TestCase query."
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
                     "items": {
@@ -197,44 +186,45 @@
                     "type": "array"
                 },
                 "test_case_input_id": {
                     "type": "string"
                 },
                 "test_case_objective": {
                     "$ref": "#/$defs/TestObjectiveEnum",
-                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)"
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
                 },
                 "test_case_predicate_id": {
                     "type": "string"
                 },
                 "test_case_predicate_name": {
                     "type": "string"
                 },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "test_case_source": {
                     "$ref": "#/$defs/TestSourceEnum",
                     "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
                 },
                 "test_env": {
                     "$ref": "#/$defs/TestEnvEnum",
                     "description": "Deployment environment within which the associated TestSuite is run."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "trapi_template": {
                     "$ref": "#/$defs/TrapiTemplateEnum",
                     "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
                 }
             },
             "required": [
                 "test_assets",
+                "test_case_runner_settings",
                 "id"
             ],
             "title": "AcceptanceTestCase",
             "type": "object"
         },
         "AcceptanceTestSuite": {
             "additionalProperties": false,
@@ -257,83 +247,143 @@
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "test_cases": {
                     "additionalProperties": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/$defs/TestCase__identifier_optional"
-                            },
-                            {
-                                "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
-                                "items": {
-                                    "$ref": "#/$defs/TestAsset"
-                                },
-                                "type": "array"
-                            }
-                        ]
+                        "$ref": "#/$defs/TestCase__identifier_optional"
                     },
                     "description": "List of explicitly enumerated Test Cases.",
                     "type": "object"
                 },
                 "test_metadata": {
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_persona": {
                     "$ref": "#/$defs/TestPersonaEnum",
                     "description": "A Test persona describes the user or operational context of a given test."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_specification": {
                     "$ref": "#/$defs/TestSuiteSpecification",
                     "description": "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source."
                 }
             },
             "required": [
+                "test_metadata",
                 "id"
             ],
             "title": "AcceptanceTestSuite",
             "type": "object"
         },
         "BenchmarkTestSuite": {
             "additionalProperties": false,
             "description": "JsonObj(is_a='TestSuite')",
             "title": "BenchmarkTestSuite",
             "type": "object"
         },
+        "ComplianceTestCase": {
+            "additionalProperties": false,
+            "description": "TRAPI and Biolink Model standards compliance test",
+            "properties": {
+                "biolink_version": {
+                    "description": "Biolink Model release (SemVer string)",
+                    "type": "string"
+                },
+                "components": {
+                    "description": "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.",
+                    "items": {
+                        "$ref": "#/$defs/ComponentEnum"
+                    },
+                    "type": "array"
+                },
+                "description": {
+                    "description": "A human-readable description for a Test Entity",
+                    "type": "string"
+                },
+                "id": {
+                    "description": "A unique identifier for a Test Entity",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "A human-readable name for a Test Entity",
+                    "type": "string"
+                },
+                "preconditions": {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "query_type": {
+                    "$ref": "#/$defs/QueryTypeEnum",
+                    "description": "Type of TestCase query."
+                },
+                "tags": {
+                    "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_assets": {
+                    "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
+                    "items": {
+                        "$ref": "#/$defs/TestAsset"
+                    },
+                    "type": "array"
+                },
+                "test_case_input_id": {
+                    "type": "string"
+                },
+                "test_case_objective": {
+                    "$ref": "#/$defs/TestObjectiveEnum",
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
+                },
+                "test_case_predicate_id": {
+                    "type": "string"
+                },
+                "test_case_predicate_name": {
+                    "type": "string"
+                },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_case_source": {
+                    "$ref": "#/$defs/TestSourceEnum",
+                    "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
+                },
+                "test_env": {
+                    "$ref": "#/$defs/TestEnvEnum",
+                    "description": "Deployment environment within which the associated TestSuite is run."
+                },
+                "trapi_template": {
+                    "$ref": "#/$defs/TrapiTemplateEnum",
+                    "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
+                },
+                "trapi_version": {
+                    "description": "TRAPI version (SemVer string)",
+                    "type": "string"
+                }
+            },
+            "required": [
+                "test_assets",
+                "test_case_runner_settings",
+                "id"
+            ],
+            "title": "ComplianceTestCase",
+            "type": "object"
+        },
         "ComponentEnum": {
             "description": "Translator components are identified by their InfoRes identifiers.",
-            "enum": [
-                "ars",
-                "arax",
-                "explanatory",
-                "improving",
-                "aragorn",
-                "bte",
-                "unsecret",
-                "rtxkg2",
-                "icees",
-                "cam",
-                "spoke",
-                "molepro",
-                "textmining",
-                "cohd",
-                "openpredict",
-                "collaboratory",
-                "connections"
-            ],
             "title": "ComponentEnum",
             "type": "string"
         },
         "DirectionEnum": {
             "description": "",
             "enum": [
                 "increased",
@@ -369,23 +419,199 @@
                 "TSV",
                 "YAML",
                 "JSON"
             ],
             "title": "FileFormatEnum",
             "type": "string"
         },
+        "KnowledgeGraphNavigationTestCase": {
+            "additionalProperties": false,
+            "description": "Knowledge Graph navigation integration test",
+            "properties": {
+                "components": {
+                    "description": "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.",
+                    "items": {
+                        "$ref": "#/$defs/ComponentEnum"
+                    },
+                    "type": "array"
+                },
+                "description": {
+                    "description": "A human-readable description for a Test Entity",
+                    "type": "string"
+                },
+                "id": {
+                    "description": "A unique identifier for a Test Entity",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "A human-readable name for a Test Entity",
+                    "type": "string"
+                },
+                "preconditions": {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "query_type": {
+                    "$ref": "#/$defs/QueryTypeEnum",
+                    "description": "Type of TestCase query."
+                },
+                "tags": {
+                    "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_assets": {
+                    "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
+                    "items": {
+                        "$ref": "#/$defs/TestAsset"
+                    },
+                    "type": "array"
+                },
+                "test_case_input_id": {
+                    "type": "string"
+                },
+                "test_case_objective": {
+                    "$ref": "#/$defs/TestObjectiveEnum",
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
+                },
+                "test_case_predicate_id": {
+                    "type": "string"
+                },
+                "test_case_predicate_name": {
+                    "type": "string"
+                },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_case_source": {
+                    "$ref": "#/$defs/TestSourceEnum",
+                    "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
+                },
+                "test_env": {
+                    "$ref": "#/$defs/TestEnvEnum",
+                    "description": "Deployment environment within which the associated TestSuite is run."
+                },
+                "trapi_template": {
+                    "$ref": "#/$defs/TrapiTemplateEnum",
+                    "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
+                }
+            },
+            "required": [
+                "test_assets",
+                "test_case_runner_settings",
+                "id"
+            ],
+            "title": "KnowledgeGraphNavigationTestCase",
+            "type": "object"
+        },
         "NodeEnum": {
             "description": "Target node of a Subject-Predicate-Object driven query",
             "enum": [
                 "subject",
                 "object"
             ],
             "title": "NodeEnum",
             "type": "string"
         },
+        "OneHopTestCase": {
+            "additionalProperties": false,
+            "description": "'One Hop' Knowledge Graph navigation integration test",
+            "properties": {
+                "components": {
+                    "description": "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.",
+                    "items": {
+                        "$ref": "#/$defs/ComponentEnum"
+                    },
+                    "type": "array"
+                },
+                "description": {
+                    "description": "A human-readable description for a Test Entity",
+                    "type": "string"
+                },
+                "id": {
+                    "description": "A unique identifier for a Test Entity",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "A human-readable name for a Test Entity",
+                    "type": "string"
+                },
+                "preconditions": {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "query_type": {
+                    "$ref": "#/$defs/QueryTypeEnum",
+                    "description": "Type of TestCase query."
+                },
+                "tags": {
+                    "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_assets": {
+                    "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
+                    "items": {
+                        "$ref": "#/$defs/TestAsset"
+                    },
+                    "type": "array"
+                },
+                "test_case_input_id": {
+                    "type": "string"
+                },
+                "test_case_objective": {
+                    "$ref": "#/$defs/TestObjectiveEnum",
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
+                },
+                "test_case_predicate_id": {
+                    "type": "string"
+                },
+                "test_case_predicate_name": {
+                    "type": "string"
+                },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_case_source": {
+                    "$ref": "#/$defs/TestSourceEnum",
+                    "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
+                },
+                "test_env": {
+                    "$ref": "#/$defs/TestEnvEnum",
+                    "description": "Deployment environment within which the associated TestSuite is run."
+                },
+                "trapi_template": {
+                    "$ref": "#/$defs/TrapiTemplateEnum",
+                    "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
+                }
+            },
+            "required": [
+                "test_assets",
+                "test_case_runner_settings",
+                "id"
+            ],
+            "title": "OneHopTestCase",
+            "type": "object"
+        },
         "OneHopTestSuite": {
             "additionalProperties": false,
             "description": "Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness.",
             "properties": {
                 "description": {
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
@@ -403,51 +629,34 @@
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "test_cases": {
                     "additionalProperties": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/$defs/TestCase__identifier_optional"
-                            },
-                            {
-                                "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
-                                "items": {
-                                    "$ref": "#/$defs/TestAsset"
-                                },
-                                "type": "array"
-                            }
-                        ]
+                        "$ref": "#/$defs/TestCase__identifier_optional"
                     },
                     "description": "List of explicitly enumerated Test Cases.",
                     "type": "object"
                 },
                 "test_metadata": {
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_persona": {
                     "$ref": "#/$defs/TestPersonaEnum",
                     "description": "A Test persona describes the user or operational context of a given test."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_specification": {
                     "$ref": "#/$defs/TestSuiteSpecification",
                     "description": "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source."
                 }
             },
             "required": [
+                "test_metadata",
                 "id"
             ],
             "title": "OneHopTestSuite",
             "type": "object"
         },
         "Precondition": {
             "additionalProperties": false,
@@ -467,21 +676,14 @@
                 },
                 "tags": {
                     "description": "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
-                },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "Precondition",
             "type": "object"
@@ -517,37 +719,24 @@
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "id": {
                     "description": "A unique identifier for a Test Entity",
                     "type": "string"
                 },
-                "input_category": {
-                    "type": "string"
-                },
                 "name": {
                     "description": "A human-readable name for a Test Entity",
                     "type": "string"
                 },
-                "output_category": {
-                    "type": "string"
-                },
                 "preconditions": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "qualifiers": {
-                    "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
-                    "items": {
-                        "$ref": "#/$defs/Qualifier"
-                    },
-                    "type": "array"
-                },
                 "query_type": {
                     "$ref": "#/$defs/QueryTypeEnum",
                     "description": "Type of TestCase query."
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
                     "items": {
@@ -563,44 +752,45 @@
                     "type": "array"
                 },
                 "test_case_input_id": {
                     "type": "string"
                 },
                 "test_case_objective": {
                     "$ref": "#/$defs/TestObjectiveEnum",
-                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)"
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
                 },
                 "test_case_predicate_id": {
                     "type": "string"
                 },
                 "test_case_predicate_name": {
                     "type": "string"
                 },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "test_case_source": {
                     "$ref": "#/$defs/TestSourceEnum",
                     "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
                 },
                 "test_env": {
                     "$ref": "#/$defs/TestEnvEnum",
                     "description": "Deployment environment within which the associated TestSuite is run."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "trapi_template": {
                     "$ref": "#/$defs/TrapiTemplateEnum",
                     "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
                 }
             },
             "required": [
                 "test_assets",
+                "test_case_runner_settings",
                 "id"
             ],
             "title": "QuantitativeTestCase",
             "type": "object"
         },
         "QueryTypeEnum": {
             "description": "Query",
@@ -641,51 +831,34 @@
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "test_cases": {
                     "additionalProperties": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/$defs/TestCase__identifier_optional"
-                            },
-                            {
-                                "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
-                                "items": {
-                                    "$ref": "#/$defs/TestAsset"
-                                },
-                                "type": "array"
-                            }
-                        ]
+                        "$ref": "#/$defs/TestCase__identifier_optional"
                     },
                     "description": "List of explicitly enumerated Test Cases.",
                     "type": "object"
                 },
                 "test_metadata": {
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_persona": {
                     "$ref": "#/$defs/TestPersonaEnum",
                     "description": "A Test persona describes the user or operational context of a given test."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_specification": {
                     "$ref": "#/$defs/TestSuiteSpecification",
                     "description": "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source."
                 }
             },
             "required": [
+                "test_metadata",
                 "id"
             ],
             "title": "StandardsComplianceTestSuite",
             "type": "object"
         },
         "TestAsset": {
             "additionalProperties": false,
@@ -740,14 +913,21 @@
                 "qualifiers": {
                     "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
                     "items": {
                         "$ref": "#/$defs/Qualifier"
                     },
                     "type": "array"
                 },
+                "runner_settings": {
+                    "description": "Settings for the test harness, e.g. \"inferred\"",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "semantic_severity": {
                     "$ref": "#/$defs/SemanticSeverityEnum"
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection",
                     "items": {
                         "type": "string"
@@ -761,26 +941,21 @@
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_reference": {
                     "description": "Document URL where original test source particulars are registered (e.g. Github repo)",
                     "type": "string"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar settings for the TestRunner, e.g. \"inferred\"",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "well_known": {
                     "type": "boolean"
                 }
             },
             "required": [
+                "runner_settings",
+                "test_metadata",
                 "id"
             ],
             "title": "TestAsset",
             "type": "object"
         },
         "TestCase": {
             "additionalProperties": false,
@@ -797,37 +972,24 @@
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "id": {
                     "description": "A unique identifier for a Test Entity",
                     "type": "string"
                 },
-                "input_category": {
-                    "type": "string"
-                },
                 "name": {
                     "description": "A human-readable name for a Test Entity",
                     "type": "string"
                 },
-                "output_category": {
-                    "type": "string"
-                },
                 "preconditions": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "qualifiers": {
-                    "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
-                    "items": {
-                        "$ref": "#/$defs/Qualifier"
-                    },
-                    "type": "array"
-                },
                 "query_type": {
                     "$ref": "#/$defs/QueryTypeEnum",
                     "description": "Type of TestCase query."
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
                     "items": {
@@ -843,44 +1005,45 @@
                     "type": "array"
                 },
                 "test_case_input_id": {
                     "type": "string"
                 },
                 "test_case_objective": {
                     "$ref": "#/$defs/TestObjectiveEnum",
-                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)"
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
                 },
                 "test_case_predicate_id": {
                     "type": "string"
                 },
                 "test_case_predicate_name": {
                     "type": "string"
                 },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "test_case_source": {
                     "$ref": "#/$defs/TestSourceEnum",
                     "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
                 },
                 "test_env": {
                     "$ref": "#/$defs/TestEnvEnum",
                     "description": "Deployment environment within which the associated TestSuite is run."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "trapi_template": {
                     "$ref": "#/$defs/TrapiTemplateEnum",
                     "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
                 }
             },
             "required": [
                 "test_assets",
+                "test_case_runner_settings",
                 "id"
             ],
             "title": "TestCase",
             "type": "object"
         },
         "TestCaseResult": {
             "additionalProperties": false,
@@ -909,38 +1072,31 @@
                     "$ref": "#/$defs/TestCase",
                     "description": "Slot referencing a single TestCase."
                 },
                 "test_case_result": {
                     "$ref": "#/$defs/TestCaseResultEnum",
                     "description": "Encoded result of a single test run of a given test case"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_id": {
                     "description": "CURIE id of a TestSuite registered in the system.",
                     "type": "string"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "TestCaseResult",
             "type": "object"
         },
         "TestCaseResultEnum": {
             "description": "",
             "enum": [
-                "PASSED",
-                "FAILED",
-                "SKIPPED"
+                "test_passed",
+                "test_failed",
+                "test_skipped"
             ],
             "title": "TestCaseResultEnum",
             "type": "string"
         },
         "TestCaseResult__identifier_optional": {
             "additionalProperties": false,
             "description": "The outcome of a TestRunner run of one specific TestCase.",
@@ -968,21 +1124,14 @@
                     "$ref": "#/$defs/TestCase",
                     "description": "Slot referencing a single TestCase."
                 },
                 "test_case_result": {
                     "$ref": "#/$defs/TestCaseResultEnum",
                     "description": "Encoded result of a single test run of a given test case"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_id": {
                     "description": "CURIE id of a TestSuite registered in the system.",
                     "type": "string"
                 }
             },
             "required": [],
             "title": "TestCaseResult",
@@ -1003,37 +1152,24 @@
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "id": {
                     "description": "A unique identifier for a Test Entity",
                     "type": "string"
                 },
-                "input_category": {
-                    "type": "string"
-                },
                 "name": {
                     "description": "A human-readable name for a Test Entity",
                     "type": "string"
                 },
-                "output_category": {
-                    "type": "string"
-                },
                 "preconditions": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "qualifiers": {
-                    "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
-                    "items": {
-                        "$ref": "#/$defs/Qualifier"
-                    },
-                    "type": "array"
-                },
                 "query_type": {
                     "$ref": "#/$defs/QueryTypeEnum",
                     "description": "Type of TestCase query."
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.",
                     "items": {
@@ -1049,44 +1185,45 @@
                     "type": "array"
                 },
                 "test_case_input_id": {
                     "type": "string"
                 },
                 "test_case_objective": {
                     "$ref": "#/$defs/TestObjectiveEnum",
-                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)"
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
                 },
                 "test_case_predicate_id": {
                     "type": "string"
                 },
                 "test_case_predicate_name": {
                     "type": "string"
                 },
+                "test_case_runner_settings": {
+                    "description": "Settings for the test harness for TestCase",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "test_case_source": {
                     "$ref": "#/$defs/TestSourceEnum",
                     "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
                 },
                 "test_env": {
                     "$ref": "#/$defs/TestEnvEnum",
                     "description": "Deployment environment within which the associated TestSuite is run."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "trapi_template": {
                     "$ref": "#/$defs/TrapiTemplateEnum",
                     "description": "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory."
                 }
             },
             "required": [
-                "test_assets"
+                "test_assets",
+                "test_case_runner_settings"
             ],
             "title": "TestCase",
             "type": "object"
         },
         "TestEdgeData": {
             "additionalProperties": false,
             "description": "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing.",
@@ -1140,14 +1277,21 @@
                 "qualifiers": {
                     "description": "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.",
                     "items": {
                         "$ref": "#/$defs/Qualifier"
                     },
                     "type": "array"
                 },
+                "runner_settings": {
+                    "description": "Settings for the test harness, e.g. \"inferred\"",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "semantic_severity": {
                     "$ref": "#/$defs/SemanticSeverityEnum"
                 },
                 "tags": {
                     "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection",
                     "items": {
                         "type": "string"
@@ -1161,26 +1305,21 @@
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_reference": {
                     "description": "Document URL where original test source particulars are registered (e.g. Github repo)",
                     "type": "string"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar settings for the TestRunner, e.g. \"inferred\"",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "well_known": {
                     "type": "boolean"
                 }
             },
             "required": [
+                "runner_settings",
+                "test_metadata",
                 "id"
             ],
             "title": "TestEdgeData",
             "type": "object"
         },
         "TestEntityParameter": {
             "additionalProperties": false,
@@ -1250,27 +1389,20 @@
                     "items": {
                         "$ref": "#/$defs/TestEntityParameter"
                     },
                     "type": "array"
                 },
                 "test_objective": {
                     "$ref": "#/$defs/TestObjectiveEnum",
-                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)"
+                    "description": "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)"
                 },
                 "test_reference": {
                     "description": "Document URL where original test source particulars are registered (e.g. Github repo)",
                     "type": "string"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_source": {
                     "$ref": "#/$defs/TestSourceEnum",
                     "description": "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string."
                 }
             },
             "required": [
                 "id"
@@ -1279,17 +1411,15 @@
             "type": "object"
         },
         "TestObjectiveEnum": {
             "description": "",
             "enum": [
                 "AcceptanceTest",
                 "BenchmarkTest",
-                "QuantitativeTest",
-                "StandardsValidationTest",
-                "OneHopTest"
+                "QuantitativeTest"
             ],
             "title": "TestObjectiveEnum",
             "type": "string"
         },
         "TestOutput": {
             "additionalProperties": false,
             "description": "The output of a TestRunner run of one specific TestCase.",
@@ -1319,21 +1449,14 @@
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "test_case_id": {
                     "description": "CURIE id of a TestCase registered in the system.",
                     "type": "string"
-                },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "TestOutput",
             "type": "object"
@@ -1386,42 +1509,28 @@
                 "tags": {
                     "description": "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "unsecret": {
                     "type": "string"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "TestResultPKSet",
             "type": "object"
         },
         "TestRunSession": {
             "additionalProperties": false,
-            "description": "Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite).",
+            "description": "A single invocation of a TestRunner.",
             "properties": {
-                "components": {
-                    "description": "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.",
-                    "items": {
-                        "$ref": "#/$defs/ComponentEnum"
-                    },
-                    "type": "array"
-                },
                 "description": {
                     "description": "A human-readable description for a Test Entity",
                     "type": "string"
                 },
                 "id": {
                     "description": "A unique identifier for a Test Entity",
                     "type": "string"
@@ -1458,51 +1567,70 @@
                                 "$ref": "#/$defs/TestEntity__identifier_optional"
                             },
                             {
                                 "type": "null"
                             }
                         ]
                     },
-                    "description": "Different TestRunners could expect specific kinds of TestEntity as an input.  These 'test_entities' are one or more instances of TestAsset, TestCase or (preferably?) TestSuite.",
+                    "description": "Different TestRunners may expect specific kinds of TestEntity as input. These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite.",
                     "type": "object"
                 },
-                "test_env": {
-                    "$ref": "#/$defs/TestEnvEnum",
-                    "description": "Deployment environment within which the associated TestSuite is run."
-                },
-                "test_run_parameters": {
-                    "description": "Different TestRunners could expect additional global test configuration parameters, like the applicable TRAPI version (\"trapi_version\") or Biolink Model versions (\"biolink_version\").",
-                    "items": {
-                        "$ref": "#/$defs/TestEntityParameter"
-                    },
-                    "type": "array"
-                },
                 "test_runner_name": {
                     "description": "Global system name of a TestRunner.",
                     "type": "string"
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "timestamp": {
                     "description": "Date time when a given entity was created.",
                     "format": "date-time",
                     "type": "string"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "TestRunSession",
             "type": "object"
         },
+        "TestRunnerConfiguration": {
+            "additionalProperties": false,
+            "description": "General configuration parameters and test data input  for a single invocation of a TestRunner.",
+            "properties": {
+                "description": {
+                    "description": "A human-readable description for a Test Entity",
+                    "type": "string"
+                },
+                "id": {
+                    "description": "A unique identifier for a Test Entity",
+                    "type": "string"
+                },
+                "name": {
+                    "description": "A human-readable name for a Test Entity",
+                    "type": "string"
+                },
+                "tags": {
+                    "description": "One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration.",
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
+                "test_run_parameters": {
+                    "description": "Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run.",
+                    "items": {
+                        "$ref": "#/$defs/TestEntityParameter"
+                    },
+                    "type": "array"
+                }
+            },
+            "required": [
+                "id"
+            ],
+            "title": "TestRunnerConfiguration",
+            "type": "object"
+        },
         "TestSourceEnum": {
             "description": "",
             "enum": [
                 "SME",
                 "SMURF",
                 "GitHubUserFeedback",
                 "TACT",
@@ -1534,51 +1662,34 @@
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "test_cases": {
                     "additionalProperties": {
-                        "anyOf": [
-                            {
-                                "$ref": "#/$defs/TestCase__identifier_optional"
-                            },
-                            {
-                                "description": "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.",
-                                "items": {
-                                    "$ref": "#/$defs/TestAsset"
-                                },
-                                "type": "array"
-                            }
-                        ]
+                        "$ref": "#/$defs/TestCase__identifier_optional"
                     },
                     "description": "List of explicitly enumerated Test Cases.",
                     "type": "object"
                 },
                 "test_metadata": {
                     "$ref": "#/$defs/TestMetadata",
                     "description": "Test metadata describes the external provenance, cross-references and objectives for a given test."
                 },
                 "test_persona": {
                     "$ref": "#/$defs/TestPersonaEnum",
                     "description": "A Test persona describes the user or operational context of a given test."
                 },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
-                },
                 "test_suite_specification": {
                     "$ref": "#/$defs/TestSuiteSpecification",
                     "description": "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source."
                 }
             },
             "required": [
+                "test_metadata",
                 "id"
             ],
             "title": "TestSuite",
             "type": "object"
         },
         "TestSuiteSpecification": {
             "additionalProperties": false,
@@ -1606,21 +1717,14 @@
                 "test_data_file_format": {
                     "$ref": "#/$defs/FileFormatEnum",
                     "description": "File format of test entity data (e.g. TSV, YAML or JSON)"
                 },
                 "test_data_file_locator": {
                     "description": "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)",
                     "type": "string"
-                },
-                "test_runner_settings": {
-                    "description": "Scalar parameters for the TestRunner processing a given TestEntity.",
-                    "items": {
-                        "type": "string"
-                    },
-                    "type": "array"
                 }
             },
             "required": [
                 "id"
             ],
             "title": "TestSuiteSpecification",
             "type": "object"
@@ -1635,14 +1739,14 @@
                 "drug-to-gene"
             ],
             "title": "TrapiTemplateEnum",
             "type": "string"
         }
     },
     "$id": "https://w3id.org/TranslatorSRI/TranslatorTestingModel",
-    "$schema": "https://json-schema.org/draft/2019-09/schema",
+    "$schema": "http://json-schema.org/draft-07/schema#",
     "additionalProperties": true,
     "metamodel_version": "1.7.0",
     "title": "Translator-Testing-Model",
     "type": "object",
     "version": "0.0.0"
 }
```

### Comparing `translator_testing_model-0.3.1/project/owl/translator_testing_model.owl.ttl` & `translator_testing_model-2.3.0/project/owl/translator_testing_model.owl.ttl`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 @prefix dcterms: <http://purl.org/dc/terms/> .
-@prefix infores: <https://w3id.org/biolink/vocab/> .
 @prefix linkml: <https://w3id.org/linkml/> .
 @prefix owl: <http://www.w3.org/2002/07/owl#> .
 @prefix pav: <http://purl.org/pav/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
 @prefix skos: <http://www.w3.org/2004/02/skos/core#> .
 @prefix ttm: <https://w3id.org/TranslatorSRI/TranslatorTestingModel/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 ttm:AcceptanceTestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AcceptanceTestCase" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom ttm:AcceptanceTestAsset ;
+            owl:minCardinality 1 ;
             owl:onProperty ttm:test_assets ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
+            owl:allValuesFrom ttm:AcceptanceTestAsset ;
             owl:onProperty ttm:test_assets ],
         ttm:TestCase ;
     skos:definition "See AcceptanceTestAsset above for more details." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:AcceptanceTestSuite a owl:Class,
         linkml:ClassDefinition ;
@@ -30,14 +29,46 @@
 
 ttm:BenchmarkTestSuite a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "BenchmarkTestSuite" ;
     skos:definition "JsonObj(is_a='TestSuite')" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:ComplianceTestCase a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "ComplianceTestCase" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:trapi_version ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:biolink_version ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:trapi_version ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:biolink_version ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:biolink_version ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:trapi_version ],
+        ttm:TestCase ;
+    skos:definition "TRAPI and Biolink Model standards compliance test" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:OneHopTestCase a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "OneHopTestCase" ;
+    rdfs:subClassOf ttm:KnowledgeGraphNavigationTestCase ;
+    skos:definition "'One Hop' Knowledge Graph navigation integration test" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:OneHopTestSuite a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "OneHopTestSuite" ;
     rdfs:subClassOf ttm:TestSuite ;
     skos:definition "Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
@@ -62,69 +93,67 @@
     skos:definition "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestRunSession a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestRunSession" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_run_parameters ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_runner_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty ttm:test_entities ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestCaseResult ;
             owl:onProperty ttm:test_case_results ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:ComponentEnum ;
-            owl:onProperty ttm:components ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_runner_name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEntity ;
-            owl:onProperty ttm:test_entities ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_results ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:timestamp ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_run_parameters ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_entities ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Datetime ;
             owl:onProperty ttm:timestamp ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEnvEnum ;
-            owl:onProperty ttm:test_env ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_run_parameters ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_entities ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:timestamp ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_runner_name ],
+        ttm:TestEntity ;
+    skos:definition "A single invocation of a TestRunner." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:TestRunnerConfiguration a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "TestRunnerConfiguration" ;
+    rdfs:subClassOf [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_env ],
+            owl:onProperty ttm:test_run_parameters ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:components ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_runner_name ],
+            owl:onProperty ttm:test_run_parameters ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_env ],
+            owl:onProperty ttm:test_run_parameters ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_runner_name ],
+            owl:onProperty ttm:tags ],
         ttm:TestEntity ;
-    skos:definition "Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite)." ;
+    skos:definition "General configuration parameters and test data input  for a single invocation of a TestRunner." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:biolink_object_aspect_qualifier a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "biolink_object_aspect_qualifier" ;
     skos:definition "The aspect of the object of the test asset predicate" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
@@ -157,157 +186,155 @@
 
 ttm:biolink_subject_direction_qualifier a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "biolink_subject_direction_qualifier" ;
     skos:definition "The direction of the subject of the test asset predicate" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:biolink_version a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "biolink_version" ;
-    skos:definition "Biolink Model release (SemVer string)" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
 ttm:results a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "results" ;
     rdfs:range ttm:TestOutput ;
     skos:definition "The results of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:trapi_version a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "trapi_version" ;
-    skos:definition "TRAPI version (SemVer string)" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
 ttm:AcceptanceTestAsset a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "AcceptanceTestAsset" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:scientific_question ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:notes ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:top_level ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
             owl:onProperty ttm:query_node ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:answer_informal_concept ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:answer_informal_concept ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEnvEnum ;
-            owl:onProperty ttm:must_pass_environment ],
+            owl:onProperty ttm:expected_result ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:answer_informal_concept ],
+            owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Date ;
-            owl:onProperty ttm:must_pass_date ],
+            owl:allValuesFrom ttm:NodeEnum ;
+            owl:onProperty ttm:query_node ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:notes ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:answer_informal_concept ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:string_entry ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:query_node ],
+        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:must_pass_environment ],
+            owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:expected_result ],
+            owl:allValuesFrom linkml:Date ;
+            owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:top_level ],
+            owl:allValuesFrom ttm:DirectionEnum ;
+            owl:onProperty ttm:direction ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:query_node ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:answer_informal_concept ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:direction ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom ttm:TestEnvEnum ;
             owl:onProperty ttm:must_pass_environment ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:NodeEnum ;
-            owl:onProperty ttm:query_node ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:notes ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:notes ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:scientific_question ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
             owl:onProperty ttm:string_entry ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:expected_result ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:notes ],
+            owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:direction ],
+            owl:onProperty ttm:must_pass_date ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:ExpectedResultsEnum ;
-            owl:onProperty ttm:expected_result ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:must_pass_environment ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:must_pass_date ],
+            owl:onProperty ttm:answer_informal_concept ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:DirectionEnum ;
-            owl:onProperty ttm:direction ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:scientific_question ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Integer ;
             owl:onProperty ttm:top_level ],
         [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:direction ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:must_pass_environment ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:expected_result ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:ExpectedResultsEnum ;
+            owl:onProperty ttm:expected_result ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:string_entry ],
         ttm:TestAsset ;
     skos:definition "Model derived from Jenn's test asset design and Shervin's runner JSON here as an example." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:KnowledgeGraphNavigationTestCase a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "KnowledgeGraphNavigationTestCase" ;
+    rdfs:subClassOf ttm:TestCase ;
+    skos:definition "Knowledge Graph navigation integration test" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/QueryTypeEnum#treats> a owl:Class,
         ttm:QueryTypeEnum ;
     rdfs:label "treats" ;
     rdfs:subClassOf ttm:QueryTypeEnum .
 
 ttm:TestOutput a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestOutput" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_case_id ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:pks ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_id ],
-        [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestResultPKSet ;
             owl:onProperty ttm:pks ],
         [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_case_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_case_id ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:test_case_id ],
         ttm:TestEntity ;
     skos:definition "The output of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:ComponentEnum a owl:Class,
+        linkml:EnumDefinition .
+
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#decreased> a owl:Class,
         ttm:DirectionEnum ;
     rdfs:label "decreased" ;
     rdfs:subClassOf ttm:DirectionEnum .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#increased> a owl:Class,
         ttm:DirectionEnum ;
@@ -377,14 +404,38 @@
 ttm:Precondition a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "Precondition" ;
     rdfs:subClassOf ttm:TestEntity ;
     skos:definition "Represents a precondition for a TestCase" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:Qualifier a owl:Class,
+        linkml:ClassDefinition ;
+    rdfs:label "Qualifier" ;
+    rdfs:subClassOf [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:parameter ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:value ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:parameter ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:value ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:parameter ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:value ],
+        ttm:TestEntityParameter ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High> a owl:Class,
         ttm:SemanticSeverityEnum ;
     rdfs:label "High" ;
     rdfs:subClassOf ttm:SemanticSeverityEnum .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low> a owl:Class,
         ttm:SemanticSeverityEnum ;
@@ -396,79 +447,79 @@
     rdfs:label "NotApplicable" ;
     rdfs:subClassOf ttm:SemanticSeverityEnum .
 
 ttm:TestCaseResult a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestCaseResult" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_suite_id ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestCaseResultEnum ;
-            owl:onProperty ttm:test_case_result ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:test_suite_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_result ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:test_suite_id ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_result ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_suite_id ],
-        [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestCase ;
             owl:onProperty ttm:test_case ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case ],
+            owl:onProperty ttm:test_suite_id ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_suite_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestCaseResultEnum ;
+            owl:onProperty ttm:test_case_result ],
         ttm:TestEntity ;
     skos:definition "The outcome of a TestRunner run of one specific TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#FAILED> a owl:Class,
+<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_failed> a owl:Class,
         ttm:TestCaseResultEnum ;
-    rdfs:label "FAILED" ;
+    rdfs:label "test_failed" ;
     rdfs:subClassOf ttm:TestCaseResultEnum .
 
-<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#PASSED> a owl:Class,
+<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_passed> a owl:Class,
         ttm:TestCaseResultEnum ;
-    rdfs:label "PASSED" ;
+    rdfs:label "test_passed" ;
     rdfs:subClassOf ttm:TestCaseResultEnum .
 
-<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#SKIPPED> a owl:Class,
+<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_skipped> a owl:Class,
         ttm:TestCaseResultEnum ;
-    rdfs:label "SKIPPED" ;
+    rdfs:label "test_skipped" ;
     rdfs:subClassOf ttm:TestCaseResultEnum .
 
 ttm:TestEntityParameter a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestEntityParameter" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:value ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:value ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:parameter ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:value ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:value ] ;
     skos:definition "A single 'tag = value' pair (where 'value' is a simple string)." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci> a owl:Class,
         ttm:TestEnvEnum ;
     rdfs:label "ci" ;
@@ -525,29 +576,19 @@
     rdfs:subClassOf ttm:TestObjectiveEnum .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#BenchmarkTest> a owl:Class,
         ttm:TestObjectiveEnum ;
     rdfs:label "BenchmarkTest" ;
     rdfs:subClassOf ttm:TestObjectiveEnum .
 
-<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#OneHopTest> a owl:Class,
-        ttm:TestObjectiveEnum ;
-    rdfs:label "OneHopTest" ;
-    rdfs:subClassOf ttm:TestObjectiveEnum .
-
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#QuantitativeTest> a owl:Class,
         ttm:TestObjectiveEnum ;
     rdfs:label "QuantitativeTest" ;
     rdfs:subClassOf ttm:TestObjectiveEnum .
 
-<https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#StandardsValidationTest> a owl:Class,
-        ttm:TestObjectiveEnum ;
-    rdfs:label "StandardsValidationTest" ;
-    rdfs:subClassOf ttm:TestObjectiveEnum .
-
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#All> a owl:Class,
         ttm:TestPersonaEnum ;
     rdfs:label "All" ;
     rdfs:subClassOf ttm:TestPersonaEnum .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Clinical> a owl:Class,
         ttm:TestPersonaEnum ;
@@ -568,72 +609,72 @@
         linkml:ClassDefinition ;
     rdfs:label "TestResultPKSet" ;
     rdfs:subClassOf [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:parent_pk ],
+            owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:bte ],
+            owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:parent_pk ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:bte ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
+            owl:onProperty ttm:arax ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:unsecret ],
+            owl:onProperty ttm:aragorn ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:improving ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:merged_pk ],
-        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:arax ],
+            owl:onProperty ttm:bte ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:parent_pk ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:unsecret ],
+            owl:onProperty ttm:bte ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:aragorn ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:bte ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:aragorn ],
+            owl:onProperty ttm:merged_pk ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:bte ],
+            owl:onProperty ttm:unsecret ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:unsecret ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:arax ],
+            owl:onProperty ttm:parent_pk ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:improving ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:unsecret ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
+            owl:onProperty ttm:parent_pk ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:arax ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:unsecret ],
+            owl:onProperty ttm:arax ],
         ttm:TestEntity ;
     skos:definition "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#BenchMark> a owl:Class,
         ttm:TestSourceEnum ;
     rdfs:label "BenchMark" ;
@@ -665,31 +706,31 @@
     rdfs:label "TranslatorTeam" ;
     rdfs:subClassOf ttm:TestSourceEnum .
 
 ttm:TestSuiteSpecification a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestSuiteSpecification" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_data_file_format ],
-        [ a owl:Restriction ;
             owl:allValuesFrom ttm:FileFormatEnum ;
             owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_data_file_locator ],
+            owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_data_file_locator ],
+            owl:onProperty ttm:test_data_file_format ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:test_data_file_locator ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_data_file_format ],
+            owl:onProperty ttm:test_data_file_locator ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_data_file_locator ],
         ttm:TestEntity ;
     skos:definition "Parameters for a Test Case instances either dynamically generated from some external source of Test Assets." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#ameliorates> a owl:Class,
         ttm:TrapiTemplateEnum ;
     rdfs:label "ameliorates" ;
@@ -719,14 +760,21 @@
         linkml:TypeDefinition ;
     rdfs:subClassOf ttm:category_type .
 
 ttm:category_type a owl:Class,
         linkml:TypeDefinition ;
     rdfs:subClassOf linkml:Uriorcurie .
 
+ttm:components a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "components" ;
+    rdfs:range ttm:ComponentEnum ;
+    skos:definition "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:pks a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "pks" ;
     rdfs:range ttm:TestResultPKSet ;
     skos:definition "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
@@ -736,21 +784,44 @@
     rdfs:range ttm:Precondition ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:predicate_type a owl:Class,
         linkml:TypeDefinition ;
     rdfs:subClassOf linkml:Uriorcurie .
 
+ttm:qualifiers a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "qualifiers" ;
+    rdfs:range ttm:Qualifier ;
+    skos:definition "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:runner_settings a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "runner_settings" ;
+    rdfs:range linkml:String ;
+    skos:altLabel "Settings" ;
+    skos:definition "Settings for the test harness for TestAsset" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:test_case_results a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_case_results" ;
     rdfs:range ttm:TestCaseResult ;
     skos:definition "One or more instances of TestCaseResult." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:test_case_runner_settings a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "test_case_runner_settings" ;
+    rdfs:range linkml:String ;
+    skos:altLabel "Settings" ;
+    skos:definition "Settings for the test harness for TestCase" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:test_cases a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_cases" ;
     rdfs:range ttm:TestCase ;
     skos:definition "List of explicitly enumerated Test Cases." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
@@ -761,210 +832,279 @@
     skos:definition "One or more instances of TestEntity, generally of class TestAsset, TestCase or TestSuite." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_entity_parameters a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_entity_parameters" ;
     rdfs:range ttm:TestEntityParameter ;
-    skos:definition "One or more 'tag = value' parameters documenting target characteristics of a TestEntity." ;
+    skos:definition "One or more parameters documenting target characteristics of a TestEntity." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-infores:aragorn a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "aragorn" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:arax a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "arax" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:biothings-explorer a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "bte" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:cam-kp a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "cam" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:cohd a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "cohd" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:connections-hypothesis a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "connections" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:explanatory-agent a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "explanatory" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:icees-kg a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "icees" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:improving-agent a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "improving" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:knowledge-collaboratory a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "collaboratory" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:molepro a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "molepro" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:ncats-ars a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "ars" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:openpredict a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "openpredict" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:rtx-kg2 a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "rtxkg2" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:spoke a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "spoke" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:textmining-kp a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "textmining" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-infores:unsecret-agent a owl:Class,
-        ttm:ComponentEnum ;
-    rdfs:label "unsecret" ;
-    rdfs:subClassOf ttm:ComponentEnum .
-
-ttm:Qualifier a owl:Class,
+ttm:TestAsset a owl:Class,
         linkml:ClassDefinition ;
-    rdfs:label "Qualifier" ;
+    rdfs:label "TestAsset" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:predicate_name ],
+        [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:parameter ],
+            owl:onProperty ttm:qualifiers ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:input_category ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:runner_settings ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_metadata ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:input_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:predicate_type ;
+            owl:onProperty ttm:predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:value ],
+            owl:onProperty ttm:predicate_id ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:value ],
+            owl:onProperty ttm:expected_output ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:semantic_severity ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:id ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:output_category ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:predicate_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestIssueEnum ;
+            owl:onProperty ttm:test_issue ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_reference ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:concept_category ;
+            owl:onProperty ttm:output_category ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:output_id ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:in_v1 ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:value ],
+            owl:onProperty ttm:output_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty ttm:well_known ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:output_category ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:input_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:input_category ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:association ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:output_name ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_issue ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:output_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Boolean ;
+            owl:onProperty ttm:in_v1 ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:tags ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:runner_settings ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:input_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:association_category ;
+            owl:onProperty ttm:association ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:well_known ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:parameter ],
+            owl:onProperty ttm:input_name ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:expected_output ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:input_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:parameter ],
-        ttm:TestEntityParameter ;
+            owl:onProperty ttm:output_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:output_id ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:input_name ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:semantic_severity ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:expected_output ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestMetadata ;
+            owl:onProperty ttm:test_metadata ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:concept_category ;
+            owl:onProperty ttm:input_category ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:tags ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:SemanticSeverityEnum ;
+            owl:onProperty ttm:semantic_severity ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:predicate_id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:test_reference ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:id ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:Qualifier ;
+            owl:onProperty ttm:qualifiers ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:predicate_name ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:in_v1 ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:well_known ],
+        [ a owl:Restriction ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_issue ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:test_metadata ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:association ],
+        ttm:TestEntity ;
+    skos:definition "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:TestMetadata a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestMetadata" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_annotations ],
+        [ a owl:Restriction ;
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_objective ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestObjectiveEnum ;
+            owl:onProperty ttm:test_objective ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:Uriorcurie ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_annotations ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_objective ],
+            owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestSourceEnum ;
             owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_objective ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_source ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_annotations ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_objective ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_reference ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_source ],
-        [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_annotations ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestObjectiveEnum ;
-            owl:onProperty ttm:test_objective ],
         ttm:TestEntity ;
     skos:definition "Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#GitHubUserFeedback> a owl:Class,
         ttm:TestSourceEnum ;
     rdfs:label "GitHubUserFeedback" ;
     rdfs:subClassOf ttm:TestSourceEnum .
 
 ttm:TestSuite a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestSuite" ;
     rdfs:subClassOf [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestSuiteSpecification ;
+            owl:onProperty ttm:test_suite_specification ],
+        [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestMetadata ;
             owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_suite_specification ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_persona ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_persona ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_cases ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_metadata ],
+            owl:onProperty ttm:test_suite_specification ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:minCardinality 1 ;
             owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_cases ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestPersonaEnum ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_persona ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_suite_specification ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_metadata ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestCase ;
             owl:onProperty ttm:test_cases ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestSuiteSpecification ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:test_suite_specification ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:TestPersonaEnum ;
+            owl:onProperty ttm:test_persona ],
         ttm:TestEntity ;
     skos:definition "Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:answer_informal_concept a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "answer_informal_concept" ;
@@ -985,14 +1125,20 @@
 ttm:association a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "association" ;
     rdfs:range ttm:association_category ;
     skos:definition "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:biolink_version a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "biolink_version" ;
+    skos:definition "Biolink Model release (SemVer string)" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:bte a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "bte" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:description a owl:ObjectProperty,
         linkml:SlotDefinition ;
@@ -1028,14 +1174,21 @@
 ttm:in_v1 a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "in_v1" ;
     rdfs:range linkml:Boolean ;
     skos:altLabel "In v1" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:input_category a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "input_category" ;
+    rdfs:range ttm:concept_category ;
+    skos:altLabel "SubjectCategory" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:input_id a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "input_id" ;
     rdfs:range linkml:Uriorcurie ;
     skos:altLabel "InputID, node normalized",
         "SubjectID" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
@@ -1075,14 +1228,21 @@
 ttm:notes a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "notes" ;
     rdfs:range linkml:String ;
     skos:definition "The notes of the query" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:output_category a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "output_category" ;
+    rdfs:range ttm:concept_category ;
+    skos:altLabel "ObjectCategory" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:output_id a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "output_id" ;
     rdfs:range linkml:Uriorcurie ;
     skos:altLabel "ObjectID",
         "OutputID" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
@@ -1179,15 +1339,15 @@
         "SubjectID" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_case_objective a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_case_objective" ;
     rdfs:range ttm:TestObjectiveEnum ;
-    skos:definition "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
+    skos:definition "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_case_predicate_id a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_case_predicate_id" ;
     skos:altLabel "Predicate" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
@@ -1222,40 +1382,47 @@
 ttm:test_data_file_locator a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_data_file_locator" ;
     rdfs:range linkml:Uriorcurie ;
     skos:definition "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:test_env a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "test_env" ;
+    rdfs:range ttm:TestEnvEnum ;
+    skos:definition "Deployment environment within which the associated TestSuite is run." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:test_issue a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_issue" ;
     rdfs:range ttm:TestIssueEnum ;
     skos:altLabel "issue label" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_objective a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_objective" ;
     rdfs:range ttm:TestObjectiveEnum ;
-    skos:definition "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
+    skos:definition "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_persona a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_persona" ;
     rdfs:range ttm:TestPersonaEnum ;
     skos:definition "A Test persona describes the user or operational context of a given test." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_run_parameters a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_run_parameters" ;
     rdfs:subPropertyOf ttm:test_entity_parameters ;
-    skos:definition "TestRunSession parameters informing a TestHarness about the global characteristics of TestRunner processing tests." ;
+    skos:definition "Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:test_runner_name a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_runner_name" ;
     skos:definition "Global system name of a TestRunner." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
@@ -1298,14 +1465,20 @@
 ttm:trapi_template a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "trapi_template" ;
     rdfs:range ttm:TrapiTemplateEnum ;
     skos:definition "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:trapi_version a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "trapi_version" ;
+    skos:definition "TRAPI version (SemVer string)" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
 ttm:unsecret a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "unsecret" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:well_known a owl:ObjectProperty,
         linkml:SlotDefinition ;
@@ -1314,221 +1487,25 @@
     skos:altLabel "Well Known" ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
 ttm:QueryTypeEnum a owl:Class,
         linkml:EnumDefinition ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/QueryTypeEnum#treats> .
 
-ttm:TestAsset a owl:Class,
-        linkml:ClassDefinition ;
-    rdfs:label "TestAsset" ;
-    rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:input_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_metadata ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:association_category ;
-            owl:onProperty ttm:association ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_runner_settings ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:association ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:input_name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:predicate_name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty ttm:well_known ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:input_name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:output_name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:well_known ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:in_v1 ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:qualifiers ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:tags ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:predicate_name ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:association ],
-        [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:predicate_type ;
-            owl:onProperty ttm:predicate_id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:semantic_severity ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_runner_settings ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_reference ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:test_reference ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:expected_output ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_category ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:expected_output ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_reference ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestIssueEnum ;
-            owl:onProperty ttm:test_issue ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:predicate_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:output_id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:input_category ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:well_known ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Boolean ;
-            owl:onProperty ttm:in_v1 ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_issue ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:predicate_name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:predicate_id ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:in_v1 ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_issue ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:semantic_severity ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestMetadata ;
-            owl:onProperty ttm:test_metadata ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:Qualifier ;
-            owl:onProperty ttm:qualifiers ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:expected_output ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:output_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:SemanticSeverityEnum ;
-            owl:onProperty ttm:semantic_severity ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_metadata ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:tags ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_name ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:output_name ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:input_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:input_category ],
-        ttm:TestEntity ;
-    skos:definition "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:components a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "components" ;
-    rdfs:range ttm:ComponentEnum ;
-    skos:definition "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:qualifiers a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "qualifiers" ;
-    rdfs:range ttm:Qualifier ;
-    skos:definition "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+ttm:concept_category a owl:Class,
+        linkml:TypeDefinition ;
+    rdfs:subClassOf ttm:category_type .
 
 ttm:test_assets a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "test_assets" ;
     rdfs:range ttm:TestAsset ;
     skos:definition "List of explicitly enumerated Test Assets. The class attributes of TestAsset would be included in the TestCase versus being referred to by the identifier (curie) of the TestAsset. That is, this would be a list of objects (in JSONSchema serialization) versus a list of strings (where each string is an identifier pointing to another class)." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:test_runner_settings a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "test_runner_settings" ;
-    rdfs:range linkml:String ;
-    skos:altLabel "Settings" ;
-    skos:definition "Scalar parameters for the TestRunner processing a given TestEntity." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
 ttm:DirectionEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#increased> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#decreased> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#decreased>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/DirectionEnum#increased> .
 
 ttm:ExpectedResultsEnum a owl:Class,
@@ -1539,357 +1516,285 @@
 
 ttm:NodeEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/NodeEnum#subject> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/NodeEnum#object> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/NodeEnum#object>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/NodeEnum#subject> .
 
+ttm:id a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "id" ;
+    rdfs:range linkml:Uriorcurie ;
+    skos:definition "A unique identifier for a Test Entity" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:parameter a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "parameter" ;
+    skos:definition "Name of a TestParameter." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:test_metadata a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "test_metadata" ;
+    rdfs:range ttm:TestMetadata ;
+    skos:definition "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:test_reference a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "test_reference" ;
+    rdfs:range linkml:Uriorcurie ;
+    skos:altLabel "GitHubIssue" ;
+    skos:definition "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:value a owl:ObjectProperty,
+        linkml:SlotDefinition ;
+    rdfs:label "value" ;
+    skos:definition "(String) value of a TestParameter." ;
+    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+
+ttm:FileFormatEnum a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#TSV> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#YAML> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#JSON> ) ;
+    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#JSON>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#TSV>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#YAML> .
+
+ttm:SemanticSeverityEnum a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#NotApplicable> ) ;
+    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#NotApplicable> .
+
 ttm:TestCase a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestCase" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_predicate_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:Precondition ;
-            owl:onProperty ttm:preconditions ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:input_category ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:trapi_template ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:QueryTypeEnum ;
             owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:qualifiers ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:tags ],
-        [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_env ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:query_type ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_input_id ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TrapiTemplateEnum ;
-            owl:onProperty ttm:trapi_template ],
+            owl:allValuesFrom ttm:TestObjectiveEnum ;
+            owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:trapi_template ],
+            owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:query_type ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestEnvEnum ;
-            owl:onProperty ttm:test_env ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:concept_category ;
-            owl:onProperty ttm:output_category ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom ttm:ComponentEnum ;
-            owl:onProperty ttm:components ],
+            owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:input_category ],
+            owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_env ],
+            owl:onProperty ttm:trapi_template ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_case_objective ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:components ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:input_category ],
+            owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:Qualifier ;
-            owl:onProperty ttm:qualifiers ],
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:test_case_predicate_name ],
         [ a owl:Restriction ;
             owl:allValuesFrom ttm:TestSourceEnum ;
             owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:test_case_input_id ],
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:query_type ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:test_case_source ],
         [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_predicate_id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_case_predicate_name ],
+            owl:onProperty ttm:test_case_runner_settings ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestObjectiveEnum ;
+            owl:maxCardinality 1 ;
             owl:onProperty ttm:test_case_objective ],
         [ a owl:Restriction ;
-            owl:allValuesFrom ttm:TestAsset ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:test_case_runner_settings ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:Precondition ;
+            owl:onProperty ttm:preconditions ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
             owl:onProperty ttm:test_assets ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_predicate_name ],
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:test_case_input_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
+            owl:allValuesFrom owl:Thing ;
+            owl:onProperty ttm:test_assets ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom ttm:ComponentEnum ;
             owl:onProperty ttm:components ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:minCardinality 0 ;
+            owl:onProperty ttm:test_case_predicate_name ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:test_case_predicate_id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
-            owl:onProperty ttm:test_case_objective ],
+            owl:onProperty ttm:preconditions ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_case_predicate_name ],
+            owl:onProperty ttm:test_case_input_id ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:trapi_template ],
+            owl:allValuesFrom ttm:TestEnvEnum ;
+            owl:onProperty ttm:test_env ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:test_assets ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:test_env ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
-            owl:onProperty ttm:test_case_input_id ],
+            owl:onProperty ttm:test_case_predicate_name ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:preconditions ],
+            owl:allValuesFrom ttm:TrapiTemplateEnum ;
+            owl:onProperty ttm:trapi_template ],
+        [ a owl:Restriction ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:tags ],
         ttm:TestEntity ;
     skos:definition "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:concept_category a owl:Class,
-        linkml:TypeDefinition ;
-    rdfs:subClassOf ttm:category_type .
-
-ttm:id a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "id" ;
-    rdfs:range linkml:Uriorcurie ;
-    skos:definition "A unique identifier for a Test Entity" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:input_category a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "input_category" ;
-    rdfs:range ttm:concept_category ;
-    skos:altLabel "SubjectCategory" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:output_category a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "output_category" ;
-    rdfs:range ttm:concept_category ;
-    skos:altLabel "ObjectCategory" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:parameter a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "parameter" ;
-    skos:definition "Name of a TestParameter." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
+ttm:TestCaseResultEnum a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_passed> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_failed> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_skipped> ) ;
+    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_failed>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_passed>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#test_skipped> .
 
 ttm:tags a owl:ObjectProperty,
         linkml:SlotDefinition ;
     rdfs:label "tags" ;
     skos:definition "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
-ttm:test_env a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "test_env" ;
-    rdfs:range ttm:TestEnvEnum ;
-    skos:definition "Deployment environment within which the associated TestSuite is run." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:test_metadata a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "test_metadata" ;
-    rdfs:range ttm:TestMetadata ;
-    skos:definition "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:test_reference a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "test_reference" ;
-    rdfs:range linkml:Uriorcurie ;
-    skos:altLabel "GitHubIssue" ;
-    skos:definition "Document URL where original test source particulars are registered (e.g. Github repo)" ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:value a owl:ObjectProperty,
-        linkml:SlotDefinition ;
-    rdfs:label "value" ;
-    skos:definition "(String) value of a TestParameter." ;
-    skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
-
-ttm:FileFormatEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#TSV> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#YAML> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#JSON> ) ;
-    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#JSON>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#TSV>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/FileFormatEnum#YAML> .
-
-ttm:SemanticSeverityEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#NotApplicable> ) ;
-    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#High>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#Low>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/SemanticSeverityEnum#NotApplicable> .
-
-ttm:TestCaseResultEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#PASSED> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#FAILED> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#SKIPPED> ) ;
-    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#FAILED>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#PASSED>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestCaseResultEnum#SKIPPED> .
-
 ttm:ExpectedOutputEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#Acceptable> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#BadButForgivable> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#NeverShow> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#TopAnswer> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#OverlyGeneric> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#Acceptable>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#BadButForgivable>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#NeverShow>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#OverlyGeneric>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/ExpectedOutputEnum#TopAnswer> .
 
+ttm:TestObjectiveEnum a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#AcceptanceTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#BenchmarkTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#QuantitativeTest> ) ;
+    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#AcceptanceTest>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#BenchmarkTest>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#QuantitativeTest> .
+
 ttm:TestPersonaEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#All> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Clinical> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#LookUp> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Mechanistic> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#All>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Clinical>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#LookUp>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestPersonaEnum#Mechanistic> .
 
 ttm:TestEntity a owl:Class,
         linkml:ClassDefinition ;
     rdfs:label "TestEntity" ;
     rdfs:subClassOf [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:description ],
-        [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:test_runner_settings ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:Uriorcurie ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:name ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:description ],
         [ a owl:Restriction ;
-            owl:maxCardinality 1 ;
+            owl:allValuesFrom linkml:String ;
             owl:onProperty ttm:name ],
         [ a owl:Restriction ;
+            owl:allValuesFrom linkml:Uriorcurie ;
+            owl:onProperty ttm:id ],
+        [ a owl:Restriction ;
             owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:name ],
+            owl:onProperty ttm:tags ],
+        [ a owl:Restriction ;
+            owl:minCardinality 1 ;
+            owl:onProperty ttm:id ],
         [ a owl:Restriction ;
             owl:minCardinality 0 ;
             owl:onProperty ttm:description ],
         [ a owl:Restriction ;
             owl:maxCardinality 1 ;
             owl:onProperty ttm:id ],
         [ a owl:Restriction ;
-            owl:minCardinality 1 ;
-            owl:onProperty ttm:id ],
-        [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
-            owl:onProperty ttm:test_runner_settings ],
+            owl:maxCardinality 1 ;
+            owl:onProperty ttm:name ],
         [ a owl:Restriction ;
-            owl:allValuesFrom linkml:String ;
+            owl:minCardinality 0 ;
             owl:onProperty ttm:tags ],
         [ a owl:Restriction ;
-            owl:minCardinality 0 ;
-            owl:onProperty ttm:tags ] ;
+            owl:allValuesFrom linkml:String ;
+            owl:onProperty ttm:description ] ;
     skos:definition "Abstract global 'identification' class shared as a parent with all major model classes within the data model for Translator testing." ;
     skos:inScheme <https://w3id.org/TranslatorSRI/TranslatorTestingModel> .
 
+ttm:TestEnvEnum a owl:Class,
+        linkml:EnumDefinition ;
+    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#dev> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#test> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#prod> ) ;
+    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#dev>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#prod>,
+        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#test> .
+
 ttm:TrapiTemplateEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#ameliorates> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#treats> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#three_hop> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#drug_treats_rare_disease> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#drug-to-gene> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#ameliorates>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#drug-to-gene>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#drug_treats_rare_disease>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#three_hop>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TrapiTemplateEnum#treats> .
 
-ttm:TestEnvEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#dev> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#test> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#prod> ) ;
-    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#ci>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#dev>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#prod>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestEnvEnum#test> .
-
 ttm:TestIssueEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#causes+not+treats> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#TMKP> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#category+too+generic> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#contraindications> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#chemical+roles> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#test_issue> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#TMKP>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#category+too+generic>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#causes+not+treats>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#chemical+roles>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#contraindications>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestIssueEnum#test_issue> .
 
-ttm:TestObjectiveEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#AcceptanceTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#BenchmarkTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#QuantitativeTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#StandardsValidationTest> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#OneHopTest> ) ;
-    linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#AcceptanceTest>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#BenchmarkTest>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#OneHopTest>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#QuantitativeTest>,
-        <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestObjectiveEnum#StandardsValidationTest> .
-
 ttm:TestSourceEnum a owl:Class,
         linkml:EnumDefinition ;
     owl:unionOf ( <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#SME> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#SMURF> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#GitHubUserFeedback> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TACT> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#BenchMark> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TranslatorTeam> <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TestDataLocation> ) ;
     linkml:permissible_values <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#BenchMark>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#GitHubUserFeedback>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#SME>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#SMURF>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TACT>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TestDataLocation>,
         <https://w3id.org/TranslatorSRI/TranslatorTestingModel/TestSourceEnum#TranslatorTeam> .
 
-ttm:ComponentEnum a owl:Class,
-        linkml:EnumDefinition ;
-    owl:unionOf ( infores:ncats-ars infores:arax infores:explanatory-agent infores:improving-agent infores:aragorn infores:biothings-explorer infores:unsecret-agent infores:rtx-kg2 infores:icees-kg infores:cam-kp infores:spoke infores:molepro infores:textmining-kp infores:cohd infores:openpredict infores:knowledge-collaboratory infores:connections-hypothesis ) ;
-    linkml:permissible_values infores:aragorn,
-        infores:arax,
-        infores:biothings-explorer,
-        infores:cam-kp,
-        infores:cohd,
-        infores:connections-hypothesis,
-        infores:explanatory-agent,
-        infores:icees-kg,
-        infores:improving-agent,
-        infores:knowledge-collaboratory,
-        infores:molepro,
-        infores:ncats-ars,
-        infores:openpredict,
-        infores:rtx-kg2,
-        infores:spoke,
-        infores:textmining-kp,
-        infores:unsecret-agent .
-
 <https://w3id.org/TranslatorSRI/TranslatorTestingModel> a owl:Ontology ;
     rdfs:label "Translator-Testing-Model" ;
     dcterms:license "MIT" ;
     dcterms:title "Translator Testing Data Model" ;
     pav:version "0.0.0" ;
     rdfs:seeAlso <https://TranslatorSRI.github.io/TranslatorTestingModel> ;
     skos:definition """Data model to formalize the structure of test assets, cases, suites and related metadata
```

### Comparing `translator_testing_model-0.3.1/project/protobuf/translator_testing_model.proto` & `translator_testing_model-2.3.0/project/protobuf/translator_testing_model.proto`

 * *Files 26% similar despite different names*

```diff
@@ -15,18 +15,18 @@
  repeated  qualifier qualifiers = 0
   string expectedOutput = 0
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
+ repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
   uriorcurie id = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   date mustPassDate = 0
   testEnvEnum mustPassEnvironment = 0
   string scientificQuestion = 0
   string stringEntry = 0
   directionEnum direction = 0
   string answerInformalConcept = 0
   expectedResultsEnum expectedResult = 0
@@ -36,101 +36,153 @@
  }
 // See AcceptanceTestAsset above for more details.
 message AcceptanceTestCase
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
- repeated  string testRunnerSettings = 0
+  testEnvEnum testEnv = 0
   queryTypeEnum queryType = 0
  repeated  precondition preconditions = 0
   trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
   testObjectiveEnum testCaseObjective = 0
   testSourceEnum testCaseSource = 0
   string testCasePredicateName = 0
   string testCasePredicateId = 0
   uriorcurie testCaseInputId = 0
- repeated  qualifier qualifiers = 0
-  conceptCategory inputCategory = 0
-  conceptCategory outputCategory = 0
- repeated  componentEnum components = 0
-  testEnvEnum testEnv = 0
+ repeated  string testCaseRunnerSettings = 0
  repeated  string tags = 0
  repeated  acceptanceTestAsset testAssets = 0
  }
 message AcceptanceTestSuite
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   testMetadata testMetadata = 0
   testPersonaEnum testPersona = 0
  repeated  testCase testCases = 0
   testSuiteSpecification testSuiteSpecification = 0
  }
+// TRAPI and Biolink Model standards compliance test
+message ComplianceTestCase
+ {
+  uriorcurie id = 0
+  string name = 0
+  string description = 0
+  testEnvEnum testEnv = 0
+  queryTypeEnum queryType = 0
+ repeated  testAsset testAssets = 0
+ repeated  precondition preconditions = 0
+  trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
+  testObjectiveEnum testCaseObjective = 0
+  testSourceEnum testCaseSource = 0
+  string testCasePredicateName = 0
+  string testCasePredicateId = 0
+  uriorcurie testCaseInputId = 0
+ repeated  string testCaseRunnerSettings = 0
+ repeated  string tags = 0
+  string trapiVersion = 0
+  string biolinkVersion = 0
+ }
+// Knowledge Graph navigation integration test
+message KnowledgeGraphNavigationTestCase
+ {
+  uriorcurie id = 0
+  string name = 0
+  string description = 0
+  testEnvEnum testEnv = 0
+  queryTypeEnum queryType = 0
+ repeated  testAsset testAssets = 0
+ repeated  precondition preconditions = 0
+  trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
+  testObjectiveEnum testCaseObjective = 0
+  testSourceEnum testCaseSource = 0
+  string testCasePredicateName = 0
+  string testCasePredicateId = 0
+  uriorcurie testCaseInputId = 0
+ repeated  string testCaseRunnerSettings = 0
+ repeated  string tags = 0
+ }
+// 'One Hop' Knowledge Graph navigation integration test
+message OneHopTestCase
+ {
+  uriorcurie id = 0
+  string name = 0
+  string description = 0
+  testEnvEnum testEnv = 0
+  queryTypeEnum queryType = 0
+ repeated  testAsset testAssets = 0
+ repeated  precondition preconditions = 0
+  trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
+  testObjectiveEnum testCaseObjective = 0
+  testSourceEnum testCaseSource = 0
+  string testCasePredicateName = 0
+  string testCasePredicateId = 0
+  uriorcurie testCaseInputId = 0
+ repeated  string testCaseRunnerSettings = 0
+ repeated  string tags = 0
+ }
 // Test case for testing the integrity of "One Hop" knowledge graph retrievals sensa legacy SRI_Testing harness.
 message OneHopTestSuite
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   testMetadata testMetadata = 0
   testPersonaEnum testPersona = 0
  repeated  testCase testCases = 0
   testSuiteSpecification testSuiteSpecification = 0
  }
 // Represents a precondition for a TestCase
 message Precondition
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
  }
 message Qualifier
  {
   string parameter = 0
   string value = 0
  }
 // Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete.
 message QuantitativeTestCase
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
- repeated  string testRunnerSettings = 0
+  testEnvEnum testEnv = 0
   queryTypeEnum queryType = 0
  repeated  testAsset testAssets = 0
  repeated  precondition preconditions = 0
   trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
   testObjectiveEnum testCaseObjective = 0
   testSourceEnum testCaseSource = 0
   string testCasePredicateName = 0
   string testCasePredicateId = 0
   uriorcurie testCaseInputId = 0
- repeated  qualifier qualifiers = 0
-  conceptCategory inputCategory = 0
-  conceptCategory outputCategory = 0
- repeated  componentEnum components = 0
-  testEnvEnum testEnv = 0
+ repeated  string testCaseRunnerSettings = 0
  repeated  string tags = 0
  }
 // Test suite for testing Translator components against releases of standards like TRAPI and the Biolink Model.
 message StandardsComplianceTestSuite
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   testMetadata testMetadata = 0
   testPersonaEnum testPersona = 0
  repeated  testCase testCases = 0
   testSuiteSpecification testSuiteSpecification = 0
  }
 // Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs.
 message TestAsset
@@ -149,50 +201,46 @@
  repeated  qualifier qualifiers = 0
   string expectedOutput = 0
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
+ repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
   uriorcurie id = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
  }
 // Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition.
 message TestCase
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
- repeated  string testRunnerSettings = 0
+  testEnvEnum testEnv = 0
   queryTypeEnum queryType = 0
  repeated  testAsset testAssets = 0
  repeated  precondition preconditions = 0
   trapiTemplateEnum trapiTemplate = 0
+ repeated  componentEnum components = 0
   testObjectiveEnum testCaseObjective = 0
   testSourceEnum testCaseSource = 0
   string testCasePredicateName = 0
   string testCasePredicateId = 0
   uriorcurie testCaseInputId = 0
- repeated  qualifier qualifiers = 0
-  conceptCategory inputCategory = 0
-  conceptCategory outputCategory = 0
- repeated  componentEnum components = 0
-  testEnvEnum testEnv = 0
+ repeated  string testCaseRunnerSettings = 0
  repeated  string tags = 0
  }
 // The outcome of a TestRunner run of one specific TestCase.
 message TestCaseResult
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   uriorcurie testSuiteId = 0
   testCase testCase = 0
   testCaseResultEnum testCaseResult = 0
  }
 // Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing.
 message TestEdgeData
  {
@@ -210,98 +258,98 @@
  repeated  qualifier qualifiers = 0
   string expectedOutput = 0
   testIssueEnum testIssue = 0
   semanticSeverityEnum semanticSeverity = 0
   boolean inV1 = 0
   boolean wellKnown = 0
   uriorcurie testReference = 0
+ repeated  string runnerSettings = 0
   testMetadata testMetadata = 0
   uriorcurie id = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
  }
 // A single 'tag = value' pair (where 'value' is a simple string).
 message TestEntityParameter
  {
   string parameter = 0
   string value = 0
  }
 // Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites.
 message TestMetadata
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   testSourceEnum testSource = 0
   uriorcurie testReference = 0
   testObjectiveEnum testObjective = 0
  repeated  testEntityParameter testAnnotations = 0
  }
 // The output of a TestRunner run of one specific TestCase.
 message TestOutput
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   string testCaseId = 0
  repeated  testResultPKSet pks = 0
  }
 // Primary keys for a given ARA result set from a SmokeTest result for a given TestCase.
 message TestResultPKSet
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   string parentPk = 0
   string mergedPk = 0
   string aragorn = 0
   string arax = 0
   string unsecret = 0
   string bte = 0
   string improving = 0
  }
-// Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite).
+// General configuration parameters and test data input  for a single invocation of a TestRunner.
+message TestRunnerConfiguration
+ {
+  uriorcurie id = 0
+  string name = 0
+  string description = 0
+ repeated  testEntityParameter testRunParameters = 0
+ repeated  string tags = 0
+ }
+// A single invocation of a TestRunner.
 message TestRunSession
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
- repeated  componentEnum components = 0
-  testEnvEnum testEnv = 0
   string testRunnerName = 0
- repeated  testEntityParameter testRunParameters = 0
  repeated  testEntity testEntities = 0
  repeated  testCaseResult testCaseResults = 0
   datetime timestamp = 0
  }
 // Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present.
 message TestSuite
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   testMetadata testMetadata = 0
   testPersonaEnum testPersona = 0
  repeated  testCase testCases = 0
   testSuiteSpecification testSuiteSpecification = 0
  }
 // Parameters for a Test Case instances either dynamically generated from some external source of Test Assets.
 message TestSuiteSpecification
  {
   uriorcurie id = 0
   string name = 0
   string description = 0
  repeated  string tags = 0
- repeated  string testRunnerSettings = 0
   uriorcurie testDataFileLocator = 0
   fileFormatEnum testDataFileFormat = 0
  }
```

### Comparing `translator_testing_model-0.3.1/project/shacl/translator_testing_model.shacl.ttl` & `translator_testing_model-2.3.0/project/shacl/translator_testing_model.shacl.ttl`

 * *Files 4% similar despite different names*

```diff
@@ -1,806 +1,1027 @@
-@prefix infores: <https://w3id.org/biolink/vocab/> .
 @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
 @prefix schema1: <http://schema.org/> .
 @prefix sh: <http://www.w3.org/ns/shacl#> .
 @prefix ttm: <https://w3id.org/TranslatorSRI/TranslatorTestingModel/> .
 @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
 
 ttm:AcceptanceTestCase a sh:NodeShape ;
     sh:closed true ;
     sh:description "See AcceptanceTestAsset above for more details." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:test_case_predicate_name ],
-        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
-            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:trapi_template ],
-        [ sh:class ttm:Precondition ;
+    sh:property [ sh:class ttm:Precondition ;
             sh:nodeKind sh:IRI ;
-            sh:order 2 ;
+            sh:order 3 ;
             sh:path ttm:preconditions ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
         [ sh:maxCount 1 ;
             sh:order 10 ;
-            sh:path ttm:input_category ],
-        [ sh:maxCount 1 ;
-            sh:order 8 ;
             sh:path ttm:test_case_input_id ],
-        [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 17 ;
-            sh:path schema1:additionalType ],
-        [ sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:output_category ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in ( infores:ncats-ars infores:arax infores:explanatory-agent infores:improving-agent infores:aragorn infores:biothings-explorer infores:unsecret-agent infores:rtx-kg2 infores:icees-kg infores:cam-kp infores:spoke infores:molepro infores:textmining-kp infores:cohd infores:openpredict infores:knowledge-collaboratory infores:connections-hypothesis ) ;
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 12 ;
-            sh:path ttm:components ],
+            sh:path schema1:identifier ],
         [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
             sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:test_case_source ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
             sh:order 7 ;
-            sh:path ttm:test_case_predicate_id ],
+            sh:path ttm:test_case_source ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 15 ;
+            sh:order 13 ;
             sh:path schema1:name ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
             sh:order 14 ;
-            sh:path schema1:identifier ],
+            sh:path schema1:description ],
         [ sh:class ttm:AcceptanceTestAsset ;
             sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 1 ;
+            sh:order 2 ;
             sh:path ttm:test_assets ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:test_env ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
         [ sh:description "Type of TestCase query." ;
             sh:in ( "treats" ) ;
             sh:maxCount 1 ;
-            sh:order 0 ;
+            sh:order 1 ;
             sh:path ttm:query_type ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 16 ;
-            sh:path schema1:description ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" "StandardsValidationTest" "OneHopTest" ) ;
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
-            sh:path ttm:test_case_objective ],
+            sh:path ttm:trapi_template ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 18 ;
-            sh:path ttm:test_runner_settings ] ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ] ;
     sh:targetClass ttm:AcceptanceTestCase .
 
 ttm:AcceptanceTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path ttm:test_metadata ],
+        [ sh:class ttm:TestSuiteSpecification ;
+            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:test_suite_specification ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 8 ;
-            sh:path ttm:test_runner_settings ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path schema1:description ],
-        [ sh:class ttm:TestSuiteSpecification ;
-            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
+        [ sh:class ttm:TestCase ;
+            sh:description "List of explicitly enumerated Test Cases." ;
             sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path ttm:test_metadata ],
+            sh:order 2 ;
+            sh:path ttm:test_cases ],
         [ sh:description "A Test persona describes the user or operational context of a given test." ;
             sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path ttm:test_persona ],
-        [ sh:class ttm:TestCase ;
-            sh:description "List of explicitly enumerated Test Cases." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_cases ] ;
+            sh:path ttm:test_persona ] ;
     sh:targetClass ttm:AcceptanceTestSuite .
 
 ttm:BenchmarkTestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "JsonObj(is_a='TestSuite')" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:targetClass ttm:BenchmarkTestSuite .
 
-ttm:OneHopTestSuite a sh:NodeShape ;
+ttm:ComplianceTestCase a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness." ;
+    sh:description "TRAPI and Biolink Model standards compliance test" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+    sh:property [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:maxCount 1 ;
+            sh:order 12 ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 6 ;
-            sh:path schema1:description ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:path ttm:trapi_template ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path ttm:test_metadata ],
+            sh:order 9 ;
+            sh:path ttm:test_case_source ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
-        [ sh:class ttm:TestSuiteSpecification ;
-            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
+            sh:order 16 ;
+            sh:path schema1:description ],
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
+            sh:order 4 ;
+            sh:path ttm:test_assets ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 7 ;
+            sh:path ttm:components ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 13 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
             sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
+            sh:path ttm:query_type ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 17 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "Biolink Model release (SemVer string)" ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:biolink_version ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 15 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_predicate_id ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:test_case_predicate_name ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 4 ;
+            sh:order 14 ;
             sh:path schema1:identifier ],
-        [ sh:description "A Test persona describes the user or operational context of a given test." ;
-            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
-            sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_persona ],
-        [ sh:class ttm:TestCase ;
-            sh:description "List of explicitly enumerated Test Cases." ;
+        [ sh:class ttm:Precondition ;
             sh:nodeKind sh:IRI ;
+            sh:order 5 ;
+            sh:path ttm:preconditions ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
             sh:order 2 ;
-            sh:path ttm:test_cases ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 8 ;
-            sh:path ttm:test_runner_settings ],
+            sh:path ttm:test_env ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "TRAPI version (SemVer string)" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ] ;
-    sh:targetClass ttm:OneHopTestSuite .
+            sh:order 0 ;
+            sh:path ttm:trapi_version ] ;
+    sh:targetClass ttm:ComplianceTestCase .
 
-ttm:QuantitativeTestCase a sh:NodeShape ;
+ttm:KnowledgeGraphNavigationTestCase a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete." ;
+    sh:description "Knowledge Graph navigation integration test" ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:description "Type of TestCase query." ;
-            sh:in ( "treats" ) ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:query_type ],
-        [ sh:class ttm:TestAsset ;
+    sh:property [ sh:class ttm:TestAsset ;
             sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 1 ;
+            sh:order 2 ;
             sh:path ttm:test_assets ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path schema1:name ],
+        [ sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
         [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
             sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
-            sh:order 3 ;
+            sh:order 4 ;
             sh:path ttm:trapi_template ],
-        [ sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:test_case_input_id ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 16 ;
+            sh:order 14 ;
             sh:path schema1:description ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 7 ;
+            sh:order 9 ;
             sh:path ttm:test_case_predicate_id ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in ( infores:ncats-ars infores:arax infores:explanatory-agent infores:improving-agent infores:aragorn infores:biothings-explorer infores:unsecret-agent infores:rtx-kg2 infores:icees-kg infores:cam-kp infores:spoke infores:molepro infores:textmining-kp infores:cohd infores:openpredict infores:knowledge-collaboratory infores:connections-hypothesis ) ;
-            sh:order 12 ;
-            sh:path ttm:components ],
         [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:test_case_predicate_name ],
-        [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:identifier ],
-        [ sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:output_category ],
-        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:order 12 ;
+            sh:path schema1:identifier ] ;
+    sh:targetClass ttm:KnowledgeGraphNavigationTestCase .
+
+ttm:OneHopTestCase a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "'One Hop' Knowledge Graph navigation integration test" ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:test_case_source ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 18 ;
-            sh:path ttm:test_runner_settings ],
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path ttm:trapi_template ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path schema1:name ],
+            sh:order 14 ;
+            sh:path schema1:description ],
         [ sh:maxCount 1 ;
             sh:order 10 ;
-            sh:path ttm:input_category ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 17 ;
-            sh:path schema1:additionalType ],
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
         [ sh:class ttm:Precondition ;
             sh:nodeKind sh:IRI ;
-            sh:order 2 ;
+            sh:order 3 ;
             sh:path ttm:preconditions ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" "StandardsValidationTest" "OneHopTest" ) ;
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:test_case_objective ],
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path schema1:name ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
         [ sh:description "Deployment environment within which the associated TestSuite is run." ;
             sh:in ( "dev" "ci" "test" "prod" ) ;
             sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:test_env ] ;
-    sh:targetClass ttm:QuantitativeTestCase .
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 12 ;
+            sh:path schema1:identifier ] ;
+    sh:targetClass ttm:OneHopTestCase .
 
-ttm:StandardsComplianceTestSuite a sh:NodeShape ;
+ttm:OneHopTestSuite a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Test suite for testing Translator components against releases of standards like TRAPI and the Biolink Model." ;
+    sh:description "Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 4 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 8 ;
-            sh:path ttm:test_runner_settings ],
         [ sh:class ttm:TestMetadata ;
             sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 0 ;
             sh:path ttm:test_metadata ],
-        [ sh:class ttm:TestCase ;
-            sh:description "List of explicitly enumerated Test Cases." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_cases ],
         [ sh:description "A Test persona describes the user or operational context of a given test." ;
             sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:test_persona ],
         [ sh:class ttm:TestSuiteSpecification ;
             sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
             sh:path ttm:test_suite_specification ],
+        [ sh:class ttm:TestCase ;
+            sh:description "List of explicitly enumerated Test Cases." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_cases ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:description ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:name ] ;
-    sh:targetClass ttm:StandardsComplianceTestSuite .
+    sh:targetClass ttm:OneHopTestSuite .
 
-ttm:TestEdgeData a sh:NodeShape ;
+ttm:QuantitativeTestCase a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing." ;
+    sh:description "Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
+    sh:property [ sh:description "Type of TestCase query." ;
+            sh:in ( "treats" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:query_type ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:predicate_name ],
+            sh:order 8 ;
+            sh:path ttm:test_case_predicate_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 19 ;
+            sh:order 14 ;
             sh:path schema1:description ],
-        [ sh:datatype xsd:boolean ;
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:in_v1 ],
+            sh:order 4 ;
+            sh:path ttm:trapi_template ],
         [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 20 ;
-            sh:path schema1:additionalType ],
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
         [ sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:output_id ],
+            sh:order 10 ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 17 ;
+            sh:order 12 ;
             sh:path schema1:identifier ],
-        [ sh:maxCount 1 ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path schema1:name ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ],
+        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
             sh:order 2 ;
-            sh:path ttm:input_category ],
+            sh:path ttm:test_assets ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ] ;
+    sh:targetClass ttm:QuantitativeTestCase .
+
+ttm:StandardsComplianceTestSuite a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Test suite for testing Translator components against releases of standards like TRAPI and the Biolink Model." ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:description "A Test persona describes the user or operational context of a given test." ;
+            sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:test_persona ],
         [ sh:class ttm:TestMetadata ;
             sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 16 ;
+            sh:order 0 ;
             sh:path ttm:test_metadata ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 18 ;
+            sh:order 5 ;
             sh:path schema1:name ],
+        [ sh:class ttm:TestSuiteSpecification ;
+            sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
+            sh:maxCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:test_suite_specification ],
+        [ sh:class ttm:TestCase ;
+            sh:description "List of explicitly enumerated Test Cases." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_cases ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:description ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ] ;
+    sh:targetClass ttm:StandardsComplianceTestSuite .
+
+ttm:TestEdgeData a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing." ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 20 ;
+            sh:path schema1:description ],
         [ sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:input_id ],
+            sh:order 3 ;
+            sh:path ttm:predicate_id ],
+        [ sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:output_category ],
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+            sh:maxCount 1 ;
+            sh:order 12 ;
+            sh:path ttm:semantic_severity ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 18 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar settings for the TestRunner, e.g. \"inferred\"" ;
-            sh:order 21 ;
-            sh:path ttm:test_runner_settings ],
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 19 ;
+            sh:path schema1:name ],
         [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:association ],
-        [ sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:output_category ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path ttm:output_name ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
             sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_issue ],
-        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+            sh:order 15 ;
+            sh:path ttm:test_reference ],
+        [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:semantic_severity ],
+            sh:order 13 ;
+            sh:path ttm:in_v1 ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
+            sh:order 21 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:input_name ],
+        [ sh:class ttm:Qualifier ;
+            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 9 ;
+            sh:path ttm:qualifiers ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:expected_output ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+            sh:maxCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_issue ],
+        [ sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path ttm:output_id ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path ttm:predicate_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
+            sh:minCount 1 ;
+            sh:order 16 ;
+            sh:path ttm:runner_settings ],
+        [ sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:input_id ],
         [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
             sh:order 14 ;
             sh:path ttm:well_known ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
-            sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path ttm:test_reference ],
-        [ sh:datatype xsd:string ;
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:expected_output ],
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 17 ;
+            sh:path ttm:test_metadata ],
         [ sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:predicate_id ] ;
+            sh:order 2 ;
+            sh:path ttm:input_category ] ;
     sh:targetClass ttm:TestEdgeData .
 
 ttm:TestOutput a sh:NodeShape ;
     sh:closed true ;
     sh:description "The output of a TestRunner run of one specific TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
             sh:description "CURIE id of a TestCase registered in the system." ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_case_id ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 6 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:name ],
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 5 ;
+            sh:path schema1:additionalType ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 5 ;
-            sh:path schema1:additionalType ],
+        [ sh:class ttm:TestResultPKSet ;
+            sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 1 ;
+            sh:path ttm:pks ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path schema1:description ],
-        [ sh:class ttm:TestResultPKSet ;
-            sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path ttm:pks ] ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:name ] ;
     sh:targetClass ttm:TestOutput .
 
 ttm:TestRunSession a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite)." ;
+    sh:description "A single invocation of a TestRunner." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 10 ;
-            sh:path schema1:additionalType ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in ( infores:ncats-ars infores:arax infores:explanatory-agent infores:improving-agent infores:aragorn infores:biothings-explorer infores:unsecret-agent infores:rtx-kg2 infores:icees-kg infores:cam-kp infores:spoke infores:molepro infores:textmining-kp infores:cohd infores:openpredict infores:knowledge-collaboratory infores:connections-hypothesis ) ;
-            sh:order 0 ;
-            sh:path ttm:components ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path schema1:description ],
+    sh:property [ sh:class ttm:TestCaseResult ;
+            sh:description "One or more instances of TestCaseResult." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_case_results ],
         [ sh:datatype xsd:dateTime ;
             sh:description "Date time when a given entity was created." ;
             sh:maxCount 1 ;
-            sh:order 6 ;
+            sh:order 3 ;
             sh:path ttm:timestamp ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "Global system name of a TestRunner." ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_env ],
-        [ sh:class ttm:TestEntityParameter ;
-            sh:description "Different TestRunners could expect additional global test configuration parameters, like the applicable TRAPI version (\"trapi_version\") or Biolink Model versions (\"biolink_version\")." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 3 ;
-            sh:path ttm:test_run_parameters ],
+            sh:order 0 ;
+            sh:path ttm:test_runner_name ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path schema1:description ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
-            sh:order 7 ;
+            sh:order 4 ;
             sh:path schema1:identifier ],
-        [ sh:class ttm:TestCaseResult ;
-            sh:description "One or more instances of TestCaseResult." ;
+        [ sh:class ttm:TestEntity ;
+            sh:description "Different TestRunners may expect specific kinds of TestEntity as input. These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite." ;
             sh:nodeKind sh:IRI ;
-            sh:order 5 ;
-            sh:path ttm:test_case_results ],
+            sh:order 1 ;
+            sh:path ttm:test_entities ],
         [ sh:datatype xsd:string ;
-            sh:description "Global system name of a TestRunner." ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:test_runner_name ],
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 11 ;
-            sh:path ttm:test_runner_settings ],
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path schema1:name ] ;
+    sh:targetClass ttm:TestRunSession .
+
+ttm:TestRunnerConfiguration a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "General configuration parameters and test data input  for a single invocation of a TestRunner." ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration." ;
+            sh:order 4 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 8 ;
+            sh:order 2 ;
             sh:path schema1:name ],
-        [ sh:class ttm:TestEntity ;
-            sh:description "Different TestRunners could expect specific kinds of TestEntity as an input.  These 'test_entities' are one or more instances of TestAsset, TestCase or (preferably?) TestSuite." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 4 ;
-            sh:path ttm:test_entities ] ;
-    sh:targetClass ttm:TestRunSession .
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 1 ;
+            sh:path schema1:identifier ],
+        [ sh:class ttm:TestEntityParameter ;
+            sh:description "Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 0 ;
+            sh:path ttm:test_run_parameters ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:description ] ;
+    sh:targetClass ttm:TestRunnerConfiguration .
 
 ttm:TestSuite a sh:NodeShape ;
     sh:closed true ;
     sh:description "Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path schema1:description ],
+            sh:order 5 ;
+            sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 7 ;
             sh:path schema1:additionalType ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 0 ;
-            sh:path ttm:test_metadata ],
-        [ sh:class ttm:TestCase ;
-            sh:description "List of explicitly enumerated Test Cases." ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:test_cases ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 8 ;
-            sh:path ttm:test_runner_settings ],
+            sh:order 6 ;
+            sh:path schema1:description ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:description "A Test persona describes the user or operational context of a given test." ;
             sh:in ( "All" "Clinical" "LookUp" "Mechanistic" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:test_persona ],
+        [ sh:class ttm:TestCase ;
+            sh:description "List of explicitly enumerated Test Cases." ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_cases ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 0 ;
+            sh:path ttm:test_metadata ],
         [ sh:class ttm:TestSuiteSpecification ;
             sh:description "Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 3 ;
-            sh:path ttm:test_suite_specification ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ] ;
+            sh:path ttm:test_suite_specification ] ;
     sh:targetClass ttm:TestSuite .
 
 ttm:AcceptanceTestAsset a sh:NodeShape ;
     sh:closed true ;
     sh:description "Model derived from Jenn's test asset design and Shervin's runner JSON here as an example." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:input_id ],
+    sh:property [ sh:class ttm:Qualifier ;
+            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 19 ;
+            sh:path ttm:qualifiers ],
+        [ sh:description "The deployment environment within which this test must pass." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:must_pass_environment ],
         [ sh:description "The direction of the expected query result triple" ;
             sh:in ( "increased" "decreased" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
             sh:path ttm:direction ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+            sh:maxCount 1 ;
+            sh:order 21 ;
+            sh:path ttm:test_issue ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 11 ;
             sh:path ttm:input_name ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
+            sh:minCount 1 ;
+            sh:order 26 ;
+            sh:path ttm:runner_settings ],
+        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 25 ;
-            sh:path ttm:test_reference ],
+            sh:minCount 1 ;
+            sh:order 28 ;
+            sh:path schema1:identifier ],
         [ sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:input_category ],
-        [ sh:datatype xsd:string ;
+            sh:order 17 ;
+            sh:path ttm:output_category ],
+        [ sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:input_id ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
-            sh:order 16 ;
-            sh:path ttm:output_name ],
+            sh:minCount 1 ;
+            sh:nodeKind sh:IRI ;
+            sh:order 27 ;
+            sh:path ttm:test_metadata ],
         [ sh:datatype xsd:boolean ;
             sh:maxCount 1 ;
             sh:order 23 ;
             sh:path ttm:in_v1 ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
-            sh:maxCount 1 ;
-            sh:order 21 ;
-            sh:path ttm:test_issue ],
-        [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 19 ;
-            sh:path ttm:qualifiers ],
-        [ sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:predicate_id ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar settings for the TestRunner, e.g. \"inferred\"" ;
-            sh:order 31 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 20 ;
-            sh:path ttm:expected_output ],
         [ sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path ttm:output_id ],
-        [ sh:description "The expected result of the query" ;
-            sh:in ( "include_good" "exclude_bad" ) ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:expected_result ],
+            sh:order 12 ;
+            sh:path ttm:input_category ],
         [ sh:datatype xsd:integer ;
             sh:description "The answer must return in these many results" ;
             sh:maxCount 1 ;
             sh:order 7 ;
             sh:path ttm:top_level ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 27 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 30 ;
-            sh:path schema1:additionalType ],
-        [ sh:datatype xsd:string ;
-            sh:description "The full human-readable scientific question a SME would ask, which is encoded into the test asset." ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:scientific_question ],
+        [ sh:maxCount 1 ;
+            sh:order 15 ;
+            sh:path ttm:output_id ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 14 ;
             sh:path ttm:predicate_name ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
             sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 26 ;
-            sh:path ttm:test_metadata ],
+            sh:order 22 ;
+            sh:path ttm:semantic_severity ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
+            sh:order 31 ;
+            sh:path schema1:additionalType ],
+        [ sh:description "The expected result of the query" ;
+            sh:in ( "include_good" "exclude_bad" ) ;
             sh:maxCount 1 ;
-            sh:order 28 ;
-            sh:path schema1:name ],
+            sh:order 6 ;
+            sh:path ttm:expected_result ],
         [ sh:datatype xsd:string ;
             sh:description "An answer that is returned from the test case, note: this must be combined with the expected_result to form a complete answer.  It might make sense to couple these in their own object instead of strictly sticking to the flat schema introduced by the spreadsheet here: https://docs.google.com/spreadsheets/d/1yj7zIchFeVl1OHqL_kE_pqvzNLmGml_FLbHDs-8Yvig/edit#gid=0" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path ttm:answer_informal_concept ],
-        [ sh:maxCount 1 ;
-            sh:order 17 ;
-            sh:path ttm:output_category ],
-        [ sh:datatype xsd:string ;
-            sh:description "The notes of the query" ;
-            sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path ttm:notes ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 29 ;
+            sh:order 30 ;
             sh:path schema1:description ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 24 ;
-            sh:path ttm:well_known ],
-        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 18 ;
-            sh:path ttm:association ],
+            sh:order 20 ;
+            sh:path ttm:expected_output ],
         [ sh:description "The node of the (templated) TRAPI query to replace" ;
             sh:in ( "subject" "object" ) ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path ttm:query_node ],
         [ sh:datatype xsd:string ;
             sh:description "The object of the core triple to be tested" ;
             sh:maxCount 1 ;
             sh:order 3 ;
             sh:path ttm:string_entry ],
-        [ sh:description "The deployment environment within which this test must pass." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
+        [ sh:datatype xsd:string ;
+            sh:description "The full human-readable scientific question a SME would ask, which is encoded into the test asset." ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:must_pass_environment ],
-        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+            sh:order 2 ;
+            sh:path ttm:scientific_question ],
+        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
             sh:maxCount 1 ;
-            sh:order 22 ;
-            sh:path ttm:semantic_severity ],
+            sh:order 25 ;
+            sh:path ttm:test_reference ],
         [ sh:datatype xsd:date ;
             sh:description "The date by which this test must pass" ;
             sh:maxCount 1 ;
             sh:order 0 ;
-            sh:path ttm:must_pass_date ] ;
+            sh:path ttm:must_pass_date ],
+        [ sh:datatype xsd:string ;
+            sh:description "The notes of the query" ;
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path ttm:notes ],
+        [ sh:datatype xsd:boolean ;
+            sh:maxCount 1 ;
+            sh:order 24 ;
+            sh:path ttm:well_known ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 29 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 16 ;
+            sh:path ttm:output_name ],
+        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
+            sh:maxCount 1 ;
+            sh:order 18 ;
+            sh:path ttm:association ],
+        [ sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path ttm:predicate_id ] ;
     sh:targetClass ttm:AcceptanceTestAsset .
 
 ttm:TestCaseResult a sh:NodeShape ;
     sh:closed true ;
     sh:description "The outcome of a TestRunner run of one specific TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 7 ;
-            sh:path ttm:test_runner_settings ],
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:name ],
         [ sh:description "Encoded result of a single test run of a given test case" ;
-            sh:in ( "PASSED" "FAILED" "SKIPPED" ) ;
+            sh:in ( "test_passed" "test_failed" "test_skipped" ) ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path ttm:test_case_result ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:name ],
+            sh:order 5 ;
+            sh:path schema1:description ],
+        [ sh:description "CURIE id of a TestSuite registered in the system." ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_suite_id ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 6 ;
             sh:path schema1:additionalType ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path schema1:description ],
         [ sh:class ttm:TestCase ;
             sh:description "Slot referencing a single TestCase." ;
             sh:maxCount 1 ;
             sh:nodeKind sh:IRI ;
             sh:order 1 ;
             sh:path ttm:test_case ],
         [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 3 ;
-            sh:path schema1:identifier ],
-        [ sh:description "CURIE id of a TestSuite registered in the system." ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_suite_id ] ;
+            sh:path schema1:identifier ] ;
     sh:targetClass ttm:TestCaseResult .
 
 ttm:TestEntity a sh:NodeShape ;
     sh:closed false ;
     sh:description "Abstract global 'identification' class shared as a parent with all major model classes within the data model for Translator testing." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 4 ;
-            sh:path ttm:test_runner_settings ],
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path schema1:name ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path schema1:description ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
@@ -808,161 +1029,62 @@
             sh:path schema1:additionalType ] ;
     sh:targetClass ttm:TestEntity .
 
 ttm:TestResultPKSet a sh:NodeShape ;
     sh:closed true ;
     sh:description "Primary keys for a given ARA result set from a SmokeTest result for a given TestCase." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:merged_pk ],
+            sh:minCount 1 ;
+            sh:order 7 ;
+            sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 9 ;
-            sh:path schema1:description ],
+            sh:order 0 ;
+            sh:path ttm:parent_pk ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 10 ;
             sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:arax ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 6 ;
-            sh:path ttm:improving ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:parent_pk ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path ttm:aragorn ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 7 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 11 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:unsecret ],
-        [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 8 ;
             sh:path schema1:name ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:bte ] ;
-    sh:targetClass ttm:TestResultPKSet .
-
-ttm:TestAsset a sh:NodeShape ;
-    sh:closed true ;
-    sh:description "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
-    sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 18 ;
-            sh:path schema1:name ],
-        [ sh:class ttm:TestMetadata ;
-            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
-            sh:maxCount 1 ;
-            sh:nodeKind sh:IRI ;
-            sh:order 16 ;
-            sh:path ttm:test_metadata ],
-        [ sh:maxCount 1 ;
             sh:order 2 ;
-            sh:path ttm:input_category ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
-            sh:maxCount 1 ;
-            sh:order 15 ;
-            sh:path ttm:test_reference ],
-        [ sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:input_id ],
-        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
-            sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:test_issue ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
-            sh:order 20 ;
-            sh:path schema1:additionalType ],
-        [ sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:output_id ],
+            sh:path ttm:aragorn ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 6 ;
-            sh:path ttm:output_name ],
-        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
-            sh:maxCount 1 ;
-            sh:order 8 ;
-            sh:path ttm:association ],
-        [ sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:predicate_id ],
+            sh:path ttm:improving ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 19 ;
-            sh:path schema1:description ],
+            sh:order 3 ;
+            sh:path ttm:arax ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar settings for the TestRunner, e.g. \"inferred\"" ;
-            sh:order 21 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 17 ;
-            sh:path schema1:identifier ],
-        [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
+            sh:order 1 ;
+            sh:path ttm:merged_pk ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path ttm:predicate_name ],
-        [ sh:in ( "High" "Low" "NotApplicable" ) ;
-            sh:maxCount 1 ;
-            sh:order 12 ;
-            sh:path ttm:semantic_severity ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:in_v1 ],
+            sh:order 5 ;
+            sh:path ttm:bte ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:input_name ],
-        [ sh:datatype xsd:boolean ;
-            sh:maxCount 1 ;
-            sh:order 14 ;
-            sh:path ttm:well_known ],
-        [ sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:output_category ],
+            sh:order 9 ;
+            sh:path schema1:description ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 10 ;
-            sh:path ttm:expected_output ] ;
-    sh:targetClass ttm:TestAsset .
+            sh:order 4 ;
+            sh:path ttm:unsecret ] ;
+    sh:targetClass ttm:TestResultPKSet .
 
 ttm:TestEntityParameter a sh:NodeShape ;
     sh:closed true ;
     sh:description "A single 'tag = value' pair (where 'value' is a simple string)." ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
             sh:description "(String) value of a TestParameter." ;
@@ -972,227 +1094,302 @@
         [ sh:datatype xsd:string ;
             sh:description "Name of a TestParameter." ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:parameter ] ;
     sh:targetClass ttm:TestEntityParameter .
 
-ttm:Precondition a sh:NodeShape ;
+ttm:Qualifier a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Represents a precondition for a TestCase" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 4 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
+            sh:description "The 'value' of should be a suitable value generally drawn from an applicable Biolink Model (\"Enum\") value set of the specified Qualifier." ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path schema1:name ],
+            sh:path ttm:value ],
         [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 2 ;
-            sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:description "The 'parameter' of a Qualifier should be a `qualifier` slot name from the Biolink Model ('biolink' namespace) 'biolink:qualifier' hierarchy." ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
             sh:order 0 ;
-            sh:path schema1:identifier ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 3 ;
-            sh:path schema1:additionalType ] ;
-    sh:targetClass ttm:Precondition .
+            sh:path ttm:parameter ] ;
+    sh:targetClass ttm:Qualifier .
 
 ttm:TestSuiteSpecification a sh:NodeShape ;
     sh:closed true ;
     sh:description "Parameters for a Test Case instances either dynamically generated from some external source of Test Assets." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable name for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path schema1:name ],
-        [ sh:datatype xsd:string ;
-            sh:description "A human-readable description for a Test Entity" ;
-            sh:maxCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:description ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
             sh:minCount 1 ;
             sh:order 2 ;
             sh:path schema1:identifier ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
             sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
             sh:order 5 ;
             sh:path schema1:additionalType ],
-        [ sh:description "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)" ;
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:test_data_file_locator ],
+            sh:order 4 ;
+            sh:path schema1:description ],
         [ sh:description "File format of test entity data (e.g. TSV, YAML or JSON)" ;
             sh:in ( "TSV" "YAML" "JSON" ) ;
             sh:maxCount 1 ;
             sh:order 1 ;
             sh:path ttm:test_data_file_format ],
-        [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 6 ;
-            sh:path ttm:test_runner_settings ] ;
+        [ sh:description "An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)" ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_data_file_locator ] ;
     sh:targetClass ttm:TestSuiteSpecification .
 
-ttm:TestCase a sh:NodeShape ;
+ttm:TestAsset a sh:NodeShape ;
     sh:closed true ;
-    sh:description "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition." ;
+    sh:description "Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:class ttm:Qualifier ;
-            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 9 ;
-            sh:path ttm:qualifiers ],
+    sh:property [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+            sh:maxCount 1 ;
+            sh:order 15 ;
+            sh:path ttm:test_reference ],
+        [ sh:maxCount 1 ;
+            sh:order 2 ;
+            sh:path ttm:input_category ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 16 ;
+            sh:order 20 ;
             sh:path schema1:description ],
-        [ sh:class ttm:Precondition ;
-            sh:nodeKind sh:IRI ;
-            sh:order 2 ;
-            sh:path ttm:preconditions ],
-        [ sh:datatype xsd:string ;
-            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
-            sh:order 17 ;
-            sh:path schema1:additionalType ],
+        [ sh:in ( "High" "Low" "NotApplicable" ) ;
+            sh:maxCount 1 ;
+            sh:order 12 ;
+            sh:path ttm:semantic_severity ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
+            sh:maxCount 1 ;
+            sh:order 4 ;
+            sh:path ttm:predicate_name ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
             sh:order 18 ;
-            sh:path ttm:test_runner_settings ],
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable name for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:order 19 ;
+            sh:path schema1:name ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 1 ;
+            sh:path ttm:input_name ],
         [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
             sh:order 6 ;
-            sh:path ttm:test_case_predicate_name ],
-        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
-            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:path ttm:output_name ],
+        [ sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:output_category ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 10 ;
+            sh:path ttm:expected_output ],
+        [ sh:datatype xsd:boolean ;
+            sh:maxCount 1 ;
+            sh:order 13 ;
+            sh:path ttm:in_v1 ],
+        [ sh:datatype xsd:boolean ;
+            sh:maxCount 1 ;
+            sh:order 14 ;
+            sh:path ttm:well_known ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness, e.g. \"inferred\"" ;
+            sh:minCount 1 ;
+            sh:order 16 ;
+            sh:path ttm:runner_settings ],
+        [ sh:description "Specific Biolink Model association 'category' which applies to the test asset defined knowledge statement" ;
+            sh:maxCount 1 ;
+            sh:order 8 ;
+            sh:path ttm:association ],
+        [ sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:input_id ],
+        [ sh:class ttm:Qualifier ;
+            sh:description "Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 9 ;
+            sh:path ttm:qualifiers ],
+        [ sh:class ttm:TestMetadata ;
+            sh:description "Test metadata describes the external provenance, cross-references and objectives for a given test." ;
             sh:maxCount 1 ;
-            sh:order 5 ;
-            sh:path ttm:test_case_source ],
-        [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
-            sh:in ( infores:ncats-ars infores:arax infores:explanatory-agent infores:improving-agent infores:aragorn infores:biothings-explorer infores:unsecret-agent infores:rtx-kg2 infores:icees-kg infores:cam-kp infores:spoke infores:molepro infores:textmining-kp infores:cohd infores:openpredict infores:knowledge-collaboratory infores:connections-hypothesis ) ;
-            sh:order 12 ;
-            sh:path ttm:components ],
-        [ sh:class ttm:TestAsset ;
-            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
             sh:nodeKind sh:IRI ;
-            sh:order 1 ;
-            sh:path ttm:test_assets ],
+            sh:order 17 ;
+            sh:path ttm:test_metadata ],
+        [ sh:maxCount 1 ;
+            sh:order 3 ;
+            sh:path ttm:predicate_id ],
+        [ sh:maxCount 1 ;
+            sh:order 5 ;
+            sh:path ttm:output_id ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection" ;
+            sh:order 21 ;
+            sh:path schema1:additionalType ],
+        [ sh:in ( "causes not treats" "TMKP" "category too generic" "contraindications" "chemical roles" "test_issue" ) ;
+            sh:maxCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_issue ] ;
+    sh:targetClass ttm:TestAsset .
+
+ttm:TestCase a sh:NodeShape ;
+    sh:closed true ;
+    sh:description "Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition." ;
+    sh:ignoredProperties ( rdf:type ) ;
+    sh:property [ sh:description "The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX." ;
+            sh:in [ rdf:rest () ] ;
+            sh:order 5 ;
+            sh:path ttm:components ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 15 ;
+            sh:order 13 ;
             sh:path schema1:name ],
-        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
-            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
+        [ sh:datatype xsd:string ;
             sh:maxCount 1 ;
-            sh:order 3 ;
-            sh:path ttm:trapi_template ],
-        [ sh:maxCount 1 ;
-            sh:order 11 ;
-            sh:path ttm:output_category ],
-        [ sh:maxCount 1 ;
             sh:order 8 ;
-            sh:path ttm:test_case_input_id ],
+            sh:path ttm:test_case_predicate_name ],
         [ sh:datatype xsd:string ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 7 ;
-            sh:path ttm:test_case_predicate_id ],
+            sh:order 14 ;
+            sh:path schema1:description ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 12 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "Settings for the test harness for TestCase" ;
+            sh:minCount 1 ;
+            sh:order 11 ;
+            sh:path ttm:test_case_runner_settings ],
+        [ sh:datatype xsd:string ;
+            sh:description "One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection." ;
+            sh:order 15 ;
+            sh:path schema1:additionalType ],
+        [ sh:class ttm:Precondition ;
+            sh:nodeKind sh:IRI ;
+            sh:order 3 ;
+            sh:path ttm:preconditions ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
+            sh:maxCount 1 ;
+            sh:order 6 ;
+            sh:path ttm:test_case_objective ],
         [ sh:maxCount 1 ;
             sh:order 10 ;
-            sh:path ttm:input_category ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" "StandardsValidationTest" "OneHopTest" ) ;
+            sh:path ttm:test_case_input_id ],
+        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
+            sh:in ( "dev" "ci" "test" "prod" ) ;
+            sh:maxCount 1 ;
+            sh:order 0 ;
+            sh:path ttm:test_env ],
+        [ sh:description "A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory." ;
+            sh:in ( "ameliorates" "treats" "three_hop" "drug_treats_rare_disease" "drug-to-gene" ) ;
             sh:maxCount 1 ;
             sh:order 4 ;
-            sh:path ttm:test_case_objective ],
+            sh:path ttm:trapi_template ],
+        [ sh:datatype xsd:string ;
+            sh:maxCount 1 ;
+            sh:order 9 ;
+            sh:path ttm:test_case_predicate_id ],
         [ sh:description "Type of TestCase query." ;
             sh:in ( "treats" ) ;
             sh:maxCount 1 ;
-            sh:order 0 ;
+            sh:order 1 ;
             sh:path ttm:query_type ],
-        [ sh:description "Deployment environment within which the associated TestSuite is run." ;
-            sh:in ( "dev" "ci" "test" "prod" ) ;
-            sh:maxCount 1 ;
-            sh:order 13 ;
-            sh:path ttm:test_env ],
-        [ sh:description "A unique identifier for a Test Entity" ;
-            sh:maxCount 1 ;
+        [ sh:class ttm:TestAsset ;
+            sh:description "One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection." ;
             sh:minCount 1 ;
-            sh:order 14 ;
-            sh:path schema1:identifier ] ;
+            sh:nodeKind sh:IRI ;
+            sh:order 2 ;
+            sh:path ttm:test_assets ],
+        [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
+            sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
+            sh:maxCount 1 ;
+            sh:order 7 ;
+            sh:path ttm:test_case_source ] ;
     sh:targetClass ttm:TestCase .
 
-ttm:Qualifier a sh:NodeShape ;
+ttm:Precondition a sh:NodeShape ;
     sh:closed true ;
+    sh:description "Represents a precondition for a TestCase" ;
     sh:ignoredProperties ( rdf:type ) ;
     sh:property [ sh:datatype xsd:string ;
-            sh:description "The 'parameter' of a Qualifier should be a `qualifier` slot name from the Biolink Model ('biolink' namespace) 'biolink:qualifier' hierarchy." ;
+            sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 0 ;
-            sh:path ttm:parameter ],
+            sh:order 2 ;
+            sh:path schema1:description ],
         [ sh:datatype xsd:string ;
-            sh:description "The 'value' of should be a suitable value generally drawn from an applicable Biolink Model (\"Enum\") value set of the specified Qualifier." ;
+            sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 1 ;
-            sh:path ttm:value ] ;
-    sh:targetClass ttm:Qualifier .
+            sh:path schema1:name ],
+        [ sh:description "A unique identifier for a Test Entity" ;
+            sh:maxCount 1 ;
+            sh:minCount 1 ;
+            sh:order 0 ;
+            sh:path schema1:identifier ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 3 ;
+            sh:path schema1:additionalType ] ;
+    sh:targetClass ttm:Precondition .
 
 ttm:TestMetadata a sh:NodeShape ;
     sh:closed true ;
     sh:description "Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites." ;
     sh:ignoredProperties ( rdf:type ) ;
-    sh:property [ sh:datatype xsd:string ;
-            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
-            sh:order 7 ;
-            sh:path schema1:additionalType ],
-        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
+    sh:property [ sh:description "A unique identifier for a Test Entity" ;
             sh:maxCount 1 ;
-            sh:order 1 ;
-            sh:path ttm:test_reference ],
+            sh:minCount 1 ;
+            sh:order 4 ;
+            sh:path schema1:identifier ],
         [ sh:description "Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string." ;
             sh:in ( "SME" "SMURF" "GitHubUserFeedback" "TACT" "BenchMark" "TranslatorTeam" "TestDataLocation" ) ;
             sh:maxCount 1 ;
             sh:order 0 ;
             sh:path ttm:test_source ],
-        [ sh:class ttm:TestEntityParameter ;
-            sh:description "Metadata annotation." ;
-            sh:nodeKind sh:BlankNodeOrIRI ;
-            sh:order 3 ;
-            sh:path ttm:test_annotations ],
-        [ sh:description "A unique identifier for a Test Entity" ;
+        [ sh:description "Document URL where original test source particulars are registered (e.g. Github repo)" ;
             sh:maxCount 1 ;
-            sh:minCount 1 ;
-            sh:order 4 ;
-            sh:path schema1:identifier ],
+            sh:order 1 ;
+            sh:path ttm:test_reference ],
+        [ sh:datatype xsd:string ;
+            sh:description "A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists." ;
+            sh:order 7 ;
+            sh:path schema1:additionalType ],
         [ sh:datatype xsd:string ;
             sh:description "A human-readable description for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 6 ;
             sh:path schema1:description ],
-        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)" ;
-            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" "StandardsValidationTest" "OneHopTest" ) ;
+        [ sh:class ttm:TestEntityParameter ;
+            sh:description "Metadata annotation." ;
+            sh:nodeKind sh:BlankNode ;
+            sh:order 3 ;
+            sh:path ttm:test_annotations ],
+        [ sh:description "Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)" ;
+            sh:in ( "AcceptanceTest" "BenchmarkTest" "QuantitativeTest" ) ;
             sh:maxCount 1 ;
             sh:order 2 ;
             sh:path ttm:test_objective ],
         [ sh:datatype xsd:string ;
-            sh:description "Scalar parameters for the TestRunner processing a given TestEntity." ;
-            sh:order 8 ;
-            sh:path ttm:test_runner_settings ],
-        [ sh:datatype xsd:string ;
             sh:description "A human-readable name for a Test Entity" ;
             sh:maxCount 1 ;
             sh:order 5 ;
             sh:path schema1:name ] ;
     sh:targetClass ttm:TestMetadata .
```

### Comparing `translator_testing_model-0.3.1/pyproject.toml` & `translator_testing_model-2.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 [tool.poetry]
 name = "translator_testing_model"
-version = "0.3.1"
+version = "2.3.0"
 description = "This is the project description."
 authors = ["Sierra Moxon <sierra.taylor@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "README.md",
     "src/data/examples",
     "src/translator_testing_model/schema",
     "src/translator_testing_model/datamodel",
     "project"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-linkml-runtime = "^1.7.5"
-linkml = "^1.7.8"
+linkml-runtime = "^1.6.1"
+linkml = "^1.6.1"
 pandas = "^2.1.2"
-pydantic = "^2"
-bmt = "^1.4.0"
-bioregistry = "^0.11.1"
+pydantic = "^1.10.13"
+bmt = "^1.2.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Bad-AcceptanceTestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-AcceptanceTestAsset-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/data/examples/Bad-TestEntity-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-001.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #      all major model classes within the data model for Translator testing.
 #    abstract: true
 #    tree_root: true
 #    slots:
 #      - id
 #      - name
 #      - description
-#      - tags
-#      - test_runner_settings
 #
 # where the slots are:
 #
 #  id:
 #    identifier: true
 #    slot_uri: schema:identifier
 #    range: uriorcurie
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestEntity-002.yaml-uriorcurie_should_fail_but_does_not`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #      all major model classes within the data model for Translator testing.
 #    abstract: true
 #    tree_root: true
 #    slots:
 #      - id
 #      - name
 #      - description
-#      - tags
-#      - test_runner_settings
 #
 # where the slots are:
 #
 #  id:
 #    identifier: true
 #    slot_uri: schema:identifier
 #    range: uriorcurie
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Bad-TestMetadata-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestMetadata-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/data/examples/Bad-TestSuite-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Bad-TestSuite-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-AcceptanceTestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestAsset-001.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 input_id: MONDO:0011426
 predicate_name: treats
 output_id: DRUGBANK:DB01592
 expected_output: NeverShow
 test_metadata:
   id: "test:1"
   test_source: SMURF
-test_runner_settings:
+runner_settings:
   - "inferred"
   - "test"
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-AcceptanceTestCase-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-AcceptanceTestCase-001.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 #    slot_usage:
 #      test_assets:
 #        range: AcceptanceTestAsset
 #
 id: example:AcceptanceTestCase001
 name: foo bar
 description: This is an acceptance test case
-test_runner_settings:
+test_case_runner_settings:
   - "inferred"
   - "test"
 test_assets:
   - id: example:AcceptanceTestAsset001
     name: AcceptanceTestAsset001
     description: Iron treats Aceruloplasminemia
     input_id: MONDO:0011426
     predicate_name: treats
     output_id: DRUGBANK:DB01592
     expected_output: NeverShow
-    test_runner_settings:
+    runner_settings:
       - "inferred"
       - "test"
     test_metadata:
         id: "test:1"
         test_source: SMURF
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestAsset-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestAsset-001.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -23,23 +23,24 @@
 #      - qualifiers
 #      - expected_output
 #      - test_issue
 #      - semantic_severity
 #      - in_v1
 #      - well_known
 #      - test_reference
+#      - runner_settings
 #    slot_usage:
 #      id:
 #        aliases: ["AssetIdentifier"]
 #        range: uriorcurie
 #      tags:
 #        description: >-
 #          One or more 'tags' slot values (inherited from TestEntity) should generally
 #          be defined to specify TestAsset membership in a "Block List" collection
-#      test_runner_settings:
+#      runner_settings:
 #        description: >-
 #          Settings for the test harness, e.g. "inferred"
 #
 id: example:TestAsset001
 name: TestAsset001
 description: Iron treats Aceruloplasminemia
 input_id: MONDO:0011426
@@ -50,10 +51,10 @@
 expected_output: NeverShow
 test_reference: https://github.com/NCATSTranslator/Feedback/issues/506
 semantic_severity: NotApplicable
 in_v1: True
 well_known: False
 test_metadata:
   id: "example:TestAsset001"
-test_runner_settings:
+runner_settings:
   - "inferred"
   - "test"
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestCase-001.json` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.65%*

 * *Differences: {"'test_assets'": "{0: {'runner_settings': ['inferred', 'test'], delete: "*

 * *                  "['test_runner_settings']}}",*

 * * "'test_case_runner_settings'": "['inferred', 'test']",*

 * * 'delete': "['test_runner_settings']"}*

```diff
@@ -7,21 +7,21 @@
             "description": "Fingolimod treats multiple sclerosis",
             "expected_output": "Acceptable",
             "id": "example:TestAsset001",
             "input_id": "PUBCHEM.COMPOUND:107970",
             "name": "TestAsset001",
             "output_id": "MONDO:0005301",
             "predicate_name": "treats",
-            "test_metadata": {
-                "id": "example:TestMetadata001"
-            },
-            "test_runner_settings": [
+            "runner_settings": [
                 "inferred",
                 "test"
-            ]
+            ],
+            "test_metadata": {
+                "id": "example:TestMetadata001"
+            }
         }
     ],
-    "test_runner_settings": [
+    "test_case_runner_settings": [
         "inferred",
         "test"
     ]
 }
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestCase-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCase-001.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 test_assets:
   - id: example:TestAsset001
     name: TestAsset001
     input_id: MONDO:0011426
     predicate_name: treats
     output_id: DRUGBANK:DB01592
     expected_output: NeverShow
-    test_runner_settings:
+    runner_settings:
       - "inferred"
       - "test"
     test_metadata:
       id: test:1
       test_source: SMURF
-test_runner_settings:
+test_case_runner_settings:
   - "inferred"
   - "test"
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestCaseSpecification-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestCaseSpecification-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestEntity-Complete.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestEntity-Complete.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 #      all major model classes within the data model for Translator testing.
 #    abstract: true
 #    tree_root: true
 #    slots:
 #      - id
 #      - name
 #      - description
-#      - tags
-#      - test_runner_settings
 #
 # where the slots are:
 #
 #  id:
 #    identifier: true
 #    slot_uri: schema:identifier
 #    range: uriorcurie
```

### Comparing `translator_testing_model-0.3.1/src/data/examples/Good-TestSuite-001.yaml` & `translator_testing_model-2.3.0/src/data/examples/Good-TestSuite-001.yaml`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/data/examples/SampleTestAssetList.json` & `translator_testing_model-2.3.0/src/data/examples/SampleTestAssetList.json`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/adaptor/test_case_generator.py` & `translator_testing_model-2.3.0/src/translator_testing_model/adaptor/test_case_generator.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/adaptor/testrunner.py` & `translator_testing_model-2.3.0/src/translator_testing_model/adaptor/testrunner.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/datamodel/pydanticmodel.py` & `translator_testing_model-2.3.0/src/translator_testing_model/datamodel/pydanticmodel_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,276 +1,262 @@
-from __future__ import annotations 
-from datetime import (
-    datetime,
-    date
-)
-from decimal import Decimal 
-from enum import Enum 
-import re
+from __future__ import annotations
+from datetime import datetime, date
+from enum import Enum
+from typing import List, Dict, Optional, Any, Union
+from pydantic import BaseModel as BaseModel, ConfigDict, Field
 import sys
-from typing import (
-    Any,
-    List,
-    Literal,
-    Dict,
-    Optional,
-    Union
-)
-from pydantic.version import VERSION  as PYDANTIC_VERSION 
-if int(PYDANTIC_VERSION[0])>=2:
-    from pydantic import (
-        BaseModel,
-        ConfigDict,
-        Field,
-        field_validator
-    )
+if sys.version_info >= (3, 8):
+    from typing import Literal
 else:
-    from pydantic import (
-        BaseModel,
-        Field,
-        validator
-    )
+    from typing_extensions import Literal
+
 
 metamodel_version = "None"
 version = "0.0.0"
 
-
 class ConfiguredBaseModel(BaseModel):
     model_config = ConfigDict(
-        validate_assignment = True,
-        validate_default = True,
-        extra = "forbid",
-        arbitrary_types_allowed = True,
-        use_enum_values = True,
-        strict = False,
-    )
-    pass
+        validate_assignment=True,
+        validate_default=True,
+        extra='forbid',
+        arbitrary_types_allowed=True,
+        use_enum_values = True)
 
 
 class TestSourceEnum(str, Enum):
+    
     # (External) Subject Matter Expert
     SME = "SME"
     # Subject Matter User Reasonably Familiar, generally Translator-internal biomedical science expert
     SMURF = "SMURF"
     # Git hub hosted issue from which a test asset/case/suite may be derived.
     GitHubUserFeedback = "GitHubUserFeedback"
     # Technical Advisory Committee, generally posting semantic use cases as Translator Feedback issues
     TACT = "TACT"
     # Curated benchmark tests
     BenchMark = "BenchMark"
     # Translator funded KP or ARA team generating test assets/cases/suites for their resources.
     TranslatorTeam = "TranslatorTeam"
     # Current SRI_Testing-like test data edges specific to KP or ARA components
     TestDataLocation = "TestDataLocation"
-
+    
+    
 
 class TestObjectiveEnum(str, Enum):
+    
     # Acceptance (pass/fail) test
     AcceptanceTest = "AcceptanceTest"
     # Semantic benchmarking
     BenchmarkTest = "BenchmarkTest"
     # Quantitative test
     QuantitativeTest = "QuantitativeTest"
-    # Release-specific TRAPI and Biolink Model ("reasoner-validator") compliance validation
-    StandardsValidationTest = "StandardsValidationTest"
-    # Knowledge graph "One Hop" query navigation integrity
-    OneHopTest = "OneHopTest"
-
+    
+    
 
 class TestEnvEnum(str, Enum):
     """
     Testing environments within which a TestSuite is run by a TestRunner scheduled by the TestHarness.
     """
     # Development
     dev = "dev"
     # Continuous Integration
     ci = "ci"
     # Test
     test = "test"
     # Production
     prod = "prod"
-
+    
+    
 
 class FileFormatEnum(str, Enum):
     """
     Text file formats for test data sources.
     """
+    
     TSV = "TSV"
+    
     YAML = "YAML"
+    
     JSON = "JSON"
-
+    
+    
 
 class ExpectedOutputEnum(str, Enum):
     """
     Expected output values for instances of Test Asset or Test Cases(?). (Note: does this Enum overlap with 'ExpectedResultsEnum' below?)
     """
+    
     Acceptable = "Acceptable"
+    
     BadButForgivable = "BadButForgivable"
+    
     NeverShow = "NeverShow"
+    
     TopAnswer = "TopAnswer"
+    
     OverlyGeneric = "OverlyGeneric"
-
+    
+    
 
 class TestIssueEnum(str, Enum):
+    
+    
     causes_not_treats = "causes not treats"
     # 'Text Mining Knowledge Provider' generated relationship?
     TMKP = "TMKP"
+    
     category_too_generic = "category too generic"
+    
     contraindications = "contraindications"
+    
     chemical_roles = "chemical roles"
+    
     test_issue = "test_issue"
-
+    
+    
 
 class SemanticSeverityEnum(str, Enum):
     """
     From Jenn's worksheet, empty or ill defined (needs elaboration)
     """
+    
     High = "High"
+    
     Low = "Low"
+    
     NotApplicable = "NotApplicable"
-
+    
+    
 
 class DirectionEnum(str, Enum):
+    
+    
     increased = "increased"
+    
     decreased = "decreased"
-
+    
+    
 
 class ExpectedResultsEnum(str, Enum):
     """
     Does this Enum overlap with 'ExpectedOutputEnum' above?
     """
     # The query should return the result in this test case
     include_good = "include_good"
     # The query should not return the result in this test case
     exclude_bad = "exclude_bad"
-
+    
+    
 
 class NodeEnum(str, Enum):
     """
     Target node of a Subject-Predicate-Object driven query
     """
+    
     subject = "subject"
+    
     object = "object"
-
+    
+    
 
 class QueryTypeEnum(str, Enum):
     """
     Query
     """
+    
     treats = "treats"
-
+    
+    
 
 class TrapiTemplateEnum(str, Enum):
+    
+    
     ameliorates = "ameliorates"
+    
     treats = "treats"
+    
     three_hop = "three_hop"
+    
     drug_treats_rare_disease = "drug_treats_rare_disease"
+    
     drug_to_gene = "drug-to-gene"
+    
+    
 
-
-class ComponentEnum(str, Enum):
+class ComponentEnum(str):
     """
     Translator components are identified by their InfoRes identifiers.
     """
-    # Automatic Relay Service component of Translator
-    ars = "ars"
-    # ARAX Translator Reasoner
-    arax = "arax"
-    # A Translator Reasoner API for the Explanatory Agent
-    explanatory = "explanatory"
-    # imProving Agent OpenAPI TRAPI Specification
-    improving = "improving"
-    # Performs a query operation which compiles data from numerous ranking agent services.
-    aragorn = "aragorn"
-    # BioThings Explorer
-    bte = "bte"
-    # Unsecret Agent OpenAPI for NCATS Biomedical Translator Reasoners
-    unsecret = "unsecret"
-    # TRAPI endpoint for the NCATS Biomedical Translator KP called RTX KG2
-    rtxkg2 = "rtxkg2"
-    # ICEES (Integrated Clinical and Environmental Exposures Service)
-    icees = "icees"
-    # Causal Activity Model KP
-    cam = "cam"
-    # SPOKE KP - an NIH NCATS Knowledge Provider to expose UCSFs SPOKE
-    spoke = "spoke"
-    # Molecular Data Provider for NCATS Biomedical Translator Reasoners
-    molepro = "molepro"
-    # Text Mining KP
-    textmining = "textmining"
-    # Columbia Open Health Data (COHD)
-    cohd = "cohd"
-    # OpenPredict API
-    openpredict = "openpredict"
-    # Translator Knowledge Collaboratory API
-    collaboratory = "collaboratory"
-    # Connections Hypothesis Provider API
-    connections = "connections"
-
+    
+    dummy = "dummy"
+    
 
 class TestPersonaEnum(str, Enum):
     """
     User persona context of a given test.
     """
+    
     All = "All"
     # An MD or someone working in the clinical field.
     Clinical = "Clinical"
     # Looking for an answer for a specific patient.
     LookUp = "LookUp"
     # Someone working on basic biology questions or drug discoveries where the study of the biological mechanism.
     Mechanistic = "Mechanistic"
-
+    
+    
 
 class TestCaseResultEnum(str, Enum):
-    # test case result indicating success.
-    PASSED = "PASSED"
-    # test case result indicating failure.
-    FAILED = "FAILED"
-    # test case result indicating that the specified test was not run.
-    SKIPPED = "SKIPPED"
-
+    
+    
+    test_passed = "test_passed"
+    
+    test_failed = "test_failed"
+    
+    test_skipped = "test_skipped"
+    
+    
 
 class TestEntityParameter(ConfiguredBaseModel):
     """
     A single 'tag = value' pair (where 'value' is a simple string).
     """
     parameter: Optional[str] = Field(None, description="""Name of a TestParameter.""")
     value: Optional[str] = Field(None, description="""(String) value of a TestParameter.""")
-
+    
 
 class Qualifier(TestEntityParameter):
+    
     parameter: Optional[str] = Field(None, description="""The 'parameter' of a Qualifier should be a `qualifier` slot name from the Biolink Model ('biolink' namespace) 'biolink:qualifier' hierarchy.""")
     value: Optional[str] = Field(None, description="""The 'value' of should be a suitable value generally drawn from an applicable Biolink Model (\"Enum\") value set of the specified Qualifier.""")
-
+    
 
 class TestEntity(ConfiguredBaseModel):
     """
     Abstract global 'identification' class shared as a parent with all major model classes within the data model for Translator testing.
     """
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestMetadata(TestEntity):
     """
     Represents metadata related to (external SME, SMURF, Translator feedback,  large scale batch, etc.) like the provenance of test assets, cases and/or suites.
     """
     test_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
-    test_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)""")
+    test_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
     test_annotations: Optional[List[TestEntityParameter]] = Field(default_factory=list, description="""Metadata annotation.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestAsset(TestEntity):
     """
     Represents a Test Asset, which is a single specific instance of TestCase-agnostic semantic parameters representing the specification of a Translator test target with inputs and (expected) outputs.
     """
     input_id: Optional[str] = Field(None)
     input_name: Optional[str] = Field(None)
@@ -284,21 +270,21 @@
     qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
     expected_output: Optional[str] = Field(None)
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar settings for the TestRunner, e.g. \"inferred\"""")
-
+    
 
 class AcceptanceTestAsset(TestAsset):
     """
     Model derived from Jenn's test asset design and Shervin's runner JSON here as an example.
     """
     must_pass_date: Optional[date] = Field(None, description="""The date by which this test must pass""")
     must_pass_environment: Optional[TestEnvEnum] = Field(None, description="""The deployment environment within which this test must pass.""")
@@ -322,21 +308,21 @@
     qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
     expected_output: Optional[str] = Field(None)
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar settings for the TestRunner, e.g. \"inferred\"""")
-
+    
 
 class TestEdgeData(TestAsset):
     """
     Represents a single Biolink Model compliant instance of a subject-predicate-object edge that can be used for testing.
     """
     input_id: Optional[str] = Field(None)
     input_name: Optional[str] = Field(None)
@@ -350,229 +336,288 @@
     qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
     expected_output: Optional[str] = Field(None)
     test_issue: Optional[TestIssueEnum] = Field(None)
     semantic_severity: Optional[SemanticSeverityEnum] = Field(None)
     in_v1: Optional[bool] = Field(None)
     well_known: Optional[bool] = Field(None)
     test_reference: Optional[str] = Field(None, description="""Document URL where original test source particulars are registered (e.g. Github repo)""")
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness, e.g. \"inferred\"""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined to specify TestAsset membership in a \"Block List\" collection""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar settings for the TestRunner, e.g. \"inferred\"""")
-
+    
 
 class Precondition(TestEntity):
     """
     Represents a precondition for a TestCase
     """
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestCase(TestEntity):
     """
     Represents a single enumerated instance of Test Case, derived from a  given collection of one or more TestAsset instances (the value of the 'test_assets' slot) which define the 'inputs' and 'outputs' of the TestCase, used to probe a particular test condition.
     """
+    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
     query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
     test_assets: List[TestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
     preconditions: Optional[List[str]] = Field(default_factory=list)
     trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
-    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)""")
+    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
     test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
     test_case_predicate_name: Optional[str] = Field(None)
     test_case_predicate_id: Optional[str] = Field(None)
     test_case_input_id: Optional[str] = Field(None)
-    qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
-    input_category: Optional[str] = Field(None)
-    output_category: Optional[str] = Field(None)
-    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
-    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class AcceptanceTestCase(TestCase):
     """
     See AcceptanceTestAsset above for more details.
     """
+    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
     query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
     test_assets: List[AcceptanceTestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
     preconditions: Optional[List[str]] = Field(default_factory=list)
     trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
-    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)""")
+    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
     test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
     test_case_predicate_name: Optional[str] = Field(None)
     test_case_predicate_id: Optional[str] = Field(None)
     test_case_input_id: Optional[str] = Field(None)
-    qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
-    input_category: Optional[str] = Field(None)
-    output_category: Optional[str] = Field(None)
-    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
-    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class QuantitativeTestCase(TestCase):
     """
     Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete.
     """
+    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
     query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
     test_assets: List[TestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
     preconditions: Optional[List[str]] = Field(default_factory=list)
     trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
-    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)""")
+    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
     test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
     test_case_predicate_name: Optional[str] = Field(None)
     test_case_predicate_id: Optional[str] = Field(None)
     test_case_input_id: Optional[str] = Field(None)
-    qualifiers: Optional[List[Qualifier]] = Field(default_factory=list, description="""Optional qualifiers which constrain to the test asset defined knowledge statement. Note that this field records such qualifier slots and values as tag=value pairs, where the tag is the Biolink Model qualifier slot named and the value is an acceptable (Biolink Model enum?) value of the said qualifier slot.""")
-    input_category: Optional[str] = Field(None)
-    output_category: Optional[str] = Field(None)
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
+    id: str = Field(..., description="""A unique identifier for a Test Entity""")
+    name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
+    description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
+    tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
+    
+
+class ComplianceTestCase(TestCase):
+    """
+    TRAPI and Biolink Model standards compliance test
+    """
+    trapi_version: Optional[str] = Field(None, description="""TRAPI version (SemVer string)""")
+    biolink_version: Optional[str] = Field(None, description="""Biolink Model release (SemVer string)""")
+    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
+    query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
+    test_assets: List[TestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
+    preconditions: Optional[List[str]] = Field(default_factory=list)
+    trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
     components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
+    test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
+    test_case_predicate_name: Optional[str] = Field(None)
+    test_case_predicate_id: Optional[str] = Field(None)
+    test_case_input_id: Optional[str] = Field(None)
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
+    id: str = Field(..., description="""A unique identifier for a Test Entity""")
+    name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
+    description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
+    tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
+    
+
+class KnowledgeGraphNavigationTestCase(TestCase):
+    """
+    Knowledge Graph navigation integration test
+    """
     test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
+    query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
+    test_assets: List[TestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
+    preconditions: Optional[List[str]] = Field(default_factory=list)
+    trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
+    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
+    test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
+    test_case_predicate_name: Optional[str] = Field(None)
+    test_case_predicate_id: Optional[str] = Field(None)
+    test_case_input_id: Optional[str] = Field(None)
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
+    
 
+class OneHopTestCase(KnowledgeGraphNavigationTestCase):
+    """
+    'One Hop' Knowledge Graph navigation integration test
+    """
+    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
+    query_type: Optional[QueryTypeEnum] = Field(None, description="""Type of TestCase query.""")
+    test_assets: List[TestAsset] = Field(default_factory=list, description="""One or more 'tags' slot values (inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in 'test_assets' slot (\"Block List\") collection.""")
+    preconditions: Optional[List[str]] = Field(default_factory=list)
+    trapi_template: Optional[TrapiTemplateEnum] = Field(None, description="""A template for a query, which can be used to generate a query for a test case.  note: the current enumerated values for this slot come from the Benchmarks repo config/benchmarks.json \"templates\" collection and refer to the \"name\" field of each template.  Templates themselves are currently stored in the config/[source_name]/templates directory.""")
+    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
+    test_case_objective: Optional[TestObjectiveEnum] = Field(None, description="""Testing objective behind specified set of test particulars (e.g. acceptance pass/fail; benchmark; quantitative)""")
+    test_case_source: Optional[TestSourceEnum] = Field(None, description="""Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this,  know about this.  We would like this to be an ORCID eventually, but currently it is just a string.""")
+    test_case_predicate_name: Optional[str] = Field(None)
+    test_case_predicate_id: Optional[str] = Field(None)
+    test_case_input_id: Optional[str] = Field(None)
+    test_case_runner_settings: List[str] = Field(default_factory=list, description="""Settings for the test harness for TestCase""")
+    id: str = Field(..., description="""A unique identifier for a Test Entity""")
+    name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
+    description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
+    tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity) should generally be defined as filters to specify TestAsset membership in a \"Block List\" collection.""")
+    
 
 class TestSuiteSpecification(TestEntity):
     """
     Parameters for a Test Case instances either dynamically generated from some external source of Test Assets.
     """
     test_data_file_locator: Optional[str] = Field(None, description="""An web accessible file resource link to test entity data (e.g. a web accessible text file of Test Asset entries)""")
     test_data_file_format: Optional[FileFormatEnum] = Field(None, description="""File format of test entity data (e.g. TSV, YAML or JSON)""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestSuite(TestEntity):
     """
     Specification of a set of Test Cases, one of either with a static list of 'test_cases' or a dynamic 'test_suite_specification' slot values. Note: at least one slot or the other, but generally not both(?) needs to be present.
     """
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     test_persona: Optional[TestPersonaEnum] = Field(None, description="""A Test persona describes the user or operational context of a given test.""")
     test_cases: Optional[Dict[str, TestCase]] = Field(default_factory=dict, description="""List of explicitly enumerated Test Cases.""")
     test_suite_specification: Optional[TestSuiteSpecification] = Field(None, description="""Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class AcceptanceTestSuite(TestSuite):
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     test_persona: Optional[TestPersonaEnum] = Field(None, description="""A Test persona describes the user or operational context of a given test.""")
     test_cases: Optional[Dict[str, TestCase]] = Field(default_factory=dict, description="""List of explicitly enumerated Test Cases.""")
     test_suite_specification: Optional[TestSuiteSpecification] = Field(None, description="""Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class BenchmarkTestSuite(ConfiguredBaseModel):
     """
     JsonObj(is_a='TestSuite')
     """
-    pass
-
+    None
+    
 
 class StandardsComplianceTestSuite(TestSuite):
     """
     Test suite for testing Translator components against releases of standards like TRAPI and the Biolink Model.
     """
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     test_persona: Optional[TestPersonaEnum] = Field(None, description="""A Test persona describes the user or operational context of a given test.""")
     test_cases: Optional[Dict[str, TestCase]] = Field(default_factory=dict, description="""List of explicitly enumerated Test Cases.""")
     test_suite_specification: Optional[TestSuiteSpecification] = Field(None, description="""Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class OneHopTestSuite(TestSuite):
     """
     Test case for testing the integrity of \"One Hop\" knowledge graph retrievals sensa legacy SRI_Testing harness.
     """
-    test_metadata: Optional[TestMetadata] = Field(None, description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
+    test_metadata: TestMetadata = Field(..., description="""Test metadata describes the external provenance, cross-references and objectives for a given test.""")
     test_persona: Optional[TestPersonaEnum] = Field(None, description="""A Test persona describes the user or operational context of a given test.""")
     test_cases: Optional[Dict[str, TestCase]] = Field(default_factory=dict, description="""List of explicitly enumerated Test Cases.""")
     test_suite_specification: Optional[TestSuiteSpecification] = Field(None, description="""Declarative specification of a Test Suite of Test Cases whose generation is deferred, (i.e. within a Test Runner) or whose creation is achieved by stream processing of an external data source.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
+    
 
+class TestRunnerConfiguration(TestEntity):
+    """
+    General configuration parameters and test data input  for a single invocation of a TestRunner.
+    """
+    test_run_parameters: Optional[List[TestEntityParameter]] = Field(default_factory=list, description="""Parameters for TestRunnerConfiguration that inform the TestHarness and TestRunners about the general characteristics of a test run.""")
+    id: str = Field(..., description="""A unique identifier for a Test Entity""")
+    name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
+    description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
+    tags: Optional[List[str]] = Field(default_factory=list, description="""One or more 'tags' slot values (slot inherited from TestEntity)  should generally identify the TestRunner(s) using this configuration.""")
+    
 
 class TestCaseResult(TestEntity):
     """
     The outcome of a TestRunner run of one specific TestCase.
     """
     test_suite_id: Optional[str] = Field(None, description="""CURIE id of a TestSuite registered in the system.""")
     test_case: Optional[TestCase] = Field(None, description="""Slot referencing a single TestCase.""")
     test_case_result: Optional[TestCaseResultEnum] = Field(None, description="""Encoded result of a single test run of a given test case""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestRunSession(TestEntity):
     """
-    Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more instances of TestSuite).
+    A single invocation of a TestRunner.
     """
-    components: Optional[List[ComponentEnum]] = Field(default_factory=list, description="""The component that this test case is intended to run against.  Most often this is the ARS for  acceptance tests, but for the Benchmarks repo integration, this can also be individual components of the system like Aragorn, or ARAX.""")
-    test_env: Optional[TestEnvEnum] = Field(None, description="""Deployment environment within which the associated TestSuite is run.""")
     test_runner_name: Optional[str] = Field(None, description="""Global system name of a TestRunner.""")
-    test_run_parameters: Optional[List[TestEntityParameter]] = Field(default_factory=list, description="""Different TestRunners could expect additional global test configuration parameters, like the applicable TRAPI version (\"trapi_version\") or Biolink Model versions (\"biolink_version\").""")
-    test_entities: Optional[Dict[str, TestEntity]] = Field(default_factory=dict, description="""Different TestRunners could expect specific kinds of TestEntity as an input.  These 'test_entities' are one or more instances of TestAsset, TestCase or (preferably?) TestSuite.""")
+    test_entities: Optional[Dict[str, TestEntity]] = Field(default_factory=dict, description="""Different TestRunners may expect specific kinds of TestEntity as input. These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite.""")
     test_case_results: Optional[Dict[str, TestCaseResult]] = Field(default_factory=dict, description="""One or more instances of TestCaseResult.""")
     timestamp: Optional[datetime ] = Field(None, description="""Date time when a given entity was created.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestOutput(TestEntity):
     """
     The output of a TestRunner run of one specific TestCase.
     """
     test_case_id: Optional[str] = Field(None, description="""CURIE id of a TestCase registered in the system.""")
     pks: Optional[List[str]] = Field(default_factory=list, description="""Primary keys for a given ARA result set from a SmokeTest result for a given TestCase.""")
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
-
+    
 
 class TestResultPKSet(TestEntity):
     """
     Primary keys for a given ARA result set from a SmokeTest result for a given TestCase.
     """
     parent_pk: Optional[str] = Field(None)
     merged_pk: Optional[str] = Field(None)
@@ -581,15 +626,15 @@
     unsecret: Optional[str] = Field(None)
     bte: Optional[str] = Field(None)
     improving: Optional[str] = Field(None)
     id: str = Field(..., description="""A unique identifier for a Test Entity""")
     name: Optional[str] = Field(None, description="""A human-readable name for a Test Entity""")
     description: Optional[str] = Field(None, description="""A human-readable description for a Test Entity""")
     tags: Optional[List[str]] = Field(default_factory=list, description="""A human-readable tags for categorical memberships of a TestEntity (preferably a URI or CURIE). Typically used to aggregate instances of TestEntity into formally typed or ad hoc lists.""")
-    test_runner_settings: Optional[List[str]] = Field(default_factory=list, description="""Scalar parameters for the TestRunner processing a given TestEntity.""")
+    
 
 
 # Model rebuild
 # see https://pydantic-docs.helpmanual.io/usage/models/#rebuilding-a-model
 TestEntityParameter.model_rebuild()
 Qualifier.model_rebuild()
 TestEntity.model_rebuild()
@@ -597,18 +642,22 @@
 TestAsset.model_rebuild()
 AcceptanceTestAsset.model_rebuild()
 TestEdgeData.model_rebuild()
 Precondition.model_rebuild()
 TestCase.model_rebuild()
 AcceptanceTestCase.model_rebuild()
 QuantitativeTestCase.model_rebuild()
+ComplianceTestCase.model_rebuild()
+KnowledgeGraphNavigationTestCase.model_rebuild()
+OneHopTestCase.model_rebuild()
 TestSuiteSpecification.model_rebuild()
 TestSuite.model_rebuild()
 AcceptanceTestSuite.model_rebuild()
 BenchmarkTestSuite.model_rebuild()
 StandardsComplianceTestSuite.model_rebuild()
 OneHopTestSuite.model_rebuild()
+TestRunnerConfiguration.model_rebuild()
 TestCaseResult.model_rebuild()
 TestRunSession.model_rebuild()
 TestOutput.model_rebuild()
 TestResultPKSet.model_rebuild()
```

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/datamodel/translator_testing_model.py` & `translator_testing_model-2.3.0/src/translator_testing_model/datamodel/translator_testing_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Auto generated from translator_testing_model.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-04-25T16:46:31
+# Generation date: 2024-03-18T12:26:26
 # Schema: Translator-Testing-Model
 #
 # id: https://w3id.org/TranslatorSRI/TranslatorTestingModel
 # description: Data model to formalize the structure of test assets, cases, suites and related metadata
 #   applied to run the diverse polymorphic testing objectives for the Biomedical Data Translator system.
 # license: MIT
 
 import dataclasses
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from datetime import date, datetime
 from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
 from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
 from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
 from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
@@ -31,15 +30,14 @@
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
 BIOLINK = CurieNamespace('biolink', 'https://w3id.org/biolink/')
 EXAMPLE = CurieNamespace('example', 'https://example.org/')
-INFORES = CurieNamespace('infores', 'https://w3id.org/biolink/vocab/')
 LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
 SCHEMA = CurieNamespace('schema', 'http://schema.org/')
 TTM = CurieNamespace('ttm', 'https://w3id.org/TranslatorSRI/TranslatorTestingModel/')
 XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = TTM
 
 
@@ -109,14 +107,26 @@
     pass
 
 
 class QuantitativeTestCaseId(TestCaseId):
     pass
 
 
+class ComplianceTestCaseId(TestCaseId):
+    pass
+
+
+class KnowledgeGraphNavigationTestCaseId(TestCaseId):
+    pass
+
+
+class OneHopTestCaseId(KnowledgeGraphNavigationTestCaseId):
+    pass
+
+
 class TestSuiteSpecificationId(TestEntityId):
     pass
 
 
 class TestSuiteId(TestEntityId):
     pass
 
@@ -129,14 +139,18 @@
     pass
 
 
 class OneHopTestSuiteId(TestSuiteId):
     pass
 
 
+class TestRunnerConfigurationId(TestEntityId):
+    pass
+
+
 class TestCaseResultId(TestEntityId):
     pass
 
 
 class TestRunSessionId(TestEntityId):
     pass
 
@@ -209,15 +223,14 @@
     class_name: ClassVar[str] = "TestEntity"
     class_model_uri: ClassVar[URIRef] = TTM.TestEntity
 
     id: Union[str, TestEntityId] = None
     name: Optional[str] = None
     description: Optional[str] = None
     tags: Optional[Union[str, List[str]]] = empty_list()
-    test_runner_settings: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestEntityId):
             self.id = TestEntityId(self.id)
 
@@ -227,18 +240,14 @@
         if self.description is not None and not isinstance(self.description, str):
             self.description = str(self.description)
 
         if not isinstance(self.tags, list):
             self.tags = [self.tags] if self.tags is not None else []
         self.tags = [v if isinstance(v, str) else str(v) for v in self.tags]
 
-        if not isinstance(self.test_runner_settings, list):
-            self.test_runner_settings = [self.test_runner_settings] if self.test_runner_settings is not None else []
-        self.test_runner_settings = [v if isinstance(v, str) else str(v) for v in self.test_runner_settings]
-
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class TestMetadata(TestEntity):
     """
     Represents metadata related to (external SME, SMURF, Translator feedback, large scale batch, etc.) like the
@@ -289,14 +298,16 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["TestAsset"]
     class_class_curie: ClassVar[str] = "ttm:TestAsset"
     class_name: ClassVar[str] = "TestAsset"
     class_model_uri: ClassVar[URIRef] = TTM.TestAsset
 
     id: Union[str, TestAssetId] = None
+    runner_settings: Union[str, List[str]] = None
+    test_metadata: Union[dict, TestMetadata] = None
     input_id: Optional[Union[str, URIorCURIE]] = None
     input_name: Optional[str] = None
     input_category: Optional[Union[str, ConceptCategory]] = None
     predicate_id: Optional[Union[str, PredicateType]] = None
     predicate_name: Optional[str] = None
     output_id: Optional[Union[str, URIorCURIE]] = None
     output_name: Optional[str] = None
@@ -305,24 +316,33 @@
     qualifiers: Optional[Union[Union[dict, Qualifier], List[Union[dict, Qualifier]]]] = empty_list()
     expected_output: Optional[str] = None
     test_issue: Optional[Union[str, "TestIssueEnum"]] = None
     semantic_severity: Optional[Union[str, "SemanticSeverityEnum"]] = None
     in_v1: Optional[Union[bool, Bool]] = None
     well_known: Optional[Union[bool, Bool]] = None
     test_reference: Optional[Union[str, URIorCURIE]] = None
-    test_metadata: Optional[Union[dict, TestMetadata]] = None
     tags: Optional[Union[str, List[str]]] = empty_list()
-    test_runner_settings: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestAssetId):
             self.id = TestAssetId(self.id)
 
+        if self._is_empty(self.runner_settings):
+            self.MissingRequiredField("runner_settings")
+        if not isinstance(self.runner_settings, list):
+            self.runner_settings = [self.runner_settings] if self.runner_settings is not None else []
+        self.runner_settings = [v if isinstance(v, str) else str(v) for v in self.runner_settings]
+
+        if self._is_empty(self.test_metadata):
+            self.MissingRequiredField("test_metadata")
+        if not isinstance(self.test_metadata, TestMetadata):
+            self.test_metadata = TestMetadata(**as_dict(self.test_metadata))
+
         if self.input_id is not None and not isinstance(self.input_id, URIorCURIE):
             self.input_id = URIorCURIE(self.input_id)
 
         if self.input_name is not None and not isinstance(self.input_name, str):
             self.input_name = str(self.input_name)
 
         if self.input_category is not None and not isinstance(self.input_category, ConceptCategory):
@@ -364,25 +384,18 @@
 
         if self.well_known is not None and not isinstance(self.well_known, Bool):
             self.well_known = Bool(self.well_known)
 
         if self.test_reference is not None and not isinstance(self.test_reference, URIorCURIE):
             self.test_reference = URIorCURIE(self.test_reference)
 
-        if self.test_metadata is not None and not isinstance(self.test_metadata, TestMetadata):
-            self.test_metadata = TestMetadata(**as_dict(self.test_metadata))
-
         if not isinstance(self.tags, list):
             self.tags = [self.tags] if self.tags is not None else []
         self.tags = [v if isinstance(v, str) else str(v) for v in self.tags]
 
-        if not isinstance(self.test_runner_settings, list):
-            self.test_runner_settings = [self.test_runner_settings] if self.test_runner_settings is not None else []
-        self.test_runner_settings = [v if isinstance(v, str) else str(v) for v in self.test_runner_settings]
-
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class AcceptanceTestAsset(TestAsset):
     """
     Model derived from Jenn's test asset design and Shervin's runner JSON here as an example.
@@ -391,14 +404,16 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["AcceptanceTestAsset"]
     class_class_curie: ClassVar[str] = "ttm:AcceptanceTestAsset"
     class_name: ClassVar[str] = "AcceptanceTestAsset"
     class_model_uri: ClassVar[URIRef] = TTM.AcceptanceTestAsset
 
     id: Union[str, AcceptanceTestAssetId] = None
+    runner_settings: Union[str, List[str]] = None
+    test_metadata: Union[dict, TestMetadata] = None
     must_pass_date: Optional[Union[str, XSDDate]] = None
     must_pass_environment: Optional[Union[str, "TestEnvEnum"]] = None
     scientific_question: Optional[str] = None
     string_entry: Optional[str] = None
     direction: Optional[Union[str, "DirectionEnum"]] = None
     answer_informal_concept: Optional[str] = None
     expected_result: Optional[Union[str, "ExpectedResultsEnum"]] = None
@@ -455,14 +470,16 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["TestEdgeData"]
     class_class_curie: ClassVar[str] = "ttm:TestEdgeData"
     class_name: ClassVar[str] = "TestEdgeData"
     class_model_uri: ClassVar[URIRef] = TTM.TestEdgeData
 
     id: Union[str, TestEdgeDataId] = None
+    runner_settings: Union[str, List[str]] = None
+    test_metadata: Union[dict, TestMetadata] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestEdgeDataId):
             self.id = TestEdgeDataId(self.id)
 
@@ -504,49 +521,60 @@
     class_class_uri: ClassVar[URIRef] = TTM["TestCase"]
     class_class_curie: ClassVar[str] = "ttm:TestCase"
     class_name: ClassVar[str] = "TestCase"
     class_model_uri: ClassVar[URIRef] = TTM.TestCase
 
     id: Union[str, TestCaseId] = None
     test_assets: Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]] = empty_dict()
+    test_case_runner_settings: Union[str, List[str]] = None
+    test_env: Optional[Union[str, "TestEnvEnum"]] = None
     query_type: Optional[Union[str, "QueryTypeEnum"]] = None
     preconditions: Optional[Union[Union[str, PreconditionId], List[Union[str, PreconditionId]]]] = empty_list()
     trapi_template: Optional[Union[str, "TrapiTemplateEnum"]] = None
+    components: Optional[Union[Union[str, "ComponentEnum"], List[Union[str, "ComponentEnum"]]]] = empty_list()
     test_case_objective: Optional[Union[str, "TestObjectiveEnum"]] = None
     test_case_source: Optional[Union[str, "TestSourceEnum"]] = None
     test_case_predicate_name: Optional[str] = None
     test_case_predicate_id: Optional[str] = None
     test_case_input_id: Optional[Union[str, URIorCURIE]] = None
-    qualifiers: Optional[Union[Union[dict, Qualifier], List[Union[dict, Qualifier]]]] = empty_list()
-    input_category: Optional[Union[str, ConceptCategory]] = None
-    output_category: Optional[Union[str, ConceptCategory]] = None
-    components: Optional[Union[Union[str, "ComponentEnum"], List[Union[str, "ComponentEnum"]]]] = empty_list()
-    test_env: Optional[Union[str, "TestEnvEnum"]] = None
     tags: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestCaseId):
             self.id = TestCaseId(self.id)
 
         if self._is_empty(self.test_assets):
             self.MissingRequiredField("test_assets")
         self._normalize_inlined_as_list(slot_name="test_assets", slot_type=TestAsset, key_name="id", keyed=True)
 
+        if self._is_empty(self.test_case_runner_settings):
+            self.MissingRequiredField("test_case_runner_settings")
+        if not isinstance(self.test_case_runner_settings, list):
+            self.test_case_runner_settings = [self.test_case_runner_settings] if self.test_case_runner_settings is not None else []
+        self.test_case_runner_settings = [v if isinstance(v, str) else str(v) for v in self.test_case_runner_settings]
+
+        if self.test_env is not None and not isinstance(self.test_env, TestEnvEnum):
+            self.test_env = TestEnvEnum(self.test_env)
+
         if self.query_type is not None and not isinstance(self.query_type, QueryTypeEnum):
             self.query_type = QueryTypeEnum(self.query_type)
 
         if not isinstance(self.preconditions, list):
             self.preconditions = [self.preconditions] if self.preconditions is not None else []
         self.preconditions = [v if isinstance(v, PreconditionId) else PreconditionId(v) for v in self.preconditions]
 
         if self.trapi_template is not None and not isinstance(self.trapi_template, TrapiTemplateEnum):
             self.trapi_template = TrapiTemplateEnum(self.trapi_template)
 
+        if not isinstance(self.components, list):
+            self.components = [self.components] if self.components is not None else []
+        self.components = [v if isinstance(v, ComponentEnum) else ComponentEnum(v) for v in self.components]
+
         if self.test_case_objective is not None and not isinstance(self.test_case_objective, TestObjectiveEnum):
             self.test_case_objective = TestObjectiveEnum(self.test_case_objective)
 
         if self.test_case_source is not None and not isinstance(self.test_case_source, TestSourceEnum):
             self.test_case_source = TestSourceEnum(self.test_case_source)
 
         if self.test_case_predicate_name is not None and not isinstance(self.test_case_predicate_name, str):
@@ -554,31 +582,14 @@
 
         if self.test_case_predicate_id is not None and not isinstance(self.test_case_predicate_id, str):
             self.test_case_predicate_id = str(self.test_case_predicate_id)
 
         if self.test_case_input_id is not None and not isinstance(self.test_case_input_id, URIorCURIE):
             self.test_case_input_id = URIorCURIE(self.test_case_input_id)
 
-        if not isinstance(self.qualifiers, list):
-            self.qualifiers = [self.qualifiers] if self.qualifiers is not None else []
-        self.qualifiers = [v if isinstance(v, Qualifier) else Qualifier(**as_dict(v)) for v in self.qualifiers]
-
-        if self.input_category is not None and not isinstance(self.input_category, ConceptCategory):
-            self.input_category = ConceptCategory(self.input_category)
-
-        if self.output_category is not None and not isinstance(self.output_category, ConceptCategory):
-            self.output_category = ConceptCategory(self.output_category)
-
-        if not isinstance(self.components, list):
-            self.components = [self.components] if self.components is not None else []
-        self.components = [v if isinstance(v, ComponentEnum) else ComponentEnum(v) for v in self.components]
-
-        if self.test_env is not None and not isinstance(self.test_env, TestEnvEnum):
-            self.test_env = TestEnvEnum(self.test_env)
-
         if not isinstance(self.tags, list):
             self.tags = [self.tags] if self.tags is not None else []
         self.tags = [v if isinstance(v, str) else str(v) for v in self.tags]
 
         super().__post_init__(**kwargs)
 
 
@@ -591,14 +602,15 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["AcceptanceTestCase"]
     class_class_curie: ClassVar[str] = "ttm:AcceptanceTestCase"
     class_name: ClassVar[str] = "AcceptanceTestCase"
     class_model_uri: ClassVar[URIRef] = TTM.AcceptanceTestCase
 
     id: Union[str, AcceptanceTestCaseId] = None
+    test_case_runner_settings: Union[str, List[str]] = None
     test_assets: Union[Dict[Union[str, AcceptanceTestAssetId], Union[dict, AcceptanceTestAsset]], List[Union[dict, AcceptanceTestAsset]]] = empty_dict()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, AcceptanceTestCaseId):
             self.id = AcceptanceTestCaseId(self.id)
@@ -620,25 +632,109 @@
     class_class_uri: ClassVar[URIRef] = TTM["QuantitativeTestCase"]
     class_class_curie: ClassVar[str] = "ttm:QuantitativeTestCase"
     class_name: ClassVar[str] = "QuantitativeTestCase"
     class_model_uri: ClassVar[URIRef] = TTM.QuantitativeTestCase
 
     id: Union[str, QuantitativeTestCaseId] = None
     test_assets: Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]] = empty_dict()
+    test_case_runner_settings: Union[str, List[str]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, QuantitativeTestCaseId):
             self.id = QuantitativeTestCaseId(self.id)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
+class ComplianceTestCase(TestCase):
+    """
+    TRAPI and Biolink Model standards compliance test
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = TTM["ComplianceTestCase"]
+    class_class_curie: ClassVar[str] = "ttm:ComplianceTestCase"
+    class_name: ClassVar[str] = "ComplianceTestCase"
+    class_model_uri: ClassVar[URIRef] = TTM.ComplianceTestCase
+
+    id: Union[str, ComplianceTestCaseId] = None
+    test_assets: Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]] = empty_dict()
+    test_case_runner_settings: Union[str, List[str]] = None
+    trapi_version: Optional[str] = None
+    biolink_version: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, ComplianceTestCaseId):
+            self.id = ComplianceTestCaseId(self.id)
+
+        if self.trapi_version is not None and not isinstance(self.trapi_version, str):
+            self.trapi_version = str(self.trapi_version)
+
+        if self.biolink_version is not None and not isinstance(self.biolink_version, str):
+            self.biolink_version = str(self.biolink_version)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class KnowledgeGraphNavigationTestCase(TestCase):
+    """
+    Knowledge Graph navigation integration test
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = TTM["KnowledgeGraphNavigationTestCase"]
+    class_class_curie: ClassVar[str] = "ttm:KnowledgeGraphNavigationTestCase"
+    class_name: ClassVar[str] = "KnowledgeGraphNavigationTestCase"
+    class_model_uri: ClassVar[URIRef] = TTM.KnowledgeGraphNavigationTestCase
+
+    id: Union[str, KnowledgeGraphNavigationTestCaseId] = None
+    test_assets: Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]] = empty_dict()
+    test_case_runner_settings: Union[str, List[str]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, KnowledgeGraphNavigationTestCaseId):
+            self.id = KnowledgeGraphNavigationTestCaseId(self.id)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class OneHopTestCase(KnowledgeGraphNavigationTestCase):
+    """
+    'One Hop' Knowledge Graph navigation integration test
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = TTM["OneHopTestCase"]
+    class_class_curie: ClassVar[str] = "ttm:OneHopTestCase"
+    class_name: ClassVar[str] = "OneHopTestCase"
+    class_model_uri: ClassVar[URIRef] = TTM.OneHopTestCase
+
+    id: Union[str, OneHopTestCaseId] = None
+    test_assets: Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]] = empty_dict()
+    test_case_runner_settings: Union[str, List[str]] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, OneHopTestCaseId):
+            self.id = OneHopTestCaseId(self.id)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
 class TestSuiteSpecification(TestEntity):
     """
     Parameters for a Test Case instances either dynamically generated from some external source of Test Assets.
     """
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = TTM["TestSuiteSpecification"]
@@ -676,26 +772,28 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["TestSuite"]
     class_class_curie: ClassVar[str] = "ttm:TestSuite"
     class_name: ClassVar[str] = "TestSuite"
     class_model_uri: ClassVar[URIRef] = TTM.TestSuite
 
     id: Union[str, TestSuiteId] = None
-    test_metadata: Optional[Union[dict, TestMetadata]] = None
+    test_metadata: Union[dict, TestMetadata] = None
     test_persona: Optional[Union[str, "TestPersonaEnum"]] = None
     test_cases: Optional[Union[Dict[Union[str, TestCaseId], Union[dict, TestCase]], List[Union[dict, TestCase]]]] = empty_dict()
     test_suite_specification: Optional[Union[dict, TestSuiteSpecification]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestSuiteId):
             self.id = TestSuiteId(self.id)
 
-        if self.test_metadata is not None and not isinstance(self.test_metadata, TestMetadata):
+        if self._is_empty(self.test_metadata):
+            self.MissingRequiredField("test_metadata")
+        if not isinstance(self.test_metadata, TestMetadata):
             self.test_metadata = TestMetadata(**as_dict(self.test_metadata))
 
         if self.test_persona is not None and not isinstance(self.test_persona, TestPersonaEnum):
             self.test_persona = TestPersonaEnum(self.test_persona)
 
         self._normalize_inlined_as_dict(slot_name="test_cases", slot_type=TestCase, key_name="id", keyed=True)
 
@@ -711,14 +809,15 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["AcceptanceTestSuite"]
     class_class_curie: ClassVar[str] = "ttm:AcceptanceTestSuite"
     class_name: ClassVar[str] = "AcceptanceTestSuite"
     class_model_uri: ClassVar[URIRef] = TTM.AcceptanceTestSuite
 
     id: Union[str, AcceptanceTestSuiteId] = None
+    test_metadata: Union[dict, TestMetadata] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, AcceptanceTestSuiteId):
             self.id = AcceptanceTestSuiteId(self.id)
 
@@ -746,14 +845,15 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["StandardsComplianceTestSuite"]
     class_class_curie: ClassVar[str] = "ttm:StandardsComplianceTestSuite"
     class_name: ClassVar[str] = "StandardsComplianceTestSuite"
     class_model_uri: ClassVar[URIRef] = TTM.StandardsComplianceTestSuite
 
     id: Union[str, StandardsComplianceTestSuiteId] = None
+    test_metadata: Union[dict, TestMetadata] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, StandardsComplianceTestSuiteId):
             self.id = StandardsComplianceTestSuiteId(self.id)
 
@@ -769,25 +869,59 @@
 
     class_class_uri: ClassVar[URIRef] = TTM["OneHopTestSuite"]
     class_class_curie: ClassVar[str] = "ttm:OneHopTestSuite"
     class_name: ClassVar[str] = "OneHopTestSuite"
     class_model_uri: ClassVar[URIRef] = TTM.OneHopTestSuite
 
     id: Union[str, OneHopTestSuiteId] = None
+    test_metadata: Union[dict, TestMetadata] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, OneHopTestSuiteId):
             self.id = OneHopTestSuiteId(self.id)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
+class TestRunnerConfiguration(TestEntity):
+    """
+    General configuration parameters and test data input  for a single invocation of a TestRunner.
+    """
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = TTM["TestRunnerConfiguration"]
+    class_class_curie: ClassVar[str] = "ttm:TestRunnerConfiguration"
+    class_name: ClassVar[str] = "TestRunnerConfiguration"
+    class_model_uri: ClassVar[URIRef] = TTM.TestRunnerConfiguration
+
+    id: Union[str, TestRunnerConfigurationId] = None
+    test_run_parameters: Optional[Union[Union[dict, TestEntityParameter], List[Union[dict, TestEntityParameter]]]] = empty_list()
+    tags: Optional[Union[str, List[str]]] = empty_list()
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, TestRunnerConfigurationId):
+            self.id = TestRunnerConfigurationId(self.id)
+
+        if not isinstance(self.test_run_parameters, list):
+            self.test_run_parameters = [self.test_run_parameters] if self.test_run_parameters is not None else []
+        self.test_run_parameters = [v if isinstance(v, TestEntityParameter) else TestEntityParameter(**as_dict(v)) for v in self.test_run_parameters]
+
+        if not isinstance(self.tags, list):
+            self.tags = [self.tags] if self.tags is not None else []
+        self.tags = [v if isinstance(v, str) else str(v) for v in self.tags]
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
 class TestCaseResult(TestEntity):
     """
     The outcome of a TestRunner run of one specific TestCase.
     """
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = TTM["TestCaseResult"]
@@ -817,53 +951,38 @@
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class TestRunSession(TestEntity):
     """
-    Single run of a TestRunner in a given environment, with a specified set of test_entities (generally, one or more
-    instances of TestSuite).
+    A single invocation of a TestRunner.
     """
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = TTM["TestRunSession"]
     class_class_curie: ClassVar[str] = "ttm:TestRunSession"
     class_name: ClassVar[str] = "TestRunSession"
     class_model_uri: ClassVar[URIRef] = TTM.TestRunSession
 
     id: Union[str, TestRunSessionId] = None
-    components: Optional[Union[Union[str, "ComponentEnum"], List[Union[str, "ComponentEnum"]]]] = empty_list()
-    test_env: Optional[Union[str, "TestEnvEnum"]] = None
     test_runner_name: Optional[str] = None
-    test_run_parameters: Optional[Union[Union[dict, TestEntityParameter], List[Union[dict, TestEntityParameter]]]] = empty_list()
     test_entities: Optional[Union[Dict[Union[str, TestEntityId], Union[dict, TestEntity]], List[Union[dict, TestEntity]]]] = empty_dict()
     test_case_results: Optional[Union[Dict[Union[str, TestCaseResultId], Union[dict, TestCaseResult]], List[Union[dict, TestCaseResult]]]] = empty_dict()
     timestamp: Optional[Union[str, XSDDateTime]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TestRunSessionId):
             self.id = TestRunSessionId(self.id)
 
-        if not isinstance(self.components, list):
-            self.components = [self.components] if self.components is not None else []
-        self.components = [v if isinstance(v, ComponentEnum) else ComponentEnum(v) for v in self.components]
-
-        if self.test_env is not None and not isinstance(self.test_env, TestEnvEnum):
-            self.test_env = TestEnvEnum(self.test_env)
-
         if self.test_runner_name is not None and not isinstance(self.test_runner_name, str):
             self.test_runner_name = str(self.test_runner_name)
 
-        if not isinstance(self.test_run_parameters, list):
-            self.test_run_parameters = [self.test_run_parameters] if self.test_run_parameters is not None else []
-        self.test_run_parameters = [v if isinstance(v, TestEntityParameter) else TestEntityParameter(**as_dict(v)) for v in self.test_run_parameters]
-
         self._normalize_inlined_as_dict(slot_name="test_entities", slot_type=TestEntity, key_name="id", keyed=True)
 
         self._normalize_inlined_as_dict(slot_name="test_case_results", slot_type=TestCaseResult, key_name="id", keyed=True)
 
         if self.timestamp is not None and not isinstance(self.timestamp, XSDDateTime):
             self.timestamp = XSDDateTime(self.timestamp)
 
@@ -989,20 +1108,14 @@
         description="Acceptance (pass/fail) test")
     BenchmarkTest = PermissibleValue(
         text="BenchmarkTest",
         description="Semantic benchmarking")
     QuantitativeTest = PermissibleValue(
         text="QuantitativeTest",
         description="Quantitative test")
-    StandardsValidationTest = PermissibleValue(
-        text="StandardsValidationTest",
-        description="Release-specific TRAPI and Biolink Model (\"reasoner-validator\") compliance validation")
-    OneHopTest = PermissibleValue(
-        text="OneHopTest",
-        description="Knowledge graph \"One Hop\" query navigation integrity")
 
     _defn = EnumDefinition(
         name="TestObjectiveEnum",
     )
 
 class TestEnvEnum(EnumDefinitionImpl):
     """
@@ -1153,83 +1266,14 @@
         setattr(cls, "drug-to-gene",
             PermissibleValue(text="drug-to-gene"))
 
 class ComponentEnum(EnumDefinitionImpl):
     """
     Translator components are identified by their InfoRes identifiers.
     """
-    ars = PermissibleValue(
-        text="ars",
-        description="Automatic Relay Service component of Translator",
-        meaning=INFORES["ncats-ars"])
-    arax = PermissibleValue(
-        text="arax",
-        description="ARAX Translator Reasoner",
-        meaning=INFORES["arax"])
-    explanatory = PermissibleValue(
-        text="explanatory",
-        description="A Translator Reasoner API for the Explanatory Agent",
-        meaning=INFORES["explanatory-agent"])
-    improving = PermissibleValue(
-        text="improving",
-        description="imProving Agent OpenAPI TRAPI Specification",
-        meaning=INFORES["improving-agent"])
-    aragorn = PermissibleValue(
-        text="aragorn",
-        description="Performs a query operation which compiles data from numerous ranking agent services.",
-        meaning=INFORES["aragorn"])
-    bte = PermissibleValue(
-        text="bte",
-        description="BioThings Explorer",
-        meaning=INFORES["biothings-explorer"])
-    unsecret = PermissibleValue(
-        text="unsecret",
-        description="Unsecret Agent OpenAPI for NCATS Biomedical Translator Reasoners",
-        meaning=INFORES["unsecret-agent"])
-    rtxkg2 = PermissibleValue(
-        text="rtxkg2",
-        description="TRAPI endpoint for the NCATS Biomedical Translator KP called RTX KG2",
-        meaning=INFORES["rtx-kg2"])
-    icees = PermissibleValue(
-        text="icees",
-        description="ICEES (Integrated Clinical and Environmental Exposures Service)",
-        meaning=INFORES["icees-kg"])
-    cam = PermissibleValue(
-        text="cam",
-        description="Causal Activity Model KP",
-        meaning=INFORES["cam-kp"])
-    spoke = PermissibleValue(
-        text="spoke",
-        description="SPOKE KP - an NIH NCATS Knowledge Provider to expose UCSFs SPOKE",
-        meaning=INFORES["spoke"])
-    molepro = PermissibleValue(
-        text="molepro",
-        description="Molecular Data Provider for NCATS Biomedical Translator Reasoners",
-        meaning=INFORES["molepro"])
-    textmining = PermissibleValue(
-        text="textmining",
-        description="Text Mining KP",
-        meaning=INFORES["textmining-kp"])
-    cohd = PermissibleValue(
-        text="cohd",
-        description="Columbia Open Health Data (COHD)",
-        meaning=INFORES["cohd"])
-    openpredict = PermissibleValue(
-        text="openpredict",
-        description="OpenPredict API",
-        meaning=INFORES["openpredict"])
-    collaboratory = PermissibleValue(
-        text="collaboratory",
-        description="Translator Knowledge Collaboratory API",
-        meaning=INFORES["knowledge-collaboratory"])
-    connections = PermissibleValue(
-        text="connections",
-        description="Connections Hypothesis Provider API",
-        meaning=INFORES["connections-hypothesis"])
-
     _defn = EnumDefinition(
         name="ComponentEnum",
         description="Translator components are identified by their InfoRes identifiers.",
     )
 
 class TestPersonaEnum(EnumDefinitionImpl):
     """
@@ -1249,23 +1293,17 @@
     _defn = EnumDefinition(
         name="TestPersonaEnum",
         description="User persona context of a given test.",
     )
 
 class TestCaseResultEnum(EnumDefinitionImpl):
 
-    PASSED = PermissibleValue(
-        text="PASSED",
-        description="test case result indicating success.")
-    FAILED = PermissibleValue(
-        text="FAILED",
-        description="test case result indicating failure.")
-    SKIPPED = PermissibleValue(
-        text="SKIPPED",
-        description="test case result indicating that the specified test was not run.")
+    test_passed = PermissibleValue(text="test_passed")
+    test_failed = PermissibleValue(text="test_failed")
+    test_skipped = PermissibleValue(text="test_skipped")
 
     _defn = EnumDefinition(
         name="TestCaseResultEnum",
     )
 
 # Slots
 class slots:
@@ -1411,16 +1449,19 @@
 
 slots.in_v1 = Slot(uri=TTM.in_v1, name="in_v1", curie=TTM.curie('in_v1'),
                    model_uri=TTM.in_v1, domain=None, range=Optional[Union[bool, Bool]])
 
 slots.well_known = Slot(uri=TTM.well_known, name="well_known", curie=TTM.curie('well_known'),
                    model_uri=TTM.well_known, domain=None, range=Optional[Union[bool, Bool]])
 
-slots.test_runner_settings = Slot(uri=TTM.test_runner_settings, name="test_runner_settings", curie=TTM.curie('test_runner_settings'),
-                   model_uri=TTM.test_runner_settings, domain=None, range=Optional[Union[str, List[str]]])
+slots.runner_settings = Slot(uri=TTM.runner_settings, name="runner_settings", curie=TTM.curie('runner_settings'),
+                   model_uri=TTM.runner_settings, domain=None, range=Union[str, List[str]])
+
+slots.test_case_runner_settings = Slot(uri=TTM.test_case_runner_settings, name="test_case_runner_settings", curie=TTM.curie('test_case_runner_settings'),
+                   model_uri=TTM.test_case_runner_settings, domain=None, range=Union[str, List[str]])
 
 slots.must_pass_date = Slot(uri=TTM.must_pass_date, name="must_pass_date", curie=TTM.curie('must_pass_date'),
                    model_uri=TTM.must_pass_date, domain=None, range=Optional[Union[str, XSDDate]])
 
 slots.must_pass_environment = Slot(uri=TTM.must_pass_environment, name="must_pass_environment", curie=TTM.curie('must_pass_environment'),
                    model_uri=TTM.must_pass_environment, domain=None, range=Optional[Union[str, "TestEnvEnum"]])
 
@@ -1475,15 +1516,15 @@
 slots.test_data_file_locator = Slot(uri=TTM.test_data_file_locator, name="test_data_file_locator", curie=TTM.curie('test_data_file_locator'),
                    model_uri=TTM.test_data_file_locator, domain=None, range=Optional[Union[str, URIorCURIE]])
 
 slots.test_data_file_format = Slot(uri=TTM.test_data_file_format, name="test_data_file_format", curie=TTM.curie('test_data_file_format'),
                    model_uri=TTM.test_data_file_format, domain=None, range=Optional[Union[str, "FileFormatEnum"]])
 
 slots.test_metadata = Slot(uri=TTM.test_metadata, name="test_metadata", curie=TTM.curie('test_metadata'),
-                   model_uri=TTM.test_metadata, domain=None, range=Optional[Union[dict, TestMetadata]])
+                   model_uri=TTM.test_metadata, domain=None, range=Union[dict, TestMetadata])
 
 slots.test_persona = Slot(uri=TTM.test_persona, name="test_persona", curie=TTM.curie('test_persona'),
                    model_uri=TTM.test_persona, domain=None, range=Optional[Union[str, "TestPersonaEnum"]])
 
 slots.test_cases = Slot(uri=TTM.test_cases, name="test_cases", curie=TTM.curie('test_cases'),
                    model_uri=TTM.test_cases, domain=None, range=Optional[Union[Dict[Union[str, TestCaseId], Union[dict, TestCase]], List[Union[dict, TestCase]]]])
 
@@ -1519,24 +1560,24 @@
 
 slots.TestAsset_id = Slot(uri=SCHEMA.identifier, name="TestAsset_id", curie=SCHEMA.curie('identifier'),
                    model_uri=TTM.TestAsset_id, domain=TestAsset, range=Union[str, TestAssetId])
 
 slots.TestAsset_tags = Slot(uri=SCHEMA.additionalType, name="TestAsset_tags", curie=SCHEMA.curie('additionalType'),
                    model_uri=TTM.TestAsset_tags, domain=TestAsset, range=Optional[Union[str, List[str]]])
 
-slots.TestAsset_test_runner_settings = Slot(uri=TTM.test_runner_settings, name="TestAsset_test_runner_settings", curie=TTM.curie('test_runner_settings'),
-                   model_uri=TTM.TestAsset_test_runner_settings, domain=TestAsset, range=Optional[Union[str, List[str]]])
+slots.TestAsset_runner_settings = Slot(uri=TTM.runner_settings, name="TestAsset_runner_settings", curie=TTM.curie('runner_settings'),
+                   model_uri=TTM.TestAsset_runner_settings, domain=TestAsset, range=Union[str, List[str]])
 
 slots.TestCase_test_assets = Slot(uri=TTM.test_assets, name="TestCase_test_assets", curie=TTM.curie('test_assets'),
                    model_uri=TTM.TestCase_test_assets, domain=TestCase, range=Union[Dict[Union[str, TestAssetId], Union[dict, TestAsset]], List[Union[dict, TestAsset]]])
 
 slots.TestCase_tags = Slot(uri=SCHEMA.additionalType, name="TestCase_tags", curie=SCHEMA.curie('additionalType'),
                    model_uri=TTM.TestCase_tags, domain=TestCase, range=Optional[Union[str, List[str]]])
 
 slots.AcceptanceTestCase_test_assets = Slot(uri=TTM.test_assets, name="AcceptanceTestCase_test_assets", curie=TTM.curie('test_assets'),
                    model_uri=TTM.AcceptanceTestCase_test_assets, domain=AcceptanceTestCase, range=Union[Dict[Union[str, AcceptanceTestAssetId], Union[dict, AcceptanceTestAsset]], List[Union[dict, AcceptanceTestAsset]]])
 
-slots.TestRunSession_test_run_parameters = Slot(uri=TTM.test_run_parameters, name="TestRunSession_test_run_parameters", curie=TTM.curie('test_run_parameters'),
-                   model_uri=TTM.TestRunSession_test_run_parameters, domain=TestRunSession, range=Optional[Union[Union[dict, TestEntityParameter], List[Union[dict, TestEntityParameter]]]])
+slots.TestRunnerConfiguration_tags = Slot(uri=SCHEMA.additionalType, name="TestRunnerConfiguration_tags", curie=SCHEMA.curie('additionalType'),
+                   model_uri=TTM.TestRunnerConfiguration_tags, domain=TestRunnerConfiguration, range=Optional[Union[str, List[str]]])
 
 slots.TestRunSession_test_entities = Slot(uri=TTM.test_entities, name="TestRunSession_test_entities", curie=TTM.curie('test_entities'),
                    model_uri=TTM.TestRunSession_test_entities, domain=TestRunSession, range=Optional[Union[Dict[Union[str, TestEntityId], Union[dict, TestEntity]], List[Union[dict, TestEntity]]]])
```

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/schema/translator_testing_model.yaml` & `translator_testing_model-2.3.0/src/translator_testing_model/schema/translator_testing_model.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 see_also:
   - https://TranslatorSRI.github.io/TranslatorTestingModel
 
 prefixes:
   ttm: https://w3id.org/TranslatorSRI/TranslatorTestingModel/
   linkml: https://w3id.org/linkml/
   biolink: https://w3id.org/biolink/
-  infores: https://w3id.org/biolink/vocab/
   schema: http://schema.org/
   example: https://example.org/
 
 default_prefix: ttm
 default_range: string
 
 imports:
@@ -85,15 +84,14 @@
     abstract: true
     tree_root: true
     slots:
       - id
       - name
       - description
       - tags
-      - test_runner_settings
 
   TestMetadata:
     description: >-
       Represents metadata related to (external SME, SMURF, Translator feedback, 
       large scale batch, etc.) like the provenance of test assets, cases and/or suites.
     is_a: TestEntity
     slots:
@@ -105,16 +103,16 @@
   #####################
   # Test Asset Models #
   #####################
 
   TestAsset:
     description: >-
       Represents a Test Asset, which is a single specific instance of
-      TestCase-agnostic semantic parameters representing the specification
-      of a Translator test target with inputs and (expected) outputs.
+      TestCase-agnostic semantic parameters representing the
+      specification of a Translator test target with inputs and (expected) outputs.
     is_a: TestEntity
     slots:
       - input_id
       - input_name
       - input_category
       - predicate_id
       - predicate_name
@@ -125,26 +123,27 @@
       - qualifiers
       - expected_output
       - test_issue
       - semantic_severity
       - in_v1
       - well_known
       - test_reference
+      - runner_settings
       - test_metadata
     slot_usage:
       id:
         aliases: ["AssetIdentifier"]
         range: uriorcurie
       tags:
         description: >-
           One or more 'tags' slot values (inherited from TestEntity) should generally
           be defined to specify TestAsset membership in a "Block List" collection
-      test_runner_settings:
+      runner_settings:
         description: >-
-          Scalar settings for the TestRunner, e.g. "inferred"
+          Settings for the test harness, e.g. "inferred"
 
   AcceptanceTestAsset:
     is_a: TestAsset
     description: >-
       Model derived from Jenn's test asset design and Shervin's runner JSON here as an example.
     slots:
       - must_pass_date
@@ -187,28 +186,26 @@
     description: >-
       Represents a single enumerated instance of Test Case, derived from a 
       given collection of one or more TestAsset instances (the value of the
       'test_assets' slot) which define the 'inputs' and 'outputs' of the
       TestCase, used to probe a particular test condition.
     is_a: TestEntity
     slots:
+      - test_env
       - query_type
       - test_assets
       - preconditions
       - trapi_template
+      - components
       - test_case_objective
       - test_case_source
       - test_case_predicate_name
       - test_case_predicate_id
       - test_case_input_id
-      - qualifiers
-      - input_category
-      - output_category
-      - components
-      - test_env
+      - test_case_runner_settings
     slot_usage:
       test_assets:
         aliases: ["Block List"]
         description: >-
           One or more 'tags' slot values (inherited from TestEntity)
           should generally be defined as filters to specify TestAsset
           membership in 'test_assets' slot ("Block List") collection.
@@ -229,14 +226,40 @@
     is_a: TestCase
     description: >-
       Assumed additional model from Shervin's runner JSON here as an example.  This schema is not yet complete.
     slot_usage:
 #      test_assets:
 #        range: QuantitativeTestAsset
 
+  ComplianceTestCase:
+    is_a: TestCase
+    description: >-
+      TRAPI and Biolink Model standards compliance test
+    slots:
+      - trapi_version
+      - biolink_version
+    slot_usage:
+#      test_assets:
+#        range: ComplianceTestAsset
+
+  KnowledgeGraphNavigationTestCase:
+    is_a: TestCase
+    description: >-
+      Knowledge Graph navigation integration test
+    slot_usage:
+#      test_assets:
+#        range: KnowledgeGraphNavigationTestAsset
+
+  OneHopTestCase:
+    is_a: KnowledgeGraphNavigationTestCase
+    description: >-
+      'One Hop' Knowledge Graph navigation integration test
+    slot_usage:
+#      test_assets:
+#        range: OneHopTestAsset
 
   #####################
   # Test Suite Models #
   #####################
 
   TestSuiteSpecification:
     description: >-
@@ -277,47 +300,50 @@
       Test case for testing the integrity of "One Hop" knowledge graph retrievals sensa legacy SRI_Testing harness.
     is_a: TestSuite
 
   #####################
   # TestRunner Models #
   #####################
 
+  TestRunnerConfiguration:
+    description: >-
+      General configuration parameters and test data input 
+      for a single invocation of a TestRunner.
+    is_a: TestEntity
+    slots:
+      - test_run_parameters
+    slot_usage:
+      tags:
+        description: >-
+          One or more 'tags' slot values (slot inherited from TestEntity) 
+          should generally identify the TestRunner(s) using this configuration.
+
   TestCaseResult:
     description: >-
       The outcome of a TestRunner run of one specific TestCase.
     is_a: TestEntity
     slots:
       - test_suite_id
       - test_case
       - test_case_result
 
   TestRunSession:
     description: >-
-      Single run of a TestRunner in a given environment, with a specified
-      set of test_entities (generally, one or more instances of TestSuite).
+      A single invocation of a TestRunner.
     is_a: TestEntity
     slots:
-      - components
-      - test_env
       - test_runner_name
-      - test_run_parameters
       - test_entities
       - test_case_results
       - timestamp
     slot_usage:
-      test_run_parameters:
-        description: >-
-          Different TestRunners could expect additional global test
-          configuration parameters, like the applicable TRAPI version
-          ("trapi_version") or Biolink Model versions ("biolink_version").
       test_entities:
         description: >-
-          Different TestRunners could expect specific kinds of TestEntity
-          as an input.  These 'test_entities' are one or more instances of
-          TestAsset, TestCase or (preferably?) TestSuite.
+          Different TestRunners may expect specific kinds of TestEntity as input.
+          These 'test_entities' one or more instances of TestAsset, TestCase or TestSuite.
 
   TestOutput:
     description: >-
       The output of a TestRunner run of one specific TestCase.
     is_a: TestEntity
     slots:
       - test_case_id
@@ -377,15 +403,15 @@
 
   value:
     description: >-
       (String) value of a TestParameter.
 
   test_entity_parameters:
     description: >-
-      One or more 'tag = value' parameters documenting target characteristics of a TestEntity.
+      One or more parameters documenting target characteristics of a TestEntity.
     range: TestEntityParameter
     multivalued: true
     inlined: true
     inlined_as_list: true
 
   timestamp:
     description: >-
@@ -424,21 +450,21 @@
     description: >-
       Document URL where original test source particulars are registered (e.g. Github repo)
     range: uriorcurie
 
   test_objective:
     description: >-
       Testing objective behind specified set of test particulars
-      (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)
+      (e.g. acceptance pass/fail; benchmark; quantitative)
     range: TestObjectiveEnum
 
   test_case_objective:
     description: >-
       Testing objective behind specified set of test particulars
-      (e.g. acceptance pass/fail; benchmark; quantitative; standards compliance; graph navigation integrity)
+      (e.g. acceptance pass/fail; benchmark; quantitative)
     range: TestObjectiveEnum
 
   test_case_source:
     description: >-
       Provenance of a specific set of test assets, cases and/or suites.  Or, the person who cares about this, 
       know about this.  We would like this to be an ORCID eventually, but currently it is just a string.
     range: TestSourceEnum
@@ -549,21 +575,29 @@
     aliases: ["In v1"]
     range: boolean
 
   well_known:
     aliases: ["Well Known"]
     range: boolean
 
-  test_runner_settings:
+  runner_settings:
     aliases: ["Settings"]
     description: >-
-      Scalar parameters for the TestRunner processing a given TestEntity.
+      Settings for the test harness for TestAsset
     range: string
     multivalued: true
-    required: false
+    required: true
+
+  test_case_runner_settings:
+    aliases: ["Settings"]
+    description: >-
+      Settings for the test harness for TestCase
+    range: string
+    multivalued: true
+    required: true
 
   must_pass_date:
     description: >-
       The date by which this test must pass
     range: date
     examples:
       - value: "2023-09-01"
@@ -710,15 +744,15 @@
     range: FileFormatEnum
 
   test_metadata:
     description: >-
       Test metadata describes the external provenance, cross-references and objectives for a given test.
     range: TestMetadata
     inlined: true
-    required: false
+    required: true
 
   test_persona:
     description: >-
       A Test persona describes the user or operational context of a given test.
     range: TestPersonaEnum
 
   test_cases:
@@ -740,16 +774,16 @@
 
   ####################
   # TestRunner Slots #
   ####################
 
   test_run_parameters:
     description: >-
-      TestRunSession parameters informing a TestHarness about
-      the global characteristics of TestRunner processing tests.
+      Parameters for TestRunnerConfiguration that inform the TestHarness
+      and TestRunners about the general characteristics of a test run.
     is_a: test_entity_parameters
 
   test_suite_id:
     description: >-
       CURIE id of a TestSuite registered in the system.
     range: uriorcurie
 
@@ -827,18 +861,14 @@
     permissible_values:
       AcceptanceTest:
         description: Acceptance (pass/fail) test
       BenchmarkTest:
         description: Semantic benchmarking
       QuantitativeTest:
         description: Quantitative test
-      StandardsValidationTest:
-        description: Release-specific TRAPI and Biolink Model ("reasoner-validator") compliance validation
-      OneHopTest:
-        description: Knowledge graph "One Hop" query navigation integrity
 
   TestEnvEnum:
     description: >-
       Testing environments within which a TestSuite is
       run by a TestRunner scheduled by the TestHarness.
     permissible_values:
       dev:
@@ -946,91 +976,19 @@
       three_hop:
       drug_treats_rare_disease:
       drug-to-gene:
 
   ComponentEnum:
     description: >-
       Translator components are identified by their InfoRes identifiers.
-    #    reachable_from:
-    #      source_ontology: biolink
-    #      source_nodes:
-    #        - biolink:infores
-    #      include_self:  false
-    permissible_values:
-      ars:
-        description: >-
-          Automatic Relay Service component of Translator
-        meaning: "infores:ncats-ars"
-      # ARA's
-      arax:
-        description: >-
-          ARAX Translator Reasoner
-        meaning: "infores:arax"
-      explanatory:
-        description: >-
-          A Translator Reasoner API for the Explanatory Agent
-        meaning: "infores:explanatory-agent"
-      improving:
-        description: >-
-          imProving Agent OpenAPI TRAPI Specification
-        meaning: "infores:improving-agent"
-      aragorn:
-        description: >-
-          Performs a query operation which compiles data from numerous ranking agent services.
-        meaning: "infores:aragorn"
-      bte:
-        description: >-
-          BioThings Explorer
-        meaning: "infores:biothings-explorer"
-      unsecret:
-        description: >-
-          Unsecret Agent OpenAPI for NCATS Biomedical Translator Reasoners
-        meaning: "infores:unsecret-agent"
-      # KP's
-      rtxkg2:
-        description: >-
-          TRAPI endpoint for the NCATS Biomedical Translator KP called RTX KG2
-        meaning: "infores:rtx-kg2"
-      icees:
-        description: >-
-          ICEES (Integrated Clinical and Environmental Exposures Service)
-        meaning: "infores:icees-kg"
-      cam:
-        description: >-
-          Causal Activity Model KP
-        meaning: "infores:cam-kp"
-      spoke:
-        description: >-
-          SPOKE KP - an NIH NCATS Knowledge Provider to expose UCSFs SPOKE
-        meaning: "infores:spoke"
-      molepro:
-        description: >-
-          Molecular Data Provider for NCATS Biomedical Translator Reasoners
-        meaning: "infores:molepro"
-      textmining:
-        description: >-
-          Text Mining KP
-        meaning: "infores:textmining-kp"
-      cohd:
-        description: >-
-          Columbia Open Health Data (COHD)
-        meaning: "infores:cohd"
-      openpredict:
-        description: >-
-          OpenPredict API
-        meaning: "infores:openpredict"
-      collaboratory:
-        description: >-
-          Translator Knowledge Collaboratory API
-        meaning: "infores:knowledge-collaboratory"
-      connections:
-        description: >-
-          Connections Hypothesis Provider API
-        meaning: "infores:connections-hypothesis"
-
+    reachable_from:
+      source_ontology: biolink
+      source_nodes:
+        - biolink:infores
+      include_self:  false
 
   #########################
   # TestSuite Model Enums #
   #########################
 
   TestPersonaEnum:
     description: >-
@@ -1050,13 +1008,10 @@
 
   ##########################
   # TestRunner Model Enums #
   ##########################
 
   TestCaseResultEnum:
     permissible_values:
-      PASSED:
-        description: test case result indicating success.
-      FAILED:
-        description: test case result indicating failure.
-      SKIPPED:
-        description: test case result indicating that the specified test was not run.
+      test_passed:
+      test_failed:
+      test_skipped:
```

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/scripts/GitHub_issue_parser.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/GitHub_issue_parser.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/scripts/generate_suite_for_demo.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/generate_suite_for_demo.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-from urllib import response
-
 from src.translator_testing_model.datamodel.pydanticmodel import TestAsset, TestCase, TestSuite, TestMetadata, Qualifier
 import csv
 import json
 import requests
 import yaml
 import bmt
-
 toolkit = bmt.Toolkit()
-import enum
-
-
-class SuiteNames(enum.Enum):
-    pass_fail = "pass_fail"
-    quantitative = "quantitative"
-    full = "full"
 
 
 def retrieve_predicate_mapping():
     # URL of the YAML file
     predicate_mapping_url = "https://w3id.org/biolink/predicate_mapping.yaml"
 
     # Fetch the content of the YAML file
@@ -49,129 +39,136 @@
         reader = csv.DictReader(tsvfile, delimiter='\t')
 
         # Convert the reader into a list of dictionaries
         return list(reader)
 
 
 # Functions to create TestAssets, TestCases, and TestSuite
-def create_test_assets_from_tsv(test_assets: list, suite_name: SuiteNames, toolkit):
+def create_test_assets_from_tsv(test_assets):
     assets = []
     for row in test_assets:
-        if row.get("Relationship") == "" or row.get("OutputID") == "" or row.get("InputID") == "":
-            print("Skipping row with missing relationship, input or output ID", row.get("id"))
+        if row.get("Relationship") == "":
             continue
-        if suite_name == SuiteNames.pass_fail:
-            if get_expected_output(row) != "TopAnswer" and get_expected_output(row) != "NeverShow":
-                continue
-            else:
-                ta = create_test_asset(row, toolkit)
-                assets.append(ta)
 
+        converted_predicate = None
+        biolink_qualified_predicate = ""
+        biolink_object_aspect_qualifier = ""
+        biolink_object_direction_qualifier = ""
+        specified_predicate = row.get("Relationship").lower().strip()
+        if specified_predicate == "decreases abundance or activity of":
+            specified_predicate = "decreases activity or abundance of"
+            print("specified predicate", specified_predicate)
+        if toolkit.get_element(specified_predicate) is not None:
+            converted_predicate = toolkit.get_element(specified_predicate).name
+            converted_predicate = converted_predicate.replace(" ", "_")
+            print("converted predicate", specified_predicate)
         else:
-            ta = create_test_asset(row, toolkit)
+            pred_mapping = toolkit.pmap
+            for collct in pred_mapping.values():
+                for map_item in collct:
+                    if map_item.get("mapped predicate") == specified_predicate:
+                        print("mapped it", map_item.get("mapped predicate"))
+                        converted_predicate = map_item.get("predicate")
+                        converted_predicate = converted_predicate.replace(" ", "_")
+                        biolink_object_aspect_qualifier = map_item.get("object aspect qualifier")
+                        biolink_object_direction_qualifier = map_item.get("object direction qualifier")
+                        biolink_qualified_predicate = "biolink:"+map_item.get("qualified predicate")
+
+        if row.get("Expected Result / Suggested Comparator") == "4_NeverShow":
+            expected_output = "NeverShow"
+        elif row.get("Expected Result / Suggested Comparator") == "3_BadButForgivable":
+            expected_output = "BadButForgivable"
+        elif row.get("Expected Result / Suggested Comparator") == "2_Acceptable":
+            expected_output = "Acceptable"
+        elif row.get("Expected Result / Suggested Comparator") == "1_TopAnswer":
+            expected_output = "TopAnswer"
+        elif row.get("Expected Result / Suggested Comparator") == "5_OverlyGeneric":
+            expected_output = "OverlyGeneric"
+        else:
+            print(f"{row.get('id')} has invalid expected output")
+            print(row.get("Expected Result / Suggested Comparator"))
+            continue
+        output_category = None
+        input_category = None
+        if row.get("InputID").startswith("NCBIGene:"):
+            input_category = 'biolink:Gene'
+
+        chem_prefixes = toolkit.get_element("chemical entity").id_prefixes
+
+        if any(row.get("InputID").startswith(prefix) for prefix in chem_prefixes):
+            input_category = 'biolink:ChemicalEntity'
+        if row.get("InputID").startswith("MONDO:"):
+            input_category = 'biolink:Disease'
+        if row.get("InputID").startswith("UBERON:"):
+            input_category = 'biolink:AnatomicalEntity'
+        if row.get("InputID").startswith("HP:"):
+            input_category = 'biolink:PhenotypicFeature'
+        if any(row.get("OutputID").startswith(prefix) for prefix in chem_prefixes):
+            output_category = 'biolink:ChemicalEntity'
+        if row.get("OutputID").startswith("MONDO:"):
+            output_category = 'biolink:Disease'
+        if row.get("OutputID").startswith("UBERON:"):
+            output_category = 'biolink:AnatomicalEntity'
+        if row.get("OutputID").startswith("HP:"):
+            output_category = 'biolink:PhenotypicFeature'
+        if row.get("OutputID").startswith("DRUGBANK:"):
+            output_category = 'biolink:ChemicalEntity'
+
+        print(converted_predicate, row, expected_output)
+        ta = TestAsset(id=row.get("id").replace(":", "_"),
+                       name=expected_output + ': ' + row.get("OutputName").strip() +" "+ row.get("Relationship").strip().lower() +" "+ row.get("InputName").strip(),
+                       description=expected_output + ': ' + row.get("OutputName").strip() +" "+ row.get("Relationship").strip().lower() +" "+ row.get("InputName").strip(),
+                       input_id=row.get("InputID").strip(),
+                       predicate_name=converted_predicate,
+                       predicate_id="biolink:"+converted_predicate,
+                       output_id=row.get("OutputID").strip(),
+                       output_name=row.get("OutputName").strip(),
+                       output_category=output_category,
+                       expected_output=expected_output.strip(),
+                       test_metadata=TestMetadata(id=1),
+                       input_category=input_category,
+                       )
+        ta.input_name = row.get("InputName").strip()
+        if row.get("Translator GitHubIssue") != "" and row.get("Translator GitHubIssue") is not None:
+            tmd = TestMetadata(id=1,
+                               test_source="SMURF",
+                               test_reference=row.get("Translator GitHubIssue").strip(),
+                               test_objective="AcceptanceTest")
+            ta.test_metadata = tmd
+        else:
+            tmd = TestMetadata(id=1,
+                               test_source="SMURF",
+                               test_objective="AcceptanceTest")
+            ta.test_metadata = tmd
+        ta.runner_settings = [row.get("Settings").lower()]
+
+        if biolink_qualified_predicate != "":
+            qp = Qualifier(parameter="biolink_qualified_predicate",
+                           value=biolink_qualified_predicate)
+            oaq = Qualifier(parameter="biolink_object_aspect_qualifier",
+                            value=biolink_object_aspect_qualifier.replace(" ", "_"))
+            odq = Qualifier(parameter="biolink_object_direction_qualifier",
+                            value=biolink_object_direction_qualifier)
+            qualifiers = [qp, oaq, odq]
+
+            ta.qualifiers=qualifiers
+        if row.get("Well Known") == "yes":
+            ta.well_known = True
+        else:
+            ta.well_known = False
         assets.append(ta)
-    return assets
-
-
-def get_converted_predicate(specified_predicate, toolkit):
-    if specified_predicate == "decreases abundance or activity of":
-        specified_predicate = "decreases activity or abundance of"
-    element = toolkit.get_element(specified_predicate)
-    if element is not None:
-        return element.name.replace(" ", "_"), "", "", "biolink:" + element.name
-    else:
-        for collection in toolkit.pmap.values():
-            for item in collection:
-                if item.get("mapped predicate") == specified_predicate:
-                    return (
-                        item.get("predicate").replace(" ", "_"),
-                        item.get("object aspect qualifier"),
-                        item.get("object direction qualifier"),
-                        "biolink:" + item.get("qualified predicate"),
-                    )
-    return specified_predicate, "", "", ""
-
-
-def get_category(prefixes, id):
-    if id.startswith("NCBIGene:"):
-        return 'biolink:Gene'
-    elif id.startswith("MONDO:"):
-        return 'biolink:Disease'
-    elif id.startswith("UBERON:"):
-        return 'biolink:AnatomicalEntity'
-    elif id.startswith("HP:"):
-        return 'biolink:PhenotypicFeature'
-    elif id.startswith("DRUGBANK:") or id.startswith("CHEBI:") or any(id.startswith(prefix) for prefix in prefixes):
-        return 'biolink:ChemicalEntity'
-    return None
-
-
-def get_expected_output(row):
-    output = row.get("Expected Result / Suggested Comparator")
-    if output in ["4_NeverShow", "3_BadButForgivable", "2_Acceptable", "1_TopAnswer", "5_OverlyGeneric"]:
-        return output.split("_")[1]
-    print(f"{row.get('id')} has invalid expected output: {output}")
-    return None
-
-
-def create_test_asset(row, toolkit):
-    specified_predicate = row.get("Relationship").lower().strip()
-    converted_predicate, biolink_object_aspect_qualifier, biolink_object_direction_qualifier, biolink_qualified_predicate = get_converted_predicate(specified_predicate, toolkit)
-
-    expected_output = get_expected_output(row)
-    if not expected_output:
-        return None
-
-    chem_prefixes = toolkit.get_element("chemical entity").id_prefixes
-    input_category = get_category(chem_prefixes, row.get("InputID"))
-    output_category = get_category(chem_prefixes, row.get("OutputID"))
-
-    ta = TestAsset(
-        id=row.get("id").replace(":", "_"),
-        name=f"{expected_output}: {row.get('OutputName').strip()} {specified_predicate} {row.get('InputName').strip()}",
-        description=f"{expected_output}: {row.get('OutputName').strip()} {specified_predicate} {row.get('InputName').strip()}",
-        input_id=row.get("InputID").strip(),
-        predicate_name=converted_predicate,
-        predicate_id=f"biolink:{converted_predicate}",
-        output_id=row.get("OutputID").strip(),
-        output_name=row.get("OutputName").strip(),
-        output_category=output_category,
-        expected_output=expected_output.strip(),
-        test_metadata=TestMetadata(
-            id=1,
-            test_source="SMURF",
-            test_reference=row.get("Translator GitHubIssue").strip() if row.get("Translator GitHubIssue") else None,
-            test_objective="AcceptanceTest"
-        ),
-        input_category=input_category,
-    )
-    ta.input_name = row.get("InputName").strip()
-    ta.test_runner_settings = [row.get("Settings").lower()]
-
-    if biolink_qualified_predicate:
-        ta.qualifiers = [
-            Qualifier(parameter="biolink_qualified_predicate", value=biolink_qualified_predicate),
-            Qualifier(parameter="biolink_object_aspect_qualifier", value=biolink_object_aspect_qualifier.replace(" ", "_")),
-            Qualifier(parameter="biolink_object_direction_qualifier", value=biolink_object_direction_qualifier),
-        ]
 
-    ta.well_known = row.get("Well Known") == "yes"
-
-    return ta
+    return assets
 
 
 def create_test_cases_from_test_assets(test_assets, test_case_model):
     # Group test assets based on input_id and relationship
     grouped_assets = {}
     for test_asset in test_assets:
-        qualifier_key = ""
-        if test_asset.qualifiers and test_asset.qualifiers is not None:
-            for qualifier in test_asset.qualifiers:
-                qualifier_key = qualifier_key+qualifier.value
-        key = (test_asset.input_id, test_asset.predicate_name, qualifier_key)
+        key = (test_asset.input_id, test_asset.predicate_name)
         if key not in grouped_assets:
             grouped_assets[key] = []
         grouped_assets[key].append(test_asset)
 
     # Create test cases from grouped test assets
     test_cases = []
     for idx, (key, assets) in enumerate(grouped_assets.items()):
@@ -180,194 +177,115 @@
         test_case = test_case_model(id=test_case_id,
                                     name="what " + key[1] + " " + key[0],
                                     description=descriptions,
                                     test_env="ci",
                                     components=["ars"],
                                     test_case_objective="AcceptanceTest",
                                     test_assets=assets,
-                                    test_runner_settings=["inferred"]
+                                    test_case_runner_settings=["inferred"]
                                     )
         if test_case.test_assets is None:
             print("test case has no assets", test_case)
 
         if test_case.test_case_objective == "AcceptanceTest":
             test_input_id = ""
             test_case_predicate_name = ""
-            test_case_qualifiers = []
-            input_category = ""
-            output_category = ""
             for asset in assets:
-                # these all assume group by applies to the same input_id and predicate_name
                 test_input_id = asset.input_id
                 test_case_predicate_name = asset.predicate_name
-                test_case_qualifiers = asset.qualifiers
-                input_category = asset.input_category
-                output_category = asset.output_category
 
             test_case.test_case_input_id = test_input_id
             test_case.test_case_predicate_name = test_case_predicate_name
             test_case.test_case_predicate_id = "biolink:" + test_case_predicate_name
-            test_case.qualifiers = test_case_qualifiers
-            test_case.input_category = input_category
-            test_case.output_category = output_category
             test_cases.append(test_case)
 
     return test_cases
 
 
 def create_test_suite_from_test_cases(test_cases, test_suite_model):
     test_suite_id = "TestSuite_1"
     test_cases_dict = {test_case.id: test_case for test_case in test_cases}
-
-    ci_test_case_collection = []
-    stress_test_case_collection = []
-
-    for i in range(len(test_cases)):
-        if i % 10 == 9:  # If the index is a multiple of 10 (accounting for 0-indexing)
-            ci_test_case_collection.append(test_cases[i])
-        if i % 2 == 1:    # If the index is a multiple of 5 (accounting for 0-indexing)
-            stress_test_case_collection.append(test_cases[i])
-    test_cases_dict_ci = {test_case.id: test_case for test_case in ci_test_case_collection}
-    test_cases_dict_stress = {test_case.id: test_case for test_case in stress_test_case_collection}
-    print(len(stress_test_case_collection), "number_stress")
-    print(len(test_cases_dict_ci), "number_ci")
-    print(len(test_cases_dict), "number_total")
-
-    # CI and DELTA have the same
-    # number: https://docs.google.com/document/d/1UNX7Z4Wjwg0FPA58VBNMYducNCq44LykzQ6_JU7FEEo/edit
-    print(len(test_cases_dict_ci), "number_delta")
-
     tmd = TestMetadata(id=1,
-                       test_source="SMURF",
-                       test_objective="AcceptanceTest")
-
-    test_suite_ci_id = "TestSuite_2"
-    ci_tmd = TestMetadata(id=2,
                           test_source="SMURF",
                           test_objective="AcceptanceTest")
+    return test_suite_model(id=test_suite_id, test_cases=test_cases_dict, test_metadata=tmd)
+
+
+if __name__ == '__main__':
+
+    # Reading the TSV file
+    tsv_file_path = 'pf_test_assets_031524.tsv'
+    tsv_data = parse_tsv(tsv_file_path)
+    print(tsv_data[0])
 
+    # Create TestAsset objects
+    test_assets = create_test_assets_from_tsv(tsv_data)
+    for asset in test_assets:
+        if asset.test_metadata is None or asset.test_metadata == "":
+            print(asset)
 
-    test_suite_stress_id = "TestSuite_3"
-    stress_tmd = TestMetadata(id=3,
-                              test_source="SMURF",
-                              test_objective="AcceptanceTest")
-
-    test_suite_delta_id = "TestSuite_4"
-    delta_tmd = TestMetadata(id=4,
-                             test_source="SMURF",
-                             test_objective="AcceptanceTest")
-
-    return (test_suite_model(id=test_suite_id, test_cases=test_cases_dict, test_metadata=tmd),
-            test_suite_model(id=test_suite_ci_id, test_cases=test_cases_dict_ci, test_metadata=ci_tmd),
-            test_suite_model(id=test_suite_stress_id, test_cases=test_cases_dict_stress, test_metadata=stress_tmd),
-            test_suite_model(id=test_suite_delta_id, test_cases=test_cases_dict_ci, test_metadata=delta_tmd))
+    # Create TestCase objects
+    test_cases = create_test_cases_from_test_assets(test_assets, TestCase)
+    for case in test_cases:
+        if case.test_assets is None or case.test_assets == "":
+            print(case)
+    #
 
+    for i, item in enumerate(test_cases):
+        file_prefix = item.id
+        filename = f"{file_prefix}.json"
+        with open(filename, 'w', encoding='utf-8') as file:
+            json.dump(item.dict(), file, ensure_ascii=False, indent=4)
+
+    for i, item in enumerate(test_assets):
+        file_prefix = item.id
+        filename = f"{file_prefix}.json"
+        with open(filename, 'w', encoding='utf-8') as file:
+            json.dump(item.dict(), file, ensure_ascii=False, indent=4)
 
-def create_benchmark_test_case(subset: bool) -> TestCase or list[TestCase]:
     url = 'https://raw.githubusercontent.com/TranslatorSRI/Benchmarks/main/benchmarks_runner/config/benchmarks.json'
-    benchmark_cases = []
+
     # Send a GET request to the URL
     response = requests.get(url)
 
     # Check if the request was successful
     if response.status_code == 200:
         # Parse the response content as JSON
         data = response.json()
         for k, v in data.items():
             tmd = TestMetadata(id=1,
                                test_source="SMURF",
                                test_objective="QuantitativeTest")
-            test_asset = TestAsset(id=k,
-                                   name=k,
-                                   description=k,
-                                   test_metadata=tmd
-                                   )
-            test_case = TestCase(id=k,
-                                 name=k,
-                                 description=k,
-                                 test_assets=[test_asset],
-                                 test_env="ci",
-                                 components=["ars"],
-                                 test_case_objective="QuantitativeTest",
-                                 test_runner_settings=["limit_queries"]
-                                 )
+            ta = TestAsset(id=k,
+                            name=k,
+                            description=k,
+                            test_metadata=tmd
+                            )
+            tc = TestCase(id=k,
+                          name=k,
+                          description=k,
+                          test_assets=[ta],
+                          test_env="ci",
+                          components=["ars"],
+                          test_case_objective="QuantitativeTest",
+                          test_case_runner_settings=["limit_queries"]
+                          )
             file_prefix = k
-            if subset and k.startswith("DrugCentral_subset"):
-                benchmark_cases.append(test_case)
-                filename = f"{file_prefix}.json"
-                with open(filename, 'w', encoding='utf-8') as file:
-                    json.dump(test_case.dict(), file, ensure_ascii=False, indent=4)
-                return test_case
-            else:
-                filename = f"{file_prefix}.json"
-                with open(filename, 'w', encoding='utf-8') as file:
-                    json.dump(test_case.dict(), file, ensure_ascii=False, indent=4)
-                benchmark_cases.append(test_case)
-        return benchmark_cases
+            if k.startswith("DrugCentral_subset"):
+                test_cases.append(tc)
+            filename = f"{file_prefix}.json"
+            with open(filename, 'w', encoding='utf-8') as file:
+                json.dump(tc.dict(), file, ensure_ascii=False, indent=4)
 
     else:
         print(f'Failed to retrieve the file. Status code: {response.status_code}')
 
-
-def dump_to_json(file_prefix):
-    filename = f"{file_prefix.id}.json"
-    with open(filename, 'w', encoding='utf-8') as file:
-        json.dump(file_prefix.dict(), file, ensure_ascii=False, indent=4)
-
-
-if __name__ == '__main__':
-
-    # Reading the TSV file
-    tsv_file_path = 'pf_test_assets_032224.tsv'
-    tsv_data = parse_tsv(tsv_file_path)
-
-    # Create TestAsset objects
-    pf_test_assets = create_test_assets_from_tsv(tsv_data, SuiteNames.pass_fail, toolkit)
-
-    # Create TestCase objects
-    test_cases = create_test_cases_from_test_assets(pf_test_assets, TestCase)
-
-    for i, item in enumerate(test_cases):
-        identifier = item.id
-        dump_to_json(item)
-
-    for i, item in enumerate(pf_test_assets):
-        identifier = item.id
-        dump_to_json(item)
-
-    # Create Benchmark Test Cases - subset for now
-    benchmark_case = create_benchmark_test_case(subset=True)
-    if isinstance(benchmark_case, list):
-        test_cases.extend(benchmark_case)
-    else:
-        test_cases.append(benchmark_case)
-
     # Assemble into a TestSuite
-    (test_suite_all, test_suite_CI, test_suite_STRESS, test_suite_DELTA) = create_test_suite_from_test_cases(test_cases, TestSuite)
+    test_suite = create_test_suite_from_test_cases(test_cases, TestSuite)
     #
-
     # Convert to JSON and save to file
-    test_suite_json_all = test_suite_all.json(indent=4)
-    test_suite_json_CI = test_suite_CI.json(indent=4)
-    test_suite_json_STRESS = test_suite_STRESS.json(indent=4)
-    test_suite_json_DELTA = test_suite_DELTA.json(indent=4)
+    test_suite_json = test_suite.json(indent=4)
 
-
-    suite_json_output_path = 'semantic_smoke_test_suite_TEST.json'
+    suite_json_output_path = 'test_suite_output.json'
 
     with open(suite_json_output_path, 'w') as file:
-        file.write(test_suite_json_all)
-
-    sst_ci_json_output_path = 'semantic_smoke_test_suite_CI.json'
-
-    with open(sst_ci_json_output_path, 'w') as file:
-        file.write(test_suite_json_CI)
-
-    suite_delta_json_output_path_prod = 'stress_test_PROD.json'
-
-    with open(suite_delta_json_output_path_prod, 'w') as file:
-        file.write(test_suite_json_STRESS)
-
-    suite_delta_json_output_path_prod = 'semantic_delta_and_time_profiling_PROD.json'
-
-    with open(suite_delta_json_output_path_prod, 'w') as file:
-        file.write(test_suite_json_DELTA)
+        file.write(test_suite_json)
```

### Comparing `translator_testing_model-0.3.1/src/translator_testing_model/scripts/test_suite_generator.py` & `translator_testing_model-2.3.0/src/translator_testing_model/scripts/test_suite_generator.py`

 * *Files identical despite different names*

### Comparing `translator_testing_model-0.3.1/PKG-INFO` & `translator_testing_model-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: translator_testing_model
-Version: 0.3.1
+Version: 2.3.0
 Summary: This is the project description.
 License: MIT
 Author: Sierra Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
-Requires-Dist: bioregistry (>=0.11.1,<0.12.0)
-Requires-Dist: bmt (>=1.4.0,<2.0.0)
-Requires-Dist: linkml (>=1.7.8,<2.0.0) ; extra == "docs"
-Requires-Dist: linkml-runtime (>=1.7.5,<2.0.0)
+Requires-Dist: bmt (>=1.2.1,<2.0.0)
+Requires-Dist: linkml (>=1.6.1,<2.0.0) ; extra == "docs"
+Requires-Dist: linkml-runtime (>=1.6.1,<2.0.0)
 Requires-Dist: pandas (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic (>=1.10.13,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Translator Testing Model
 
 This is a preliminary schema repo for defining test cases in Translator that can be reused in different test suites.  e.g. a test case in plain language might be something like _"what drugs may treat MS? I expect fingolimod to return in the top 10 results in less than 5 mins."_  
 
 Capturing these details in metadata that is parsable and usable by test runners is the objective of this schema.  We also want to harmonize our language and nomenclature for the metadata we need (which of these data are required and which are optional for each kind of test case, etc.) so that downstream testing code can utilize a common framework for understanding.
@@ -37,15 +36,16 @@
 * [project/](project/) - project files (do not edit these)
 * [src/](src/translator_testing_model/README.md) - source files (edit these)
   * [translator testing model specification](src/translator_testing_model/README.md)
     * [schema](src/translator_testing_model/schema/translator_testing_model.yaml) -- LinkML schema
       (edit this)
     * [datamodel](src/translator_testing_model/datamodel/README.md) -- generated
       Python datamodels
-      * [Pydantic](src/translator_testing_model/datamodel/pydanticmodel.py) - this is a version 2 model.
+      * [Pydantic V1](src/translator_testing_model/datamodel/pydanticmodel.py)
+      * [Pydantic V2](src/translator_testing_model/datamodel/pydanticmodel_v2.py)
       * [Python Dataclasses](src/translator_testing_model/datamodel/translator_testing_model.py)
 * [tests/](tests/test_data.py) - Python tests
 
 ## Developer Documentation
 
 <details>
 The project uses [Poetry](https://python-poetry.org/) to manage its dependencies. Install Poetry then:
```

