# Comparing `tmp/bblib-1.2.1.tar.gz` & `tmp/bblib-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-1.2.1.tar", max compression
+gzip compressed data, was "bblib-2.0.0.tar", max compression
```

## Comparing `bblib-1.2.1.tar` & `bblib-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-04-15 09:19:19.691922 bblib-1.2.1/LICENSE
--rw-r--r--   0        0        0     3753 2024-04-15 09:19:19.691922 bblib-1.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/__init__.py
--rwxr-xr-x   0        0        0    35521 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/methods.py
--rwxr-xr-x   0        0        0     9226 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/models.py
--rwxr-xr-x   0        0        0    18198 2024-04-15 09:19:19.691922 bblib-1.2.1/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-04-15 09:19:29.111997 bblib-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-04-26 13:21:02.375355 bblib-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3753 2024-04-26 13:21:02.375355 bblib-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 13:21:02.375355 bblib-2.0.0/bblib/__init__.py
+-rwxr-xr-x   0        0        0    37001 2024-04-26 13:21:02.375355 bblib-2.0.0/bblib/methods.py
+-rwxr-xr-x   0        0        0     9961 2024-04-26 13:21:02.379356 bblib-2.0.0/bblib/models.py
+-rwxr-xr-x   0        0        0    18198 2024-04-26 13:21:02.379356 bblib-2.0.0/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-04-26 13:21:22.327287 bblib-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 bblib-2.0.0/PKG-INFO
```

### Comparing `bblib-1.2.1/LICENSE` & `bblib-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-1.2.1/README.md` & `bblib-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bblib-1.2.1/bblib/methods.py` & `bblib-2.0.0/bblib/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,20 +114,28 @@
         center = center_of_mass(self.visual_data, self.mask_for_center_of_mass)
         if self.centering_converged(center):
             center[0] += self.config["offset"]["x"]
             center[1] += self.config["offset"]["y"]
 
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
-            ax1.imshow(
-                self.visual_data * self.mask_for_center_of_mass,
-                norm=LogNorm(),
-                cmap="YlGn",
-                origin="lower",
-            )
+            if self.plots_info["value_auto"]:
+                ax1.imshow(
+                    self.visual_data * self.mask_for_center_of_mass,
+                    norm=LogNorm(),
+                    cmap="spring",
+                    origin="lower",
+                )
+            else: 
+                ax1.imshow(
+                    self.visual_data * self.mask_for_center_of_mass,
+                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+                    cmap="spring",
+                    origin="lower",
+                )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
                 marker="o",
                 label=f"Initial detector center: ({np.round(self.initial_detector_center[0])}, {np.round(self.initial_detector_center[1])})",
             )
@@ -139,14 +147,18 @@
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_of_mass/'
             )
             path.mkdir(parents=True, exist_ok=True)
             ax1.legend()
+            if not self.plots_info["axis_lim_auto"]:
+                ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
+                ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
+
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_of_mass/{self.plots_info["file_name"]}.png'
             )
             plt.close()
         return np.round(center, 0)
 
 
@@ -253,20 +265,28 @@
         else:
             xc = -1
             yc = -1
 
         center = [xc, yc]
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
-            ax1.imshow(
-                self.visual_data * self.mask_for_circle_detection,
-                norm=LogNorm(),
-                origin="lower",
-                cmap="YlGn",
-            )
+            if self.plots_info["value_auto"]:
+                ax1.imshow(
+                    self.visual_data * self.mask_for_circle_detection,
+                    norm=LogNorm(),
+                    origin="lower",
+                    cmap="spring",
+                )
+            else:
+                ax1.imshow(
+                    self.visual_data * self.mask_for_circle_detection,
+                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+                    origin="lower",
+                    cmap="spring",
+                )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
                 marker="o",
                 label=f"Initial detector center: ({np.round(self.initial_detector_center[0])}, {np.round(self.initial_detector_center[1])})",
             )
@@ -278,14 +298,17 @@
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_circle_detection/'
             )
             path.mkdir(parents=True, exist_ok=True)
             ax1.legend()
