# Comparing `tmp/stepcount-3.4.0.tar.gz` & `tmp/stepcount-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.4.0.tar", last modified: Sun Apr 14 06:26:52 2024, max compression
+gzip compressed data, was "stepcount-3.5.0.tar", last modified: Fri Apr 26 19:11:28 2024, max compression
```

## Comparing `stepcount-3.4.0.tar` & `stepcount-3.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.861367 stepcount-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-14 06:26:38.000000 stepcount-3.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-14 06:26:52.849367 stepcount-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-14 06:26:38.000000 stepcount-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-14 06:26:38.000000 stepcount-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 06:26:52.861367 stepcount-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-14 06:26:38.000000 stepcount-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.861367 stepcount-3.4.0/src/stepcount/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 06:26:52.861367 stepcount-3.4.0/src/stepcount/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/hmm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/sslmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    22140 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/stepcount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/stepcount/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/stepcount.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-14 06:26:39.000000 stepcount-3.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.266127 stepcount-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-26 19:11:19.000000 stepcount-3.5.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-26 19:11:28.258127 stepcount-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6677 2024-04-26 19:11:19.000000 stepcount-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-26 19:11:19.000000 stepcount-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:11:28.266127 stepcount-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-26 19:11:19.000000 stepcount-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.254127 stepcount-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.266127 stepcount-3.5.0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-26 19:11:28.266127 stepcount-3.5.0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23588 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.258127 stepcount-3.5.0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-26 19:11:19.000000 stepcount-3.5.0/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:11:28.258127 stepcount-3.5.0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 19:11:28.000000 stepcount-3.5.0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-26 19:11:19.000000 stepcount-3.5.0/versioneer.py
```

### Comparing `stepcount-3.4.0/LICENSE.md` & `stepcount-3.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/PKG-INFO` & `stepcount-3.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.4.0
+Version: 3.5.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -19,15 +19,19 @@
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+
+Two underlying models are available:
+- Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
+- Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
 The following instructions make use of Anaconda to meet the minimum requirements:
 
@@ -94,14 +98,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
+Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.4.0/README.md` & `stepcount-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+
+Two underlying models are available:
+- Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
+- Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
 The following instructions make use of Anaconda to meet the minimum requirements:
 
@@ -73,14 +77,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
+Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.4.0/pyproject.toml` & `stepcount-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/setup.py` & `stepcount-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/__init__.py` & `stepcount-3.5.0/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/features.py` & `stepcount-3.5.0/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/hmm_utils.py` & `stepcount-3.5.0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/models.py` & `stepcount-3.5.0/src/stepcount/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,16 +201,16 @@
         (Y_[w_], Z_[w_]) = batch_count_peaks(
             X_[w_],
             self.sample_rate,
             self.lowpass_hz,
             self.find_peaks_params,
             return_peaks=True
         )
-
-        # TODO: should we zero out < steptol windows?
+        # zero-out windows below the threshold
+        Y_[Y_ < self.steptol] = 0
 
         Y = np.full(len(X), fill_value=np.nan)
         Y[ok] = Y_
 
         W = None
         if return_walk:
             W = np.full(len(X), fill_value=np.nan)
```

### Comparing `stepcount-3.4.0/src/stepcount/sslmodel.py` & `stepcount-3.5.0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/stepcount.py` & `stepcount-3.5.0/src/stepcount/stepcount.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,163 +84,213 @@
     Y.to_csv(f"{outdir}/{basename}-Steps.csv.gz")
     # Save timestamps of each step
     T_steps.to_csv(f"{outdir}/{basename}-StepTimes.csv.gz", index=False)
 
     # ENMO summary
     enmo_summary = summarize_enmo(data)
     info['ENMO(mg)'] = enmo_summary['avg']
