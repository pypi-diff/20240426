# Comparing `tmp/immuneML-3.0.0a3.tar.gz` & `tmp/immuneml-3.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immuneML-3.0.0a3.tar", last modified: Tue Feb  6 18:13:26 2024, max compression
+gzip compressed data, was "immuneml-3.0.0a4.tar", last modified: Fri Apr 26 16:11:26 2024, max compression
```

## Comparing `immuneML-3.0.0a3.tar` & `immuneml-3.0.0a4.tar`

### file list

```diff
@@ -1,698 +1,700 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.604027 immuneML-3.0.0a3/immuneML/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.608027 immuneML-3.0.0a3/immuneML/IO/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.608027 immuneML-3.0.0a3/immuneML/IO/dataset_export/
--rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_export/AIRRExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_export/DataExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_export/ImmuneMLExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.608027 immuneML-3.0.0a3/immuneML/IO/dataset_import/
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/AIRRImport.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/DataImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/DatasetImportParams.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/GenericImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/IGoRImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    20557 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/IReceptorImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmuneMLImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    10591 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/MiXCRImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/OLGAImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     5438 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/TenxGenomicsImport.py
--rw-r--r--   0 runner    (1001) docker     (127)    12185 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/VDJdbImport.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.608027 immuneML-3.0.0a3/immuneML/IO/dataset_import/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/IO/ml_method/
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/ml_method/MLExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/ml_method/MLImport.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/ml_method/MLMethodConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/ml_method/UtilIO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/IO/ml_method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/AxisType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/SequenceMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/BooleanType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/CriteriaMatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/DataType.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/OperationType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/criteria_matches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/analysis/data_manipulation/
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/data_manipulation/DataReshaper.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/data_manipulation/NormalizationType.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       78 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/data_manipulation/ReductionMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/data_manipulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/analysis/entropy_calculations/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/entropy_calculations/EntropyCalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/entropy_calculations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/analysis/similarities/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/similarities/SimilarityMeasureType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/analysis/similarities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.612027 immuneML-3.0.0a3/immuneML/api/aggregated_runs/
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/aggregated_runs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/api_encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.616027 immuneML-3.0.0a3/immuneML/api/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/DataSimulationTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/DatasetGenerationOverviewTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/DatasetGenerationTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyMLApplicationTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxySimulationTool.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTrainGenModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTrainMLModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyYamlTool.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/RepertoireClassificationTool.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/build_dataset_overview_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/build_dataset_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/api/galaxy/build_yaml_from_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.616027 immuneML-3.0.0a3/immuneML/app/
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/app/ImmuneMLApp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/app/LigoApp.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.616027 immuneML-3.0.0a3/immuneML/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/caching/CacheHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/caching/CacheObjectType.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/caching/CacheType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/caching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.596027 immuneML-3.0.0a3/immuneML/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.596027 immuneML-3.0.0a3/immuneML/config/default_params/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.620027 immuneML-3.0.0a3/immuneML/config/default_params/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/airr_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/generic_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/i_receptor_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/igor_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/mixcr_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/olga_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/random_receptor_dataset_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/random_sequence_dataset_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/tenx_genomics_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/datasets/vdjdb_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.620027 immuneML-3.0.0a3/immuneML/config/default_params/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/atchley_kmer_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/comp_airr_distance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/comp_airr_sequence_abundance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/distance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/kmer_abundance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/kmer_frequency_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/matched_receptors_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/matched_regex_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/matched_sequences_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/motif_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/one_hot_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/sequence_abundance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/similar_to_positive_sequence_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/encodings/word2_vec_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.620027 immuneML-3.0.0a3/immuneML/config/default_params/example_weighting/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/example_weighting/predefined_weighting_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.624027 immuneML-3.0.0a3/immuneML/config/default_params/instructions/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/exploratory_analysis_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/export_parser_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/feasibility_summary_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/ligo_sim_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/ml_application_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/split_config_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/subsampling_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/train_gen_model_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/instructions/train_ml_model_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.624027 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/atchley_kmer_mil_classifier_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/binary_feature_classifier_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/deep_rc_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/keras_sequence_cnn_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/ml_method_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/receptor_cnn_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/simple_vae_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/tcrdist_classifier_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.624027 immuneML-3.0.0a3/immuneML/config/default_params/motif_instantiation_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/motif_instantiation_strategy/gapped_kmer_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.624027 immuneML-3.0.0a3/immuneML/config/default_params/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/preprocessing/duplicate_sequence_filter_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/preprocessing/sequence_length_filter_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/config/default_params/reports/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/amino_acid_frequency_distribution_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/coefficients_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/cv_feature_performance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/cytoscape_network_exporter_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/deep_rc_motif_discovery_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/design_matrix_exporter_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/feature_comparison_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/feature_value_barplot_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/ml_settings_performance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/motif_generalization_analysis_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/motif_overlap_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/motif_seed_recovery_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/motif_test_set_performance_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/receptor_dataset_overview_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/recovered_significant_features_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/reference_sequence_overlap_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/repertoire_clonotype_summary_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/sequence_length_distribution_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/significant_features_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/tcrdist_motif_discovery_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/reports/vj_gene_distribution_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/config/default_params/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/simulation/ligo_sim_config_item_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/config/default_params/simulation/ligo_sim_config_params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/DatasetItem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/SequenceSet.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/bnp_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/data_model/cell/
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/cell/Cell.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/cell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/data_model/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/ElementDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/ReceptorDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/RepertoireDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/SequenceDataset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.628027 immuneML-3.0.0a3/immuneML/data_model/encoded_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/encoded_data/EncodedData.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/encoded_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.632027 immuneML-3.0.0a3/immuneML/data_model/receptor/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/BCKReceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/BCReceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/ChainPair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/ElementGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/Receptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/ReceptorBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/RegionType.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/TCABReceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/TCGDReceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.632027 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/Chain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/SequenceFrameType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.632027 immuneML-3.0.0a3/immuneML/data_model/repertoire/
--rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/repertoire/Repertoire.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/data_model/repertoire/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.632027 immuneML-3.0.0a3/immuneML/dev_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dev_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dev_util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.632027 immuneML-3.0.0a3/immuneML/dsl/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/DefaultParamsLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/ImmuneMLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/InstructionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/ObjectParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/OutputParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/Parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/DefinitionParser.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/DefinitionParserOutput.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/EncodingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/ExampleWeightingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/MLParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/MotifParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/PreprocessingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/ReportParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/SignalParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/SimulationParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/definition_parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/dsl/import_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/import_parsers/ImportParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/import_parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ApplyGenModelParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ClusteringParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/DatasetExportParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/FeasibilitySummaryParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/LabelHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/LigoSimParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/MLApplicationParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/SubsamplingParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/TrainGenModelParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/TrainMLModelParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/dsl/semantic_model/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/semantic_model/MLResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/semantic_model/SemanticModel.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/semantic_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/dsl/symbol_table/
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/symbol_table/SymbolTable.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/symbol_table/SymbolTableEntry.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/symbol_table/SymbolType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/dsl/symbol_table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.636027 immuneML-3.0.0a3/immuneML/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/DatasetEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/EncoderParams.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19981 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14047 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/RelativeAbundanceType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/deeprc/
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/deeprc/DeepRCEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/deeprc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)    12427 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/DistanceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/DistanceMetricType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/TCRdistEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/distance_encoding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/evenness_profile/
--rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/evenness_profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.640027 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/MotifEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/PositionalMotifHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/PositionalMotifParams.py
--rw-r--r--   0 runner    (1001) docker     (127)    12656 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/SimilarToPositiveSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/motif_encoding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/onehot/
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotReceptorEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotRepertoireEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/onehot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/preprocessing/FeatureScaler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/
--rw-r--r--   0 runner    (1001) docker     (127)    15433 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8336 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/SequenceMatchingSummaryType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/reference_encoding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.644027 immuneML-3.0.0a3/immuneML/encodings/word2vec/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/W2VRepertoireEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/W2VSequenceEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/Word2VecEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/EnvironmentSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/Label.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/LabelConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/LabelType.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/SequenceType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/example_weighting/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/example_weighting/ExampleWeightingParams.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/example_weighting/ExampleWeightingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/example_weighting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/example_weighting/predefined_weighting/
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/example_weighting/predefined_weighting/PredefinedWeighting.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/example_weighting/predefined_weighting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/HPSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/HPSettingResult.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/LeaveOneOutConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/ManualSplitConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/ReportConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/SplitConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/SplitType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.648027 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPAssessment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPSelection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.652027 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPAssessmentState.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPLabelState.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPSelectionState.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/TrainMLModelState.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.652027 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/GridSearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.652027 immuneML-3.0.0a3/immuneML/ml_methods/
--rw-r--r--   0 runner    (1001) docker     (127)    19683 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/BinaryFeatureClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/KerasSequenceCNN.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.652027 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/AtchleyKmerMILClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    25265 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/DeepRC.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/KNN.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (127)    15878 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/MLMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/PrecomputedKNN.py
--rw-r--r--   0 runner    (1001) docker     (127)    21223 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/ProbabilisticBinaryClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    17227 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/ReceptorCNN.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SVC.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SVM.py
--rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SklearnMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/TCRdistClassifier.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/classifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.656027 immuneML-3.0.0a3/immuneML/ml_methods/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/clustering/ClusteringMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/clustering/KMeans.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.656027 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/DimRedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/PCA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/TSNE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/UMAP.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.656027 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/BackgroundSequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/ExperimentalImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/GenerativeModel.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/InternalOlgaModel.py
--rw-r--r--   0 runner    (1001) docker     (127)    13797 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/OLGA.py
--rw-r--r--   0 runner    (1001) docker     (127)     7365 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/PWM.py
--rw-r--r--   0 runner    (1001) docker     (127)    10991 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SimpleLSTM.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SimpleVAE.py
--rw-r--r--   0 runner    (1001) docker     (127)     6717 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SoNNia.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/generative_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.656027 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/SimpleLSTMGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/SimpleVAEGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.656027 immuneML-3.0.0a3/immuneML/ml_methods/util/
--rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/util/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_methods/util/pytorch_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.660027 immuneML-3.0.0a3/immuneML/ml_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_metrics/ClassificationMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_metrics/ClusteringMetric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_metrics/MetricUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/ml_metrics/ml_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.660027 immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/ComparisonData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.660027 immuneML-3.0.0a3/immuneML/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/ReferenceSequenceAnnotator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/SubjectRepertoireCollector.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.660027 immuneML-3.0.0a3/immuneML/preprocessing/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/ChainRepertoireFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/CountAggregationFunction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/CountPerSequenceFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/DuplicateSequenceFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/MetadataRepertoireFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/SequenceLengthFilter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/preprocessing/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.660027 immuneML-3.0.0a3/immuneML/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/InstructionPresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/PresentationFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/PresentationFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/TemplateParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.664027 immuneML-3.0.0a3/immuneML/presentation/html/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/ClusteringHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/DatasetExportHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/FeasibilitySummaryHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/GenModelHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/HPHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/HTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/LIgOSimulationHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/MLApplicationHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/SubsamplingHTMLBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.664027 immuneML-3.0.0a3/immuneML/presentation/html/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/AssessmentSplitDetails.html
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/Clustering.html
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/DatasetExport.html
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/ExploratoryAnalysis.html
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/FeasibilitySummary.html
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/GenModel.html
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/HPOptimization.html
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/MLApplication.html
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/MLTraining.html
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/MultiDatasetBenchmark.html
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/Reports.html
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/SelectionDetails.html
--rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/Simulation.html
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/Subsampling.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.664027 immuneML-3.0.0a3/immuneML/presentation/html/templates/css/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/presentation/html/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.668027 immuneML-3.0.0a3/immuneML/reports/
--rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/PlotlyUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/Report.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ReportOutput.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ReportResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ReportUtil.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.668027 immuneML-3.0.0a3/immuneML/reports/clustering_reports/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/clustering_reports/ClusteringReport.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/clustering_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.668027 immuneML-3.0.0a3/immuneML/reports/data_reports/
--rw-r--r--   0 runner    (1001) docker     (127)    16227 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/DataReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/GLIPH2Exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    25989 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/MotifGeneralizationAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/ReceptorDatasetOverview.py
--rw-r--r--   0 runner    (1001) docker     (127)    12576 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/RecoveredSignificantFeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/RepertoireClonotypeSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/SequenceLengthDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/SequencesWithSignificantKmers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/SignificantFeatures.py
--rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/SignificantKmerPositions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/SimpleDatasetOverview.py
--rw-r--r--   0 runner    (1001) docker     (127)    19201 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/VJGeneDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5901 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/WeightsDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/data_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.672027 immuneML-3.0.0a3/immuneML/reports/encoding_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/DesignMatrixExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/EncodingReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureComparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureDistribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureValueBarplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/GroundTruthMotifOverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)    12280 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/Matches.py
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/MotifTestSetPerformance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/NonMotifSequenceSimilarity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/PositionalMotifFrequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/RelevantSequenceExporter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/encoding_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.672027 immuneML-3.0.0a3/immuneML/reports/gen_model_reports/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/gen_model_reports/GenModelReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/gen_model_reports/VAESummary.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/gen_model_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.672027 immuneML-3.0.0a3/immuneML/reports/ml_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/BinaryFeaturePrecisionRecall.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/CoefficientPlottingSetting.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/Coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/ConfounderAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/KernelSequenceLogo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/MLReport.py
--rw-r--r--   0 runner    (1001) docker     (127)    14462 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/MotifSeedRecovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/ROCCurve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/TrainingPerformance.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/ml_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/PerformanceOverview.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10385 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/LigoSimState.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/SimConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/SimConfigItem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/simulation/dataset_generation/
--rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/dataset_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/simulation/implants/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/ImplantAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/LigoPWM.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/Motif.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/MotifInstance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/SeedMotif.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/Signal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/implants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.676027 immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/ImplantingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/RejectionSamplingStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/SimulationStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.680027 immuneML-3.0.0a3/immuneML/simulation/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/util/bnp_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/util/igor_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/simulation/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/util/
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/AdaptiveImportHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/CompAIRRHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/CompAIRRParams.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/DistanceMetrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/DocEnumHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/EncoderHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/ExporterHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/FilenameHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/ImportHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/KmerHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/MotifPerformancePlotHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/NameBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/NumpyHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/ParameterValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/PathBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/PositionHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/ReadsType.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/ReflectionHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/RepertoireBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/SequenceAnalysisHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/SignificantFeaturesHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/StringHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/TCRdistHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/GenModelInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/Instruction.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/MLProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    19055 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/TrainMLModelInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/apply_gen_model/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/apply_gen_model/ApplyGenModelInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/apply_gen_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/ClusteringInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/clustering_run_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/dataset_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/dataset_generation/DatasetExportState.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/dataset_generation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisState.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.684027 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/
--rw-r--r--   0 runner    (1001) docker     (127)    13686 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.688027 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/LigoSimInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/runtime_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.688027 immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/quickstart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.688027 immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/SubsamplingState.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.688027 immuneML-3.0.0a3/immuneML/workflows/instructions/train_gen_model/
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/train_gen_model/TrainGenModelInstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/instructions/train_gen_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.688027 immuneML-3.0.0a3/immuneML/workflows/steps/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/DataEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/DataEncoderParams.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/DataWeighter.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/DataWeighterParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodAssessment.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodAssessmentParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodTrainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodTrainerParams.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/Step.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/StepParams.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/DataSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/DataSplitterParams.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/ManualSplitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/Util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/immuneML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30573 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 18:13:26.000000 immuneML-3.0.0a3/immuneML.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/scripts/DocumentatonFormat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/scripts/specification_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/scripts/specs_docs_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 18:13:26.692027 immuneML-3.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-02-06 18:13:09.000000 immuneML-3.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.410246 immuneml-3.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-26 16:11:26.410246 immuneml-3.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.306245 immuneml-3.0.0a4/immuneML/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.306245 immuneml-3.0.0a4/immuneML/IO/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.306245 immuneml-3.0.0a4/immuneML/IO/dataset_export/
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_export/AIRRExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_export/DataExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_export/ImmuneMLExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.310245 immuneml-3.0.0a4/immuneML/IO/dataset_import/
+-rw-r--r--   0 runner    (1001) docker     (127)    13088 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/AIRRImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/DataImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/DatasetImportParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/GenericImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/IGoRImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20808 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/IReceptorImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmuneMLImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10582 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10504 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10842 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/MiXCRImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/OLGAImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/TenxGenomicsImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/VDJdbImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.310245 immuneml-3.0.0a4/immuneML/IO/dataset_import/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)    14265 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.310245 immuneml-3.0.0a4/immuneML/IO/ml_method/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/ml_method/MLExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/ml_method/MLImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/ml_method/MLMethodConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/ml_method/UtilIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/IO/ml_method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/AxisType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/SequenceMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/BooleanType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/CriteriaMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/DataType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/OperationType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/criteria_matches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/analysis/data_manipulation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/data_manipulation/DataReshaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/data_manipulation/NormalizationType.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       78 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/data_manipulation/ReductionMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/data_manipulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/analysis/entropy_calculations/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/entropy_calculations/EntropyCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/entropy_calculations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/analysis/similarities/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/similarities/SimilarityMeasureType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/analysis/similarities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.314245 immuneml-3.0.0a4/immuneML/api/aggregated_runs/
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/aggregated_runs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/api_encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.318245 immuneml-3.0.0a4/immuneML/api/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/DataSimulationTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4154 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/DatasetGenerationOverviewTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/DatasetGenerationTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyMLApplicationTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxySimulationTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTrainGenModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTrainMLModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyYamlTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/RepertoireClassificationTool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/build_dataset_overview_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/build_dataset_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11895 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/api/galaxy/build_yaml_from_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.318245 immuneml-3.0.0a4/immuneML/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/app/ImmuneMLApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/app/LigoApp.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.318245 immuneml-3.0.0a4/immuneML/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/caching/CacheHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/caching/CacheObjectType.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/caching/CacheType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/caching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.294245 immuneml-3.0.0a4/immuneML/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.298245 immuneml-3.0.0a4/immuneML/config/default_params/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.322245 immuneml-3.0.0a4/immuneML/config/default_params/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/airr_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/generic_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/i_receptor_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/igor_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/mixcr_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/olga_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/random_receptor_dataset_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/random_sequence_dataset_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/tenx_genomics_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/datasets/vdjdb_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/atchley_kmer_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/comp_airr_distance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/comp_airr_sequence_abundance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/distance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/kmer_abundance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/kmer_frequency_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/matched_receptors_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/matched_regex_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/matched_sequences_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/motif_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/one_hot_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/sequence_abundance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/similar_to_positive_sequence_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/encodings/word2_vec_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/example_weighting/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/example_weighting/predefined_weighting_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/instructions/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/exploratory_analysis_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/export_parser_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/feasibility_summary_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/ligo_sim_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/ml_application_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/split_config_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/subsampling_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/train_gen_model_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/instructions/train_ml_model_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/atchley_kmer_mil_classifier_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/binary_feature_classifier_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/deep_rc_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/keras_sequence_cnn_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/ml_method_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/receptor_cnn_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/simple_vae_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/tcrdist_classifier_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/motif_instantiation_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/motif_instantiation_strategy/gapped_kmer_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.326245 immuneml-3.0.0a4/immuneML/config/default_params/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/preprocessing/duplicate_sequence_filter_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/preprocessing/sequence_length_filter_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.330245 immuneml-3.0.0a4/immuneML/config/default_params/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/amino_acid_frequency_distribution_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/coefficients_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/cv_feature_performance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/cytoscape_network_exporter_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/deep_rc_motif_discovery_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/design_matrix_exporter_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/feature_comparison_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/feature_value_barplot_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/ml_settings_performance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/motif_generalization_analysis_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/motif_overlap_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/motif_seed_recovery_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/motif_test_set_performance_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/receptor_dataset_overview_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/recovered_significant_features_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/reference_sequence_overlap_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/repertoire_clonotype_summary_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/sequence_length_distribution_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/significant_features_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/tcrdist_motif_discovery_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/reports/vj_gene_distribution_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.330245 immuneml-3.0.0a4/immuneML/config/default_params/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/simulation/ligo_sim_config_item_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/config/default_params/simulation/ligo_sim_config_params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.334245 immuneml-3.0.0a4/immuneML/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/DatasetItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/SequenceSet.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/bnp_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.334245 immuneml-3.0.0a4/immuneML/data_model/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/cell/Cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/cell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.334245 immuneml-3.0.0a4/immuneML/data_model/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6193 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/ElementDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/ReceptorDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/RepertoireDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/SequenceDataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.334245 immuneml-3.0.0a4/immuneML/data_model/encoded_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/encoded_data/EncodedData.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/encoded_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.338245 immuneml-3.0.0a4/immuneML/data_model/receptor/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/BCKReceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/BCReceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/ChainPair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/ElementGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/Receptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/ReceptorBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/RegionType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/TCABReceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/TCGDReceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.338245 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/Chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/SequenceFrameType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.338245 immuneml-3.0.0a4/immuneML/data_model/repertoire/
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/repertoire/Repertoire.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/data_model/repertoire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.338245 immuneml-3.0.0a4/immuneML/dev_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dev_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dev_util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.338245 immuneml-3.0.0a4/immuneML/dsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/DefaultParamsLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/ImmuneMLParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5885 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/InstructionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/ObjectParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/OutputParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.342245 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/DefinitionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/DefinitionParserOutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/EncodingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/ExampleWeightingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7118 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/MLParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/MotifParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/PreprocessingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/ReportParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/SignalParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14254 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/SimulationParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/definition_parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.342245 immuneml-3.0.0a4/immuneML/dsl/import_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/import_parsers/ImportParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/import_parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.342245 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ApplyGenModelParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ClusteringParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/DatasetExportParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/FeasibilitySummaryParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/LabelHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/LigoSimParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/MLApplicationParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/SubsamplingParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/TrainGenModelParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16322 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/TrainMLModelParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.342245 immuneml-3.0.0a4/immuneML/dsl/semantic_model/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/semantic_model/MLResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/semantic_model/SemanticModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/semantic_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.346245 immuneml-3.0.0a4/immuneML/dsl/symbol_table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/symbol_table/SymbolTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/symbol_table/SymbolTableEntry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/symbol_table/SymbolType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/dsl/symbol_table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.346245 immuneml-3.0.0a4/immuneML/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/DatasetEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/EncoderParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.346245 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19791 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13841 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.346245 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/RelativeAbundanceType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.346245 immuneml-3.0.0a4/immuneML/encodings/deeprc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/deeprc/DeepRCEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/deeprc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.350245 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/DistanceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/DistanceMetricType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/TCRdistEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/distance_encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.350245 immuneml-3.0.0a4/immuneML/encodings/evenness_profile/
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/evenness_profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.350245 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.350245 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/SequenceEncodingType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.350245 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)    22604 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/MotifEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/PositionalMotifHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/PositionalMotifParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/SimilarToPositiveSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/motif_encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.354246 immuneml-3.0.0a4/immuneML/encodings/onehot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotReceptorEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotRepertoireEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/onehot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.354246 immuneml-3.0.0a4/immuneML/encodings/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/preprocessing/FeatureScaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.354246 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)    15568 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/SequenceMatchingSummaryType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/reference_encoding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.354246 immuneml-3.0.0a4/immuneML/encodings/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/W2VRepertoireEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/W2VSequenceEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/Word2VecEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.354246 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.358245 immuneml-3.0.0a4/immuneML/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/EnvironmentSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/Label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/LabelConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/LabelType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/SequenceType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.358245 immuneml-3.0.0a4/immuneML/example_weighting/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/example_weighting/ExampleWeightingParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/example_weighting/ExampleWeightingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/example_weighting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.358245 immuneml-3.0.0a4/immuneML/example_weighting/predefined_weighting/
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/example_weighting/predefined_weighting/PredefinedWeighting.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/example_weighting/predefined_weighting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.358245 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/HPSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/HPSettingResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.358245 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/LeaveOneOutConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/ManualSplitConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/ReportConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/SplitConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/SplitType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.362246 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPAssessment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPSelection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7622 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.362246 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPAssessmentState.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPLabelState.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPSelectionState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/TrainMLModelState.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.362246 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/GridSearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.362246 immuneml-3.0.0a4/immuneML/ml_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.366246 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/AtchleyKmerMILClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18207 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/BinaryFeatureClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23880 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/DeepRC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/KNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/KerasSequenceCNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16032 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/MLMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/PrecomputedKNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19299 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/ProbabilisticBinaryClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/ReceptorCNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SVC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SVM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14312 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SklearnMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/TCRdistClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/classifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.366246 immuneml-3.0.0a4/immuneML/ml_methods/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/clustering/ClusteringMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/clustering/KMeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.366246 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/DimRedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/PCA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/TSNE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/UMAP.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.366246 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/BackgroundSequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/ExperimentalImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/GenerativeModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/InternalOlgaModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/OLGA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/PWM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SimpleLSTM.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17876 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SimpleVAE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SoNNia.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/generative_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.370246 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/SimpleLSTMGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/SimpleVAEGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.370246 immuneml-3.0.0a4/immuneML/ml_methods/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/util/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_methods/util/pytorch_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.370246 immuneml-3.0.0a4/immuneML/ml_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_metrics/ClassificationMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_metrics/ClusteringMetric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_metrics/MetricUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/ml_metrics/ml_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.370246 immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/ComparisonData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.370246 immuneml-3.0.0a4/immuneML/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/ReferenceSequenceAnnotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/SubjectRepertoireCollector.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.374246 immuneml-3.0.0a4/immuneML/preprocessing/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/ChainRepertoireFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/CountAggregationFunction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/CountPerSequenceFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/DuplicateSequenceFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/MetadataRepertoireFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4282 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/SequenceLengthFilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/preprocessing/filters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.374246 immuneml-3.0.0a4/immuneML/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/InstructionPresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/PresentationFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/PresentationFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/TemplateParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.378246 immuneml-3.0.0a4/immuneML/presentation/html/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/ClusteringHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/DatasetExportHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/FeasibilitySummaryHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/GenModelHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21405 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/HPHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/HTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/LIgOSimulationHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/MLApplicationHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/SubsamplingHTMLBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.378246 immuneml-3.0.0a4/immuneML/presentation/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/AssessmentSplitDetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/Clustering.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/DatasetExport.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/ExploratoryAnalysis.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/FeasibilitySummary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/GenModel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/HPOptimization.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/MLApplication.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/MLTraining.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/MultiDatasetBenchmark.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/Reports.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/SelectionDetails.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/Simulation.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/Subsampling.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.378246 immuneml-3.0.0a4/immuneML/presentation/html/templates/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/presentation/html/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.382246 immuneml-3.0.0a4/immuneML/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/PlotlyUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7418 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/Report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ReportOutput.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ReportResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ReportUtil.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.382246 immuneml-3.0.0a4/immuneML/reports/clustering_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/clustering_reports/ClusteringReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/clustering_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.382246 immuneml-3.0.0a4/immuneML/reports/data_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)    16331 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/DataReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/GLIPH2Exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26131 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/MotifGeneralizationAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/ReceptorDatasetOverview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12770 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/RecoveredSignificantFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/RepertoireClonotypeSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/SequenceLengthDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/SequencesWithSignificantKmers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13084 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/SignificantFeatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/SignificantKmerPositions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/SimpleDatasetOverview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19278 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/VJGeneDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/data_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.386246 immuneml-3.0.0a4/immuneML/reports/encoding_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/DesignMatrixExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/EncodingReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureComparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureDistribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureValueBarplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/GroundTruthMotifOverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/Matches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/MotifTestSetPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/NonMotifSequenceSimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11514 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/PositionalMotifFrequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/RelevantSequenceExporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/encoding_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.386246 immuneml-3.0.0a4/immuneML/reports/gen_model_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/gen_model_reports/GenModelReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/gen_model_reports/VAESummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/gen_model_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.390246 immuneml-3.0.0a4/immuneML/reports/ml_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/BinaryFeaturePrecisionRecall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/CoefficientPlottingSetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/Coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6121 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/ConfounderAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15792 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/KernelSequenceLogo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/MLReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/MotifSeedRecovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/ROCCurve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/TrainingPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/ml_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.390246 immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/PerformanceOverview.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.390246 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.390246 immuneml-3.0.0a4/immuneML/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/LigoSimState.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/SimConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/SimConfigItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.390246 immuneml-3.0.0a4/immuneML/simulation/dataset_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14829 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/dataset_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.394246 immuneml-3.0.0a4/immuneML/simulation/implants/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/ImplantAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/LigoPWM.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/Motif.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/MotifInstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/SeedMotif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/Signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/implants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.394246 immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)    11517 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/ImplantingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/RejectionSamplingStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/SimulationStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.394246 immuneml-3.0.0a4/immuneML/simulation/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/util/bnp_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5363 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/util/igor_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25998 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/simulation/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.398246 immuneml-3.0.0a4/immuneML/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/AdaptiveImportHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/CompAIRRHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/CompAIRRParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/DistanceMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/DocEnumHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/EncoderHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/ExporterHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/FilenameHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26551 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/ImportHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/KmerHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/MotifPerformancePlotHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/NameBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/NumpyHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/ParameterValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/PathBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/PositionHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/ReadsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/ReflectionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/RepertoireBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/SequenceAnalysisHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/SignificantFeaturesHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/StringHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/TCRdistHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.398246 immuneml-3.0.0a4/immuneML/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.398246 immuneml-3.0.0a4/immuneML/workflows/instructions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/GenModelInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/Instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/MLProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/TrainMLModelInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/apply_gen_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/apply_gen_model/ApplyGenModelInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/apply_gen_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)     9852 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/ClusteringInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/clustering_run_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/dataset_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/dataset_generation/DatasetExportState.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/dataset_generation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisState.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/
+-rw-r--r--   0 runner    (1001) docker     (127)    13733 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)    24294 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/LigoSimInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/runtime_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.402246 immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/quickstart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.406246 immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/SubsamplingState.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.406246 immuneml-3.0.0a4/immuneML/workflows/instructions/train_gen_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/train_gen_model/TrainGenModelInstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/instructions/train_gen_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.406246 immuneml-3.0.0a4/immuneML/workflows/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/DataEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/DataEncoderParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/DataWeighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/DataWeighterParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodAssessment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodAssessmentParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodTrainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodTrainerParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/Step.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/StepParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.406246 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/DataSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/DataSplitterParams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/ManualSplitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/Util.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.410246 immuneml-3.0.0a4/immuneML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 16:11:26.000000 immuneml-3.0.0a4/immuneML.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:26.410246 immuneml-3.0.0a4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/DocumentatonFormat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/check_new_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17505 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/check_new_ml_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/checker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/specification_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/scripts/specs_docs_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:11:26.410246 immuneml-3.0.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-26 16:11:22.000000 immuneml-3.0.0a4/setup.py
```

### Comparing `immuneML-3.0.0a3/LICENSE.md` & `immuneml-3.0.0a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/PKG-INFO` & `immuneml-3.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immuneML
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: immuneML is a software platform for machine learning analysis of immune receptor repertoires.
 Home-page: https://github.com/uio-bmi/immuneML
 Author: immuneML Team
 Author-email: milenpa@student.matnat.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `immuneML-3.0.0a3/README.md` & `immuneml-3.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_export/AIRRExporter.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_export/AIRRExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_export/ImmuneMLExporter.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_export/ImmuneMLExporter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/AIRRImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/AIRRImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     immune receptors respectively, like antigen specificity.
 
     The AIRR .tsv format is explained here: https://docs.airr-community.org/en/stable/datarep/format.html
     And the AIRR rearrangement schema can be found here: https://docs.airr-community.org/en/stable/datarep/rearrangements.html
 
     When importing a ReceptorDataset, the AIRR field cell_id is used to determine the chain pairs.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with AIRR files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset or ReceptorDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the AIRR files included under the column 'filename' are imported into the RepertoireDataset. For setting SequenceDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -64,41 +64,43 @@
     - column_mapping_synonyms (dict): This is a column mapping that can be used if a column could have alternative names. The formatting is the same as column_mapping. If some columns specified in column_mapping are not found in the file, the columns specified in column_mapping_synonyms are instead attempted to be loaded. For AIRR format, there is no default column_mapping_synonyms.
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are AIRR column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. This parameter can also be used to specify sequence-level metadata columns for RepertoireDatasets, which can be used by reports. To set prediction label metadata for RepertoireDatasets, see metadata_file instead. For AIRR format, there is no default metadata_column_mapping.
 
     - separator (str): Column separator, for AIRR this is by default "\\t".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_airr_dataset:
-            format: AIRR
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                metadata_column_mapping: # metadata column mapping AIRR: immuneML for Sequence- or ReceptorDatasetDataset
-                    airr_column_name1: metadata_label1
-                    airr_column_name2: metadata_label2
-                import_productive: True # whether to include productive sequences in the dataset
-                import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
-                import_out_of_frame: False # whether to include out of frame sequences in the dataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even if the `sequences` column is empty (provided that other fields are as specified here)
-                import_empty_aa_sequences: False # remove all sequences with empty `sequence_aa` column
-                # Optional fields with AIRR-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping AIRR: immuneML
-                    junction: sequence
-                    junction_aa: sequence_aa
-                    locus: chain
+        definitions:
+            datasets:
+                my_airr_dataset:
+                    format: AIRR
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping AIRR: immuneML for Sequence- or ReceptorDatasetDataset
+                            airr_column_name1: metadata_label1
+                            airr_column_name2: metadata_label2
+                        import_productive: True # whether to include productive sequences in the dataset
+                        import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
+                        import_out_of_frame: False # whether to include out of frame sequences in the dataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even if the `sequences` column is empty (provided that other fields are as specified here)
+                        import_empty_aa_sequences: False # remove all sequences with empty `sequence_aa` column
+                        # Optional fields with AIRR-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping AIRR: immuneML
+                            junction: sequence
+                            junction_aa: sequence_aa
+                            locus: chain
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(AIRRImport, params, dataset_name)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/DatasetImportParams.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/DatasetImportParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/GenericImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/GenericImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     and can therefore be tailored to import data from various different tabular files with headers.
 
     For ReceptorDatasets: this importer assumes the two receptor sequences appear on different lines in the file, and can
     be paired together by a common sequence identifier. If you instead want to import a ReceptorDataset from a tabular
     file that contains both receptor chains on one line, see :ref:`SingleLineReceptor` import
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset or ReceptorDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. For setting Sequence- or ReceptorDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -65,45 +65,47 @@
                 file_column_antigen_specificity: antigen_specificity
 
     - columns_to_load (list): Optional; specifies which columns to load from the input file. This may be useful if the input files contain many unused columns. If no value is specified, all columns are loaded.
 
     - separator (str): Required parameter. Column separator, for example "\\t" or ",". The default value is "\\t"
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_generic_dataset:
-            format: Generic
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
-                receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
-                separator: "\\t" # column separator
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping file: immuneML
-                    file_column_amino_acids: sequence_aas
-                    file_column_v_genes: v_call
-                    file_column_j_genes: j_call
-                    file_column_frequencies: duplicate_count
-                metadata_column_mapping: # metadata column mapping file: immuneML
-                    file_column_antigen_specificity: antigen_specificity
-                columns_to_load:  # which subset of columns to load from the file
-                    - file_column_amino_acids
-                    - file_column_v_genes
-                    - file_column_j_genes
-                    - file_column_frequencies
-                    - file_column_antigen_specificity
+        definitions:
+            datasets:
+                my_generic_dataset:
+                    format: Generic
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
+                        receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
+                        separator: "\\t" # column separator
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping file: immuneML
+                            file_column_amino_acids: sequence_aas
+                            file_column_v_genes: v_call
+                            file_column_j_genes: j_call
+                            file_column_frequencies: duplicate_count
+                        metadata_column_mapping: # metadata column mapping file: immuneML
+                            file_column_antigen_specificity: antigen_specificity
+                        columns_to_load:  # which subset of columns to load from the file
+                            - file_column_amino_acids
+                            - file_column_v_genes
+                            - file_column_j_genes
+                            - file_column_frequencies
+                            - file_column_antigen_specificity
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(GenericImport, params, dataset_name)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/IGoRImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/IGoRImport.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Sequences with missing anchors are not imported, meaning only sequences with value '1' in the anchors_found column are imported.
     Nucleotide sequences are automatically translated to amino acid sequences.
 
     Reference: Quentin Marcou, Thierry Mora, Aleksandra M. Walczak
     ‘High-throughput immune repertoire analysis with IGoR’. Nature Communications, (2018)
     `doi.org/10.1038/s41467-018-02832-w <https://doi.org/10.1038/s41467-018-02832-w>`_.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with IGoR files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the IGoR files included under the column 'filename' are imported into the RepertoireDataset. For setting SequenceDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -53,38 +53,40 @@
     - column_mapping_synonyms (dict): This is a column mapping that can be used if a column could have alternative names. The formatting is the same as column_mapping. If some columns specified in column_mapping are not found in the file, the columns specified in column_mapping_synonyms are instead attempted to be loaded. For IGoR format, there is no default column_mapping_synonyms.
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are IGoR column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. This parameter can also be used to specify sequence-level metadata columns for RepertoireDatasets, which can be used by reports. To set prediction label metadata for RepertoireDatasets, see metadata_file instead. For IGoR format, there is no default metadata_column_mapping.
 
     - separator (str): Column separator, for IGoR this is by default ",".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_igor_dataset:
-            format: IGoR
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                metadata_column_mapping: # metadata column mapping IGoR: immuneML for SequenceDataset
-                    igor_column_name1: metadata_label1
-                    igor_column_name2: metadata_label2
-                import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
-                import_out_of_frame: False # whether to include out of frame sequences in the dataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                # Optional fields with IGoR-specific defaults, only change when different behavior is required:
-                separator: "," # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping IGoR: immuneML
-                    nt_CDR3: sequences
-                    seq_index: sequence_identifiers
+        definitions:
+            datasets:
+                my_igor_dataset:
+                    format: IGoR
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping IGoR: immuneML for SequenceDataset
+                            igor_column_name1: metadata_label1
+                            igor_column_name2: metadata_label2
+                        import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
+                        import_out_of_frame: False # whether to include out of frame sequences in the dataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        # Optional fields with IGoR-specific defaults, only change when different behavior is required:
+                        separator: "," # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping IGoR: immuneML
+                            nt_CDR3: sequences
+                            seq_index: sequence_identifiers
 
     """
     CODON_TABLE = {
         'ATA': 'I', 'ATC': 'I', 'ATT': 'I', 'ATG': 'M',
         'ACA': 'T', 'ACC': 'T', 'ACG': 'T', 'ACT': 'T',
         'AAC': 'N', 'AAT': 'N', 'AAA': 'K', 'AAG': 'K',
         'AGC': 'S', 'AGT': 'S', 'AGA': 'R', 'AGG': 'R',
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/IReceptorImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/IReceptorImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     immune receptors respectively, like antigen specificity.
 
     AIRR rearrangement schema can be found here: https://docs.airr-community.org/en/stable/datarep/rearrangements.html
 
     When importing a ReceptorDataset, the AIRR field cell_id is used to determine the chain pairs.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): This is the path to a directory **with .zip files** retrieved from the iReceptor Gateway. These .zip files should include AIRR files (with .tsv extension) and corresponding metadata.json files with matching names (e.g., for my_dataset.tsv the corresponding metadata file is called my_dataset-metadata.json). The zip files must use the .zip extension.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset or ReceptorDataset. By default, is_repertoire is set to True.
 
     - paired (str): Required for Sequence- or ReceptorDatasets. This parameter determines whether to import a SequenceDataset (paired = False) or a ReceptorDataset (paired = True). In a ReceptorDataset, two sequences with chain types specified by receptor_chains are paired together based on the identifier given in the AIRR column named 'cell_id'.
 
@@ -76,44 +76,46 @@
     - column_mapping_synonyms (dict): This is a column mapping that can be used if a column could have alternative names. The formatting is the same as column_mapping. If some columns specified in column_mapping are not found in the file, the columns specified in column_mapping_synonyms are instead attempted to be loaded. For AIRR format, there is no default column_mapping_synonyms.
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are AIRR column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. For AIRR format, there is no default metadata_column_mapping. When importing a RepertoireDataset, the metadata is automatically extracted from the metadata json files.
 
     - separator (str): Column separator, for AIRR this is by default "\\t".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_airr_dataset:
-            format: IReceptor
-            params:
-                path: path/to/zipfiles/
-                is_repertoire: True # whether to import a RepertoireDataset
-                metadata_column_mapping: # metadata column mapping AIRR: immuneML for Sequence- or ReceptorDatasetDataset
-                    airr_column_name1: metadata_label1
-                    airr_column_name2: metadata_label2
-                import_productive: True # whether to include productive sequences in the dataset
-                import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
-                import_out_of_frame: False # whether to include out of frame sequences in the dataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even if the `sequences` column is empty (provided that other fields are as specified here)
-                import_empty_aa_sequences: False # remove all sequences with empty `sequence_aas` column
-                # Optional fields with AIRR-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping AIRR: immuneML
-                    junction: sequences
-                    junction_aa: sequence_aas
-                    v_call: v_alleles
-                    j_call: j_alleles
-                    locus: chains
-                    duplicate_count: counts
-                    sequence_id: sequence_identifiers
+        definitions:
+            datasets:
+                my_airr_dataset:
+                    format: IReceptor
+                    params:
+                        path: path/to/zipfiles/
+                        is_repertoire: True # whether to import a RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping AIRR: immuneML for Sequence- or ReceptorDatasetDataset
+                            airr_column_name1: metadata_label1
+                            airr_column_name2: metadata_label2
+                        import_productive: True # whether to include productive sequences in the dataset
+                        import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
+                        import_out_of_frame: False # whether to include out of frame sequences in the dataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even if the `sequences` column is empty (provided that other fields are as specified here)
+                        import_empty_aa_sequences: False # remove all sequences with empty `sequence_aas` column
+                        # Optional fields with AIRR-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping AIRR: immuneML
+                            junction: sequences
+                            junction_aa: sequence_aas
+                            v_call: v_alleles
+                            j_call: j_alleles
+                            locus: chains
+                            duplicate_count: counts
+                            sequence_id: sequence_identifiers
 
     """
     REPERTOIRES_FOLDER = "repertoires/"
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         if params["is_repertoire"]:
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmuneMLImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmuneMLImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,34 +35,36 @@
     2. a csv metadata file (only for repertoire datasets, should be in the same folder as the iml_dataset file),
 
     3. data files for different types of data. For repertoire datasets, data files include one binary numpy file per
        repertoire with sequences and associated information and one metadata yaml file per repertoire with details
        such as repertoire identifier, disease status, subject id and other similar available information. For sequence
        and receptor datasets, sequences or receptors respectively, are stored in batches in binary numpy files.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): The path to the previously created dataset file. This file should have an '.yaml' extension. If the
       path has not been specified, immuneML attempts to load the dataset from a specified metadata file (only for
       RepertoireDatasets).
 
     - metadata_file (str): An optional metadata file for a RepertoireDataset. If specified, the RepertoireDataset
       metadata will be updated to the newly specified metadata without otherwise changing the Repertoire objects
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_dataset:
-            format: ImmuneML
-            params:
-                path: path/to/dataset.yaml
-                metadata_file: path/to/metadata.csv
+        definitions:
+            datasets:
+                my_dataset:
+                    format: ImmuneML
+                    params:
+                        path: path/to/dataset.yaml
+                        metadata_file: path/to/metadata.csv
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         iml_params = DatasetImportParams.build_object(**params)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmunoSEQRearrangementImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     The format of the files imported by this importer is described here:
     https://www.adaptivebiotech.com/wp-content/uploads/2019/07/MRK-00342_immunoSEQ_TechNote_DataExport_WEB_REV.pdf
     Alternatively, to import sample-level .tsv files, see :ref:`ImmunoSEQSample` import
 
     The only difference between these two importers is which columns they load from the .tsv files.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the files included under the column 'filename' are imported into the RepertoireDataset. For setting SequenceDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -74,56 +74,58 @@
     - separator (str): Column separator, for ImmunoSEQ files this is by default "\\t".
 
     - import_empty_nt_sequences (bool): imports sequences which have an empty nucleotide sequence field; can be True or False
 
     - import_empty_aa_sequences (bool): imports sequences which have an empty amino acid sequence field; can be True or False; for analysis on amino acid sequences, this parameter will typically be False (import only non-empty amino acid sequences)
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_immunoseq_dataset:
-            format: ImmunoSEQRearrangement
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                metadata_column_mapping: # metadata column mapping ImmunoSEQ: immuneML for SequenceDataset
-                    immunoseq_column_name1: metadata_label1
-                    immunoseq_column_name2: metadata_label2
-                import_productive: True # whether to include productive sequences in the dataset
-                import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
-                import_out_of_frame: False # whether to include out of frame sequences in the dataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with ImmunoSEQ rearrangement-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                columns_to_load: # subset of columns to load
-                - rearrangement
-                - v_family
-                - v_gene
-                - v_resolved
-                - j_family
-                - j_gene
-                - j_resolved
-                - amino_acid
-                - templates
-                - frame_type
-                - locus
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping immunoSEQ: immuneML
-                    rearrangement: sequence
-                    amino_acid: sequence_aa
-                    v_resolved: v_call
-                    j_resolved: j_call
-                    templates: duplicate_count
-                    locus: chain
+        definitions:
+            datasets:
+                my_immunoseq_dataset:
+                    format: ImmunoSEQRearrangement
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping ImmunoSEQ: immuneML for SequenceDataset
+                            immunoseq_column_name1: metadata_label1
+                            immunoseq_column_name2: metadata_label2
+                        import_productive: True # whether to include productive sequences in the dataset
+                        import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
+                        import_out_of_frame: False # whether to include out of frame sequences in the dataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with ImmunoSEQ rearrangement-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        columns_to_load: # subset of columns to load
+                        - rearrangement
+                        - v_family
+                        - v_gene
+                        - v_resolved
+                        - j_family
+                        - j_gene
+                        - j_resolved
+                        - amino_acid
+                        - templates
+                        - frame_type
+                        - locus
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping immunoSEQ: immuneML
+                            rearrangement: sequence
+                            amino_acid: sequence_aa
+                            v_resolved: v_call
+                            j_resolved: j_call
+                            templates: duplicate_count
+                            locus: chain
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(ImmunoSEQRearrangementImport, params, dataset_name)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/ImmunoSEQSampleImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     The format of the files imported by this importer is described here in section 3.4.13
     https://clients.adaptivebiotech.com/assets/downloads/immunoSEQ_AnalyzerManual.pdf
     Alternatively, to import rearrangement-level .tsv files, see :ref:`ImmunoSEQRearrangement` import.
     The only difference between these two importers is which columns they load from the .tsv files.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the files included under the column 'filename' are imported into the RepertoireDataset. For setting SequenceDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -67,59 +67,61 @@
     - columns_to_load (list): Specifies which subset of columns must be loaded from the file. By default, this is: [nucleotide, aminoAcid, count (templates/reads), vFamilyName, vGeneName, vGeneAllele, jFamilyName, jGeneName, jGeneAllele, sequenceStatus]; these are the columns from the original file that will be imported
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are immunoSEQ column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. This parameter can also be used to specify sequence-level metadata columns for RepertoireDatasets, which can be used by reports. To set prediction label metadata for RepertoireDatasets, see metadata_file instead. For immunoSEQ sample .tsv files, there is no default metadata_column_mapping.
 
     - separator (str): Column separator, for ImmunoSEQ files this is by default "\\t".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_immunoseq_dataset:
-            format: ImmunoSEQSample
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                metadata_column_mapping: # metadata column mapping ImmunoSEQ: immuneML for SequenceDataset
-                    immunoseq_column_name1: metadata_label1
-                    immunoseq_column_name2: metadata_label2
-                import_productive: True # whether to include productive sequences in the dataset
-                import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
-                import_out_of_frame: False # whether to include out of frame sequences in the dataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with ImmunoSEQ sample-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                columns_to_load: # subset of columns to load
-                - nucleotide
-                - aminoAcid
-                - count (templates/reads)
-                - vFamilyName
-                - vGeneName
-                - vGeneAllele
-                - jFamilyName
-                - jGeneName
-                - jGeneAllele
-                - sequenceStatus
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping immunoSEQ: immuneML
-                    nucleotide: sequence
-                    aminoAcid: sequence_aa
-                    vGeneName: v_call
-                    jGeneName: j_call
-                    sequenceStatus: frame_type
-                    vFamilyName: v_family
-                    jFamilyName: j_family
-                    vGeneAllele: v_allele
-                    jGeneAllele: j_allele
-                    count (templates/reads): duplicate_count
+        definitions:
+            datasets:
+                my_immunoseq_dataset:
+                    format: ImmunoSEQSample
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping ImmunoSEQ: immuneML for SequenceDataset
+                            immunoseq_column_name1: metadata_label1
+                            immunoseq_column_name2: metadata_label2
+                        import_productive: True # whether to include productive sequences in the dataset
+                        import_with_stop_codon: False # whether to include sequences with stop codon in the dataset
+                        import_out_of_frame: False # whether to include out of frame sequences in the dataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with ImmunoSEQ sample-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        columns_to_load: # subset of columns to load
+                        - nucleotide
+                        - aminoAcid
+                        - count (templates/reads)
+                        - vFamilyName
+                        - vGeneName
+                        - vGeneAllele
+                        - jFamilyName
+                        - jGeneName
+                        - jGeneAllele
+                        - sequenceStatus
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping immunoSEQ: immuneML
+                            nucleotide: sequence
+                            aminoAcid: sequence_aa
+                            vGeneName: v_call
+                            jGeneName: j_call
+                            sequenceStatus: frame_type
+                            vFamilyName: v_family
+                            jFamilyName: j_family
+                            vGeneAllele: v_allele
+                            jGeneAllele: j_allele
+                            count (templates/reads): duplicate_count
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(ImmunoSEQSampleImport, params, dataset_name)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/MiXCRImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/MiXCRImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Imports data in MiXCR format into a Repertoire-, or SequenceDataset.
     RepertoireDatasets should be used when making predictions per repertoire, such as predicting a disease state.
     SequenceDatasets should be used when predicting values for unpaired (single-chain) immune receptors, like
     antigen specificity.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with MiXCR files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the MiXCR files included under the column 'filename' are imported into the RepertoireDataset. For setting SequenceDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -48,44 +48,46 @@
     - columns_to_load (list): Specifies which subset of columns must be loaded from the MiXCR file. By default, this is: [cloneCount, allVHitsWithScore, allJHitsWithScore, aaSeqCDR3, nSeqCDR3]
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are MiXCR column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. This parameter can also be used to specify sequence-level metadata columns for RepertoireDatasets, which can be used by reports. To set prediction label metadata for RepertoireDatasets, see metadata_file instead. For MiXCR format, there is no default metadata_column_mapping.
 
     - separator (str): Column separator, for MiXCR this is by default "\\t".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_mixcr_dataset:
-            format: MiXCR
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                metadata_column_mapping: # metadata column mapping MiXCR: immuneML for SequenceDataset
-                    mixcrColumnName1: metadata_label1
-                    mixcrColumnName2: metadata_label2
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with MiXCR-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                columns_to_load: # subset of columns to load, sequence columns are handled by region_type parameter
-                - cloneCount
-                - allVHitsWithScore
-                - allJHitsWithScore
-                - aaSeqCDR3
-                - nSeqCDR3
-                column_mapping: # column mapping MiXCR: immuneML
-                    cloneCount: duplicate_count
-                    allVHitsWithScore: v_call
-                    allJHitsWithScore: j_call
+        definitions:
+            datasets:
+                my_mixcr_dataset:
+                    format: MiXCR
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        metadata_column_mapping: # metadata column mapping MiXCR: immuneML for SequenceDataset
+                            mixcrColumnName1: metadata_label1
+                            mixcrColumnName2: metadata_label2
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with MiXCR-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        columns_to_load: # subset of columns to load, sequence columns are handled by region_type parameter
+                        - cloneCount
+                        - allVHitsWithScore
+                        - allJHitsWithScore
+                        - aaSeqCDR3
+                        - nSeqCDR3
+                        column_mapping: # column mapping MiXCR: immuneML
+                            cloneCount: duplicate_count
+                            allVHitsWithScore: v_call
+                            allJHitsWithScore: j_call
 
     """
 
     SEQUENCE_NAME_MAP = {
         RegionType.IMGT_CDR3: {"AA": "aaSeqCDR3", "NT": "nSeqCDR3"},
         RegionType.IMGT_CDR1: {"AA": "aaSeqCDR1", "NT": "nSeqCDR1"},
         RegionType.IMGT_CDR2: {"AA": "aaSeqCDR2", "NT": "nSeqCDR2"},
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/OLGAImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/OLGAImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Imports data generated by `OLGA <https://github.com/statbiophys/OLGA>`_ simulations into a Repertoire-, or SequenceDataset. Assumes that the columns in each
     file correspond to: nucleotide sequences, amino acid sequences, v genes, j genes
 
     Reference: Sethna, Zachary et al.
     ‘High-throughput immune repertoire analysis with IGoR’. Bioinformatics, (2019)
     `doi.org/10.1093/bioinformatics/btz035 <https://doi.org/10.1093/bioinformatics/btz035>`_.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with OLGA files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. Only the OLGA files included under the column 'filename' are imported into the RepertoireDataset. SequenceDataset metadata is currently not supported.
 
@@ -34,37 +34,39 @@
     - region_type (str): Which part of the sequence to import. By default, this value is set to IMGT_CDR3. This means the first and last amino acids are removed from the CDR3 sequence, as OLGA uses the IMGT junction. Specifying any other value will result in importing the sequences as they are. Valid values for region_type are the names of the :py:obj:`~immuneML.data_model.receptor.RegionType.RegionType` enum.
 
     - separator (str): Column separator, for OLGA this is by default "\\t".
 
     - column_mapping (dict): defines which columns to import from olga format: keys are the number of the columns and values are the names of the columns to be mapped to
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_olga_dataset:
-            format: OLGA
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with OLGA-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                columns_to_load: [0, 1, 2, 3]
-                column_mapping:
-                    0: sequence
-                    1: sequence_aa
-                    2: v_call
-                    3: j_call
+        definitions:
+            datasets:
+                my_olga_dataset:
+                    format: OLGA
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset (True) or a SequenceDataset (False)
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with OLGA-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        columns_to_load: [0, 1, 2, 3]
+                        column_mapping:
+                            0: sequence
+                            1: sequence_aa
+                            2: v_call
+                            3: j_call
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
 
         assert sorted(params["columns_to_load"]) == sorted(list(params["column_mapping"].keys()))
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomReceptorDatasetImport.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class RandomReceptorDatasetImport(DataImport):
     """
     Returns a ReceptorDataset consisting of randomly generated sequences, which can be used for benchmarking purposes.
     The sequences consist of uniformly chosen amino acids or nucleotides.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - receptor_count (int): The number of receptors the ReceptorDataset should contain.
 
     - chain_1_length_probabilities (dict): A mapping where the keys correspond to different sequence lengths for chain 1, and the values are the probabilities for choosing each sequence length. For example, to create a random ReceptorDataset where 40% of the sequences for chain 1 would be of length 10, and 60% of the sequences would have length 12, this mapping would need to be specified:
 
         .. indent with spaces
         .. code-block:: yaml
@@ -30,45 +30,47 @@
         .. code-block:: yaml
 
                 cmv_epitope:
                     binding: 0.7
                     not_binding: 0.3
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_random_dataset:
-            format: RandomReceptorDataset
-            params:
-                receptor_count: 100 # number of random receptors to generate
-                chain_1_length_probabilities:
-                    14: 0.8 # 80% of all generated sequences for all receptors (for chain 1) will have length 14
-                    15: 0.2 # 20% of all generated sequences across all receptors (for chain 1) will have length 15
-                chain_2_length_probabilities:
-                    14: 0.8 # 80% of all generated sequences for all receptors (for chain 2) will have length 14
-                    15: 0.2 # 20% of all generated sequences across all receptors (for chain 2) will have length 15
-                labels:
-                    epitope1: # label name
-                        True: 0.5 # 50% of the receptors will have class True
-                        False: 0.5 # 50% of the receptors will have class False
-                    epitope2: # next label with classes that will be assigned to receptors independently of the previous label or other parameters
-                        1: 0.3 # 30% of the generated receptors will have class 1
-                        0: 0.7 # 70% of the generated receptors will have class 0
+        definitions:
+            datasets:
+                my_random_dataset:
+                    format: RandomReceptorDataset
+                    params:
+                        receptor_count: 100 # number of random receptors to generate
+                        chain_1_length_probabilities:
+                            14: 0.8 # 80% of all generated sequences for all receptors (for chain 1) will have length 14
+                            15: 0.2 # 20% of all generated sequences across all receptors (for chain 1) will have length 15
+                        chain_2_length_probabilities:
+                            14: 0.8 # 80% of all generated sequences for all receptors (for chain 2) will have length 14
+                            15: 0.2 # 20% of all generated sequences across all receptors (for chain 2) will have length 15
+                        labels:
+                            epitope1: # label name
+                                True: 0.5 # 50% of the receptors will have class True
+                                False: 0.5 # 50% of the receptors will have class False
+                            epitope2: # next label with classes that will be assigned to receptors independently of the previous label or other parameters
+                                1: 0.3 # 30% of the generated receptors will have class 1
+                                0: 0.7 # 70% of the generated receptors will have class 0
 
     """
 
     @staticmethod
     def import_dataset(params, name: str) -> ReceptorDataset:
         """
         Returns randomly generated receptor dataset according to the parameters;
 
-        YAML specification:
+        **YAML specification:**
 
             result_path: path/where/to/store/results/
             receptor_count: 100 # number of random receptors to generate
             chain_1_length_probabilities:
                 14: 0.8 # 80% of all generated sequences for all receptors (for chain 1) will have length 14
                 15: 0.2 # 20% of all generated sequences across all receptors (for chain 1) will have length 15
             chain_2_length_probabilities:
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomRepertoireDatasetImport.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class RandomRepertoireDatasetImport(DataImport):
     """
     Returns a RepertoireDataset consisting of randomly generated sequences, which can be used for benchmarking purposes.
     The sequences consist of uniformly chosen amino acids or nucleotides.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - repertoire_count (int): The number of repertoires the RepertoireDataset should contain.
 
     - sequence_count_probabilities (dict): A mapping where the keys are the number of sequences per repertoire, and the values are the probabilities that any of the repertoires would have that number of sequences. For example, to create a random RepertoireDataset where 40% of the repertoires would have 1000 sequences, and the other 60% would have 1100 sequences, this mapping would need to be specified:
 
         .. indent with spaces
         .. code-block:: yaml
@@ -35,33 +35,35 @@
         .. code-block:: yaml
 
                 CMV:
                     cmv_positive: 0.7
                     cmv_negative: 0.3
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_random_dataset:
-            format: RandomRepertoireDataset
-            params:
-                repertoire_count: 100 # number of random repertoires to generate
-                sequence_count_probabilities:
-                    10: 0.5 # probability that any of the repertoires would have 10 receptor sequences
-                    20: 0.5
-                sequence_length_probabilities:
-                    10: 0.5 # probability that any of the receptor sequences would be 10 amino acids in length
-                    12: 0.5
-                labels: # randomly assigned labels (only useful for simple benchmarking)
-                    cmv:
-                        True: 0.5 # probability of value True for label cmv to be assigned to any repertoire
-                        False: 0.5
+        definitions:
+            datasets:
+                my_random_dataset:
+                    format: RandomRepertoireDataset
+                    params:
+                        repertoire_count: 100 # number of random repertoires to generate
+                        sequence_count_probabilities:
+                            10: 0.5 # probability that any of the repertoires would have 10 receptor sequences
+                            20: 0.5
+                        sequence_length_probabilities:
+                            10: 0.5 # probability that any of the receptor sequences would be 10 amino acids in length
+                            12: 0.5
+                        labels: # randomly assigned labels (only useful for simple benchmarking)
+                            cmv:
+                                True: 0.5 # probability of value True for label cmv to be assigned to any repertoire
+                                False: 0.5
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> RepertoireDataset:
         valid_keys = ["result_path", "repertoire_count", "sequence_count_probabilities", "sequence_length_probabilities", "labels"]
         ParameterValidator.assert_all_in_valid_list(list(params.keys()), valid_keys, "RandomRepertoireDatasetImport", "params")
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/RandomSequenceDatasetImport.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class RandomSequenceDatasetImport(DataImport):
     """
     Returns a SequenceDataset consisting of randomly generated sequences, which can be used for benchmarking purposes.
     The sequences consist of uniformly chosen amino acids or nucleotides.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - sequence_count (int): The number of sequences the SequenceDataset should contain.
 
     - length_probabilities (dict): A mapping where the keys correspond to different sequence lengths and the values are the probabilities for choosing each sequence length. For example, to create a random SequenceDataset where 40% of the sequences would be of length 10, and 60% of the sequences would have length 12, this mapping would need to be specified:
 
         .. indent with spaces
         .. code-block:: yaml
@@ -28,41 +28,43 @@
         .. code-block:: yaml
 
                 cmv_epitope:
                     binding: 0.7
                     not_binding: 0.3
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_random_dataset:
-            format: RandomSequenceDataset
-            params:
-                sequence_count: 100 # number of random sequences to generate
-                length_probabilities:
-                    14: 0.8 # 80% of all generated sequences for all sequences will have length 14
-                    15: 0.2 # 20% of all generated sequences across all sequences will have length 15
-                labels:
-                    epitope1: # label name
-                        True: 0.5 # 50% of the sequences will have class True
-                        False: 0.5 # 50% of the sequences will have class False
-                    epitope2: # next label with classes that will be assigned to sequences independently of the previous label or other parameters
-                        1: 0.3 # 30% of the generated sequences will have class 1
-                        0: 0.7 # 70% of the generated sequences will have class 0
+        definitions:
+            datasets:
+                my_random_dataset:
+                    format: RandomSequenceDataset
+                    params:
+                        sequence_count: 100 # number of random sequences to generate
+                        length_probabilities:
+                            14: 0.8 # 80% of all generated sequences for all sequences will have length 14
+                            15: 0.2 # 20% of all generated sequences across all sequences will have length 15
+                        labels:
+                            epitope1: # label name
+                                True: 0.5 # 50% of the sequences will have class True
+                                False: 0.5 # 50% of the sequences will have class False
+                            epitope2: # next label with classes that will be assigned to sequences independently of the previous label or other parameters
+                                1: 0.3 # 30% of the generated sequences will have class 1
+                                0: 0.7 # 70% of the generated sequences will have class 0
     """
 
     @staticmethod
     def import_dataset(params, name: str) -> SequenceDataset:
         """
         Returns randomly generated receptor dataset according to the parameters;
 
-        YAML specification:
+        **YAML specification:**
 
             result_path: path/where/to/store/results/
             sequence_count: 100 # number of random sequences to generate
             chain_1_length_probabilities:
                 14: 0.8 # 80% of all generated sequences for all sequences will have length 14
                 15: 0.2 # 20% of all generated sequences across all sequences will have length 15
             labels:
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/TenxGenomicsImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/TenxGenomicsImport.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     as described here: https://support.10xgenomics.com/single-cell-vdj/software/pipelines/latest/output/annotation#consensus
 
     Note: by default the 10xGenomics field 'umis' is used to define the immuneML field counts. If you want to use the 10x Genomics
     field reads instead, this can be changed in the column_mapping (set reads: counts).
     Furthermore, the 10xGenomics field clonotype_id is used for the immuneML field cell_id.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with 10xGenomics files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset or ReceptorDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. For setting Sequence- or ReceptorDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -68,44 +68,46 @@
     - column_mapping_synonyms (dict): This is a column mapping that can be used if a column could have alternative names. The formatting is the same as column_mapping. If some columns specified in column_mapping are not found in the file, the columns specified in column_mapping_synonyms are instead attempted to be loaded. For 10xGenomics format, there is no default column_mapping_synonyms.
 
     - metadata_column_mapping (dict): Specifies metadata for Sequence- and ReceptorDatasets. This should specify a mapping similar to column_mapping where keys are 10xGenomics column names and values are the names that are internally used in immuneML as metadata fields. These metadata fields can be used as prediction labels for Sequence- and ReceptorDatasets. This parameter can also be used to specify sequence-level metadata columns for RepertoireDatasets, which can be used by reports. To set prediction label metadata for RepertoireDatasets, see metadata_file instead. For 10xGenomics format, there is no default metadata_column_mapping.
 
     - separator (str): Column separator, for 10xGenomics this is by default ",".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_10x_dataset:
-            format: 10xGenomics
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
-                receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
-                metadata_column_mapping: # metadata column mapping 10xGenomics: immuneML for SequenceDataset
-                    tenx_column_name1: metadata_label1
-                    tenx_column_name2: metadata_label2
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with 10xGenomics-specific defaults, only change when different behavior is required:
-                separator: "," # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping 10xGenomics: immuneML
-                    cdr3: sequence_aa
-                    cdr3_nt: sequence
-                    v_gene: v_call
-                    j_gene: j_call
-                    umis: duplicate_count
-                    clonotype_id: cell_id
-                    consensus_id: sequence_id
+        definitions:
+            datasets:
+                my_10x_dataset:
+                    format: 10xGenomics
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
+                        receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
+                        metadata_column_mapping: # metadata column mapping 10xGenomics: immuneML for SequenceDataset
+                            tenx_column_name1: metadata_label1
+                            tenx_column_name2: metadata_label2
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with 10xGenomics-specific defaults, only change when different behavior is required:
+                        separator: "," # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping 10xGenomics: immuneML
+                            cdr3: sequence_aa
+                            cdr3_nt: sequence
+                            v_gene: v_call
+                            j_gene: j_call
+                            umis: duplicate_count
+                            clonotype_id: cell_id
+                            consensus_id: sequence_id
 
     """
 
     @staticmethod
     def import_dataset(params: dict, dataset_name: str) -> Dataset:
         return ImportHelper.import_dataset(TenxGenomicsImport, params, dataset_name)
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/VDJdbImport.py` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/VDJdbImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     Imports data in VDJdb format into a Repertoire-, Sequence- or ReceptorDataset.
     RepertoireDatasets should be used when making predictions per repertoire, such as predicting a disease state.
     SequenceDatasets or ReceptorDatasets should be used when predicting values for unpaired (single-chain) and paired
     immune receptors respectively, like antigen specificity.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - path (str): For RepertoireDatasets, this is the path to a directory with VDJdb files to import. For Sequence- or ReceptorDatasets this path may either be the path to the file to import, or the path to the folder locating one or multiple files with .tsv, .csv or .txt extensions. By default path is set to the current working directory.
 
     - is_repertoire (bool): If True, this imports a RepertoireDataset. If False, it imports a SequenceDataset or ReceptorDataset. By default, is_repertoire is set to True.
 
     - metadata_file (str): Required for RepertoireDatasets. This parameter specifies the path to the metadata file. This is a csv file with columns filename, subject_id and arbitrary other columns which can be used as labels in instructions. For setting Sequence- or ReceptorDataset metadata, metadata_file is ignored, see metadata_column_mapping instead.
 
@@ -63,43 +63,45 @@
                 Epitope: epitope
                 Epitope gene: epitope_gene
                 Epitope species: epitope_species
 
     - separator (str): Column separator, for VDJdb this is by default "\\t".
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_vdjdb_dataset:
-            format: VDJdb
-            params:
-                path: path/to/files/
-                is_repertoire: True # whether to import a RepertoireDataset
-                metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
-                paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
-                receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
-                import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
-                import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
-                import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
-                # Optional fields with VDJdb-specific defaults, only change when different behavior is required:
-                separator: "\\t" # column separator
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping VDJdb: immuneML
-                    V: v_call
-                    J: j_call
-                    CDR3: sequence_aa
-                    complex.id: sequence_id
-                    Gene: chain
-                metadata_column_mapping: # metadata column mapping VDJdb: immuneML
-                    Epitope: epitope
-                    Epitope gene: epitope_gene
-                    Epitope species: epitope_species
+        definitions:
+            datasets:
+                my_vdjdb_dataset:
+                    format: VDJdb
+                    params:
+                        path: path/to/files/
+                        is_repertoire: True # whether to import a RepertoireDataset
+                        metadata_file: path/to/metadata.csv # metadata file for RepertoireDataset
+                        paired: False # whether to import SequenceDataset (False) or ReceptorDataset (True) when is_repertoire = False
+                        receptor_chains: TRA_TRB # what chain pair to import for a ReceptorDataset
+                        import_illegal_characters: False # remove sequences with illegal characters for the sequence_type being used
+                        import_empty_nt_sequences: True # keep sequences even though the nucleotide sequence might be empty
+                        import_empty_aa_sequences: False # filter out sequences if they don't have sequence_aa set
+                        # Optional fields with VDJdb-specific defaults, only change when different behavior is required:
+                        separator: "\\t" # column separator
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping VDJdb: immuneML
+                            V: v_call
+                            J: j_call
+                            CDR3: sequence_aa
+                            complex.id: sequence_id
+                            Gene: chain
+                        metadata_column_mapping: # metadata column mapping VDJdb: immuneML
+                            Epitope: epitope
+                            Epitope gene: epitope_gene
+                            Epitope species: epitope_species
 
     """
 
     KEY_MAPPING = {
         "subject.id": "subject_id"
     }
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv` & `immuneml-3.0.0a4/immuneML/IO/dataset_import/conversion/imgt_adaptive_conversion.csv`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/ml_method/MLExporter.py` & `immuneml-3.0.0a4/immuneML/IO/ml_method/MLExporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     @staticmethod
     def export(hp_item: HPItem, path: Path) -> Path:
         PathBuilder.build(path)
         preproc_filename = MLExporter._store_preprocessing_sequence(hp_item.hp_setting.preproc_sequence, path).name
         encoder_filename = MLExporter._store_encoder(hp_item.hp_setting.encoder, path).name
 
-        hp_item.method.store(path, hp_item.method.get_feature_names())
+        hp_item.method.store(path)
 
         method_config = MLMethodConfiguration(label_name=hp_item.method.get_label_name(),
                                               label_positive_class=hp_item.method.get_positive_class(),
                                               label_values=hp_item.method.get_classes(),
                                               software_used=hp_item.method.get_package_info(),
                                               encoding_name=hp_item.hp_setting.encoder_name, encoding_parameters=hp_item.hp_setting.encoder_params,
                                               encoding_file=encoder_filename, encoding_class=type(hp_item.hp_setting.encoder).__name__,
```

### Comparing `immuneML-3.0.0a3/immuneML/IO/ml_method/MLImport.py` & `immuneml-3.0.0a4/immuneML/IO/ml_method/MLImport.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/ml_method/MLMethodConfiguration.py` & `immuneml-3.0.0a4/immuneML/IO/ml_method/MLMethodConfiguration.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/IO/ml_method/UtilIO.py` & `immuneml-3.0.0a4/immuneML/IO/ml_method/UtilIO.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/analysis/SequenceMatcher.py` & `immuneml-3.0.0a4/immuneML/analysis/SequenceMatcher.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/analysis/criteria_matches/CriteriaMatcher.py` & `immuneml-3.0.0a4/immuneML/analysis/criteria_matches/CriteriaMatcher.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py` & `immuneml-3.0.0a4/immuneML/analysis/criteria_matches/CriteriaTypeInstantiator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/analysis/data_manipulation/DataReshaper.py` & `immuneml-3.0.0a4/immuneML/analysis/data_manipulation/DataReshaper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/analysis/entropy_calculations/EntropyCalculator.py` & `immuneml-3.0.0a4/immuneML/analysis/entropy_calculations/EntropyCalculator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py` & `immuneml-3.0.0a4/immuneML/api/aggregated_runs/MultiDatasetBenchmarkTool.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class MultiDatasetBenchmarkTool:
     """
     MultiDatasetBenchmarkTool trains the models using nested cross-validation (CV) to determine optimal model on multiple datasets. Internally, it uses
     TrainMLModel instruction for each of the listed datasets and performs nested CV on each, accumulates the results of these runs and then
     generates reports on the cumulative results.
 
-    YAML specification:
+    **YAML specification:**
 
     .. highlight:: yaml
     .. code-block:: yaml
 
         definitions: # everything under definitions can be defined in a standard way
             datasets:
                 d1: ...
```

### Comparing `immuneML-3.0.0a3/immuneML/api/api_encoding.py` & `immuneml-3.0.0a4/immuneML/api/api_encoding.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/DataSimulationTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/DataSimulationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/DatasetGenerationOverviewTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/DatasetGenerationOverviewTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/DatasetGenerationTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/DatasetGenerationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyMLApplicationTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyMLApplicationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxySimulationTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxySimulationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTrainGenModel.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTrainGenModel.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyTrainMLModel.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyTrainMLModel.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/GalaxyYamlTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/GalaxyYamlTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/RepertoireClassificationTool.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/RepertoireClassificationTool.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/Util.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/build_dataset_overview_yaml.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/build_dataset_overview_yaml.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/build_dataset_yaml.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/build_dataset_yaml.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/api/galaxy/build_yaml_from_arguments.py` & `immuneml-3.0.0a4/immuneML/api/galaxy/build_yaml_from_arguments.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/app/ImmuneMLApp.py` & `immuneml-3.0.0a4/immuneML/app/ImmuneMLApp.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,22 +32,23 @@
 
     def clear_cache(self):
         shutil.rmtree(self._cache_path, ignore_errors=True)
         EnvironmentSettings.reset_cache_path()
         del os.environ[Constants.CACHE_TYPE]
 
     def run(self):
+        print_log(f"Running immuneML version {Constants.VERSION}\n", include_datetime=True)
 
         self.set_cache()
 
-        print_log(f"ImmuneML: parsing the specification...\n", include_datetime=True)
+        print_log(f"immuneML: parsing the specification...\n", include_datetime=True)
 
         symbol_table, self._specification_path = ImmuneMLParser.parse_yaml_file(self._specification_path, self._result_path)
 
-        print_log(f"ImmuneML: starting the analysis...\n", include_datetime=True)
+        print_log(f"immuneML: starting the analysis...\n", include_datetime=True)
 
         instructions = symbol_table.get_by_type(SymbolType.INSTRUCTION)
         output = symbol_table.get("output")
         model = SemanticModel([instruction.item for instruction in instructions], self._result_path, output)
         result = model.run()
 
         self.clear_cache()
@@ -84,10 +85,9 @@
 
     namespace = parser.parse_args()
     namespace.specification_path = Path(namespace.specification_path)
     namespace.result_path = Path(namespace.result_path)
 
     run_immuneML(namespace)
 
-
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `immuneML-3.0.0a3/immuneML/app/LigoApp.py` & `immuneml-3.0.0a4/immuneML/app/LigoApp.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/caching/CacheHandler.py` & `immuneml-3.0.0a4/immuneML/caching/CacheHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/airr_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/airr_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/i_receptor_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/i_receptor_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/igor_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/igor_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/immuno_seq_rearrangement_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/immuno_seq_sample_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/mixcr_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/mixcr_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/olga_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/olga_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/random_repertoire_dataset_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/tenx_genomics_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/tenx_genomics_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/datasets/vdjdb_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/datasets/vdjdb_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/encodings/kmer_frequency_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/encodings/kmer_frequency_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/instructions/train_ml_model_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/instructions/train_ml_model_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/config/default_params/ml_methods/deep_rc_params.yaml` & `immuneml-3.0.0a4/immuneML/config/default_params/ml_methods/deep_rc_params.yaml`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/SequenceSet.py` & `immuneml-3.0.0a4/immuneML/data_model/SequenceSet.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/bnp_util.py` & `immuneml-3.0.0a4/immuneML/data_model/bnp_util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/dataset/Dataset.py` & `immuneml-3.0.0a4/immuneML/data_model/dataset/Dataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/dataset/ElementDataset.py` & `immuneml-3.0.0a4/immuneML/data_model/dataset/ElementDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/dataset/ReceptorDataset.py` & `immuneml-3.0.0a4/immuneML/data_model/dataset/ReceptorDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/dataset/RepertoireDataset.py` & `immuneml-3.0.0a4/immuneML/data_model/dataset/RepertoireDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/dataset/SequenceDataset.py` & `immuneml-3.0.0a4/immuneML/data_model/dataset/SequenceDataset.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/BCKReceptor.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/BCKReceptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/BCReceptor.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/BCReceptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/ChainPair.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/ChainPair.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/ElementGenerator.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/ElementGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/Receptor.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/Receptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/ReceptorBuilder.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/ReceptorBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/TCABReceptor.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/TCABReceptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/TCGDReceptor.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/TCGDReceptor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/Chain.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/Chain.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/ReceptorSequence.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py` & `immuneml-3.0.0a4/immuneML/data_model/receptor/receptor_sequence/SequenceMetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,19 @@
             if region_type and isinstance(region_type, str) and region_type != 'nan' else region_type if isinstance(
             region_type, RegionType) else None
         self.cell_id = cell_id
         self.custom_params = custom_params if custom_params is not None else {}
 
     @property
     def v_gene(self):
-        return self.v_call.split("\*")[0]
+        return self.v_call.split("*")[0]
 
     @property
     def j_gene(self):
-        return self.j_call.split("\*")[0]
+        return self.j_call.split("*")[0]
 
     def get_attribute(self, name: str):
         """Returns the attribute value if attribute is present either directly or in custom_params, otherwise returns
         None"""
         if hasattr(self, name):
             return getattr(self, name)
         elif name in self.custom_params:
```

### Comparing `immuneML-3.0.0a3/immuneML/data_model/repertoire/Repertoire.py` & `immuneml-3.0.0a4/immuneML/data_model/repertoire/Repertoire.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,25 +141,25 @@
     def _type_dict(self):
         return {key: SequenceSet.STR_TO_TYPE[val] for key, val in self.metadata["type_dict"].items()}
 
     @property
     def _buffer_type(self):
         return self._create_buffer_type_from_field_dict(self._type_dict)
 
-    def get_sequence_aas(self):
-        return self.get_attribute("sequence_aa")
+    def get_sequence_aas(self, as_list: bool = False):
+        return self.get_attribute("sequence_aa", as_list)
 
-    def get_sequence_identifiers(self):
-        return self.get_attribute("sequence_id")
+    def get_sequence_identifiers(self, as_list: bool = False):
+        return self.get_attribute("sequence_id", as_list)
 
     def get_v_genes(self):
-        return self.get_attribute("v_call")
+        return [v_call.split("*")[0] for v_call in self.get_attribute("v_call", as_list=True)]
 
     def get_j_genes(self):
-        return self.get_attribute("j_call")
+        return [j_call.split("*")[0] for j_call in self.get_attribute("j_call", as_list=True)]
 
     def get_counts(self):
         counts = self.get_attribute("duplicate_count")
         if counts is not None:
             counts = np.array([int(count) if count != SequenceSet.get_neutral_value(int) else None for count in counts])
         return counts
```

### Comparing `immuneML-3.0.0a3/immuneML/dev_util/util.py` & `immuneml-3.0.0a4/immuneML/dev_util/util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/DefaultParamsLoader.py` & `immuneml-3.0.0a4/immuneML/dsl/DefaultParamsLoader.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/ImmuneMLParser.py` & `immuneml-3.0.0a4/immuneML/dsl/ImmuneMLParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/InstructionParser.py` & `immuneml-3.0.0a4/immuneML/dsl/InstructionParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,16 +95,7 @@
     @staticmethod
     def make_docs(instruction, name, path: Path):
         file_path = path / f"{name}.rst"
 
         with file_path.open("w") as file:
             write_class_docs(DocumentationFormat(instruction, "", DocumentationFormat.LEVELS[1]), file)
         return file_path
-
-    @staticmethod
-    def make_trainmlmodel_docs(path):
-        file_path = path / "hp.rst"
-        with file_path.open("w") as file:
-            write_class_docs(DocumentationFormat(TrainMLModelInstruction, "", DocumentationFormat.LEVELS[1]), file)
-            write_class_docs(DocumentationFormat(SplitConfig, "SplitConfig", DocumentationFormat.LEVELS[1]), file)
-            write_class_docs(DocumentationFormat(ReportConfig, "ReportConfig", DocumentationFormat.LEVELS[1]), file)
-        return file_path
```

### Comparing `immuneML-3.0.0a3/immuneML/dsl/ObjectParser.py` & `immuneml-3.0.0a4/immuneML/dsl/ObjectParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/OutputParser.py` & `immuneml-3.0.0a4/immuneML/dsl/OutputParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/Util.py` & `immuneml-3.0.0a4/immuneML/dsl/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/DefinitionParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/DefinitionParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from immuneML.dsl.definition_parsers.ReportParser import ReportParser
 from immuneML.dsl.definition_parsers.SignalParser import SignalParser
 from immuneML.dsl.definition_parsers.SimulationParser import SimulationParser
 from immuneML.dsl.import_parsers.ImportParser import ImportParser
 from immuneML.dsl.symbol_table.SymbolTable import SymbolTable
 from immuneML.encodings.DatasetEncoder import DatasetEncoder
 from immuneML.ml_methods.classifiers.MLMethod import MLMethod
+from immuneML.ml_methods.clustering.ClusteringMethod import ClusteringMethod
 from immuneML.ml_methods.dim_reduction.DimRedMethod import DimRedMethod
 from immuneML.ml_methods.generative_models.GenerativeModel import GenerativeModel
 from immuneML.preprocessing.Preprocessor import Preprocessor
 from immuneML.reports.data_reports.DataReport import DataReport
 from immuneML.reports.encoding_reports.EncodingReport import EncodingReport
 from immuneML.reports.ml_reports.MLReport import MLReport
 from immuneML.reports.multi_dataset_reports.MultiDatasetReport import MultiDatasetReport
@@ -71,20 +72,21 @@
         DefinitionParser.make_encodings_docs(def_path)
         DefinitionParser.make_reports_docs(def_path)
         DefinitionParser.make_ml_methods_docs(def_path)
         DefinitionParser.make_preprocessing_docs(def_path)
 
     @staticmethod
     def make_simulation_docs(path: Path):
-        classes_to_document = [DocumentationFormat(SeedMotif, SeedMotif.__name__, DocumentationFormat.LEVELS[1]),
-                               DocumentationFormat(LigoPWM, "PWM", DocumentationFormat.LEVELS[1]),
-                               DocumentationFormat(Signal, Signal.__name__, DocumentationFormat.LEVELS[1]),
+        classes_to_document = [DocumentationFormat(Motif, "Motifs", DocumentationFormat.LEVELS[1]),
+                               DocumentationFormat(SeedMotif, SeedMotif.__name__, DocumentationFormat.LEVELS[2]),
+                               DocumentationFormat(LigoPWM, "PWM", DocumentationFormat.LEVELS[2]),
+                               DocumentationFormat(Signal, "Signals", DocumentationFormat.LEVELS[1]),
                                DocumentationFormat(SimConfig, "Simulation config", DocumentationFormat.LEVELS[1]),
                                DocumentationFormat(SimConfigItem, "Simulation config item",
-                                                   DocumentationFormat.LEVELS[1])]
+                                                   DocumentationFormat.LEVELS[2])]
 
         file_path = path / "simulation.rst"
         with file_path.open("w") as file:
             for doc_format in classes_to_document:
                 write_class_docs(doc_format, file)
 
     @staticmethod
@@ -101,32 +103,32 @@
     def make_reports_docs(path: Path):
         filename = "reports.rst"
         file_path = path / filename
 
         for report_type_class in [DataReport, EncodingReport, MLReport, TrainMLModelReport, MultiDatasetReport]:
             with file_path.open("a") as file:
                 doc_format = DocumentationFormat(cls=report_type_class,
-                                                 cls_name=f"**{report_type_class.get_title()}**",
+                                                 cls_name=f"**{report_type_class.DOCS_TITLE}**",
                                                  level_heading=DocumentationFormat.LEVELS[1])
                 write_class_docs(doc_format, file)
 
             subdir = DefaultParamsLoader.convert_to_snake_case(report_type_class.__name__) + "s"
 
             classes = ReflectionHandler.all_nonabstract_subclasses(report_type_class, "", f"reports/{subdir}/")
             make_docs(path, classes, filename, "", "a")
 
     @staticmethod
     def make_ml_methods_docs(path: Path):
         filename = 'ml_methods.rst'
         file_path = path / filename
 
-        method_mapping = [{'method_type': MLMethod, 'subdir': 'classifiers', 'title': 'Classifiers'},
-                          {'method_type': GenerativeModel, 'subdir': 'generative_models', 'title': 'Generative models'},
-                          {'method_type': DimRedMethod, 'subdir': 'dim_reduction',
-                           'title': 'Dimensionality reduction methods'}]
+        method_mapping = [{'method_type': MLMethod, 'subdir': 'classifiers', 'title': MLMethod.DOCS_TITLE},
+                          {'method_type': ClusteringMethod, 'subdir': 'clustering', 'title': ClusteringMethod.DOCS_TITLE},
+                          {'method_type': GenerativeModel, 'subdir': 'generative_models', 'title': GenerativeModel.DOCS_TITLE},
+                          {'method_type': DimRedMethod, 'subdir': 'dim_reduction', 'title': DimRedMethod.DOCS_TITLE}]
 
         for method in method_mapping:
             with file_path.open('a') as file:
                 doc_format = DocumentationFormat(cls=method['method_type'],
                                                  cls_name=f"**{method['title']}**",
                                                  level_heading=DocumentationFormat.LEVELS[1])
                 write_class_docs(doc_format, file)
```

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/DefinitionParserOutput.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/DefinitionParserOutput.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/EncodingParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/EncodingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/ExampleWeightingParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/ExampleWeightingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/MLParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/MLParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/MotifParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/MotifParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/PreprocessingParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/PreprocessingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/ReportParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/ReportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/SignalParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/SignalParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/definition_parsers/SimulationParser.py` & `immuneml-3.0.0a4/immuneML/dsl/definition_parsers/SimulationParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/import_parsers/ImportParser.py` & `immuneml-3.0.0a4/immuneML/dsl/import_parsers/ImportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ApplyGenModelParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ApplyGenModelParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ClusteringParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ClusteringParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/DatasetExportParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/DatasetExportParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/ExploratoryAnalysisParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/FeasibilitySummaryParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/FeasibilitySummaryParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/LabelHelper.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/LabelHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/LigoSimParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/LigoSimParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/MLApplicationParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/MLApplicationParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/SubsamplingParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/SubsamplingParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/TrainGenModelParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/TrainGenModelParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/instruction_parsers/TrainMLModelParser.py` & `immuneml-3.0.0a4/immuneML/dsl/instruction_parsers/TrainMLModelParser.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/semantic_model/SemanticModel.py` & `immuneml-3.0.0a4/immuneML/dsl/semantic_model/SemanticModel.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/dsl/symbol_table/SymbolTable.py` & `immuneml-3.0.0a4/immuneML/dsl/symbol_table/SymbolTable.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py` & `immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/AbundanceEncoderHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py` & `immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/CompAIRRBatchIterator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/CompAIRRSequenceAbundanceEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     ‘Immunosequencing Identifies Signatures of Cytomegalovirus Exposure History and HLA-Mediated Effects on the T Cell Repertoire’.
     Nature Genetics 49, no. 5 (May 2017): 659–65. `doi.org/10.1038/ng.3822 <https://doi.org/10.1038/ng.3822>`_.
 
     Note: to use this encoder, it is necessary to explicitly define the positive class for the label when defining the label
     in the instruction. With positive class defined, it can then be determined which sequences are indicative of the positive class.
     See :ref:`Reproduction of the CMV status predictions study` for an example using :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder`.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - p_value_threshold (float): The p value threshold to be used by the statistical test.
 
     - compairr_path (Path): optional path to the CompAIRR executable. If not given, it is assumed that CompAIRR
       has been installed such that it can be called directly on the command line with the command 'compairr',
       or that it is located at /usr/local/bin/compairr.
 
@@ -67,35 +67,37 @@
     - threads (int): The number of threads to use for parallelization. This does not affect the results of the encoding, only the speed.
       The default number of threads is 8.
 
     - keep_temporary_files (bool): whether to keep temporary files, including CompAIRR input, output and log files, and the sequence
       presence matrix. This may take a lot of storage space if the input dataset is large. By default, temporary files are not kept.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. code-block:: yaml
 
-        my_sa_encoding:
-            CompAIRRSequenceAbundance:
-                compairr_path: optional/path/to/compairr
-                p_value_threshold: 0.05
-                ignore_genes: False
-                threads: 8
+        definitions:
+            encodings:
+                my_sa_encoding:
+                    CompAIRRSequenceAbundance:
+                        compairr_path: optional/path/to/compairr
+                        p_value_threshold: 0.05
+                        ignore_genes: False
+                        threads: 8
 
     """
 
     RELEVANT_SEQUENCE_ABUNDANCE = "relevant_sequence_abundance"
     TOTAL_SEQUENCE_ABUNDANCE = "total_sequence_abundance"
     OUTPUT_FILENAME = "compairr_out.tsv"
     LOG_FILENAME = "compairr_log.txt"
 
     def __init__(self, p_value_threshold: float, compairr_path: str, sequence_batch_size: int, ignore_genes: bool, keep_temporary_files: bool,
                  threads: int, name: str = None):
-        self.name = name
+        super().__init__(name=name)
         self.p_value_threshold = p_value_threshold
         self.sequence_batch_size = sequence_batch_size
         self.keep_temporary_files = keep_temporary_files
 
         self.repertoires_filepath = None
         self.sequences_filepaths = None
         self.relevant_indices_path = None
@@ -356,22 +358,14 @@
 
         return attributes
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
-    def store(self, encoded_dataset, params: EncoderParams):
-        EncoderHelper.store(encoded_dataset, params)
-
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
     def get_additional_files(self) -> List[Path]:
         return [file for file in [self.relevant_indices_path, self.relevant_sequence_path, self.contingency_table_path, self.p_values_path] if file]
 
     @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         encoder.relevant_indices_path = DatasetEncoder.load_attribute(encoder, encoder_file, "relevant_indices_path")
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/KmerAbundanceEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     The encoder also writes out files containing the contingency table used for fisher's exact test,
     the resulting p-values, and the significantly abundant k-mers.
 
     Note: to use this encoder, it is necessary to explicitly define the positive class for the label when defining the label
     in the instruction. With positive class defined, it can then be determined which sequences are indicative of the positive class.
     See :ref:`Reproduction of the CMV status predictions study` for an example using :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder`.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - p_value_threshold (float): The p value threshold to be used by the statistical test.
 
     - sequence_encoding (:py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType`): The type of k-mers that are used. The simplest (default) sequence_encoding is :py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.CONTINUOUS_KMER`, which uses contiguous subsequences of length k to represent the k-mers. When gapped k-mers are used (:py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.GAPPED_KMER`, :py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.GAPPED_KMER`), the k-mers may contain gaps with a size between min_gap and max_gap, and the k-mer length is defined as a combination of k_left and k_right. When IMGT k-mers are used (:py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.IMGT_CONTINUOUS_KMER`, :py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.IMGT_GAPPED_KMER`), IMGT positional information is taken into account (i.e. the same sequence in a different position is considered to be a different k-mer).
 
     - k (int): Length of the k-mer (number of amino acids) when ungapped k-mers are used. The default value for k is 3.
 
@@ -53,32 +53,34 @@
     - k_right (int): Same as k_left, but k_right determines the length of the k-mer right of the gap. The default value for k_right is 1.
 
     - min_gap (int): Minimum gap size when gapped k-mers are used. The default value for min_gap is 0.
 
     - max_gap: (int): Maximum gap size when gapped k-mers are used. The default value for max_gap is 0.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_sa_encoding:
-            KmerAbundance:
-                p_value_threshold: 0.05
-                threads: 8
+        definitions:
+            encodings:
+                my_ka_encoding:
+                    KmerAbundance:
+                        p_value_threshold: 0.05
+                        threads: 8
 
     """
 
     RELEVANT_SEQUENCE_ABUNDANCE = "relevant_sequence_abundance"
     TOTAL_SEQUENCE_ABUNDANCE = "total_sequence_abundance"
 
     def __init__(self, p_value_threshold: float, sequence_encoding: SequenceEncodingType, k: int,
                  k_left: int, k_right: int, min_gap: int, max_gap: int, name: str = None):
-        self.name = name
+        super().__init__(name=name)
         self.p_value_threshold = p_value_threshold
 
         self.kmer_frequency_params = {"normalization_type": NormalizationType.BINARY, "reads": ReadsType.UNIQUE,
                                       "sequence_encoding": sequence_encoding, "k": k, "k_left": k_left, "k_right": k_right,
                                       "min_gap": min_gap, "max_gap": max_gap, "scale_to_unit_variance": False,
                                       "scale_to_zero_mean": False, "sequence_type": EnvironmentSettings.get_sequence_type()}
 
@@ -216,22 +218,14 @@
         df = pd.DataFrame(relevant_kmers, columns=["k-mer"])
         df.to_csv(self.relevant_sequence_path, sep=",", index=False)
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
-    def store(self, encoded_dataset, params: EncoderParams):
-        EncoderHelper.store(encoded_dataset, params)
-
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
     def get_additional_files(self) -> List[Path]:
         return [file for file in [self.relevant_indices_path, self.relevant_sequence_path, self.contingency_table_path, self.p_values_path] if file]
 
     @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         encoder.relevant_indices_path = DatasetEncoder.load_attribute(encoder, encoder_file, "relevant_indices_path")
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/abundance_encoding/SequenceAbundanceEncoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,54 +34,56 @@
     ‘Immunosequencing Identifies Signatures of Cytomegalovirus Exposure History and HLA-Mediated Effects on the T Cell Repertoire’.
     Nature Genetics 49, no. 5 (May 2017): 659–65. `doi.org/10.1038/ng.3822 <https://doi.org/10.1038/ng.3822>`_.
 
     Note: to use this encoder, it is necessary to explicitly define the positive class for the label when defining the label
     in the instruction. With positive class defined, it can then be determined which sequences are indicative of the positive class.
     For full example of using this encoder, see :ref:`Reproduction of the CMV status predictions study`.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - comparison_attributes (list): The attributes to be considered to group receptors into clonotypes. Only the fields specified in
       comparison_attributes will be considered, all other fields are ignored. Valid comparison value can be any repertoire field name.
 
     - p_value_threshold (float): The p value threshold to be used by the statistical test.
 
     - sequence_batch_size (int): The number of sequences in a batch when comparing sequences across repertoires, typically 100s of thousands.
       This does not affect the results of the encoding, only the speed. The default value is 1.000.000
 
     - repertoire_batch_size (int): How many repertoires will be loaded at once. This does not affect the result of the encoding, only the speed.
       This value is a trade-off between the number of repertoires that can fit the RAM at the time and loading time from disk.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_sa_encoding:
-            SequenceAbundance:
-                comparison_attributes:
-                    - sequence_aa
-                    - v_call
-                    - j_call
-                    - chain
-                    - region_type
-                p_value_threshold: 0.05
-                sequence_batch_size: 100000
-                repertoire_batch_size: 32
+        definitions:
+            encodings:
+                my_sa_encoding:
+                    SequenceAbundance:
+                        comparison_attributes:
+                            - sequence_aa
+                            - v_call
+                            - j_call
+                            - chain
+                            - region_type
+                        p_value_threshold: 0.05
+                        sequence_batch_size: 100000
+                        repertoire_batch_size: 32
 
     """
 
     RELEVANT_SEQUENCE_ABUNDANCE = "relevant_sequence_abundance"
     TOTAL_SEQUENCE_ABUNDANCE = "total_sequence_abundance"
 
     def __init__(self, comparison_attributes, p_value_threshold: float, sequence_batch_size: int, repertoire_batch_size: int, name: str = None):
+        super().__init__(name=name)
         self.comparison_attributes = comparison_attributes
         self.sequence_batch_size = sequence_batch_size
-        self.name = name
         self.relevant_sequence_indices = None
         self.context = None
         self.p_value_threshold = p_value_threshold
         self.relevant_indices_path = None
         self.relevant_sequence_path = None
         self.contingency_table_path = None
         self.p_values_path = None
@@ -175,23 +177,14 @@
 
         return abundance_matrix
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
-    def store(self, encoded_dataset, params: EncoderParams):
-        EncoderHelper.store(encoded_dataset, params)
-
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        UtilIO.export_comparison_data(encoder.comparison_data, path)
-        return encoder_file
-
     def get_additional_files(self) -> List[Path]:
         return [self.relevant_indices_path]
 
     @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         encoder.relevant_indices_path = DatasetEncoder.load_attribute(encoder, encoder_file, "relevant_indices_path")
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/AtchleyKmerEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,38 +28,40 @@
     For more details, see the original publication: Ostmeyer J,
     Christley S, Toby IT, Cowell LG. Biophysicochemical motifs in T cell receptor sequences distinguish repertoires from tumor-infiltrating
     lymphocytes and adjacent healthy tissue. Cancer Res. Published online January 1, 2019:canres.2292.2018. `doi:10.1158/0008-5472.CAN-18-2292
     <https://cancerres.aacrjournals.org/content/79/7/1671>`_ .
 
     Note that sequences in the repertoire with length shorter than skip_first_n_aa + skip_last_n_aa + k will not be encoded.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - k (int): k-mer length
 
     - skip_first_n_aa (int): number of amino acids to remove from the beginning of the receptor sequence
 
     - skip_last_n_aa (int): number of amino acids to remove from the end of the receptor sequence
 
     - abundance: how to compute abundance term for k-mers
 
     - normalize_all_features (bool): when normalizing features to have 0 mean and unit variance, this parameter indicates if the abundance feature should be included in the normalization
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_encoder:
-            AtchleyKmer:
-                k: 4
-                skip_first_n_aa: 3
-                skip_last_n_aa: 3
-                abundance: RELATIVE_ABUNDANCE
-                normalize_all_features: False
+        definitions:
+            encodings:
+                my_encoder:
+                    AtchleyKmer:
+                        k: 4
+                        skip_first_n_aa: 3
+                        skip_last_n_aa: 3
+                        abundance: RELATIVE_ABUNDANCE
+                        normalize_all_features: False
 
     """
 
     @staticmethod
     def build_object(dataset, **params):
         if isinstance(dataset, RepertoireDataset):
             location = "AtchleyKmerEncoder"
@@ -70,20 +72,20 @@
             ParameterValidator.assert_type_and_value(params["normalize_all_features"], bool, location, "normalize_all_features")
 
             return AtchleyKmerEncoder(**params)
         else:
             raise ValueError(f"AtchleyKmerEncoder can only be applied to repertoire dataset, got {type(dataset).__name__} instead.")
 
     def __init__(self, k: int, skip_first_n_aa: int, skip_last_n_aa: int, abundance: str, normalize_all_features: bool, name: str = None):
+        super().__init__(name=name)
         self.k = k
         self.skip_first_n_aa = skip_first_n_aa
         self.skip_last_n_aa = skip_last_n_aa
         self.abundance = RelativeAbundanceType[abundance.upper()]
         self.normalize_all_features = normalize_all_features
-        self.name = name
         self.scaler = None
         self.kmer_keys = None
 
     def encode(self, dataset, params: EncoderParams):
 
         examples, keys, labels = self._encode_examples(dataset, params)
         examples = self._vectorize_examples(examples, params, keys)
@@ -187,19 +189,14 @@
             sequences = remove_aa_func(sequences.tolist())
         return sequences, counts
 
     def get_additional_files(self) -> List[str]:
         return []
 
     @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         return encoder
 
     @staticmethod
     def get_documentation():
         doc = str(AtchleyKmerEncoder.__doc__)
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/Util.py` & `immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv` & `immuneml-3.0.0a4/immuneML/encodings/atchley_kmer_encoding/atchley_factors.csv`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/deeprc/DeepRCEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/deeprc/DeepRCEncoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,46 +3,49 @@
 
 import pandas as pd
 
 from immuneML.data_model.dataset.RepertoireDataset import RepertoireDataset
 from immuneML.data_model.encoded_data.EncodedData import EncodedData
 from immuneML.encodings.DatasetEncoder import DatasetEncoder
 from immuneML.encodings.EncoderParams import EncoderParams
+from immuneML.util.EncoderHelper import EncoderHelper
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class DeepRCEncoder(DatasetEncoder):
     """
     DeepRCEncoder should be used in combination with the DeepRC ML method (:ref:`DeepRC`).
     This encoder writes the data in a RepertoireDataset to .tsv files.
     For each repertoire, one .tsv file is created containing the amino acid sequences and the counts.
     Additionally, one metadata .tsv file is created, which describes the subset of repertoires that is encoded by
     a given instance of the DeepRCEncoder.
 
     Note: sequences where count is None, the count value will be set to 1
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_deeprc_encoder: DeepRC
+        definitions:
+            encodings:
+                my_deeprc_encoder: DeepRC
 
     """
     ID_COLUMN = "ID"
     SEQUENCE_COLUMN = "amino_acid"
     COUNTS_COLUMN = "templates"
     SEP = "\t"
     EXTENSION = "tsv"
     METADATA_EXTENSION = "csv"
     METADATA_SEP = ","
 
     def __init__(self, context: dict = None, name: str = None):
+        super().__init__(name=name)
         self.context = context
-        self.name = name
         self.max_sequence_length = 0
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
     @staticmethod
@@ -84,24 +87,21 @@
 
     def encode(self, dataset, params: EncoderParams) -> RepertoireDataset:
         result_path = params.result_path / "encoding"
         PathBuilder.build(result_path)
 
         self.export_repertoire_tsv_files(result_path)
 
-        labels = params.label_config.get_labels_by_name()
-        metadata_filepath = self.export_metadata_file(dataset, labels, result_path)
+
+        metadata_filepath = self.export_metadata_file(dataset, params.label_config.get_labels_by_name(), result_path)
 
         encoded_dataset = dataset.clone()
-        encoded_dataset.encoded_data = EncodedData(examples=None, labels=dataset.get_metadata(labels) if params.encode_labels else None,
+        encoded_dataset.encoded_data = EncodedData(examples=None,
+                                                   labels=EncoderHelper.encode_dataset_labels(dataset, params.label_config, params.encode_labels),
                                                    example_ids=dataset.get_repertoire_ids(),
                                                    example_weights=dataset.get_example_weights(),
                                                    encoding=DeepRCEncoder.__name__,
                                                    info={"metadata_filepath": metadata_filepath,
                                                          "max_sequence_length": self.max_sequence_length})
 
         return encoded_dataset
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/distance_encoding/CompAIRRDistanceEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     defined to permit 1 or 2 mismatching amino acid/nucleotide positions and 1 indel in the sequence. Furthermore,
     matching may or may not include V and J gene information, and sequence frequencies may be included or ignored.
 
     When mismatches (differences and indels) are allowed, the Morisita-Horn similarity may exceed 1. In this case, the
     Morisita-Horn distance (= similarity - 1) is set to 0 to avoid negative distance scores.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - compairr_path (Path): optional path to the CompAIRR executable. If not given, it is assumed that CompAIRR has been
       installed such that it can be called directly on the command line with the command 'compairr', or that it is
       located at /usr/local/bin/compairr.
 
     - keep_compairr_input (bool): whether to keep the input file that was passed to CompAIRR. This may take a lot of
       storage space if the input dataset is large. By default, the input file is not kept.
@@ -49,26 +49,28 @@
       only the number of unique overlapping immune receptors ('clones') are considered. By default, ignore_counts is False.
 
     - ignore_genes (bool): Whether to ignore V and J gene information. If False, the V and J genes between two receptor
       chains have to match. If True, gene information is ignored. By default, ignore_genes is False.
 
     - threads (int): The number of threads to use for parallelization. Default is 8.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_distance_encoder:
-            CompAIRRDistance:
-                compairr_path: optional/path/to/compairr
-                differences: 0
-                indels: False
-                ignore_counts: False
-                ignore_genes: False
+        definitions:
+            encodings:
+                my_distance_encoder:
+                    CompAIRRDistance:
+                        compairr_path: optional/path/to/compairr
+                        differences: 0
+                        indels: False
+                        ignore_counts: False
+                        ignore_genes: False
 
     """
 
     OUTPUT_FILENAME = "compairr_results.txt"
     INPUT_FILENAME = "compairr_input.tsv"
     LOG_FILENAME = "compairr_log.txt"
 
@@ -226,16 +228,7 @@
             repertoire_contents.to_csv(filename, mode=mode, header=header, index=False, sep="\t")
 
             mode = "a"
             header = False
 
         return repertoire_sizes, repertoire_indices
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
-    def load_encoder(encoder_file: Path):
-        encoder = DatasetEncoder.load_encoder(encoder_file)
-        return encoder
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/distance_encoding/DistanceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/distance_encoding/DistanceEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,53 +22,55 @@
     """
     Encodes a given RepertoireDataset as distance matrix, where the pairwise distance between each of the repertoires
     is calculated. The distance is calculated based on the presence/absence of elements defined under attributes_to_match.
     Thus, if attributes_to_match contains only 'sequence_aas', this means the distance between two repertoires is maximal
     if they contain the same set of sequence_aas, and the distance is minimal if none of the sequence_aas are shared between
     two repertoires.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - distance_metric (:py:mod:`~immuneML.encodings.distance_encoding.DistanceMetricType`): The metric used to calculate the
       distance between two repertoires. Names of different distance metric types are allowed values in the specification.
       The default distance metric is JACCARD (inverse Jaccard).
 
     - sequence_batch_size (int): The number of sequences to be processed at once. Increasing this number increases the memory use.
       The default value is 1000.
 
     - attributes_to_match (list): The attributes to consider when determining whether a sequence is present in both repertoires.
       Only the fields defined under attributes_to_match will be considered, all other fields are ignored.
       Valid values include any repertoire attribute (sequence, amino acid sequence, V gene etc). The default value is ['sequence_aas']
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_distance_encoder:
-            Distance:
-                distance_metric: JACCARD
-                sequence_batch_size: 1000
-                attributes_to_match:
-                    - sequence_aa
-                    - v_call
-                    - j_call
-                    - chain
-                    - region_type
+        definitions:
+            encodings:
+                my_distance_encoder:
+                    Distance:
+                        distance_metric: JACCARD
+                        sequence_batch_size: 1000
+                        attributes_to_match:
+                            - sequence_aa
+                            - v_call
+                            - j_call
+                            - chain
+                            - region_type
 
     """
 
     def __init__(self, distance_metric: DistanceMetricType, attributes_to_match: list, sequence_batch_size: int, context: dict = None,
                  name: str = None):
+        super().__init__(name=name)
         self.distance_metric = distance_metric
         self.distance_fn = ReflectionHandler.import_function(self.distance_metric.value, DistanceMetrics)
         self.attributes_to_match = attributes_to_match
         self.sequence_batch_size = sequence_batch_size
         self.context = context
-        self.name = name
         self.comparison = None
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
     @staticmethod
@@ -126,18 +128,14 @@
         encoded_dataset = dataset.clone()
         encoded_dataset.encoded_data = EncodedData(examples=distance_matrix, labels=labels, example_ids=distance_matrix.index.values,
                                                    example_weights=EncoderHelper.get_example_weights_by_identifiers(dataset, distance_matrix.index.values),
                                                    encoding=DistanceEncoder.__name__)
 
         return encoded_dataset
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
 
     @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         encoder.comparison = UtilIO.import_comparison_data(encoder_file.parent)
         return encoder
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/distance_encoding/TCRdistEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/distance_encoding/TCRdistEncoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,32 +15,34 @@
     Encodes the given ReceptorDataset as a distance matrix between all receptors, where the distance is computed using TCRdist from the paper:
     Dash P, Fiore-Gartland AJ, Hertz T, et al. Quantifiable predictive features define epitope-specific T cell receptor repertoires.
     Nature. 2017; 547(7661):89-93. `doi:10.1038/nature22383 <https://www.nature.com/articles/nature22383>`_.
 
     For the implementation, `TCRdist3 <https://tcrdist3.readthedocs.io/en/latest/>`_ library was used (source code available
     `here <https://github.com/kmayerb/tcrdist3>`_).
 
-    Specification arguments:
+    **Specification arguments:**
 
     - cores (int): number of processes to use for the computation
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_tcr_dist_enc: # user-defined name
-            TCRdist:
-                cores: 4
+        definitions:
+            encodings:
+                my_tcr_dist_enc:
+                    TCRdist:
+                        cores: 4
 
     """
 
     def __init__(self, cores: int, name: str = None):
+        super().__init__(name=name)
         self.cores = cores
-        self.name = name
         self.distance_matrix = None
         self.context = None
 
     @staticmethod
     def build_object(dataset, **params):
         if isinstance(dataset, ReceptorDataset):
             return TCRdistEncoder(**params)
@@ -77,11 +79,7 @@
     def _build_labels(self, dataset: ReceptorDataset, params: EncoderParams) -> dict:
         labels = {label: [] for label in params.label_config.get_labels_by_name()}
         for receptor in dataset.get_data():
             for label_name in labels.keys():
                 labels[label_name].append(receptor.metadata[label_name])
         return labels
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> str:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/evenness_profile/EvennessProfileEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,49 +24,51 @@
     That is, it is the exponential of Renyi entropy at a given alpha divided by the species richness, or number of unique
     sequences.
 
     Reference: Greiff et al. (2015). A bioinformatic framework for immune repertoire diversity profiling enables detection of immunological
     status. Genome Medicine, 7(1), 49. `doi.org/10.1186/s13073-015-0169-8 <https://doi.org/10.1186/s13073-015-0169-8>`_
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - min_alpha (float): minimum alpha value to use
 
     - max_alpha (float): maximum alpha value to use
 
     - dimension (int): dimension of output evenness profile vector, or the number of alpha values to linearly space
       between min_alpha and max_alpha
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-            my_evenness_profile:
-                EvennessProfile:
-                    min_alpha: 0
-                    max_alpha: 10
-                    dimension: 51
+        definitions:
+            encodings:
+                my_evenness_profile:
+                    EvennessProfile:
+                        min_alpha: 0
+                        max_alpha: 10
+                        dimension: 51
 
 
     """
 
     STEP_ENCODED = "encoded"
     STEP_VECTORIZED = "vectorized"
 
     dataset_mapping = {
         "RepertoireDataset": "EvennessProfileRepertoireEncoder",
     }
 
     def __init__(self, min_alpha: float, max_alpha: float, dimension: int, name: str = None):
+        super().__init__(name=name)
         self.min_alpha = min_alpha
         self.max_alpha = max_alpha
         self.dimension = dimension
-        self.name = name
 
     @staticmethod
     def _prepare_parameters(min_alpha: float, max_alpha: float, dimension: int, name: str = None):
 
         return {
             "min_alpha": min_alpha,
             "max_alpha": max_alpha,
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/evenness_profile/EvennessProfileRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqReceptorEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFreqSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/KmerFrequencyEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 class KmerFrequencyEncoder(DatasetEncoder):
     """
     The KmerFrequencyEncoder class encodes a repertoire, sequence or receptor by frequencies of k-mers it contains.
     A k-mer is a sequence of letters of length k into which an immune receptor sequence can be decomposed.
     K-mers can be defined in different ways, as determined by the sequence_encoding.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - sequence_encoding (:py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType`): The type
       of k-mers that are used. The simplest sequence_encoding is
       :py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.CONTINUOUS_KMER`, which uses
       contiguous subsequences of length k to represent the k-mers. When gapped k-mers are used
       (:py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.GAPPED_KMER`,
       :py:mod:`~immuneML.encodings.kmer_frequency.sequence_encoding.SequenceEncodingType.GAPPED_KMER`),
@@ -77,40 +77,42 @@
 
     - scale_to_zero_mean (bool): whether to scale the design matrix after normalization to have zero mean per feature.
       Setting this argument to True might improve the subsequent classifier's performance depending on the type of the
       classifier. However, if the original design matrix was sparse, setting this argument to True will destroy the
       sparsity and will increase the memory consumption. The default value for scale_to_zero_mean is false.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_continuous_kmer:
-            KmerFrequency:
-                normalization_type: RELATIVE_FREQUENCY
-                reads: UNIQUE
-                sequence_encoding: CONTINUOUS_KMER
-                sequence_type: NUCLEOTIDE
-                k: 3
-                scale_to_unit_variance: True
-                scale_to_zero_mean: True
-        my_gapped_kmer:
-            KmerFrequency:
-                normalization_type: RELATIVE_FREQUENCY
-                reads: UNIQUE
-                sequence_encoding: GAPPED_KMER
-                sequence_type: AMINO_ACID
-                k_left: 2
-                k_right: 2
-                min_gap: 1
-                max_gap: 3
-                scale_to_unit_variance: True
-                scale_to_zero_mean: False
+        definitions:
+            encodings:
+                my_continuous_kmer:
+                    KmerFrequency:
+                        normalization_type: RELATIVE_FREQUENCY
+                        reads: UNIQUE
+                        sequence_encoding: CONTINUOUS_KMER
+                        sequence_type: NUCLEOTIDE
+                        k: 3
+                        scale_to_unit_variance: True
+                        scale_to_zero_mean: True
+                my_gapped_kmer:
+                    KmerFrequency:
+                        normalization_type: RELATIVE_FREQUENCY
+                        reads: UNIQUE
+                        sequence_encoding: GAPPED_KMER
+                        sequence_type: AMINO_ACID
+                        k_left: 2
+                        k_right: 2
+                        min_gap: 1
+                        max_gap: 3
+                        scale_to_unit_variance: True
+                        scale_to_zero_mean: False
 
     """
 
     STEP_ENCODED = "encoded"
     STEP_VECTORIZED = "vectorized"
     STEP_NORMALIZED = "normalized"
     STEP_SCALED = "scaled"
@@ -120,25 +122,25 @@
         "SequenceDataset": "KmerFreqSequenceEncoder",
         "ReceptorDataset": "KmerFreqReceptorEncoder"
     }
 
     def __init__(self, normalization_type: NormalizationType, reads: ReadsType, sequence_encoding: SequenceEncodingType, k: int = 0,
                  k_left: int = 0, k_right: int = 0, min_gap: int = 0, max_gap: int = 0, metadata_fields_to_include: list = None,
                  name: str = None, scale_to_unit_variance: bool = False, scale_to_zero_mean: bool = False, sequence_type: SequenceType = None):
+        super().__init__(name=name)
         self.normalization_type = normalization_type
         self.reads = reads
         self.sequence_encoding = sequence_encoding
         self.sequence_type = sequence_type
         self.k = k
         self.k_left = k_left
         self.k_right = k_right
         self.min_gap = min_gap
         self.max_gap = max_gap
         self.metadata_fields_to_include = metadata_fields_to_include if metadata_fields_to_include is not None else []
-        self.name = name
         self.scale_to_unit_variance = scale_to_unit_variance
         self.scale_to_zero_mean = scale_to_zero_mean
         self.scaler = None
         self.vectorizer = None
 
     @staticmethod
     def _prepare_parameters(normalization_type: str, reads: str, sequence_encoding: str, k: int = 0, k_left: int = 0,
@@ -289,16 +291,7 @@
                 elif self.reads == ReadsType.ALL:
                     counts[i] += sequence.metadata.duplicate_count
         return counts
 
     def get_additional_files(self) -> List[str]:
         return []
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
-    def load_encoder(encoder_file: Path):
-        encoder = DatasetEncoder.load_encoder(encoder_file)
-        return encoder
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/GappedKmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTGappedKmerEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IMGTKmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/IdentitySequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/kmer_frequency/sequence_encoding/KmerSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/motif_encoding/MotifEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/motif_encoding/MotifEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,81 +37,83 @@
 
     This encoder can be used in combination with the :py:obj:`~immuneML.ml_methods.BinaryFeatureClassifier` in order to
     learn a minimal set of compatible motifs for predicting the positive class.
     Alternatively, it may be combined with scikit-learn methods, such as for example :py:obj:`~immuneML.ml_methods.LogisticRegression`,
     to learn a weight per motif.
 
 
-    Arguments:
+    **Specification arguments:**
 
-        max_positions (int): The maximum motif size. This is number of positional amino acids the motif consists of (excluding gaps). The default value for max_positions is 4.
+    - max_positions (int): The maximum motif size. This is number of positional amino acids the motif consists of (excluding gaps). The default value for max_positions is 4.
 
-        min_positions (int): The minimum motif size (see also: max_positions). The default value for max_positions is 1.
+    - min_positions (int): The minimum motif size (see also: max_positions). The default value for max_positions is 1.
 
-        min_precision (float): The minimum precision threshold for keeping a motif. The default value for min_precision is 0.8.
+    - min_precision (float): The minimum precision threshold for keeping a motif. The default value for min_precision is 0.8.
 
-        min_recall (float): The minimum recall threshold for keeping a motif. The default value for min_precision is 0.
-        It is also possible to specify a recall threshold for each motif size. In this case, a dictionary must be specified where
-        the motif sizes are keys and the recall values are values. Use the :py:obj:`~immuneML.reports.data_reports.MotifGeneralizationAnalysis` report
-        to calibrate the optimal recall threshold given a user-defined precision threshold to ensure generalisability to unseen data.
+    - min_recall (float): The minimum recall threshold for keeping a motif. The default value for min_precision is 0.
+      It is also possible to specify a recall threshold for each motif size. In this case, a dictionary must be specified where
+      the motif sizes are keys and the recall values are values. Use the :py:obj:`~immuneML.reports.data_reports.MotifGeneralizationAnalysis` report
+      to calibrate the optimal recall threshold given a user-defined precision threshold to ensure generalisability to unseen data.
 
-        min_true_positives (int): The minimum number of true positive sequences that a motif needs to occur in. The default value for min_true_positives is 10.
+    - min_true_positives (int): The minimum number of true positive sequences that a motif needs to occur in. The default value for min_true_positives is 10.
 
-        candidate_motif_filepath (str): Optional filepath for pre-filterd candidate motifs. This may be used to save time. Only the given candidate motifs are considered.
-        When this encoder has been run previously, a candidate motifs file named 'all_candidate_motifs.tsv' will have been exported. This file contains all
-        possible motifs with high enough min_true_positives without applying precision and recall thresholds.
-        The file must be a tab-separated file, structured as follows:
+    - candidate_motif_filepath (str): Optional filepath for pre-filterd candidate motifs. This may be used to save time. Only the given candidate motifs are considered.
+      When this encoder has been run previously, a candidate motifs file named 'all_candidate_motifs.tsv' will have been exported. This file contains all
+      possible motifs with high enough min_true_positives without applying precision and recall thresholds.
+      The file must be a tab-separated file, structured as follows:
 
-        ========  ==============
-        indices    amino_acids
-        ========  ==============
-        1&2&3      A&G&C
-        5&7        E&D
-        ========  ==============
+      ========  ==============
+      indices    amino_acids
+      ========  ==============
+      1&2&3      A&G&C
+      5&7        E&D
+      ========  ==============
 
-        The example above contains two motifs: AGC in positions 123, and E-D in positions 5-7 (with a gap at position 6).
+      The example above contains two motifs: AGC in positions 123, and E-D in positions 5-7 (with a gap at position 6).
 
-        label (str): The name of the binary label to train the encoder for. This is only necessary when the dataset contains multiple labels.
+    - label (str): The name of the binary label to train the encoder for. This is only necessary when the dataset contains multiple labels.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-            my_motif_encoder:
-                MotifEncoder:
-                    max_positions: 4
-                    min_precision: 0.8
-                    min_recall:  # different recall thresholds for each motif size
-                        1: 0.5   # For shorter motifs, a stricter recall threshold is used
-                        2: 0.1
-                        3: 0.01
-                        4: 0.001
-                    min_true_positives: 10
+        definitions:
+            encodings:
+                my_motif_encoder:
+                    MotifEncoder:
+                        max_positions: 4
+                        min_precision: 0.8
+                        min_recall:  # different recall thresholds for each motif size
+                            1: 0.5   # For shorter motifs, a stricter recall threshold is used
+                            2: 0.1
+                            3: 0.01
+                            4: 0.001
+                        min_true_positives: 10
 
 
 
 
     """
 
     def __init__(self, max_positions: int = None, min_positions: int = None,
                  min_precision: float = None, min_recall: dict = None,
                  min_true_positives: int = None,
                  candidate_motif_filepath: str = None, label: str = None, name: str = None):
+        super().__init__(name=name)
         self.max_positions = max_positions
         self.min_positions = min_positions
         self.min_precision = min_precision
         self.min_recall = min_recall
         self.min_true_positives = min_true_positives
         self.candidate_motif_filepath = Path(candidate_motif_filepath) if candidate_motif_filepath is not None else None
         self.learned_motif_filepath = None
 
         self.label = label
-        self.name = name
         self.context = None
 
     @staticmethod
     def _prepare_parameters(max_positions: int = None, min_positions: int = None, min_precision: float = None, min_recall: dict = None,
                             min_true_positives: int = None, candidate_motif_filepath: str = None, label: str = None, name: str = None):
 
         location = MotifEncoder.__name__
@@ -411,16 +413,7 @@
     # def _get_tp(self, pred, y_true):
     #     return sum(pred & y_true)
 
     def set_context(self, context: dict):
         self.context = context
         return self
 
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
-    def load_encoder(encoder_file: Path):
-        encoder = DatasetEncoder.load_encoder(encoder_file)
-        return encoder
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/motif_encoding/PositionalMotifHelper.py` & `immuneml-3.0.0a4/immuneML/encodings/motif_encoding/PositionalMotifHelper.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,17 +248,18 @@
                                                    f"Specify the correct path under motif_filepath."
 
         with open(motif_filepath) as file:
             PositionalMotifHelper.check_file_header(file.readline(), motif_filepath, expected_header)
 
     @staticmethod
     def read_motifs_from_file(filepath):
+        expected_header = "indices\tamino_acids\n"
         with open(filepath) as file:
-            PositionalMotifHelper.check_file_header(file.readline(), filepath, expected_header="indices\tamino_acids\n")
-            motifs = [PositionalMotifHelper.string_to_motif(line, value_sep="&", motif_sep="\t") for line in file.readlines()]
+            PositionalMotifHelper.check_file_header(file.readline(), filepath, expected_header=expected_header)
+            motifs = [PositionalMotifHelper.string_to_motif(line, value_sep="&", motif_sep="\t") for line in file.readlines() if line != expected_header]
 
         return motifs
 
     @staticmethod
     def write_motifs_to_file(motifs, filepath):
         PathBuilder.build(filepath.parent)
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/motif_encoding/SimilarToPositiveSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/motif_encoding/SimilarToPositiveSequenceEncoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,55 +22,56 @@
 class SimilarToPositiveSequenceEncoder(DatasetEncoder):
     """
     A simple baseline encoding, to be used in combination with :py:obj:`~immuneML.ml_methods.BinaryFeatureClassifier.BinaryFeatureClassifier` using keep_all = True.
     This encoder keeps track of all positive sequences in the training set, and ignores the negative sequences.
     Any sequence within a given hamming distance from a positive training sequence will be classified positive,
     all other sequences will be classified negative.
 
-    Arguments:
+    **Specification arguments:**
 
-        hamming_distance (int): Maximum number of differences allowed between any positive sequence of the training set and a
-        new observed sequence in order for the observed sequence to be classified as 'positive'.
+    - hamming_distance (int): Maximum number of differences allowed between any positive sequence of the training set and a
+      new observed sequence in order for the observed sequence to be classified as 'positive'.
 
-        compairr_path (Path): optional path to the CompAIRR executable. If not given, it is assumed that CompAIRR
-        has been installed such that it can be called directly on the command line with the command 'compairr',
-        or that it is located at /usr/local/bin/compairr.
+    - compairr_path (Path): optional path to the CompAIRR executable. If not given, it is assumed that CompAIRR
+      has been installed such that it can be called directly on the command line with the command 'compairr',
+      or that it is located at /usr/local/bin/compairr.
 
-        ignore_genes (bool): Only used when compairr is used. Whether to ignore V and J gene information. If False, the V and J genes between two sequences
-        have to match for the sequence to be considered 'similar'. If True, gene information is ignored. By default, ignore_genes is False.
+    - ignore_genes (bool): Only used when compairr is used. Whether to ignore V and J gene information. If False, the V and J genes between two sequences
+      have to match for the sequence to be considered 'similar'. If True, gene information is ignored. By default, ignore_genes is False.
 
-        threads (int): The number of threads to use for parallelization. This does not affect the results of the encoding, only the speed.
-        The default number of threads is 8.
+    - threads (int): The number of threads to use for parallelization. This does not affect the results of the encoding, only the speed.
+      The default number of threads is 8.
 
-        keep_temporary_files (bool): whether to keep temporary files, including CompAIRR input, output and log files, and the sequence
-        presence matrix. This may take a lot of storage space if the input dataset is large. By default temporary files are not kept.
+    - keep_temporary_files (bool): whether to keep temporary files, including CompAIRR input, output and log files, and the sequence
+      presence matrix. This may take a lot of storage space if the input dataset is large. By default temporary files are not kept.
 
 
-
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-            my_sequence_encoder:
-                SimilarToPositiveSequenceEncoder:
-                    hamming_distance: 2
+        definitions:
+            encodings:
+                my_sequence_encoder:
+                    SimilarToPositiveSequenceEncoder:
+                        hamming_distance: 2
     """
 
     def __init__(self, hamming_distance: int = None, compairr_path: str = None,
                  ignore_genes: bool = None, threads: int = None, keep_temporary_files: bool = None,
                  name: str = None):
+        super().__init__(name=name)
         self.hamming_distance = hamming_distance
         self.compairr_path = Path(compairr_path) if compairr_path is not None else None
         self.ignore_genes = ignore_genes
         self.threads = threads
         self.keep_temporary_files = keep_temporary_files
 
         self.positive_sequences = None
-        self.name = name
         self.context = None
 
     @staticmethod
     def _prepare_parameters(hamming_distance: int = None, compairr_path: str = None, ignore_genes: bool = None,
                             threads: int = None, keep_temporary_files: bool = None, name: str = None):
         location = SimilarToPositiveSequenceEncoder.__name__
 
@@ -238,17 +239,7 @@
         label = label_config.get_label_object(label_name)
 
         return label.positive_class
 
     def set_context(self, context: dict):
         self.context = context
         return self
-
-    @staticmethod
-    def export_encoder(path: Path, encoder) -> Path:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
-    def load_encoder(encoder_file: Path):
-        encoder = DatasetEncoder.load_encoder(encoder_file)
-        return encoder
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class OneHotEncoder(DatasetEncoder):
     """
     One-hot encoding for repertoires, sequences or receptors. In one-hot encoding, each alphabet character
     (amino acid or nucleotide) is replaced by a sparse vector with one 1 and the rest zeroes. The position of the
     1 represents the alphabet character.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - use_positional_info (bool): whether to include features representing the positional information.
       If True, three additional feature vectors will be added, representing the sequence start, sequence middle
       and sequence end. The values in these features are scaled between 0 and 1. A graphical representation of
       the values of these vectors is given below.
 
     .. code-block:: console
@@ -64,55 +64,56 @@
     - flatten (bool): whether to flatten the final onehot matrix to a 2-dimensional matrix [examples, other_dims_combined]
       This must be set to True when using onehot encoding in combination with scikit-learn ML methods (inheriting :py:obj:`~source.ml_methods.SklearnMethod.SklearnMethod`),
       such as :ref:`LogisticRegression`, :ref:`SVM`, :ref:`SVC`, :ref:`RandomForestClassifier` and :ref:`KNN`.
 
     - sequence_type: whether to use nucleotide or amino acid sequence for encoding. Valid values are 'nucleotide' and 'amino_acid'.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        one_hot_vanilla:
-            OneHot:
-                use_positional_info: False
-                flatten: False
-                sequence_type: amino_acid
-
-        one_hot_positional:
-            OneHot:
-                use_positional_info: True
-                distance_to_seq_middle: 3
-                flatten: False
-                sequence_type: nucleotide
+        definitions:
+            encodings:
+                one_hot_vanilla:
+                    OneHot:
+                        use_positional_info: False
+                        flatten: False
+                        sequence_type: amino_acid
+
+                one_hot_positional:
+                    OneHot:
+                        use_positional_info: True
+                        distance_to_seq_middle: 3
+                        flatten: False
+                        sequence_type: nucleotide
 
     """
 
     dataset_mapping = {
         "RepertoireDataset": "OneHotRepertoireEncoder",
         "SequenceDataset": "OneHotSequenceEncoder",
         "ReceptorDataset": "OneHotReceptorEncoder"
     }
 
     def __init__(self, use_positional_info: bool, distance_to_seq_middle: int, flatten: bool, name: str = None, sequence_type: SequenceType = None):
+        super().__init__(name=name)
         self.use_positional_info = use_positional_info
         self.distance_to_seq_middle = distance_to_seq_middle
         self.flatten = flatten
         self.sequence_type = sequence_type
         self.alphabet = EnvironmentSettings.get_sequence_alphabet(self.sequence_type)
 
         if distance_to_seq_middle:
             self.pos_increasing = [1 / self.distance_to_seq_middle * i for i in range(self.distance_to_seq_middle)]
             self.pos_decreasing = self.pos_increasing[::-1]
         else:
             self.pos_decreasing = None
 
-        self.name = name
-
         if self.sequence_type == SequenceType.NUCLEOTIDE and self.distance_to_seq_middle is not None:  # todo check this / explain in docs
             self.distance_to_seq_middle = self.distance_to_seq_middle * 3
 
         self.onehot_dimensions = self.alphabet + ["start", "mid", "end"] if self.use_positional_info else self.alphabet  # todo test this
 
     @staticmethod
     def _prepare_parameters(use_positional_info: bool, distance_to_seq_middle: int, flatten: bool, sequence_type: str, name: str = None):
@@ -145,31 +146,26 @@
 
     def encode(self, dataset, params: EncoderParams):
         encoded_dataset = CacheHandler.memo_by_params(self._prepare_caching_params(dataset, params),
                                                       lambda: self._encode_new_dataset(dataset, params))
 
         return encoded_dataset
 
-    def _prepare_caching_params(self, dataset, params: EncoderParams, step: str = ""):
-        return (("example_identifiers", tuple(dataset.get_example_ids())),
-                ("dataset_metadata", dataset.metadata_file if hasattr(dataset, "metadata_file") else None),
+    def _prepare_caching_params(self, dataset, params: EncoderParams):
+        return (("dataset_identifier", dataset.identifier),
+                ("example_identifiers", tuple(dataset.get_example_ids())),
                 ("dataset_type", dataset.__class__.__name__),
                 ("labels", tuple(params.label_config.get_labels_by_name())),
                 ("encoding", OneHotEncoder.__name__),
-                ("learn_model", params.learn_model),
-                ("step", step),
                 ("encoding_params", tuple(vars(self).items())))
 
     @abc.abstractmethod
     def _encode_new_dataset(self, dataset, params: EncoderParams):
         pass
 
-    def store(self, encoded_dataset, params: EncoderParams):
-        ImmuneMLExporter.export(encoded_dataset, params.result_path)
-
     def _encode_sequence_list(self, sequences, pad_n_sequences, pad_sequence_len):
         char_array = np.array(sequences, dtype=str)
         char_array = char_array.view('U1').reshape((char_array.size, -1))
 
         n_sequences, sequence_len = char_array.shape
 
         sklearn_enc = SklearnOneHotEncoder(categories=[self.alphabet for i in range(sequence_len)], handle_unknown='ignore')
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotReceptorEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotReceptorEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotRepertoireEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/onehot/OneHotSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/onehot/OneHotSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/preprocessing/FeatureScaler.py` & `immuneml-3.0.0a4/immuneML/encodings/preprocessing/FeatureScaler.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedReceptorsEncoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     This encoding can be used in combination with the :ref:`Matches` report.
 
     When sum_matches and normalize are set to True, this encoder behaves similarly as described in: Yao, Y. et al. ‘T cell receptor repertoire as a potential diagnostic marker for celiac disease’.
     Clinical Immunology Volume 222 (January 2021): 108621. `doi.org/10.1016/j.clim.2020.108621 <https://doi.org/10.1016/j.clim.2020.108621>`_
     with the only exception being that this encoder uses paired receptors, while the original publication used single sequences (see also: :ref:`MatchedSequences` encoder).
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference (dict): A dictionary describing the reference dataset file. Import should be specified the same way as
       regular dataset import. It is only allowed to import a receptor dataset here (i.e., is_repertoire is False and
       paired is True by default, and these are not allowed to be changed).
 
     - max_edit_distances (dict): A dictionary specifying the maximum edit distance between a target sequence (from the
       repertoire) and the reference sequence. A maximum distance can be specified per chain, for example to allow for
@@ -54,42 +54,44 @@
       must be set to False. When sum_matches is set to True, this encoder behaves similarly to the encoder described by
       Yao, Y. et al. By default, sum_matches is False.
 
     - normalize (bool): If True, the chain matches are divided by the total number of unique receptors in the repertoire
       (when reads = unique) or the total number of reads in the repertoire (when reads = all).
 
 
-    YAML Specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_mr_encoding:
-            MatchedReceptors:
-                reference:
-                    format: VDJDB
-                    params:
-                        path: path/to/file.txt
-                max_edit_distances:
-                    alpha: 1
-                    beta: 0
+        definitions:
+            encodings:
+                my_mr_encoding:
+                    MatchedReceptors:
+                        reference:
+                            format: VDJDB
+                            params:
+                                path: path/to/file.txt
+                        max_edit_distances:
+                            alpha: 1
+                            beta: 0
     """
 
     dataset_mapping = {
         "RepertoireDataset": "MatchedReceptorsRepertoireEncoder"
     }
 
     def __init__(self, reference: List[Receptor], max_edit_distances: dict, reads: ReadsType, sum_matches: bool, normalize: bool, name: str = None):
+        super().__init__(name=name)
         self.reference_receptors = reference
         self.max_edit_distances = max_edit_distances
         self.reads = reads
         self.sum_matches = sum_matches
         self.normalize = normalize
         self.feature_count = 2 if self.sum_matches else len(self.reference_receptors) * 2
-        self.name = name
 
     @staticmethod
     def _prepare_parameters(reference: dict, max_edit_distances: dict, reads: str, sum_matches: bool, normalize: bool, name: str = None):
         location = "MatchedReceptorsEncoder"
 
         ParameterValidator.assert_type_and_value(sum_matches, bool, location, "sum_matches")
         ParameterValidator.assert_type_and_value(normalize, bool, location, "normalize")
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py` & `immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedReferenceUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedRegexEncoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     The regular expressions are defined per chain, and it is possible to require a V gene match in addition to the
     CDR3 sequence containing the regular expression.
 
     This encoding can be used in combination with the :ref:`Matches` report.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - match_v_genes (bool): Whether V gene matches are required. If this is True, a match is only counted if the
       V gene matches the gene specified in the motif input file. By default match_v_genes is False.
 
     - reads (:py:mod:`~immuneML.util.ReadsType`): Reads type signify whether the counts of the sequences in the
       repertoire will be taken into account. If :py:mod:`~immuneML.util.ReadsType.UNIQUE`, only unique sequences
       (clonotypes) are counted, and if :py:mod:`~immuneML.util.ReadsType.ALL`, the sequence 'count' value is
@@ -62,39 +62,41 @@
         id    TRA_regex   TRAV     TRB_regex   TRBV
         ====  ==========  =======  ==========  ========
         1     AGQ.GSS     TRAV35   S[APL]GQY   TRBV29-1
         2                          ASS.R.*     TRBV7-3
         ====  ==========  =======  ==========  ========
 
 
-    YAML Specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_mr_encoding:
-            MatchedRegex:
-                motif_filepath: path/to/file.txt
-                match_v_genes: True
-                reads: unique
+        definitions:
+            encodings:
+                my_mr_encoding:
+                    MatchedRegex:
+                        motif_filepath: path/to/file.txt
+                        match_v_genes: True
+                        reads: unique
 
     """
 
     dataset_mapping = {
         "RepertoireDataset": "MatchedRegexRepertoireEncoder"
     }
 
     def __init__(self, motif_filepath: Path, match_v_genes: bool, reads: ReadsType, chains: list, name: str = None):
+        super().__init__(name=name)
         self.motif_filepath = motif_filepath
         self.match_v_genes = match_v_genes
         self.reads = reads
         self.chains = chains
         self.regex_df = None
         self.feature_count = None
-        self.name = name
 
     @staticmethod
     def _prepare_parameters(motif_filepath: str, match_v_genes: bool, reads: str, name: str = None):
 
         ParameterValidator.assert_type_and_value(match_v_genes, bool, "MatchedRegexEncoder", "match_v_genes")
         ParameterValidator.assert_in_valid_list(reads.upper(), [item.name for item in ReadsType], "MatchedRegexEncoder", "reads")
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedRegexRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/reference_encoding/MatchedSequencesEncoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     This encoding can be used in combination with the :ref:`Matches` report.
 
     When sum_matches and normalize are set to True, this encoder behaves as described in: Yao, Y. et al. ‘T cell receptor repertoire as a potential diagnostic marker for celiac disease’.
     Clinical Immunology Volume 222 (January 2021): 108621. `doi.org/10.1016/j.clim.2020.108621 <https://doi.org/10.1016/j.clim.2020.108621>`_
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference (dict): A dictionary describing the reference dataset file. Import should be specified the same way as
       regular dataset import. It is only allowed to import a sequence dataset here (i.e., is_repertoire and paired are
       False by default, and are not allowed to be set to True).
 
     - max_edit_distance (int): The maximum edit distance between a target sequence (from the repertoire) and the
       reference sequence.
@@ -47,37 +47,39 @@
       To use this encoder in combination with the :ref:`Matches` report, sum_matches must be set to False. When
       sum_matches is set to True, this encoder behaves as described by Yao, Y. et al. By default, sum_matches is False.
 
     - normalize (bool): If True, the sequence matches are divided by the total number of unique sequences in the
       repertoire (when reads = unique) or the total number of reads in the repertoire (when reads = all).
 
 
-    YAML Specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_ms_encoding:
-            MatchedSequences:
-                reference:
-                    format: VDJDB
-                    params:
-                        path: path/to/file.txt
-                max_edit_distance: 1
+        definitions:
+            encodings:
+                my_ms_encoding:
+                    MatchedSequences:
+                        reference:
+                            format: VDJDB
+                            params:
+                                path: path/to/file.txt
+                        max_edit_distance: 1
     """
 
     def __init__(self, max_edit_distance: int, reference: List[ReceptorSequence], reads: ReadsType, sum_matches: bool, normalize: bool,
                  name: str = None):
+        super().__init__(name=name)
         self.max_edit_distance = max_edit_distance
         self.reference_sequences = reference
         self.reads = reads
         self.sum_matches = sum_matches
         self.normalize = normalize
         self.feature_count = 1 if self.sum_matches else len(self.reference_sequences)
-        self.name = name
 
     @staticmethod
     def _prepare_parameters(max_edit_distance: int, reference: dict, reads: str, sum_matches: bool, normalize: bool,
                             name: str = None):
         location = "MatchedSequencesEncoder"
 
         ParameterValidator.assert_type_and_value(max_edit_distance, int, location, "max_edit_distance", min_inclusive=0)
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/W2VRepertoireEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/W2VRepertoireEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/W2VSequenceEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/W2VSequenceEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/Word2VecEncoder.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/Word2VecEncoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Word2VecEncoder learns the vector representations of k-mers based on the context (receptor sequence). It works for
     sequence and repertoire datasets. Similar idea was discussed in: Ostrovsky-Berman, M., Frankel, B., Polak, P. & Yaari, G.
     Immune2vec: Embedding B/T Cell Receptor Sequences in ℝN Using Natural Language Processing. Frontiers in Immunology 12, (2021).
 
     This encoder relies on gensim's implementation of Word2Vec and KmerHelper for k-mer extraction. Currently it works on amino acid level.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - vector_size (int): The size of the vector to be learnt.
 
     - model_type (:py:obj:`~immuneML.encodings.word2vec.model_creator.ModelType.ModelType`):  The context which will be
       used to infer the representation of the sequence.
       If :py:obj:`~immuneML.encodings.word2vec.model_creator.ModelType.ModelType.SEQUENCE` is used, the context of
       a k-mer is defined by the sequence it occurs in (e.g. if the sequence is CASTTY and k-mer is AST,
@@ -53,27 +53,29 @@
     - k (int): The length of the k-mers used for the encoding.
 
     - epochs (int): for how many epochs to train the word2vec model for a given set of sentences (corresponding to epochs parameter in gensim package)
 
     - window (int): max distance between two k-mers in a sequence (same as window parameter in gensim's word2vec)
 
 
-    YAML specification:
+    **YAML pecification:**
 
     .. highlight:: yaml
     .. code-block:: yaml
 
-        encodings:
-            my_w2v:
-                Word2Vec:
-                    vector_size: 16
-                    k: 3
-                    model_type: SEQUENCE
-                    epochs: 100
-                    window: 8
+        definitions:
+            encodings:
+                encodings:
+                    my_w2v:
+                        Word2Vec:
+                            vector_size: 16
+                            k: 3
+                            model_type: SEQUENCE
+                            epochs: 100
+                            window: 8
 
     """
 
     DESCRIPTION_REPERTOIRES = "repertoires"
     DESCRIPTION_LABELS = "labels"
 
     dataset_mapping = {
@@ -231,19 +233,14 @@
         else:
             return self.model_path
 
     def get_additional_files(self) -> List[str]:
         return [self.model_path]
 
     @staticmethod
-    def export_encoder(path: Path, encoder) -> str:
-        encoder_file = DatasetEncoder.store_encoder(encoder, path / "encoder.pickle")
-        return encoder_file
-
-    @staticmethod
     def load_encoder(encoder_file: Path):
         encoder = DatasetEncoder.load_encoder(encoder_file)
         encoder = DatasetEncoder.load_attribute(encoder, encoder_file, "model_path")
         return encoder
 
     @staticmethod
     def get_documentation():
```

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/KmerPairModelCreator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/ModelCreatorStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py` & `immuneml-3.0.0a4/immuneML/encodings/word2vec/model_creator/SequenceModelCreator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/environment/EnvironmentSettings.py` & `immuneml-3.0.0a4/immuneML/environment/EnvironmentSettings.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/environment/Label.py` & `immuneml-3.0.0a4/immuneML/environment/Label.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,26 @@
         self._values = values
         self.auxiliary_label_names = auxiliary_label_names
         self._positive_class = positive_class
 
     def __str__(self):
         return f"label {self.name} ({', '.join([str(val) for val in self.values])})"
 
+    def __eq__(self, other):
+        if not isinstance(other, Label):
+            return False
+
+        return self.name == other.name and self.values == other.values and \
+            self.positive_class == other.positive_class and self.auxiliary_label_names == other.auxiliary_label_names
+
     @property
     def positive_class(self):
+        '''
+        Ensures the same class is always returned as the 'positive class', even when it was not explicitly set.
+        '''
         if self._positive_class is not None:
             return self._positive_class
         else:
             assert self._values is not None, f"Label: cannot access positive class for label {self.name} " \
                                              f"when neither 'positive_class' nor 'values' are set."
 
             positive_class = sorted(self._values)[0]
@@ -25,23 +35,30 @@
                          f"Assuming default positive class '{positive_class}'.")
 
             return positive_class
 
     @property
     def values(self):
         '''
-        Make sure the positive class is listed last
+        Returns the label values and makes sure the positive class is listed last
         This is needed for compatibility with `~immuneML.ml_methods.util.Util.binarize_label_classes`
         '''
         if self._positive_class is not None:
             negative_classes = sorted(self._values)
             negative_classes.remove(self._positive_class)
             return negative_classes + [self._positive_class]
         else:
             return sorted(self._values)
 
     def get_binary_negative_class(self):
+        '''
+        Ensures the correct 'negative class' is returned when using the Label for binary classification.
+        '''
         assert len(self._values) == 2, f"Label: binary negative class was requested for label {self.name} but this label contains {len(self._values)} classes: {self.values}"
         return [val for val in self._values if val != self.positive_class][0]
 
     def get_desc_for_storage(self):
+        '''
+        Method to call when storing a label to YAML format
+        '''
         return {key.lstrip("_"): value for key, value in vars(self).items()}
+
```

### Comparing `immuneML-3.0.0a3/immuneML/environment/LabelConfiguration.py` & `immuneml-3.0.0a4/immuneML/environment/LabelConfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         if len(classes) != 2:
             return None
         if classes[0] == True and classes[1] == False:
             return classes[0]
         if classes[1] == True and classes[0] == False:
             return classes[1]
 
-        for positive_str, negative_str in [("1", "0"), ("true", "false"), ("positive", "negative"), ("+", "-")]:
+        for positive_str, negative_str in [("1", "0"), ("true", "false"), ("positive", "negative"), ("+", "-"), ("yes", "no")]:
             if set(classes) == {positive_str, negative_str}:
                 return positive_str
             if set(classes) == {positive_str.upper(), negative_str.upper()}:
                 return positive_str.upper()
             if set(classes) == {positive_str.title(), negative_str.title()}:
                 return positive_str.title()
```

### Comparing `immuneML-3.0.0a3/immuneML/example_weighting/predefined_weighting/PredefinedWeighting.py` & `immuneml-3.0.0a4/immuneML/example_weighting/predefined_weighting/PredefinedWeighting.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 
 class PredefinedWeighting(ExampleWeightingStrategy):
     '''
 
     Example weighting strategy where weights are supplied in a file.
 
-    Arguments:
+    **Specification arguments:**
 
-        file_path (Path): Path to the example weights, should contain the columns 'identifier' and 'example_weight':
+    - file_path (Path): Path to the example weights, should contain the columns 'identifier' and 'example_weight':
 
-        ==========  ==============
-        identifier  example_weight
-        ==========  ==============
-        1           0.5
-        2           1
-        3           1
-        ========  ==============
+      ==========  ==============
+      identifier  example_weight
+      ==========  ==============
+      1           0.5
+      2           1
+      3           1
+      ========  ==============
 
-        separator (str): Column separator in the input file.
+    - separator (str): Column separator in the input file.
 
     '''
 
     def __init__(self, file_path, separator, name: str = None):
         super().__init__(name)
         self.file_path = Path(file_path)
         self.separator = separator
```

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/HPSetting.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/HPSetting.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/HPSettingResult.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/HPSettingResult.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/ReportConfig.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/ReportConfig.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 class ReportConfig:
     """
     A class encapsulating different report lists which can be executed while performing nested cross-validation (CV) using TrainMLModel
     instruction. All arguments are optional.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - data (dict): :ref:`Data reports` to be executed on the whole dataset before it is split to training/test or training/validation
 
     - data_splits (dict): :ref:`Data reports` to be executed after the data has been split into training and test (assessment CV loop) or training and validation (selection CV loop) datasets before they are encoded
 
     - models (dict): :ref:`ML model reports` to be executed on all trained classifiers
 
     - encoding (dict): :ref:`Encoding reports` to be executed on each of the encoded training/test datasets or training/validation datasets
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         # as a part of a TrainMLModel instruction, defining the outer (assessment) loop of nested cross-validation:
         assessment: # outer loop of nested CV
             split_strategy: random # perform Monte Carlo CV (randomly split the data into train and test)
```

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/config/SplitConfig.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/config/SplitConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     - random (Monte Carlo cross-validation - randomly splitting the dataset to training and test datasets)
 
     - manual (train and test dataset are explicitly specified by providing metadata files for the two datasets)
 
     - leave_one_out_stratification (leave-one-out CV where one refers to a specific parameter, e.g. if subject is known in a receptor dataset, it is possible to have leave-subject-out CV - currently only available for receptor and sequence datasets).
 
-    Specification arguments:
+    **Specification arguments:**
 
     - split_strategy (SplitType): one of the types of cross-validation listed above (`LOOCV`, `K_FOLD`, `STRATIFIED_K_FOLD`, `MANUAL`, ``  or `RANDOM`)
 
     - split_count (int): if split_strategy is `K_FOLD`, then this defined how many splits to make (K), if split_strategy is RANDOM, split_count defines how many random splits to make, resulting in split_count training/test dataset pairs, or if split_strategy is `LOOCV`, `MANUAL` or `LEAVE_ONE_OUT_STRATIFICATION`, split_count does not need to be specified.
 
     - training_percentage: if split_strategy is RANDOM, this defines which portion of the original dataset to use for creating the training dataset; for other values of split_strategy, this parameter is not used.
 
@@ -41,15 +41,15 @@
     - leave_one_out_config (:py:obj:`~immuneML.hyperparameter_optimization.config.LeaveOneOutConfig.LeaveOneOutConfig`): if split strategy is
       `LEAVE_ONE_OUT_STRATIFICATION`, this config describes which parameter to use for stratification thus making a list of train/test dataset
       combinations in which in the test set there are examples with only one value of the specified parameter. `leave_one_out_config` argument
       accepts two inputs: `parameter` which is the name of the parameter to use for stratification and `min_count` which defines the minimum
       number of examples that can be present in the test dataset. This type of generating train and test datasets is only supported for receptor
       and sequence datasets so far. If split strategy is anything else, this field has no effect and can be omitted.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         # as a part of a TrainMLModel instruction, defining the outer (assessment) loop of nested cross-validation:
         assessment: # outer loop of nested CV
             split_strategy: random # perform Monte Carlo CV (randomly split the data into train and test)
```

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPAssessment.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPAssessment.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPSelection.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPSelection.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/core/HPUtil.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/core/HPUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPAssessmentState.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPAssessmentState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPItem.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPItem.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
     method: MLMethod = None
     encoder: DatasetEncoder = None
     performance: dict = None
     hp_setting: HPSetting = None
     train_predictions_path: Path = None
     test_predictions_path: Path = None
-    ml_details_path: Path = None
     ml_settings_export_path: Path = None
     train_dataset: Dataset = None
     test_dataset: Dataset = None
     split_index: int = None
     model_report_results: List[ReportResult] = field(default_factory=list)
     encoding_train_results: List[ReportResult] = field(default_factory=list)
     encoding_test_results: List[ReportResult] = field(default_factory=list)
```

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/HPSelectionState.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/HPSelectionState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/states/TrainMLModelState.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/states/TrainMLModelState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/GridSearch.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/GridSearch.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py` & `immuneml-3.0.0a4/immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/BinaryFeatureClassifier.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/BinaryFeatureClassifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,42 +38,44 @@
     This results in a set of complementary motifs, minimizing the redundant predictions made by different motifs.
 
     - Alternatively, this classifier can be combined with the :py:obj:`~immuneML.encodings.motif_encoding.SimilarToPositiveSequenceEncoder.SimilarToPositiveSequenceEncoder`
     such that any sequence that falls within a given hamming distance from any of the positive class sequences in the training set
     are classified as positive. Parameter keep_all should be set to true, since this encoder creates only 1 feature.
 
 
-    Arguments:
+    **Specification arguments:**
 
-        training_percentage (float): What percentage of data to use for training (the rest will be used for validation); values between 0 and 1
+    - training_percentage (float): What percentage of data to use for training (the rest will be used for validation); values between 0 and 1
 
-        keep_all (bool): Whether to keep all the input features (true) or learn a reduced subset (false). By default, keep_all is false.
+    - keep_all (bool): Whether to keep all the input features (true) or learn a reduced subset (false). By default, keep_all is false.
 
-        random_seed (int): Random seed for splitting the data into training and validation sets when learning a minimal subset of features. This is only used when keep_all is false.
+    - random_seed (int): Random seed for splitting the data into training and validation sets when learning a minimal subset of features. This is only used when keep_all is false.
 
-        max_features (int): The maximum number of features to allow in the reduced subset. When this number is reached, no more features are added even if the earlystopping criterion is not reached yet.
-        This is only used when keep_all is false. By default, max_features is 100.
+    - max_features (int): The maximum number of features to allow in the reduced subset. When this number is reached, no more features are added even if the earlystopping criterion is not reached yet.
+      This is only used when keep_all is false. By default, max_features is 100.
 
-        patience (int): The patience for earlystopping. When earlystopping is reached, <patience> more features are added to the reduced set to test whether the optimization metric on the validation set improves again. By default, patience is 5.
+    - patience (int): The patience for earlystopping. When earlystopping is reached, <patience> more features are added to the reduced set to test whether the optimization metric on the validation set improves again. By default, patience is 5.
 
-        min_delta (float): The delta value used to test if there was improvement between the previous set of features and the new set of features (+1). By default, min_delta is 0, meaning the new set of features does not need to yield a higher optimization metric score on the validation set, but it needs to be at least equally high as the previous set.
+    - min_delta (float): The delta value used to test if there was improvement between the previous set of features and the new set of features (+1). By default, min_delta is 0, meaning the new set of features does not need to yield a higher optimization metric score on the validation set, but it needs to be at least equally high as the previous set.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_motif_classifier:
-            MotifClassifier:
-                training_percentage: 0.7
-                max_features: 100
-                patience: 5
-                min_delta: 0
-                keep_all: false
+        definitions:
+            ml_methods:
+                my_motif_classifier:
+                    MotifClassifier:
+                        training_percentage: 0.7
+                        max_features: 100
+                        patience: 5
+                        min_delta: 0
+                        keep_all: false
 
     """
 
     def __init__(self, training_percentage: float = None,
                  random_seed: int = None, max_features: int = None, patience: int = None,
                  min_delta: float = None, keep_all: bool = None,
                  result_path: Path = None):
@@ -86,35 +88,27 @@
         self.keep_all = keep_all
 
         self.train_indices = None
         self.val_indices = None
         self.feature_names = None
         self.rule_tree_indices = None
         self.rule_tree_features = None
-        self.label = None
-        self.optimization_metric = None
-        self.class_mapping = None
 
         self.result_path = result_path
 
-    def predict(self, encoded_data: EncodedData, label: Label):
+    def _predict(self, encoded_data: EncodedData):
         self._check_features(encoded_data.feature_names)
 
         return {self.label.name: self._get_rule_tree_predictions_class(encoded_data, self.rule_tree_indices)}
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         warnings.warn(f"{BinaryFeatureClassifier.__name__}: cannot predict probabilities.")
         return None
 
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric: str, cores_for_training: int = 2):
-        self.feature_names = encoded_data.feature_names
-        self.label = label
-        self.class_mapping = Util.make_binary_class_mapping(encoded_data.labels[self.label.name])
-        self.optimization_metric = optimization_metric
-
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
         self.rule_tree_indices = self._build_rule_tree(encoded_data, cores_for_training)
         self.rule_tree_features = self._get_rule_tree_features_from_indices(self.rule_tree_indices, self.feature_names)
         self._export_selected_features(self.result_path, self.rule_tree_features)
 
         logging.info(f"{BinaryFeatureClassifier.__name__}: finished training.")
 
     def _get_optimization_scoring_fn(self):
@@ -262,22 +256,14 @@
             return prev_train_performance
         else:
             optimization_scoring_fn = self._get_optimization_scoring_fn()
             return optimization_scoring_fn(y_true=y_true_train,
                                            y_pred=new_predictions,
                                            sample_weight=example_weights)
 
-
-    # def _apply_optimization_fn_to_new_rule_combo(self, optimization_scoring_fn, examples, y_true_train,
-    #                                              example_weights, prev_predictions, new_rule_idx):
-    #     return optimization_scoring_fn(y_true=y_true_train,
-    #                                    y_pred=np.logical_or(prev_predictions, examples[:, new_rule_idx]),
-    #                                    sample_weight=example_weights)
-    #
-
     def _get_unused_rule_indices(self, encoded_train_data, rule_indices):
         return [idx for idx in range(encoded_train_data.examples.shape[1]) if idx not in rule_indices]
 
     def _test_performance_predictions(self, encoded_data, pred):
         y_true = Util.map_to_new_class_values(encoded_data.labels[self.label.name], self.class_mapping)
         optimization_scoring_fn = self._get_optimization_scoring_fn()
 
@@ -309,76 +295,62 @@
 
     def _export_selected_features(self, path, rule_tree_features):
         if path is not None:
             PathBuilder.build(path)
             with open(path / "selected_features.txt", "w") as file:
                 file.writelines([f"{feature}\n" for feature in rule_tree_features])
 
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5, cores_for_training: int = -1):
-        logging.warning(f"{BinaryFeatureClassifier.__name__}: cross_validation is not implemented for this method. Using standard fitting instead...")
-        self.fit(encoded_data=encoded_data, label=label)
-
     def _prepare_and_split_data(self, encoded_data: EncodedData):
         train_indices, val_indices = Util.get_train_val_indices(len(encoded_data.example_ids), self.training_percentage, random_seed=self.random_seed)
 
         self.train_indices = train_indices
         self.val_indices = val_indices
 
         train_data = Util.subset_encoded_data(encoded_data, train_indices)
         val_data = Util.subset_encoded_data(encoded_data, val_indices)
 
         return train_data, val_data
 
-    def store(self, path: Path, feature_names=None, details_path: Path = None):
+    def store(self, path: Path):
         PathBuilder.build(path)
 
-        custom_vars = copy.deepcopy(vars(self))
-        del custom_vars["result_path"]
-
-        if self.label:
-            custom_vars["label"] = {key.lstrip("_"): value for key, value in vars(self.label).items()}
-
-        params_path = path / "custom_params.yaml"
+        custom_vars = self.get_params()
+        params_path = self._get_custom_params_path(path)
         with params_path.open('w') as file:
             yaml.dump(custom_vars, file)
 
     def load(self, path):
-        params_path = path / "custom_params.yaml"
+        params_path = self._get_custom_params_path(path)
         with params_path.open("r") as file:
             custom_params = yaml.load(file, Loader=yaml.SafeLoader)
 
         for param, value in custom_params.items():
             if hasattr(self, param):
                 if param == "label":
                     setattr(self, "label", Label(**value))
                 else:
                     setattr(self, param, value)
 
-    def check_if_exists(self, path):
-        return self.rule_tree_indices is not None
+    def _get_custom_params_path(self, path):
+        return path / "custom_params.yaml"
 
     def get_params(self):
         params = copy.deepcopy(vars(self))
-        return params
-
-    def get_label_name(self):
-        return self.label.name
+        del params["result_path"]
 
-    def get_package_info(self) -> str:
-        return Util.get_immuneML_version()
+        if self.label:
+            params["label"] = self.label.get_desc_for_storage()
 
-    def get_feature_names(self) -> list:
-        return self.feature_names
+        return params
 
     def can_predict_proba(self) -> bool:
         return False
 
-    def get_class_mapping(self) -> dict:
-        return self.class_mapping
+    def can_fit_with_example_weights(self) -> bool:
+        return True
 
     def get_compatible_encoders(self):
         from immuneML.encodings.motif_encoding.MotifEncoder import MotifEncoder
         from immuneML.encodings.motif_encoding.SimilarToPositiveSequenceEncoder import SimilarToPositiveSequenceEncoder
         return [MotifEncoder, SimilarToPositiveSequenceEncoder]
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/KerasSequenceCNN.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/KerasSequenceCNN.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,75 +20,76 @@
 
     Reference:
     Derek M. Mason, Simon Friedensohn, Cédric R. Weber, Christian Jordi, Bastian Wagner, Simon M. Men1, Roy A. Ehling,
     Lucia Bonati, Jan Dahinden, Pablo Gainza, Bruno E. Correia and Sai T. Reddy
     ‘Optimization of therapeutic antibodies by predicting antigen specificity from antibody sequence via deep learning’.
     Nat Biomed Eng 5, 600–612 (2021). https://doi.org/10.1038/s41551-021-00699-9
 
-    Arguments:
+    **Specification arguments:**
 
-        units_per_layer (list): A nested list specifying the layers of the CNN. The first element in each nested list defines the layer type, other elements define the layer parameters.
-        Valid layer types are: CONV (keras.layers.Conv1D), DROP (keras.layers.Dropout), POOL (keras.layers.MaxPool1D), FLAT (keras.layers.Flatten), DENSE (keras.layers.Dense).
-        The parameters per layer type are as follows:
+    - units_per_layer (list): A nested list specifying the layers of the CNN. The first element in each nested list defines the layer type, other elements define the layer parameters.
+      Valid layer types are: CONV (keras.layers.Conv1D), DROP (keras.layers.Dropout), POOL (keras.layers.MaxPool1D), FLAT (keras.layers.Flatten), DENSE (keras.layers.Dense).
+      The parameters per layer type are as follows:
 
         - [CONV, <filters>, <kernel_size>, <strides>]
 
         - [DROP, <rate>]
 
         - [POOL, <pool_size>, <strides>]
 
         - [FLAT]
 
         - [DENSE, <units>]
 
-        activation (str): The Activation function to use in the convolutional or dense layers. Activation functions can be chosen from keras.activations. For example, rely or softmax. By default, relu is used.
+    - activation (str): The Activation function to use in the convolutional or dense layers. Activation functions can be chosen from keras.activations. For example, rely or softmax. By default, relu is used.
 
-        training_percentage (float): The fraction of sequences that will be randomly assigned to form the training set (the rest will be the validation set). Should be a value between 0 and 1. By default, training_percentage is 0.7.
+    - training_percentage (float): The fraction of sequences that will be randomly assigned to form the training set (the rest will be the validation set). Should be a value between 0 and 1. By default, training_percentage is 0.7.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_cnn:
-            KerasSequenceCNN:
-                training_percentage: 0.7
-                units_per_layer: [[CONV, 400, 3, 1], [DROP, 0.5], [POOL, 2, 1], [FLAT], [DENSE, 50]]
-                activation: relu
+        definitions:
+            ml_methods:
+                my_cnn:
+                    KerasSequenceCNN:
+                        training_percentage: 0.7
+                        units_per_layer: [[CONV, 400, 3, 1], [DROP, 0.5], [POOL, 2, 1], [FLAT], [DENSE, 50]]
+                        activation: relu
 
 
 
     """
 
     def __init__(self, units_per_layer: list = None, activation: str = None, training_percentage: float = None):
 
         super().__init__()
 
         self.units_per_layer = units_per_layer # todo refactor this to something more sensible
         self.activation = activation
         self.training_percentage = training_percentage
 
         self.background_probabilities = None
-        self.CNN = None
         self.label = None
         self.class_mapping = None
         self.result_path = None
         self.feature_names = None
 
-    def predict(self, encoded_data: EncodedData, label: Label):
-        predictions_proba = self.predict_proba(encoded_data, label)[label.name][label.positive_class]
+    def _predict(self, encoded_data: EncodedData):
+        predictions_proba = self._predict_proba(encoded_data)[self.label.name][self.label.positive_class]
 
-        return {label.name: [self.class_mapping[val] for val in (predictions_proba > 0.5).tolist()]}
+        return {self.label.name: [self.class_mapping[val] for val in (predictions_proba > 0.5).tolist()]}
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         predictions = self.model.predict(x=encoded_data.examples).flatten()
 
-        return {label.name: {label.positive_class: predictions,
-                             label.get_binary_negative_class(): 1 - predictions}}
+        return {self.label.name: {self.label.positive_class: predictions,
+                                  self.label.get_binary_negative_class(): 1 - predictions}}
 
     def _create_cnn(self, units_per_layer, input_shape,
                activation):
         """
         Based on: https://github.com/dahjan/DMS_opt/blob/master/scripts/CNN.py
 
         Generate the CNN layers with a Keras wrapper.
@@ -143,37 +144,33 @@
 
         # Output layer
         # Activation function: Sigmoid
         model.add(keras.layers.Dense(1, activation='sigmoid'))
 
         return model
 
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-        self.feature_names = encoded_data.feature_names
-        self.label = label
-        self.class_mapping = Util.make_binary_class_mapping(encoded_data.labels[self.label.name])
-
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
         encoded_train_data, encoded_val_data = self._prepare_and_split_data(encoded_data)
 
-        self.model = self._create_cnn(units_per_layer=self.units_per_layer, # todo better input format...
+        self.model = self._create_cnn(units_per_layer=self.units_per_layer,
                                       input_shape=encoded_data.examples.shape[1:],
                                       activation=self.activation)
 
-        self._fit(encoded_train_data=encoded_train_data, encoded_val_data=encoded_val_data)
+        self._fit_model(encoded_train_data=encoded_train_data, encoded_val_data=encoded_val_data)
 
 
     def _prepare_and_split_data(self, encoded_data: EncodedData):
         train_indices, val_indices = Util.get_train_val_indices(len(encoded_data.example_ids), self.training_percentage)
 
         train_data = Util.subset_encoded_data(encoded_data, train_indices)
         val_data = Util.subset_encoded_data(encoded_data, val_indices)
 
         return train_data, val_data
 
-    def _fit(self, encoded_train_data, encoded_val_data):
+    def _fit_model(self, encoded_train_data, encoded_val_data):
         """reference to original code, maybe the input should just be the encoded data instead? #todo"""
         from keras.optimizers import Adam
 
         X_train = encoded_train_data.examples
         X_val = encoded_val_data.examples
         y_train = Util.map_to_new_class_values(encoded_train_data.labels[self.label.name], self.class_mapping)
         y_val = Util.map_to_new_class_values(encoded_val_data.labels[self.label.name], self.class_mapping)
@@ -187,26 +184,20 @@
         # Fit the CNN to the training set
         _ = self.model.fit(
             x=X_train, y=y_train, sample_weight=w_train, shuffle=True,
             validation_data=(X_val, y_val, w_val) if w_val is not None else (X_val, y_val),
             epochs=20, batch_size=16, verbose=0
         )
 
-
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5, cores_for_training: int = -1):
-        logging.warning(f"{KerasSequenceCNN.__name__}: cross_validation is not implemented for this method. Using standard fitting instead...")
-        self.fit(encoded_data=encoded_data, label=label)
-
-    def store(self, path: Path, feature_names=None, details_path: Path = None):
+    def store(self, path: Path):
         PathBuilder.build(path)
 
-        self.model.save(path / "model")
+        self.model.save(path / "model.keras")
 
-        custom_vars = copy.deepcopy(vars(self))
+        custom_vars = self.get_params()
         del custom_vars["model"]
         del custom_vars["result_path"]
 
         if self.label:
             custom_vars["label"] = self.label.get_desc_for_storage()
 
         params_path = path / "custom_params.yaml"
@@ -224,38 +215,33 @@
         for param, value in custom_params.items():
             if hasattr(self, param):
                 if param == "label":
                     setattr(self, "label", Label(**value))
                 else:
                     setattr(self, param, value)
 
-        self.model = keras.models.load_model(path / "model")
-
-    def check_if_exists(self, path):
-        return self.model is not None
+        self.model = keras.models.load_model(path / "model.keras")
 
     def get_params(self):
-        params = copy.deepcopy(vars(self))
-        params["model"] = copy.deepcopy(self.model).state_dict()
-        return params
+        params = dict()
 
-    def get_label_name(self):
-        return self.label.name
+        # using 'deepcopy' on the model directly results in an error, therefore loop over all other items
+        for key, value in vars(self).items():
+            if key != "model":
+                params[key] = copy.deepcopy(value)
 
-    def get_package_info(self) -> str:
-        return Util.get_immuneML_version()
+        params["model"] = copy.deepcopy(self.model.get_config())
 
-    def get_feature_names(self) -> list:
-        return self.feature_names
+        return params
 
     def can_predict_proba(self) -> bool:
         return True
 
-    def get_class_mapping(self) -> dict:
-        return self.class_mapping
+    def can_fit_with_example_weights(self) -> bool:
+        return True
 
     def get_compatible_encoders(self):
         from immuneML.encodings.onehot.OneHotEncoder import OneHotEncoder
         return [OneHotEncoder]
 
     def check_encoder_compatibility(self, encoder):
         """Checks whether the given encoder is compatible with this ML method, and throws an error if it is not."""
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/AtchleyKmerMILClassifier.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/AtchleyKmerMILClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     A binary Repertoire classifier which uses the data encoded by :ref:`AtchleyKmer` encoder to predict the repertoire label.
 
     The original publication:
     Ostmeyer J, Christley S, Toby IT, Cowell LG. Biophysicochemical motifs in T cell receptor sequences distinguish repertoires from tumor-infiltrating
     lymphocytes and adjacent healthy tissue. Cancer Res. Published online January 1, 2019:canres.2292.2018. `doi:10.1158/0008-5472.CAN-18-2292
     <https://cancerres.aacrjournals.org/content/79/7/1671>`_ .
 
-    Specification arguments:
+    **Specification arguments:**
 
     - iteration_count (int): max number of training iterations
 
     - threshold (float): loss threshold at which to stop training if reached
 
     - evaluate_at (int): log model performance every 'evaluate_at' iterations and store the model every 'evaluate_at' iterations if early stopping
       is used
@@ -46,68 +46,59 @@
 
     - number_of_threads: number of threads to be used for training
 
     - initialization_count (int): how many times to repeat the fitting procedure from the beginning before choosing the optimal model (trains the model with multiple random initializations)
 
     - pytorch_device_name (str): The name of the pytorch device to use. This name will be passed to torch.device(pytorch_device_name).
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_kmer_mil_classifier:
-            AtchleyKmerMILClassifier:
-                iteration_count: 100
-                evaluate_at: 15
-                use_early_stopping: False
-                learning_rate: 0.01
-                random_seed: 100
-                zero_abundance_weight_init: True
-                number_of_threads: 8
-                threshold: 0.00001
-                initialization_count: 4
+        definitions:
+            ml_methods:
+                my_kmer_mil_classifier:
+                    AtchleyKmerMILClassifier:
+                        iteration_count: 100
+                        evaluate_at: 15
+                        use_early_stopping: False
+                        learning_rate: 0.01
+                        random_seed: 100
+                        zero_abundance_weight_init: True
+                        number_of_threads: 8
+                        threshold: 0.00001
+                        initialization_count: 4
 
     """
 
     MIN_SEED_VALUE = 1
     MAX_SEED_VALUE = 100000
 
     def __init__(self, iteration_count: int = None, threshold: float = None, evaluate_at: int = None, use_early_stopping: bool = None,
                  random_seed: int = None, learning_rate: float = None, zero_abundance_weight_init: bool = None, number_of_threads: int = None,
-                 result_path: Path = None, initialization_count: int = None, pytorch_device_name: str = None):
+                 initialization_count: int = None, pytorch_device_name: str = None):
         super().__init__()
         self.logistic_regression = None
         self.random_seed = random_seed
         self.iteration_count = iteration_count
         self.threshold = threshold
         self.evaluate_at = evaluate_at
         self.use_early_stopping = use_early_stopping
         self.learning_rate = learning_rate
         self.zero_abundance_weight_init = zero_abundance_weight_init
         self.number_of_threads = number_of_threads
-        self.class_mapping = None
         self.input_size = 0
-        self.result_path = result_path
-        self.feature_names = None
         self.initialization_count = initialization_count
         self.pytorch_device_name = pytorch_device_name
 
     def _make_log_reg(self):
         return PyTorchLogisticRegression(in_features=self.input_size, zero_abundance_weight_init=self.zero_abundance_weight_init)
 
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-        if encoded_data.example_weights is not None:
-            warnings.warn(f"{self.__class__.__name__}: cannot fit this classifier with example weights, fitting without example weights instead... Example weights will still be applied when computing evaluation metrics after fitting.")
-
-        self.feature_names = encoded_data.feature_names
-
-        self.label = label
-        self.class_mapping = Util.make_binary_class_mapping(encoded_data.labels[self.label.name], self.label.positive_class)
-
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int):
         mapped_y = Util.map_to_new_class_values(encoded_data.labels[self.label.name], self.class_mapping)
         self.logistic_regression = None
         min_loss = np.inf
 
         for initialization in range(self.initialization_count):
 
             random.seed(self.random_seed)
@@ -165,89 +156,74 @@
                 logits = log_reg(torch.from_numpy(np.swapaxes(data, 1, 2).reshape(data.shape[0] * data.shape[2], -1)))
             else:
                 logits = self.logistic_regression(torch.from_numpy(np.swapaxes(data, 1, 2).reshape(data.shape[0] * data.shape[2], -1)))
         logits = torch.reshape(logits, (data.shape[0], data.shape[2]))
         max_logits_indices = torch.argmax(logits, dim=1)
         return max_logits_indices.long()
 
-    def predict(self, encoded_data: EncodedData, label: Label):
-        predictions_proba = self.predict_proba(encoded_data, label)
-        return {label.name: [self.class_mapping[val] for val in (predictions_proba[label.name][label.positive_class] > 0.5).tolist()]}
-
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5, cores_for_training: int = -1):
-        logging.warning(f"AtchleyKmerMILClassifier: fitting by cross validation is not implemented internally for the model, fitting without "
-                        f"cross-validation instead.")
-        self.fit(encoded_data=encoded_data, label=label)
+    def _predict(self, encoded_data: EncodedData):
+        predictions_proba = self._predict_proba(encoded_data)
+        return {self.label.name: [self.class_mapping[val] for val in (predictions_proba[self.label.name][self.label.positive_class] > 0.5).tolist()]}
 
-    def store(self, path: Path, feature_names=None, details_path: Path = None):
+    def store(self, path: Path):
         PathBuilder.build(path)
         torch.save(copy.deepcopy(self.logistic_regression).state_dict(), str(path / "log_reg.pt"))
         custom_vars = copy.deepcopy(vars(self))
 
-        coefficients_df = pd.DataFrame(custom_vars["logistic_regression"].linear.weight.detach().numpy(), columns=feature_names)
+        coefficients_df = pd.DataFrame(custom_vars["logistic_regression"].linear.weight.detach().numpy(), columns=self.feature_names)
         coefficients_df["bias"] = custom_vars["logistic_regression"].linear.bias.detach().numpy()
         coefficients_df.to_csv(path / "coefficients.csv", index=False)
 
         del custom_vars["result_path"]
         del custom_vars["logistic_regression"]
         del custom_vars["label"]
 
         if self.label:
             custom_vars["label"] = self.label.get_desc_for_storage()
 
-        params_path = path / "custom_params.yaml"
+        params_path = self._get_custom_params_path(path)
         with params_path.open('w') as file:
             yaml.dump(custom_vars, file)
 
     def load(self, path):
-        params_path = path / "custom_params.yaml"
+        params_path = self._get_custom_params_path(path)
         with params_path.open("r") as file:
             custom_params = yaml.load(file, Loader=yaml.SafeLoader)
 
         for param, value in custom_params.items():
             if hasattr(self, param):
                 if param == "label":
                     setattr(self, "label", Label(**value))
                 else:
                     setattr(self, param, value)
 
         self.logistic_regression = self._make_log_reg()
         self.logistic_regression.load_state_dict(torch.load(str(path / "log_reg.pt")))
 
-    def check_if_exists(self, path) -> bool:
-        return self.logistic_regression is not None
+    def _get_custom_params_path(self, path):
+        return path / "custom_params.yaml"
 
     def get_params(self):
         params = copy.deepcopy(vars(self))
         params["logistic_regression"] = copy.deepcopy(self.logistic_regression).state_dict()
         return params
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         self.logistic_regression.eval()
         example_count = encoded_data.examples.shape[0]
         max_logit_indices = self._get_max_logits_indices(encoded_data.examples)
         with torch.no_grad():
             data = torch.from_numpy(encoded_data.examples).float()[torch.arange(example_count).long(), :, max_logit_indices]
             predictions = torch.sigmoid(self.logistic_regression(data)).numpy()
 
-        return {label.name: {label.positive_class: predictions,
-                             label.get_binary_negative_class(): 1 - predictions}}
-
-    def get_label_name(self):
-        return self.label.name
-
-    def get_package_info(self) -> str:
-        return Util.get_immuneML_version()
-
-    def get_feature_names(self) -> list:
-        return self.feature_names
+        return {self.label.name: {self.label.positive_class: predictions,
+                                  self.label.get_binary_negative_class(): 1 - predictions}}
 
     def can_predict_proba(self) -> bool:
         return True
 
-    def get_class_mapping(self) -> dict:
-        return self.class_mapping
+    def can_fit_with_example_weights(self) -> bool:
+        return False
 
     def get_compatible_encoders(self):
         from immuneML.encodings.atchley_kmer_encoding.AtchleyKmerEncoder import AtchleyKmerEncoder
         return [AtchleyKmerEncoder]
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/DeepRC.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/DeepRC.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Reference:
     Michael Widrich, Bernhard Schäfl, Milena Pavlović, Geir Kjetil Sandve, Sepp Hochreiter, Victor Greiff, Günter Klambauer
     ‘DeepRC: Immune repertoire classification with attention-based deep massive multiple instance learning’.
     bioRxiv preprint doi: `https://doi.org/10.1101/2020.04.12.038158 <https://doi.org/10.1101/2020.04.12.038158>`_
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - validation_part (float):  the part of the data that will be used for validation, the rest will be used for training.
 
     - add_positional_information (bool): whether positional information should be included in the input features.
 
     - kernel_size (int): the size of the 1D-CNN kernels.
 
@@ -81,24 +81,26 @@
     - training_batch_size (int): Number of repertoires per minibatch during training.
 
     - n_workers (int): Number of background processes to use for converting dataset to hdf5 container and training set data loader.
 
     - pytorch_device_name (str): The name of the pytorch device to use. This name will be passed to  torch.device(self.pytorch_device_name). The default value is cuda:0
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_deeprc_method:
-            DeepRC:
-                validation_part: 0.2
-                add_positional_information: True
-                kernel_size: 9
+        definitions:
+            ml_methods:
+                my_deeprc_method:
+                    DeepRC:
+                        validation_part: 0.2
+                        add_positional_information: True
+                        kernel_size: 9
 
     """
 
     def __init__(self, validation_part, add_positional_information, kernel_size, n_kernels,
                  n_additional_convs, n_attention_network_layers, n_attention_network_units, n_output_network_units,
                  consider_seq_counts, sequence_reduction_fraction, reduction_mb_size, n_updates, n_torch_threads,
                  learning_rate, l1_weight_decay, l2_weight_decay, evaluate_at, sample_n_sequences, training_batch_size,
@@ -110,18 +112,15 @@
                                f"https://docs.immuneml.uio.no/installation/install_with_package_manager.html for "
                                f"instructions how to install it.")
 
         from deeprc.training import train
         self.training_function = train
 
         self.model = None
-        self.result_path = None
-
         self.max_seq_len = None
-        self.label = None
 
         self.keep_dataset_in_ram = keep_dataset_in_ram
         self.pytorch_device_name = pytorch_device_name
         self.pytorch_device = torch.device(self.pytorch_device_name)
 
         # ML model setting (not inherited from DeepRC code)
         self.validation_part = validation_part
@@ -152,16 +151,14 @@
         self.l2_weight_decay = l2_weight_decay
 
         # Dataloader related settings:
         self.sample_n_sequences = sample_n_sequences
         self.training_batch_size = training_batch_size
         self.n_workers = n_workers
 
-        self.feature_names = None
-
     def _metadata_to_hdf5(self, metadata_filepath: Path, label_name: str):
         from deeprc.dataset_converters import DatasetToHDF5
 
         hdf5_filepath = metadata_filepath.parent / f"{metadata_filepath.stem}.hdf5"
         converter = DatasetToHDF5(repertoiresdata_directory=str(metadata_filepath.parent),
                                   sequence_column=DeepRCEncoder.SEQUENCE_COLUMN,
                                   sequence_counts_column=DeepRCEncoder.COUNTS_COLUMN,
@@ -245,24 +242,19 @@
                 ("l2_weight_decay", self.l2_weight_decay),
                 ("sample_n_sequences", self.sample_n_sequences),
                 ("training_batch_size", self.training_batch_size),
                 ("n_workers", self.n_workers),
                 ("evaluate_at", self.evaluate_at),
                 ("pytorch_device_name", self.pytorch_device_name))
 
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-        if encoded_data.example_weights is not None:
-            warnings.warn(f"{self.__class__.__name__}: cannot fit this classifier with example weights, fitting without example weights instead... Example weights will still be applied when computing evaluation metrics after fitting.")
-
-        self.feature_names = encoded_data.feature_names
-        self.label = label
-        self.model = CacheHandler.memo_by_params(self._prepare_caching_params(encoded_data, "fit", label.name),
-                                                 lambda: self._fit(encoded_data, label, cores_for_training))
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
+        self.model = CacheHandler.memo_by_params(self._prepare_caching_params(encoded_data, "fit", self.label.name),
+                                                 lambda: self._fit(encoded_data, self.label, cores_for_training))
 
-    def _fit(self, encoded_data: EncodedData, label: Label, cores_for_training: int = 2):
+    def _fit_model(self, encoded_data: EncodedData, label: Label, cores_for_training: int = 2):
 
         hdf5_filepath, pre_loaded_hdf5_file = self._convert_dataset_to_hdf5(encoded_data, label)
 
         train_indices, val_indices = self._get_train_val_indices(len(encoded_data.example_ids),
                                                                  encoded_data.labels[label.name])
         self.max_seq_len = encoded_data.info["max_sequence_length"]
 
@@ -348,53 +340,47 @@
                                results_directory=self.result_path / "deep_rc_log",
                                n_updates=self.n_updates, num_torch_threads=self.n_torch_threads,
                                learning_rate=self.learning_rate,
                                l1_weight_decay=self.l1_weight_decay, l2_weight_decay=self.l2_weight_decay,
                                show_progress=False, device=self.pytorch_device, evaluate_at=self.evaluate_at,
                                task_definition=task_definition, early_stopping_target_id=label.name)
 
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5,  cores_for_training: int = -1):
-        warnings.warn("DeepRC: cross-validation on this classifier is not defined: fitting one model instead...")
-        self.fit(encoded_data, label)
-
     def get_params(self):
         return {name: param.data.tolist() for name, param in self.model.named_parameters()}
 
     def check_is_fitted(self, label_name: str):
         if label_name != self.label.name:
             raise NotFittedError("This DeepRCs instance is not fitted yet. "
                                  "Call 'fit' with appropriate arguments before using this method.")
 
-    def predict(self, encoded_data: EncodedData, label: Label):
-        probabilities = self.predict_proba(encoded_data, label)
+    def _predict(self, encoded_data: EncodedData):
+        probabilities = self._predict_proba(encoded_data)
 
-        pos_class_probs = probabilities[label.name][label.positive_class]
-        negative_class = label.get_binary_negative_class()
+        pos_class_probs = probabilities[self.label.name][self.label.positive_class]
+        negative_class = self.label.get_binary_negative_class()
 
-        # TODO: check what is returned here and how it works with multiclass
-        return {label.name: [label.positive_class if probability > 0.5 else negative_class for probability in
+        return {self.label.name: [self.label.positive_class if probability > 0.5 else negative_class for probability in
                              pos_class_probs]}
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         from deeprc.dataset_readers import RepertoireDataset as DeepRCRepDataset
-        self.check_is_fitted(label.name)
+        self.check_is_fitted(self.label.name)
 
-        hdf5_filepath, _ = self._convert_dataset_to_hdf5(encoded_data, label)
-        task_definition = self._make_task_definition(label)
+        hdf5_filepath, _ = self._convert_dataset_to_hdf5(encoded_data, self.label)
+        task_definition = self._make_task_definition(self.label)
 
         test_dataset = DeepRCRepDataset(metadata_filepath=encoded_data.info['metadata_filepath'],
                                         hdf5_filepath=str(hdf5_filepath),
                                         sample_id_column=DeepRCEncoder.ID_COLUMN,
                                         metadata_file_column_sep=DeepRCEncoder.SEP,
                                         task_definition=task_definition, keep_in_ram=self.keep_dataset_in_ram,
                                         inputformat='NCL',
                                         sequence_counts_scaling_fn=self.sequence_counts_scaling_fn)
 
-        test_dataloader = self.make_data_loader(test_dataset, indices=None, label_name=label.name, eval_only=True,
+        test_dataloader = self.make_data_loader(test_dataset, indices=None, label_name=self.label.name, eval_only=True,
                                                 is_train=False)
 
         probs_pos_class = self._model_predict(self.model, test_dataloader)
 
         # TODO: update for multiclass
         return {label.name: {label.positive_class: probs_pos_class,
                              label.get_binary_negative_class(): 1 - probs_pos_class}}
@@ -421,75 +407,58 @@
                 scoring_predictions.append(prediction)
 
             # predictions
             scoring_predictions = torch.cat(scoring_predictions, dim=0).float().cpu().numpy()
 
         return scoring_predictions
 
-    def load(self, path: Path, details_path: Path = None):
+    def load(self, path: Path):
         name = FilenameHandler.get_filename(self.__class__.__name__, "pt")
         file_path = path / name
         if file_path.is_file():
             self.model = torch.load(str(file_path))
             self.model.eval()
         else:
             raise FileNotFoundError(f"{self.__class__.__name__} model could not be loaded from {file_path}. "
                                     f"Check if the path to the {name} file is properly set.")
 
-        if details_path is None:
-            params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
-        else:
-            params_path = details_path
+        params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
 
         if params_path.is_file():
             with params_path.open("r") as file:
                 desc = yaml.safe_load(file)
                 if "label" in desc:
                     setattr(self, "label", Label(**desc["label"]))
                 for param in ["feature_names", "classes"]:
                     if param in desc:
                         setattr(self, param, desc[param])
 
-    def store(self, path, feature_names=None, details_path: Path = None):
+    def store(self, path):
         PathBuilder.build(path)
         name = FilenameHandler.get_filename(self.__class__.__name__, "pt")
         torch.save(self.model, str(path / name))
 
-        if details_path is None:
-            params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
-        else:
-            params_path = details_path
+        params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
 
         with params_path.open("w") as file:
             desc = {
                 **(self.get_params()),
-                "feature_names": feature_names,
+                "feature_names": self.get_feature_names(),
                 "classes": self.get_classes()
             }
             if self.label is not None:
                 desc["label"] = self.label.get_desc_for_storage()
 
             yaml.dump(desc, file)
 
-    def check_if_exists(self, path):
-        file_path = path / FilenameHandler.get_filename(self.__class__.__name__, "pt")
-
-        return file_path.is_file()
 
     def get_package_info(self) -> str:
-        return 'immuneML ' + Util.get_immuneML_version() + '; deepRC ' + pkg_resources.get_distribution(
-            'DeepRC').version
-
-    def get_feature_names(self) -> list:
-        return self.feature_names
+        return Util.get_immuneML_version() + '; deepRC ' + pkg_resources.get_distribution('DeepRC').version
 
     def can_predict_proba(self) -> bool:
         return True
 
-    def get_class_mapping(self) -> dict:
-        return {}
-
-    def get_label_name(self) -> str:
-        return self.label.name
+    def can_fit_with_example_weights(self) -> bool:
+        return False
 
     def get_compatible_encoders(self):
         return [DeepRCEncoder]
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/KNN.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/KNN.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,33 +11,35 @@
     matrix (for example, when using the :ref:`Distance` or :ref:`CompAIRRDistance` encoders), please use :ref:`PrecomputedKNN` instead.
 
     Please see the `scikit-learn documentation <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html>`_
     of KNeighborsClassifier for the parameters.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_knn_method:
-            KNN:
-                # sklearn parameters (same names as in original sklearn class)
-                weights: uniform # always use this setting for weights
-                n_neighbors: [5, 10, 15] # find the optimal number of neighbors
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under KNN is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_knn: KNN
+        definitions:
+            ml_methods:
+                my_knn_method:
+                    KNN:
+                        # sklearn parameters (same names as in original sklearn class)
+                        weights: uniform # always use this setting for weights
+                        n_neighbors: [5, 10, 15] # find the optimal number of neighbors
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under KNN is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_knn: KNN
 
     """
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         parameters = parameters if parameters is not None else {}
         parameter_grid = parameter_grid if parameter_grid is not None else {}
 
@@ -50,14 +52,17 @@
 
     def get_params(self):
         return self.model.get_params(deep=True)
 
     def can_predict_proba(self) -> bool:
         return True
 
+    def can_fit_with_example_weights(self) -> bool:
+        return False
+
     def get_compatible_encoders(self):
         from immuneML.encodings.distance_encoding.DistanceEncoder import DistanceEncoder
         from immuneML.encodings.evenness_profile.EvennessProfileEncoder import EvennessProfileEncoder
         from immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder import SequenceAbundanceEncoder
         from immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder import CompAIRRSequenceAbundanceEncoder
         from immuneML.encodings.abundance_encoding.KmerAbundanceEncoder import KmerAbundanceEncoder
         from immuneML.encodings.kmer_frequency.KmerFrequencyEncoder import KmerFrequencyEncoder
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/LogisticRegression.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/LogisticRegression.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 
     Note: if you are interested in plotting the coefficients of the logistic regression model,
     consider running the :ref:`Coefficients` report.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_logistic_regression: # user-defined method name
-            LogisticRegression: # name of the ML method
-                # sklearn parameters (same names as in original sklearn class)
-                penalty: l1 # always use penalty l1
-                C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under LogisticRegression is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_logistic_regression: LogisticRegression
+        definitions:
+            ml_methods:
+                my_logistic_regression: # user-defined method name
+                    LogisticRegression: # name of the ML method
+                        # sklearn parameters (same names as in original sklearn class)
+                        penalty: l1 # always use penalty l1
+                        C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under LogisticRegression is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_logistic_regression: LogisticRegression
 
     """
 
     default_parameters = {"max_iter": 1000, "solver": "saga"}
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         parameters = {**self.default_parameters, **(parameters if parameters is not None else {})}
@@ -54,14 +56,17 @@
         params = self._parameters.copy()
         params["n_jobs"] = cores_for_training
         return SklearnLogisticRegression(**params)
 
     def can_predict_proba(self) -> bool:
         return True
 
+    def can_fit_with_example_weights(self) -> bool:
+        return True
+
     def get_params(self):
         params = self.model.get_params()
         params["coefficients"] = self.model.coef_[0].tolist()
         params["intercept"] = self.model.intercept_.tolist()
         return params
 
     @staticmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/PrecomputedKNN.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/PrecomputedKNN.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,35 @@
 
     Please see the `scikit-learn documentation <https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html>`_
     of KNeighborsClassifier for the parameters.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_knn_method:
-            PrecomputedKNN:
-                # sklearn parameters (same names as in original sklearn class)
-                weights: uniform # always use this setting for weights
-                n_neighbors: [5, 10, 15] # find the optimal number of neighbors
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under KNN is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_knn: PrecomputedKNN
+        definitions:
+            ml_methods:
+                my_knn_method:
+                    PrecomputedKNN:
+                        # sklearn parameters (same names as in original sklearn class)
+                        weights: uniform # always use this setting for weights
+                        n_neighbors: [5, 10, 15] # find the optimal number of neighbors
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under KNN is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_knn: PrecomputedKNN
 
     """
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         parameters = parameters if parameters is not None else {}
         parameter_grid = parameter_grid if parameter_grid is not None else {}
 
@@ -53,14 +55,17 @@
 
     def get_params(self):
         return self.model.get_params(deep=True)
 
     def can_predict_proba(self) -> bool:
         return True
 
+    def can_fit_with_example_weights(self) -> bool:
+        return False
+
     def get_compatible_encoders(self):
         from immuneML.encodings.distance_encoding.CompAIRRDistanceEncoder import CompAIRRDistanceEncoder
         from immuneML.encodings.distance_encoding.DistanceEncoder import DistanceEncoder
 
         return [DistanceEncoder, CompAIRRDistanceEncoder]
 
     @staticmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/ProbabilisticBinaryClassifier.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/ProbabilisticBinaryClassifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,31 +26,33 @@
     examples using log-posterior odds ratio with threshold at 0.
 
     ProbabilisticBinaryClassifier is based on the paper (details on the classification can be found in the Online Methods section):
     Emerson, Ryan O., William S. DeWitt, Marissa Vignali, Jenna Gravley, Joyce K. Hu, Edward J. Osborne, Cindy Desmarais, et al.
     ‘Immunosequencing Identifies Signatures of Cytomegalovirus Exposure History and HLA-Mediated Effects on the T Cell Repertoire’.
     Nature Genetics 49, no. 5 (May 2017): 659–65. `doi.org/10.1038/ng.3822 <https://doi.org/10.1038/ng.3822>`_.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - max_iterations (int): maximum number of iterations while optimizing the parameters of the beta distribution (same for both classes)
 
     - update_rate (float): how much the computed gradient should influence the updated value of the parameters of the beta distribution
 
     - likelihood_threshold (float): at which threshold to stop the optimization (default -1e-10)
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_probabilistic_classifier: # user-defined name of the ML method
-            ProbabilisticBinaryClassifier: # method name
-                max_iterations: 1000
-                update_rate: 0.01
+        definitions:
+            ml_methods:
+                my_probabilistic_classifier: # user-defined name of the ML method
+                    ProbabilisticBinaryClassifier: # method name
+                        max_iterations: 1000
+                        update_rate: 0.01
 
     """
 
     SMALL_POSITIVE_NUMBER = 1e-15
 
     def __init__(self, max_iterations: int = None, update_rate: float = None, likelihood_threshold: float = None):
         super().__init__()
@@ -59,44 +61,30 @@
         self.N_0 = None
         self.N_1 = None
         self.alpha_0 = None
         self.alpha_1 = None
         self.beta_0 = None
         self.beta_1 = None
         self.likelihood_threshold = likelihood_threshold if likelihood_threshold is not None else -1e-10
-        self.class_mapping = None
-        self.label = None
-        self.feature_names = None
-
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-        if encoded_data.example_weights is not None:
-            warnings.warn(f"{self.__class__.__name__}: cannot fit this classifier with example weights, fitting without example weights instead... Example weights will still be applied when computing evaluation metrics after fitting.")
 
-        self.feature_names = encoded_data.feature_names
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
         X = encoded_data.examples
         assert X.shape[1] == 2, "ProbabilisticBinaryClassifier: the shape of the input is not compatible with the classifier. " \
                                 "The classifier is defined when examples are encoded by two counts: the number of successful trials " \
                                 "and the total number of trials. If this is not targeted use-case and the encoding, please consider using " \
                                 "another classifier."
 
-        self.class_mapping = Util.make_binary_class_mapping(encoded_data.labels[label.name], label.positive_class)
-        self.label = label
-        self.N_0 = int(np.sum(np.array(encoded_data.labels[label.name]) == self.class_mapping[0]))
-        self.N_1 = int(np.sum(np.array(encoded_data.labels[label.name]) == self.class_mapping[1]))
+        self.N_0 = int(np.sum(np.array(encoded_data.labels[self.label.name]) == self.class_mapping[0]))
+        self.N_1 = int(np.sum(np.array(encoded_data.labels[self.label.name]) == self.class_mapping[1]))
         self.alpha_0, self.beta_0 = self._find_beta_distribution_parameters(
             X[np.nonzero(np.array(encoded_data.labels[self.label.name]) == self.class_mapping[0])], self.N_0)
         self.alpha_1, self.beta_1 = self._find_beta_distribution_parameters(
             X[np.nonzero(np.array(encoded_data.labels[self.label.name]) == self.class_mapping[1])], self.N_1)
 
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5, cores_for_training: int = -1):
-        warnings.warn("ProbabilisticBinaryClassifier: cross-validation on this classifier is not defined: fitting one model instead...")
-        self.fit(encoded_data=encoded_data, label=label)
-
-    def predict(self, encoded_data: EncodedData, label: Label):
+    def _predict(self, encoded_data: EncodedData):
         """
         Predict the class assignment for examples in X (where X is validation or test set - examples not seen during training).
 
         .. math::
 
             \\widehat{c} \\, (k, n) = \\left\\{\\begin{matrix} 0, & F(k, n) \\leq 0\\\\ 1, & F(k, n) > 0 \\end{matrix}\\right
 
@@ -110,25 +98,24 @@
 
         Returns:
 
             a dictionary of the following format: {label_name: predictions} where predictions is a list of predicted classes for each example
 
         """
         X = encoded_data.examples
-        self._check_labels(label.name)
         predictions_list = []
         for example in X:
             k, n = example[0], example[1]
             F = self._compute_log_posterior_odds_ratio(k, n)
             predicted_class = int(F > 0)
             predictions_list.append(self.class_mapping[predicted_class])
 
         return {self.label.name: predictions_list}
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         """
         Predict the probability of the class for examples in X.
 
         .. math::
 
             \\widehat{c} \\, (k, n) = '\\left\\{\\begin{matrix} 0, & F(k, n) \\leq 0\\ 1, & F(k, n) > 0 \\end{matrix}\\right
 
@@ -140,24 +127,23 @@
             label (str): the label used for classification (e.g. CMV)
 
         Returns:
 
             class probabilities for all examples in X
 
         """
-        self._check_labels(label.name)
         X = encoded_data.examples
         class_probabilities = np.zeros((X.shape[0], len(list(self.class_mapping.keys()))), dtype=float)
 
         for index, example in enumerate(X):
             k, n = example[0], example[1]
             posterior_class_probabilities = self._compute_posterior_class_probability(k, n)
             class_probabilities[index] = posterior_class_probabilities
 
-        return {label.name: {self.class_mapping[i]: class_probabilities[:, i] for i in range(class_probabilities.shape[1])}}
+        return {self.label.name: {self.class_mapping[i]: class_probabilities[:, i] for i in range(class_probabilities.shape[1])}}
 
     def _find_beta_distribution_parameters(self, X, N_l: int) -> Tuple[float, float]:
         """
         Function implementing gradient ascent to find parameters of the beta distribution for the given class.
         It maximizes the following log-likelihood:
 
         .. math::
@@ -373,31 +359,28 @@
             elif isinstance(value, Label):
                 result[key] = value.name
             else:
                 result[key] = float(value)
 
         return result
 
-    def store(self, path: Path, feature_names=None, details_path=None):
+    def store(self, path: Path):
         content = self._convert_object_to_dict()
         PathBuilder.build(path)
         file_path = path / FilenameHandler.get_filename(self.__class__.__name__, "pickle")
 
         with file_path.open("wb") as file:
             pickle.dump(content, file)
 
-        if details_path is None:
-            params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
-        else:
-            params_path = details_path
+        params_path = path / FilenameHandler.get_filename(self.__class__.__name__, "yaml")
 
         with params_path.open("w") as file:
             desc = {self.label.name: {
                 **content,
-                "feature_names": feature_names,
+                "feature_names": self.get_feature_names(),
                 "classes": list(self.class_mapping.values())
             }}
             if self.label is not None:
                 desc["label"] = self.label.get_desc_for_storage()
 
             yaml.dump(desc, file)
 
@@ -420,41 +403,18 @@
         else:
             raise FileNotFoundError(f"{self.__class__.__name__} model could not be loaded from {file_path}. "
                                     f"Check if the path to the {file_path.name} file is properly set.")
 
     def get_params(self):
         return vars(self)
 
-    def check_if_exists(self, path):
-        vals = vars(self).values()
-        if any(val is None for val in vals):
-            return False
-        else:
-            return True
-
-    def _check_labels(self, label_name):
-        assert label_name == self.label.name, f"ProbabilisticBinaryClassifier: classifier cannot predict the labels " \
-                                              f"on which it was not trained: got: {label_name}, expected: {self.label.name}."
-
-    def get_label_name(self):
-        return self.label.name
-
-    def get_package_info(self) -> str:
-        return Util.get_immuneML_version()
-
-    def get_feature_names(self) -> list:
-        return self.feature_names
-
     def can_predict_proba(self) -> bool:
         return True
 
-    def get_classes(self) -> list:
-        return list(self.class_mapping.values())
-
-    def get_class_mapping(self) -> dict:
-        return self.class_mapping
+    def can_fit_with_example_weights(self) -> bool:
+        return False
 
     def get_compatible_encoders(self):
         from immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder import SequenceAbundanceEncoder
         from immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder import CompAIRRSequenceAbundanceEncoder
         from immuneML.encodings.abundance_encoding.KmerAbundanceEncoder import KmerAbundanceEncoder
         return [SequenceAbundanceEncoder, CompAIRRSequenceAbundanceEncoder, KmerAbundanceEncoder]
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/RandomForestClassifier.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/RandomForestClassifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 
     Note: if you are interested in plotting the coefficients of the random forest classifier model,
     consider running the :ref:`Coefficients` report.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_random_forest_classifier: # user-defined method name
-            RandomForestClassifier: # name of the ML method
-                # sklearn parameters (same names as in original sklearn class)
-                random_state: 100 # always use this value for random state
-                n_estimators: [10, 50, 100] # find the optimal number of trees in the forest
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under RandomForestClassifier is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_random_forest: RandomForestClassifier
+        definitions:
+            ml_methods:
+                my_random_forest_classifier: # user-defined method name
+                    RandomForestClassifier: # name of the ML method
+                        # sklearn parameters (same names as in original sklearn class)
+                        random_state: 100 # always use this value for random state
+                        n_estimators: [10, 50, 100] # find the optimal number of trees in the forest
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under RandomForestClassifier is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_random_forest: RandomForestClassifier
 
     """
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         parameters = parameters if parameters is not None else {}
 
         if parameter_grid is not None:
@@ -52,14 +54,17 @@
         params = self._parameters.copy()
         params["n_jobs"] = cores_for_training
         return RFC(**params)
 
     def can_predict_proba(self) -> bool:
         return True
 
+    def can_fit_with_example_weights(self) -> bool:
+        return True
+
     def get_params(self):
         params = self.model.get_params(deep=True)
         params["feature_importances"] = self.model.feature_importances_.tolist()
         return params
 
     @staticmethod
     def get_documentation():
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/ReceptorCNN.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/ReceptorCNN.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     Notes:
 
     - ReceptorCNN can only be used with ReceptorDatasets, it does not work with SequenceDatasets
 
     - ReceptorCNN can only be used for binary classification, not multi-class classification.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - kernel_count (count): number of kernels that will look for motifs for one chain
 
     - kernel_size (list): sizes of the kernels = how many amino acids to consider at the same time in the chain sequence, can be a tuple of values; e.g. for value [3, 4] of kernel_size, kernel_count*len(kernel_size) kernels will be created, with kernel_count kernels of size 3 and kernel_count kernels of size 4 per chain
 
     - positional_channels (int): how many positional channels where included in one-hot encoding of the receptor sequences (:ref:`OneHot` encoder adds 3 positional channels positional information is enabled)
 
@@ -66,41 +66,42 @@
 
     - training_percentage (float): what percentage of data to use for training (the rest will be used for validation); values between 0 and 1
 
     - evaluate_at (int): when to evaluate the model, e.g. every 100 iterations
 
     - background_probabilities: used for rescaling the kernel values to produce information gain matrix; represents the background probability of each amino acid (without positional information); if not specified, uniform background is assumed
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_receptor_cnn:
-            ReceptorCNN:
-                kernel_count: 5
-                kernel_size: [3]
-                positional_channels: 3
-                sequence_type: amino_acid
-                device: cpu
-                number_of_threads: 16
-                random_seed: 100
-                learning_rate: 0.01
-                iteration_count: 10000
-                l1_weight_decay: 0
-                l2_weight_decay: 0
-                batch_size: 5000
+        definitions:
+            ml_methods:
+                my_receptor_cnn:
+                    ReceptorCNN:
+                        kernel_count: 5
+                        kernel_size: [3]
+                        positional_channels: 3
+                        sequence_type: amino_acid
+                        device: cpu
+                        number_of_threads: 16
+                        random_seed: 100
+                        learning_rate: 0.01
+                        iteration_count: 10000
+                        l1_weight_decay: 0
+                        l2_weight_decay: 0
+                        batch_size: 5000
 
     """
 
     def __init__(self, kernel_count: int = None, kernel_size=None, positional_channels: int = None, sequence_type: str = None, device=None,
                  number_of_threads: int = None, random_seed: int = None, learning_rate: float = None, iteration_count: int = None,
                  l1_weight_decay: float = None, l2_weight_decay: float = None, batch_size: int = None, training_percentage: float = None,
-                 evaluate_at: int = None, background_probabilities=None, result_path: Path = None):
-
+                 evaluate_at: int = None, background_probabilities=None):
         super().__init__()
         self.kernel_count = kernel_count
         self.kernel_size = kernel_size
         self.positional_channels = positional_channels
         self.number_of_threads = number_of_threads
         self.random_seed = random_seed
         self.device = device
@@ -111,64 +112,51 @@
         self.batch_size = batch_size
         self.evaluate_at = evaluate_at
         self.training_percentage = training_percentage
         self.sequence_type = None if sequence_type is None else SequenceType[sequence_type.upper()]
 
         self.background_probabilities = None
         self.CNN = None
-        self.label = None
-        self.class_mapping = None
-        self.result_path = result_path
         self.chain_names = None
-        self.feature_names = None
 
-    def predict(self, encoded_data: EncodedData, label: Label):
-        predictions_proba = self.predict_proba(encoded_data, label)[label.name][label.positive_class]
-        return {label.name: [self.class_mapping[val] for val in (predictions_proba > 0.5).tolist()]}
+    def _predict(self, encoded_data: EncodedData):
+        predictions_proba = self._predict_proba(encoded_data)[self.label.name][self.label.positive_class]
+        return {self.label.name: [self.class_mapping[val] for val in (predictions_proba > 0.5).tolist()]}
 
     def set_background_probabilities(self):
         self.background_probabilities = np.array([1. / len(EnvironmentSettings.get_sequence_alphabet(self.sequence_type))
                            for i in range(len(EnvironmentSettings.get_sequence_alphabet(self.sequence_type)))])
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         # set the model to evaluation mode for inference
         self.CNN.eval()
 
         # convert encoded data from numpy arrays to tensors
         encoded_data_pt = self._make_encoded_data(encoded_data, np.arange(len(encoded_data.example_ids)))
 
         # make predictions
         with torch.no_grad():
             predictions = []
-            for examples, labels, example_ids in self._get_data_batch(encoded_data_pt, label.name):
+            for examples, labels, example_ids in self._get_data_batch(encoded_data_pt, self.label.name):
                 logit_outputs = self.CNN(examples)
                 prediction = torch.sigmoid(logit_outputs)
                 predictions.extend(prediction.numpy())
 
         return {self.label.name: {self.label.positive_class: np.array(predictions),
                                   self.label.get_binary_negative_class(): 1 - np.array(predictions)}}
 
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-        if encoded_data.example_weights is not None:
-            warnings.warn(f"{self.__class__.__name__}: cannot fit this classifier with example weights, fitting without example weights instead... Example weights will still be applied when computing evaluation metrics after fitting.")
-
-        self.feature_names = encoded_data.feature_names
-
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
         Util.setup_pytorch(self.number_of_threads, self.random_seed)
         if "chain_names" in encoded_data.info and encoded_data.info["chain_names"] is not None and len(encoded_data.info["chain_names"]) == 2:
             self.chain_names = encoded_data.info["chain_names"]
         else:
             self.chain_names = ["chain_1", "chain_2"]
 
         self._make_CNN()
         self.CNN.to(device=self.device)
-
-        self.label = label
-        self.class_mapping = Util.make_binary_class_mapping(encoded_data.labels[self.label.name], self.label.positive_class)
-
         self.CNN.train()
 
         iteration = 0
         loss_function = nn.BCEWithLogitsLoss().to(device=self.device)
         optimizer = torch.optim.Adam(self.CNN.parameters(), lr=self.learning_rate, weight_decay=self.l2_weight_decay, eps=1e-4)
         state = dict(model=copy.deepcopy(self.CNN).state_dict(), optimizer=optimizer, iteration=iteration, best_validation_loss=np.inf)
         train_data, validation_data = self._prepare_and_split_data(encoded_data)
@@ -201,19 +189,14 @@
 
                 if iteration >= self.iteration_count:
                     self.CNN.load_state_dict(state["model"])
                     break
 
         logging.info("ReceptorCNN: finished training.")
 
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric: str = None,
-                                number_of_splits: int = 5, cores_for_training: int = -1):
-        logging.warning(f"{ReceptorCNN.__name__}: cross_validation is not implemented for this method. Using standard fitting instead...")
-        self.fit(encoded_data=encoded_data, label=label)
-
     def _get_data_batch(self, encoded_data: EncodedData, label_name: str):
         batch_count = int(math.ceil(len(encoded_data.example_ids) / self.batch_size))
         for i in range(batch_count):
             start_index, end_index = int(self.batch_size * i), int(self.batch_size * (i + 1))
             yield encoded_data.examples[start_index: end_index], encoded_data.labels[label_name][start_index: end_index], \
                   encoded_data.example_ids[start_index: end_index]
 
@@ -262,15 +245,15 @@
             with torch.no_grad():
                 for examples, labels, example_ids in self._get_data_batch(data, self.label.name):
                     logit_outputs = self.CNN(examples)
                     loss += loss_func(logit_outputs, labels) / len(data.example_ids)
 
         return loss
 
-    def store(self, path: Path, feature_names=None, details_path: Path = None):
+    def store(self, path: Path):
         PathBuilder.build(path)
 
         torch.save(copy.deepcopy(self.CNN).state_dict(), str(path / "CNN.pt"))
 
         custom_vars = copy.deepcopy(vars(self))
         del custom_vars["CNN"]
         del custom_vars["result_path"]
@@ -307,36 +290,24 @@
     def _make_CNN(self):
         if self.background_probabilities is None:
             self.set_background_probabilities()
 
         self.CNN = RCNN(kernel_count=self.kernel_count, kernel_size=self.kernel_size, positional_channels=self.positional_channels,
                         sequence_type=self.sequence_type, background_probabilities=self.background_probabilities, chain_names=self.chain_names)
 
-    def check_if_exists(self, path):
-        return self.CNN is not None
-
     def get_params(self):
         params = copy.deepcopy(vars(self))
         params["CNN"] = copy.deepcopy(self.CNN).state_dict()
         return params
 
-    def get_label_name(self):
-        return self.label.name
-
-    def get_package_info(self) -> str:
-        return Util.get_immuneML_version()
-
-    def get_feature_names(self) -> list:
-        return self.feature_names
-
     def can_predict_proba(self) -> bool:
         return True
 
-    def get_class_mapping(self) -> dict:
-        return self.class_mapping
+    def can_fit_with_example_weights(self) -> bool:
+        return False
 
     def get_compatible_encoders(self):
         from immuneML.encodings.onehot.OneHotEncoder import OneHotEncoder
         return [OneHotEncoder]
 
     def check_encoder_compatibility(self, encoder):
         """Checks whether the given encoder is compatible with this ML method, and throws an error if it is not."""
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SVC.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SVC.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,32 +12,34 @@
 
     Note: if you are interested in plotting the coefficients of the SVC model,
     consider running the :ref:`Coefficients` report.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_svc: # user-defined method name
-            SVC: # name of the ML method
-                # sklearn parameters (same names as in original sklearn class)
-                C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under SVC is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_svc: SVC
+        definitions:
+            ml_methods:
+                my_svc: # user-defined method name
+                    SVC: # name of the ML method
+                        # sklearn parameters (same names as in original sklearn class)
+                        C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under SVC is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_svc: SVC
 
     """
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         _parameter_grid = parameter_grid if parameter_grid is not None else {}
         _parameters = parameters if parameters is not None else {}
 
@@ -45,14 +47,17 @@
 
     def _get_ml_model(self, cores_for_training: int = 2, X=None):
         return SklearnSVC(**self._parameters)
 
     def can_predict_proba(self) -> bool:
         return False
 
+    def can_fit_with_example_weights(self) -> bool:
+        return True
+
     def get_params(self):
         params = self.model.get_params()
         params["coefficients"] = self.model.coef_[0].tolist()
         params["intercept"] = self.model.intercept_.tolist()
         return params
 
     @staticmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SVM.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SVM.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,35 @@
 
     Note: if you are interested in plotting the coefficients of the SVM model,
     consider running the :ref:`Coefficients` report.
 
     For usage instructions, check :py:obj:`~immuneML.ml_methods.classifiers.SklearnMethod.SklearnMethod`.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_svm: # user-defined method name
-            SVM: # name of the ML method
-                # sklearn parameters (same names as in original sklearn class)
-                C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
-                kernel: linear
-                # Additional parameter that determines whether to print convergence warnings
-                show_warnings: True
-            # if any of the parameters under SVM is a list and model_selection_cv is True,
-            # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-            # and the optimal model will be selected
-            model_selection_cv: True
-            model_selection_n_folds: 5
-        # alternative way to define ML method with default values:
-        my_default_svm: SVM
+        definitions:
+            ml_methods:
+                my_svm: # user-defined method name
+                    SVM: # name of the ML method
+                        # sklearn parameters (same names as in original sklearn class)
+                        C: [0.01, 0.1, 1, 10, 100] # find the optimal value for C
+                        kernel: linear
+                        # Additional parameter that determines whether to print convergence warnings
+                        show_warnings: True
+                    # if any of the parameters under SVM is a list and model_selection_cv is True,
+                    # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                    # and the optimal model will be selected
+                    model_selection_cv: True
+                    model_selection_n_folds: 5
+                # alternative way to define ML method with default values:
+                my_default_svm: SVM
 
     """
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
         _parameter_grid = parameter_grid if parameter_grid is not None else {}
         _parameters = parameters if parameters is not None else {}
 
@@ -46,14 +48,17 @@
 
     def _get_ml_model(self, cores_for_training: int = 2, X=None):
         return SVC(**self._parameters)
 
     def can_predict_proba(self) -> bool:
         return False
 
+    def can_fit_with_example_weights(self) -> bool:
+        return False
+
     def get_params(self):
         params = self.model.get_params()
         params["coefficients"] = self.model.coef_[0].tolist() if self.model.kernel == 'linear' else self.model.dual_coef_.toarray().tolist() if hasattr(self.model.dual_coef_, "toarray") else self.model.dual_coef_.tolist()
         params["intercept"] = self.model.intercept_.tolist()
         return params
 
     @staticmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/SklearnMethod.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/SklearnMethod.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,48 +27,50 @@
     ML methods from scikit-learn have to implement:
         - the __init__() method,
         - get_params(label) and
         - _get_ml_model()
     Other methods can also be overwritten if needed.
     The arguments and specification described bellow applied for all classes inheriting SklearnMethod.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - parameters: a dictionary of parameters that will be directly passed to scikit-learn's class upon calling __init__()
       method; for detailed list see scikit-learn's documentation of the specific class inheriting SklearnMethod
 
     - parameter_grid: a dictionary of parameters which all have to be valid arguments for scikit-learn's corresponding class' __init__() method
       (same as parameters), but unlike parameters argument can contain list of values instead of one value; if this is specified and
       "model_selection_cv" is True (in the specification) or just if fit_by_cross_validation() is called, a grid search will be performed over
       these parameters and the optimal model will be kept
 
 
-    YAML specification:
+    **YAML specification:**
 
-        ml_methods:
-            log_reg:
-                LogisticRegression: # name of the class inheriting SklearnMethod
-                    # sklearn parameters (same names as in original sklearn class)
-                    max_iter: 1000 # specific parameter value
-                    penalty: l1
-                    # Additional parameter that determines whether to print convergence warnings
-                    show_warnings: True
-                # if any of the parameters under LogisticRegression is a list and model_selection_cv is True,
-                # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
-                # and the optimal model will be selected
-                model_selection_cv: True
-                model_selection_n_folds: 5
-            svm_with_cv:
-                SVM: # name of another class inheriting SklearnMethod
-                    # sklearn parameters (same names as in original sklearn class)
-                    alpha: 10
-                    # Additional parameter that determines whether to print convergence warnings
-                    show_warnings: True
-                # no grid search will be done
-                model_selection_cv: False
+        definitions:
+            ml_methods:
+                ml_methods:
+                    log_reg:
+                        LogisticRegression: # name of the class inheriting SklearnMethod
+                            # sklearn parameters (same names as in original sklearn class)
+                            max_iter: 1000 # specific parameter value
+                            penalty: l1
+                            # Additional parameter that determines whether to print convergence warnings
+                            show_warnings: True
+                        # if any of the parameters under LogisticRegression is a list and model_selection_cv is True,
+                        # a grid search will be done over the given parameters, using the number of folds specified in model_selection_n_folds,
+                        # and the optimal model will be selected
+                        model_selection_cv: True
+                        model_selection_n_folds: 5
+                    svm_with_cv:
+                        SVM: # name of another class inheriting SklearnMethod
+                            # sklearn parameters (same names as in original sklearn class)
+                            alpha: 10
+                            # Additional parameter that determines whether to print convergence warnings
+                            show_warnings: True
+                        # no grid search will be done
+                        model_selection_cv: False
 
     """
 
     FIT_CV = "fit_CV"
     FIT = "fit"
 
     def __init__(self, parameter_grid: dict = None, parameters: dict = None):
@@ -80,51 +82,43 @@
         elif parameters is not None and "show_warnings" in parameters:
             self.show_warnings = parameters.pop("show_warnings")
         else:
             self.show_warnings = True
 
         self._parameter_grid = parameter_grid
         self._parameters = parameters
-        self.feature_names = None
-        self.class_mapping = None
-        self.label = None
-
-    def fit(self, encoded_data: EncodedData, label: Label, optimization_metric=None, cores_for_training: int = 2):
-
-        self.label = label
-        self.class_mapping = Util.make_class_mapping(encoded_data.labels[self.label.name], self.label.positive_class)
-        self.feature_names = encoded_data.feature_names
 
+    def _fit(self, encoded_data: EncodedData, cores_for_training: int = 2):
         mapped_y = Util.map_to_new_class_values(encoded_data.labels[self.label.name], self.class_mapping)
 
-        self.model = self._fit(encoded_data.examples, mapped_y, encoded_data.example_weights, cores_for_training)
+        self.model = self._fit_model(encoded_data.examples, mapped_y, encoded_data.example_weights, cores_for_training)
 
-    def predict(self, encoded_data: EncodedData, label: Label):
-        self.check_is_fitted(label.name)
+    def _predict(self, encoded_data: EncodedData):
+        self.check_is_fitted(self.label.name)
 
         predictions = self.apply_with_weights(self.model.predict,
                                               encoded_data.example_weights,
                                               X=encoded_data.examples)
 
-        return {label.name: Util.map_to_old_class_values(np.array(predictions), self.class_mapping)}
+        return {self.label.name: Util.map_to_old_class_values(np.array(predictions), self.class_mapping)}
 
-    def predict_proba(self, encoded_data: EncodedData, label: Label):
+    def _predict_proba(self, encoded_data: EncodedData):
         if self.can_predict_proba():
             probabilities = self.apply_with_weights(self.model.predict_proba, encoded_data.example_weights, X=encoded_data.examples)
             class_names = Util.map_to_old_class_values(self.model.classes_, self.class_mapping)
 
-            return {label.name: {class_name: probabilities[:, i] for i, class_name in enumerate(class_names)}}
+            return {self.label.name: {class_name: probabilities[:, i] for i, class_name in enumerate(class_names)}}
         else:
             warnings.warn(f"{self.__class__.__name__}: cannot predict probabilities.")
             return None
 
-    def _fit(self, X, y, w=None, cores_for_training: int = 1):
+    def _fit_model(self, X, y, w=None, cores_for_training: int = 1):
         self.model = self._get_ml_model(cores_for_training, X)
 
-        if w is not None and not self.supports_example_weight(self.model.fit) and not self.supports_example_weight(self.model.predict):
+        if w is not None and not self._check_method_supports_example_weight(self.model.fit) and not self._check_method_supports_example_weight(self.model.predict):
             warnings.warn(f"{self.__class__.__name__}: cannot fit this classifier with example weights, fitting without example weights instead... Example weights will still be applied when computing evaluation metrics after fitting.")
 
         if not self.show_warnings:
             warnings.simplefilter("ignore")
             os.environ["PYTHONWARNINGS"] = "ignore"
 
         self.model = self._get_ml_model(cores_for_training, X)
@@ -139,51 +133,45 @@
     def apply_with_weights(self, method, weights, **kwargs):
         '''
         Can be used to run self.model.fit, self.model.predict or self.model.predict_proba with sample weights if supported
 
         :param method: self.model.fit, self.model.predict or self.model.predict_proba
         :return: the result of the supplied method
         '''
-        if weights is not None and self.supports_example_weight(method):
+        if weights is not None and self._check_method_supports_example_weight(method):
             return method(**kwargs, sample_weight=weights)
         else:
             return method(**kwargs)
 
-    def supports_example_weight(self, method):
+    def _check_method_supports_example_weight(self, method):
         return "sample_weight" in inspect.signature(method).parameters
 
     def can_predict_proba(self) -> bool:
         return False
 
     def check_is_fitted(self, label_name: str):
         if self.label.name == label_name or label_name is None:
-            return check_is_fitted(self.model, ["estimators_", "coef_", "estimator", "_fit_X", "dual_coef_"], all_or_any=any)
+            return check_is_fitted(self.model, ["estimators_", "coef_", "estimator", "_fit_X", "dual_coef_", "classes_"], all_or_any=any)
 
-    def fit_by_cross_validation(self, encoded_data: EncodedData, label: Label = None, optimization_metric="balanced_accuracy",
-                                number_of_splits: int = 5, cores_for_training: int = -1):
+    def _fit_by_cross_validation(self, encoded_data: EncodedData, number_of_splits: int, cores_for_training: int):
 
-        self.class_mapping = Util.make_class_mapping(encoded_data.labels[label.name], label.positive_class)
-        self.feature_names = encoded_data.feature_names
-        self.label = label
         mapped_y = Util.map_to_new_class_values(encoded_data.labels[self.label.name], self.class_mapping)
 
-        self.model = self._fit_by_cross_validation(X=encoded_data.examples, y=mapped_y, w=encoded_data.example_weights,
-                                                   label=label, optimization_metric=optimization_metric,
-                                                   number_of_splits=number_of_splits, cores_for_training=cores_for_training)
+        self.model = self._fit_model_by_cross_validation(X=encoded_data.examples, y=mapped_y, w=encoded_data.example_weights,
+                                                         number_of_splits=number_of_splits, cores_for_training=cores_for_training)
 
-    def _fit_by_cross_validation(self, X, y, w, label: Label = None, optimization_metric: str = "balanced_accuracy",
-                                 number_of_splits: int = 5, cores_for_training: int = 1):
+    def _fit_model_by_cross_validation(self, X, y, w, number_of_splits: int, cores_for_training: int):
 
         model = self._get_ml_model()
-        scoring = ClassificationMetric.get_sklearn_score_name(ClassificationMetric.get_metric(optimization_metric.upper()))
+        scoring = ClassificationMetric.get_sklearn_score_name(ClassificationMetric.get_metric(self.optimization_metric))
 
         if scoring not in get_scorer_names():
             scoring = "balanced_accuracy"
             warnings.warn(
-                f"{self.__class__.__name__}: specified optimization metric ({optimization_metric}) is not defined as a sklearn scoring function, using {scoring} instead... ")
+                f"{self.__class__.__name__}: specified optimization metric ({self.optimization_metric}) is not defined as a sklearn scoring function, using {scoring} instead... ")
 
         if not self.show_warnings:
             warnings.simplefilter("ignore")
             os.environ["PYTHONWARNINGS"] = "ignore"
 
         self.model = RandomizedSearchCV(model, param_distributions=self._parameter_grid, cv=number_of_splits, n_jobs=cores_for_training,
                                         scoring=scoring, refit=True)
@@ -194,90 +182,70 @@
             del os.environ["PYTHONWARNINGS"]
             warnings.simplefilter("always")
 
         self.model = self.model.best_estimator_  # do not leave RandomSearchCV object to be in models, use the best estimator instead
 
         return self.model
 
-    def store(self, path: Path, feature_names=None, details_path: Path = None):
+    def store(self, path: Path):
         PathBuilder.build(path)
         file_path = path / f"{self._get_model_filename()}.pickle"
         with file_path.open("wb") as file:
             dill.dump(self.model, file)
 
-        if details_path is None:
-            params_path = path / f"{self._get_model_filename()}.yaml"
-        else:
-            params_path = details_path
+        params_path = path / f"{self._get_model_filename()}.yaml"
 
         with params_path.open("w") as file:
             desc = {
                 **(self.get_params()),
-                "feature_names": feature_names,
+                "feature_names": self.get_feature_names(),
                 "classes": self.model.classes_.tolist(),
                 "class_mapping": self.class_mapping,
             }
 
             if self.label is not None:
                 desc["label"] = self.label.get_desc_for_storage()
 
             yaml.dump(desc, file)
 
     def _get_model_filename(self):
         return FilenameHandler.get_filename(self.__class__.__name__, "")
 
-    def load(self, path: Path, details_path: Path = None):
+    def load(self, path: Path):
         name = f"{self._get_model_filename()}.pickle"
         file_path = path / name
         if file_path.is_file():
             with file_path.open("rb") as file:
                 self.model = dill.load(file)
         else:
             raise FileNotFoundError(f"{self.__class__.__name__} model could not be loaded from {file_path}"
                                     f". Check if the path to the {name} file is properly set.")
 
-        if details_path is None:
-            params_path = path / f"{self._get_model_filename()}.yaml"
-        else:
-            params_path = details_path
+        params_path = path / f"{self._get_model_filename()}.yaml"
 
         if params_path.is_file():
             with params_path.open("r") as file:
                 desc = yaml.safe_load(file)
                 if "label" in desc:
                     setattr(self, "label", Label(**desc["label"]))
                 for param in ["feature_names", "classes", "class_mapping"]:
                     if param in desc:
                         setattr(self, param, desc[param])
 
-    def check_if_exists(self, path: Path):
-        file_path = path / f"{self._get_model_filename()}.pickle"
-        return file_path.is_file()
-
     @abc.abstractmethod
     def _get_ml_model(self, cores_for_training: int = 2, X=None):
         pass
 
     @abc.abstractmethod
     def get_params(self):
         """Returns the model parameters in a readable yaml-friendly way (consisting of lists, dictionaries and strings)."""
         pass
 
-    def get_label_name(self):
-        return self.label.name
-
     def get_package_info(self) -> str:
-        return 'scikit-learn ' + pkg_resources.get_distribution('scikit-learn').version
-
-    def get_feature_names(self) -> list:
-        return self.feature_names
-
-    def get_class_mapping(self) -> dict:
-        """Returns a dictionary containing the mapping between label values and values internally used in the classifier"""
-        return self.class_mapping
+        return Util.get_immuneML_version() + '; scikit-learn ' + pkg_resources.get_distribution('scikit-learn').version
 
     def get_compatible_encoders(self):
         from immuneML.encodings.evenness_profile.EvennessProfileEncoder import EvennessProfileEncoder
         from immuneML.encodings.kmer_frequency.KmerFrequencyEncoder import KmerFrequencyEncoder
         from immuneML.encodings.onehot.OneHotEncoder import OneHotEncoder
         from immuneML.encodings.word2vec.Word2VecEncoder import Word2VecEncoder
         from immuneML.encodings.reference_encoding.MatchedSequencesEncoder import MatchedSequencesEncoder
@@ -300,15 +268,15 @@
     2. Passing a range of different hyperparameters to {model_name}, and using a third layer of nested cross-validation 
     to find the optimal hyperparameters through grid search. In this case, only the {model_name} model with the optimal 
     hyperparameter settings is further used in the inner selection loop of the TrainMLModel instruction. 
     
     By default, mode 1 is used. In order to use mode 2, model_selection_cv and model_selection_n_folds must be set. 
     
     
-    Specification arguments:
+    **Specification arguments:**
 
     - {model_name} (dict): Under this key, hyperparameters can be specified that will be passed to the scikit-learn class.
       Any scikit-learn hyperparameters can be specified here. In mode 1, a single value must be specified for each of the scikit-learn
       hyperparameters. In mode 2, it is possible to specify a range of different hyperparameters values in a list. It is also allowed
       to mix lists and single values in mode 2, in which case the grid search will only be done for the lists, while the
       single-value hyperparameters will be fixed. 
       In addition to the scikit-learn hyperparameters, parameter show_warnings (True/False) can be specified here. This determines
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/classifiers/TCRdistClassifier.py` & `immuneml-3.0.0a4/immuneML/ml_methods/classifiers/TCRdistClassifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,35 +12,36 @@
     Implementation of a nearest neighbors classifier based on TCR distances as presented in
     Dash P, Fiore-Gartland AJ, Hertz T, et al. Quantifiable predictive features define epitope-specific T cell receptor repertoires.
     Nature. 2017; 547(7661):89-93. `doi:10.1038/nature22383 <https://www.nature.com/articles/nature22383>`_.
 
     This method is implemented using scikit-learn's KNeighborsClassifier with k determined at runtime from the training dataset size and weights
     linearly scaled to decrease with the distance of examples.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - percentage (float): percentage of nearest neighbors to consider when determining receptor specificity based on known receptors (between 0 and 1)
 
     - show_warnings (bool): whether to show warnings generated by scikit-learn, by default this is True.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_tcr_method:
-            TCRdistClassifier:
-                percentage: 0.1
-                show_warnings: True
+        definitions:
+            ml_methods:
+                my_tcr_method:
+                    TCRdistClassifier:
+                        percentage: 0.1
+                        show_warnings: True
 
     """
 
     def __init__(self, percentage: float, show_warnings: bool = True):
         super().__init__()
-
         ParameterValidator.assert_type_and_value(percentage, float, "TCRdistClassifier", "percentage", min_inclusive=0., max_inclusive=1.)
 
         self.percentage = percentage
         self.k = None
         self.show_warnings = show_warnings
 
     def _get_ml_model(self, cores_for_training: int = 2, X=None):
@@ -60,13 +61,16 @@
 
     def get_params(self):
         return {**self.model.get_params(deep=True), **copy.deepcopy(vars(self))}
 
     def can_predict_proba(self) -> bool:
         return True
 
+    def can_fit_with_example_weights(self) -> bool:
+        return False
+
     def _get_model_filename(self):
         return "tcrdist_classifier"
 
     def get_compatible_encoders(self):
         from immuneML.encodings.distance_encoding.TCRdistEncoder import TCRdistEncoder
         return [TCRdistEncoder]
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/PCA.py` & `immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/PCA.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-import scipy
 from sklearn.decomposition import PCA as SklearnPCA
 
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.ml_methods.dim_reduction.DimRedMethod import DimRedMethod
 
 
 class PCA(DimRedMethod):
     """
     Principal component analysis (PCA) method which wraps scikit-learn's PCA. Input arguments for the method are the
     same as supported by scikit-learn (see `PCA scikit-learn documentation
     <https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html#sklearn.decomposition.PCA>`_ for details).
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_pca: # user-defined name of the dimensionality reduction method
-            PCA: # name of the class
-                # arguments as defined by scikit-learn
-                n_components: 2
+        definitions:
+            ml_methods:
+                my_pca:
+                    PCA:
+                        # arguments as defined by scikit-learn
+                        n_components: 2
 
     """
 
     def __init__(self, name: str = None, **kwargs):
         super().__init__(name)
         self.method_kwargs = kwargs
         self.method = SklearnPCA(**self.method_kwargs)
@@ -31,11 +32,8 @@
     def fit(self, dataset: Dataset):
         self.method.fit(dataset.encoded_data.examples)
 
     def transform(self, dataset: Dataset):
         return self.method.transform(dataset.encoded_data.examples)
 
     def fit_transform(self, dataset: Dataset):
-        data = dataset.encoded_data.examples.toarray() if scipy.sparse.issparse(dataset.encoded_data.examples) \
-            else dataset.encoded_data.examples
-
-        return self.method.fit_transform(data)
+        return self.method.fit_transform(dataset.encoded_data.get_examples_as_np_matrix())
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/TSNE.py` & `immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/TSNE.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 class TSNE(DimRedMethod):
     """
     t-distributed Stochastic Neighbor Embedding (t-SNE) method which wraps scikit-learn's TSNE. It can be useful for
     visualizing high-dimensional data. Input arguments for the method are the
     same as supported by scikit-learn (see `TSNE scikit-learn documentation
     <https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html#sklearn.manifold.TSNE>`_ for details).
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_tsne: # user-defined name of the dimensionality reduction method
-            TSNE: # name of the class
-                # arguments as defined by scikit-learn
-                n_components: 2
-                init: pca
+        definitions:
+            ml_methods:
+                my_tsne:
+                    TSNE:
+                        # arguments as defined by scikit-learn
+                        n_components: 2
+                        init: pca
 
     """
     def __init__(self, name: str = None, **kwargs):
         super().__init__(name)
         self.method_kwargs = kwargs
         self.method = SklearnTSNE(**self.method_kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/dim_reduction/UMAP.py` & `immuneml-3.0.0a4/immuneML/ml_methods/dim_reduction/UMAP.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,27 @@
     same as supported by umap-learn (see `UMAP in the umap-learn documentation
     <https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html#sklearn.decomposition.PCA>`_ for details).
 
     Note that when providing the arguments for UMAP in the immuneML's specification, it is not possible to set
     functions as input values (e.g., for the metric parameter, it has to be one of the predefined metrics available
     in umap-learn).
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_umap: # user-defined name of the dimensionality reduction method
-            UMAP: # name of the class
-                n_components: 2
-                n_neighbors: 15
-                metric: euclidean
+        definitions:
+            ml_methods:
+                my_umap:
+                    UMAP:
+                        # arguments as defined by scikit-learn
+                        n_components: 2
+                        n_neighbors: 15
+                        metric: euclidean
 
     """
 
     def __init__(self, name: str = None, **kwargs):
         super().__init__(name)
         self.method_kwargs = kwargs
         self.method = umap.UMAP(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/BackgroundSequences.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/BackgroundSequences.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/ExperimentalImport.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/ExperimentalImport.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class ExperimentalImport(GenerativeModel):
     """
     Allows to import existing experimental data and do annotations and simulations on top of them.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        generative_model:
-            import_format: AIRR
-            tmp_import_path: ./tmp/
-            import_params:
-                path: path/to/files/
-                region_type: IMGT_CDR3 # what part of the sequence to import
-                column_mapping: # column mapping AIRR: immuneML
-                    junction: sequence
-                    junction_aa: sequence_aa
-                    locus: chain
-            type: ExperimentalImport
-
+        definitions:
+            ml_methods:
+                generative_model:
+                    type: ExperimentalImport
+                    import_format: AIRR
+                    tmp_import_path: ./tmp/
+                    import_params:
+                        path: path/to/files/
+                        region_type: IMGT_CDR3 # what part of the sequence to import
+                        column_mapping: # column mapping AIRR: immuneML
+                            junction: sequence
+                            junction_aa: sequence_aa
+                            locus: chain
     """
 
     def __init__(self, dataset: SequenceDataset, original_input_file: Path = None):
         self._dataset = dataset
         self._counter = 0
         self._original_input_file = original_input_file
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/OLGA.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/OLGA.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,36 +43,37 @@
       https://github.com/statbiophys/OLGA for more details.
 
     - Gene names are as provided in OLGA (either in default models or in the user-specified model files). For
       simulation, one should use gene names in the same format.
 
     .. note::
 
-        While this is a generative model, in version 3.0.0a1, it cannot be used in combination with TrainGenModel or
-        ApplyGenModel instruction. If you want to use OLGA for sequence simulation, see :ref:`How to simulate antigen
-        or disease-associated signals in AIRR datasets`.
+        While this is a generative model, in the current version of immuneML it cannot be used in combination with TrainGenModel or
+        ApplyGenModel instruction. If you want to use OLGA for sequence simulation, see :ref:`Dataset simulation with LIgO`.
 `
 
-    Specification arguments:
+    **Specification arguments:**
 
     - model_path (str): if not default model, this parameter should point to a folder where the four OLGA/IGOR format
       files are stored (could also be inferred from some experimental data)
 
     - default_model_name (str): if not using custom models, one of the OLGA default models could be specified here;
       the value should be the same as it would be passed to command line in OLGA: e.g., humanTRB, human IGH
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        generative_model:
-            type: OLGA
-            model_path: None
-            default_model_name: humanTRB
+        definitions:
+            ml_methods:
+                generative_model:
+                    type: OLGA
+                    model_path: None
+                    default_model_name: humanTRB
 
     """
 
     model_path: Path = None
     default_model_name: str = None
     chain: Chain = None
     region_type: RegionType = RegionType.IMGT_JUNCTION
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/PWM.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/PWM.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,43 @@
 from immuneML.environment.SequenceType import SequenceType
 from immuneML.ml_methods.generative_models.GenerativeModel import GenerativeModel
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class PWM(GenerativeModel):
     """
+    .. note::
+
+        This is an experimental feature
+
     This is a baseline implementation of a positional weight matrix. It is estimated from a set of sequences for each
     of the different lengths that appear in the dataset.
 
-    Specification arguments:
 
-    - chain (str): which chain is generated (for now, it is only assigned to the generated sequences) # TODO: fix
+    **Specification arguments:**
+
+    - chain (str): which chain is generated (for now, it is only assigned to the generated sequences)
 
     - sequence_type (str): amino_acid or nucleotide
 
-    - region_type (str): which region type to use (e.g., IMGT_CDR3), this is only assigned to the generated sequences; # TODO: fix
+    - region_type (str): which region type to use (e.g., IMGT_CDR3), this is only assigned to the generated sequences
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_pwm:
-          PWM:
-            chain: beta
-            sequence_type: amino_acid
-            region_type: IMGT_CDR3
+        definitions:
+            ml_methods:
+                my_pwm:
+                    PWM:
+                        chain: beta
+                        sequence_type: amino_acid
+                        region_type: IMGT_CDR3
 
     """
 
     @classmethod
     def load_model(cls, path: Path):
 
         assert path.exists(), f"{cls.__name__}: {path} does not exist."
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SimpleLSTM.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SimpleLSTM.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Similar models have been proposed in:
 
     Akbar, R. et al. (2022). In silico proof of principle of machine learning-based antibody design at unconstrained scale. mAbs, 14(1), 2031482. https://doi.org/10.1080/19420862.2022.2031482
 
     Saka, K. et al. (2021). Antibody design using LSTM based deep generative model from phage display library for affinity maturation. Scientific Reports, 11(1), Article 1. https://doi.org/10.1038/s41598-021-85274-7
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - sequence_type (str): whether the model should work on amino_acid or nucleotide level
 
     - hidden_size (int): how many LSTM cells should exist per layer
 
     - num_layers (int): how many hidden LSTM layers should there be
 
@@ -46,29 +46,32 @@
 
     - learning_rate (float): what learning rate to use for optimization
 
     - batch_size (int): how many examples (sequences) to use for training for one batch
 
     - embed_size (int): the dimension of the sequence embedding
 
-    - temperature (float)
+    - temperature (float): a higher temperature leads to faster yet more unstable learning
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_simple_lstm:
-            sequence_type: amino_acid
-            hidden_size: 50
-            num_layers: 1
-            num_epochs: 5000
-            learning_rate: 0.001
-            batch_size: 100
-            embed_size: 100
+        definitions:
+            ml_methods:
+                my_simple_lstm:
+                    sequence_type: amino_acid
+                    hidden_size: 50
+                    num_layers: 1
+                    num_epochs: 5000
+                    learning_rate: 0.001
+                    batch_size: 100
+                    embed_size: 100
 
 
     """
 
     @classmethod
     def load_model(cls, path: Path):
         assert path.exists(), f"{cls.__name__}: {path} does not exist."
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SimpleVAE.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SimpleVAE.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     References:
 
     Davidsen, K., Olson, B. J., DeWitt, W. S., III, Feng, J., Harkins, E., Bradley, P., & Matsen, F. A., IV. (2019).
     Deep generative models for T cell receptor protein sequences. eLife, 8, e46935. https://doi.org/10.7554/eLife.46935
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - chain (str): which chain the sequence come from, e.g., TRB
 
     - beta (float): VAE hyperparameter that balanced the reconstruction loss and latent dimension regularization
 
     - latent_dim (int): latent dimension of the VAE
 
@@ -74,34 +74,36 @@
     - unique_v_genes (list): list of allowed V genes (this will be automatically filled from the dataset if not provided here manually)
 
     - unique_j_genes (list): list of allowed J genes (this will be automatically filled from the dataset if not provided here manually)
 
     - device (str): name of the device where to train the model (e.g., cpu)
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_vae:
-            SimpleVAE:
-                chain: beta
-                beta: 0.75
-                latent_dim: 20
-                linear_nodes_count: 75
-                num_epochs: 5000
-                batch_size: 10000
-                j_gene_embed_dim: 13
-                v_gene_embed_dim: 30
-                cdr3_embed_dim: 21
-                pretrains: 10
-                warmup_epochs: 20
-                patience: 20
-                device: cpu
+        definitions:
+            ml_methods:
+                my_vae:
+                    SimpleVAE:
+                        chain: beta
+                        beta: 0.75
+                        latent_dim: 20
+                        linear_nodes_count: 75
+                        num_epochs: 5000
+                        batch_size: 10000
+                        j_gene_embed_dim: 13
+                        v_gene_embed_dim: 30
+                        cdr3_embed_dim: 21
+                        pretrains: 10
+                        warmup_epochs: 20
+                        patience: 20
+                        device: cpu
 
     """
 
     @classmethod
     def load_model(cls, path: Path):
         assert path.exists(), f"{cls.__name__}: {path} does not exist."
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/generative_models/SoNNia.py` & `immuneml-3.0.0a4/immuneML/ml_methods/generative_models/SoNNia.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import shutil
 from pathlib import Path
 
 import numpy as np
 from olga import load_model
-from sonia.sequence_generation import SequenceGeneration
-from sonnia.sonnia import SoNNia as InternalSoNNia
 
 from immuneML.data_model.bnp_util import write_yaml, read_yaml
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.data_model.dataset.SequenceDataset import SequenceDataset
 from immuneML.data_model.receptor.RegionType import RegionType
 from immuneML.data_model.receptor.receptor_sequence.Chain import Chain
 from immuneML.data_model.receptor.receptor_sequence.ReceptorSequence import ReceptorSequence
@@ -26,15 +24,15 @@
     It supports SequenceDataset as input, but not RepertoireDataset.
 
     Original publication:
     Isacchini, G., Walczak, A. M., Mora, T., & Nourmohammad, A. (2021). Deep generative selection models of T and B
     cell receptor repertoires with soNNia. Proceedings of the National Academy of Sciences, 118(14), e2023141118.
     https://doi.org/10.1073/pnas.2023141118
 
-    Specification arguments:
+    **Specification arguments:**
 
     - chain (str)
 
     - batch_size (int)
 
     - epochs (int)
 
@@ -44,18 +42,31 @@
 
     - n_gen_seqs (int)
 
     - custom_model_path (str)
 
     - default_model_name (str)
 
+        **YAML specification:**
+
+    .. indent with spaces
+    .. code-block:: yaml
+
+        definitions:
+            ml_methods:
+                my_sonnia_model:
+                    SoNNia:
+                        ...
+
     """
 
     @classmethod
     def load_model(cls, path: Path):
+        from sonnia.sonnia import SoNNia as InternalSoNNia
+
         assert path.exists(), f"{cls.__name__}: {path} does not exist."
 
         model_overview_file = path / 'model_overview.yaml'
 
         for file in [model_overview_file]:
             assert file.exists(), f"{cls.__name__}: {file} is not a file."
 
@@ -82,14 +93,16 @@
         if custom_model_path is None or custom_model_path == '':
             self._model_path = Path(
                 load_model.__file__).parent / f"default_models/{OLGA.DEFAULT_MODEL_FOLDER_MAP[self.default_model_name]}"
         else:
             self._model_path = custom_model_path
 
     def fit(self, dataset: Dataset, path: Path = None):
+        from sonnia.sonnia import SoNNia as InternalSoNNia
+
         print_log(f"{SoNNia.__name__}: fitting a selection model...", True)
 
         data = dataset.get_attributes(['sequence_aa', 'v_call', 'j_call'], as_list=True)
         data_seqs = [[data['sequence_aa'][i], data['v_call'][i], data['j_call'][i]]
                      for i in range(len(data['sequence_aa']))]
 
         self._model = InternalSoNNia(data_seqs=data_seqs,
@@ -105,14 +118,16 @@
 
         print_log(f"{SoNNia.__name__}: selection model fitted.", True)
 
     def is_same(self, model) -> bool:
         raise NotImplementedError
 
     def generate_sequences(self, count: int, seed: int, path: Path, sequence_type: SequenceType, compute_p_gen: bool):
+        from sonia.sequence_generation import SequenceGeneration
+
         gen_model = SequenceGeneration(self._model)
         sequences = gen_model.generate_sequences_post(count)
         return SequenceDataset.build_from_objects(sequences=[ReceptorSequence(sequence_aa=seq[0], sequence=seq[3],
                                                                               metadata=SequenceMetadata(
                                                                                   v_call=seq[1],
                                                                                   j_call=seq[2],
                                                                                   region_type=RegionType.IMGT_JUNCTION.name))
```

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py` & `immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/PyTorchLogisticRegression.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py` & `immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/PyTorchReceptorCNN.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/SimpleLSTMGenerator.py` & `immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/SimpleLSTMGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/pytorch_implementations/SimpleVAEGenerator.py` & `immuneml-3.0.0a4/immuneML/ml_methods/pytorch_implementations/SimpleVAEGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_methods/util/Util.py` & `immuneml-3.0.0a4/immuneML/ml_methods/util/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_metrics/ClassificationMetric.py` & `immuneml-3.0.0a4/immuneML/ml_metrics/ClassificationMetric.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_metrics/ClusteringMetric.py` & `immuneml-3.0.0a4/immuneML/ml_metrics/ClusteringMetric.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_metrics/MetricUtil.py` & `immuneml-3.0.0a4/immuneML/ml_metrics/MetricUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/ml_metrics/ml_metrics.py` & `immuneml-3.0.0a4/immuneML/ml_metrics/ml_metrics.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/ComparisonData.py` & `immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/ComparisonData.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py` & `immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/ComparisonDataBatch.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py` & `immuneml-3.0.0a4/immuneML/pairwise_repertoire_comparison/PairwiseRepertoireComparison.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/Preprocessor.py` & `immuneml-3.0.0a4/immuneML/preprocessing/Preprocessor.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/ReferenceSequenceAnnotator.py` & `immuneml-3.0.0a4/immuneML/preprocessing/ReferenceSequenceAnnotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class ReferenceSequenceAnnotator(Preprocessor):
     """
     Annotates each sequence in each repertoire if it matches any of the reference sequences provided as input parameter. This report uses CompAIRR internally. To match CDR3 sequences (and not JUNCTION), CompAIRR v1.10 or later is needed.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference_sequences (dict): A dictionary describing the reference dataset file. Import should be specified the same way as regular dataset import. It is only allowed to import a receptor dataset here (i.e., is_repertoire is False and paired is True by default, and these are not allowed to be changed).
 
     - max_edit_distance (int): The maximum edit distance between a target sequence (from the repertoire) and the reference sequence.
 
     - compairr_path (str): optional path to the CompAIRR executable. If not given, it is assumed that CompAIRR has been installed such that it can be called directly on the command line with the command 'compairr', or that it is located at /usr/local/bin/compairr.
 
@@ -40,15 +40,15 @@
     - ignore_genes (bool): Whether to ignore V and J gene information. If False, the V and J genes between two receptor chains have to match. If True, gene information is ignored. By default, ignore_genes is False.
 
     - output_column_name (str): in case there are multiple annotations, it is possible here to define the name of the column in the output repertoire files for this specific annotation
 
     - repertoire_batch_size (int): how many repertoires to process simultaneously; depending on the repertoire size, this parameter might be use to limit the memory usage
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - step1:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/SubjectRepertoireCollector.py` & `immuneml-3.0.0a4/immuneML/preprocessing/SubjectRepertoireCollector.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Merges all the Repertoires in a RepertoireDataset that have the same 'subject_id' specified in the metadata. The result
     is a RepertoireDataset with one Repertoire per subject. This preprocessing cannot be used in combination with :ref:`TrainMLModel`
     instruction because it can change the number of examples. To combine the repertoires in this way, use this preprocessing
     with :ref:`DatasetExport` instruction.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter: SubjectRepertoireCollector
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/ChainRepertoireFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/ChainRepertoireFilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,20 +10,20 @@
     Removes all repertoires from the RepertoireDataset object which contain at least one sequence
     with chain different than "keep_chain" parameter.
     Note that this filter filters out repertoires, not individual sequences, and can thus only be applied to RepertoireDatasets.
 
     Since the filter removes repertoires from the dataset (examples in machine learning setting), it cannot be used with :ref:`TrainMLModel`
     instruction. If you want to filter out repertoires including a given chain, see :ref:`DatasetExport` instruction with preprocessing.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - keep_chain (str): Which chain should be kept, valid values are "TRA", "TRB", "IGH", "IGL", "IGK"
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/ClonesPerRepertoireFilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 
 
 class ClonesPerRepertoireFilter(Filter):
     """
     Removes all repertoires from the RepertoireDataset, which contain fewer clonotypes than specified by the
     lower_limit, or more clonotypes than specified by the upper_limit.
     Note that this filter filters out repertoires, not individual sequences, and can thus only be applied to RepertoireDatasets.
+    When no lower or upper limit is specified, or the value -1 is specified, the limit is ignored.
 
     Since the filter removes repertoires from the dataset (examples in machine learning setting), it cannot be used with :ref:`TrainMLModel`
     instruction. If you want to use this filter, see :ref:`DatasetExport` instruction with preprocessing.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - lower_limit (int): The minimal inclusive lower limit for the number of clonotypes allowed in a repertoire.
 
     - upper_limit (int): The maximal inclusive upper limit for the number of clonotypes allowed in a repertoire.
 
-    When no lower or upper limit is specified, or the value -1 is specified, the limit is ignored.
-
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/CountPerSequenceFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/CountPerSequenceFilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 
 
 class CountPerSequenceFilter(Filter):
     """
     Removes all sequences from a Repertoire when they have a count below low_count_limit, or sequences with no count
     value if remove_without_counts is True. This filter can be applied to Repertoires and RepertoireDatasets.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - low_count_limit (int): The inclusive minimal count value in order to retain a given sequence.
 
     - remove_without_count (bool): Whether the sequences without a reported count value should be removed.
 
     - remove_empty_repertoires (bool): Whether repertoires without sequences should be removed.
       Only has an effect when remove_without_count is also set to True. If this is true, this preprocessing cannot be used with :ref:`TrainMLModel`
       instruction, but only with :ref:`DatasetExport` instruction instead.
 
     - batch_size (int): number of repertoires that can be loaded at the same time (only affects the speed when applying this filter on a RepertoireDataset)
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/DuplicateSequenceFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/DuplicateSequenceFilter.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,24 @@
 
     For all other fields (the non-specified sequence type, custom lists, sequence identifier) only the first occurring
     value is kept.
 
     Note that this means the count value of a sequence with a given sequence identifier might not be the same as before
     removing duplicates, unless count_agg = FIRST is used.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - filter_sequence_type (:py:obj:`~immuneML.environment.SequenceType.SequenceType`): Whether the sequences should be collapsed on the nucleotide or amino acid level. Valid options are defined by the SequenceType enum.
 
     - batch_size (int): number of repertoires that can be loaded at the same time (only affects the speed)
 
     - count_agg (:py:obj:`~immuneML.preprocessing.filters.CountAggregationFunction.CountAggregationFunction`): determines how the sequence counts of duplicate sequences are aggregated. Valid options are defined by the CountAggregationFunction enum.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/Filter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/Filter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/MetadataRepertoireFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/MetadataRepertoireFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     Removes repertoires from a RepertoireDataset based on information stored in the metadata_file.
     Note that this filters out repertoires, not individual sequences, and can thus only be applied to RepertoireDatasets.
 
     Since this filter changes the number of repertoires (examples for the machine learning task), it cannot be used with
     :ref:`TrainMLModel` instruction. To filter out repertoires, use preprocessing from the :ref:`DatasetExport` instruction that will create
     a new dataset ready to be used for training machine learning models.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - criteria (dict): a nested dictionary that specifies the criteria for keeping certain columns. See :py:obj:`~immuneML.analysis.criteria_matches.CriteriaMatcher.CriteriaMatcher` for a more detailed explanation.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/preprocessing/filters/SequenceLengthFilter.py` & `immuneml-3.0.0a4/immuneML/preprocessing/filters/SequenceLengthFilter.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class SequenceLengthFilter(Filter):
     """
     Removes sequences with length out of the predefined range.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - sequence_type (:py:obj:`~immuneML.environment.SequenceType.SequenceType`): Whether the sequences should be filtered on the nucleotide or amino acid level. Valid options are defined by the SequenceType enum.
 
     - min_len (int): minimum length of the sequence (sequences shorter than min_len will be removed); to not use min_len, set it to -1
 
     - max_len (int): maximum length of the sequence (sequences longer than max_len will be removed); to not use max_len, set it to -1
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
         preprocessing_sequences:
             my_preprocessing:
                 - my_filter:
```

### Comparing `immuneML-3.0.0a3/immuneML/presentation/PresentationFactory.py` & `immuneml-3.0.0a4/immuneML/presentation/PresentationFactory.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/ClusteringHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/ClusteringHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/DatasetExportHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/DatasetExportHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/ExploratoryAnalysisHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/FeasibilitySummaryHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/FeasibilitySummaryHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/GenModelHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/GenModelHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/HPHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/HPHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/HTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/HTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/LIgOSimulationHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/LIgOSimulationHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/MLApplicationHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/MLApplicationHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/MultiDatasetBenchmarkHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/SubsamplingHTMLBuilder.py` & `immuneml-3.0.0a4/immuneML/presentation/html/SubsamplingHTMLBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/Util.py` & `immuneml-3.0.0a4/immuneML/presentation/html/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/AssessmentSplitDetails.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/AssessmentSplitDetails.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/DatasetExport.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/DatasetExport.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/ExploratoryAnalysis.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/ExploratoryAnalysis.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/FeasibilitySummary.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/FeasibilitySummary.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/GenModel.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/GenModel.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/HPOptimization.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/HPOptimization.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/MLApplication.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/MLApplication.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/MLTraining.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/MLTraining.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/MultiDatasetBenchmark.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/MultiDatasetBenchmark.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/Reports.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/Reports.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/SelectionDetails.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/SelectionDetails.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/Simulation.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/Simulation.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/Subsampling.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/Subsampling.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/css/custom.css` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/css/custom.css`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/presentation/html/templates/index.html` & `immuneml-3.0.0a4/immuneML/presentation/html/templates/index.html`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/reports/PlotlyUtil.py` & `immuneml-3.0.0a4/immuneML/reports/PlotlyUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/reports/Report.py` & `immuneml-3.0.0a4/immuneML/reports/Report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import abc
 import logging
+from pathlib import Path
 
 from immuneML.reports.ReportOutput import ReportOutput
 from immuneML.reports.ReportResult import ReportResult
 
 
 class Report(metaclass=abc.ABCMeta):
     """
     This class defines what report classes should look like: they all have to inherit this class and implement the abstract methods: build_object()
     from parameters and generate() the report once all properties are set (in immuneML this will be taken care of by the instructions). If there are
     any prerequisites needed to run the report (e.g., check if all parameter values are properly set), the check_prerequisites function should be
     overwritten to reflect that and determine if everything is set before generate() is run. See specific functions for more details.
 
     """
 
-    def __init__(self, name: str = None, number_of_processes: int = 1):
+    def __init__(self, name: str = None, result_path: Path = None, number_of_processes: int = 1):
         self.name = name
+        self.result_path = result_path
         self.number_of_processes = number_of_processes
 
     @classmethod
     @abc.abstractmethod
     def build_object(cls, **kwargs):
         """
         Creates the object of the subclass of the Report class from the parameters so that it can be used in the analysis. Depending on the type of
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ReportUtil.py` & `immuneml-3.0.0a4/immuneML/reports/ReportUtil.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/AminoAcidFrequencyDistribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from immuneML.util.PositionHelper import PositionHelper
 
 
 class AminoAcidFrequencyDistribution(DataReport):
     """
     Generates a barplot showing the relative frequency of each amino acid at each position in the sequences of a dataset.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - imgt_positions (bool): Whether to use IMGT positional numbering or sequence index numbering. When imgt_positions
       is True, IMGT positions are used, meaning sequences of unequal length are aligned according to their IMGT
       positions. By default, imgt_positions is True.
 
     - relative_frequency (bool): Whether to plot relative frequencies (true) or absolute counts (false) of the
       positional amino acids. By default, relative_frequency is True.
@@ -38,24 +38,26 @@
     - split_by_label (bool): Whether to split the plots by a label. If set to true, the Dataset must either contain a
       single label, or alternatively the label of interest can be specified under 'label'. If split_by_label is set to
       true, the percentage-wise frequency difference between classes is plotted additionally. By default,
       split_by_label is False.
 
     - label (str): if split_by_label is set to True, a label can be specified here.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_aa_freq_report:
-          AminoAcidFrequencyDistribution:
-            relative_frequency: False
-            split_by_label: True
-            label: CMV
+        definitions:
+            reports:
+                my_aa_freq_report:
+                    AminoAcidFrequencyDistribution:
+                        relative_frequency: False
+                        split_by_label: True
+                        label: CMV
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = AminoAcidFrequencyDistribution.__name__
         ParameterValidator.assert_type_and_value(kwargs["imgt_positions"], bool, location, "imgt_positions")
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/DataReport.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/DataReport.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,23 @@
             type: ExploratoryAnalysis
             analyses:
                 my_first_analysis:
                     report: my_data_report
                     # other parameters...
             # other parameters...
     '''
+    DOCS_TITLE = "Data reports"
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, name: str = None, number_of_processes: int = 1):
         '''
         The arguments defined below are set at runtime by the instruction.
         Concrete classes inheriting DataReport may include additional parameters that will be set by the user in the form of input arguments.
 
         dataset (Dataset): a dataset object (can be repertoire, receptor or sequence dataset, depending on the specific report)
         result_path (Path): location where the results (plots, tables, etc.) will be stored
         name (str): user-defined name of the report used in the HTML overview automatically generated by the platform
         number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
         '''
-        super().__init__(name=name, number_of_processes=number_of_processes)
+        super().__init__(name=name, result_path=result_path, number_of_processes=number_of_processes)
         self.dataset = dataset
-        self.result_path = result_path
 
-    @staticmethod
-    def get_title():
-        return "Data reports"
+
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/GLIPH2Exporter.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/GLIPH2Exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,27 +14,29 @@
     Report which exports the receptor data to GLIPH2 format so that it can be directly used in GLIPH2 tool. Currently, the report accepts only
     receptor datasets.
 
     GLIPH2 publication: Huang H, Wang C, Rubelt F, Scriba TJ, Davis MM. Analyzing the Mycobacterium tuberculosis immune response by T-cell receptor
     clustering with GLIPH2 and genome-wide antigen screening. Nature Biotechnology. Published online April 27,
     2020:1-9. `doi:10.1038/s41587-020-0505-4 <https://www.nature.com/articles/s41587-020-0505-4>`_
 
-    Specification arguments:
+    **Specification arguments:**
 
     - condition (str): name of the parameter present in the receptor metadata in the dataset; condition can be anything which can be processed in
       GLIPH2, such as tissue type or treatment.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_gliph2_exporter: # user-defined name
-            GLIPH2Exporter:
-                condition: epitope # for instance, epitope parameter is present in receptors' metadata with values such as "MtbLys" for Mycobacterium tuberculosis (as shown in the original paper).
+        definitions:
+            reports:
+                my_gliph2_exporter:
+                    GLIPH2Exporter:
+                        condition: epitope # for instance, epitope parameter is present in receptors' metadata with values such as "MtbLys" for Mycobacterium tuberculosis (as shown in the original paper).
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return GLIPH2Exporter(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/MotifGeneralizationAnalysis.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/MotifGeneralizationAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,67 +31,69 @@
     - determine the optimal recall cutoff for motifs of a given size
     - investigate how well motifs learned on a training set generalize to a test set
 
     After running this report and determining the optimal recall cutoffs, the report
     :py:obj:`~immuneML.reports.encoding_reports.MotifTestSetPerformance.MotifTestSetPerformance` can be run to
     plot the performance on an independent test set.
 
-    Arguments:
+    **Specification arguments:**
 
-        label (dict): A label configuration. One label should be specified, and the positive_class for this label should be defined. See the YAML specification below for an example.
+    - label (dict): A label configuration. One label should be specified, and the positive_class for this label should be defined. See the YAML specification below for an example.
 
-        training_set_identifier_path (str): Path to a file containing 'sequence_identifiers' of the sequences used for the training set. This file should have a single column named 'example_id' and have one sequence identifier per line. If training_set_identifier_path is not set, a random subset of the data (according to training_percentage) will be assigned to be the training set.
+    - training_set_identifier_path (str): Path to a file containing 'sequence_identifiers' of the sequences used for the training set. This file should have a single column named 'example_id' and have one sequence identifier per line. If training_set_identifier_path is not set, a random subset of the data (according to training_percentage) will be assigned to be the training set.
 
-        training_percentage (float): If training_set_identifier_path is not set, this value is used to specify the fraction of sequences that will be randomly assigned to form the training set. Should be a value between 0 and 1. By default, training_percentage is 0.7.
+    - training_percentage (float): If training_set_identifier_path is not set, this value is used to specify the fraction of sequences that will be randomly assigned to form the training set. Should be a value between 0 and 1. By default, training_percentage is 0.7.
 
-        random_seed (int): Random seed for splitting the data into training and validation sets a training_set_identifier_path is not provided.
+    - random_seed (int): Random seed for splitting the data into training and validation sets a training_set_identifier_path is not provided.
 
-        split_by_motif_size (bool): Whether to split the analysis per motif size. If true, a recall threshold is learned for each motif size, and figures are generated for each motif size independently. By default, split_by_motif_size is true.
+    - split_by_motif_size (bool): Whether to split the analysis per motif size. If true, a recall threshold is learned for each motif size, and figures are generated for each motif size independently. By default, split_by_motif_size is true.
 
-        min_precision: :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum precision threshold for keeping a motif on the training set. By default, min_precision is 0.9.
+    - min_precision: :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum precision threshold for keeping a motif on the training set. By default, min_precision is 0.9.
 
-        test_precision_threshold (float). The desired precision on the test set, given that motifs are learned by using a training set with a precision threshold of min_precision. It is recommended for test_precision_threshold to be lower than min_precision, e.g., min_precision - 0.1. By default, test_precision_threshold is 0.8.
+    - test_precision_threshold (float). The desired precision on the test set, given that motifs are learned by using a training set with a precision threshold of min_precision. It is recommended for test_precision_threshold to be lower than min_precision, e.g., min_precision - 0.1. By default, test_precision_threshold is 0.8.
 
-        min_recall (float): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum recall threshold for keeping a motif. Any learned recall threshold will be at least as high as the set min_recall value. The default value for min_recall is 0.
+    - min_recall (float): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum recall threshold for keeping a motif. Any learned recall threshold will be at least as high as the set min_recall value. The default value for min_recall is 0.
 
-        min_true_positives (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum number of true positive training sequences that a motif needs to occur in. The default value for min_true_positives is 1.
+    - min_true_positives (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum number of true positive training sequences that a motif needs to occur in. The default value for min_true_positives is 1.
 
-        max_positions (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The maximum motif size. This is number of positional amino acids the motif consists of (excluding gaps). The default value for max_positions is 4.
+    - max_positions (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The maximum motif size. This is number of positional amino acids the motif consists of (excluding gaps). The default value for max_positions is 4.
 
-        min_positions (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum motif size (see also: max_positions). The default value for min_positions is 1.
+    - min_positions (int): :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder` parameter. The minimum motif size (see also: max_positions). The default value for min_positions is 1.
 
-        smoothen_combined_precision (bool): whether to add a smoothed line representing the combined precision to the precision-vs-TP plot. When set to True, this may take considerable extra time to compute. By default, plot_smoothed_combined_precision is set to True.
+    - smoothen_combined_precision (bool): whether to add a smoothed line representing the combined precision to the precision-vs-TP plot. When set to True, this may take considerable extra time to compute. By default, plot_smoothed_combined_precision is set to True.
 
-        min_points_in_window (int): Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing with adaptive window size. This parameter determines the minimum number of points that need to be present in a window to determine the adaptive window size. By default, min_points_in_window is 50.
+    - min_points_in_window (int): Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing with adaptive window size. This parameter determines the minimum number of points that need to be present in a window to determine the adaptive window size. By default, min_points_in_window is 50.
 
-        smoothing_constant1: Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing with adaptive window size. This smoothing constant determines the dependence of the smoothness on the window size. Increasing this increases smoothness for regions where few points are present. By default, smoothing_constant1 is 5.
+    - smoothing_constant1: Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing with adaptive window size. This smoothing constant determines the dependence of the smoothness on the window size. Increasing this increases smoothness for regions where few points are present. By default, smoothing_constant1 is 5.
 
-        smoothing_constant2: Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing. with adaptive window size. This smoothing constant can be used to scale the overall kernel width, thus influencing the smoothness of all regions regardless of data density. By default, smoothing_constant2 is 10.
+    - smoothing_constant2: Parameter for smoothing the combined_precision line in the precision-vs-TP plot through lognormal kernel smoothing. with adaptive window size. This smoothing constant can be used to scale the overall kernel width, thus influencing the smoothness of all regions regardless of data density. By default, smoothing_constant2 is 10.
 
-        training_set_name (str): Name of the training set to be used in figures. By default, the training_set_name is 'training set'.
+    - training_set_name (str): Name of the training set to be used in figures. By default, the training_set_name is 'training set'.
 
-        test_set_name (str): Name of the test set to be used in figures. By default, the test_set_name is 'test set'.
+    - test_set_name (str): Name of the test set to be used in figures. By default, the test_set_name is 'test set'.
 
-        highlight_motifs_path (str): Path to a set of motifs of interest to highlight in the output figures (such as implanted ground-truth motifs). By default, no motifs are highlighted.
+    - highlight_motifs_path (str): Path to a set of motifs of interest to highlight in the output figures (such as implanted ground-truth motifs). By default, no motifs are highlighted.
 
-        highlight_motifs_name (str): IF highlight_motifs_path is defined, this name will be used to label the motifs of interest in the output figures.
+    - highlight_motifs_name (str): IF highlight_motifs_path is defined, this name will be used to label the motifs of interest in the output figures.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-
-        my_report:
-            MotifGeneralizationAnalysis:
-                ...
-                label: # Define a label, and the positive class for that given label
-                    CMV:
-                        positive_class: +
+        definitions:
+            reports:
+                my_motif_generalization:
+                    MotifGeneralizationAnalysis:
+                        min_precision: 0.9
+                        min_recall: 0.1
+                        label: # Define a label, and the positive class for that given label
+                            CMV:
+                                positive_class: +
     """
 
     def __init__(self, training_set_identifier_path: str = None, training_percentage: float = None,
                  max_positions: int = None, min_positions: int = None, min_precision: float = None, min_recall: float = None,
                  min_true_positives: int = None,
                  test_precision_threshold: float = None,
                  split_by_motif_size: bool = None, random_seed: int = None, label: dict = None,
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/ReceptorDatasetOverview.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/ReceptorDatasetOverview.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class ReceptorDatasetOverview(DataReport):
     """
     This report plots the length distribution per chain for a receptor (paired-chain) dataset.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - batch_size (int): how many receptors to load at once; 50 000 by default
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports:
-            my_receptor_overview_report: ReceptorDatasetOverview
+        definitions:
+            reports:
+                my_receptor_overview_report: ReceptorDatasetOverview
 
     """
 
     def __init__(self, batch_size: int, dataset: ReceptorDataset = None, result_path: Path = None, number_of_processes: int = 1, name: str = None):
         super().__init__(dataset=dataset, result_path=result_path, number_of_processes=number_of_processes, name=name)
         self.batch_size = batch_size
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/RecoveredSignificantFeatures.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/RecoveredSignificantFeatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       ground truth implanted signals.
 
     To compare k-mers or sequences of differing lengths, the ground truth sequences or long k-mers are split into k-mers
     of the given size through a sliding window approach. When comparing 'full_sequences' to ground truth sequences, a match
     is only registered if both sequences are of equal length.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - groundtruth_sequences_path (str): Path to a file containing the true implanted (sub)sequences, e.g., full sequences or k-mers.
       The file should contain one sequence per line, without a header, and without V or J genes.
 
     - trim_leading_trailing (bool): Whether to trim the leading and trailing first positions from the provided groundtruth sequences,
       e.g., the leading C and trailing Y/F amino acids.
       This is necessary for comparing full sequences when the main dataset is imported using settings that also trim
@@ -61,37 +61,39 @@
 
     - compairr_path (str): If 'full_sequence' is listed under k_values, the path to the CompAIRR executable may be provided.
       If the compairr_path is specified, the :py:obj:`~immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder.CompAIRRSequenceAbundanceEncoder`
       will be used to compute the significant sequences. If the path is not specified and 'full_sequence' is listed under
       k-values, :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder` will be used.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_recovered_significant_features_report:
-            RecoveredSignificantFeatures:
-                groundtruth_sequences_path: path/to/groundtruth/sequences.txt
-                trim_leading_trailing: False
-                p_values:
-                    - 0.1
-                    - 0.01
-                    - 0.001
-                    - 0.0001
-                k_values:
-                    - 3
-                    - 4
-                    - 5
-                    - full_sequence
-                compairr_path: path/to/compairr # can be specified if 'full_sequence' is listed under k_values
-                label: # Define a label, and the positive class for that given label
-                    CMV:
-                        positive_class: +
+        definitions:
+            reports:
+                my_recovered_significant_features_report:
+                    RecoveredSignificantFeatures:
+                        groundtruth_sequences_path: path/to/groundtruth/sequences.txt
+                        trim_leading_trailing: False
+                        p_values:
+                            - 0.1
+                            - 0.01
+                            - 0.001
+                            - 0.0001
+                        k_values:
+                            - 3
+                            - 4
+                            - 5
+                            - full_sequence
+                        compairr_path: path/to/compairr # can be specified if 'full_sequence' is listed under k_values
+                        label: # Define a label, and the positive class for that given label
+                            CMV:
+                                positive_class: +
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = RecoveredSignificantFeatures.__name__
 
         kwargs = SignificantFeaturesHelper.parse_parameters(kwargs, location)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/RepertoireClonotypeSummary.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/RepertoireClonotypeSummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,28 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class RepertoireClonotypeSummary(DataReport):
     """
     Shows the number of distinct clonotypes per repertoire in a given dataset as a bar plot.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - color_by_label (str): name of the label to use to color the plot, e.g., could be disease label, or None
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_clonotype_summary_rep:
-          RepertoireClonotypeSummary:
-            color_by_label: celiac
+        definitions:
+            reports:
+                my_clonotype_summary_rep:
+                    RepertoireClonotypeSummary:
+                        color_by_label: celiac
 
     """
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, name: str = None, number_of_processes: int = 1, color_by_label: str = None):
         super().__init__(dataset, result_path, name, number_of_processes)
         self.color_by_label = color_by_label
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/SequenceLengthDistribution.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/SequenceLengthDistribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,28 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class SequenceLengthDistribution(DataReport):
     """
     Generates a histogram of the lengths of the sequences in a repertoire or sequence dataset.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - sequence_type (str): whether to check the length of amino acid or nucleotide sequences; default value is 'amino_acid'
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_sld_report:
-            SequenceLengthDistribution:
-                sequence_type: amino_acid
+        definitions:
+            reports:
+                my_sld_report:
+                    SequenceLengthDistribution:
+                        sequence_type: amino_acid
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         ParameterValidator.assert_sequence_type(kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/SequencesWithSignificantKmers.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/SequencesWithSignificantKmers.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     Given a list of reference sequences, this report writes out the subsets of reference sequences containing significant k-mers
     (as computed by the :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder` using Fisher's exact test).
 
     For each combination of p-value and k-mer size given, a file is written containing all sequences containing a significant
     k-mer of the given size at the given p-value.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference_sequences_path (str): Path to a file containing the reference sequences,
       The file should contain one sequence per line, without a header, and without V or J genes.
 
     - p_values (list): The p value thresholds to be used by Fisher's exact test. Each p-value specified here will become
       one panel in the output figure.
 
@@ -34,34 +34,36 @@
       :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder`.
       Each k-mer length will become one panel in the output figure.
 
     - label (dict): A label configuration. One label should be specified, and the positive_class for this label should
       be defined. See the YAML specification below for an example.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_sequences_with_significant_kmers:
-            SequencesWithSignificantKmers:
-                reference_sequences_path: path/to/reference/sequences.txt
-                p_values:
-                    - 0.1
-                    - 0.01
-                    - 0.001
-                    - 0.0001
-                k_values:
-                    - 3
-                    - 4
-                    - 5
-                label: # Define a label, and the positive class for that given label
-                    CMV:
-                        positive_class: +
+        definitions:
+            reports:
+                my_sequences_with_significant_kmers:
+                    SequencesWithSignificantKmers:
+                        reference_sequences_path: path/to/reference/sequences.txt
+                        p_values:
+                            - 0.1
+                            - 0.01
+                            - 0.001
+                            - 0.0001
+                        k_values:
+                            - 3
+                            - 4
+                            - 5
+                        label: # Define a label, and the positive class for that given label
+                            CMV:
+                                positive_class: +
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = SequencesWithSignificantKmers.__name__
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/SignificantFeatures.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/SignificantFeatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Internally uses the :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder` for calculating
     significant k-mers, and
     :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder` or
     :py:obj:`~immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder.CompAIRRSequenceAbundanceEncoder`
     to calculate significant full sequences (depending on whether the argument compairr_path was set).
 
-    Specification arguments:
+    **Specification arguments:**
 
     - p_values (list): The p value thresholds to be used by Fisher's exact test. Each p-value specified here will become
       one panel in the output figure.
 
     - k_values (list): Length of the k-mers (number of amino acids) created by the
       :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder`.
       When using a full sequence encoding (:py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder` or
@@ -48,36 +48,38 @@
       If the compairr_path is specified, the :py:obj:`~immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder.CompAIRRSequenceAbundanceEncoder`
       will be used to compute the significant sequences. If the path is not specified and 'full_sequence' is listed under
       k-values, :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder` will be used.
 
     - log_scale (bool): Whether to plot the y axis in log10 scale (log_scale = True) or continuous scale (log_scale = False). By default, log_scale is False.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_significant_features_report:
-            SignificantFeatures:
-                p_values:
-                    - 0.1
-                    - 0.01
-                    - 0.001
-                    - 0.0001
-                k_values:
-                    - 3
-                    - 4
-                    - 5
-                    - full_sequence
-                compairr_path: path/to/compairr # can be specified if 'full_sequence' is listed under k_values
-                label: # Define a label, and the positive class for that given label
-                    CMV:
-                        positive_class: +
-                log_scale: False
+        definitions:
+            reports:
+                my_significant_features_report:
+                    SignificantFeatures:
+                        p_values:
+                            - 0.1
+                            - 0.01
+                            - 0.001
+                            - 0.0001
+                        k_values:
+                            - 3
+                            - 4
+                            - 5
+                            - full_sequence
+                        compairr_path: path/to/compairr # can be specified if 'full_sequence' is listed under k_values
+                        label: # Define a label, and the positive class for that given label
+                            CMV:
+                                positive_class: +
+                        log_scale: False
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = SignificantFeatures.__name__
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/SignificantKmerPositions.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/SignificantKmerPositions.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,47 +20,49 @@
 class SignificantKmerPositions(DataReport):
     """
     Plots the number of significant k-mers (as computed by the :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder` using Fisher's exact test)
     observed at each IMGT position of a given list of reference sequences.
     This report creates a stacked bar chart, where each bar represents an IMGT position, and each segment of the stack represents the observed frequency
     of one 'significant' k-mer at that position.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference_sequences_path (str): Path to a file containing the reference sequences,
       The file should contain one sequence per line, without a header, and without V or J genes.
 
     - p_values (list): The p value thresholds to be used by Fisher's exact test. Each p-value specified here will become one panel in the output figure.
 
     - k_values (list): Length of the k-mers (number of amino acids) created by the :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder`.
       Each k-mer length will become one panel in the output figure.
 
     - label (dict): A label configuration. One label should be specified, and the positive_class for this label should be defined. See the YAML specification below for an example.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_significant_kmer_positions_report:
-            SignificantKmerPositions:
-                reference_sequences_path: path/to/reference/sequences.txt
-                p_values:
-                    - 0.1
-                    - 0.01
-                    - 0.001
-                    - 0.0001
-                k_values:
-                    - 3
-                    - 4
-                    - 5
-                label: # Define a label, and the positive class for that given label
-                    CMV:
-                        positive_class: +
+        definitions:
+            reports:
+                my_significant_kmer_positions_report:
+                    SignificantKmerPositions:
+                        reference_sequences_path: path/to/reference/sequences.txt
+                        p_values:
+                            - 0.1
+                            - 0.01
+                            - 0.001
+                            - 0.0001
+                        k_values:
+                            - 3
+                            - 4
+                            - 5
+                        label: # Define a label, and the positive class for that given label
+                            CMV:
+                                positive_class: +
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = SignificantKmerPositions.__name__
 
         kwargs = SignificantFeaturesHelper.parse_parameters(kwargs, location)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/SimpleDatasetOverview.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/SimpleDatasetOverview.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,22 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class SimpleDatasetOverview(DataReport):
     """
     Generates a simple text-based overview of the properties of any dataset, including the dataset name, size, and metadata labels.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports:
-            my_overview: SimpleDatasetOverview
+        definitions:
+            reports:
+                my_overview: SimpleDatasetOverview
 
     """
     UNKNOWN_CHAIN = "unknown"
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, number_of_processes: int = 1, name: str = None):
         super().__init__(dataset=dataset, result_path=result_path, number_of_processes=number_of_processes, name=name)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/data_reports/VJGeneDistribution.py` & `immuneml-3.0.0a4/immuneML/reports/data_reports/VJGeneDistribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,31 @@
     size (original count values are additionaly exported in tsv files).
 
     - Combined V and J gene distributions: for sequence and receptor datasets, a heatmap is created showing how often each
     combination of V and J genes occurs in the dataset. A similar plot is created for repertoire datasets, except in this
     case only the average value for the normalised gene usage frequencies are shown (original count values are additionaly exported in tsv files).
 
 
-    Arguments:
+    **Specification arguments:**
 
-        split_by_label (bool): Whether to split the plots by a label. If set to true, the Dataset must either contain a single label, or alternatively the label of interest can be specified under 'label'. By default, split_by_label is False.
+    - split_by_label (bool): Whether to split the plots by a label. If set to true, the Dataset must either contain a single label, or alternatively the label of interest can be specified under 'label'. By default, split_by_label is False.
 
-        label (str): Optional label for separating the results by color/creating separate plots. Note that this should the name of a valid dataset label.
+    - label (str): Optional label for separating the results by color/creating separate plots. Note that this should the name of a valid dataset label.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_vj_gene_report:
-          VJGeneDistribution:
-            label: ag_binding
+        definitions:
+            reports:
+                my_vj_gene_report:
+                    VJGeneDistribution:
+                        label: ag_binding
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = VJGeneDistribution.__name__
 
@@ -285,17 +287,17 @@
 
     def _get_repertoire_count_dfs(self):
         v_dfs = []
         j_dfs = []
         vj_dfs = []
 
         for repertoire in self.dataset.repertoires:
-            repertoire_attributes = {"v_call": repertoire.get_v_genes().tolist(),
-                                     "j_call": repertoire.get_j_genes().tolist(),
-                                     "chain": repertoire.get_attribute("chain").tolist()}
+            repertoire_attributes = {"v_call": repertoire.get_v_genes(),
+                                     "j_call": repertoire.get_j_genes(),
+                                     "chain": repertoire.get_attribute("chain", as_list=True)}
 
             v_rep_df = self._get_gene_count_df(repertoire_attributes, "v_call", include_label=False)
             j_rep_df = self._get_gene_count_df(repertoire_attributes, "j_call", include_label=False)
             vj_rep_df = self._get_vj_combo_count_df(repertoire_attributes, include_label=False)
 
             self._supplement_repertoire_df(v_rep_df, repertoire)
             self._supplement_repertoire_df(j_rep_df, repertoire)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/DesignMatrixExporter.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/DesignMatrixExporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import os
 import warnings
 import zipfile
-from dataclasses import dataclass
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import yaml
 
 from immuneML.data_model.dataset.Dataset import Dataset
@@ -19,30 +18,32 @@
 
 class DesignMatrixExporter(EncodingReport):
     """
     Exports the design matrix and related information of a given encoded Dataset to csv files.
     If the encoded data has more than 2 dimensions (such as when using the OneHot encoder with option Flatten=False),
     the data are then exported to different formats to facilitate their import with external software.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - file_format (str): the format and extension of the file to store the design matrix. The supported formats are:
       npy, csv, hdf5, npy.zip, csv.zip or hdf5.zip.
 
     Note: when using hdf5 or hdf5.zip output formats, make sure the 'hdf5' dependency is installed.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_dme_report:
-            DesignMatrixExporter:
-                file_format: csv
+        definitions:
+            reports:
+                my_dme_report:
+                    DesignMatrixExporter:
+                        file_format: csv
 
     """
     def __init__(self, dataset: Dataset = None, result_path: Path = None, file_format: str = None, number_of_processes: int = 1, name: str = None):
         super().__init__(dataset=dataset, result_path=result_path, number_of_processes=number_of_processes, name=name)
         self.file_format = file_format
 
     @classmethod
@@ -62,24 +63,25 @@
         return ReportResult(self.name,
                             info="The design matrix and related information of a given encoded Dataset",
                             output_tables=[matrix_result, label_result], output_text=[details_result])
 
     def _export_matrix(self) -> ReportOutput:
         """Create a file for the design matrix in the desired format."""
         
-        data = self._get_data()
+        data = self.dataset.encoded_data.get_examples_as_np_matrix()
         file_path = self.result_path / "design_matrix"
         ext = os.path.splitext(self.file_format)[0]
         file_path = file_path.with_suffix('.' + ext)
 
         # Use h5py to create a hdf5 file.
         if ext == "hdf5":
             import h5py
             with h5py.File(str(file_path), 'w') as hf_object:
                 hf_object.create_dataset(str(file_path), data=data)
+
         # Use numpy to create a csv or npy file.
         elif len(data.shape) <= 2 and ext == "csv":
             feature_names = self.dataset.encoded_data.feature_names
             header = ",".join(str(name) for name in feature_names) if feature_names is not None else ""
             np.savetxt(fname=str(file_path), X=data, delimiter=",", comments='',
                        header=header)
         else:
@@ -94,23 +96,14 @@
             file_path_zip = file_path.with_suffix('.' + ext + '.zip')
             with zipfile.ZipFile(str(file_path_zip), 'w') as zipped_file:
                 zipped_file.write(str(file_path), compress_type=zipfile.ZIP_DEFLATED)
             os.remove(str(file_path)) 
             file_path = file_path_zip
         return ReportOutput(file_path, "design matrix")
 
-    def _get_data(self) -> np.ndarray:
-        if isinstance(self.dataset.encoded_data.examples, np.ndarray):
-            data = self.dataset.encoded_data.examples
-        elif isinstance(self.dataset.encoded_data.examples, pd.DataFrame):
-            data = self.dataset.encoded_data.examples.to_numpy()
-        else: #scipy
-            data = self.dataset.encoded_data.examples.toarray()
-        return data
-
     def _export_details(self) -> ReportOutput:
         file_path = self.result_path / "encoding_details.yaml"
         with file_path.open("w") as file:
             details = {
                 "feature_names": self.dataset.encoded_data.feature_names,
                 "encoding": self.dataset.encoded_data.encoding,
                 "example_ids": list(self.dataset.encoded_data.example_ids)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/DimensionalityReduction.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/DimensionalityReduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,26 +13,29 @@
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class DimensionalityReduction(EncodingReport):
     """
     This report visualizes the data obtained by dimensionality reduction.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - label (str): name of the label to use for highlighting data points
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        rep1:
-            DimensionalityReduction:
-                label: epitope
+        definitions:
+            reports:
+                rep1:
+                    DimensionalityReduction:
+                        label: epitope
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return DimensionalityReduction(**{**kwargs})
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/EncodingReport.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/EncodingReport.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,25 +40,21 @@
             analyses:
                 my_first_analysis:
                     report: my_encoding_report
                     # other parameters...
             # other parameters...
 
     """
+    DOCS_TITLE = "Encoding reports"
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, name: str = None, number_of_processes: int = 1):
         """
         The arguments defined below are set at runtime by the instruction.
         Concrete classes inheriting EncodingReport may include additional parameters that will be set by the user in the form of input arguments.
 
         dataset (Dataset): an encoded dataset where encoded_data attribute is set to an instance of EncodedData object
         result_path (Path): path where the results will be stored (plots, tables, etc.)
         name (str): user-defined name of the report that will be shown in the HTML overview later
         number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
         """
-        super().__init__(name, number_of_processes)
+        super().__init__(name=name, result_path=result_path, number_of_processes=number_of_processes)
         self.dataset = dataset
-        self.result_path = result_path
-
-    @staticmethod
-    def get_title():
-        return "Encoding reports"
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureComparison.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     scatterplot is determined by their frequency in the subset of the data where disease=true and disease=false.
 
     Optional metadata labels can be specified to divide the scatterplot into groups based on color, row facets or column facets.
 
     Alternatively, when the feature values are of interest without comparing them between labelled subgroups of the data, please
     use :ref:`FeatureValueBarplot` or :ref:`FeatureDistribution` instead.
 
-    Specification arguments:
+
+    **Specification arguments:**
 
     - comparison_label (str): Mandatory label. This label is used to split the encoded data matrix and define the x and y axes of the plot.
       This label is only allowed to have 2 classes (for example: sick and healthy, binding and non-binding).
 
     - color_grouping_label (str): Optional label that is used to color the points in the scatterplot. This can not be the same as comparison_label.
 
     - row_grouping_label (str): Optional label that is used to group scatterplots into different row facets. This can not be the same as comparison_label.
@@ -45,22 +46,24 @@
       comparison labels may be of interest. When the keep_fraction parameter is set below 1, only the fraction of features that
       differs the most across comparison labels is kept for plotting (note that the produced .csv file still contains all data).
       By default, keep_fraction is 1, meaning that all features are plotted.
 
     - opacity (float): a value between 0 and 1 setting the opacity for data points making it easier to see if there are overlapping points
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_comparison_report:
-            FeatureComparison: # compare the different classes defined in the label disease
-                comparison_label: disease
+        definitions:
+            reports:
+                my_comparison_report:
+                    FeatureComparison: # compare the different classes defined in the label disease
+                        comparison_label: disease
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         comparison_label = kwargs["comparison_label"] if "comparison_label" in kwargs else None
         color_grouping_label = kwargs["color_grouping_label"] if "color_grouping_label" in kwargs else None
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureDistribution.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureDistribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,37 +25,39 @@
     These labels are specified in the metadata file for repertoire datasets, or as metadata columns for sequence and receptor datasets.
 
     Alternatively, when only the mean feature values are of interest (as opposed to showing the complete distribution, as done here),
     please consider using :ref:`FeatureValueBarplot` instead.
     When comparing the feature values between two subsets of the data, please use :ref:`FeatureComparison`.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - color_grouping_label (str): The label that is used to color each bar, at each level of the grouping_label.
 
     - row_grouping_label (str): The label that is used to group bars into different row facets.
 
     - column_grouping_label (str): The label that is used to group bars into different column facets.
 
     - mode (str): either 'normal', 'sparse' or 'auto' (default)
 
     - x_title (str): x-axis label
 
     - y_title (str): y-axis label
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_fdistr_report:
-            FeatureDistribution:
-                mode: sparse
+        definitions:
+            reports:
+                my_fdistr_report:
+                    FeatureDistribution:
+                        mode: sparse
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return FeatureDistribution(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureReport.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureReport.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/FeatureValueBarplot.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/FeatureValueBarplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     In this case, the average feature values in each group are plotted.
     These labels are specified in the metadata file for repertoire datasets, or as metadata columns for sequence and receptor datasets.
 
     Alternatively, when the distribution of feature values is of interest (as opposed to showing only the mean, as done here),
     please consider using :ref:`FeatureDistribution` instead.
     When comparing the feature values between two subsets of the data, please use :ref:`FeatureComparison`.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - color_grouping_label (str): The label that is used to color each bar, at each level of the grouping_label.
 
     - row_grouping_label (str): The label that is used to group bars into different row facets.
 
     - column_grouping_label (str): The label that is used to group bars into different column facets.
 
@@ -41,27 +41,29 @@
     - plot_top_n (int): plot n of the largest features on average separately (useful when there are too many features to plot at the same time)
 
     - plot_bottom_n (int): plot n of the smallest features on average separately (useful when there are too many features to plot at the same time)
 
     - plot_all_features (bool): whether to plot all (might be slow for large number of features)
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_fvb_report:
-            FeatureValueBarplot: # timepoint, disease_status and age_group are metadata labels
-                column_grouping_label: timepoint
-                row_grouping_label: disease_status
-                color_grouping_label: age_group
-                plot_all_features: true
-                plot_top_n: 10
-                plot_bottom_n: 5
+        definitions:
+            reports:
+                my_fvb_report:
+                    FeatureValueBarplot: # timepoint, disease_status and age_group are metadata labels
+                        column_grouping_label: timepoint
+                        row_grouping_label: disease_status
+                        color_grouping_label: age_group
+                        plot_all_features: true
+                        plot_top_n: 10
+                        plot_bottom_n: 5
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return FeatureValueBarplot(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/GroundTruthMotifOverlap.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/GroundTruthMotifOverlap.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,47 @@
 from immuneML.encodings.motif_encoding.MotifEncoder import MotifEncoder
 from immuneML.reports.encoding_reports.EncodingReport import EncodingReport
 from immuneML.util.PathBuilder import PathBuilder
 
 
 class GroundTruthMotifOverlap(EncodingReport):
     """
-    Creates report displaying overlap between learned motifs and groundtruth motifs
+    Creates report displaying overlap between learned motifs and groundtruth motifs implanted in a given sequence dataset.
+    This report must be used in combination with the MotifEncoder.
 
-    # todo: arguments, yaml spec, explanation of format of highlight motifs file
-    """
+    **Specification arguments:**
+
+    - groundtruth_motifs_path (str): Path to a .tsv file containing groundtruth position-specific motifs.
+      The file should specify the motifs as position-specific amino acids, one column representing the positions
+      concatenated with an '&' symbol, the next column specifying the amino acids concatenated with '&' symbol,
+      and the last column specifying the implant rate.
+
+      Example:
+
+      =======  ===========  ===========
+      indices  amino_acids  n_sequences
+      =======  ===========  ===========
+      0        A            4
+      4&8&9    G&A&C        30
+      =======  ===========  ===========
+
+      This file shows a motif 'A' at position 0 implanted in 4 sequences, and motif G---AC implanted between positions 4 and 9 in 30 sequences
+
+
+    **YAML specification:**
+
+    .. indent with spaces
+    .. code-block:: yaml
+
+        definitions:
+            reports:
+                my_ground_truth_motif_report:
+                    GroundTruthMotifOverlap:
+                        groundtruth_motifs_path: path/to/file.tsv
+            """
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, name: str = None,
                  number_of_processes: int = 1, groundtruth_motifs_path: str = None):
         super().__init__(dataset=dataset, result_path=result_path, name=name, number_of_processes=number_of_processes)
         self.groundtruth_motifs_path = groundtruth_motifs_path
 
     @classmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/Matches.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/Matches.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,20 +33,22 @@
       :ref:`MatchedReceptors` encoder, tables describing
       the chains and receptors (ids, chains, V and J genes and sequences).
     * When using :ref:`MatchedReceptors` encoder or using
       :ref:`MatchedRegex` encoder with chain pairs, tables describing
       the paired matches (where a match was found in both chains) per repertoire.
 
 
-    YAML Specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_match_report: Matches
+        definitions:
+            reports:
+                my_match_report: Matches
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return Matches(**kwargs)
 
     def __init__(self, dataset: RepertoireDataset = None, result_path: Path = None, name: str = None, number_of_processes: int = 1):
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/MotifTestSetPerformance.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/MotifTestSetPerformance.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,34 +27,36 @@
     """
     This report can be used to show the performance of a learned set motifs using the :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder`
     on an independent test set of unseen data.
 
     It is recommended to first run the report :py:obj:`~immuneML.reports.data_reports.MotifGeneralizationAnalysis.MotifGeneralizationAnalysis`
     in order to calibrate the optimal recall thresholds and plot the performance of motifs on training- and validation sets.
 
-    Arguments:
+    **Specification arguments:**
 
-        test_dataset (dict): parameters for importing a SequenceDataset to use as an independent test set. By default,
-        the import parameters 'is_repertoire' and 'paired' will be set to False to ensure a SequenceDataset is imported.
+    - test_dataset (dict): parameters for importing a SequenceDataset to use as an independent test set. By default,
+      the import parameters 'is_repertoire' and 'paired' will be set to False to ensure a SequenceDataset is imported.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_motif_report:
-            MotifTestSetPerformance:
-                test_dataset:
-                    format: AIRR # choose any valid import format
-                    params:
-                        path: path/to/files/
-                        is_repertoire: False  # is_repertoire must be False to import a SequenceDataset
-                        paired: False         # paired must be False to import a SequenceDataset
-                        # optional other parameters...
+        definitions:
+            reports:
+                my_motif_report:
+                    MotifTestSetPerformance:
+                        test_dataset:
+                            format: AIRR # choose any valid import format
+                            params:
+                                path: path/to/files/
+                                is_repertoire: False  # is_repertoire must be False to import a SequenceDataset
+                                paired: False         # paired must be False to import a SequenceDataset
+                                # optional other parameters...
 
     """
 
     def __init__(self, dataset: Dataset = None, result_path: Path = None, test_dataset_import_cls: DataImport = None,
                  test_dataset_import_params: DatasetImportParams = None,
                  training_set_name: str = None, test_set_name: str = None,
                  split_by_motif_size: bool = None,
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/NonMotifSequenceSimilarity.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/NonMotifSequenceSimilarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,30 +26,32 @@
     For each motif, the subset of sequences containing the motif is selected, and the hamming distances are computed
     between all sequences in this subset. Finally, a plot is created showing the distribution of hamming distances
     between the sequences containing the motif. For motifs occurring in sets of very similar sequences, this distribution
     will lean towards small hamming distances. Likewise, for motifs occurring in a very diverse set of sequences, the
     distribution will lean towards containing more large hamming distances.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
-        motif_color_map (dict): An optional mapping between motif sizes and colors. If no mapping is given, default colors will be chosen.
+    - motif_color_map (dict): An optional mapping between motif sizes and colors. If no mapping is given, default colors will be chosen.
 
 
-    YAML specification example:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_motif_sim:
-            NonMotifSimilarity:
-                motif_color_map:
-                    3: "#66C5CC"
-                    4: "#F6CF71"
-                    5: "#F89C74"
+        definitions:
+            reports:
+                my_motif_sim:
+                    NonMotifSimilarity:
+                        motif_color_map:
+                            3: "#66C5CC"
+                            4: "#F6CF71"
+                            5: "#F89C74"
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         if "motif_color_map" in kwargs:
             ParameterValidator.assert_type_and_value(kwargs["motif_color_map"], dict, NonMotifSequenceSimilarity.__name__, "motif_color_map")
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/PositionalMotifFrequencies.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/PositionalMotifFrequencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,23 +23,34 @@
 class PositionalMotifFrequencies(EncodingReport):
     """
     This report must be used in combination with the :py:obj:`~immuneML.encodings.motif_encoding.MotifEncoder.MotifEncoder`.
     Plots a stacked bar plot of amino acid occurrence at different indices in any given dataset, along with a plot
     investigating motif continuity which displays a bar plot of the gap sizes between the amino acids in the motifs in
     the given dataset. Note that a distance of 1 means that the amino acids are continuous (next to each other).
 
-    Arguments:
+    **Specification arguments:**
 
+    - motif_color_map (dict): Optional mapping between motif lengths and specific colors to be used. Example:
 
-    YAML specification example:
+        motif_color_map:
+            1: #66C5CC
+            2: #F6CF71
+            3: #F89C74
+
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_pos_motif_report: PositionalMotifFrequencies
+        definitions:
+            reports:
+                my_pos_motif_report:
+                    PositionalMotifFrequencies:
+                        motif_color_map:
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         if "motif_color_map" in kwargs:
             ParameterValidator.assert_type_and_value(kwargs["motif_color_map"], dict, PositionalMotifFrequencies.__name__, "motif_color_map")
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/encoding_reports/RelevantSequenceExporter.py` & `immuneml-3.0.0a4/immuneML/reports/encoding_reports/RelevantSequenceExporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 
 
 class RelevantSequenceExporter(EncodingReport):
     """
     Exports the sequences that are extracted as label-associated when using the :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder` or
     :py:obj:`~immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder.CompAIRRSequenceAbundanceEncoder` in AIRR-compliant format.
 
-    Specification arguments: there are no arguments for this report.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_relevant_sequences: RelevantSequenceExporter
+        definitions:
+            reports:
+                my_relevant_sequences: RelevantSequenceExporter
 
     """
 
     COLUMN_MAPPING = {
         "v_gene": "v_call",
         "j_gene": "j_call",
         "sequence": "cdr3",
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/gen_model_reports/VAESummary.py` & `immuneml-3.0.0a4/immuneML/reports/gen_model_reports/VAESummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,31 @@
     """
     This report provides the summary of the train SimpleVAE and shows the following:
 
     - plots of the latent space after applying PCA to reduce the data to 2 dimensions, highlighted by V and J gene
     - plots the histogram for each latent dimension
     - plots loss per epoch
 
-    Arguments:
+    **Specification arguments:**
 
-        dim_dist_cols (int): how many columns to use to plot the histograms of latent dimensions (either this or dim_dist_rows has to be set, or both)
+    - dim_dist_cols (int): how many columns to use to plot the histograms of latent dimensions (either this or dim_dist_rows has to be set, or both)
 
-        dim_dist_rows (int): how many rows to use to plot the histogram of latent dimensions (either this or dim_dist_cols has to be set, or both)
+    - dim_dist_rows (int): how many rows to use to plot the histogram of latent dimensions (either this or dim_dist_cols has to be set, or both)
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_vae_summary:
-          VAESummary:
-            dim_dist_cols: 4
-            dim_dist_rows: None
+        definitions:
+            reports:
+                my_vae_summary:
+                    VAESummary:
+                        dim_dist_cols: 4
+                        dim_dist_rows: None
 
     """
     @classmethod
     def build_object(cls, **kwargs):
         name = kwargs["name"] if "name" in kwargs else "VAESummary"
 
         ParameterValidator.assert_keys_present(list(kwargs.keys()), ['dim_dist_cols', 'dim_dist_rows'],
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/BinaryFeaturePrecisionRecall.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/BinaryFeaturePrecisionRecall.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 
 from sklearn.metrics import precision_score, recall_score, accuracy_score, balanced_accuracy_score
 
 from immuneML.ml_methods.util.Util import Util
 from immuneML.data_model.dataset.Dataset import Dataset
 from immuneML.encodings.motif_encoding.MotifEncoder import MotifEncoder
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
-from immuneML.ml_methods.BinaryFeatureClassifier import BinaryFeatureClassifier
+from immuneML.ml_methods.classifiers.BinaryFeatureClassifier import BinaryFeatureClassifier
 from immuneML.reports.ReportOutput import ReportOutput
 from immuneML.reports.ReportResult import ReportResult
 from immuneML.reports.ml_reports.MLReport import MLReport
 from immuneML.util.PathBuilder import PathBuilder
 
 
 
 
 class BinaryFeaturePrecisionRecall(MLReport):
     """
+    Plots the precision and recall scores for each added feature to the collection of features selected by the BinaryFeatureClassifier.
 
 
-    Arguments:
-
-
-
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_report: BinaryFeaturePrecisionRecall
+        definitions:
+            reports:
+                my_report: BinaryFeaturePrecisionRecall
     """
 
     @classmethod
     def build_object(cls, **kwargs):
 
         return BinaryFeaturePrecisionRecall(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/CoefficientPlottingSettingList.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/Coefficients.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/Coefficients.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,41 +32,43 @@
     the selection and assessment levels.
 
     Which coefficients should be plotted (for example: only nonzero, above a certain threshold, ...) can be specified.
     Multiple options can be specified simultaneously. By default the 25 largest coefficients are plotted.
     The full set of coefficients will also be exported as a csv file.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - coefs_to_plot (list): A list specifying which coefficients should be plotted. For options see :py:obj:`~immuneML.reports.ml_reports.CoefficientPlottingSetting.CoefficientPlottingSetting`.
 
     - cutoff (list): If 'cutoff' is specified under 'coefs_to_plot', the cutoff values can be specified here. The coefficients which have an absolute value equal to or greater than the cutoff will be plotted.
 
     - n_largest (list): If 'n_largest' is specified under 'coefs_to_plot', the values for n can be specified here. These should be integer values. The n largest coefficients are determined based on their absolute values.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_coef_report:
-            Coefficients:
-                coefs_to_plot:
-                    - all
-                    - nonzero
-                    - cutoff
-                    - n_largest
-                cutoff:
-                    - 0.1
-                    - 0.01
-                n_largest:
-                    - 5
-                    - 10
+        definitions:
+            reports:
+                my_coef_report:
+                    Coefficients:
+                        coefs_to_plot:
+                            - all
+                            - nonzero
+                            - cutoff
+                            - n_largest
+                        cutoff:
+                            - 0.1
+                            - 0.01
+                        n_largest:
+                            - 5
+                            - 10
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = "Coefficients"
         coefs_to_plot = [coef.upper() for coef in kwargs["coefs_to_plot"]]
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/ConfounderAnalysis.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/ConfounderAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 
 class ConfounderAnalysis(MLReport):
     """
     A report that plots the numbers of false positives and false negatives with respect to each value of
     the metadata features specified by the user. This allows checking whether a given machine learning model makes more
     misclassifications for some values of a metadata feature than for the others.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - metadata_labels (list): A list of the metadata features to use as a basis for the calculations
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_confounder_report:
-            ConfounderAnalysis:
-                metadata_labels:
-                  - age
-                  - sex
+        definitions:
+            reports:
+                my_confounder_report:
+                    ConfounderAnalysis:
+                        metadata_labels:
+                          - age
+                          - sex
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
 
         ParameterValidator.assert_keys(kwargs.keys(), ['metadata_labels', 'name'], ConfounderAnalysis.__name__, ConfounderAnalysis.__name__)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/DeepRCMotifDiscovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,30 +34,32 @@
 
     Reference:
 
     Widrich, M., et al. (2020). Modern Hopfield Networks and Attention for Immune Repertoire Classification. Advances in
     Neural Information Processing Systems, 33. https://proceedings.neurips.cc//paper/2020/hash/da4902cb0bc38210839714ebdcf0efc3-Abstract.html
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - n_steps (int): Number of IG steps (more steps -> better path integral -> finer contribution values). 50 is usually good enough.
 
     - threshold (float): Only applies to the plotting of kernels. Contributions are normalized to range [0, 1], and only kernels with normalized contributions above threshold are plotted.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_deeprc_report:
-            DeepRCMotifDiscovery:
-                threshold: 0.5
-                n_steps: 50
+        definitions:
+            reports:
+                my_deeprc_report:
+                    DeepRCMotifDiscovery:
+                        threshold: 0.5
+                        n_steps: 50
 
     """
 
     def __init__(self, n_steps, threshold, train_dataset: Dataset = None, test_dataset: Dataset = None,
                  method: MLMethod = None, result_path: Path = None, name: str = None, hp_setting: HPSetting = None,
                  label=None, number_of_processes: int = 1):
         super().__init__(train_dataset=train_dataset, test_dataset=test_dataset, method=method, result_path=result_path,
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/KernelSequenceLogo.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/KernelSequenceLogo.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     A report that plots kernels of a CNN model as sequence logos. It works only with trained ReceptorCNN models which has kernels already normalized
     to represent information gain matrices. Additionally, it also plots the weights in the final fully-connected layer of the network associated with
     kernel outputs. For more information on how the model works, see :ref:`ReceptorCNN`.
 
     The kernels are visualized using Logomaker. Original publication: Tareen A, Kinney JB. Logomaker: beautiful sequence logos in Python.
     Bioinformatics. 2020; 36(7):2272-2274. `doi:10.1093/bioinformatics/btz921 <https://academic.oup.com/bioinformatics/article/36/7/2272/5671693>`_.
 
-    Specification arguments: this report does not take any arguments as input.
 
-
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_kernel_seq_logo: KernelSequenceLogo
+        definitions:
+            reports:
+                my_kernel_seq_logo: KernelSequenceLogo
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return KernelSequenceLogo(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/MLReport.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/MLReport.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from immuneML.hyperparameter_optimization.HPSetting import HPSetting
 from immuneML.ml_methods.classifiers.MLMethod import MLMethod
 from immuneML.reports.Report import Report
 
 
 class MLReport(Report):
     """
-    ML model reports show some type of features or statistics about one trained ML model.
+    ML model reports show some type of features or statistics about a single trained ML model.
 
     In the :ref:`TrainMLModel` instruction, ML model reports can be specified inside the 'selection' or 'assessment' specification under the key 'reports/models'.
     Example:
 
     .. indent with spaces
     .. code-block:: yaml
 
@@ -27,14 +27,15 @@
             assessment:
                 reports:
                     models:
                         - my_ml_report
                 # other parameters...
             # other parameters...
     """
+    DOCS_TITLE = "ML model reports"
 
     def __init__(self, train_dataset: Dataset = None, test_dataset: Dataset = None, method: MLMethod = None,
                  result_path: Path = None, name: str = None, hp_setting: HPSetting = None, label: Label =None, number_of_processes: int = 1):
         """
         The arguments defined below are set at runtime by the instruction.
         Concrete classes inheriting MLReport may include additional parameters that will be set by the user in the form of input arguments.
 
@@ -43,19 +44,15 @@
         method (MLMethod): a trained instance of a concrete subclass of MLMethod object
         result_path (Path): location where the report results will be stored
         hp_setting (HPSetting): a HPSetting object describing the ML method, encoding and preprocessing used
         label (Label): the label for which the model was trained
         name (str): user-defined name of the report used in the HTML overview automatically generated by the platform
         number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
         """
-        super().__init__(name, number_of_processes)
+        super().__init__(name=name, result_path=result_path, number_of_processes=number_of_processes)
         self.train_dataset = train_dataset
         self.test_dataset = test_dataset
         self.method = method
-        self.result_path = result_path
         self.name = name
         self.hp_setting = hp_setting
         self.label = label
 
-    @staticmethod
-    def get_title():
-        return "ML model reports"
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/MotifSeedRecovery.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/MotifSeedRecovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,53 +64,55 @@
         Seed:     A/AA  -> score = 3
         Feature: xAxAAx
                   ^/^^
 
     See :ref:`Recovering simulated immune signals` for more details and an example plot.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - implanted_motifs_per_label (dict): a nested dictionary that specifies the motif seeds that were implanted in the given dataset. The first
       level of keys in this dictionary represents the different labels. In the inner dictionary there should be two keys: "seeds" and
       "hamming_distance":
 
       - seeds: a list of motif seeds. The seeds may contain gaps, specified by a '/' symbol.
 
       - hamming_distance: A boolean value that specifies whether hamming distance was allowed when implanting the motif
         seeds for a given label. Note that this applies to all seeds for this label.
 
       - gap_sizes: a list of all the possible gap sizes that were used when implanting a gapped motif seed. When no
         gapped seeds are used, this value has no effect.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_motif_report:
-            MotifSeedRecovery:
-                implanted_motifs_per_label:
-                    CD:
-                        seeds:
-                        - AA/A
-                        - AAA
-                        hamming_distance: False
-                        gap_sizes:
-                        - 0
-                        - 1
-                        - 2
-                    T1D:
-                        seeds:
-                        - CC/C
-                        - CCC
-                        hamming_distance: True
-                        gap_sizes:
-                        - 2
+        definitions:
+            reports:
+                my_motif_report:
+                    MotifSeedRecovery:
+                        implanted_motifs_per_label:
+                            CD:
+                                seeds:
+                                - AA/A
+                                - AAA
+                                hamming_distance: False
+                                gap_sizes:
+                                - 0
+                                - 1
+                                - 2
+                            T1D:
+                                seeds:
+                                - CC/C
+                                - CCC
+                                hamming_distance: True
+                                gap_sizes:
+                                - 2
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         ParameterValidator.assert_keys_present(list(kwargs.keys()),
                                                ["implanted_motifs_per_label"],
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/ROCCurve.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/ROCCurve.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 
 class ROCCurve(MLReport):
     """
     A report that plots the ROC curve for a binary classifier.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports:
-          my_roc_report: ROCCurve
+        definitions:
+            reports:
+                my_roc_report: ROCCurve
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         name = kwargs["name"] if "name" in kwargs else "ROC_curve"
         return ROCCurve(name=name)
@@ -34,18 +35,18 @@
     def _generate(self) -> ReportResult:
         x = self.test_dataset.encoded_data
 
         if self.method.can_predict_proba():
             predicted_y = self.method.predict_proba(x, self.label)[self.label.name][self.label.positive_class]
         else:
             predicted_y = self.method.predict(x, self.label)[self.label.name]
-            predicted_y = Util.map_to_new_class_values(predicted_y, self.method.get_class_mapping())
+            predicted_y = Util.map_to_new_class_values(predicted_y, self.method.class_mapping)
 
         true_y = x.labels[self.label.name]
-        true_y = Util.map_to_new_class_values(true_y, self.method.get_class_mapping())
+        true_y = Util.map_to_new_class_values(true_y, self.method.class_mapping)
 
         fpr, tpr, _ = roc_curve(true_y, predicted_y)
         roc_auc = auc(fpr, tpr)
 
 
         trace1 = go.Scatter(x=fpr, y=tpr,
                             mode='lines',
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/SequenceAssociationLikelihood.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 
 
 class SequenceAssociationLikelihood(MLReport):
     """
     Plots the beta distribution used as a prior for class assignment in ProbabilisticBinaryClassifier. The distribution plotted shows
     the probability that a sequence is associated with a given class for a label.
 
-    Attributes: the report does not take in any arguments.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_sequence_assoc_report: SequenceAssociationLikelihood
+        definitions:
+            reports:
+                my_sequence_assoc_report: SequenceAssociationLikelihood
 
     """
 
     DISTRIBUTION_PERCENTAGE_TO_SHOW = 0.999
     STEP = 400
 
     @classmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/TCRdistMotifDiscovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,40 +29,42 @@
     Nature. 2017; 547(7661):89-93. `doi:10.1038/nature22383 <https://www.nature.com/articles/nature22383>`_
 
     Mayer-Blackwell K, Schattgen S, Cohen-Lavi L, et al. TCR meta-clonotypes for biomarker discovery with tcrdist3: quantification of public,
     HLA-restricted TCR biomarkers of SARS-CoV-2 infection. bioRxiv. Published online December 26, 2020:2020.12.24.424260.
     `doi:10.1101/2020.12.24.424260 <https://www.biorxiv.org/content/10.1101/2020.12.24.424260v1>`_
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - positive_class_name (str): the class value (e.g., epitope) used to select only the receptors that are specific to the given epitope so that
       only those sequences are used to infer motifs; the reference receptors as required by TCRdist will be the ones from the dataset that have
       different or no epitope specified in their metadata; if the labels are available only on the epitope level (e.g., label is "AVFDRKSDAK" and
       classes are True and False), then here it should be specified that only the receptors with value "True" for label "AVFDRKSDAK" should be used;
       there is no default value for this argument
 
     - cores (int): number of processes to use for the computation of the distance and motifs
 
     - min_cluster_size (int): the minimum size of the cluster to discover the motifs for
 
     - use_reference_sequences (bool): when showing motifs, this parameter defines if reference sequences should be provided as well as a background
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_tcr_dist_report: # user-defined name
-            TCRdistMotifDiscovery:
-                positive_class_name: True # class name, could also be epitope name, depending on how it's defined in the dataset
-                cores: 4
-                min_cluster_size: 30
-                use_reference_sequences: False
+        definitions:
+            reports:
+                my_tcr_dist_report: # user-defined name
+                    TCRdistMotifDiscovery:
+                        positive_class_name: True # class name, could also be epitope name, depending on how it's defined in the dataset
+                        cores: 4
+                        min_cluster_size: 30
+                        use_reference_sequences: False
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return TCRdistMotifDiscovery(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/ml_reports/TrainingPerformance.py` & `immuneml-3.0.0a4/immuneML/reports/ml_reports/TrainingPerformance.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,37 +19,39 @@
 
 class TrainingPerformance(MLReport):
     """
     A report that plots the evaluation metrics for the performance given machine learning model and training dataset.
     The available metrics are accuracy, balanced_accuracy, confusion_matrix, f1_micro, f1_macro, f1_weighted, precision,
     recall, auc and log_loss (see :py:obj:`immuneML.environment.Metric.Metric`).
 
-    Specification arguments:
+    **Specification arguments:**
 
     - metrics (list): A list of metrics used to evaluate training performance. See :py:obj:`immuneML.environment.Metric.Metric` for available options.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_performance_report:
-            TrainingPerformance: 
-                metrics:
-                    - accuracy
-                    - balanced_accuracy
-                    - confusion_matrix
-                    - f1_micro
-                    - f1_macro
-                    - f1_weighted
-                    - precision
-                    - recall
-                    - auc
-                    - log_loss
+        definitions:
+            reports:
+                my_performance_report:
+                    TrainingPerformance:
+                        metrics:
+                            - accuracy
+                            - balanced_accuracy
+                            - confusion_matrix
+                            - f1_micro
+                            - f1_macro
+                            - f1_weighted
+                            - precision
+                            - recall
+                            - auc
+                            - log_loss
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = "TrainingPerformance"        
         valid_metrics = [m.name for m in ClassificationMetric]
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py` & `immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/DiseaseAssociatedSequenceOverlap.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 
         overlap(X,Y) = \\frac{|X \\cap Y|}{min(|X|, |Y|)} * 100
 
     For details, see:
     Greiff V, Menzel U, Miho E, et al. Systems Analysis Reveals High Genetic and Antigen-Driven Predetermination of Antibody
     Repertoires throughout B Cell Development. Cell Reports. 2017;19(7):1467-1478. doi:10.1016/j.celrep.2017.04.054.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports: # the report is defined with all other reports under definitions/reports
-            my_overlap_report: DiseaseAssociatedSequenceOverlap # report has no parameters
+        definitions:
+            reports:
+                my_overlap_report: DiseaseAssociatedSequenceOverlap # report has no parameters
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return DiseaseAssociatedSequenceOverlap(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py` & `immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/MultiDatasetReport.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,38 +4,35 @@
 from immuneML.hyperparameter_optimization.states.TrainMLModelState import TrainMLModelState
 from immuneML.reports.Report import Report
 
 
 class MultiDatasetReport(Report):
     '''
     Multi dataset reports are special reports that can be specified when running immuneML with the :py:obj:`~immuneML.api.aggregated_runs.MultiDatasetBenchmarkTool.MultiDatasetBenchmarkTool`.
+    See Manuscript use case 1: :ref:`Robustness assessment` for an example.
 
     When running the :py:obj:`~immuneML.api.aggregated_runs.MultiDatasetBenchmarkTool.MultiDatasetBenchmarkTool`, multi dataset reports can be specified under 'benchmark_reports'.
     Example:
 
     .. indent with spaces
     .. code-block:: yaml
 
         my_instruction:
             type: TrainMLModel
             benchmark_reports:
                 - my_benchmark_report
             # other parameters...
     '''
+    DOCS_TITLE = "Multi dataset reports"
 
     def __init__(self, instruction_states: List[TrainMLModelState] = None, name: str = None, result_path: Path = None, number_of_processes: int = 1):
         '''
          When using the reports with MultiDatasetBenchmarkTool, the arguments defined below are set at runtime by the instruction.
         Concrete classes inheriting MultiDatasetReport may include additional parameters that will be set by the user in the form of input arguments.
 
         name (str): user-defined name of the report used in the HTML overview automatically generated by the platform
         result_path (Path): location where the report results will be stored
         instruction_states (list): a list of states for each instruction that was run as a part of the tool, e.g., TrainMLModelState objects
         number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
         '''
-        super().__init__(name, number_of_processes)
+        super().__init__(name=name, result_path=result_path, number_of_processes=number_of_processes)
         self.instruction_states = instruction_states
-        self.result_path = result_path
-
-    @staticmethod
-    def get_title():
-        return "Multi dataset reports"
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/multi_dataset_reports/PerformanceOverview.py` & `immuneml-3.0.0a4/immuneML/reports/multi_dataset_reports/PerformanceOverview.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 
     If datasets have the same number of examples, the baseline PR curve will be plotted as described in this publication:
     Saito T, Rehmsmeier M. The Precision-Recall Plot Is More Informative than the ROC Plot When Evaluating Binary Classifiers on Imbalanced Datasets.
     PLOS ONE. 2015;10(3):e0118432. doi:10.1371/journal.pone.0118432
 
     If the datasets have different number of examples, the baseline PR curve will not be plotted.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports:
-            my_performance_report: PerformanceOverview
+        definitions:
+            reports:
+                my_performance_report: PerformanceOverview
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return PerformanceOverview(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/CVFeaturePerformance.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,32 +16,34 @@
 
 class CVFeaturePerformance(TrainMLModelReport):
     """
     This report plots the average training vs test performance w.r.t. given encoding parameter which is explicitly set
     in the feature attribute. It can be used only in combination with TrainMLModel instruction and can be only specified under 'reports'
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - feature: name of the encoder parameter w.r.t. which the performance across training and test will be shown. Possible values depend
       on the encoder on which it is used.
 
     - is_feature_axis_categorical (bool): if the x-axis of the plot where features are shown should be categorical; alternatively it is
       automatically determined based on the feature values
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        report1:
-            CVFeaturePerformance:
-                feature: p_value_threshold # parameter value of SequenceAbundance encoder
-                is_feature_axis_categorical: True # show x-axis as categorical
+        definitions:
+            reports:
+                report1:
+                    CVFeaturePerformance:
+                        feature: p_value_threshold # parameter value of SequenceAbundance encoder
+                        is_feature_axis_categorical: True # show x-axis as categorical
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return CVFeaturePerformance(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/DiseaseAssociatedSequenceCVOverlap.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,29 +30,30 @@
 
         overlap(X,Y) = \\frac{|X \\cap Y|}{min(|X|, |Y|)} x 100
 
     For details, see Greiff V, Menzel U, Miho E, et al. Systems Analysis Reveals High Genetic and Antigen-Driven Predetermination of Antibody
     Repertoires throughout B Cell Development. Cell Reports. 2017;19(7):1467-1478. doi:10.1016/j.celrep.2017.04.054.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - compare_in_selection (bool): whether to compute the overlap over the inner loop of the nested CV - the sequence overlap is shown across CV
       folds for the model chosen as optimal within that selection
 
     - compare_in_assessment (bool): whether to compute the overlap over the optimal models in the outer loop of the nested CV
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports: # the report is defined with all other reports under definitions/reports
-            my_overlap_report: DiseaseAssociatedSequenceCVOverlap # report has no parameters
+        definitions:
+            reports:
+                my_overlap_report: DiseaseAssociatedSequenceCVOverlap # report has no parameters
 
     """
     COMPATIBLE_ENCODERS = (SequenceAbundanceEncoder, CompAIRRSequenceAbundanceEncoder, KmerAbundanceEncoder)
 
     @classmethod
     def build_object(cls, **kwargs):
         return DiseaseAssociatedSequenceCVOverlap(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/MLSettingsPerformance.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,29 +22,31 @@
     The performances are grouped by label (horizontal panels) encoding (vertical panels) and ML method (bar color).
     When multiple data splits are used, the average performance over the data splits is shown with an error bar
     representing the standard deviation.
 
     This report can be used only with TrainMLModel instruction under 'reports'.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - single_axis_labels (bool): whether to use single axis labels. Note that using single axis labels makes the figure unsuited for rescaling, as the label position is given in a fixed distance from the axis. By default, single_axis_labels is False, resulting in standard plotly axis labels.
 
     - x_label_position (float): if single_axis_labels is True, this should be an integer specifying the x axis label position relative to the x axis. The default value for label_position is -0.1.
 
     - y_label_position (float): same as x_label_position, but for the y-axis.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_hp_report: MLSettingsPerformance
+        definitions:
+            reports:
+                my_hp_report: MLSettingsPerformance
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         location = "MLSettingsPerformance"
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/ROCCurveSummary.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 class ROCCurveSummary(TrainMLModelReport):
     """
     This report plots ROC curves for all trained ML settings ([preprocessing], encoding, ML model) in the outer loop of cross-validation in the
     :ref:`TrainMLModel` instruction. If there are multiple splits in the outer loop, this report will make one plot per split. This report is
     defined only for binary classification. If there are multiple labels defined in the instruction, each label has to have two classes to be included
     in this report.
 
-    Specification arguments: there are no arguments for this report.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-    reports:
-        my_roc_summary_report: ROCCurveSummary
+        definitions:
+            reports:
+                my_roc_summary_report: ROCCurveSummary
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
         return ROCCurveSummary(**kwargs)
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/ReferenceSequenceOverlap.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,44 +25,45 @@
     :py:obj:`~immuneML.encodings.abundance_encoding.SequenceAbundanceEncoder.SequenceAbundanceEncoder`,
     :py:obj:`~immuneML.encodings.abundance_encoding.CompAIRRSequenceAbundanceEncoder.CompAIRRSequenceAbundanceEncoder` or
     :py:obj:`~immuneML.encodings.abundance_encoding.KmerAbundanceEncoder.KmerAbundanceEncoder` to
     a list of reference sequences. It outputs a Venn diagram and a list of sequences found both in the encoder and reference list.
 
     The report compares the sequences by their sequence content and the additional comparison_attributes (such as V or J gene), as specified by the user.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - reference_path (str): path to the reference file in csv format which contains one entry per row and has columns that correspond to the attributes
       listed under comparison_attributes argument
 
     - comparison_attributes (list): list of attributes to use for comparison; all of them have to be present in the reference file where they should
       be the names of the columns
 
     - label (str): name of the label for which the reference sequences/k-mers should be compared to the model; if none, it takes the one label from the
       instruction; if it is none and multiple labels were specified for the instruction, the report will not be generated
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        reports: # the report is defined with all other reports under definitions/reports
-            my_reference_overlap_report:
-                ReferenceSequenceOverlap:
-                    reference_path: reference_sequences.csv  # example usage with SequenceAbundanceEncoder or CompAIRRSequenceAbundanceEncoder
-                    comparison_attributes:
-                        - sequence_aa
-                        - v_call
-                        - j_call
-            my_reference_overlap_report_with_kmers:
-                ReferenceSequenceOverlap:
-                    reference_path: reference_kmers.csv  # example usage with KmerAbundanceEncoder
-                    comparison_attributes:
-                        - k-mer
+        definitions:
+            reports:
+                my_reference_overlap_report:
+                    ReferenceSequenceOverlap:
+                        reference_path: reference_sequences.csv  # example usage with SequenceAbundanceEncoder or CompAIRRSequenceAbundanceEncoder
+                        comparison_attributes:
+                            - sequence_aa
+                            - v_call
+                            - j_call
+                my_reference_overlap_report_with_kmers:
+                    ReferenceSequenceOverlap:
+                        reference_path: reference_kmers.csv  # example usage with KmerAbundanceEncoder
+                        comparison_attributes:
+                            - k-mer
 
     """
 
     @classmethod
     def build_object(cls, **kwargs):
 
         ParameterValidator.assert_keys(kwargs.keys(), ['reference_path', 'comparison_attributes', 'name', 'label'], ReferenceSequenceOverlap.__name__,
```

### Comparing `immuneML-3.0.0a3/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py` & `immuneml-3.0.0a4/immuneML/reports/train_ml_model_reports/TrainMLModelReport.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,26 +16,23 @@
 
         my_instruction:
             type: TrainMLModel
             reports:
                 - my_train_ml_model_report
             # other parameters...
     """
+    DOCS_TITLE = "Train ML model reports"
 
     def __init__(self, name: str = None, state: TrainMLModelState = None, label: Label = None, result_path: Path = None, number_of_processes: int = 1):
         '''
         The arguments defined below are set at runtime by the instruction.
 
         Concrete classes inheriting TrainMLModelReport may include additional parameters that will be set by the user in the form of input arguments.
         name (str): user-defined name of the report used in the HTML overview automatically generated by the platform
         state (TrainMLModelState): a state object that includes all the information, trained models, encodings and datasets from the nested cross-validation procedure used to train the optimal model.
         result_path (Path): location where the report results will be stored
         number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
         '''
-        super().__init__(name, number_of_processes)
+        super().__init__(name=name, result_path=result_path, number_of_processes=number_of_processes)
         self.state = state
-        self.result_path = result_path
         self.label = label
 
-    @staticmethod
-    def get_title():
-        return "Train ML model reports"
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/LigoSimState.py` & `immuneml-3.0.0a4/immuneML/simulation/LigoSimState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/SimConfig.py` & `immuneml-3.0.0a4/immuneML/simulation/SimConfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 from immuneML.simulation.SimConfigItem import SimConfigItem
 from immuneML.simulation.simulation_strategy.SimulationStrategy import SimulationStrategy
 
 
 @dataclass
 class SimConfig:
     """
-    Defines all parameters of the simulation.
+    The simulation config defines all parameters of the simulation.
+    It can contain one or more simulation config items, which define groups of repertoires or receptors
+    that have the same simulation parameters, such as signals, generative model, clonal frequencies, and noise parameters.
 
-    Specification arguments:
+
+    **Specification arguments:**
 
     - sim_items (dict): a list of SimConfigItems defining individual units of simulation
 
     - is_repertoire (bool): whether the simulation is on a repertoire (person) or sequence/receptor level
 
     - paired: if the simulation should output paired data, this parameter should contain a list of a list of sim_item pairs referenced by name that should be combined; if paired data is not needed, then it should be False
 
@@ -29,36 +32,38 @@
 
     - remove_seqs_with_signals (bool): if true, it explicitly controls the proportions of signals in sequences and removes any accidental occurrences
 
     - species (str): species that the sequences come from; used to select correct genes to export full length sequences; default is 'human'
 
     - implanting_scaling_factor (int): determines in how many receptors to implant the signal in reach iteration; this is computed as number_of_receptors_needed_for_signal * implanting_scaling_factor; useful when using Implanting simulation strategy in combination with importance sampling, since the generation probability of some receptors with implanted signals might be very rare and those receptors might end up not being kept often with importance sampling; this parameter is only used when keep_p_gen_dist is set to True
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent-with-spaces
     .. code-block:: yaml
 
-      simulations:
-        sim1:
-          is_repertoire: false
-          paired: false
-          sequence_type: amino_acid
-          simulation_strategy: RejectionSampling
-          sim_items:
-            sim_item1: # group of sequences with same simulation params
-              generative_model:
-                chain: beta
-                default_model_name: humanTRB
-                model_path: null
-                type: OLGA
-              number_of_examples: 100
-              seed: 1002
-              signals:
-               signal1: 1
+        definitions:
+            simulations:
+                sim1:
+                    is_repertoire: false
+                    paired: false
+                    sequence_type: amino_acid
+                    simulation_strategy: RejectionSampling
+                    sim_items:
+                        sim_item1: # group of sequences with same simulation params
+                            generative_model:
+                                chain: beta
+                                default_model_name: humanTRB
+                                model_path: null
+                                type: OLGA
+                            number_of_examples: 100
+                            seed: 1002
+                            signals:
+                                signal1: 1
 
     """
     sim_items: List[SimConfigItem] = None
     identifier: str = None
     is_repertoire: bool = None
     paired: Union[bool, List[List[str]]] = None
     sequence_type: SequenceType = None
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/SimConfigItem.py` & `immuneml-3.0.0a4/immuneML/simulation/SimConfigItem.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from immuneML.ml_methods.generative_models.GenerativeModel import GenerativeModel
 from immuneML.simulation.implants.Signal import Signal, SignalPair
 
 
 @dataclass
 class SimConfigItem:
     """
-    When performing a simulation, one or more simulation config items can be specified. Config items define groups of
-    repertoires or receptors that have the same simulation parameters, such as signals, generative model, clonal
-    frequencies, noise parameters.
+    When performing a simulation, one or more simulation config items can be specified.
+    Config items define groups of repertoires or receptors that have the same simulation parameters,
+    such as signals, generative model, clonal frequencies, noise parameters.
 
 
-    Specification arguments:
+    **Specification arguments:**
 
     - signals (dict): signals for the simulation item and the proportion of sequences in the repertoire that will have the given signal. For receptor-level simulation, the proportion will always be 1.
 
     - is_noise (bool): indicates whether the implanting should be regarded as noise; if it is True, the signals will be implanted as specified, but the repertoire/receptor in question will have negative class.
 
     - generative_model: parameters of the generative model, including its type, path to the model; currently supported models are OLGA and ExperimentalImport
 
@@ -43,50 +43,51 @@
     .. indent with spaces
     .. code-block:: yaml
 
         sequence_len_limits:
             min: 4 # keep sequences of length 4 and longer
             max: -1 # no limit on the max length of the sequences
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        simulations: # definitions of simulations should be under key simulations in the definitions part of the specification
-            # one simulation with multiple implanting objects, a part of definition section
-            my_simulation:
-                sim_item1:
-                    number_of_examples: 10
-                    seed: null # don't use seed
-                    receptors_in_repertoire_count: 100
-                    generative_model:
-                        chain: beta
-                        default_model_name: humanTRB
-                        model_path: null
-                        type: OLGA
-                    signals:
-                        my_signal: 0.25
-                        my_signal2: 0.01
-                        my_signal__my_signal2: 0.02 # my_signal and my_signal2 will co-occur in 2% of the receptors in all 10 repertoires
-                sim_item2:
-                    number_of_examples: 5
-                    receptors_in_repertoire_count: 150
-                    seed: 10 #
-                    generative_model:
-                        chain: beta
-                        default_model_name: humanTRB
-                        model_path: null
-                        type: OLGA
-                    signals:
-                        my_signal: 0.75
-                    default_clonal_frequency:
-                        a: 2
-                    sequence_len_limits:
-                        min: 3
+        definitions:
+            simulations: # definitions of simulations should be under key simulations in the definitions part of the specification
+                # one simulation with multiple implanting objects, a part of definition section
+                my_simulation:
+                    sim_item1:
+                        number_of_examples: 10
+                        seed: null # don't use seed
+                        receptors_in_repertoire_count: 100
+                        generative_model:
+                            chain: beta
+                            default_model_name: humanTRB
+                            model_path: null
+                            type: OLGA
+                        signals:
+                            my_signal: 0.25
+                            my_signal2: 0.01
+                            my_signal__my_signal2: 0.02 # my_signal and my_signal2 will co-occur in 2% of the receptors in all 10 repertoires
+                    sim_item2:
+                        number_of_examples: 5
+                        receptors_in_repertoire_count: 150
+                        seed: 10 #
+                        generative_model:
+                            chain: beta
+                            default_model_name: humanTRB
+                            model_path: null
+                            type: OLGA
+                        signals:
+                            my_signal: 0.75
+                        default_clonal_frequency:
+                            a: 2
+                        sequence_len_limits:
+                            min: 3
 
 
     """
 
     signal_proportions: Dict[Union[Signal, SignalPair], float]
     name: str = ""
     is_noise: bool = False
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py` & `immuneml-3.0.0a4/immuneML/simulation/dataset_generation/RandomDatasetGenerator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/implants/LigoPWM.py` & `immuneml-3.0.0a4/immuneML/simulation/implants/LigoPWM.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 @dataclass
 class LigoPWM(Motif):
     """
     Motifs defined by a positional weight matrix and using bionumpy's PWM internally.
     For more details on bionumpy's implementation of PWM, as well as for supported formats,
     see the documentation at https://bionumpy.github.io/bionumpy/tutorials/position_weight_matrix.html.
 
-    Arguments:
+    **Specification arguments:**
 
     - file_path: path to the file where the PWM is stored
 
     - threshold (float): when matching PWM to a sequence, this is the threshold to consider the sequence as containing the motif
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        motifs:
-            my_custom_pwm: # this will be the identifier of the motif
-                file_path: my_pwm_1.csv
-                threshold: 2
+        definitions:
+            motifs:
+                my_custom_pwm: # this will be the identifier of the motif
+                    file_path: my_pwm_1.csv
+                    threshold: 2
 
     """
     file_path: Path
     pwm_matrix: bnp_PWM  # with log-likelihood
     threshold: float
 
     @classmethod
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/implants/MotifInstance.py` & `immuneml-3.0.0a4/immuneML/simulation/implants/MotifInstance.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/implants/SeedMotif.py` & `immuneml-3.0.0a4/immuneML/simulation/implants/SeedMotif.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,52 +13,53 @@
 
 
 @dataclass
 class SeedMotif(Motif):
     """
     Describes motifs by seed, possible gaps, allowed hamming distances, positions that can be changed and what they can be changed to.
 
-    Arguments:
+    **Specification arguments:**
 
     - seed (str): An amino acid sequence that represents the basic motif seed. All implanted motifs correspond to the seed, or a modified version thereof, as specified in its instantiation strategy. If this argument is set, seed_chain1 and seed_chain2 arguments are not used.
 
     - min_gap (int): The minimum gap length, in case the original seed contains a gap.
 
     - max_gap (int): The maximum gap length, in case the original seed contains a gap.
 
     - hamming_distance_probabilities (dict): The probability of modifying the given seed with each number of modifications. The keys represent the number of modifications (hamming distance) between the original seed and the implanted motif, and the values represent the probabilities for the respective number of modifications. For example {0: 0.7, 1: 0.3} means that 30% of the time one position will be modified, and the remaining 70% of the time the motif will remain unmodified with respect to the seed. The values of hamming_distance_probabilities must sum to 1.
 
     - position_weights (dict): A dictionary containing the relative probabilities of choosing each position for hamming distance modification. The keys represent the position in the seed, where counting starts at 0. If the index of a gap is specified in position_weights, it will be removed. The values represent the relative probabilities for modifying each position when it gets selected for modification. For example {0: 0.6, 1: 0, 2: 0.4} means that when a sequence is selected for a modification (as specified in hamming_distance_probabilities), then 60% of the time the amino acid at index 0 is modified, and the remaining 40% of the time the amino acid at index 2. If the values of position_weights do not sum to 1, the remainder will be redistributed over all positions, including those not specified.
 
     - alphabet_weights (dict): A dictionary describing the relative probabilities of choosing each amino acid for hamming distance modification. The keys of the dictionary represent the amino acids and the values are the relative probabilities for choosing this amino acid. If the values of alphabet_weights do not sum to 1, the remainder will be redistributed over all possible amino acids, including those not specified.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        motifs:
-            # examples for single chain receptor data
-            my_simple_motif: # this will be the identifier of the motif
-                seed: AAA # motif is always AAA
-            my_gapped_motif:
-                seed: AA/A # this motif can be AAA, AA_A, CAA, CA_A, DAA, DA_A, EAA, EA_A
-                min_gap: 0
-                max_gap: 1
-                hamming_distance_probabilities: # it can have a max of 1 substitution
-                    0: 0.7
-                    1: 0.3
-                position_weights: # note that index 2, the position of the gap, is excluded from position_weights
-                    0: 1 # only first position can be changed
-                    1: 0
-                    3: 0
-                alphabet_weights: # the first A can be replaced by C, D or E
-                    C: 0.4
-                    D: 0.4
-                    E: 0.2
+        definitions:
+            motifs:
+                # examples for single chain receptor data
+                my_simple_motif: # this will be the identifier of the motif
+                    seed: AAA # motif is always AAA
+                my_gapped_motif:
+                    seed: AA/A # this motif can be AAA, AA_A, CAA, CA_A, DAA, DA_A, EAA, EA_A
+                    min_gap: 0
+                    max_gap: 1
+                    hamming_distance_probabilities: # it can have a max of 1 substitution
+                        0: 0.7
+                        1: 0.3
+                    position_weights: # note that index 2, the position of the gap, is excluded from position_weights
+                        0: 1 # only first position can be changed
+                        1: 0
+                        3: 0
+                    alphabet_weights: # the first A can be replaced by C, D or E
+                        C: 0.4
+                        D: 0.4
+                        E: 0.2
 
     """
 
     seed: str = None
     min_gap: int = 0
     max_gap: int = 0
     hamming_distance_probabilities: dict = None
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/implants/Signal.py` & `immuneml-3.0.0a4/immuneML/simulation/implants/Signal.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 from immuneML.simulation.implants.Motif import Motif
 from immuneML.simulation.implants.MotifInstance import MotifInstanceGroup
 
 
 @dataclass
 class Signal:
     """
-    This class represents the simulated signal.
-    A signal is represented by a list of motifs, and optionally, position weights showing where one of the motifs of the signal can
-    occur in a sequence.
+    A signal represents a collection of motifs, and optionally, position weights showing where one
+    of the motifs of the signal can occur in a sequence.
+    The signals are defined under :code:`definitions/signals`.
 
     A signal is associated with a metadata label, which is assigned to a receptor or repertoire.
     For example antigen-specific/disease-associated (receptor) or diseased (repertoire).
 
     .. note:: IMGT positions
 
         To use sequence position weights, IMGT positions should be explicitly specified as strings, under quotation marks, to allow for all positions to be properly distinguished.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - motifs (list): A list of the motifs associated with this signal, either defined by seed or by position weight matrix. Alternatively, it can be a list of a list of motifs, in which case the motifs in the same sublist (max 2 motifs) have to co-occur in the same sequence
 
     - sequence_position_weights (dict): a dictionary specifying for each IMGT position in the sequence how likely it is for the signal to be there. If the position is not present in the sequence, the probability of the signal occurring at that position will be redistributed to other positions with probabilities that are not explicitly set to 0 by the user.
 
     - v_call (str): V gene with allele if available that has to co-occur with one of the motifs for the signal to exist; can be used in combination with rejection sampling, or full sequence implanting, otherwise ignored; to match in a sequence for rejection sampling, it is checked if this value is contained in the same field of generated sequence;
 
@@ -47,37 +47,38 @@
     .. code-block:: yaml
 
       clonal_frequency:
         a: 2 # shape parameter of the distribution
         loc: 0 # 0 by default but can be used to shift the distribution
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. code-block:: yaml
 
-        signals:
-            my_signal:
-                motifs:
-                    - my_simple_motif
-                    - my_gapped_motif
-                sequence_position_weights:
-                    '109': 0.5
-                    '110': 0.5
-                v_call: TRBV1
-                j_call: TRBJ1
-                clonal_frequency:
-                    a: 2
-                    loc: 0
-            signal_with_custom_func:
-                source_file: signal_func.py
-                is_present_func: is_signal_present
-                clonal_frequency:
-                    a: 2
-                    loc: 0
+        definitions:
+            signals:
+                my_signal:
+                    motifs:
+                        - my_simple_motif
+                        - my_gapped_motif
+                    sequence_position_weights:
+                        '109': 0.5
+                        '110': 0.5
+                    v_call: TRBV1
+                    j_call: TRBJ1
+                    clonal_frequency:
+                        a: 2
+                        loc: 0
+                signal_with_custom_func:
+                    source_file: signal_func.py
+                    is_present_func: is_signal_present
+                    clonal_frequency:
+                        a: 2
+                        loc: 0
 
     """
     id: str
     motifs: List[Union[Motif, List[Motif]]] = None
     sequence_position_weights: dict = None
     v_call: str = None
     j_call: str = None
```

### Comparing `immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/ImplantingStrategy.py` & `immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/ImplantingStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/RejectionSamplingStrategy.py` & `immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/RejectionSamplingStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/simulation_strategy/SimulationStrategy.py` & `immuneml-3.0.0a4/immuneML/simulation/simulation_strategy/SimulationStrategy.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/util/bnp_util.py` & `immuneml-3.0.0a4/immuneML/simulation/util/bnp_util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/util/igor_helper.py` & `immuneml-3.0.0a4/immuneML/simulation/util/igor_helper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/simulation/util/util.py` & `immuneml-3.0.0a4/immuneML/simulation/util/util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/AdaptiveImportHelper.py` & `immuneml-3.0.0a4/immuneML/util/AdaptiveImportHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/CompAIRRHelper.py` & `immuneml-3.0.0a4/immuneML/util/CompAIRRHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/EncoderHelper.py` & `immuneml-3.0.0a4/immuneML/util/EncoderHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -49,18 +49,14 @@
                                    sequence_batch_size, params.result_path)
 
         comp_data.process_dataset(dataset)
 
         return comp_data
 
     @staticmethod
-    def store(encoded_dataset, params: EncoderParams):
-        ImmuneMLExporter.export(encoded_dataset, params.result_path)
-
-    @staticmethod
     def sync_encoder_with_cache(cache_params: tuple, encoder_memo_func, encoder, param_names):
         encoder_cache_params = tuple((key, val) for key, val in dict(cache_params).items() if key != 'learn_model')
         encoder_cache_params = (encoder_cache_params, "encoder")
 
         encoder_from_cache = CacheHandler.memo_by_params(encoder_cache_params, encoder_memo_func)
         for param in param_names:
             setattr(encoder, param, copy.deepcopy(encoder_from_cache[param]))
@@ -71,25 +67,44 @@
     def check_dataset_type_available_in_mapping(dataset, class_name):
         if dataset.__class__.__name__ not in class_name.dataset_mapping.keys():
             raise ValueError(f"{class_name.__name__}: this encoder is not defined for dataset of type {dataset.__class__.__name__}. "
                              f"Valid dataset types for this encoder are: {', '.join(list(class_name.dataset_mapping.keys()))}")
 
     @staticmethod
     def encode_element_dataset_labels(dataset: ElementDataset, label_config: LabelConfiguration):
-
+        '''Automatically generates the encoded labels for an ElementDataset (= SequenceDataset or ReceptorDataset)'''
         labels = {name: [] for name in label_config.get_labels_by_name()}
 
         for sequence in dataset.get_data():
             for label_name in label_config.get_labels_by_name():
                 label = sequence.get_attribute(label_name)
                 labels[label_name].append(label)
 
         return labels
 
     @staticmethod
+    def encode_repertoire_dataset_labels(dataset: RepertoireDataset, label_config: LabelConfiguration):
+        '''Automatically generates the encoded labels for a RepertoireDataset'''
+        label_names = label_config.get_labels_by_name()
+        return dataset.get_metadata(label_names)
+
+    @staticmethod
+    def encode_dataset_labels(dataset: Dataset, label_config: LabelConfiguration, encode_labels: bool = True):
+        '''Automatically generates the encoded labels for a Dataset.
+        This contains labels in the following format: {'label_name': ['label_class1', 'label_class2', 'label_class2']}
+        where the inner list(s) contain the class label for each example in the dataset'''
+        if not encode_labels:
+            return None
+
+        if isinstance(dataset, RepertoireDataset):
+            return EncoderHelper.encode_repertoire_dataset_labels(dataset, label_config)
+        else:
+            return EncoderHelper.encode_element_dataset_labels(dataset, label_config)
+
+    @staticmethod
     def check_positive_class_labels(label_config: LabelConfiguration, location: str):
         '''
         Performs checks for Encoders that explicitly predict a positive class. These Encoders can only be trained for a
         single binary label at a time.
         '''
 
         labels = label_config.get_label_objects()
```

### Comparing `immuneML-3.0.0a3/immuneML/util/ExporterHelper.py` & `immuneml-3.0.0a4/immuneML/util/ExporterHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/FilenameHandler.py` & `immuneml-3.0.0a4/immuneML/util/FilenameHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/ImportHelper.py` & `immuneml-3.0.0a4/immuneML/util/ImportHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/KmerHelper.py` & `immuneml-3.0.0a4/immuneML/util/KmerHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/Logger.py` & `immuneml-3.0.0a4/immuneML/util/Logger.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/MotifPerformancePlotHelper.py` & `immuneml-3.0.0a4/immuneML/util/MotifPerformancePlotHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/NameBuilder.py` & `immuneml-3.0.0a4/immuneML/util/NameBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/NumpyHelper.py` & `immuneml-3.0.0a4/immuneML/util/NumpyHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/ParameterValidator.py` & `immuneml-3.0.0a4/immuneML/util/ParameterValidator.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/PathBuilder.py` & `immuneml-3.0.0a4/immuneML/util/PathBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/PositionHelper.py` & `immuneml-3.0.0a4/immuneML/util/PositionHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/ReflectionHandler.py` & `immuneml-3.0.0a4/immuneML/util/ReflectionHandler.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/RepertoireBuilder.py` & `immuneml-3.0.0a4/immuneML/util/RepertoireBuilder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/SequenceAnalysisHelper.py` & `immuneml-3.0.0a4/immuneML/util/SequenceAnalysisHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/SignificantFeaturesHelper.py` & `immuneml-3.0.0a4/immuneML/util/SignificantFeaturesHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/StringHelper.py` & `immuneml-3.0.0a4/immuneML/util/StringHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/util/TCRdistHelper.py` & `immuneml-3.0.0a4/immuneML/util/TCRdistHelper.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/GenModelInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/GenModelInstruction.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/MLProcess.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/MLProcess.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                  label_config: LabelConfiguration = None, report_context: dict = None, hp_setting: HPSetting = None, example_weighting: ExampleWeightingStrategy = None):
         self.train_dataset = train_dataset
         self.test_dataset = test_dataset
         self.label = label
         self.label_config = label_config
         self.method = copy.deepcopy(hp_setting.ml_method)
         self.path = PathBuilder.build(path) if path is not None else None
-        self.ml_details_path = path / "ml_details.yaml" if path is not None else None
         self.ml_settings_export_path = path / "ml_settings_config" if path is not None else None
         self.ml_score_path = path / "ml_score.csv" if path is not None else None
         self.train_predictions_path = path / "train_predictions.csv" if path is not None else None
         self.test_predictions_path = path / "test_predictions.csv" if path is not None else None
         self.report_path = PathBuilder.build(path / "reports") if path is not None else None
         self.number_of_processes = number_of_processes
         assert all([isinstance(metric, ClassificationMetric) for metric in metrics]), \
@@ -56,15 +55,14 @@
         self.report_context = report_context
         self.hp_setting = copy.deepcopy(hp_setting)
         self.example_weighting = example_weighting
 
     def _set_paths(self):
         if self.path is None:
             raise RuntimeError("MLProcess: path is not set, stopping execution...")
-        self.ml_details_path = self.path / "ml_details.yaml"
         self.ml_settings_export_path = self.path / "ml_settings_config"
         self.ml_score_path = self.path / "ml_score.csv"
         self.train_predictions_path = self.path / "train_predictions.csv"
         self.test_predictions_path = self.path / "test_predictions.csv"
         self.report_path = PathBuilder.build(self.path / "reports")
 
     def run(self, split_index: int) -> HPItem:
@@ -97,15 +95,14 @@
     def _train_method(self, dataset) -> MLMethod:
         method = MLMethodTrainer.run(MLMethodTrainerParams(
             method=copy.deepcopy(self.hp_setting.ml_method),
             result_path=self.path / "ml_method",
             dataset=dataset,
             label=self.label,
             train_predictions_path=self.train_predictions_path,
-            ml_details_path=self.ml_details_path,
             model_selection_cv=self.hp_setting.ml_params["model_selection_cv"],
             model_selection_n_folds=self.hp_setting.ml_params["model_selection_n_folds"],
             cores_for_training=self.number_of_processes,
             optimization_metric=self.optimization_metric.name.lower()
         ))
         return method
 
@@ -127,18 +124,18 @@
 
             encoding_test_results = ReportUtil.run_encoding_reports(encoded_test_dataset, self.encoding_reports, self.report_path / "encoding_test", self.number_of_processes)
 
             model_report_results = ReportUtil.run_ML_reports(encoded_train_dataset, encoded_test_dataset, method, self.ml_reports,
                                                              self.report_path / "ml_method", self.hp_setting, self.label, self.number_of_processes, self.report_context)
 
             hp_item = HPItem(method=method, hp_setting=self.hp_setting, train_predictions_path=self.train_predictions_path,
-                             test_predictions_path=self.test_predictions_path, ml_details_path=self.ml_details_path, train_dataset=self.train_dataset,
+                             test_predictions_path=self.test_predictions_path, train_dataset=self.train_dataset,
                              test_dataset=self.test_dataset, split_index=split_index, model_report_results=model_report_results,
                              encoding_train_results=encoding_train_results, encoding_test_results=encoding_test_results, performance=performance,
                              encoder=self.hp_setting.encoder, ml_settings_export_path=self.ml_settings_export_path)
         else:
             hp_item = HPItem(method=method, hp_setting=self.hp_setting, train_predictions_path=self.train_predictions_path,
-                             test_predictions_path=None, ml_details_path=self.ml_details_path, train_dataset=self.train_dataset,
+                             test_predictions_path=None, train_dataset=self.train_dataset,
                              split_index=split_index, encoding_train_results=encoding_train_results, encoder=self.hp_setting.encoder,
                              ml_settings_export_path=self.ml_settings_export_path)
 
         return hp_item
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/TrainMLModelInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/TrainMLModelInstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,21 @@
     - the outer loop over defined splits of the dataset for performance assessment
 
     - the inner loop over defined hyperparameter space and with cross-validation or train & validation split
       to choose the best hyperparameters.
 
     Optimal model chosen by the inner loop is then retrained on the whole training dataset in the outer loop.
 
-    Note: If you are interested in plotting the performance of all combinations of encodings and ML methods on the test set,
-    consider running the :ref:`MLSettingsPerformance` report as hyperparameter report in the assessment loop.
+    .. note::
 
+        If you are interested in plotting the performance of all combinations of encodings and ML methods on the test set,
+        consider running the :ref:`MLSettingsPerformance` report as hyperparameter report in the assessment loop.
 
-    Specification arguments:
+
+    **Specification arguments:**
 
     - dataset (Dataset): dataset to use for training and assessing the classifier
 
     - hp_strategy (HPOptimizationStrategy): how to search different hyperparameters; common options include grid search, random search. Valid values are objects of any class inheriting :py:obj:`~immuneML.hyperparameter_optimization.strategy.HPOptimizationStrategy.HPOptimizationStrategy`.
 
     - hp_settings (list): a list of combinations of `preprocessing_sequence`, `encoding` and `ml_method`. `preprocessing_sequence` is optional, while `encoding` and `ml_method` are mandatory. These three options (and their parameters) can be optimized over, choosing the highest performing combination.
 
@@ -71,64 +73,65 @@
     - refit_optimal_model (bool): if the final combination of preprocessing-encoding-ML model should be refitted on the full dataset thus providing
       the final model to be exported from instruction; alternatively, train combination from one of the assessment folds will be used
 
     - export_all_models (bool): if set to True, all trained models in the assessment split are exported as .zip files.
       If False, only the optimal model is exported. By default, export_all_models is False.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_nested_cv_instruction: # user-defined name of the instruction
-            type: TrainMLModel # which instruction should be executed
-            settings: # a list of combinations of preprocessing, encoding and ml_method to optimize over
-                - preprocessing: seq1 # preprocessing is optional
-                  encoding: e1 # mandatory field
-                  ml_method: simpleLR # mandatory field
-                - preprocessing: seq1 # the second combination
-                  encoding: e2
-                  ml_method: simpleLR
-            assessment: # outer loop of nested CV
-                split_strategy: random # perform Monte Carlo CV (randomly split the data into train and test)
-                split_count: 1 # how many train/test datasets to generate
-                training_percentage: 0.7 # what percentage of the original data should be used for the training set
-                reports: # reports to execute on training/test datasets, encoded datasets and trained ML methods
-                    data_splits: # list of reports to execute on training/test datasets (before they are encoded)
-                        - rep1
-                    encoding: # list of reports to execute on encoded training/test datasets
-                        - rep2
-                    models: # list of reports to execute on trained ML methods for each assessment CV split
-                        - rep3
-            selection: # inner loop of nested CV
-                split_strategy: k_fold # perform k-fold CV
-                split_count: 5 # how many fold to create: here these two parameters mean: do 5-fold CV
-                reports:
-                    data_splits: # list of reports to execute on training/test datasets (in the inner loop, so these are actually training and validation datasets)
-                        - rep1
-                    models: # list of reports to execute on trained ML methods for each selection CV split
-                        - rep2
-                    encoding: # list of reports to execute on encoded training/test datasets (again, it is training/validation here)
-                        - rep3
-            labels: # list of labels to optimize the classifier for, as given in the metadata for the dataset
-                - celiac:
-                    positive_class: + # if it's binary classification, positive class parameter should be set
-                - T1D # this is not binary label, so no need to specify positive class
-            dataset: d1 # which dataset to use for the nested CV
-            strategy: GridSearch # how to choose the combinations which to test from settings (GridSearch means test all)
-            metrics: # list of metrics to compute for all settings, but these do not influence the choice of optimal model
-                - accuracy
-                - auc
-            reports: # list of reports to execute when nested CV is finished to show overall performance
-                - rep4
-            number_of_processes: 4 # number of parallel processes to create (could speed up the computation)
-            optimization_metric: balanced_accuracy # the metric to use for choosing the optimal model and during training
-            refit_optimal_model: False # use trained model, do not refit on the full dataset
-            export_all_ml_settings: False # only export the optimal setting
+        instructions:
+            my_nested_cv_instruction: # user-defined name of the instruction
+                type: TrainMLModel # which instruction should be executed
+                settings: # a list of combinations of preprocessing, encoding and ml_method to optimize over
+                    - preprocessing: seq1 # preprocessing is optional
+                      encoding: e1 # mandatory field
+                      ml_method: simpleLR # mandatory field
+                    - preprocessing: seq1 # the second combination
+                      encoding: e2
+                      ml_method: simpleLR
+                assessment: # outer loop of nested CV
+                    split_strategy: random # perform Monte Carlo CV (randomly split the data into train and test)
+                    split_count: 1 # how many train/test datasets to generate
+                    training_percentage: 0.7 # what percentage of the original data should be used for the training set
+                    reports: # reports to execute on training/test datasets, encoded datasets and trained ML methods
+                        data_splits: # list of reports to execute on training/test datasets (before they are encoded)
+                            - rep1
+                        encoding: # list of reports to execute on encoded training/test datasets
+                            - rep2
+                        models: # list of reports to execute on trained ML methods for each assessment CV split
+                            - rep3
+                selection: # inner loop of nested CV
+                    split_strategy: k_fold # perform k-fold CV
+                    split_count: 5 # how many fold to create: here these two parameters mean: do 5-fold CV
+                    reports:
+                        data_splits: # list of reports to execute on training/test datasets (in the inner loop, so these are actually training and validation datasets)
+                            - rep1
+                        models: # list of reports to execute on trained ML methods for each selection CV split
+                            - rep2
+                        encoding: # list of reports to execute on encoded training/test datasets (again, it is training/validation here)
+                            - rep3
+                labels: # list of labels to optimize the classifier for, as given in the metadata for the dataset
+                    - celiac:
+                        positive_class: + # if it's binary classification, positive class parameter should be set
+                    - T1D # this is not binary label, so no need to specify positive class
+                dataset: d1 # which dataset to use for the nested CV
+                strategy: GridSearch # how to choose the combinations which to test from settings (GridSearch means test all)
+                metrics: # list of metrics to compute for all settings, but these do not influence the choice of optimal model
+                    - accuracy
+                    - auc
+                reports: # list of reports to execute when nested CV is finished to show overall performance
+                    - rep4
+                number_of_processes: 4 # number of parallel processes to create (could speed up the computation)
+                optimization_metric: balanced_accuracy # the metric to use for choosing the optimal model and during training
+                refit_optimal_model: False # use trained model, do not refit on the full dataset
+                export_all_ml_settings: False # only export the optimal setting
 
     """
 
     def __init__(self, dataset, hp_strategy: HPOptimizationStrategy, hp_settings: list, assessment: SplitConfig, selection: SplitConfig,
                  metrics: set, optimization_metric: ClassificationMetric, label_configuration: LabelConfiguration, path: Path = None, context: dict = None,
                  number_of_processes: int = 1, reports: dict = None, name: str = None, refit_optimal_model: bool = False,
                  export_all_ml_settings: bool = False, example_weighting: ExampleWeightingStrategy = None):
@@ -249,11 +252,11 @@
             "optimization_metric (Metric)": "optimization_metric",
             "label_configuration (LabelConfiguration)": "labels (list)",
             "data_reports": "reports",
             "a list of metrics": f"a list of metrics ({valid_values})",
             "a metric to use for optimization": f"a metric to use for optimization (one of {valid_values})",
             "Valid values are objects of any class inheriting :py:obj:`~immuneML.hyperparameter_optimization.strategy."
             "HPOptimizationStrategy.HPOptimizationStrategy`.": f"Valid values are: {valid_strategies}.",
-            "the reports to be specified here have to be :py:obj:`~immuneML.reports.train_ml_model_reports.TrainMLModelReport.TrainMLModelReport` reports.": f"the reports that can be provided here are :ref:`{TrainMLModelReport.get_title()}`."
+            "the reports to be specified here have to be :py:obj:`~immuneML.reports.train_ml_model_reports.TrainMLModelReport.TrainMLModelReport` reports.": f"the reports that can be provided here are :ref:`{TrainMLModelReport.DOCS_TITLE}`."
         }
         doc = update_docs_per_mapping(doc, mapping)
         return doc
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/apply_gen_model/ApplyGenModelInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/apply_gen_model/ApplyGenModelInstruction.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,46 @@
 
 class ApplyGenModelState(GenModelState):
     pass
 
 
 class ApplyGenModelInstruction(GenModelInstruction):
     """
-    ApplyGenModel instruction implements applying generative AIRR models on the sequence level.
+    .. note::
 
-    This instruction takes as input a trained model which will be used for generating data and the number of
-    sequences to be generated. It can also produce reports of the applied model and reports of generated
-    sequences.
+        This is an experimental feature
 
-    To train generative model with immuneML, see TrainGenModel instruction.
+    ApplyGenModel instruction implements applying generative AIRR models on the sequence level.
 
-    .. note::
+    This instruction takes as input a trained model (trained in the :ref:`TrainGenModel` instruction)
+    which will be used for generating data and the number of sequences to be generated.
+    It can also produce reports of the applied model and reports of generated sequences.
 
-        This is an experimental feature in version 3.0.0a1.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - gen_examples_count (int): how many examples (sequences, repertoires) to generate from the applied model
 
     - reports (list): list of report ids (defined under definitions/reports) to apply after generating
       gen_examples_count examples; these can be data reports (to be run on generated examples), ML reports (to be run
       on the fitted model)
 
     - config_path (str): path to the trained model in zip format (as provided by TrainGenModel instruction)
 
-    YAML specification:
+    **YAML specification:**
 
     .. highlight:: yaml
     .. code-block:: yaml
 
-        my_apply_gen_model_inst: # user-defined instruction name
-            type: ApplyGenModel
-            gen_examples_count: 100
-            ml_config_path: ./config.zip
-            reports: [data_rep1, ml_rep2]
+        instructions:
+            my_apply_gen_model_inst: # user-defined instruction name
+                type: ApplyGenModel
+                gen_examples_count: 100
+                ml_config_path: ./config.zip
+                reports: [data_rep1, ml_rep2]
 
     """
     def __init__(self, method: GenerativeModel = None, reports: list = None, result_path: Path = None,
                  name: str = None, gen_examples_count: int = None):
         super().__init__(ApplyGenModelState(result_path, name, gen_examples_count), method, reports)
 
     def run(self, result_path: Path) -> GenModelState:
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/ClusteringInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/ClusteringInstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,23 +34,24 @@
     predictions_path: Path = None
     cl_item_report_results: Dict[str, Dict[str, List[ReportResult]]] = None
     clustering_report_results: List[ReportResult] = field(default_factory=list)
 
 
 class ClusteringInstruction(Instruction):
     """
+    .. note::
+
+        This is an experimental feature
+
     Clustering instruction fits clustering methods to the provided encoded dataset and compares the combinations of
     clustering method with its hyperparameters, and encodings across a pre-defined set of metrics. Finally, it
     provides options to include a set of reports to visualize the results.
 
-    .. note::
-
-        This is an experimental feature in version 3.0.0a1.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - dataset (str): name of the dataset to be clustered
 
     - metrics (list): a list of metrics to use for comparison of clustering algorithms and encodings (it can include
       metrics for either internal evaluation if no labels are provided or metrics for external evaluation so that the
       clusters can be compared against a list of predefined labels)
 
@@ -59,31 +60,32 @@
     - clustering_settings (list): a list of combinations of encoding, optional dimensionality reduction algorithm, and
       the clustering algorithm that will be evaluated
 
     - reports (list): a list of reports to be run on the clustering results or the encoded data
 
     - number_of_processes (int): how many processes to use for parallelization
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_clustering_instruction:
-            type: Clustering
-            dataset: d1
-            metrics: [adjusted_rand_score, adjusted_mutual_info_score]
-            labels: [epitope, v_call]
-            clustering_settings:
-                - encoding: e1
-                  dim_reduction: pca
-                  method: k_means1
-                - encoding: e2
-                  method: dbscan
-            reports: [rep1, rep2]
+        instructions:
+            my_clustering_instruction:
+                type: Clustering
+                dataset: d1
+                metrics: [adjusted_rand_score, adjusted_mutual_info_score]
+                labels: [epitope, v_call]
+                clustering_settings:
+                    - encoding: e1
+                      dim_reduction: pca
+                      method: k_means1
+                    - encoding: e2
+                      method: dbscan
+                reports: [rep1, rep2]
 
     """
 
     def __init__(self, dataset: Dataset, metrics: List[str], clustering_settings: List[ClusteringSetting],
                  name: str, label_config: LabelConfiguration = None, reports: List[Report] = None,
                  number_of_processes: int = None):
         self.state = ClusteringState(name, dataset, metrics, clustering_settings, label_config=label_config)
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/clustering/clustering_run_model.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/clustering/clustering_run_model.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/dataset_generation/DatasetExportInstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,41 +12,42 @@
 
 
 class DatasetExportInstruction(Instruction):
     """
     DatasetExport instruction takes a list of datasets as input, optionally applies preprocessing steps, and outputs
     the data in specified formats.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - datasets (list): a list of datasets to export in all given formats
 
     - preprocessing_sequence (list): which preprocessing sequence to use on the dataset(s), this item is optional and does not have to be specified.
       When specified, the same preprocessing sequence will be applied to all datasets.
 
     - exporters (list): a list of formats in which to export the datasets. Valid formats are class names of any
       non-abstract class inheriting :py:obj:`~immuneML.IO.dataset_export.DataExporter.DataExporter`.
 
     - number_of_processes (int): how many processes to use during repertoire export (not used for sequence datasets)
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_dataset_export_instruction: # user-defined instruction name
-            type: DatasetExport # which instruction to execute
-            datasets: # list of datasets to export
-                - my_generated_dataset
-                - my_dataset_from_adaptive
-            preprocessing_sequence: my_preprocessing_sequence
-            number_of_processes: 4
-            export_formats: # list of formats to export the datasets to
-                - AIRR
-                - ImmuneML
+        instructions:
+            my_dataset_export_instruction: # user-defined instruction name
+                type: DatasetExport # which instruction to execute
+                datasets: # list of datasets to export
+                    - my_generated_dataset
+                    - my_dataset_from_adaptive
+                preprocessing_sequence: my_preprocessing_sequence
+                number_of_processes: 4
+                export_formats: # list of formats to export the datasets to
+                    - AIRR
+                    - ImmuneML
 
     """
 
     def __init__(self, datasets: List[Dataset], exporters: List[DataExporter], number_of_processes: int = 1,
                  preprocessing_sequence: List[Preprocessor] = None, result_path: Path = None, name: str = None):
         self.datasets = datasets
         self.exporters = exporters
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisInstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,62 +18,63 @@
     """
     Allows exploratory analysis of different datasets using encodings and reports.
 
     Analysis is defined by a dictionary of ExploratoryAnalysisUnit objects that encapsulate a dataset, an encoding [optional]
     and a report to be executed on the [encoded] dataset. Each analysis specified under `analyses` is completely independent from all
     others.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - analyses (dict): a dictionary of analyses to perform. The keys are the names of different analyses, and the values for each
       of the analyses are:
 
       - dataset: dataset on which to perform the exploratory analysis
 
       - preprocessing_sequence: which preprocessings to use on the dataset, this item is optional and does not have to be specified.
 
       - example_weighting: which example weighting strategy to use before encoding the data, this item is optional and does not have to be specified.
 
       - encoding: how to encode the dataset before running the report, this item is optional and does not have to be specified.
 
       - labels: if encoding is specified, the relevant labels should be specified here.
 
-      - dim_reduction: which dimensionality reduction to apply; this is an experimental feature in version 3.0.0a1
+      - dim_reduction: which dimensionality reduction to apply; this is an experimental feature
 
       - report: which report to run on the dataset. Reports specified here may be of the category :ref:`Data reports` or :ref:`Encoding reports`, depending on whether 'encoding' was specified.
 
     - number_of_processes: (int): how many processes should be created at once to speed up the analysis. For personal
       machines, 4 or 8 is usually a good choice.
 
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_expl_analysis_instruction: # user-defined instruction name
-            type: ExploratoryAnalysis # which instruction to execute
-            analyses: # analyses to perform
-                my_first_analysis: # user-defined name of the analysis
-                    dataset: d1 # dataset to use in the first analysis
-                    preprocessing_sequence: p1 # preprocessing sequence to use in the first analysis
-                    report: r1 # which report to generate using the dataset d1
-                my_second_analysis: # user-defined name of another analysis
-                    dataset: d1 # dataset to use in the second analysis - can be the same or different from other analyses
-                    encoding: e1 # encoding to apply on the specified dataset (d1)
-                    report: r2 # which report to generate in the second analysis
-                    labels: # labels present in the dataset d1 which will be included in the encoded data on which report r2 will be run
-                        - celiac # name of the first label as present in the column of dataset's metadata file
-                        - CMV # name of the second label as present in the column of dataset's metadata file
-                my_third_analysis: # user-defined name of another analysis
-                    dataset: d1 # dataset to use in the second analysis - can be the same or different from other analyses
-                    encoding: e1 # encoding to apply on the specified dataset (d1)
-                    dim_reduction: umap # or None; which dimensionality reduction method to apply to encoded d1
-                    report: r3 # which report to generate in the third analysis
-            number_of_processes: 4 # number of parallel processes to create (could speed up the computation)
+        instructions:
+            my_expl_analysis_instruction: # user-defined instruction name
+                type: ExploratoryAnalysis # which instruction to execute
+                analyses: # analyses to perform
+                    my_first_analysis: # user-defined name of the analysis
+                        dataset: d1 # dataset to use in the first analysis
+                        preprocessing_sequence: p1 # preprocessing sequence to use in the first analysis
+                        report: r1 # which report to generate using the dataset d1
+                    my_second_analysis: # user-defined name of another analysis
+                        dataset: d1 # dataset to use in the second analysis - can be the same or different from other analyses
+                        encoding: e1 # encoding to apply on the specified dataset (d1)
+                        report: r2 # which report to generate in the second analysis
+                        labels: # labels present in the dataset d1 which will be included in the encoded data on which report r2 will be run
+                            - celiac # name of the first label as present in the column of dataset's metadata file
+                            - CMV # name of the second label as present in the column of dataset's metadata file
+                    my_third_analysis: # user-defined name of another analysis
+                        dataset: d1 # dataset to use in the second analysis - can be the same or different from other analyses
+                        encoding: e1 # encoding to apply on the specified dataset (d1)
+                        dim_reduction: umap # or None; which dimensionality reduction method to apply to encoded d1
+                        report: r3 # which report to generate in the third analysis
+                number_of_processes: 4 # number of parallel processes to create (could speed up the computation)
     """
 
     def __init__(self, exploratory_analysis_units: dict, name: str = None):
         assert all(isinstance(unit, ExploratoryAnalysisUnit) for unit in exploratory_analysis_units.values()), \
             ("ExploratoryAnalysisInstruction: not all elements passed to init method are instances of "
              "ExploratoryAnalysisUnit.")
         self.state = ExploratoryAnalysisState(exploratory_analysis_units, name=name)
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/exploratory_analysis/ExploratoryAnalysisUnit.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/FeasibilitySummaryInstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,31 +46,33 @@
     FeasibilitySummary instruction creates a small synthetic dataset and reports summary metrics to show if the simulation with the given
     parameters is feasible. The input parameters to this analysis are the name of the simulation
     (the same that can be used with LigoSim instruction later if feasibility analysis looks acceptable), and the number of sequences to
     simulate for estimating the feasibility.
 
     The feasibility analysis is performed for each generative model separately as these could differ in the analyses that will be reported.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - simulation (str): a name of a simulation object containing a list of SimConfigItem as specified under definitions key; defines how to combine signals with simulated data; specified under definitions
 
     - sequence_count (int): how many sequences to generate to estimate feasibility (default value: 100 000)
 
     - number_of_processes (int): for the parts of the analysis that are possible to parallelize, how many processes to use
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_feasibility_summary: # user-defined name of the instruction
-            type: FeasibilitySummary # which instruction to execute
-            simulation: sim1
-            sequence_count: 10000
+        instructions:
+            my_feasibility_summary: # user-defined name of the instruction
+                type: FeasibilitySummary # which instruction to execute
+                simulation: sim1
+                sequence_count: 10000
 
     """
 
     MIN_SIG_FREQ = 1e-5
     MAX_SIG_FREQ = 0.1
 
     def __init__(self, simulation, sequence_count: int, number_of_processes: int, signals: List[Signal],
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_sim_feasibility/feasibility_reports.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/LigoSimInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/LigoSimInstruction.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,38 +43,40 @@
 
 
 class LigoSimInstruction(Instruction):
     """
     LIgO simulation instruction creates a synthetic dataset from scratch based on the generative model and a set of signals provided by
     the user.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - simulation (str): a name of a simulation object containing a list of SimConfigItem as specified under definitions key; defines how to combine signals with simulated data; specified under definitions
 
     - sequence_batch_size (int): how many sequences to generate at once using the generative model before checking for signals and filtering
 
     - max_iterations (int): how many iterations are allowed when creating sequences
 
     - export_p_gens (bool): whether to compute generation probabilities (if supported by the generative model) for sequences and include them as part of output
 
     - number_of_processes (int): determines how many simulation items can be simulated in parallel
 
-    YAML specification:
+
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_simulation_instruction: # user-defined name of the instruction
-            type: LIgOSim # which instruction to execute
-            simulation: sim1
-            sequence_batch_size: 1000
-            max_iterations: 1000
-            export_p_gens: False
-            number_of_processes: 4
+        instructions:
+            my_simulation_instruction: # user-defined name of the instruction
+                type: LIgOSim # which instruction to execute
+                simulation: sim1
+                sequence_batch_size: 1000
+                max_iterations: 1000
+                export_p_gens: False
+                number_of_processes: 4
 
     """
 
     def __init__(self, simulation: SimConfig, signals: List[Signal], name: str,
                  sequence_batch_size: int, max_iterations: int, number_of_processes: int, export_p_gens: bool = None):
 
         self.state = LigoSimState(simulation=simulation, signals=signals, name=name)
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ligo_simulation/runtime_reports.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ligo_simulation/runtime_reports.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/MLApplicationInstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,39 +73,40 @@
           - 0
         * - e3
           - 1
           - 0.78
           - 0.22
           - 0
 
-    Specification arguments:
+    **Specification arguments:**
 
     - dataset: dataset for which examples need to be classified
 
     - config_path: path to the zip file exported from MLModelTraining instruction (which includes train ML model, encoder, preprocessing etc.)
 
     - number_of_processes (int): how many processes should be created at once to speed up the analysis. For personal machines, 4 or 8 is usually a good choice.
 
     - metrics (list): a list of metrics to compute between the true and predicted classes. These metrics will only be computed when the same label with the same classes is provided for the dataset as the original label the ML setting was trained for.
 
 
-    Specification example for the MLApplication instruction:
+    **YAML specification:**
 
     .. highlight:: yaml
     .. code-block:: yaml
 
-        instruction_name:
-            type: MLApplication
-            dataset: d1
-            config_path: ./config.zip
-            metrics:
-            - accuracy
-            - precision
-            - recall
-            number_of_processes: 4
+        instructions:
+            instruction_name:
+                type: MLApplication
+                dataset: d1
+                config_path: ./config.zip
+                metrics:
+                - accuracy
+                - precision
+                - recall
+                number_of_processes: 4
 
     """
 
     def __init__(self, dataset: Dataset, label_configuration: LabelConfiguration, hp_setting: HPSetting, metrics: List[ClassificationMetric], number_of_processes: int, name: str):
 
         self.state = MLApplicationState(dataset=dataset, hp_setting=hp_setting, label_config=label_configuration, metrics=metrics, pool_size=number_of_processes, name=name)
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/ml_model_application/MLApplicationState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/quickstart.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/quickstart.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/SubsamplingInstruction.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,36 +12,37 @@
 from scripts.specification_util import update_docs_per_mapping
 
 
 class SubsamplingInstruction(Instruction):
     """
     Subsampling is an instruction that subsamples a given dataset and creates multiple smaller dataset according to the parameters provided.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - dataset (str): original dataset which will be used as a basis for subsampling
 
     - subsampled_dataset_sizes (list): a list of dataset sizes (number of examples) each subsampled dataset should have
 
     - dataset_export_formats (list): in which formats to export the subsampled datasets. Valid formats are class names of any non-abstract class inheriting :py:obj:`~immuneML.IO.dataset_export.DataExporter.DataExporter`.
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_subsampling_instruction: # user-defined name of the instruction
-            type: Subsampling # which instruction to execute
-            dataset: my_dataset # original dataset to be subsampled, with e.g., 300 examples
-            subsampled_dataset_sizes: # how large the subsampled datasets should be, one dataset will be created for each list item
-                - 200 # one subsampled dataset with 200 examples (200 repertoires if my_dataset was repertoire dataset)
-                - 100 # the other subsampled dataset will have 100 examples
-            dataset_export_formats: # in which formats to export the subsampled datasets
-                - ImmuneML
-                - AIRR
+        instructions:
+            my_subsampling_instruction: # user-defined name of the instruction
+                type: Subsampling # which instruction to execute
+                dataset: my_dataset # original dataset to be subsampled, with e.g., 300 examples
+                subsampled_dataset_sizes: # how large the subsampled datasets should be, one dataset will be created for each list item
+                    - 200 # one subsampled dataset with 200 examples (200 repertoires if my_dataset was repertoire dataset)
+                    - 100 # the other subsampled dataset will have 100 examples
+                dataset_export_formats: # in which formats to export the subsampled datasets
+                    - ImmuneML
+                    - AIRR
 
     """
 
     def __init__(self, dataset: Dataset, subsampled_dataset_sizes: List[int], dataset_export_formats: list, result_path: Path = None, name: str = None):
         self.state = SubsamplingState(dataset, subsampled_dataset_sizes, dataset_export_formats, result_path, name)
 
     def run(self, result_path: Path):
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/subsampling/SubsamplingState.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/subsampling/SubsamplingState.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/instructions/train_gen_model/TrainGenModelInstruction.py` & `immuneml-3.0.0a4/immuneML/workflows/instructions/train_gen_model/TrainGenModelInstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,53 +8,55 @@
 
 class TrainGenModelState(GenModelState):
     pass
 
 
 class TrainGenModelInstruction(GenModelInstruction):
     """
+    .. note::
+
+        This is an experimental feature
+
     TrainGenModel instruction implements training generative AIRR models on receptor level. Models that can be trained
     for sequence generation are listed under Generative Models section.
 
     This instruction takes a dataset as input which will be used to train a model, the model itself, and the number of
     sequences to generate to illustrate the applicability of the model. It can also produce reports of the fitted model
     and reports of original and generated sequences.
 
-    To use the generative model previously trained with immuneML, see ApplyGenModel instruction.
-
-    .. note::
+    To use the generative model previously trained with immuneML, see :ref:`ApplyGenModel` instruction.
 
-        This is an experimental feature in version 3.0.0a1.
 
-    Specification arguments:
+    **Specification arguments:**
 
     - dataset: dataset to use for fitting the generative model; it has to be defined under definitions/datasets
 
     - method: which model to fit (defined previously under definitions/ml_methods)
 
     - number_of_processes (int): how many processes to use for fitting the model
 
     - gen_examples_count (int): how many examples (sequences, repertoires) to generate from the fitted model
 
     - reports (list): list of report ids (defined under definitions/reports) to apply after fitting a generative model
       and generating gen_examples_count examples; these can be data reports (to be run on generated examples), ML
       reports (to be run on the fitted model)
 
-    YAML specification:
+    **YAML specification:**
 
     .. indent with spaces
     .. code-block:: yaml
 
-        my_train_gen_model_inst: # user-defined instruction name
-            type: TrainGenModel
-            dataset: d1 # defined previously under definitions/datasets
-            model: model1 # defined previously under definitions/ml_methods
-            gen_examples_count: 100
-            number_of_processes: 4
-            reports: [data_rep1, ml_rep2]
+        instructions:
+            my_train_gen_model_inst: # user-defined instruction name
+                type: TrainGenModel
+                dataset: d1 # defined previously under definitions/datasets
+                model: model1 # defined previously under definitions/ml_methods
+                gen_examples_count: 100
+                number_of_processes: 4
+                reports: [data_rep1, ml_rep2]
 
     """
 
     MAX_ELEMENT_COUNT_TO_SHOW = 10
 
     def __init__(self, dataset: Dataset = None, method: GenerativeModel = None, number_of_processes: int = 1,
                  gen_examples_count: int = 100, result_path: Path = None, name: str = None, reports: list = None):
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/DataEncoder.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/DataEncoder.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/DataWeighter.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/DataWeighter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodAssessment.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodAssessment.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodAssessmentParams.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodAssessmentParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodTrainer.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodTrainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                        cores_for_training=input_params.cores_for_training,
                        optimization_metric=input_params.optimization_metric)
 
         return method
 
     @staticmethod
     def store(method: MLMethod, input_params: MLMethodTrainerParams):
-        method.store(input_params.result_path, input_params.dataset.encoded_data.feature_names, input_params.ml_details_path)
+        method.store(input_params.result_path)
         train_predictions = method.predict(input_params.dataset.encoded_data, input_params.label)
         train_proba_predictions = method.predict_proba(input_params.dataset.encoded_data, input_params.label)
 
         df = pd.DataFrame({"example_ids": input_params.dataset.encoded_data.example_ids,
                            f"{input_params.label.name}_predicted_class": train_predictions[input_params.label.name],
                            f"{input_params.label.name}_true_class": input_params.dataset.encoded_data.labels[input_params.label.name]})
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/MLMethodTrainerParams.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/MLMethodTrainerParams.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from immuneML.ml_methods.classifiers.MLMethod import MLMethod
 from immuneML.workflows.steps.StepParams import StepParams
 
 
 class MLMethodTrainerParams(StepParams):
 
     def __init__(self, method: MLMethod, dataset: Dataset, result_path: Path, label: Label, model_selection_cv: bool,
-                 model_selection_n_folds: int, cores_for_training: int, train_predictions_path: Path, ml_details_path: Path,
+                 model_selection_n_folds: int, cores_for_training: int, train_predictions_path: Path,
                  optimization_metric: str):
         self.method = method
         self.result_path = result_path
         self.dataset = dataset
         self.label = label
         self.model_selection_cv = model_selection_cv
         self.model_selection_n_folds = model_selection_n_folds
         self.cores_for_training = cores_for_training
         self.train_predictions_path = train_predictions_path
-        self.ml_details_path = ml_details_path
         self.optimization_metric = optimization_metric
```

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/Step.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/Step.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/DataSplitter.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/DataSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/DataSplitterParams.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/DataSplitterParams.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/ManualSplitter.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/ManualSplitter.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML/workflows/steps/data_splitter/Util.py` & `immuneml-3.0.0a4/immuneML/workflows/steps/data_splitter/Util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/immuneML.egg-info/PKG-INFO` & `immuneml-3.0.0a4/immuneML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immuneML
-Version: 3.0.0a3
+Version: 3.0.0a4
 Summary: immuneML is a software platform for machine learning analysis of immune receptor repertoires.
 Home-page: https://github.com/uio-bmi/immuneML
 Author: immuneML Team
 Author-email: milenpa@student.matnat.uio.no
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.7
```

### Comparing `immuneML-3.0.0a3/immuneML.egg-info/SOURCES.txt` & `immuneml-3.0.0a4/immuneML.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -318,20 +318,20 @@
 immuneML/hyperparameter_optimization/states/HPLabelState.py
 immuneML/hyperparameter_optimization/states/HPSelectionState.py
 immuneML/hyperparameter_optimization/states/TrainMLModelState.py
 immuneML/hyperparameter_optimization/states/__init__.py
 immuneML/hyperparameter_optimization/strategy/GridSearch.py
 immuneML/hyperparameter_optimization/strategy/HPOptimizationStrategy.py
 immuneML/hyperparameter_optimization/strategy/__init__.py
-immuneML/ml_methods/BinaryFeatureClassifier.py
-immuneML/ml_methods/KerasSequenceCNN.py
 immuneML/ml_methods/__init__.py
 immuneML/ml_methods/classifiers/AtchleyKmerMILClassifier.py
+immuneML/ml_methods/classifiers/BinaryFeatureClassifier.py
 immuneML/ml_methods/classifiers/DeepRC.py
 immuneML/ml_methods/classifiers/KNN.py
+immuneML/ml_methods/classifiers/KerasSequenceCNN.py
 immuneML/ml_methods/classifiers/LogisticRegression.py
 immuneML/ml_methods/classifiers/MLMethod.py
 immuneML/ml_methods/classifiers/PrecomputedKNN.py
 immuneML/ml_methods/classifiers/ProbabilisticBinaryClassifier.py
 immuneML/ml_methods/classifiers/RandomForestClassifier.py
 immuneML/ml_methods/classifiers/ReceptorCNN.py
 immuneML/ml_methods/classifiers/SVC.py
@@ -438,15 +438,14 @@
 immuneML/reports/data_reports/RepertoireClonotypeSummary.py
 immuneML/reports/data_reports/SequenceLengthDistribution.py
 immuneML/reports/data_reports/SequencesWithSignificantKmers.py
 immuneML/reports/data_reports/SignificantFeatures.py
 immuneML/reports/data_reports/SignificantKmerPositions.py
 immuneML/reports/data_reports/SimpleDatasetOverview.py
 immuneML/reports/data_reports/VJGeneDistribution.py
-immuneML/reports/data_reports/WeightsDistribution.py
 immuneML/reports/data_reports/__init__.py
 immuneML/reports/encoding_reports/DesignMatrixExporter.py
 immuneML/reports/encoding_reports/DimensionalityReduction.py
 immuneML/reports/encoding_reports/EncodingReport.py
 immuneML/reports/encoding_reports/FeatureComparison.py
 immuneML/reports/encoding_reports/FeatureDistribution.py
 immuneML/reports/encoding_reports/FeatureReport.py
@@ -580,9 +579,12 @@
 immuneML/workflows/steps/data_splitter/DataSplitterParams.py
 immuneML/workflows/steps/data_splitter/LeaveOneOutSplitter.py
 immuneML/workflows/steps/data_splitter/ManualSplitter.py
 immuneML/workflows/steps/data_splitter/Util.py
 immuneML/workflows/steps/data_splitter/__init__.py
 scripts/DocumentatonFormat.py
 scripts/__init__.py
+scripts/check_new_encoder.py
+scripts/check_new_ml_method.py
+scripts/checker_util.py
 scripts/specification_util.py
 scripts/specs_docs_generation.py
```

### Comparing `immuneML-3.0.0a3/scripts/specification_util.py` & `immuneml-3.0.0a4/scripts/specification_util.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/scripts/specs_docs_generation.py` & `immuneml-3.0.0a4/scripts/specs_docs_generation.py`

 * *Files identical despite different names*

### Comparing `immuneML-3.0.0a3/setup.py` & `immuneml-3.0.0a4/setup.py`

 * *Files identical despite different names*