+            if not self.plots_info["axis_lim_auto"]:
+                ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
+                ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_circle_detection/{self.plots_info["file_name"]}.png'
             )
             plt.close()
         return center
 
 
@@ -371,16 +394,16 @@
                 x_fit,
                 y_fit,
                 "r--",
                 label=f"gaussian fit \n a:{round(popt[0],2)} \n x0:{round(popt[1],2)} \n sigma:{round(popt[2],2)} \n R² {round(r_squared, 4)}\n FWHM : {round(fwhm,3)}",
             )
 
             plt.title("Azimuthal integration")
-            plt.xlim(0, 500)
-            plt.ylim(0, 5)
+            #plt.xlim(0, 500)
+            #plt.ylim(0, 5)
             plt.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/radial_average/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/radial_average/{self.plots_info["file_name"]}.png'
@@ -486,22 +509,22 @@
             n=self.config["pixels_for_mask_of_bragg_peaks"],
         )
         self.mask_for_fwhm_min = only_peaks_mask * visual_mask
 
         self.pixel_step = 1
         xx, yy = np.meshgrid(
             np.arange(
-                self.initial_guess[0] - self.config["outlier_distance"],
-                self.initial_guess[0] + self.config["outlier_distance"] + 1,
+                self.initial_guess[0] - 20,
+                self.initial_guess[0] + 21,
                 self.pixel_step,
                 dtype=int,
             ),
             np.arange(
-                self.initial_guess[1] - self.config["outlier_distance"],
-                self.initial_guess[1] + self.config["outlier_distance"] + 1,
+                self.initial_guess[1] - 20,
+                self.initial_guess[1] + 21,
                 self.pixel_step,
                 dtype=int,
             ),
         )
         coordinates = np.column_stack((np.ravel(xx), np.ravel(yy)))
 
         ## TEST avoid effects from secondary peaks
@@ -530,20 +553,28 @@
         if self.centering_converged(center):
             self.plot_fwhm_flag = True
             self._calculate_fwhm(center)
             self.plot_fwhm_flag = False
 
         if self.config["plots_flag"]:
             fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
-            ax1.imshow(
-                self.visual_data * self.mask_for_fwhm_min,
-                norm=LogNorm(),
-                origin="lower",
-                cmap="YlGn",
-            )
+            if self.plots_info["value_auto"]:
+                ax1.imshow(
+                    self.visual_data * self.mask_for_fwhm_min,
+                    norm=LogNorm(),
+                    origin="lower",
+                    cmap="spring",
+                )
+            else:
+                ax1.imshow(
+                    self.visual_data * self.mask_for_fwhm_min,
+                    norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]),
+                    origin="lower",
+                    cmap="spring",
+                )
             ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="blue",
                 marker="o",
                 label=f"Initial detector center: ({np.round(self.initial_detector_center[0])}, {np.round(self.initial_detector_center[1])})",
             )
@@ -562,14 +593,17 @@
                 label=f"Refined detector center: ({center[0]}, {center[1]})",
             )
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_fwhm_minimization/'
             )
             path.mkdir(parents=True, exist_ok=True)
             ax1.legend()
+            if not self.plots_info["axis_lim_auto"]:
+                ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
+                ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/center_fwhm_minimization/{self.plots_info["file_name"]}.png'
             )
             plt.close()
 
         return center
 
@@ -586,98 +620,66 @@
         
         if not config["plots_flag"] and not plots_info:
             plots_info =  {
 	        "file_name": "",
 	        "folder_name": "",
 	        "root_path": ""
             }
