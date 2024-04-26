# Comparing `tmp/lottokit-0.9.tar.gz` & `tmp/lottokit-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lottokit-0.9.tar", last modified: Tue Apr 16 15:22:16 2024, max compression
+gzip compressed data, was "lottokit-1.0.tar", last modified: Fri Apr 26 15:00:00 2024, max compression
```

## Comparing `lottokit-0.9.tar` & `lottokit-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-16 15:22:16.068103 lottokit-0.9/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-0.9/LICENSE
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-16 15:22:16.067986 lottokit-0.9/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-0.9/README.md
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-16 15:22:16.066902 lottokit-0.9/lottokit/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-0.9/lottokit/__init__.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    51548 2024-04-14 09:15:12.000000 lottokit-0.9/lottokit/daletou.py
--rw-r--r--   0 zhengdongqi   (501) staff       (20)    67656 2024-04-16 15:21:15.000000 lottokit-0.9/lottokit/util.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-16 15:22:16.067550 lottokit-0.9/lottokit.egg-info/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-16 15:22:16.000000 lottokit-0.9/lottokit.egg-info/PKG-INFO
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-04-16 15:22:16.000000 lottokit-0.9/lottokit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-04-16 15:22:16.000000 lottokit-0.9/lottokit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-04-16 15:22:16.000000 lottokit-0.9/lottokit.egg-info/requires.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-04-16 15:22:16.000000 lottokit-0.9/lottokit.egg-info/top_level.txt
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-0.9/pyproject.toml
--rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-04-16 15:22:16.068152 lottokit-0.9/setup.cfg
--rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-04-16 15:21:37.000000 lottokit-0.9/setup.py
-drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-16 15:22:16.067707 lottokit-0.9/tests/
--rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-0.9/tests/test.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.737191 lottokit-1.0/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    11357 2024-01-29 15:26:41.000000 lottokit-1.0/LICENSE
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-26 15:00:00.737076 lottokit-1.0/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      465 2024-04-15 06:05:32.000000 lottokit-1.0/README.md
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.735698 lottokit-1.0/lottokit/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      380 2024-01-29 15:26:41.000000 lottokit-1.0/lottokit/__init__.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    60914 2024-04-26 14:59:00.000000 lottokit-1.0/lottokit/daletou.py
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)    85145 2024-04-26 14:52:49.000000 lottokit-1.0/lottokit/util.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.736664 lottokit-1.0/lottokit.egg-info/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      857 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      272 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        1 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      155 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/requires.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)        9 2024-04-26 15:00:00.000000 lottokit-1.0/lottokit.egg-info/top_level.txt
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      218 2024-02-01 15:03:38.000000 lottokit-1.0/pyproject.toml
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)       38 2024-04-26 15:00:00.737230 lottokit-1.0/setup.cfg
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)     1182 2024-04-26 14:59:00.000000 lottokit-1.0/setup.py
+drwxr-xr-x   0 zhengdongqi   (501) staff       (20)        0 2024-04-26 15:00:00.736793 lottokit-1.0/tests/
+-rw-r--r--   0 zhengdongqi   (501) staff       (20)      216 2024-02-12 12:13:32.000000 lottokit-1.0/tests/test.py
```

### Comparing `lottokit-0.9/LICENSE` & `lottokit-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lottokit-0.9/PKG-INFO` & `lottokit-1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 0.9
+Version: 1.0
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-0.9/lottokit/daletou.py` & `lottokit-1.0/lottokit/daletou.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 @Email   : nickdecodes@163.com
 @Usage   :
 @FileName: daletou.py
 @DateTime: 2023/12/7 19:58
 @SoftWare:
 """
 
-
 import os
 import time
+import math
+from scipy.stats import randint
 from datetime import datetime, timedelta
 from itertools import combinations
 from collections import Counter, namedtuple
 from typing import List, Tuple, Any, Optional, Union, Dict, NamedTuple, Callable, Generator, Iterable
 from selenium.webdriver.common.by import By
 from .util import IOUtil, ModelUtil, SpiderUtil, CalculateUtil, AnalyzeUtil, re, WebDriverWait, EC
 
@@ -145,14 +146,15 @@
             # 'cold_hot_numbers': 4,
             # 'omitted_numbers': 9
         }
 
     """
     A pure virtual method inherited from util.SpiderUtil
     """
+
     def spider_recent_data(self) -> List[List[str]]:
         """
         Fetch the recent data from the web page.
 
         :return: A list of lists containing recent data entries.
         """
         driver = self.spider_chrome_driver()
@@ -218,14 +220,15 @@
         sorted_full_data = sorted(full_data, key=lambda x: int(x[0]))
 
         return sorted_full_data
 
     """
     A pure virtual method inherited from util.AnalyzeUtil
     """
+
     def analyze_same_period_numbers(self, data=None, **kwargs: Any) -> None:
         """
         Analyze same period number in the last period.
         """
         if data is None:
             return
 
@@ -453,14 +456,15 @@
 
         # Write updated data back to files
         self.write_json_data_to_file(self.omitted_record_path, record_data, app_log=self.app_log)
 
     """
     A pure virtual method inherited from util.CalculateUtil
     """
+
     def calculate_winning_amount(self,
                                  winning_number_combination: Union[NamedTuple, List[int], None],
                                  purchase_number_combinations: Union[List[NamedTuple], List[List[int]], None],
                                  **kwargs: Any) -> Tuple[int, int]:
         """
         Calculate the winning amount based on matching combinations.
 
@@ -495,14 +499,15 @@
                 award_count += 1
 
         return award_amount, award_count
 
     """
     Static methods with no side effects
     """
+
     @staticmethod
     def get_chunks_with_next(data: List[Any],
                              chunk_size: int = 10) -> Generator[Tuple[List[Any], Optional[Any]], None, None]:
         """
         Yields consecutive chunks of size `chunk_size` from `data` after removing elements from the start of `data`
         based on the remainder of the length of `data` divided by `chunk_size`. Exits if the next element is None.
 
@@ -522,14 +527,15 @@
             if next_element is None:
                 break  # Break if we've reached or passed the end of the list
             yield chunk, next_element
 
     """
     other instance method
     """
+
     def download_data(self, force: bool = False) -> None:
         """
         spider full data and save data to history record file
 
         Parameters:
         - force: If True, files will write even if they already exist. Defaults to False.
         """
@@ -726,14 +732,15 @@
         # If none of the above conditions are met, raise an IndexError.
         raise IndexError(f'length:{length} does not match any expected size')
 
     def revised_features(self, last_window_period_datas: Dict[str, Any]) -> Dict[str, Any]:
         """
         Prepares the features data structure for the prediction algorithm.
         """
+
         def _feature_reviser(predictions: Counter, delta_size: int, feature_key: str) -> Counter:
             """
             Filters predictions based on the feature key and delta size.
 
             If the feature key includes 'ratio', only predictions where the sum equals the delta size are returned.
             Otherwise, all predictions are returned.
 
