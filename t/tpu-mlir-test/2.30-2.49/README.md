# Comparing `tmp/tpu_mlir_test-2.30-py3-none-any.whl.zip` & `tmp/tpu_mlir_test-2.49-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12148 bytes, number of entries: 10
--rw-r--r--  2.0 unx     2463 b- defN 24-Jan-30 11:37 tpu_mlir_test/__init__.py
--rw-r--r--  2.0 unx     6337 b- defN 24-Jan-30 11:37 tpu_mlir_test/entry.py
--rw-r--r--  2.0 unx     3102 b- defN 24-Jan-30 11:37 tpu_mlir_test/entryconfig.py
--rwxr-xr-x  2.0 unx     1065 b- defN 24-Jan-30 10:52 tpu_mlir_test-2.30.data/scripts/envsetup.sh
--rw-r--r--  2.0 unx     1622 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/LICENSE
--rw-r--r--  2.0 unx    16718 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/WHEEL
--rw-r--r--  2.0 unx     5090 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      860 b- defN 24-Jan-30 11:37 tpu_mlir_test-2.30.dist-info/RECORD
-10 files, 37363 bytes uncompressed, 10672 bytes compressed:  71.4%
+Zip file size: 12152 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     2463 b- defN 24-Apr-26 09:35 tpu_mlir_test/__init__.py
+-rw-r--r--  2.0 unx     6337 b- defN 24-Apr-26 09:35 tpu_mlir_test/entry.py
+-rw-r--r--  2.0 unx     3102 b- defN 24-Apr-26 09:35 tpu_mlir_test/entryconfig.py
+-rwxr-xr-x  2.0 unx     1065 b- defN 24-Apr-26 08:50 tpu_mlir_test-2.49.data/scripts/envsetup.sh
+-rw-r--r--  2.0 unx     1622 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16718 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/WHEEL
+-rw-r--r--  2.0 unx     5090 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      860 b- defN 24-Apr-26 09:35 tpu_mlir_test-2.49.dist-info/RECORD
+10 files, 37363 bytes uncompressed, 10676 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: tpu_mlir_test/entry.py
 Comment: 
 
 Filename: tpu_mlir_test/entryconfig.py
 Comment: 
 
-Filename: tpu_mlir_test-2.30.data/scripts/envsetup.sh
+Filename: tpu_mlir_test-2.49.data/scripts/envsetup.sh
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/LICENSE
+Filename: tpu_mlir_test-2.49.dist-info/LICENSE
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/METADATA
+Filename: tpu_mlir_test-2.49.dist-info/METADATA
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/WHEEL
+Filename: tpu_mlir_test-2.49.dist-info/WHEEL
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/entry_points.txt
+Filename: tpu_mlir_test-2.49.dist-info/entry_points.txt
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/top_level.txt
+Filename: tpu_mlir_test-2.49.dist-info/top_level.txt
 Comment: 
 
-Filename: tpu_mlir_test-2.30.dist-info/RECORD
+Filename: tpu_mlir_test-2.49.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tpu_mlir_test/entry.py

 * *Ordering differences only*