-    def _remove_repeated_pairs(self, pairs_list: list) -> list:
-        x_vector = []
-        y_vector = []
-        unique_pairs = []
-
-        for pair in pairs_list:
-            peak_0, peak_1 = pair
-            x = peak_0[0] - peak_1[0]
-            y = peak_0[1] - peak_1[1]
-            if x not in x_vector and y not in y_vector:
-                x_vector.append(x)
-                y_vector.append(y)
-                unique_pairs.append((peak_0, peak_1))
-        return unique_pairs
-
-    def _shift_inverted_peaks_and_calculate_minimum_distance(
-        self,
-        shift: list,
-    ) -> dict:
-        peaks_list = self.peaks_list_original.copy()
-        inverted_peaks = self.peaks_list_inverted.copy()
-
-        shifted_inverted_peaks = [
-            (x + shift[0], y + shift[1]) for x, y in inverted_peaks
-        ]
-        distance = self.calculate_pair_distance(peaks_list, shifted_inverted_peaks)
-
-        return {
-            "shift_x": shift[0],
-            "xc": (shift[0] / 2) + self.initial_guess[0] + 0.5,
-            "shift_y": shift[1],
-            "yc": (shift[1] / 2) + self.initial_guess[1] + 0.5,
-            "d": distance,
-        }
-
-    def calculate_pair_distance(
-        self, peaks_list: list, shifted_peaks_list: list
-    ) -> float:
-        d = [
-            math.sqrt(
-                (peaks_list[idx][0] - i[0]) ** 2 + (peaks_list[idx][1] - i[1]) ** 2
-            )
-            for idx, i in enumerate(shifted_peaks_list)
-        ]
-        return sum(d)
 
     def _select_closest_peaks(self, peaks_list: list, inverted_peaks: list) -> list:
-        peaks = []
-        for i in inverted_peaks:
-            radius = 1
+        pairs_list = []
+        for i in peaks_list:
+            radius = 0.1
             found_peak = False
             while not found_peak and radius <= self.config["search_radius"]:
-                found_peak = self._find_a_peak_in_the_surrounding(peaks_list, i, radius)
-                radius += 1
+                found_peak = self._find_a_peak_in_the_surrounding(i, inverted_peaks, radius)
+                radius += 0.1
             if found_peak:
-                peaks.append((found_peak, i))
-        # peaks = self._remove_repeated_pairs(peaks)
-        return peaks
+                pairs_list.append((i, found_peak))
+        pairs_list = self._check_paired_reflections(pairs_list)
+        return pairs_list
 
     def _find_a_peak_in_the_surrounding(
-        self, peaks_list: list, inverted_peak: list, radius: int
+        self, peak: list, inverted_peaks_list: list, radius: float
     ) -> list:
         cut_peaks_list = []
         cut_peaks_list = [
             (
-                peak,
+                inverted_peak,
                 math.sqrt(
                     (peak[0] - inverted_peak[0]) ** 2
                     + (peak[1] - inverted_peak[1]) ** 2
                 ),
             )
-            for peak in peaks_list
+            for inverted_peak in inverted_peaks_list
             if math.sqrt(
                 (peak[0] - inverted_peak[0]) ** 2 + (peak[1] - inverted_peak[1]) ** 2
             )
             <= radius
         ]
         cut_peaks_list.sort(key=lambda x: x[1])
 
         if cut_peaks_list == []:
             return False
         else:
             return cut_peaks_list[0][0]
 
+    def _check_paired_reflections(self, pairs_list:list)-> list:
+        ## check if the reversed peak is also on the list
+        filtered_pairs = []
+        
+        for original_peak, inverted_peak in pairs_list:
+            inverted_peak_inverted_twice = (-1*inverted_peak[0],-1*inverted_peak[1])
+            original_peak_inverted_twice = (-1*original_peak[0],-1*original_peak[1])
+            inverted_pair=(inverted_peak_inverted_twice,original_peak_inverted_twice)
+            if inverted_pair in pairs_list:
+                filtered_pairs.append((original_peak, inverted_peak))
+
+        return filtered_pairs
+
     def _prep_for_centering(self, data: np.ndarray, initial_guess: tuple) -> None:
 
         self.initial_guess = initial_guess
         self.initial_detector_center = self.PF8Config.get_detector_center()
         non_shifted_pixel_maps_for_visualization = self.PF8Config.pixel_maps.copy()
 
         ## Find peaks