-    enmo_summary['minutely'].to_csv(f"{outdir}/{basename}-MinutelyENMO.csv.gz")
-    enmo_summary['hourly'].to_csv(f"{outdir}/{basename}-HourlyENMO.csv.gz")
-    enmo_summary['daily'].to_csv(f"{outdir}/{basename}-DailyENMO.csv.gz")
 
     # ENMO summary, adjusted
     enmo_summary_adj = summarize_enmo(data, adjust_estimates=True)
     info['ENMOAdjusted(mg)'] = enmo_summary_adj['avg']
-    enmo_summary_adj['minutely'].to_csv(f"{outdir}/{basename}-MinutelyENMOAdjusted.csv.gz")
-    enmo_summary_adj['hourly'].to_csv(f"{outdir}/{basename}-HourlyENMOAdjusted.csv.gz")
-    enmo_summary_adj['daily'].to_csv(f"{outdir}/{basename}-DailyENMOAdjusted.csv.gz")
 
     # Steps summary
-    summary = summarize_steps(Y, model.steptol)
-    summary['minutely'].to_csv(f"{outdir}/{basename}-MinutelySteps.csv.gz")
-    summary['hourly'].to_csv(f"{outdir}/{basename}-HourlySteps.csv.gz")
-    summary['daily'].to_csv(f"{outdir}/{basename}-DailySteps.csv.gz")
-    info['TotalSteps'] = summary['total']
-    info['StepsDayAvg'] = summary['daily_avg']
-    info['StepsDayMed'] = summary['daily_med']
-    info['StepsDayMin'] = summary['daily_min']
-    info['StepsDayMax'] = summary['daily_max']
-    info['TotalWalking(mins)'] = summary['total_walk']
-    info['WalkingDayAvg(mins)'] = summary['daily_walk_avg']
-    info['WalkingDayMed(mins)'] = summary['daily_walk_med']
-    info['WalkingDayMin(mins)'] = summary['daily_walk_min']
-    info['WalkingDayMax(mins)'] = summary['daily_walk_max']
-    info['CadencePeak1(steps/min)'] = summary['cadence_peak1']
-    info['CadencePeak30(steps/min)'] = summary['cadence_peak30']
-    info['Cadence95th(steps/min)'] = summary['cadence_p95']
-    info['Steps5thDayAvgAt'] = summary['daily_ptile_at_avg']['p05_at']
-    info['Steps25thDayAvgAt'] = summary['daily_ptile_at_avg']['p25_at']
-    info['Steps50thDayAvgAt'] = summary['daily_ptile_at_avg']['p50_at']
-    info['Steps75thDayAvgAt'] = summary['daily_ptile_at_avg']['p75_at']
-    info['Steps95thDayAvgAt'] = summary['daily_ptile_at_avg']['p95_at']
-    info['Steps5thDayMedAt'] = summary['daily_ptile_at_med']['p05_at']
-    info['Steps25thDayMedAt'] = summary['daily_ptile_at_med']['p25_at']
-    info['Steps50thDayMedAt'] = summary['daily_ptile_at_med']['p50_at']
-    info['Steps75thDayMedAt'] = summary['daily_ptile_at_med']['p75_at']
-    info['Steps95thDayMedAt'] = summary['daily_ptile_at_med']['p95_at']
+    steps_summary = summarize_steps(Y, model.steptol)
+    info['TotalSteps'] = steps_summary['total']
+    info['StepsDayAvg'] = steps_summary['daily_avg']
+    info['StepsDayMed'] = steps_summary['daily_med']
+    info['StepsDayMin'] = steps_summary['daily_min']
+    info['StepsDayMax'] = steps_summary['daily_max']
+    info['TotalWalking(mins)'] = steps_summary['total_walk']
+    info['WalkingDayAvg(mins)'] = steps_summary['daily_walk_avg']
+    info['WalkingDayMed(mins)'] = steps_summary['daily_walk_med']
+    info['WalkingDayMin(mins)'] = steps_summary['daily_walk_min']
+    info['WalkingDayMax(mins)'] = steps_summary['daily_walk_max']
+    info['Steps5thAt'] = steps_summary['daily_ptile_at_avg']['p05_at']
+    info['Steps25thAt'] = steps_summary['daily_ptile_at_avg']['p25_at']
+    info['Steps50thAt'] = steps_summary['daily_ptile_at_avg']['p50_at']
+    info['Steps75thAt'] = steps_summary['daily_ptile_at_avg']['p75_at']
+    info['Steps95thAt'] = steps_summary['daily_ptile_at_avg']['p95_at']
 
     # Steps summary, adjusted