@@ -773,15 +780,16 @@
         additional parameters for certain compute methods. The results are stored in a new dictionary
         and returned.
 
         :param lottery_datas: A list of Lottery objects containing the front and back data.
         :param region: Integer to select the compute region, 1: front, 2: back, 3: all.
         :return: A dictionary with computed feature results.
         """
-        def _calculate_parser(caller: Callable, data: List[int], param: Optional[List] = None,) -> List[int]:
+
+        def _calculate_parser(caller: Callable, data: List[int], param: Optional[List] = None, ) -> List[int]:
             return caller(data, param) if param is not None else compute_method(data)
 
         features = {}
         add_ranges_params: Dict[str, Tuple[List, List]] = {
             'zone_ratio': (self.front_zone_ranges, self.back_zone_ranges),
             'big_small_ratio': (self.front_big_small_ranges, self.back_big_small_ranges),
             'road_012_ratio': (self.front_road_012_ranges, self.back_road_012_ranges),
@@ -854,17 +862,17 @@
         for feature, item in feature_results.items():
             for region, matrix in item.items():
                 # Transpose the matrix to iterate over columns (sequences)
                 # matrix_flip = list(map(list, zip(*matrix)))
                 matrix_flip = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
 
                 for predictor in [
-                    self.moving_average,
-                    self.linear_regression,
-                    self.random_forest_regressor
+                    self.exponential_moving_average_next_value,
+                    self.linear_regression_next_value_by_index,
+                    self.random_forest_regressor_next_value_by_index
                 ]:
                     # Initialize the nested sets for each feature and region if not already present
                     region_predictions = predictions.setdefault(feature, {}).setdefault(region, Counter())
 
                     # Apply each predictor to each sequence and store the results
                     if 'ratio' in feature:
                         # For 'ratio' features, store results as tuples in a set
@@ -921,116 +929,142 @@
 
         # Transpose the matrix
         matrix_flip = [[matrix[j][i] for j in range(len(matrix))] for i in range(len(matrix[0]))]
 
         # Apply the transposed matrix to each predictor and generate predictions
         predictions = [
             tuple(predictor(seq) for seq in matrix_flip) for predictor in [
-                self.moving_average,
-                self.linear_regression,
-                self.random_forest_regressor,
+                self.exponential_moving_average_next_value,
+                self.linear_regression_next_value_by_index,
+                self.random_forest_regressor_next_value_by_index,
             ]
         ]
 
         # Create a list of Lottery objects based on the predictions
         return [
             self.Lottery('', '', '', self.calculate_front(d), self.calculate_back(d))
             for d in predictions
         ]
 
-    def predict_by_last_period(self, next_period: int = None, show_details: bool = False) -> List[List[int]]:
+    def predict_by_last_period(
+            self,
+            next_period: int = None,
+            show_details: bool = False,
+            window_size: int = 15
+    ) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
+        :param window_size: int, default is 15
         """
         history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
         if next_period is None:
             history_data = history_data[:]
         else:
             index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
             history_data = history_data[:index] if index != -1 else history_data[:]
 
-        maybe_combinations = self.predict_by_last_window_data(history_data, window=15)
+        maybe_combinations = self.predict_by_last_window_data(history_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
-        handle_result = self.handle_last_window_data(data=history_data, window=15)
+        handle_result = self.handle_last_window_data(data=history_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
 
         return predict_data
 
-    def predict_by_same_period(self, next_period: int = None, show_details: bool = False) -> List[List[int]]:
+    def predict_by_same_period(
+            self,
+            next_period: int = None,
+            show_details: bool = False,
+            window_size: int = 15
+    ) -> List[List[int]]:
         """
         Predicts features by the last period window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
+        :param window_size: int, default is 15
         """
         period_data = self.read_json_data_from_file(self.period_record_path, app_log=self.app_log)
         if next_period is None:
             period_data = period_data.get(str(self.get_next_period()).zfill(3))
         else:
             period_data = period_data.get(str(next_period % 100).zfill(3))
             index = next((i for i, sublist in enumerate(period_data) if sublist[0] == str(next_period)), -1)
             period_data = period_data[:index] if index != -1 else period_data[:]
 
-        maybe_combinations = self.predict_by_last_window_data(period_data, window=15)
+        maybe_combinations = self.predict_by_last_window_data(period_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
-        handle_result = self.handle_last_window_data(data=period_data, window=15)
+        handle_result = self.handle_last_window_data(data=period_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
 
         return predict_data
 
-    def predict_by_last_weekday(self,
-                                next_weekday: int = None,
-                                next_period: int = None,
-                                show_details: bool = False) -> List[List[int]]:
+    def predict_by_last_weekday(
+            self,
+            next_weekday: int = None,
+            next_period: int = None,
+            show_details: bool = False,
+            window_size: int = 15
+    ) -> List[List[int]]:
         """
         Predicts features by the last weekday window of historical data and prints the results.
         Skips predictions where the sum of 'ratio' features does not match the expected size.
         :param next_weekday: int eg: [1 | 3 | 6]
         :param next_period: int eg: 24001
         :param show_details: boolean flag to output details about the prediction
+        :param window_size: int, default is 15
         """
         weekday_data = self.read_json_data_from_file(self.weekday_record_path, app_log=self.app_log)
         if next_weekday is None:
             weekday_data = weekday_data.get(str(self.get_next_weekday()))
         else:
             weekday_data = weekday_data.get(str(next_weekday))
             if next_period is not None:
                 index = next((i for i, sublist in enumerate(weekday_data) if sublist[0] == str(next_period)), -1)
                 weekday_data = weekday_data[:index] if index != -1 else weekday_data[:]
 
-        maybe_combinations = self.predict_by_last_window_data(weekday_data, window=15)
+        maybe_combinations = self.predict_by_last_window_data(weekday_data, window=window_size)
         predict_data = [mc.front + mc.back for mc in maybe_combinations]
         self.app_log.info(predict_data) if show_details is True else None
 
-        handle_result = self.handle_last_window_data(data=weekday_data, window=15)
+        handle_result = self.handle_last_window_data(data=weekday_data, window=window_size)
         self.app_log.info(handle_result) if show_details is True else None
 
         return predict_data
 
-    def predict(self, next_period: int = None, next_weekday: int = None, show_details: bool = False) -> List[List[int]]:
+    def predict(
+            self,
+            next_period: int = None,
+            next_weekday: int = None,
+            show_details: bool = False,
+            window_size: int = 15
+    ) -> List[List[int]]:
         """
         :param next_period: int eg: 24001
         :param next_weekday: int eg: [1 | 3 | 6]
         :param show_details: boolean flag to output details about the prediction
+        :param window_size: int, the default is 15
         """
         predict_data = []
         predict_data.extend(self.predict_by_last_period(next_period=next_period,
-                                                        show_details=show_details))
+                                                        show_details=show_details,
+                                                        window_size=window_size))
         predict_data.extend(self.predict_by_same_period(next_period=next_period,
-                                                        show_details=show_details))
+                                                        show_details=show_details,
+                                                        window_size=window_size))
         predict_data.extend(self.predict_by_last_weekday(next_weekday=next_weekday,
                                                          next_period=next_period,
-                                                         show_details=show_details))
+                                                         show_details=show_details,
+                                                         window_size=window_size))
 
         if show_details is True:
             self.app_log.info("The following is a preliminary forecast of the data analysis : ")
             # Splitting the data into first 5 and last 2 numbers
             front_zone = [num for row in predict_data for num in row[:5]]
             back_zone = [num for row in predict_data for num in row[5:]]
 