@@ -746,108 +748,99 @@
                 visual_mask = visualize_single_panel(
                     mask,
                     self.PF8Config.transformation_matrix,
                     self.PF8Config.ss_in_rows,
                 )
 
         peak_list_in_slab = pf8.peak_list_in_slab(peak_list)
-        #print(peak_list_in_slab)
         self.peak_list_x_in_frame, self.peak_list_y_in_frame = peak_list_in_slab
 
     def _run_centering(self, **kwargs) -> tuple:
        
         peak_list_x_in_frame = self.peak_list_x_in_frame.copy()
         peak_list_y_in_frame = self.peak_list_y_in_frame.copy()
 
         peaks = list(zip(peak_list_x_in_frame, peak_list_y_in_frame))
         inverted_peaks_x = [-1 * k for k in peak_list_x_in_frame]
         inverted_peaks_y = [-1 * k for k in peak_list_y_in_frame]
         inverted_peaks = list(zip(inverted_peaks_x, inverted_peaks_y))
         pairs_list = self._select_closest_peaks(peaks, inverted_peaks)
 
-        ## Grid search of shifts around the detector center
-        self.pixel_step = 0.2
-        xx, yy = np.meshgrid(
-            np.arange(
-                -self.config["outlier_distance"],
-                self.config["outlier_distance"] + 0.2,
-                self.pixel_step,
-                dtype=float,
-            ),
-            np.arange(
-                -self.config["outlier_distance"],
-                self.config["outlier_distance"] + 0.2,
-                self.pixel_step,
-                dtype=float,
-            ),
-        )
-        coordinates = np.column_stack((np.ravel(xx), np.ravel(yy)))
+        ## Calculcate the beam center shift
+        
         self.peaks_list_original = [x for x, y in pairs_list]
         self.peaks_list_inverted = [y for x, y in pairs_list]
 
-        pool = multiprocessing.Pool()
-        with pool:
-            distance_summary = pool.map(
-                self._shift_inverted_peaks_and_calculate_minimum_distance, coordinates
-            )
-
-        ## Minimize distance
-        if self.config["plots_flag"]:
-            path = pathlib.Path(
-                f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/distance_map/'
-            )
-            path.mkdir(parents=True, exist_ok=True)
-
-        center = get_distance_map_global_min(
-            distance_summary,
-            f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}',
-            f'{self.plots_info["file_name"]}',
-            self.pixel_step,
-            self.config["plots_flag"],
-        )
+        if len(pairs_list)>0:
+            print(f"--------------  Friedel pairs search --------------\nNumber of Friedel Pairs in frame: {len(pairs_list)/2}")
+            print(f"Pairs list for debug:")
+            print(pairs_list)
 
+            friedel_coordinates_in_x = [x for x, y in self.peaks_list_original]
+            friedel_coordinates_in_y = [y for x, y in self.peaks_list_original]
+            
+            print(f"Friedel pairs position before center correction in pixels:")
+            print(self.peaks_list_original)
+            
+            shift_x = sum(friedel_coordinates_in_x)/len(friedel_coordinates_in_x)
+            shift_y = sum(friedel_coordinates_in_y)/len(friedel_coordinates_in_y)
+            print("Center shift in x", shift_x)
+            print("Center shift in y", shift_y)
+            center = [self.initial_guess[0]+shift_x, self.initial_guess[1]+shift_y]
+
+            print(f"Friedel pairs position after center correction in pixels:")
+            pairs_list_after_correction=[(x[0]-shift_x, x[1]-shift_y) for x in self.peaks_list_original]
+            print(pairs_list_after_correction)
+        else:
+            center = [-1, -1]
 
         if self.config["plots_flag"] and self.centering_converged(center):
-            shift_x = 2 * (center[0] - self.initial_guess[0])
-            shift_y = 2 * (center[1] - self.initial_guess[1])
 
