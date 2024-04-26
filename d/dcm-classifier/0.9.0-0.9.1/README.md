# Comparing `tmp/dcm_classifier-0.9.0.tar.gz` & `tmp/dcm_classifier-0.9.1.tar.gz`

## Comparing `dcm_classifier-0.9.0.tar` & `dcm_classifier-0.9.1.tar`

### file list

```diff
@@ -1,619 +1,621 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.git
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.gitattributes
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/push_pip.sh
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/requirements_dev.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.github/workflows/push_to_main.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/EndNote_citation.enw
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/RIS_citation.ris
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/citations/bib_citation.bib
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/make.bat
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/conf.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/dcm_classifier.rst
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/index.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/modules.rst
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_static/dcm-classifier.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_templates/class.rst
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/_templates/function.rst
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/docs/source/installation/index.rst
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    21140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    17820 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    17996 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16172 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/src/dcm_classifier/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/.gitignore
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_0.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_1.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_10.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_11.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_12.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_13.0.dcm
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_14.0.dcm
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_15.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_16.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_17.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_18.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_19.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_2.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_20.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_21.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_3.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_4.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_5.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_6.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_7.0.dcm
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_8.0.dcm
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_9.0.dcm
--rw-r--r--   0        0        0    64900 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/all_fields_data/all_fields_file.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
--rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
--rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
--rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
--rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
--rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
--rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
--rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
--rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
--rw-r--r--   0        0        0   218166 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
--rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
--rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
--rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
--rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
--rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
--rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
--rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
--rw-r--r--   0        0        0   314416 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
--rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
--rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
--rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
--rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
--rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
--rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
--rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
--rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
--rw-r--r--   0        0        0   166952 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
--rw-r--r--   0        0        0   166956 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
--rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
--rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
--rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
--rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
--rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
--rw-r--r--   0        0        0   166946 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
--rw-r--r--   0        0        0   166948 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
--rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
--rw-r--r--   0        0        0   832602 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
--rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
--rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
--rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
--rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
--rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
--rw-r--r--   0        0        0   111700 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
--rw-r--r--   0        0        0   111704 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
--rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
--rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
--rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
--rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
--rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
--rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
--rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
--rw-r--r--   0        0        0   111696 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
--rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
--rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
--rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
--rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
--rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
--rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
--rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
--rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
--rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
--rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
--rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
--rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
--rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
--rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
--rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
--rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
--rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
--rw-r--r--   0        0        0    66392 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
--rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
--rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
--rw-r--r--   0        0        0    66388 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
--rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
--rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
--rw-r--r--   0        0        0    66384 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
--rw-r--r--   0        0        0    66396 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
--rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
--rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
--rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
--rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
--rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
--rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
--rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
--rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
--rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
--rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
--rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
--rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
--rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
--rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
--rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
--rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
--rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
--rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
--rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
--rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
--rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
--rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
--rw-r--r--   0        0        0   149132 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
--rw-r--r--   0        0        0   149148 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
--rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
--rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
--rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
--rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
--rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
--rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
--rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
--rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
--rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
--rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
--rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
--rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
--rw-r--r--   0        0        0   234544 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
--rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
--rw-r--r--   0        0        0   234548 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
--rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
--rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
--rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
--rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
--rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
--rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
--rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
--rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
--rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
--rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
--rw-r--r--   0        0        0   234540 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
--rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
--rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
--rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
--rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
--rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
--rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
--rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
--rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
--rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
--rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
--rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
--rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
--rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
--rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
--rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
--rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
--rw-r--r--   0        0        0   437476 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
--rw-r--r--   0        0        0   132600 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
--rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/no_valid_fields.dcm
--rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
--rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
--rw-r--r--   0        0        0    64842 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
--rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
--rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
--rw-r--r--   0        0        0    64850 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
--rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
--rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_0.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_1.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_10.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_11.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_12.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_13.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_14.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_15.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_2.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_3.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_4.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_5.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_6.0.dcm
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_7.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_8.0.dcm
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_9.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_0.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_1.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_10.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_11.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_12.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_13.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_14.0.dcm
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_15.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_16.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_17.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_18.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_19.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_2.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_3.0.dcm
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_4.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_5.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_6.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_7.0.dcm
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_8.0.dcm
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_9.0.dcm
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/LICENSE
--rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.git
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.gitattributes
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/citations/EndNote_citation.enw
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/citations/RIS_citation.ris
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/citations/bib_citation.bib
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/make.bat
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/requirements-docs.txt
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/conf.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/dcm_classifier.rst
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/index.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/modules.rst
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/_static/dcm-classifier.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/_templates/class.rst
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/_templates/function.rst
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/docs/source/installation/index.rst
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    21140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    17820 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22707 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    18185 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    19620 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/src/dcm_classifier/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_16.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_17.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_18.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_19.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_20.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_21.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0    64900 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/all_fields_data/all_fields_file.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm
+-rw-r--r--   0        0        0    64876 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm
+-rw-r--r--   0        0        0    64874 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm
+-rw-r--r--   0        0        0    64878 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm
+-rw-r--r--   0        0        0    64872 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm
+-rw-r--r--   0        0        0   218166 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm
+-rw-r--r--   0        0        0   218156 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm
+-rw-r--r--   0        0        0   218160 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm
+-rw-r--r--   0        0        0   218162 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm
+-rw-r--r--   0        0        0   314416 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm
+-rw-r--r--   0        0        0   314418 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm
+-rw-r--r--   0        0        0   314414 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm
+-rw-r--r--   0        0        0   314412 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm
+-rw-r--r--   0        0        0   314410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm
+-rw-r--r--   0        0        0   166952 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm
+-rw-r--r--   0        0        0   166956 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm
+-rw-r--r--   0        0        0   166958 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm
+-rw-r--r--   0        0        0   166954 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm
+-rw-r--r--   0        0        0   166946 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm
+-rw-r--r--   0        0        0   166948 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm
+-rw-r--r--   0        0        0   166950 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm
+-rw-r--r--   0        0        0   832602 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm
+-rw-r--r--   0        0        0   832592 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm
+-rw-r--r--   0        0        0   832596 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm
+-rw-r--r--   0        0        0   832598 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm
+-rw-r--r--   0        0        0   111700 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm
+-rw-r--r--   0        0        0   111704 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm
+-rw-r--r--   0        0        0   111706 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm
+-rw-r--r--   0        0        0   111702 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm
+-rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm
+-rw-r--r--   0        0        0   111694 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm
+-rw-r--r--   0        0        0   111696 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm
+-rw-r--r--   0        0        0   111698 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm
+-rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm
+-rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm
+-rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm
+-rw-r--r--   0        0        0   653406 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm
+-rw-r--r--   0        0        0   653410 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm
+-rw-r--r--   0        0        0   653402 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm
+-rw-r--r--   0        0        0   653404 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm
+-rw-r--r--   0        0        0   653408 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm
+-rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm
+-rw-r--r--   0        0        0   653400 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm
+-rw-r--r--   0        0        0   653398 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm
+-rw-r--r--   0        0        0    66392 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm
+-rw-r--r--   0        0        0    66390 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm
+-rw-r--r--   0        0        0    66388 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm
+-rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm
+-rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm
+-rw-r--r--   0        0        0    66384 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm
+-rw-r--r--   0        0        0    66396 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm
+-rw-r--r--   0        0        0    66382 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm
+-rw-r--r--   0        0        0    66394 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm
+-rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm
+-rw-r--r--   0        0        0   149140 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm
+-rw-r--r--   0        0        0   149138 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm
+-rw-r--r--   0        0        0   149142 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm
+-rw-r--r--   0        0        0   149146 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm
+-rw-r--r--   0        0        0   149150 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm
+-rw-r--r--   0        0        0   149132 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm
+-rw-r--r--   0        0        0   149148 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm
+-rw-r--r--   0        0        0   149144 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm
+-rw-r--r--   0        0        0   149134 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm
+-rw-r--r--   0        0        0   149136 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm
+-rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm
+-rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm
+-rw-r--r--   0        0        0   149120 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm
+-rw-r--r--   0        0        0   149114 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm
+-rw-r--r--   0        0        0   149110 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm
+-rw-r--r--   0        0        0   149112 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm
+-rw-r--r--   0        0        0   234544 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm
+-rw-r--r--   0        0        0   234548 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm
+-rw-r--r--   0        0        0   234550 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm
+-rw-r--r--   0        0        0   234546 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm
+-rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm
+-rw-r--r--   0        0        0   234538 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm
+-rw-r--r--   0        0        0   234540 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm
+-rw-r--r--   0        0        0   234542 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/flair.xml
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm
+-rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm
+-rw-r--r--   0        0        0   111492 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm
+-rw-r--r--   0        0        0   111502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm
+-rw-r--r--   0        0        0   111500 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm
+-rw-r--r--   0        0        0   111494 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm
+-rw-r--r--   0        0        0   111498 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm
+-rw-r--r--   0        0        0   111496 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm
+-rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm
+-rw-r--r--   0        0        0   832220 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm
+-rw-r--r--   0        0        0   832640 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm
+-rw-r--r--   0        0        0   437476 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm
+-rw-r--r--   0        0        0   132600 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm
+-rw-r--r--   0        0        0    13532 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/no_valid_fields.dcm
+-rw-r--r--   0        0        0   149116 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm
+-rw-r--r--   0        0        0    64842 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm
+-rw-r--r--   0        0        0    64868 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm
+-rw-r--r--   0        0        0    64870 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm
+-rw-r--r--   0        0        0    64850 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm
+-rw-r--r--   0        0        0    64880 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm
+-rw-r--r--   0        0        0   314422 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_0.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_1.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_10.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_11.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_12.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_13.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_14.0.dcm
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_15.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_16.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_17.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_18.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_19.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_2.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_3.0.dcm
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_4.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_5.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_6.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_7.0.dcm
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_8.0.dcm
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_9.0.dcm
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9393 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6314 2020-02-02 00:00:00.000000 dcm_classifier-0.9.1/PKG-INFO
```