@@ -1039,22 +1073,178 @@
             back_zone_frequency = Counter(back_zone)
 
             # Sorting the counts
             sorted_front_zone_frequency = sorted(front_zone_frequency.items(), key=lambda x: x[1], reverse=True)
             sorted_back_zone_frequency = sorted(back_zone_frequency.items(), key=lambda x: x[1], reverse=True)
 
             # Printing the results
-            print("Counts of the front zone numbers in each row sorted by frequency:")
+            self.app_log.info("Counts of the front zone numbers in each row sorted by frequency:")
             for number, count in sorted_front_zone_frequency:
-                print(f"Number {number}: {count} times")
+                self.app_log.info(f"Number {number}: {count} times")
+            self.app_log.info(f"Total count of the front zone numbers in each row: {len(sorted_front_zone_frequency)}")
 
-            print("\nCounts of the back zone numbers in each row sorted by frequency:")
+            self.app_log.info("\nCounts of the back zone numbers in each row sorted by frequency:")
             for number, count in sorted_back_zone_frequency:
-                print(f"Number {number}: {count} times")
+                self.app_log.info(f"Number {number}: {count} times")
+            self.app_log.info(f"Total count of the back zone numbers in each row: {len(sorted_back_zone_frequency)}")
 
             self.app_log.info("\nHere are the preliminary predictions: ")
             for data in predict_data:
-                self.app_log.info(','.join(map(str, data)))
+                self.app_log.info(', '.join(map(str, data)))
         return predict_data
 