-            fig, ax = plt.subplots(1, 1, figsize=(10, 10))
-            pos = ax.imshow(
-                self.visual_data, norm=LogNorm(), cmap="YlGn", origin="lower"
-            )
-            ax.scatter(
+            fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
+            if self.plots_info["value_auto"]:
+                pos = ax1.imshow(
+                    self.visual_data, norm=LogNorm(), cmap="spring", origin="lower"
+                )
+            else:
+                pos = ax1.imshow(
+                    self.visual_data, norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]), cmap="spring", origin="lower"
+                )
+            ax1.scatter(
                 self.initial_detector_center[0],
                 self.initial_detector_center[1],
                 color="b",
                 marker="o",
                 s=25,
                 label=f"Initial detector center:({np.round(self.initial_detector_center[0],1)},{np.round(self.initial_detector_center[1], 1)})",
             )
-            ax.scatter(
+            ax1.scatter(
                 self.initial_guess[0],
                 self.initial_guess[1],
                 color="lime",
                 marker="+",
                 s=150,
                 label=f"Initial guess:({np.round(self.initial_guess[0],1)},{np.round(self.initial_guess[1], 1)})",
             )
 
-            ax.scatter(
+            ax1.scatter(
                 center[0],
                 center[1],
                 color="r",
                 marker="o",
                 s=25,
                 label=f"Refined detector center:({np.round(center[0],1)}, {np.round(center[1],1)})",
             )
-            ax.set_xlim(200, 900)
-            ax.set_ylim(200, 900)
+            
             plt.title("Center refinement: autocorrelation of Friedel pairs")
             fig.colorbar(pos, shrink=0.6)
-            ax.legend()
+            ax1.legend()
+            if not self.plots_info["axis_lim_auto"]:
+                ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
+                ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
+
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/centered_friedel/{self.plots_info["file_name"]}.png'
             )
@@ -857,70 +850,78 @@
                 np.round(k + self.initial_guess[0]) for k in peak_list_x_in_frame
             ]
             original_peaks_y = [
                 np.round(k + self.initial_guess[1]) for k in peak_list_y_in_frame
             ]
 
             inverted_non_shifted_peaks_x = [
-                np.round(k + self.initial_guess[0]) for k in inverted_peaks_x
+                np.round(k[0] + self.initial_guess[0]) for k in self.peaks_list_inverted
             ]
             inverted_non_shifted_peaks_y = [
-                np.round(k + self.initial_guess[1]) for k in inverted_peaks_y
+                np.round(k[1] + self.initial_guess[1]) for k in self.peaks_list_inverted
             ]
             inverted_shifted_peaks_x = [
-                np.round(k + self.initial_guess[0] + shift_x) for k in inverted_peaks_x
+                np.round(k[0] + self.initial_guess[0] + shift_x) for k in self.peaks_list_inverted
             ]
             inverted_shifted_peaks_y = [
-                np.round(k + self.initial_guess[1] + shift_y) for k in inverted_peaks_y
+                np.round(k[1] + self.initial_guess[1] + shift_y) for k in self.peaks_list_inverted
             ]
 
             ## Check pairs alignement