-    summary_adj = summarize_steps(Y, model.steptol, adjust_estimates=True)
-    summary_adj['minutely'].to_csv(f"{outdir}/{basename}-MinutelyStepsAdjusted.csv.gz")
-    summary_adj['hourly'].to_csv(f"{outdir}/{basename}-HourlyStepsAdjusted.csv.gz")
-    summary_adj['daily'].to_csv(f"{outdir}/{basename}-DailyStepsAdjusted.csv.gz")
-    info['TotalStepsAdjusted'] = summary_adj['total']
-    info['StepsDayAvgAdjusted'] = summary_adj['daily_avg']
-    info['StepsDayMedAdjusted'] = summary_adj['daily_med']
-    info['StepsDayMinAdjusted'] = summary_adj['daily_min']
-    info['StepsDayMaxAdjusted'] = summary_adj['daily_max']
-    info['TotalWalkingAdjusted(mins)'] = summary_adj['total_walk']
-    info['WalkingDayAvgAdjusted(mins)'] = summary_adj['daily_walk_avg']
-    info['WalkingDayMedAdjusted(mins)'] = summary_adj['daily_walk_med']
-    info['WalkingDayMinAdjusted(mins)'] = summary_adj['daily_walk_min']
-    info['WalkingDayMaxAdjusted(mins)'] = summary_adj['daily_walk_max']
-    info['CadencePeak1Adjusted(steps/min)'] = summary_adj['cadence_peak1']
-    info['CadencePeak30Adjusted(steps/min)'] = summary_adj['cadence_peak30']
-    info['Cadence95thAdjusted(steps/min)'] = summary_adj['cadence_p95']
-    info['Steps5thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p05_at']
-    info['Steps25thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p25_at']
-    info['Steps50thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p50_at']
-    info['Steps75thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p75_at']
-    info['Steps95thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p95_at']
-    info['Steps5thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p05_at']
-    info['Steps25thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p25_at']
-    info['Steps50thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p50_at']
-    info['Steps75thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p75_at']
-    info['Steps95thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p95_at']
+    steps_summary_adj = summarize_steps(Y, model.steptol, adjust_estimates=True)
+    info['TotalStepsAdjusted'] = steps_summary_adj['total']
+    info['StepsDayAvgAdjusted'] = steps_summary_adj['daily_avg']
+    info['StepsDayMedAdjusted'] = steps_summary_adj['daily_med']
+    info['StepsDayMinAdjusted'] = steps_summary_adj['daily_min']
+    info['StepsDayMaxAdjusted'] = steps_summary_adj['daily_max']
+    info['TotalWalkingAdjusted(mins)'] = steps_summary_adj['total_walk']
+    info['WalkingDayAvgAdjusted(mins)'] = steps_summary_adj['daily_walk_avg']
+    info['WalkingDayMedAdjusted(mins)'] = steps_summary_adj['daily_walk_med']
+    info['WalkingDayMinAdjusted(mins)'] = steps_summary_adj['daily_walk_min']
+    info['WalkingDayMaxAdjusted(mins)'] = steps_summary_adj['daily_walk_max']
+    info['Steps5thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p05_at']
+    info['Steps25thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p25_at']
+    info['Steps50thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p50_at']
+    info['Steps75thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p75_at']
+    info['Steps95thAtAdjusted'] = steps_summary_adj['daily_ptile_at_avg']['p95_at']
+
+    # Cadence summary
+    cadence_summary = summary_cadence(Y, model.steptol)
+    info['CadencePeak1(steps/min)'] = cadence_summary['cadence_peak1']
+    info['CadencePeak30(steps/min)'] = cadence_summary['cadence_peak30']
+    info['Cadence95th(steps/min)'] = cadence_summary['cadence_p95']
+
+    # Cadence summary, adjusted
+    cadence_summary_adj = summary_cadence(Y, model.steptol, adjust_estimates=True)
+    info['CadencePeak1Adjusted(steps/min)'] = cadence_summary_adj['cadence_peak1']
+    info['CadencePeak30Adjusted(steps/min)'] = cadence_summary_adj['cadence_peak30']
+    info['Cadence95thAdjusted(steps/min)'] = cadence_summary_adj['cadence_p95']
 