### Comparing `dcm_classifier-0.9.0/.pre-commit-config.yaml` & `dcm_classifier-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/CONTRIBUTING.md` & `dcm_classifier-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.9.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.github/workflows/push_to_main.yml` & `dcm_classifier-0.9.1/.github/workflows/push_to_main.yml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/citations/bib_citation.bib` & `dcm_classifier-0.9.1/citations/bib_citation.bib`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/Makefile` & `dcm_classifier-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/make.bat` & `dcm_classifier-0.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/source/conf.py` & `dcm_classifier-0.9.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/source/dcm_classifier.rst` & `dcm_classifier-0.9.1/docs/source/dcm_classifier.rst`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/source/index.rst` & `dcm_classifier-0.9.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/source/_static/dcm-classifier.css` & `dcm_classifier-0.9.1/docs/source/_static/dcm-classifier.css`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/docs/source/installation/index.rst` & `dcm_classifier-0.9.1/docs/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/models/ova_rf_classifier.onnx` & `dcm_classifier-0.9.1/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/models/rf_classifier.onnx` & `dcm_classifier-0.9.1/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.9.1/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/classify_study.py` & `dcm_classifier-0.9.1/scripts/classify_study.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.9.1/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/create_training_sheet.py` & `dcm_classifier-0.9.1/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.9.1/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/modality_classifier_training.py` & `dcm_classifier-0.9.1/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.9.1/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/orientation_model_training.py` & `dcm_classifier-0.9.1/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/run_all_dicom_data_sheets.sh` & `dcm_classifier-0.9.1/scripts/run_all_dicom_data_sheets.sh`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/running_classifier.ipynb` & `dcm_classifier-0.9.1/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/todo_list` & `dcm_classifier-0.9.1/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/training_config.py` & `dcm_classifier-0.9.1/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/scripts/utilities.py` & `dcm_classifier-0.9.1/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.9.1/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.9.1/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.9.1/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.9.1/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.9.1/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.9.1/src/dcm_classifier/image_type_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,14 +375,18 @@
         # if there is only a single volume in the series, the series modality and acquisition plane are set to the
         # volume's modality and acquisition plane
         if len(self.series.get_volume_list()) == 1:
             volume = self.series.get_volume_list()[0]
             modality = volume.get_volume_modality().replace("LOW_PROBABILITY_", "")
 
             self.series.set_series_modality(modality)