+    def calculate_predictions_and_intervals(
+            self,
+            data: List[Union[float, int]],
+            sd_threshold: float,
+            rolling_size: int,
+            warm_start: bool = False,
+            random_state: int = 12,
+            param_distributions: Optional[Dict] = None,
+            param_overrides: Optional[Dict] = None
+    ) -> Tuple[Union[float, int], int, int]:
+        """
+        Calculate prediction intervals based on historical data and a specified rolling size.
+
+        Args:
+            data (List[float]): The list of historical data points.
+            sd_threshold (float): The threshold for standard deviation calculations.
+            rolling_size (int): The number of recent data points to consider for rolling calculations.
+            warm_start (bool, optional): Whether to use the previous model state for training. Defaults to False.
+            random_state (int, optional): A seed used by the random number generator for reproducibility. Defaults to 12.
+            param_distributions (Optional[Dict]): The distribution of parameters to try in randomized search.
+            param_overrides (Optional[Dict]): Additional parameters for the RandomizedSearchCV.
+
+        Returns:
+            Tuple[float, int, int]: A tuple containing the predicted value, and the minimum and maximum values of the prediction interval.
+        """
+        # Calculate standard deviation and tendency using a Welford's method based implementation
+        sd = self.calculate_standard_deviation_welford(data[-rolling_size:])
+        tendency = 0
+        rsi = self.relative_strength_index(data[-rolling_size:], period=rolling_size // 2)
+        if data[-1] >= math.floor(0.75 * sd_threshold) or rsi > 69:
+            tendency = -1
+        elif data[-1] <= math.ceil(0.12 * sd_threshold) or rsi < 31:
+            tendency = 1
+        param_overrides = param_overrides or {
+            'n_iter': 100,
+            'cv': 3,
+            'scoring': 'neg_mean_squared_error',
+            'verbose': 0,
+            'random_state': 12,
+            'n_jobs': -1
+        }
+        # Predict the next value using a random forest regressor
+        pred = self.random_forest_regressor_next_value(data, rolling_size=rolling_size,
+                                                       warm_start=warm_start,
+                                                       random_state=random_state,
+                                                       param_distributions=param_distributions,
+                                                       param_overrides=param_overrides)
+
+        # Set default interval values based on zero tendency
+        min_val = math.floor(pred - sd)
+        max_val = math.ceil(pred + sd)
+
+        # Adjust interval based on the tendency
+        if tendency < 0:
+            max_val = math.ceil(pred + sd)
+        elif tendency > 0:
+            min_val = math.floor(pred - sd)
+
+        return pred, min_val, max_val
+
+    def analyze_predict(
+            self,
+            next_period: int = None,
+            next_weekday: int = None,
+            show_details: bool = False,
+            window_size: int = 15
+    ) -> List[List[int]]:
+        def filter_combs(combs, criteria, intersection_set, required_intersection_count):
+            filtered_combs = []
+            for comb in combs:
+                sum_val = self.calculate_sum_total(comb)
+                span_val = self.calculate_span(comb)
+                avg_val = self.calculate_avg(comb)
+
+                if all([
+                    criteria['sum_total']['min'] <= sum_val <= criteria['sum_total']['max'],
+                    criteria['span']['min'] <= span_val <= criteria['span']['max'],
+                    criteria['avg']['min'] <= avg_val <= criteria['avg']['max'],
+                    # len(intersection_set.intersection(set(comb))) >= required_intersection_count,
+                ]):
+                    filtered_combs.append(comb)
+            return filtered_combs
+
+        predict_data = self.predict(next_period=next_period, next_weekday=next_weekday,
+                                    show_details=show_details, window_size=window_size)
+        front_set, back_set = set(), set()
+        for data in predict_data:
+            front_set.update(self.calculate_front(data))
+            back_set.update(self.calculate_back(data))
+
+        self.app_log.info("Now, Will analyze the predictions..., Then adjust data")
+        history_data = self.read_csv_data_from_file(self.history_record_path, app_log=self.app_log)
+        if next_period is not None:
+            index = next((i for i, sublist in enumerate(history_data) if sublist[0] == str(next_period)), -1)
+            history_data = history_data[:index] if index != -1 else history_data[:]
+
+        features = ['sum_total', 'span', 'avg']
+        history_data_features = {zone: {feat: [] for feat in features} for zone in ['front', 'back']}
+        # Use results as needed
+        for data in history_data:
+            for zone in ['front', 'back']:
+                zone_data = self.calculate_front(data) if zone == 'front' else self.calculate_back(data)
+                for feature in features:
+                    func = getattr(self, f'calculate_{feature}')
+                    history_data_features[zone][feature].append(func(zone_data))
+
+        params = {
+            'front': {
+                'sum_total': {'sd_threshold': sum([31, 32, 33, 34, 35]), 'rolling_size': 5, 'warm_start': True,
+                              'random_state': 12},
+                'span': {'sd_threshold': abs(35 - 1), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
+                'avg': {'sd_threshold': sum([31, 32, 33, 34, 35]) // 5, 'rolling_size': 5, 'warm_start': True,
+                        'random_state': 12}
+            },
+            'back': {
+                'sum_total': {'sd_threshold': sum([11, 12]), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
+                'span': {'sd_threshold': abs(12 - 1), 'rolling_size': 5, 'warm_start': True, 'random_state': 12},
+                'avg': {'sd_threshold': sum([11, 12]) // 2, 'rolling_size': 5, 'warm_start': True, 'random_state': 12}
+            }
+        }
+        results = {'front': {}, 'back': {}}
+
+        for zone in ['front', 'back']:
+            for feature in features:
+                pred, min_val, max_val = self.calculate_predictions_and_intervals(
+                    history_data_features[zone][feature],
+                    params[zone][feature]['sd_threshold'],
+                    params[zone][feature]['rolling_size'],
+                    params[zone][feature]['warm_start'],
+                    params[zone][feature]['random_state'],
+                    param_distributions={
+                        'n_estimators': randint(100, 500),
+                        'max_depth': [None, ] + [i for i in range(10, 100)],
+                        'max_features': ['sqrt', 'log2'],
+                        'min_samples_split': randint(2, 80),
+                        'min_samples_leaf': randint(1, 40)
+                    }
+                )
+                results[zone][feature] = {'prediction': pred, 'min': min_val, 'max': max_val}
+                self.app_log.info(f'zone:{zone} {feature}: {pred}, min: {min_val}, max: {max_val}')
+
+        # Filter front and back combinations
+        # filter_front_comb = filter_combs(self.all_fronts, results['front'], front_set, 4)
+        filter_front_comb = filter_combs(list(combinations(front_set, self.front_size)), results['front'], front_set, 4)
+        # filter_back_comb = filter_combs(self.all_backs, results['back'], back_set, 1)
+        filter_back_comb = filter_combs(list(combinations(back_set, self.back_size)), results['back'], back_set, 1)
+        self.app_log.info(f'Front filter result count: {len(filter_front_comb)}')
+        self.app_log.info(f'Back filter result count: {len(filter_back_comb)}')
+
+        # Combine front and back combinations
+        final_combinations = [front + back for front in filter_front_comb for back in filter_back_comb]
+        self.app_log.info(f'Final result count: {len(final_combinations)}')
+        return final_combinations
+
     def test(self):
         pass
```

### Comparing `lottokit-0.9/lottokit/util.py` & `lottokit-1.0/lottokit/util.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,28 +9,35 @@
 @DateTime: 2023/8/23 23:13
 @SoftWare: 
 """
 
 import re
 import sys
 import csv
+import math
 import time
 import json
 import datetime
 import logging
 import logging.handlers
 from abc import ABC, abstractmethod
 from typing import Iterable, List, Tuple, Any, Optional, Union, Set, Dict
 import random
 import numpy as np
 import pandas as pd
 from pmdarima import auto_arima
 from selenium import webdriver
+from sklearn.pipeline import Pipeline
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.pipeline import make_pipeline
+from sklearn.preprocessing import StandardScaler
 from sklearn.ensemble import RandomForestRegressor
 from sklearn.linear_model import LinearRegression
+from sklearn.preprocessing import PolynomialFeatures
+from sklearn.model_selection import RandomizedSearchCV
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 
 
 class IOUtil:
     @classmethod
@@ -319,68 +326,131 @@
         except Exception as ex:
             app_log.exception(f"An error occurred while reading the JSON file: {ex}")
             return None
 
 
 class ModelUtil:
     @staticmethod
-    def moving_average(numeric_sequence: List[int]) -> int:
+    def exponential_moving_average_next_value(numeric_sequence: List[int], span: int = 5) -> int:
         """
         Calculate the Exponential Moving Average (EMA) of a given numeric sequence.
 
         EMA is a type of moving average that places a greater weight and significance
         on the most recent data points. It's more responsive to new information compared
         to a simple moving average (SMA).
 
         :param numeric_sequence: A list or sequence of numbers for which the EMA is to be calculated.
+        :param span: The number of periods over which to calculate the EMA. Default is 5.
         :return: The EMA value as an integer.
+        :raises ValueError: If the input list is empty or contains non-numeric values.
         """
+        if not numeric_sequence:
+            raise ValueError("The numeric sequence cannot be empty.")
+        if not all(isinstance(x, (int, float)) for x in numeric_sequence):
+            raise ValueError("All elements in the numeric sequence must be numbers.")
+
         # Convert the numeric sequence into a pandas Series object
         series = pd.Series(numeric_sequence)
 
         # Calculate the EMA using pandas' ewm method
-        # 'span' defines the period over which to calculate the EMA
-        # 'min_periods' sets the minimum number of observations in window required to have a value
-        # 'adjust=False' specifies that we are interested in the recursive calculation mode
-        ema = series.ewm(span=5, min_periods=len(numeric_sequence), adjust=False).mean()
+        # Adjust 'min_periods' to handle shorter sequences gracefully
+        ema = series.ewm(span=span, min_periods=min(span, len(numeric_sequence)), adjust=False).mean()
 
         # Return the last value of the EMA series as an integer
         return round(ema.iloc[-1])
 
     @staticmethod
-    def linear_regression(numeric_sequence: List[int]) -> int:
+    def linear_regression_next_value_by_index(numeric_sequence: List[int]) -> int:
         """
         Predicts the next value in a sequence using linear regression.
 
         Linear regression involves fitting a line to the data points in such a way
         that the distance between the data points and the line is minimized. This function
         uses the method to predict the next value in a given sequence of numbers by fitting
-        a model to the sequence and looking at the slope of the line.
+        a model to the sequence and examining the slope of the line.
 
         :param numeric_sequence: A list or sequence of numbers to model.
         :return: The predicted next value in the sequence as an integer.
+        :raises ValueError: If the input sequence is empty or too short for regression analysis.
         """
+        if not numeric_sequence:
+            raise ValueError("The numeric sequence cannot be empty.")
+        if len(numeric_sequence) < 2:
+            raise ValueError("The numeric sequence must contain at least two elements for linear regression.")
+
         # Convert the numeric sequence into a numpy array and reshape for sklearn
         data = np.array(numeric_sequence).reshape(-1, 1)
 
         # Create an array representing time or the independent variable, reshaped as a column
-        time = np.array(range(len(data))).reshape(-1, 1)
+        index = np.array(range(len(data))).reshape(-1, 1)
 
         # Create a LinearRegression model and fit it to the data
         model = LinearRegression()
-        model.fit(time, data)
+        model.fit(index, data)
 
         # Predict the next value in the sequence using the fitted model
         prediction = model.predict([[len(data)]])[0][0]
 
         # Return the predicted value as an integer
         return round(prediction)
 
     @staticmethod
-    def harmonic_regression(numeric_sequence: List[int], frequency: float = 1.0) -> int:
+    def multivariate_polynomial_regression_next_value(
+            numeric_sequence: List[int],
+            rolling_size: int,
+            degrees: int = 3,
+    ) -> float:
+        """
+        Predicts the next value in a numeric sequence using multivariate polynomial regression.
+
+        This method applies a polynomial regression model to a numeric sequence to predict the next value.
+        It utilizes a rolling window approach to create datasets, scales the features, and fits a polynomial
+        regression model to make the prediction.
+
+        Args:
+            numeric_sequence (List[int]): The list of integers representing the sequence.
+            rolling_size (int): The number of elements in each rolling window.
+            degrees (int): The degree of the polynomial regression. Defaults to 3.
+
+        Returns:
+            float: The predicted next value in the sequence.
+
+        Raises:
+            ValueError: If the rolling_size is larger than the size of numeric_sequence.
+        """
+        if rolling_size > len(numeric_sequence):
+            raise ValueError("rolling_size cannot be larger than the size of numeric_sequence")
+
+        # Generate datasets with the specified rolling size
+        train_x, train_y = CalculateUtil.generate_datasets_with_rolling_size(
+            data=numeric_sequence, rolling_size=rolling_size
+        )
+
+        # Preparing input data for model training
+        input_x = np.array(train_x)
+        output_y = np.array(train_y)
+
+        # Scaling the features
+        scaler = StandardScaler()
+        input_x_scaled = scaler.fit_transform(input_x)
+
+        # Creating and training the polynomial regression model
+        model = make_pipeline(PolynomialFeatures(degrees), LinearRegression())
+        model.fit(input_x_scaled, output_y)
+
+        # Preparing the last rolling window of data for prediction
+        test_x = np.array([numeric_sequence[-rolling_size:]])
+        test_x_scaled = scaler.transform(test_x)
+
+        # Predicting the next value
+        pred_y = model.predict(test_x_scaled)
+        return pred_y[0]
+
+    @staticmethod
+    def harmonic_regression_next_value_by_index(numeric_sequence: List[int], frequency: float = 1.0) -> int:
         """
         Predicts the next value in a sequence using harmonic regression.
 
         Harmonic regression involves fitting a model with sine and cosine components to capture
         periodic patterns in the data. This function predicts the next value in a given sequence
         of numbers by fitting a harmonic model to the sequence.
 
@@ -388,19 +458,19 @@
         :param frequency: The frequency of the periodic component to model.
         :return: The predicted next value in the sequence as an integer.
         """
         # Convert the numeric sequence into a numpy array
         data = np.array(numeric_sequence).reshape(-1, 1)
 
         # Create an array representing time or the independent variable
-        time = np.array(range(len(data))).reshape(-1, 1)
+        index = np.array(range(len(data))).reshape(-1, 1)
 
         # Generate sine and cosine features based on the time array and given frequency
-        sine_feature = np.sin(2 * np.pi * frequency * time)
-        cosine_feature = np.cos(2 * np.pi * frequency * time)
+        sine_feature = np.sin(2 * np.pi * frequency * index)
+        cosine_feature = np.cos(2 * np.pi * frequency * index)
 
         # Combine sine and cosine features into a single feature matrix
         features = np.hstack((sine_feature, cosine_feature))
 
         # Create a LinearRegression model and fit it to the data with harmonic features
         model = LinearRegression()
         model.fit(features, data)
@@ -413,15 +483,143 @@
 
         prediction = model.predict(next_features)[0][0]
 
         # Return the predicted value as an integer
         return round(prediction)
 
     @staticmethod
-    def random_forest_regressor(numeric_sequence: List[int]) -> int:
+    def random_forest_regressor_transformer(
+            numeric_sequence: List[int],
+            rolling_size: int,
+            warm_start: bool = False,
+            random_state: int = 12,
+            param_distributions: Optional[Dict] = None,
+            param_overrides: Optional[Dict] = None
+    ) -> float:
+        train_x, train_y = CalculateUtil.generate_datasets_with_rolling_size(
+            data=numeric_sequence, rolling_size=rolling_size
+        )
+
+        # Convert lists to numpy arrays for compatibility with scikit-learn
+        input_x = np.array(train_x)
+        output_y = np.array(train_y)
+
+        # Scale the features to normalize data
+        scaler = StandardScaler()
+        input_x_scaled = scaler.fit_transform(input_x)
+
+        # Initialize and train the Random Forest Regressor
+        model = RandomForestRegressor(warm_start=warm_start, random_state=random_state)
+        if param_distributions:
+            param_overrides = param_overrides or {}
+            random_search = RandomizedSearchCV(estimator=model, param_distributions=param_distributions,
+                                               **param_overrides)
+            random_search.fit(input_x_scaled, output_y)
+            model = RandomForestRegressor(warm_start=warm_start, random_state=random_state,
+                                          **random_search.best_params_)
+
+        model_pipline = Pipeline([
+            ('prediction_transformer', RandomForestRegressorTransformer(model)),
+            ('prediction_transformer_two', RandomForestRegressor(warm_start=warm_start, random_state=random_state)),
+            # ('poly_features', PolynomialFeatures(degree=2)),
+            # ('linear_regression', LinearRegression())
+        ])
+        model_pipline.fit(input_x_scaled, output_y)
+
+        # Prepare the last rolling window of data for prediction
+        test_x = np.array([numeric_sequence[-rolling_size:]])
+        test_x_scaled = scaler.transform(test_x)
+
+        # Predicting the next value
+        pred_y = model_pipline.predict(test_x_scaled)
+        return pred_y
+
+    @staticmethod
+    def random_forest_regressor_next_value(
+            numeric_sequence: List[int],
+            rolling_size: int,
+            warm_start: bool = False,
+            random_state: int = 12,
+            param_distributions: Optional[Dict] = None,
+            param_overrides: Optional[Dict] = None
+    ) -> float:
+        """
+        Predicts the next value in a numeric sequence using a Random Forest Regressor model.
+
+        This method uses a Random Forest Regressor to predict the next value in a sequence based on
+        the values in a rolling window. The sequence is first transformed into a dataset suitable for
+        regression by creating overlapping windows of specified size.
+
+        Args:
+            numeric_sequence (List[int]): The list of integers representing the sequence.
+            rolling_size (int): The number of elements in each rolling window.
+            warm_start (bool): Whether to reuse the solution of the previous call to fit and add more estimators to the ensemble.
+            random_state (int): Controls both the randomness of the bootstrapping of the samples used when building trees
+                                (if `bootstrap=True`) and the sampling of the features to consider when looking for the best split at each node.
+            param_distributions (Optional[Dict]): The distribution of parameters to try in randomized search.
+                                                eg: {
+                                                    'n_estimators': stats.randint(100, 500),
+                                                    'max_depth': [None, ] + [i for i in range(10, 100)],
+                                                    'max_features': ['sqrt', 'log2'],
+                                                    'min_samples_split': stats.randint(2, 80),
+                                                    'min_samples_leaf': stats.randint(1, 40)
+                                                }
+            param_overrides (Optional[Dict]): Additional parameters for the RandomizedSearchCV.
+                                                eg: {
+                                                    'n_iter': 100,
+                                                    'cv': 3,
+                                                    'scoring': 'neg_mean_squared_error',
+                                                    'verbose': 0,
+                                                    'random_state': 12,
+                                                    'n_jobs': -1
+                                                }
+
+        Returns:
+            float: The predicted next value in the sequence.
+
+        Raises:
+            ValueError: If the rolling_size is larger than the size of numeric_sequence.
+        """
+        if rolling_size > len(numeric_sequence):
+            raise ValueError("rolling_size cannot be larger than the size of numeric_sequence")
+
+        # Generate datasets with the specified rolling size
+        train_x, train_y = CalculateUtil.generate_datasets_with_rolling_size(
+            data=numeric_sequence, rolling_size=rolling_size
+        )
+
+        # Convert lists to numpy arrays for compatibility with scikit-learn
+        input_x = np.array(train_x)
+        output_y = np.array(train_y)
+
+        # Scale the features to normalize data
+        scaler = StandardScaler()
+        input_x_scaled = scaler.fit_transform(input_x)
+
+        # Initialize and train the Random Forest Regressor
+        model = RandomForestRegressor(warm_start=warm_start, random_state=random_state)
+        if param_distributions:
+            param_overrides = param_overrides or {}
+            random_search = RandomizedSearchCV(estimator=model, param_distributions=param_distributions,
+                                               **param_overrides)
+            random_search.fit(input_x_scaled, output_y)
+            model = RandomForestRegressor(warm_start=warm_start, random_state=random_state,
+                                          **random_search.best_params_)
+        model.fit(input_x_scaled, output_y)
+
+        # Prepare the last rolling window of data for prediction
+        test_x = np.array([numeric_sequence[-rolling_size:]])
+        test_x_scaled = scaler.transform(test_x)
+
+        # Predicting the next value
+        pred_y = model.predict(test_x_scaled)
+        return pred_y[0]
+
+    @staticmethod
+    def random_forest_regressor_next_value_by_index(numeric_sequence: List[int]) -> int:
         """
         Predicts the next value in a sequence using a Random Forest Regressor.
 
         A Random Forest Regressor is a type of ensemble machine learning model that uses
         multiple decision trees to make predictions. It is particularly useful for regression
         tasks on complex datasets because it can capture non-linear relationships between
         variables. This function applies the model to a sequence of numbers to predict the
@@ -430,70 +628,60 @@
         :param numeric_sequence: A list or sequence of numbers to model.
         :return: The predicted next value in the sequence as an integer.
         """
         # Convert the numeric sequence into a numpy array and reshape for sklearn
         data = np.array(numeric_sequence).reshape(-1, 1)
 
         # Create an array representing time or the independent variable, reshaped as a column
-        time = np.array(range(len(data))).reshape(-1, 1)
+        time_feature = np.array(range(len(data))).reshape(-1, 1)
 
         # Create a RandomForestRegressor model and fit it to the data
         model = RandomForestRegressor()
-        model.fit(time, data.ravel())  # Flatten the array to fit the model
+        model.fit(time_feature, data.ravel())  # Flatten the array to fit the model
 
         # Predict the next value in the sequence using the fitted model
         future_time = np.array([len(data)]).reshape(-1, 1)
         future_pred = model.predict(future_time)
 
         # Return the predicted value as an integer
         return round(future_pred[0])
 
     @staticmethod
-    def relative_strength_index(numeric_sequence: List[int], period: int = 10) -> int:
+    def relative_strength_index(numeric_sequence: List[int], period: int = 14) -> float:
         """
-        Calculate the Relative Strength Index (RSI) for a given list of prices.
-
-        The RSI is a momentum oscillator that measures the speed and change of price movements.
-        It oscillates between zero and 100. Traditionally, and according to Wilder, RSI is considered
-        overbought when above 70 and oversold when below 30.
+        Calculate the Relative Strength Index (RSI) using Exponential Moving Average (EMA).
 
         :param numeric_sequence: A list of prices for a particular stock or asset.
         :param period: The period over which to calculate the RSI, typically 14.
         :return: The calculated RSI value.
         """
-        # Ensure there are enough data points to calculate RSI
         if len(numeric_sequence) < period:
             raise ValueError("Not enough data points to calculate RSI")
 
-        # Calculate the differences between consecutive prices
         deltas = [numeric_sequence[i + 1] - numeric_sequence[i] for i in range(len(numeric_sequence) - 1)]
+        gains = [max(delta, 0) for delta in deltas]
+        losses = [max(-delta, 0) for delta in deltas]
 
-        # Separate the positive gains and negative losses from the deltas
-        gains = [delta if delta > 0 else 0 for delta in deltas]
-        losses = [-delta if delta < 0 else 0 for delta in deltas]
-
-        # Calculate the initial average gain and average loss
+        # Initialize EMA with SMA for the first 'period'
         avg_gain = sum(gains[:period]) / period
         avg_loss = sum(losses[:period]) / period
 
-        # The Exponential Moving Average (EMA) for gains and losses
+        # Apply EMA formula for gains and losses
+        ema_factor = 2 / (period + 1)
         for i in range(period, len(deltas)):
-            avg_gain = ((avg_gain * (period - 1)) + gains[i]) / period
-            avg_loss = ((avg_loss * (period - 1)) + losses[i]) / period
+            avg_gain = (gains[i] * ema_factor) + (avg_gain * (1 - ema_factor))
+            avg_loss = (losses[i] * ema_factor) + (avg_loss * (1 - ema_factor))
 
-        # Calculate the Relative Strength (RS)
         rs = avg_gain / avg_loss if avg_loss != 0 else 0
-
-        # Calculate the RSI
         rsi = 100 - (100 / (1 + rs)) if avg_loss != 0 else 100
 
         return rsi
 
     @staticmethod
-    def seasonal_autoregressive_integrated_moving_average(numeric_sequence: List[int]) -> int:
+    def seasonal_autoregressive_integrated_moving_average_next_value(numeric_sequence: List[int]) -> int:
         """
         Fit a Seasonal Autoregressive Integrated Moving Average (SARIMA) model to
         the provided time series data and predict the next value in the series.
 
         SARIMA models are used to forecast future points in a time series. They are
         capable of modeling complex seasonal patterns by incorporating both non-seasonal
         (ARIMA) and seasonal elements.
@@ -625,14 +813,59 @@
 
 
 class CalculateUtil(ABC):
     """
     Compute features based on a single or multi of data
     """
 
+    @staticmethod
+    def generate_datasets_with_rolling_size(data: List[int],
+                                            rolling_size: int = 5,
+                                            adjust: bool = False) -> Tuple[List[List[int]], List[int]]:
+        """
+        Generates sequential test and validation datasets from a list of integers. It optionally adjusts
+        test datasets by removing extreme values.
+
+        The function iterates over the data to create overlapping test sets of a specified size. Each test set is
+        followed by a validation set which is the next single element in the list. If the 'adjust' flag is True,
+        the maximum and minimum values are removed from each test set.
+
+        Args:
+            data (List[int]): The input data list from which datasets are generated.
+            rolling_size (int): The number of elements in each test set. Defaults to 5.
+            adjust (bool): Whether to remove the maximum and minimum values from each test set. Defaults to False.
+
+        Returns:
+            Tuple[List[List[int]], List[int]]: A tuple containing two lists:
+                - The first list contains the test sets, possibly adjusted.
+                - The second list contains the single-element validation sets.
+        """
+        x_sets = []  # List to hold the test sets
+        y_sets = []  # List to hold the validation sets
+
+        # Iterate over the data to form test and validation sets
+        for i in range(len(data) - rolling_size):
+            test_set = data[i:i + rolling_size]  # Extract size elements for the test set
+            validation_set = data[i + rolling_size]  # Take the next element as the validation set
+
+            if len(test_set) > 2 and adjust:
+                # Remove the maximum and minimum values if adjusting
+                max_val = max(test_set)
+                min_val = min(test_set)
+                max_index = test_set.index(max_val)
+                min_index = test_set.index(min_val)
+                filtered_test_set = [x for idx, x in enumerate(test_set) if idx != max_index and idx != min_index]
+                x_sets.append(filtered_test_set)
+            else:
+                x_sets.append(test_set)  # Append the test set as is if not adjusting
+
+            y_sets.append(validation_set)  # Append the validation element
+
+        return x_sets, y_sets
+
     @classmethod
     def calculate_zone_ratio(
             cls,
             number_combination: Iterable[int],
             zone_ranges: List[Tuple[int, int]],
             **kwargs: Any
     ) -> Tuple[int, ...]:
@@ -794,15 +1027,15 @@
             # Consider 1 as a prime number for the purpose of this calculation
             if num == 1:
                 return True
             # Exclude numbers less than 1 and even numbers greater than 2 as they are not prime
             if num < 1 or (num % 2 == 0 and num > 2):
                 return False
             # Check for factors from 3 to the square root of num
-            for i in range(3, int(num**0.5) + 1, 2):
+            for i in range(3, int(num ** 0.5) + 1, 2):
                 if num % i == 0:
                     return False
             return True
 
         # Count prime numbers in the number_combination
         prime_count = sum(1 for num in number_combination if is_prime(num))
         # Count composite numbers as the remaining numbers in the number_combination
@@ -934,14 +1167,18 @@
                 # Add the absolute difference to the set of distinct differences
                 distinct_diffs.add(diff)
 
         # Return the number of distinct differences minus the number of elements minus one
         return len(distinct_diffs) - (num_count - 1)
 
     @classmethod
+    def calculate_avg(cls, number_combination: Iterable[int], **kwargs: Any) -> int:
+        return math.floor(sum(number_combination) / len(list(number_combination)))
+
+    @classmethod
     def calculate_consecutive_numbers(
             cls,
             number_combination: Iterable[int],
             **kwargs: Any
     ) -> List[List[int]]:
         """
         Calculate the sequences of consecutive numbers in a given iterable of integers.
@@ -1050,15 +1287,16 @@
         :param kwargs: Additional keyword arguments.
         :return: A tuple containing two lists - the first with 'cold numbers' and the second with 'hot numbers'.
         """
         # Convert the input to a list for indexed access
         number_combinations_list = list(number_combinations[-window:])
 
         # Determine the range for the last 5 periods
-        last_five_periods = number_combinations_list if len(number_combinations_list) >= window else number_combinations_list
+        last_five_periods = number_combinations_list if len(
+            number_combinations_list) >= window else number_combinations_list
 
         # Flatten the list of last five periods and convert to a set to remove duplicates
         numbers_in_last_five_periods: Set[int] = set(num for period in last_five_periods for num in period)
 
         # Convert all_numbers to a set for efficient lookup
         all_numbers_set: Set[int] = set(all_numbers)
 
@@ -1090,15 +1328,16 @@
         # Initialize the omission values for each number to 0
         omission_values: Dict[int, int] = {number: -1 for number in all_numbers}
 
         # Convert the input to a list for indexed access
         number_combinations_list = list(number_combinations[-window:])
 
         # Determine the range for the last 5 periods
-        last_ten_periods = number_combinations_list if len(number_combinations_list) >= window else number_combinations_list
+        last_ten_periods = number_combinations_list if len(
+            number_combinations_list) >= window else number_combinations_list
 
         # The number of draws since the last appearance
         draws_since_last_appearance = 0
 
         # Iterate over the past draws in reverse order (most recent first)
         for draw in reversed(last_ten_periods):
             # Check each number in all_numbers
@@ -1113,14 +1352,93 @@
         # For any number that hasn't appeared yet, set its omission value to the total number of draws
         for number in all_numbers:
             if omission_values[number] == -1:
                 omission_values[number] = draws_since_last_appearance
 
         return omission_values
 
+    @staticmethod
+    def calculate_standard_deviation_welford(numeric_sequence: List[Union[int, float]],
+                                             decay_factor: Union[int, float] = 0.95) -> Union[int, float]:
+        """
+        Calculates the standard deviation of a numeric sequence using Welford's method.
+
+        This method is an online algorithm designed to compute the standard deviation of a sequence of numbers
+        iteratively, which can be useful for large datasets where all data cannot be loaded into memory at once.
+
+        Args:
+            numeric_sequence (List[Union[int, float]]): The sequence of numbers (integers or floats) for which the standard deviation is to be calculated.
+            decay_factor (Union[int, float]): The decay factor for weighting recent values more heavily. Defaults to 0.95.
+
+        Returns:
+            float: The standard deviation of the sequence. Returns 0 if the sequence contains fewer than two elements.
+
+        Notes:
+            This function uses an exponential decay to weight recent observations more heavily in the calculation
+            of the mean and variance, which makes it sensitive to recent changes in the sequence.
+        """
+
+        if len(numeric_sequence) == 0:
+            raise ValueError("The numeric sequence cannot be empty.")
+        n = 0
+        mean = 0.0
+        M2 = 0.0
+        weighted_n = 0.0  # Weighted sample count
+
+        for x in numeric_sequence:
+            n += 1
+            weight = decay_factor ** (len(numeric_sequence) - n)  # Compute weight, newer data has higher weight
+            delta = x - mean
+            weighted_n += weight
+            mean += (delta * weight) / weighted_n
+            delta2 = x - mean
+            M2 += delta * delta2 * weight
+
+        if weighted_n < 2:
+            return 0.0  # Not enough samples to compute standard deviation
+        variance = M2 / weighted_n  # Compute variance using weighted sample count
+        return math.sqrt(variance)
+
+    @staticmethod
+    def calculate_standard_deviation(numeric_sequence: List[Union[int, float]]) -> Union[int, float]:
+        """
+        Calculates the standard deviation of a numeric sequence.
+
+        This method computes the standard deviation by first calculating the mean of the numbers,
+        then the variance as the average of the squared differences from the mean, and finally
+        taking the square root of the variance.
+
+        Args:
+            numeric_sequence (List[Union[int, float]]): The sequence of numbers (integers or floats) for which the standard deviation is to be calculated.
+
+        Returns:
+            float: The standard deviation of the sequence.
+
+        Raises:
+            ValueError: If the numeric_sequence is empty, as standard deviation cannot be calculated.
+        Notes:
+            This function uses an exponential decay to weight recent observations more heavily in the calculation
+            of the mean and variance, which makes it sensitive to recent changes in the sequence.
+        """
+        if len(numeric_sequence) == 0:
+            raise ValueError("The numeric sequence cannot be empty.")
+
+        # Calculate the mean of the sequence
+        mean = sum(numeric_sequence) / len(numeric_sequence)
+
+        # Calculate the squared differences from the mean
+        squared_diffs = [(x - mean) ** 2 for x in numeric_sequence]
+
+        # Calculate the variance
+        variance = sum(squared_diffs) / len(numeric_sequence)
+
+        # Calculate and return the standard deviation
+        standard_deviation = math.sqrt(variance)
+        return standard_deviation
+
     @abstractmethod
     def calculate_winning_amount(
             self,
             winning_number_combination: List[int],
             purchase_number_combinations: List[List[int]],
             **kwargs: Any
     ) -> Tuple[float, int]:
@@ -1424,15 +1742,16 @@
                 # Check diagonals
                 move_r = False
                 move_r_count = 0
                 move_c_count = 0
                 for dc in [-1, 1]:  # Check both left and right diagonals
                     count = 0
                     r, c = rows, num_index
-                    while rows - dfs_row <= r <= rows + 1 and pre_index - dfs_col <= c <= min(num_index + dfs_col, cols - 1):
+                    while rows - dfs_row <= r <= rows + 1 and pre_index - dfs_col <= c <= min(num_index + dfs_col,
+                                                                                              cols - 1):
                         if new_matrix[r][c] == 1:
                             count += 1
                         if dfs_row == dfs_col:
                             r += dr
                             c += dc
                         else:
                             if move_r:
@@ -1549,9 +1868,62 @@
             self.population = new_population
 
         # Find and return the best individual based on fitness
         best_individual = min([list(item) for item in self.population], key=self.fitness)
         return best_individual
 
 
+class RandomForestRegressorTransformer(BaseEstimator, TransformerMixin):
+    def __init__(self, model: RandomForestRegressor):
+        """
+        Initialize the transformer with a RandomForestRegressor model and a StandardScaler for feature scaling.
+
+        Parameters:
+        model (RandomForestRegressor): The RandomForestRegressor model to be used for predictions.
+        """
+        self.calculate_util = CalculateUtil
+        self.model_util = ModelUtil
+        self.model = model
+        self.scaler = StandardScaler()
+
+    def fit(self, X: np.ndarray, y: Optional[np.ndarray] = None) -> 'RandomForestRegressorTransformer':
+        """
+        Fit the RandomForest model and the scaler on the training data.
+
+        Parameters:
+        X (np.ndarray): Training data features.
+        y (Optional[np.ndarray]): Training data labels.
+
+        Returns:
+        RandomForestRegressorTransformer: The instance of this transformer.
+        """
+        X_scaled = self.scaler.fit_transform(X)
+        self.model.fit(X_scaled, y)
+        return self
+
+    def transform(self, X: np.ndarray) -> np.ndarray:
+        """
+        Transform the input data by scaling, making predictions, and calculating per-row statistics.
+
+        Parameters:
+        X (np.ndarray): Data to transform.
+
+        Returns:
+        np.ndarray: Transformed data including last elements, predictions, standard deviations, and RSI values.
+        """
+        X_scaled = self.scaler.transform(X)
+        predictions = self.model.predict(X_scaled)
+
+        # Calculate standard deviation and RSI for each row
+        sd_per_row = np.array([self.calculate_util.calculate_standard_deviation_welford(row) for row in X])
+        rsi_per_row = np.array([self.model_util.relative_strength_index(row, period=len(row) // 2) for row in X])
+
+        # Extract the last element from each row
+        last_elements = X[:, -1]
+
+        # Combine all the computed features into a single array
+        transformed_data = np.c_[last_elements, predictions, sd_per_row, rsi_per_row]
+        return transformed_data
+
+
 if __name__ == '__main__':
     pass
```

### Comparing `lottokit-0.9/lottokit.egg-info/PKG-INFO` & `lottokit-1.0/lottokit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lottokit
-Version: 0.9
+Version: 1.0
 Summary: Lotto Kit Package
 Author: nickdecodes
 Author-email: nickdecodes <nickdecodes@163.com>
 Project-URL: Documentation, http://python-lottokit.readthedocs.io
 Project-URL: Source, https://github.com/nickdecodes/python-lottokit
 Keywords: lottokit,lottery
 Requires-Python: >=3.9
```

### Comparing `lottokit-0.9/setup.py` & `lottokit-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lottokit',
-    version='0.9',
+    version='1.0',
     keywords=['lottokit', 'lottery'],
     packages=find_packages(),
     package_data={"": ["LICENSE", "NOTICE"]},
     include_package_data=True,
     author="nickdecodes",
     author_email="nickdecodes@163.com",
     description="Lotto Kit Package",
```