-    # Save info
+    # Save Info.json
     with open(f"{outdir}/{basename}-Info.json", 'w') as f:
         json.dump(info, f, indent=4, cls=NpEncoder)
 
+    hourly = pd.concat([
+        steps_summary['hourly'],
+        enmo_summary['hourly'],
+    ], axis=1)
+    hourly.to_csv(f"{outdir}/{basename}-Hourly.csv.gz")
+    del hourly  # free memory
+
+    hourly_adj = pd.concat([
+        steps_summary_adj['hourly'],
+        enmo_summary_adj['hourly'],
+    ], axis=1)
+    hourly_adj.to_csv(f"{outdir}/{basename}-HourlyAdjusted.csv.gz")
+    del hourly_adj  # free memory
+
+    minutely = pd.concat([
+        steps_summary['minutely'],
+        enmo_summary['minutely'],
+    ], axis=1)
+    minutely.to_csv(f"{outdir}/{basename}-Minutely.csv.gz")
+    del minutely  # free memory
+
+    minutely_adj = pd.concat([
+        steps_summary_adj['minutely'],
+        enmo_summary_adj['minutely'],
+    ], axis=1)
+    minutely_adj.to_csv(f"{outdir}/{basename}-MinutelyAdjusted.csv.gz")
+    del minutely_adj  # free memory
+
+    daily = pd.concat([
+        steps_summary['daily'],
+        cadence_summary['daily'],
+        enmo_summary['daily'],
+    ], axis=1)
+    daily.to_csv(f"{outdir}/{basename}-Daily.csv.gz")
+    # del daily  # still needed for printing
+
+    daily_adj = pd.concat([
+        steps_summary_adj['daily'],
+        cadence_summary_adj['daily'],
+        enmo_summary_adj['daily'],
+    ], axis=1)
+    daily_adj.to_csv(f"{outdir}/{basename}-DailyAdjusted.csv.gz")
+    # del daily_adj  # still needed for printing
+
     # Print
     print("\nSummary\n-------")
     print(json.dumps(info, indent=4, cls=NpEncoder))
     print("\nEstimated Daily Stats\n---------------------")
-    print(summary['daily'])
+    print(daily)
     print("\nEstimated Daily Stats (Adjusted)\n---------------------")
-    print(summary_adj['daily'])
+    print(daily_adj)
+    print("\nOutput files saved in:", outdir)
 
     after = time.time()
     print(f"Done! ({round(after - before,2)}s)")
 
 
 def summarize_enmo(data: pd.DataFrame, adjust_estimates=False):
     """ Summarize ENMO data """
 
+    def _mean(x, skipna=True):
+        if not skipna and x.isna().any():
+            return np.nan
+        return x.mean()
+
     # Truncated ENMO: Euclidean norm minus one and clipped at zero
     v = np.sqrt(data['x'] ** 2 + data['y'] ** 2 + data['z'] ** 2)
     v = np.clip(v - 1, a_min=0, a_max=None)
     v *= 1000  # convert to mg
+    # promptly downsample to minutely to reduce future computation and memory at minimal loss to accuracy
+    v = v.resample('T').agg(_mean, skipna=False)
 
     if adjust_estimates:
         v = impute_missing(v)
         skipna = False
     else:
         # crude summary ignores missing data
         skipna = True
 