```diff
@@ -1,204 +1,204 @@
 import tpu_mlir_test,os
 from tpu_mlir_test import run_subprocess_c, run_subprocess_py
 
 # f"{package_path}/bin/
+def tpuc_opt():
+	file_name = f"{os.getenv('TPUC_ROOT')}/bin/tpuc-opt"
+	run_subprocess_c(file_name)
+
 def model_tool():
 	file_name = f"{os.getenv('TPUC_ROOT')}/bin/model_tool"
 	run_subprocess_c(file_name)
 
 def cvimodel_debug():
 	file_name = f"{os.getenv('TPUC_ROOT')}/bin/cvimodel_debug"
 	run_subprocess_c(file_name)
 
-def tpuc_opt():
-	file_name = f"{os.getenv('TPUC_ROOT')}/bin/tpuc-opt"
-	run_subprocess_c(file_name)
-
 ### total 3 entry generated for f"{package_path}/bin/
 
 # f"{package_path}/python/tools/
-def gen_shell():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/gen_shell.py"
-	run_subprocess_py(file_name)
-
 def mlir2onnx():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/mlir2onnx.py"
 	run_subprocess_py(file_name)
 
-def fp_forward():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/fp_forward.py"
+def run_calibration():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_calibration.py"
 	run_subprocess_py(file_name)
 
-def bmodel_checker():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmodel_checker.py"
+def model_runner():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_runner.py"
 	run_subprocess_py(file_name)
 
-def model_eval_imagenet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_eval_imagenet.py"
+def assign_output():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/assign_output.py"
 	run_subprocess_py(file_name)
 
-def run_qtable():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_qtable.py"
+def tdb():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/tdb.py"
 	run_subprocess_py(file_name)
 
-def mlir2graph():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/mlir2graph.py"
+def tpu_profile():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/tpu_profile.py"
 	run_subprocess_py(file_name)
 
-def model_deploy():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_deploy.py"
+def bmodel_checker():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmodel_checker.py"
 	run_subprocess_py(file_name)
 
 def mlir_cut():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/mlir_cut.py"
 	run_subprocess_py(file_name)
 
-def model_transform():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_transform.py"
+def run_sensitive_layer():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_sensitive_layer.py"
 	run_subprocess_py(file_name)
 
-def model_eval():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_eval.py"
+def gen_shell():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/gen_shell.py"
 	run_subprocess_py(file_name)
 
-def tpu_profile():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/tpu_profile.py"
+def gen_rand_input():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/gen_rand_input.py"
 	run_subprocess_py(file_name)
 
-def model_runner():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_runner.py"
+def bmodel_dis():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmodel_dis.py"
 	run_subprocess_py(file_name)
 
-def model_inference_cpu():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_inference_cpu.py"
+def model_eval_imagenet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_eval_imagenet.py"
 	run_subprocess_py(file_name)
 
-def assign_output():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/assign_output.py"
+def model_transform():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_transform.py"
 	run_subprocess_py(file_name)
 
-def bmodel_dis():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmodel_dis.py"
+def mlir2graph():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/mlir2graph.py"
 	run_subprocess_py(file_name)
 
-def gen_rand_input():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/gen_rand_input.py"
+def bmrt_test():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmrt_test.py"
 	run_subprocess_py(file_name)
 
-def npz_tool():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/npz_tool.py"
+def model_deploy():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_deploy.py"
 	run_subprocess_py(file_name)
 
-def bmrt_test():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/bmrt_test.py"
+def model_inference_cpu():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_inference_cpu.py"
 	run_subprocess_py(file_name)
 
-def run_sensitive_layer():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_sensitive_layer.py"
+def visual():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/visual.py"
 	run_subprocess_py(file_name)
 
-def tdb():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/tdb.py"
+def model_eval():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/model_eval.py"
 	run_subprocess_py(file_name)
 
-def run_calibration():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_calibration.py"
+def fp_forward():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/fp_forward.py"
 	run_subprocess_py(file_name)
 
-def visual():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/visual.py"
+def run_qtable():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/run_qtable.py"
 	run_subprocess_py(file_name)
 
 def code_stripper():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/code_stripper.py"
 	run_subprocess_py(file_name)
 
+def npz_tool():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/tools/npz_tool.py"
+	run_subprocess_py(file_name)
+
 ### total 24 entry generated for f"{package_path}/python/tools/
 
 # f"{package_path}/python/samples/
-def detect_yolov3():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_yolov3.py"
+def detect_yolov5():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_yolov5.py"
 	run_subprocess_py(file_name)
 
-def detect_ssd_12():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_ssd-12.py"
+def detect_ultraface():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_ultraface.py"
 	run_subprocess_py(file_name)
 
-def detect_pp_yolox():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_yolox.py"
+def classify_LeNet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_LeNet.py"
 	run_subprocess_py(file_name)
 
-def detect_yolov5():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_yolov5.py"
+def classify_shufflenet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_shufflenet.py"
 	run_subprocess_py(file_name)
 
-def classify_inception_v3():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_inception_v3.py"
+def classify_efficientnet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_efficientnet.py"
 	run_subprocess_py(file_name)
 
-def detect_pp_picodet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_picodet.py"
+def classify_xception():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_xception.py"
 	run_subprocess_py(file_name)
 
-def classify_squeezenet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_squeezenet.py"
+def classify_mobilenet_v2():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_mobilenet_v2.py"
 	run_subprocess_py(file_name)
 
-def classify_vgg16():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_vgg16.py"
+def detect_ssd_12():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_ssd-12.py"
 	run_subprocess_py(file_name)
 
-def classify_resnext50():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_resnext50.py"
+def classify_inception_v3():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_inception_v3.py"
 	run_subprocess_py(file_name)
 
-def detect_ultraface():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_ultraface.py"
+def detect_pp_yolox():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_yolox.py"
 	run_subprocess_py(file_name)
 
-def classify_DenseNet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_DenseNet.py"
+def detect_pp_yoloe():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_yoloe.py"
+	run_subprocess_py(file_name)
+
+def classify_resnext50():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_resnext50.py"
+	run_subprocess_py(file_name)
+
+def classify_squeezenet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_squeezenet.py"
 	run_subprocess_py(file_name)
 
 def classify_resnet50():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_resnet50.py"
 	run_subprocess_py(file_name)
 
-def classify_shufflenet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_shufflenet.py"
+def classify_vgg16():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_vgg16.py"
 	run_subprocess_py(file_name)
 
-def detect_retinaface():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_retinaface.py"
+def detect_yolov3():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_yolov3.py"
 	run_subprocess_py(file_name)
 
-def classify_LeNet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_LeNet.py"
+def detect_pp_picodet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_picodet.py"
 	run_subprocess_py(file_name)
 
 def classify_resnet18():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_resnet18.py"
 	run_subprocess_py(file_name)
 
-def detect_pp_yoloe():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_pp_yoloe.py"
-	run_subprocess_py(file_name)
-
-def classify_xception():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_xception.py"
+def detect_retinaface():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/detect_retinaface.py"
 	run_subprocess_py(file_name)
 
 def seg_humanseg():
 	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/seg_humanseg.py"
 	run_subprocess_py(file_name)
 
-def classify_efficientnet():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_efficientnet.py"
-	run_subprocess_py(file_name)
-
-def classify_mobilenet_v2():
-	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_mobilenet_v2.py"
+def classify_DenseNet():
+	file_name = f"{os.getenv('TPUC_ROOT')}/python/samples/classify_DenseNet.py"
 	run_subprocess_py(file_name)
 
 ### total 21 entry generated for f"{package_path}/python/samples/
```