+            bval = volume.get_volume_bvalue()
+            if bval > 0 and modality not in ["tracew", "adc", "fa", "eadc", "dwig"]:
+                self._update_diffusion_series_modality()
+
             self.series.set_modality_probabilities(volume.get_modality_probabilities())
             self.series.set_acquisition_plane(volume.get_acquisition_plane())
             self.series.set_is_isotropic(volume.get_is_isotropic())
             self.series.set_has_contrast(volume.get_has_contrast())
         else:
             # for acquisition plane we assume as volumes in series have the same acquisition plane
             # similarly we propagate the isotropic and contrast
```

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.9.1/src/dcm_classifier/study_processing.py`

 * *Files 22% similar despite different names*

```diff
@@ -231,14 +231,80 @@
         """
         for (
             series_number,
             series_object,
         ) in self.series_dictionary.items():
             self.inferer.set_series(series_object)
             self.inferer.run_inference()
+        self.fixup_adjacent_series()
+
+    def fixup_adjacent_series(self):
+        # Fix up case where adjacent volumes make up a family of tracew images and one of them is a bvalue=0 image
+        for current_series_number, series_obj in self.get_study_dictionary().items():
+            if series_obj.get_volume_list()[
+                0
+            ].get_volume_bvalue() == 0 and series_obj.get_series_modality() not in [
+                "tracew",
+                "adc",
+                "fa",
+                "eadc",
+                "dwig",
+            ]:
+                for (
+                    adjacent_series_number,
+                    adjacent_series_obj,
+                ) in self.get_study_dictionary().items():
+                    if adjacent_series_number != current_series_number:
+                        list_of_candidate_adjacent = [
+                            int(current_series_number + 1),
+                            int(current_series_number - 1),
+                        ]
+                        if adjacent_series_number in list_of_candidate_adjacent:
+                            if adjacent_series_obj.get_series_modality() == "tracew":
+                                # if an adjacent image is a tracew image, and has same physical space as
+                                # the current image then assume it is also a tracew image
+                                itk_volume = series_obj.get_volume_list()[
+                                    0
+                                ].get_itk_image()
+                                itk_adjacent_volume = (
+                                    adjacent_series_obj.get_volume_list()[
+                                        0
+                                    ].get_itk_image()
+                                )
+
+                                same_size: bool = (
+                                    itk_volume.GetLargestPossibleRegion().GetSize()
+                                    == itk_adjacent_volume.GetLargestPossibleRegion().GetSize()
+                                )
+                                same_space: bool = (
+                                    itk_volume.GetSpacing()
+                                    == itk_adjacent_volume.GetSpacing()
+                                )
+                                same_origin: bool = (
+                                    itk_volume.GetOrigin()
+                                    == itk_adjacent_volume.GetOrigin()
+                                )
+                                same_direction: bool = (
+                                    itk_volume.GetDirection()
+                                    == itk_adjacent_volume.GetDirection()
+                                )
+
+                                if (
+                                    same_size
+                                    and same_space
+                                    and same_origin
+                                    and same_direction
+                                ):
+                                    series_obj.set_series_modality("tracew")
+                                else:
+                                    print(
+                                        f"Adjacent series {adjacent_series_number} does not have same physical space as {current_series_number}"
+                                    )
+                                    print(itk_volume)
+                                    print(itk_adjacent_volume)
 
     def validate(self) -> None:
         pass
 
     def __identify_single_volumes(
         self,
         study_directory: Path,
```

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.9.1/src/dcm_classifier/utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/src/dcm_classifier/models/ova_rf_classifier.onnx` & `dcm_classifier-0.9.1/src/dcm_classifier/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/conftest.py` & `dcm_classifier-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/mock_data.txt` & `dcm_classifier-0.9.1/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_0.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_0.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_1.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_1.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_10.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_10.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_11.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_11.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_12.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_12.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_13.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_13.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_14.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_14.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_15.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_15.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_16.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_16.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_17.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_17.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_18.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_18.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_19.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_19.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_2.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_2.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_20.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_20.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_21.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_21.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_3.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_3.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_4.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_4.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_5.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_5.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_6.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_6.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_7.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_7.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_8.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_8.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/adc_volumes/volume_0/test_dcm_9.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/adc_volumes/volume_0/test_dcm_9.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/all_fields_data/all_fields_file.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/all_fields_data/all_fields_file.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-10-1xysu14.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-100-19qrakc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-101-1lerkgh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-102-ud6kyp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-103-1gopr5n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-104-4u8pw1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-105-n1vi8j.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-106-1uc0j0n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-107-1hguaf6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-108-uouo61.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-109-unrs9s.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-11-5tfjad.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-110-rel8ya.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-111-1y5vtne.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-112-1p25iu6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-113-z68zh9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-114-dzgu2w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-115-v9n4wf.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-116-m08bc8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-117-1mxau93.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-118-1u23uus.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-119-wa2f4l.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-12-1gc977m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-120-1fntu45.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-121-qgtx29.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-122-233id4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-123-1lqv1t3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-124-1ybp4af.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-125-19h2jfj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-126-w2wllu.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-127-1f371lh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-128-pq9c6v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-13-gnnoar.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-14-10wq5d1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-15-1ha5m1j.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-16-4qi5pf.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-17-1ohohsv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-18-1mexxdv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-19-1h81yec.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-2-1poz2m2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-20-1c505ik.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-21-5h1q9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-22-nq4icb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-23-1mbcv3u.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-24-8tvg2n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-25-zg853z.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-26-1uh4leh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-27-1indy7p.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-28-jpmfcg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-29-9pz0v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-3-1y37xyq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-30-8b33jo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-31-76xubd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-32-o5q003.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-33-h2vbhq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-34-721wu6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-35-u2xx88.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-36-mfix7m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-37-m7va10.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-38-hoxvrn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-39-13zh078.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-4-d1fih8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-40-1r09it4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-41-19s3vir.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-42-10xwnaz.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-43-1e09rnb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-44-13aqkku.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-45-1vpws2t.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-46-yjwr6j.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-47-18ejfud.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-48-8mqd7v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-49-1ttjbqn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-5-1pr736k.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-50-179qx0w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-51-x4hdkv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-52-1pk6pyd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-53-hm8s9y.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-54-3l6wf5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-55-1b24ldg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-56-ipmfob.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-57-1jlu3en.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-58-j6bf73.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-59-qnoban.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-6-nk6485.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-60-148owa9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-61-qcpysk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-62-8d3k16.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-63-jgxf99.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-64-jqoo93.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-65-19shtnm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-66-14qdmkp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-67-1vpb2i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-68-s9kwrc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-69-19478s5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-7-1cq29b5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-70-p7n6ma.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-71-1mnfekn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-72-m27dcc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-73-qpoqy4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-74-1cmr0c4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-75-133p6vn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-76-g85zn3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-77-6l9xxa.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-78-towy03.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-79-xk5g74.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-8-1vevq6l.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-80-1nnz6vj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-81-w9xiv6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-82-180mv0y.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-83-310bbb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-84-v4t7iu.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-85-1362r72.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-86-wh0h58.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-87-3u8j27.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-88-fwa5ka.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-89-1pqsq6p.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-9-1a6kl36.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-90-1ji04qi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-91-a0p4qc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-92-agemkm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-93-itttod.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-94-fzm4q6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-95-1fjy3sd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-96-lmk6b2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-97-1bj9qy2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-98-dguayf.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/1/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-99-1uwqu26.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-1-15hb89z.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-10-t0ppfl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-11-1s8tn1e.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-12-vi2y6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-13-og6kii.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-14-1rg2wyo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-15-xdyoma.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-16-vxmscd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-17-g96ig8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-18-1y3kog9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-19-nzuik9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-2-17h3v1o.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-3-q41r31.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-4-twpat0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-5-1kw5tv3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-6-18vwd34.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-7-kkrgt3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-8-1yvyqoc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/10/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-10-9-72wnbk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-1-1t16lwn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-10-1i6psfb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-11-1dy473d.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-12-rykg48.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-13-zkpx2f.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-14-1il55c9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-15-9mlqjw.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-16-1h6pq2n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-17-1xt3xg4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-18-rldk7n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-19-7h6ym1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-2-145dqnp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-20-134cbdn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-3-4fpcov.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-4-19gzyef.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-5-1ylzw3x.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-6-12lo636.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-7-1qit8ra.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-8-wd8z1a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/11/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-9-lwvysx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-1-1m5n7dn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-10-sjmio8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-11-k2p6gi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-12-59wsam.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-13-sacu5u.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-14-92caen.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-15-nuihid.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-16-6d8gn7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-17-17vkw86.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-18-j5f2ih.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-19-1yute86.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-2-11cirx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-20-1bpwhb4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-21-1as1u2s.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-3-hslyt1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-4-oh5rth.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-5-1vc6xcb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-6-1wjcqv7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-7-s5wjm4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-8-7w26ka.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/12/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-12-9-1deai4l.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-1-10uggr7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-10-tgkiip.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-11-1vs231w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-12-k6qqp6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-13-132ftsk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-14-y2xcn7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-15-lsm6s2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-16-1nkgmy3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-17-1r649p1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-18-s06pqr.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-19-1vf8sfi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-2-12967q4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-3-183557a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-4-14pe876.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-5-38ybs0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-6-v6lqy5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-7-1hfpfg7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-8-1ebnj0m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/13/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-13-9-1uv1ex6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-1-148iz91.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-10-kp4ljg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-11-151hnd7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-12-3hibgp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-13-11snsb5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-14-cinmgp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-15-yj3jn3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-16-2duahv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-17-1u82pmg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-18-16v0x8x.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-19-1v859ws.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-2-vo7uh4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-20-ohf5b4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-21-1evse13.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-3-99kgsp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-4-8f3fkt.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-5-1io5vpr.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-6-g8ss03.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-7-wu9mww.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-8-6atp6f.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/14/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-14-9-ajjvkh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-1-wdu9cz.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-10-lvvina.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-11-16yvenf.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-12-mwfljw.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-13-14fkxvc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-14-vkjd8b.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-15-1xrwpvx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-16-roaha0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-17-1ghy535.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-18-9flequ.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-19-ymqig6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-2-rbjg0y.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-20-10q0z2k.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-21-15dvtr7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-22-6q7qr2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-3-xf7b6v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-4-1qdmhdy.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-5-cq4b2q.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-6-93vwyc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-7-1cj1zuq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-8-w1gpvl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/15/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-15-9-nnm3oo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-1-19m8olr.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-2-1wqh5ct.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-3-f6mlzj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-4-7mt3sm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/2/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-2-5-py31xt.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-1-122zl3y.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-2-o412pc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/3/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-3-3-67awbx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-1-k5jl9w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-2-2n4wps.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/4/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-4-3-18j29r6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-1-phj6rx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-10-18t9xxw.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-11-1of7j11.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-12-g87q4m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-13-l7u4a1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-14-hhkhv3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-15-r1dr3z.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-16-r2yjb7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-17-19yvxy9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-18-gfxjhs.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-19-nrxs6o.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-2-1dytpw5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-20-11fqt3v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-21-3chbmp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-22-1tra7s.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-23-2dopd7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-24-1rhn0zy.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-25-1ti5jon.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-26-vqel0a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-27-1doe58p.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-28-a8h73r.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-29-3iriik.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-3-jstuhr.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-30-gtecpk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-31-1ffbkps.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-32-mrryah.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-33-7wye8b.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-34-oefepl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-35-1maq2fg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-36-13sjukx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-37-l7nvb0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-38-1phrlla.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-39-snlr9m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-4-153sh8w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-40-84d1fh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-41-nqpbbl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-42-1pmqnes.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-5-18p0d4y.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-6-19gtga3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-7-t4q81m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-8-12xngqg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/5/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-5-9-13g3g2d.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-1-xv45la.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-10-1sbgkr0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-11-1hcjle9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-12-1i8d4g7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-13-xyu2q3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-14-1zxtz0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-15-1ae2q17.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-16-1lt3s62.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-17-fgp0aw.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-18-ftlw3z.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-19-8qdslo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-2-1gwoqkm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-20-9jr71h.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-21-1lt471e.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-3-oszlip.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-4-s0m8k4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-5-ouodpn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-6-grkmc8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-7-y7bhpg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-8-1o5vwa7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/6/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-6-9-84252n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-1-1lwbe5o.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-10-1a90h3l.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-11-2qf598.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-12-eaa388.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-13-1vfv48v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-14-pgxw42.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-15-t62a2p.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-16-146fgct.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-17-wy6sqo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-18-1axyol3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-19-bw8ctt.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-2-k3oyc1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-20-ryktlj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-21-1r5ad4m.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-3-1vf7o81.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-4-uzuqgm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-5-1agqy5i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-6-153czxf.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-7-lbz1bt.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-8-1bes89u.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-7-9-bnqbs2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/flair.xml` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/7/DICOM/flair.xml`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-1-15ncxxk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-10-osifub.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-11-ipd88o.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-12-1qmfhm2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-13-g40gip.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-14-1jxjnz3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-15-14s3bvv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-16-zueovp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-17-1tqedv1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-18-1dfttqy.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-19-8hhuq3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-2-15etcad.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-20-1uhuak5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-21-wk4nls.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-22-rdr82a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-23-1ttv0tj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-24-zd9nnj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-25-x4487e.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-26-1o13ogj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-27-1hdzcja.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-28-v1sg4e.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-29-165pvwq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-3-1lknwyl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-30-1fijzj1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-31-1wfu108.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-32-166y6qo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-33-p7wfo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-34-1pvgarj.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-35-bbcpv5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-36-1rnh7qt.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-37-12sf5qz.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-38-lyqn7i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-39-1e5u2fz.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-4-zn2a05.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-40-1oghzkh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-41-1tl9feg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-42-v34jag.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-43-11jafrp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-44-146c10r.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-45-gxoriq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-46-8xca7i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-47-d57w1n.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-48-4ausia.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-49-7r1x1a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-5-y7hb67.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-6-q3q2iq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-7-82z0a9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-8-n0ymz4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/8/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-8-9-1w6qf59.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-1-14ejdyx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-10-tg0rh4.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-11-14ddr2i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-12-1if4l92.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-13-841hvq.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-14-f555es.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-15-16wao1f.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-16-12ydcs6.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-17-1nbxhqn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-18-1niibu8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-19-1xqztu0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-2-18i4bao.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-20-1w55zzh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-21-1j856uu.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-22-1sv5xgw.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-23-1bmgze2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-24-1kfwo5b.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-25-5mp033.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-26-153clsz.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-27-nvkwfo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-28-snif8i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-29-43slwm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-3-pqvvc9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-30-1civbg3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-31-vqg14i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-32-1hifrme.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-33-1pc84tk.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-34-ld3236.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-35-1vemduc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-36-vqwaqx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-37-91hlk8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-38-1mjzhw7.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-39-5kh4de.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-4-1ofsfnd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-40-2lxshi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-41-1mtvjsv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-42-1k3ms6j.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-43-2dj4bg.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-44-14j88c3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-45-etddx1.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-46-1eosrbb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-47-1vb155x.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-48-71f9q8.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-49-qsyyma.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-5-9963dp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-50-l5kptm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-51-8efy3c.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-52-i1799o.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-53-15iqzmn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-54-1kb9700.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-55-kq8huc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-56-2zpaub.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-6-ftjhdp.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-7-1yrhfo3.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-8-1ta7c5.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_data/9/DICOM/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-9-9-11s9c6v.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-1-sxzyrb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-10-e2ws99.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-11-1f3745p.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-12-a2kgb2.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-13-v78wxd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-14-vt0tpn.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-15-geavao.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-16-11hpj9w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-17-itux3b.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-18-1n7qq1a.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-19-1krapto.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-2-m3fh9.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-20-27f98.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-21-onzawa.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-22-zcurzc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-23-1ohi0oi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-24-5hif1i.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-25-k2v87w.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-26-j2v5jh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-3-1q9sxvd.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-4-j1vatm.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-5-1ezb2sl.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-6-bf4zvi.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-7-19cthhv.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-8-ekjcxh.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/anonymized_dwi_series/DICOM/1.3.12.2.1107.5.1.4.91493331060615608073226796366526631566-2-9-1pbtofx.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/contrast_data/with_contrast/0424.MR.PHD_050.8.0001.20100122.165135.421000.1md0v5z.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/contrast_data/without_contrast/custom.0428.MR.PHD_144.1.1.20060428.123606.e29xoc.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/no_valid_fields.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/no_valid_fields.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/emptyBValue.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidEchoTime.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidPixelBW.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/invalidSeriesNum.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noEchoTime.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noImgType.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noPixelBW.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/noSeriesNum.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/invalid_fields/unknownImgType.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-1-1-mvhslo.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm` & `dcm_classifier-0.9.1/tests/testing_data/anonymized_testing_data/invalid_data/mult_series_uid/1.3.12.2.1107.5.1.4.3024295249861856527476734919304407350-11-21-1svccb.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_0.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_0.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_1.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_1.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_10.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_10.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_11.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_11.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_12.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_12.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_13.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_13.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_14.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_14.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_15.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_15.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_2.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_2.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_3.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_3.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_4.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_4.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_5.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_5.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_6.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_6.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_7.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_7.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_8.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_8.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_0/test_dcm_9.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_0/test_dcm_9.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_0.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_0.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_1.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_1.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_10.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_10.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_11.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_11.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_12.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_12.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_13.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_13.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_14.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_14.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_15.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_15.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_16.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_16.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_17.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_17.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_18.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_18.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_19.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_19.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_2.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_2.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_3.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_3.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_4.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_4.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_5.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_5.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_6.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_6.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_7.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_7.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_8.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_8.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/testing_data/dwi_volumes/volume_1/test_dcm_9.0.dcm` & `dcm_classifier-0.9.1/tests/testing_data/dwi_volumes/volume_1/test_dcm_9.0.dcm`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.9.1/tests/unit_testing/test_dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.9.1/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.9.1/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.9.1/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.9.1/tests/unit_testing/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/.gitignore` & `dcm_classifier-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/LICENSE` & `dcm_classifier-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/README.md` & `dcm_classifier-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.9.0/pyproject.toml` & `dcm_classifier-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.9.0'
+version = '0.9.1'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
   { name="Cavan Riley", email="cavan-riley@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
```

### Comparing `dcm_classifier-0.9.0/PKG-INFO` & `dcm_classifier-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.9.0
+Version: 0.9.1
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>, Cavan Riley <cavan-riley@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: itk-core>=5.3.0
```