-    def _mean(x):
-        if not skipna and x.isna().any():
-            return np.nan
-        return x.mean()
-
     # steps
-    hourly = v.resample('H').agg(_mean).rename('ENMO(mg)')  # ENMO, hourly
-    daily = v.resample('D').agg(_mean).rename('ENMO(mg)')  # ENMO, daily
-    minutely = v.resample('T').agg(_mean).rename('ENMO(mg)')  # ENMO, minutely
+    hourly = v.resample('H').agg(_mean, skipna=skipna).rename('ENMO(mg)')  # ENMO, hourly
+    daily = v.resample('D').agg(_mean, skipna=skipna).rename('ENMO(mg)')  # ENMO, daily
+    minutely = v = v.rename('ENMO(mg)')  # ENMO, minutely
 
     # steps, daily stats
     if not adjust_estimates:
-        avg = daily.mean()
+        avg = daily.agg(_mean, skipna=skipna)
     else:
-        day_of_week = daily.groupby(daily.index.weekday).mean()
-        avg = day_of_week.mean()
+        day_of_week = daily.groupby(daily.index.weekday).agg(_mean, skipna=skipna)
+        avg = day_of_week.agg(_mean, skipna=skipna)
 
     return {
         'avg': avg,
         'hourly': hourly,
         'daily': daily,
         'minutely': minutely,
     }
 
 
 def summarize_steps(Y, steptol=3, adjust_estimates=False):
     """ Summarize step count data """
 
+    dt = infer_freq(Y.index).total_seconds()
+    W = Y.mask(~Y.isna(), Y >= steptol).astype('float')
+
     if adjust_estimates:
         Y = impute_missing(Y)
+        W = impute_missing(W)
         skipna = False
     else:
         # crude summary ignores missing data
         skipna = True
 
     def _sum(x):
-        if not skipna and x.isna().any():
+        na = x.isna()
+        if not skipna and na.any():
+            return np.nan
+        if na.all():  # have to do this explicitly because pandas' .sum() returns 0 if all-NaN
             return np.nan
         return x.sum()
 
-    def _max(x, n=1):
+    def _mean(x):
+        if not skipna and x.isna().any():
+            return np.nan
+        return x.mean()
+
+    def _min(x):
         if not skipna and x.isna().any():
             return np.nan
-        return x.nlargest(n, keep='all').mean()
+        return x.min()
 
-    def _p95(x, steptol):
+    def _max(x):
         if not skipna and x.isna().any():
             return np.nan
-        return x[x >= steptol].quantile(.95)
+        return x.max()
+
+    def _median(x):
+        if not skipna and x.isna().any():
+            return np.nan
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='Mean of empty slice')
+            return x.median()
 
     def _percentile_at(x, ps=(5, 25, 50, 75, 95)):
         percentiles = {f'p{p:02}_at': np.nan for p in ps}
         if not skipna and x.isna().any():
             return percentiles
         z = x.cumsum() / x.sum()
         for p in ps:
@@ -266,79 +316,49 @@
     total = np.round(Y.agg(_sum))  # total steps
     hourly = Y.resample('H').agg(_sum).rename('Steps')  # steps, hourly
     daily = Y.resample('D').agg(_sum).rename('Steps')  # steps, daily
     minutely = Y.resample('T').agg(_sum).rename('Steps')  # steps, minutely
 
     # steps, daily stats
     if not adjust_estimates:
-        daily_avg = np.round(daily.mean())
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', message='Mean of empty slice')
-            daily_med = np.round(daily.median())
-        daily_min = np.round(daily.min())
-        daily_max = np.round(daily.max())
+        daily_avg = np.round(daily.agg(_mean))
+        daily_med = np.round(daily.agg(_median))
+        daily_min = np.round(daily.agg(_min))
+        daily_max = np.round(daily.agg(_max))
     else:
-        day_of_week = daily.groupby(daily.index.weekday).mean()
-        daily_avg = np.round(day_of_week.mean())
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', message='Mean of empty slice')
-            daily_med = np.round(day_of_week.median())
-        daily_min = np.round(day_of_week.min())
-        daily_max = np.round(day_of_week.max())
+        day_of_week = daily.groupby(daily.index.weekday).agg(_mean)
+        daily_avg = np.round(day_of_week.agg(_mean))
+        daily_med = np.round(day_of_week.agg(_median))
+        daily_min = np.round(day_of_week.agg(_min))
+        daily_max = np.round(day_of_week.agg(_max))
 
     # walking
-    dt = pd.Timedelta(infer_freq(Y.index)).seconds
-    W = Y.mask(~Y.isna(), Y >= steptol)
     total_walk = np.round(W.agg(_sum) * dt / 60)
     daily_walk = (W.resample('D').agg(_sum) * dt / 60).rename('Walk(mins)')
 
     # walking, daily stats
     if not adjust_estimates:
-        daily_walk_avg = np.round(daily_walk.mean())
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', message='Mean of empty slice')
-            daily_walk_med = np.round(daily_walk.median())
-        daily_walk_min = np.round(daily_walk.min())
-        daily_walk_max = np.round(daily_walk.max())
-    else:
-        day_of_week_walk = daily_walk.groupby(daily_walk.index.weekday).mean()
-        daily_walk_avg = np.round(day_of_week_walk.mean())
-        with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', message='Mean of empty slice')
-            daily_walk_med = np.round(day_of_week_walk.median())
-        daily_walk_min = np.round(day_of_week_walk.min())
-        daily_walk_max = np.round(day_of_week_walk.max())
-
-    # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
-    daily_cadence_peak1 = minutely.resample('D').agg(_max, n=1).rename('CadencePeak1')
-    daily_cadence_peak30 = minutely.resample('D').agg(_max, n=30).rename('CadencePeak30')
-    daily_cadence_p95 = minutely.resample('D').agg(_p95, steptol=steptol * 60 / dt).rename('Cadence95th')  # scale steptol to steps/min
-    if not adjust_estimates:
-        cadence_peak1 = np.round(daily_cadence_peak1.mean())
-        cadence_peak30 = np.round(daily_cadence_peak30.mean())
-        cadence_p95 = np.round(daily_cadence_p95.mean())
+        daily_walk_avg = np.round(daily_walk.agg(_mean))
+        daily_walk_med = np.round(daily_walk.agg(_median))
+        daily_walk_min = np.round(daily_walk.agg(_min))
+        daily_walk_max = np.round(daily_walk.agg(_max))
     else:
-        day_of_week_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).mean()
-        day_of_week_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).mean()
-        day_of_week_cadence_p95 = daily_cadence_p95.groupby(daily_cadence_p95.index.weekday).mean()
-        cadence_peak1 = np.round(day_of_week_cadence_peak1.mean())
-        cadence_peak30 = np.round(day_of_week_cadence_peak30.mean())
-        cadence_p95 = np.round(day_of_week_cadence_p95.mean())
+        day_of_week_walk = daily_walk.groupby(daily_walk.index.weekday).agg(_mean)
+        daily_walk_avg = np.round(day_of_week_walk.agg(_mean))
+        daily_walk_med = np.round(day_of_week_walk.agg(_median))
+        daily_walk_min = np.round(day_of_week_walk.agg(_min))
+        daily_walk_max = np.round(day_of_week_walk.agg(_max))
 
     daily_ptile_at = Y.groupby(pd.Grouper(freq='D')).apply(_percentile_at).unstack(1)
     daily_ptile_at_avg = daily_ptile_at.mean()