-            fig, ax = plt.subplots(1, 1, figsize=(10, 10))
-            pos = ax.imshow(
-                self.visual_data, norm=LogNorm(), cmap="YlGn", origin="lower"
-            )
-            ax.scatter(
+            fig, ax1 = plt.subplots(1, 1, figsize=(10, 10))
+            if self.plots_info["value_auto"]:
+                pos = ax1.imshow(
+                    self.visual_data, norm=LogNorm(), cmap="spring", origin="lower"
+                )
+            else:
+                pos = ax1.imshow(
+                    self.visual_data, norm=LogNorm(self.plots_info["value_min"], self.plots_info["value_max"]), cmap="spring", origin="lower"
+                )
+                
+            ax1.scatter(
                 original_peaks_x,
                 original_peaks_y,
                 facecolor="none",
                 s=80,
                 marker="s",
                 edgecolor="red",
                 linewidth=1.5,
                 label="original peaks",
             )
             
-            ax.scatter(
+            ax1.scatter(
                 inverted_non_shifted_peaks_x,
                 inverted_non_shifted_peaks_y,
                 s=80,
                 facecolor="none",
                 marker="s",
                 edgecolor="tab:orange",
                 linewidth=1.5,
                 label="inverted peaks",
                 alpha=0.8,
             )
-            ax.scatter(
+            ax1.scatter(
                 inverted_shifted_peaks_x,
                 inverted_shifted_peaks_y,
                 facecolor="none",
                 s=120,
                 marker="D",
                 linewidth=1.8,
                 alpha=0.8,
                 edgecolor="blue",
                 label="shift of inverted peaks",
             )
             
-            ax.set_xlim(200, 900)
-            ax.set_ylim(200, 900)
+            if not self.plots_info["axis_lim_auto"]:
+                ax1.set_xlim(self.plots_info["xlim_min"], self.plots_info["xlim_max"])
+                ax1.set_ylim(self.plots_info["ylim_min"], self.plots_info["ylim_max"])
+            
             plt.title("Bragg peaks alignement")
             fig.colorbar(pos, shrink=0.6)
-            ax.legend()
+            ax1.legend()
             path = pathlib.Path(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/peaks/'
             )
             path.mkdir(parents=True, exist_ok=True)
             plt.savefig(
                 f'{self.plots_info["root_path"]}/center_refinement/plots/{self.plots_info["folder_name"]}/peaks/{self.plots_info["file_name"]}.png'
             )
```

### Comparing `bblib-1.2.1/bblib/models.py` & `bblib-2.0.0/bblib/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,23 +50,40 @@
 
     def set_geometry_from_file(self, geometry_filename: str = None):
         if geometry_filename:
             self.geometry_txt = open(geometry_filename, "r").readlines()
         else:
             if not self.geometry_txt:
                 raise ValueError("Please, specify the detector geometry in CrystFEL format.")
+        
+        # Passing bad pixel maps to PF8. 
+        # Warning! It will look for campus in the geom file either 'mask0_file' or 'mask_file'. 
+        # It doesn't look for multiple masks. 
+        # It assumes bad pixels as zeros and good pixels as ones.
+        try:
+            self.bad_pixel_map_filename = [
+                x.split(" = ")[-1][:-1]
+                for x in self.geometry_txt
+                if x.split(" = ")[0] == "mask0_file"
+            ][0]
+        except IndexError:
+            self.bad_pixel_map_filename = [
+               x.split(" = ")[-1][:-1]
+                for x in self.geometry_txt
+                if x.split(" = ")[0] == "mask_file"
+            ][0]
 
-        self.bad_pixel_map_filename = [
-            x.split(" = ")[-1][:-1]
-            for x in self.geometry_txt
-            if x.split(" = ")[0] == "mask_file"
-        ][0]
-        self.bad_pixel_map_hdf5_path = [
-            x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask"
-        ][0]
+        try:
+            self.bad_pixel_map_hdf5_path = [
+                x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask0_data"
+            ][0]
+        except IndexError:
+            self.bad_pixel_map_hdf5_path = [
+                x.split(" = ")[-1][:-1] for x in self.geometry_txt if x.split(" = ")[0] == "mask"
+            ][0]
 
         geom = GeometryInformation(
             geometry_description=self.geometry_txt, geometry_format="crystfel"
         )
         self.pixel_resolution = 1 / geom.get_pixel_size()
         self.pixel_maps = geom.get_pixel_maps()
         self._data_shape = self.pixel_maps["x"].shape
```

### Comparing `bblib-1.2.1/bblib/utils.py` & `bblib-2.0.0/bblib/utils.py`

 * *Files identical despite different names*

### Comparing `bblib-1.2.1/pyproject.toml` & `bblib-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "1.2.1"
+version = "2.0.0"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-1.2.1/PKG-INFO` & `bblib-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 1.2.1
+Version: 2.0.0
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