## Comparing `tpu_mlir_test-2.30.data/scripts/envsetup.sh` & `tpu_mlir_test-2.49.data/scripts/envsetup.sh`

 * *Files identical despite different names*

## Comparing `tpu_mlir_test-2.30.dist-info/LICENSE` & `tpu_mlir_test-2.49.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tpu_mlir_test-2.30.dist-info/METADATA` & `tpu_mlir_test-2.49.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tpu_mlir_test
-Version: 2.30
-Summary: Machine learning compiler based on MLIR for Sophgo TPU v2.30-20240130.
+Version: 2.49
+Summary: Machine learning compiler based on MLIR for Sophgo TPU v2.49-20240426.
 Home-page: https://github.com/sophgo/tpu-mlir
 Author: SOPHGO
 Author-email: sales@sophgo.com
 License: 2-Clause BSD
 Keywords: python3.10,unbuntu22.04,linux,tpu-mlir
 Platform: unbuntu22.04
 Classifier: Intended Audience :: Developers
```

## Comparing `tpu_mlir_test-2.30.dist-info/entry_points.txt` & `tpu_mlir_test-2.49.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `tpu_mlir_test-2.30.dist-info/RECORD` & `tpu_mlir_test-2.49.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 tpu_mlir_test/__init__.py,sha256=R8Vtf1AtS8iMa0iV_r_sSFd_nXUtrCBNVYIXjE6klvA,2463
-tpu_mlir_test/entry.py,sha256=PAfMipXsZGn7HQj2KS9eRiUu4HqOK3KR58D5SbElECc,6337
+tpu_mlir_test/entry.py,sha256=OVKtLHq4WKCbwVtB8bqh50t-C1zbfakY6lUiwG8Tw_g,6337
 tpu_mlir_test/entryconfig.py,sha256=fmpOoUp8Nufnsy50RM9O-o6T4_rkLLA0j3S0_cqxCxg,3102
-tpu_mlir_test-2.30.data/scripts/envsetup.sh,sha256=ulfaR67OEc73aOiZjM3lnsiBCaRpMK2xPqSucHFhGXk,1065
-tpu_mlir_test-2.30.dist-info/LICENSE,sha256=BJ3f-ZSv4-KBvvGTUS5gs8MxFPmgTpnhhR1SgxBmYAQ,1622
-tpu_mlir_test-2.30.dist-info/METADATA,sha256=65p1mvaZ5ii-iMWtDYs7stbR67-X22ClX1hRfHQt7UA,16718
-tpu_mlir_test-2.30.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-tpu_mlir_test-2.30.dist-info/entry_points.txt,sha256=3gIv5ia6aWYWjijY08D1Prpnt9cHBE7F_ElE6PMEp2o,5090
-tpu_mlir_test-2.30.dist-info/top_level.txt,sha256=6xTHG0VPaunqlLCMusM6rAS2mNq-SGPC5Xy3rjtDVdo,14
-tpu_mlir_test-2.30.dist-info/RECORD,,
+tpu_mlir_test-2.49.data/scripts/envsetup.sh,sha256=ulfaR67OEc73aOiZjM3lnsiBCaRpMK2xPqSucHFhGXk,1065
+tpu_mlir_test-2.49.dist-info/LICENSE,sha256=BJ3f-ZSv4-KBvvGTUS5gs8MxFPmgTpnhhR1SgxBmYAQ,1622
+tpu_mlir_test-2.49.dist-info/METADATA,sha256=NYNppsU7bHXKGJKki1wk4aNfJ1QYfG27e2yUyvJjcrc,16718
+tpu_mlir_test-2.49.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+tpu_mlir_test-2.49.dist-info/entry_points.txt,sha256=3gIv5ia6aWYWjijY08D1Prpnt9cHBE7F_ElE6PMEp2o,5090
+tpu_mlir_test-2.49.dist-info/top_level.txt,sha256=6xTHG0VPaunqlLCMusM6rAS2mNq-SGPC5Xy3rjtDVdo,14
+tpu_mlir_test-2.49.dist-info/RECORD,,
```