-    daily_ptile_at_med = daily_ptile_at.median()
 
     # daily stats
     daily = pd.concat([
         pd.to_numeric(daily_walk.round(), downcast='integer'),
         pd.to_numeric(daily.round(), downcast='integer'),
-        pd.to_numeric(daily_cadence_peak1.round(), downcast='integer'),
-        pd.to_numeric(daily_cadence_peak30.round(), downcast='integer'),
-        pd.to_numeric(daily_cadence_p95.round(), downcast='integer'),
         daily_ptile_at.rename(columns={
             'p05_at': 'Steps5thAt',
             'p25_at': 'Steps25thAt',
             'p50_at': 'Steps50thAt',
             'p75_at': 'Steps75thAt',
             'p95_at': 'Steps95thAt'
         }).applymap(_tdelta_to_str),
@@ -353,19 +373,15 @@
     daily_min = nanint(daily_min)
     daily_max = nanint(daily_max)
     total_walk = nanint(total_walk)
     daily_walk_avg = nanint(daily_walk_avg)
     daily_walk_med = nanint(daily_walk_med)
     daily_walk_min = nanint(daily_walk_min)
     daily_walk_max = nanint(daily_walk_max)
-    cadence_peak1 = nanint(cadence_peak1)
-    cadence_peak30 = nanint(cadence_peak30)
-    cadence_p95 = nanint(cadence_p95)
     daily_ptile_at_avg = daily_ptile_at_avg.map(_tdelta_to_str)
-    daily_ptile_at_med = daily_ptile_at_med.map(_tdelta_to_str)
 
     return {
         'total': total,
         'minutely': minutely,
         'hourly': hourly,
         'daily': daily,
         'daily_avg': daily_avg,
@@ -373,19 +389,94 @@
         'daily_min': daily_min,
         'daily_max': daily_max,
         'total_walk': total_walk,
         'daily_walk_avg': daily_walk_avg,
         'daily_walk_med': daily_walk_med,
         'daily_walk_min': daily_walk_min,
         'daily_walk_max': daily_walk_max,
-        'cadence_peak1': cadence_peak1,
-        'cadence_peak30': cadence_peak30,
-        'cadence_p95': cadence_p95,
         'daily_ptile_at_avg': daily_ptile_at_avg,
-        'daily_ptile_at_med': daily_ptile_at_med,
+    }
+
+
+def summary_cadence(Y, steptol=3, adjust_estimates=False):
+    """ Summarize cadence data """
+
+    # TODO: split walking and running cadence?
+
+    def _cadence_max(x, steptol, walktol=30, n=1):
+        y = x[x >= steptol]
+        # if not enough walking time, return NA.
+        # note: walktol in minutes, x must be minutely
+        if len(y) < walktol:
+            return np.nan
+        return y.nlargest(n, keep='all').mean()
+
+    def _cadence_p95(x, steptol, walktol=30):
+        y = x[x >= steptol]
+        # if not enough walking time, return NA.
+        # note: walktol in minutes, x must be minutely
+        if len(y) < walktol:
+            return np.nan
+        return y.quantile(.95)
+
+    def _impute_days(x):
+        def na_to_median(x):
+            return x.fillna(x.median())
+        if x.isna().all():
+            return x
+        return (
+            x
+            .groupby(x.index.weekday).transform(na_to_median)
+            .groupby(x.index.weekday >= 5).transform(na_to_median)
+            .transform(na_to_median)
+        )
+
+    dt = infer_freq(Y.index).total_seconds()
+    steptol_in_minutes = steptol * 60 / dt  # rescale steptol to steps/min
+    minutely = Y.resample('T').sum().rename('Steps')  # steps/min
+
+    # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
+
+    daily_cadence_peak1 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, n=1).rename('CadencePeak1(steps/min)')
+    daily_cadence_peak30 = minutely.resample('D').agg(_cadence_max, steptol=steptol_in_minutes, n=30).rename('CadencePeak30(steps/min)')
+    daily_cadence_p95 = minutely.resample('D').agg(_cadence_p95, steptol=steptol_in_minutes).rename('Cadence95th(steps/min)')
+
+    with warnings.catch_warnings():
+        warnings.filterwarnings('ignore', message='Mean of empty slice')
+
+        if adjust_estimates:
+            daily_cadence_peak1 = _impute_days(daily_cadence_peak1)
+            daily_cadence_peak30 = _impute_days(daily_cadence_peak30)
+            daily_cadence_p95 = _impute_days(daily_cadence_p95)
+
+            # representative week
+            day_of_week_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).median()
+            day_of_week_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).median()
+            day_of_week_cadence_p95 = daily_cadence_p95.groupby(daily_cadence_p95.index.weekday).median()
+
+            cadence_peak1 = np.round(day_of_week_cadence_peak1.median())
+            cadence_peak30 = np.round(day_of_week_cadence_peak30.median())
+            cadence_p95 = np.round(day_of_week_cadence_p95.median())
+
+        else:
+            cadence_peak1 = np.round(daily_cadence_peak1.median())
+            cadence_peak30 = np.round(daily_cadence_peak30.median())
+            cadence_p95 = np.round(daily_cadence_p95.median())
+
+    daily = pd.concat([
+        daily_cadence_peak1.round().astype(pd.Int64Dtype()),
+        daily_cadence_peak30.round().astype(pd.Int64Dtype()),
+        daily_cadence_p95.round().astype(pd.Int64Dtype()),
+    ], axis=1)
+
+    return {
+        'daily': daily,
+        'cadence_peak1': nanint(cadence_peak1),
+        'cadence_peak30': nanint(cadence_peak30),
+        'cadence_p95': nanint(cadence_p95),
     }
 
 
 def impute_missing(data: pd.DataFrame, extrapolate=True):
 
     if extrapolate:  # extrapolate beyond start/end times to have full 24h
         freq = infer_freq(data.index)
