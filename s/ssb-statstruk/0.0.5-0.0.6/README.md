# Comparing `tmp/ssb_statstruk-0.0.5.tar.gz` & `tmp/ssb_statstruk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_statstruk-0.0.5.tar", max compression
+gzip compressed data, was "ssb_statstruk-0.0.6.tar", max compression
```

## Comparing `ssb_statstruk-0.0.5.tar` & `ssb_statstruk-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2024-04-17 08:15:02.070561 ssb_statstruk-0.0.5/LICENSE
--rw-r--r--   0        0        0     3633 2024-04-17 08:15:02.070561 ssb_statstruk-0.0.5/README.md
--rw-r--r--   0        0        0     4218 2024-04-17 08:15:14.810610 ssb_statstruk-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       86 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/__init__.py
--rw-r--r--   0        0        0      213 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/__main__.py
--rw-r--r--   0        0        0        0 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/py.typed
--rw-r--r--   0        0        0    32529 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/ratemodel.py
--rw-r--r--   0        0        0     4899 2024-04-17 08:15:02.074561 ssb_statstruk-0.0.5/src/statstruk/ssbmodel.py
--rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 ssb_statstruk-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-26 10:13:44.186749 ssb_statstruk-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3633 2024-04-26 10:13:44.186749 ssb_statstruk-0.0.6/README.md
+-rw-r--r--   0        0        0     4218 2024-04-26 10:13:54.970770 ssb_statstruk-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       86 2024-04-26 10:13:44.190749 ssb_statstruk-0.0.6/src/statstruk/__init__.py
+-rw-r--r--   0        0        0      213 2024-04-26 10:13:44.190749 ssb_statstruk-0.0.6/src/statstruk/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:13:44.190749 ssb_statstruk-0.0.6/src/statstruk/py.typed
+-rw-r--r--   0        0        0    33914 2024-04-26 10:13:54.970770 ssb_statstruk-0.0.6/src/statstruk/ratemodel.py
+-rw-r--r--   0        0        0     4557 2024-04-26 10:13:54.970770 ssb_statstruk-0.0.6/src/statstruk/ssbmodel.py
+-rw-r--r--   0        0        0     4644 1970-01-01 00:00:00.000000 ssb_statstruk-0.0.6/PKG-INFO
```

### Comparing `ssb_statstruk-0.0.5/LICENSE` & `ssb_statstruk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_statstruk-0.0.5/README.md` & `ssb_statstruk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ssb_statstruk-0.0.5/pyproject.toml` & `ssb_statstruk-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-statstruk"
-version = "0.0.5"
+version = "0.0.6"
 description = "SSB Statstruk"
 authors = ["Susie Jentoft <coo@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/ssb-statstruk"
 repository = "https://github.com/statisticsnorway/ssb-statstruk"
 documentation = "https://statisticsnorway.github.io/ssb-statstruk"
```

### Comparing `ssb_statstruk-0.0.5/src/statstruk/ratemodel.py` & `ssb_statstruk-0.0.6/src/statstruk/ratemodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -427,24 +427,45 @@
             di_2 = ei**2 / (1.0 - hi)
             di_3 = ei**2 / ((1.0 - hi) ** 2)
 
             # Caluclate variances
             V1 = sum(ai**2 * di_1) + sum(di_1) * ai
             V2 = sum(ai**2 * di_2) + sum(di_2) * ai
             V3 = sum(ai**2 * di_3) + sum(di_3) * ai
+
+            # Adjust negative variance to zero
+            if any(x < 0 for x in [V1, V2, V3]):
+                if self.verbose == 2:
+                    print(
+                        "Negative variances calculated. These are being adjusted to 0."
+                    )
+                V1 = max(V1, 0)
+                V2 = max(V2, 0)
+                V3 = max(V3, 0)
+
             return (V1, V2, V3)
         else:
             return (0, 0, 0)
 
-    def _get_variance(self, strata: str) -> Any:
+    def _get_standard_variance(self, strata: str) -> Any:
         """Get standard variance estimates."""
         x_pop = self.strata_results[strata]["x_sum_pop"]
         x_utv = self.strata_results[strata]["x_sum_sample"]
         s2 = self.strata_results[strata]["sigma2"]
-        V = x_pop**2 * (x_pop - x_utv) / x_pop * s2 / x_utv
+
+        if (x_pop > 0) and (x_utv > 0):
+            V = x_pop**2 * (x_pop - x_utv) / x_pop * s2 / x_utv
+        else:
+            V = np.nan
+
+        if V < 0:
+            if self.verbose == 2:
+                print("Negative variances calculated. These are being adjusted to 0.")
+            V = 0
+
         return V
 
     def _get_domain_estimates(self, domain: str, uncertainty_type: str) -> pd.DataFrame:
         """Get domain estimation for case where domains are not an aggregation of strata."""
         # Collect data
         self._add_flag()
         pop = self.get_imputed()  # add imputed y values
@@ -459,56 +480,106 @@
         # loop through domains and calculate variance
         for d in domain_unique:
             temp_dom = pop.loc[pop[domain] == d]
 
             # Get additional domain information on sample, pop sizes and estimates
             N = temp_dom.shape[0]
             n = np.sum(temp_dom[self.flag_var] == 1)
-            est = np.sum(temp_dom[f"{self.y_var}_imputed"])
+            est = np.sum(temp_dom[f"{self.y_var}_imp"])
 
             # Loop through strata to get the partial variances
             var = 0
+            x_sum_sample = 0
+            x_sum_pop = 0
             for s in strata_unique:
                 mask_s = (temp_dom[strata_var] == s) & (
                     temp_dom[self.flag_var] == 0
                 )  # Those not in sample
-                Uh_sh = np.sum(temp_dom.loc[mask_s, self.x_var])
-                xh = res[s]["x_sum_sample"]
+                Uh_sh = np.sum(
+                    temp_dom.loc[mask_s, self.x_var]
+                )  # Sum of x not in sample
+                xh = res[s]["x_sum_sample"]  # Sum of x in sample
                 s2 = res[s]["sigma2"]
-                var += s2 * (Uh_sh + xh) / xh * Uh_sh
+                x_sum_pop += np.sum(temp_dom.loc[temp_dom[strata_var] == s, self.x_var])
+                x_sum_sample += np.sum(
+                    temp_dom.loc[
+                        (temp_dom[strata_var] == s) & (temp_dom[self.flag_var] == 1),
+                        self.x_var,
+                    ]
+                )
+
+                # Add in variance for stratum if sum of x is greater than 0 and var is not na or inf!!!
+                if (xh > 0) & (not np.isinf(s2)) & (not np.isnan(s2)):
+                    var += s2 * Uh_sh * ((Uh_sh + xh) / xh)
 
             # Add calculations to domain dict
             domain_df[d] = {
                 "domain": d,
                 "N": N,
                 "n": n,
+                f"{self.x_var}_sum_pop": x_sum_pop,
+                f"{self.x_var}_sum_sample": x_sum_sample,
                 f"{self.y_var}_EST": est,
                 f"{self.y_var}_VAR": var,
-                f"{self.y_var}_SE": np.sqrt(var),
-                f"{self.y_var}_LB": est - (1.96 * np.sqrt(var)),
-                f"{self.y_var}_UB": est + (1.96 * np.sqrt(var)),
-                f"{self.y_var}_CV": np.sqrt(var) / est * 100,
             }
 
-        # Format and drop variables that are not asked for
-        domain_pd = pd.DataFrame(domain_df).T
+        # Convert to pandas
+        domain_pd = pd.DataFrame([v for k, v in domain_df.items()])
+        domain_pd = self._clean_output(
+            domain_pd,
+            uncertainty_type=uncertainty_type,
+            variance_type="standard",
+            return_type="unbiased",
+        )
 
-        if "CV" not in uncertainty_type:
-            domain_pd = domain_pd.drop([f"{self.y_var}_CV"], axis=1)
+        return domain_pd
 
-        if "SE" not in uncertainty_type:
-            domain_pd = domain_pd.drop([f"{self.y_var}_SE"], axis=1)
+    def _clean_output(
+        self,
+        result: pd.DataFrame,
+        uncertainty_type: str,
+        variance_type: str,
+        return_type: str,
+    ) -> pd.DataFrame:
+        """Clean up results set to include the chosen return type."""
+        y_var = self.y_var
 
-        if "CI" not in uncertainty_type:
-            domain_pd = domain_pd.drop([f"{self.y_var}_LB", f"{self.y_var}_UB"], axis=1)
+        # Format and add in CV, SE, CI
+        if variance_type == "standard":
+            variance_list = [""]
+        if (variance_type == "robust") & (return_type == "unbiased"):
+            variance_list = ["2"]
+        if (variance_type == "robust") & (return_type == "all"):
+            variance_list = ["1", "2", "3"]
+
+        for i in variance_list:
+            if "CV" in uncertainty_type:
+                result[f"{y_var}_CV{i}"] = (
+                    np.sqrt(result[f"{y_var}_VAR{i}"]) / result[f"{y_var}_EST"] * 100
+                )
 
-        if "VAR" not in uncertainty_type:
-            domain_pd = domain_pd.drop([f"{self.y_var}_VAR"], axis=1)
+            if "SE" in uncertainty_type:
+                result[f"{y_var}_SE{i}"] = np.sqrt(result[f"{y_var}_VAR{i}"])
 
-        return domain_pd
+            if "CI" in uncertainty_type:
+                result[f"{y_var}_LB{i}"] = result[f"{y_var}_EST"] - (
+                    1.96 * np.sqrt(result[f"{y_var}_VAR{i}"])
+                )
+                result[f"{y_var}_UB{i}"] = result[f"{y_var}_EST"] + (
+                    1.96 * np.sqrt(result[f"{y_var}_VAR{i}"])
+                )
+
+            if "VAR" not in uncertainty_type:
+                result = result.drop([f"{y_var}_VAR{i}"], axis=1)
+
+            if (return_type == "unbiased") & (variance_type == "robust"):
+                result = result.drop([f"{y_var}_VAR1"], axis=1)
+                result = result.drop([f"{y_var}_VAR3"], axis=1)
+
+        return result
 
     def _get_domain(self, domain: str) -> Any:
         """Get mapping of domain to the strata results."""
         strata_var = "_strata_var_mod"
 
         # create key form population file
         pop = self.pop_data[[strata_var, domain]]
@@ -527,15 +598,15 @@
         assert (
             len(one_to_many) == 0
         ), "1-to-many relationship(s) found in strata/domain aggregation. Only aggregated variances are programmed."
 
         # map key
         strata_res = pd.DataFrame(self.strata_results).T
         domain_mapped = strata_res["_strata_var_mod"].map(domain_key)
-        # print(f"domain mapped: {type(domain_mapped)}")
+
         return domain_mapped.str[0]
 
     def get_estimates(
         self,
         domain: str = "",
         uncertainty_type: str = "CV",
         variance_type: str = "robust",
@@ -573,33 +644,29 @@
                 )
             return self._get_domain_estimates(domain, uncertainty_type)
 
         # Format variables
         strata_df["N"] = pd.to_numeric(strata_df["N"])
         strata_df["n"] = pd.to_numeric(strata_df["n"])
 
-        strata_df["x_sum_sample"] = pd.to_numeric(strata_df["x_sum_sample"])
-        strata_df["x_sum_pop"] = pd.to_numeric(strata_df["x_sum_pop"])
+        strata_df[f"{self.x_var}_sum_pop"] = pd.to_numeric(strata_df["x_sum_pop"])
+        strata_df[f"{self.x_var}_sum_sample"] = pd.to_numeric(strata_df["x_sum_sample"])
 
         # Add estimates
         strata_df["beta"] = pd.to_numeric(strata_df["beta"])
         strata_df[f"{self.y_var}_EST"] = pd.to_numeric(
             strata_df["beta"] * strata_df["x_sum_pop"]
         )
 
         # Add variance standard or robust
         if variance_type == "standard":
             var1 = []
             for s in strata_df["_strata_var_mod"]:
-                var1.append(self._get_variance(s))
+                var1.append(self._get_standard_variance(s))
 
-            # Check for negative variances
-            if any(x < 0 for x in var1):
-                print("Negative variances calculated. These are being adjusted to 0.")
-                var1 = [i if i >= 0 else 0 for i in var1]
             strata_df[f"{self.y_var}_VAR"] = np.array(var1)
 
             # Aggregate to domain
             result = (
                 strata_df[[domain, "N", "n", f"{self.y_var}_EST", f"{self.y_var}_VAR"]]
                 .groupby(domain)
                 .sum()
@@ -611,74 +678,46 @@
             for s in strata_df["_strata_var_mod"]:
                 var = self._get_robust(s)
                 if isinstance(var, tuple):
                     var1.append(var[0])
                     var2.append(var[1])
                     var3.append(var[2])
 
-            # Adjust negative variance to zero
-            if any(x < 0 for x in var1 + var2 + var3):
-                print("Negative variances calculated. These are being adjusted to 0.")
-            strata_df[f"{self.y_var}_VAR1"] = np.array(
-                [i if i >= 0 else 0 for i in var1]
-            )
-            strata_df[f"{self.y_var}_VAR2"] = np.array(
-                [i if i >= 0 else 0 for i in var2]
-            )
-            strata_df[f"{self.y_var}_VAR3"] = np.array(
-                [i if i >= 0 else 0 for i in var3]
-            )
+            # Add to results
+            variables = ["VAR1", "VAR2", "VAR3"]
+            variance_list = [var1, var2, var3]
+            for var_name, data in zip(variables, variance_list, strict=False):
+                strata_df[f"{self.y_var}_{var_name}"] = data
 
             # Aggregate to domain
             result = (
                 strata_df[
                     [
                         domain,
                         "N",
                         "n",
+                        f"{self.x_var}_sum_pop",
+                        f"{self.x_var}_sum_sample",
                         f"{self.y_var}_EST",
                         f"{self.y_var}_VAR1",
                         f"{self.y_var}_VAR2",
                         f"{self.y_var}_VAR3",
                     ]
                 ]
                 .groupby(domain)
                 .sum()
             )
 
         # Format and add in CV, SE, CI
-        if variance_type == "standard":
-            variance_list = [""]
-        if (variance_type == "robust") & (return_type == "unbiased"):
-            variance_list = ["2"]
-        if (variance_type == "robust") & (return_type == "all"):
-            variance_list = ["1", "2", "3"]
-
-        for i in variance_list:
-
-            if "CV" in uncertainty_type:
-                result[f"{self.y_var}_CV{i}"] = (
-                    np.sqrt(result[f"{self.y_var}_VAR{i}"])
-                    / result[f"{self.y_var}_EST"]
-                    * 100
-                )
-
-            if "SE" in uncertainty_type:
-                result[f"{self.y_var}_SE{i}"] = np.sqrt(result[f"{self.y_var}_VAR{i}"])
-
-            if "CI" in uncertainty_type:
-                result[f"{self.y_var}_LB{i}"] = result[f"{self.y_var}_EST"] - (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR{i}"])
-                )
-                result[f"{self.y_var}_UB{i}"] = result[f"{self.y_var}_EST"] + (
-                    1.96 * np.sqrt(result[f"{self.y_var}_VAR{i}"])
-                )
-
-            if "VAR" not in uncertainty_type:
-                result = result.drop([f"{self.y_var}_VAR{i}"], axis=1)
+        result = self._clean_output(
+            result,
+            uncertainty_type=uncertainty_type,
+            variance_type=variance_type,
+            return_type=return_type,
+        )
 
         return result
 
     def get_extremes(
         self, threshold_type: str = "both", rbound: float = 2, gbound: float = 2
     ) -> pd.DataFrame:
         """Get observations with extreme values based on their rstudized residual value or G value.
@@ -753,20 +792,20 @@
         def _get_beta(stratum: str) -> Any:
             """Get beta values from model for stratum."""
             return self.strata_results.get(stratum, {}).get("beta", None)
 
         pop["beta"] = pop["_strata_var_mod"].apply(_get_beta)
 
         # Calculate imputed values
-        pop[f"{self.y_var}_imputed"] = pop["beta"] * pop[self.x_var]
+        pop[f"{self.y_var}_imp"] = pop["beta"] * pop[self.x_var]
 
         # Link in survey values
         id_to_yvar_map = utvalg.set_index(self.id_nr)[self.y_var]
-        pop[f"{self.y_var}_imputed"] = (
-            pop[self.id_nr].map(id_to_yvar_map).fillna(pop[f"{self.y_var}_imputed"])
+        pop[f"{self.y_var}_imp"] = (
+            pop[self.id_nr].map(id_to_yvar_map).fillna(pop[f"{self.y_var}_imp"])
         )
         pop_pd = pd.DataFrame(pop)
         return pop_pd
 
     def get_weights(self) -> pd.DataFrame:
         """Get sample data with weights based on model.
 
@@ -801,7 +840,15 @@
 
         is_rstud_present = "rstud" in next(iter(self.obs_data.values()))
 
         if not is_rstud_present:
             raise RuntimeError(
                 "Model has not been fitted for calculating extreme values. Please re-run fit() with control_extremes = True"
             )
+
+    def _add_flag(self) -> None:
+        """Add flag in population data to say if unit is in the sample or not."""
+        self.flag_var = f"{self.y_var}_flag_sample"
+        sample_ids = set(self.sample_data[self.id_nr])
+        self.pop_data[self.flag_var] = self.pop_data[self.id_nr].apply(
+            lambda x: 1 if x in sample_ids else 0
+        )
```

### Comparing `ssb_statstruk-0.0.5/src/statstruk/ssbmodel.py` & `ssb_statstruk-0.0.6/src/statstruk/ssbmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -98,22 +98,14 @@
         else:
             # Give error for missing values
             if value.isna().any():
                 raise ValueError(
                     f"Variable '{var_name}' contains missing values. Please fix and try again."
                 )
 
-    def _add_flag(self) -> None:
-        """Add flag in population data to say if unit is in the sample or not."""
-        self.flag_var = "_flag_sample"
-        sample_ids = set(self.sample_data[self.id_nr])
-        self.pop_data[self.flag_var] = self.pop_data[self.id_nr].apply(
-            lambda x: 1 if x in sample_ids else 0
-        )
-
     def _check_model_run(self) -> None:
         """Check to ensure that model has been run before proceeding with other functions."""
         if not hasattr(self, "strata_results"):
             raise RuntimeError("Model has not been run. Please run fit() first")
 
     def _convert_var(self, var_name: str, dataset: pd.DataFrame) -> None:
         if dataset[var_name].dtype == "Int64":
```

### Comparing `ssb_statstruk-0.0.5/PKG-INFO` & `ssb_statstruk-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-statstruk
-Version: 0.0.5
+Version: 0.0.6
 Summary: SSB Statstruk
 Home-page: https://github.com/statisticsnorway/ssb-statstruk
 License: MIT
 Author: Susie Jentoft
 Author-email: coo@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