@@ -416,21 +507,21 @@
                 return x  # will be cast back to a Series automatically
             else:
                 return subframe
 
     data = (
         data
         # first attempt imputation using same day of week
-        .groupby([data.index.weekday, data.index.hour, data.index.minute])
+        .groupby([data.index.weekday, data.index.hour, data.index.minute // 5])
         .transform(fillna)
         # then try within weekday/weekend
-        .groupby([data.index.weekday >= 5, data.index.hour, data.index.minute])
+        .groupby([data.index.weekday >= 5, data.index.hour, data.index.minute // 5])
         .transform(fillna)
         # finally, use all other days
-        .groupby([data.index.hour, data.index.minute])
+        .groupby([data.index.hour, data.index.minute // 5])
         .transform(fillna)
     )
 
     return data
 
 
 def nanint(x):
```

### Comparing `stepcount-3.4.0/src/stepcount/utils/collate_outputs.py` & `stepcount-3.5.0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount/utils/generate_commands.py` & `stepcount-3.5.0/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.5.0/src/stepcount.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.4.0
+Version: 3.5.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
@@ -19,15 +19,19 @@
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
-The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649). 
+The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
+
+Two underlying models are available:
+- Self-supervised learning model of Hang et al. (default): https://www.nature.com/articles/s41746-024-01062-3
+- Random forest (enable with the flag `-t rf`)
 
 ## Install
 
 *Minimum requirements*: Python>=3.8, Java 8 (1.8)
 
 The following instructions make use of Anaconda to meet the minimum requirements:
 
@@ -94,14 +98,15 @@
 2013-10-21     5368
 2013-10-22     7634
 2013-10-23    10009
 ...
 
 Output: outputs/sample/
 ```
+Refer to the [Data Dictionary](data-dictionary.md) for a comprehensive list of outputs.
 
 ### Troubleshooting 
 Some systems may face issues with Java when running the script. If this is your case, try fixing OpenJDK to version 8:
 ```console
 $ conda install -n stepcount openjdk=8
 ```
```

### Comparing `stepcount-3.4.0/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.5.0/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.4.0/versioneer.py` & `stepcount-3.5.0/versioneer.py`

 * *Files identical despite different names*

