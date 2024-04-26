# Comparing `tmp/akhdefo_functions-2.5.3.tar.gz` & `tmp/akhdefo_functions-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akhdefo_functions-2.5.3.tar", last modified: Sat Apr 20 15:52:50 2024, max compression
+gzip compressed data, was "akhdefo_functions-2.5.4.tar", last modified: Fri Apr 26 05:21:24 2024, max compression
```

## Comparing `akhdefo_functions-2.5.3.tar` & `akhdefo_functions-2.5.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/
--rw-rw-rw-   0        0        0     9914 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.3/README.md
--rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.3/README_pypi.md
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.597880 akhdefo_functions-2.5.3/akhdefo_functions/
--rw-rw-rw-   0        0        0    53716 2024-04-20 15:48:45.000000 akhdefo_functions-2.5.3/akhdefo_functions/AkhdefoPlot.py
--rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Classification.py
--rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Coreg.py
--rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_GOI.py
--rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_TS.py
--rw-rw-rw-   0        0        0    76847 2024-04-06 22:26:04.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Tools.py
--rw-rw-rw-   0        0        0   156103 2024-04-18 20:56:23.000000 akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Utilities.py
--rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.3/akhdefo_functions/Filter_PreProc.py
--rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.3/akhdefo_functions/Mosaic_Crop.py
--rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.3/akhdefo_functions/OpticalFlow.py
--rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.3/akhdefo_functions/Stacked_Velocity.py
--rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.3/akhdefo_functions/Unzip_CopyFiles.py
--rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.3/akhdefo_functions/Video_Streamer.py
--rw-rw-rw-   0        0        0      717 2024-04-20 15:52:36.000000 akhdefo_functions-2.5.3/akhdefo_functions/__init__.py
--rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.3/akhdefo_functions/backend.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/
--rw-rw-rw-   0        0        0     9914 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2024-04-20 15:52:50.000000 akhdefo_functions-2.5.3/akhdefo_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 15:52:50.613386 akhdefo_functions-2.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-04-19 23:45:20.000000 akhdefo_functions-2.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:21:24.677401 akhdefo_functions-2.5.4/
+-rw-rw-rw-   0        0        0     9914 2024-04-26 05:21:24.676400 akhdefo_functions-2.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8947 2024-04-08 23:20:02.000000 akhdefo_functions-2.5.4/README.md
+-rw-rw-rw-   0        0        0     8982 2024-04-14 02:06:02.000000 akhdefo_functions-2.5.4/README_pypi.md
+drwxrwxrwx   0        0        0        0 2024-04-26 05:21:24.662404 akhdefo_functions-2.5.4/akhdefo_functions/
+-rw-rw-rw-   0        0        0    79472 2024-04-26 05:03:44.000000 akhdefo_functions-2.5.4/akhdefo_functions/AkhdefoPlot.py
+-rw-rw-rw-   0        0        0    10947 2024-04-06 22:52:15.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Classification.py
+-rw-rw-rw-   0        0        0     9269 2024-04-06 23:22:26.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Coreg.py
+-rw-rw-rw-   0        0        0   114256 2024-04-07 00:41:09.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_GOI.py
+-rw-rw-rw-   0        0        0    45641 2024-02-16 03:08:55.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_TS.py
+-rw-rw-rw-   0        0        0    82895 2024-04-24 06:53:38.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Tools.py
+-rw-rw-rw-   0        0        0   156103 2024-04-18 20:56:23.000000 akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Utilities.py
+-rw-rw-rw-   0        0        0    27027 2024-04-07 01:34:16.000000 akhdefo_functions-2.5.4/akhdefo_functions/Filter_PreProc.py
+-rw-rw-rw-   0        0        0     8035 2024-04-07 00:09:47.000000 akhdefo_functions-2.5.4/akhdefo_functions/Mosaic_Crop.py
+-rw-rw-rw-   0        0        0    45101 2024-01-03 23:08:00.000000 akhdefo_functions-2.5.4/akhdefo_functions/OpticalFlow.py
+-rw-rw-rw-   0        0        0    38672 2024-04-07 00:13:18.000000 akhdefo_functions-2.5.4/akhdefo_functions/Stacked_Velocity.py
+-rw-rw-rw-   0        0        0    11726 2024-04-06 23:46:27.000000 akhdefo_functions-2.5.4/akhdefo_functions/Unzip_CopyFiles.py
+-rw-rw-rw-   0        0        0     3321 2024-04-09 19:48:10.000000 akhdefo_functions-2.5.4/akhdefo_functions/Video_Streamer.py
+-rw-rw-rw-   0        0        0      717 2024-04-26 05:20:36.000000 akhdefo_functions-2.5.4/akhdefo_functions/__init__.py
+-rw-rw-rw-   0        0        0     3715 2024-04-20 03:34:34.000000 akhdefo_functions-2.5.4/akhdefo_functions/backend.py
+drwxrwxrwx   0        0        0        0 2024-04-26 05:21:24.675401 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/
+-rw-rw-rw-   0        0        0     9914 2024-04-26 05:21:24.000000 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-04-26 05:21:24.000000 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-26 05:21:24.000000 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-01-05 01:42:12.000000 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2024-04-26 05:21:24.000000 akhdefo_functions-2.5.4/akhdefo_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-26 05:21:24.677401 akhdefo_functions-2.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-04-26 05:20:56.000000 akhdefo_functions-2.5.4/setup.py
```

### Comparing `akhdefo_functions-2.5.3/PKG-INFO` & `akhdefo_functions-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akhdefo_functions
-Version: 2.5.3
+Version: 2.5.4
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.3/README.md` & `akhdefo_functions-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/README_pypi.md` & `akhdefo_functions-2.5.4/README_pypi.md`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/AkhdefoPlot.py` & `akhdefo_functions-2.5.4/akhdefo_functions/AkhdefoPlot.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,14 +58,370 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 import re
 from datetime import datetime
 
+def create_kmz_with_overlay(image_path, raster_path, output_path, bbox=None):
+    """
+    Create a KMZ file with an image overlay based on the geographic bounds of a GeoTIFF file.
+
+    This function reads a GeoTIFF raster file to determine its geographic bounds and coordinate reference system (CRS).
+    It then uses these bounds to overlay an image on a KML file, which is subsequently saved as a KMZ file.
+    If the CRS of the raster is not EPSG:4326 (latitude and longitude), the function will transform the coordinates
+    to EPSG:4326 using pyproj.
+
+    Parameters
+    ----------
+    image_path : str
+        Path to the image file that will be overlaid on the KML. This image should ideally be a PNG or JPEG file.
+    raster_path : str
+        Path to the GeoTIFF raster file from which geographic bounds are derived.
+    output_path : str
+        Path where the output KMZ file will be saved.
+    bbox: list
+        [N,E,S,W]
+    Returns
+    -------
+    None
+        The function does not return any value but saves the KMZ file at the specified output location.
+
+    Example
+    -------
+    >>> create_kmz_with_overlay('./Figure_Analysis/East_universal.png', 
+                                './las_cropped_aoi/Sep_13th2017_lidar_crop.tif', 
+                                'output_overlay.kmz')
+    """
+    
+    import rasterio
+    from rasterio.crs import CRS
+    from pyproj import Transformer, CRS as PyProjCRS
+    import simplekml
+    # Open the GeoTIFF file to read its bounds and CRS
+    
+    with rasterio.open(raster_path) as dataset:
+        bounds = dataset.bounds
+        src_crs = dataset.crs  # Source CRS
+
+        # Manually create a CRS object for EPSG:4326 if from_epsg fails
+        epsg_4326_crs = PyProjCRS.from_proj4("+proj=longlat +datum=WGS84 +no_defs")
+
+        # Check if the source CRS is not EPSG:4326
+        if src_crs != epsg_4326_crs:
+            # Create a transformer to convert from source CRS to EPSG:4326
+            transformer = Transformer.from_crs(src_crs, epsg_4326_crs, always_xy=True)
+            
+            # Transform each corner of the bounding box
+            west, south = transformer.transform(bounds.left, bounds.bottom)
+            east, north = transformer.transform(bounds.right, bounds.top)
+        else:
+            # Use the bounds directly if they are already in EPSG:4326
+            north = bounds.top
+            south = bounds.bottom
+            east = bounds.right
+            west = bounds.left
+    
+    # import rasterio
+    # import re
+
+    
+   
+    
+    if bbox is not None:
+        # Calculate coordinates for each corner
+        north, east= bbox[0], bbox[1]    
+        south, west =  bbox[2], bbox[3]
+        # # Check if the source CRS is not EPSG:4326
+        # if src_crs != epsg_4326_crs:
+        #    east, north=convert_utm_to_latlon(east, north, crs_info['UTM Zone'], crs_info['Hemisphere'] )
+        #    west, south=convert_utm_to_latlon(west, south, crs_info['UTM Zone'], crs_info['Hemisphere'] )
+        
+    # Create a KML object
+    kml = simplekml.Kml()
+     
+
+
+    # Create a ground overlay
+    ground = kml.newgroundoverlay(name='Sample Overlay')
+    ground.icon.href = image_path
+    ground.latlonbox.north = north
+    ground.latlonbox.south = south
+    ground.latlonbox.east = east
+    ground.latlonbox.west = west
+    
+   
+    # Save to KMZ
+    kml.savekmz(output_path)
+
+
+def get_crs_info(raster_path):
+        # Open the raster file
+        with rasterio.open(raster_path) as dataset:
+            # Get CRS
+            crs = dataset.crs
+            
+            if not crs:
+                return "CRS not found."
+
+            # Initialize info dictionary
+            crs_info = {'EPSG': None, 'UTM Zone': None, 'Hemisphere': None}
+            
+            # Extract EPSG code
+            if crs.is_epsg_code:
+                crs_info['EPSG'] = crs.to_epsg()
+            
+            # Convert CRS to WKT for easier parsing
+            crs_wkt = crs.to_wkt()
+            
+            # Find UTM zone and hemisphere from WKT
+            utm_match = re.search(r'UTM zone (\d+)(N|S)', crs_wkt)
+            if utm_match:
+                crs_info['UTM Zone'] = int(utm_match.group(1))
+                crs_info['Hemisphere'] = 'north' if utm_match.group(2) == 'N' else 'south'
+
+            return crs_info
+from pyproj import Proj, transform
+
+def convert_utm_to_latlon(easting, northing, zone, hemisphere):
+    # Define the UTM projection string
+    utm_proj = Proj(proj='utm', zone=zone, ellps='WGS84', south=hemisphere==hemisphere)
+    
+    # Define the latitude/longitude projection string
+    latlon_proj = Proj(proj='latlong', ellps='WGS84')
+    
+    # Convert UTM to latitude and longitude
+    longitude, latitude = transform(utm_proj, latlon_proj, easting, northing)
+    return latitude, longitude
+
+
+import rasterio
+from rasterio.warp import transform_bounds
+from shapely.geometry import box
+from rasterio.errors import CRSError
+from pyproj import Transformer, CRS as PyProjCRS
+from rasterio.transform import from_origin
+import akhdefo_functions
+import shutil
+import tempfile
+import os
+
+def save_images_to_temp_folder(image_path1, image_path2):
+    # Create a temporary directory
+    temp_dir = tempfile.mkdtemp()
+    
+    # Define the destination paths within the temporary directory
+    dest_path1 = os.path.join(temp_dir, os.path.basename(image_path1))
+    dest_path2 = os.path.join(temp_dir, os.path.basename(image_path2))
+    
+    # Copy images to the temporary directory
+    shutil.copy(image_path1, dest_path1)
+    shutil.copy(image_path2, dest_path2)
+    
+    akhdefo_functions.crop_to_overlap(temp_dir)
+    
+    # Print the paths of the saved images
+    #print("Image 1 saved at:", dest_path1)
+    #print("Image 2 saved at:", dest_path2)
+    
+    return dest_path1, dest_path2, temp_dir
+
+def delete_temp_folder(temp_folder_path):
+    # Check if the folder exists
+    if os.path.exists(temp_folder_path):
+        # Remove the directory and all its contents
+        shutil.rmtree(temp_folder_path)
+
+def crop_rasters_and_return_info(path1, path2):
+    
+    path1, path2, temp_dir=save_images_to_temp_folder(path1, path2)
+    
+    
+    
+    #try:
+    with rasterio.open(path1) as src1, rasterio.open(path2) as src2:
+        # Use EPSG code directly for both sources if they are the same and well-defined.
+        epsg_code = 'EPSG:32610'  # Standard EPSG code for WGS 84 / UTM zone 10N
+        src_crs=src2.crs
+        bbox1 = box(*src1.bounds)
+        bbox2 = box(*src2.bounds)
+
+        intersection = bbox1.intersection(bbox2)
+        if intersection.is_empty:
+            return "No overlapping area found."
+
+        window1 = rasterio.windows.from_bounds(*intersection.bounds, src1.transform)
+        window2 = rasterio.windows.from_bounds(*intersection.bounds, src2.transform)
+
+        data1 = src1.read(1, window=window1, masked=True)
+        data2 = src2.read(1, window=window2, masked=True)
+       
+        
+            # Mask no data values
+        if src1.nodata is not None:
+            data1 = np.where(data1 == src1.nodata, np.nan, data1)
+        else:
+            data1 = data1  # Use original data if no no_data_value defined
+            
+              # Mask no data values
+        if src2.nodata is not None:
+            data2 = np.where(data2 == src2.nodata, np.nan, data2)
+        else:
+            data2 = data2  # Use original data if no no_data_value defined
+        
+        
+        
+        crs_info = get_crs_info(path2)
+        utm_zone=crs_info['UTM Zone']
+        hemisphere=crs_info['Hemisphere']
+        
+        # Convert intersection bounds to geographic coordinates
+        west, south = src1.xy(intersection.bounds[1], intersection.bounds[0])
+        east, north = src1.xy(intersection.bounds[3], intersection.bounds[2])
+
+        # Calculate the width and height of the bounding box
+        width = intersection.bounds[2] - intersection.bounds[0]
+        height = intersection.bounds[3] - intersection.bounds[1]
+        
+        #Transform of the subset intersection
+        subset_transform=src1.window_transform(window1)
+        # Extracting values from the transform
+        west = subset_transform.c
+        north = subset_transform.f
+        pixel_size_x = subset_transform.a
+        pixel_size_y = -subset_transform.e 
+        
+        # Calculating the east and south boundaries
+        east = west + (width * pixel_size_x)
+        south = north - (height * pixel_size_y)
+
+        #print(north, south, east, west)
+        
+        # east, north=convert_utm_to_latlon(east, north, crs_info['UTM Zone'], crs_info['Hemisphere'] )
+        # west, south=convert_utm_to_latlon(west, south, crs_info['UTM Zone'], crs_info['Hemisphere'] )
+        
+            # Manually create a CRS object for EPSG:4326 if from_epsg fails
+        epsg_4326_crs = PyProjCRS.from_proj4("+proj=longlat +datum=WGS84 +no_defs")
+
+        # Check if the source CRS is not EPSG:4326
+        if src_crs != epsg_4326_crs:
+            # # Create a transformer to convert from source CRS to EPSG:4326
+            # transformer = Transformer.from_crs(src_crs, epsg_4326_crs, always_xy=True)
+            
+            # # Transform each corner of the bounding box
+            # west, south = transformer.transform(intersection.bounds[2], intersection.bounds[0])
+            # east, north = transformer.transform(intersection.bounds[3], intersection.bounds[2])
+            # Assume transformation is needed to WGS84
+            target_crs = PyProjCRS.from_epsg(4326)
+            # transformer = Transformer.from_crs(src1.crs, target_crs, always_xy=True)
+            # # Perform the transformation
+            # west, south = transformer.transform(west, south)
+            # east, north = transformer.transform(east, north)
+            west, south, east, north = transform_bounds(src1.crs, target_crs, *intersection.bounds)
+            ####################
+            import math
+            # Constants
+            meters_per_degree_latitude = 111320  # meters per degree of latitude
+            latitude = north
+            # Conversion formulas
+            pixel_size_y_in_degrees = pixel_size_y / meters_per_degree_latitude
+            pixel_size_x_in_degrees = pixel_size_x / (meters_per_degree_latitude * math.cos(math.radians(latitude)))
+            pixel_size_x_in_degrees, pixel_size_y_in_degrees
+            subset_transform_updated=from_origin(west, north, pixel_size_x_in_degrees, pixel_size_y_in_degrees)
+        else:
+            west, south , east, north 
+            subset_transform_updated=subset_transform
+        
+        #print(north, south, east, west)
+        from rasterio.coords import BoundingBox
+        
+        
+        
+        import math
+        # Constants
+        meters_per_degree_latitude = 111320  # meters per degree of latitude
+        latitude = north
+        # Conversion formulas
+        pixel_size_y_in_degrees = pixel_size_y / meters_per_degree_latitude
+        pixel_size_x_in_degrees = pixel_size_x / (meters_per_degree_latitude * math.cos(math.radians(latitude)))
+        pixel_size_x_in_degrees, pixel_size_y_in_degrees
+        subset_transform_updated=from_origin(west, north, pixel_size_x_in_degrees, pixel_size_y_in_degrees)
+        
+        
+        
+        
+        # Define the custom bounds
+        bounds = BoundingBox(left=west, bottom=south, right=east, top=north)
+        print('bounds: ', bounds)
+
+        from scipy.ndimage import zoom
+        data2 = np.where(data2 == -32767, np.nan, data2)
+        data1 = np.where(data1 == -32767, np.nan, data1)
+        # Calculate the zoom factor
+        zoom_factor = len(data1) / len(data2)
+         # Get the no-data value from the dataset's metadata
+        
+        # Use the zoom function to resize array1
+        data2 = zoom(data2, zoom_factor, order=1)
+        data2 = np.where(data2 == src2.nodata, np.nan, data2)
+        
+        
+        
+        
+        
+            # Prepare the return information including pixel dimensions and bounding box size
+        info1 = {
+            'array': data1,
+            'transform': src1.window_transform(window1),
+            'crs': src1.crs,
+            'resolution': (src1.res[0], src1.res[0]),
+            'bbox_size': {'width': width, 'height': height},
+            'bounds_latlong': {'north': north, 'south': south, 'east': east, 'west': west} , 'utm_zone':utm_zone,
+            'trasnform_latlon':subset_transform_updated, 'resolution_latlon':(pixel_size_x_in_degrees, pixel_size_y_in_degrees)
+        }
+        info2 = {
+            'array': data2,
+            'transform': src2.window_transform(window2),
+            'crs':src2.crs,
+            'resolution': (src1.res[0], src1.res[1]),
+            'bbox_size': {'width': width, 'height': height},
+            'bounds_latlong': {'north': north, 'south': south, 'east': east, 'west': west}, 'utm_zone':utm_zone, 
+            'trasnform_latlon':subset_transform_updated, 'resolution_latlon':(pixel_size_x_in_degrees, pixel_size_y_in_degrees)
+        }
+        
+    
+        
+    src1.close()
+    src2.close()
+    delete_temp_folder(temp_dir)
+    return info1, info2
+        
+        
+        
+    # except CRSError as e:
+    #     raise RuntimeError(f"CRS transformation error: {e}")
+    # except Exception as e:
+    #     raise RuntimeError(f"An unexpected error occurred: {e}")
+    
+    
+
+# Usage
+# info1, info2 = crop_rasters_and_return_info(path_to_raster1, path_to_raster2)
+
+
+
+
+
+
+
+
+
+
+
+
 
 
 def akhdefo_viewer(path_to_dem_file, raster_file, output_folder, title='', 
                    pixel_resolution_meters=3.125, output_file_name="", 
                    alpha=0.5, unit_conversion=None, no_data_mask=False, 
                    colormap='jet', min_value=None, max_value=None, 
                    normalize=False, colorbar_label=None, show_figure=True , aspect_raster=None, cmap_aspect=None, step=10):
@@ -93,61 +449,121 @@
     step (int, optional): density of the aspect vector arraows. Defulat is 10 pixel unit draw 1 arrow
 
     Returns:
     None
     """
     try:
         
-        with rasterio.open(path_to_dem_file) as src:
-            # Number of bands
-            band_count = src.count
-            xres, yres=src.res
-            if band_count >2:
-                dem = src.read(masked=True)
-                dem_transform = src.transform
-                hillshade=dem
+        # with rasterio.open(path_to_dem_file) as src_dem:
+        #     # Number of bands
+        #     band_count = src_dem.count
+        #     xres, yres=src_dem.res
+        #     if band_count >2:
+        #         dem = src_dem.read(masked=True)
+        #         dem_transform = src_dem.transform
+        #         hillshade=dem
                 
-            else:
-                dem = src.read(1, masked=True)
-                dem_transform = src.transform
+        #     else:
+        #         dem = src_dem.read(1, masked=True)
+        #         dem_transform = src_dem.transform
             
-                hillshade = es.hillshade(dem)
+        #         hillshade = es.hillshade(dem)
                 
 
-        with rasterio.open(raster_file) as src:
-            raster = src.read(1, masked=True)
-            raster_transform = src.transform
-            raster_crs = src.crs
+        # with rasterio.open(raster_file) as src_raster:
+        #     raster = src_raster.read(1, masked=True)
+        #     raster_transform = src_raster.transform
+        #     raster_crs = src_raster.crs
     
 
+        dem_data, raster_data=crop_rasters_and_return_info(path_to_dem_file, raster_file)
+        
+        if aspect_raster is not None:
+            
+            _, aspect_data=crop_rasters_and_return_info(path_to_dem_file, aspect_raster)
+            aspect_arr=aspect_data['array']
+            aspect_transform=aspect_data['trasnform_latlon'] 
+        else:
+            aspect_arr=None
+            aspect_transform=None
+            
+        dem_arr=dem_data['array']
+        dem_transform=dem_data['transform'] 
+        dem_res=dem_data['resolution']
+        dem_crs=dem_data['crs']
+        utm_zone=dem_data['utm_zone']
+        raster=raster_data['array']
+        raster_transform=raster_data['transform']
+        raster_res=raster_data['resolution']
+        raster_crs=raster_data['crs']
+        xres=dem_res[0]
+        hillshade = es.hillshade(dem_arr)
+        
+        with rasterio.open(path_to_dem_file) as src_dem:
+            # Number of bands
+            band_count = src_dem.count
+            if band_count >2:
+                hillshade=dem_arr
+        
+        # Assuming you've already executed the function and have the results stored in cropped_info1 and cropped_info2
+        width = dem_data['bbox_size']['width']
+        height = dem_data['bbox_size']['height']
+        
+        west=dem_data['bounds_latlong']['west']
+        south=dem_data['bounds_latlong']['south']
+        east=dem_data['bounds_latlong']['east']
+        north=dem_data['bounds_latlong']['north']
+        
         if no_data_mask:
             raster = np.ma.masked_where(raster == 0, raster)
 
         if unit_conversion:
             unit_type, unit_factor = _separate_floats_letters(unit_conversion)
             raster *= float(unit_factor)
 
         if pixel_resolution_meters is None:
             pixel_resolution_meters=xres
 
         # Set the output file name if it's not provided
         if not output_file_name:
             output_file_name = os.path.splitext(os.path.basename(raster_file))[0] + ".png"
 
-        _create_plot(hillshade, raster, dem_transform, raster_transform, raster_crs, alpha, colormap, normalize,
-                     title, output_folder, output_file_name, colorbar_label, pixel_resolution_meters, min_value, max_value, aspect_raster, cmap_aspect, step)
+        _create_plot(hillshade=hillshade, raster=raster, dem_transform=dem_transform, raster_transform=raster_transform, raster_crs=raster_crs, alpha=alpha, colormap=colormap, normalize=normalize,
+                     title=title, output_folder=output_folder, output_file_name=output_file_name, colorbar_label=colorbar_label, pixel_resolution_meters=pixel_resolution_meters,
+                     min_value=min_value, max_value=max_value, aspect_raster=aspect_arr, cmap_aspect=cmap_aspect, step=step, UTM_zone=utm_zone)
+        
+        
+        create_kmz_overlay(hillshade=hillshade, raster=raster, colormap=colormap, alpha=alpha, west=west,south=south,east=east,north=north,output_folder= output_folder, 
+                           output_file_name=output_file_name+'.kmz', colorbar_label=colorbar_label, normalize=normalize, min_value=min_value, max_value=max_value, title=title, 
+                           aspect_raster=aspect_arr, step=step, cmap_aspect=cmap_aspect, transform=aspect_transform)
+
+        
+       
+       
+    
+        
+        
 
         if show_figure:
             plt.show()
         else:
             plt.close()
+            
+            
+        # create_kmz_with_overlay(image_path=os.path.join(output_folder, output_file_name),raster_path=raster_file, output_path=os.path.join(output_folder, output_file_name[:-4]+'.kmz'),
+        #                         bbox= None )
 
     except Exception as e:
         raise RuntimeError(f"An error occurred: {e}")
 
+
+
+
+
+
 def _separate_floats_letters(input_string):
     """
     Separates floats and letters from a string.
     """
     floats = re.findall(r'\d+\.\d+|\d+', input_string)
     letters = re.findall(r'[a-zA-Z]+', input_string)
     if not floats or not letters:
@@ -173,96 +589,103 @@
     
     
     
     return raster, norm
 
 
 def _create_plot(hillshade, raster, dem_transform, raster_transform, raster_crs, alpha, colormap, normalize,
-                 title, output_folder, output_file_name, colorbar_label, pixel_resolution_meters, min_value, max_value , aspect_raster=None, cmap_aspect=None, step=10):
+                 title, output_folder, output_file_name, colorbar_label, pixel_resolution_meters, min_value, max_value , aspect_raster=None, cmap_aspect=None, step=10 , UTM_zone=None):
     """
     Creates and saves a plot of hillshade and raster overlay.
     """
     
     basemap_dimensions = hillshade.ndim
-    fig, ax = plt.subplots(figsize=(10, 10))
-
+  
+        
+    fig, ax = plt.subplots(figsize=(15, 10))
+    
     # Plot the hillshade layer using dem_transform for its extent
     if basemap_dimensions > 2:
         #ep.plot_rgb(hillshade, rgb=(0, 1, 2), str_clip=2, ax=ax, extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform))
         rasterio.plot.show(hillshade, transform=dem_transform, ax=ax)
     else:
-        rasterio.plot.show(hillshade,extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform), ax=ax , cmap='gray')
+        
+           
+        #rasterio.plot.show(hillshade,extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform), ax=ax , cmap='gray')
+        ax.imshow(hillshade,extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform), cmap='gray')
         # ep.plot_bands(
         #     hillshade,
         #     ax=ax,
         #     cmap='gray',
-        #     scale=False,
+        #     scale=True,
         #     cbar=False,
-        #     extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform)  # ensure correct transform
-        # )
+        #     extent=rasterio.plot.plotting_extent(raster, transform=raster_transform))  # ensure correct transform
+        # # )
 
     if aspect_raster is not None:
         alpha_basemap=0.45
     else:
         alpha_basemap=alpha
     
     if normalize:
         raster, norm = _normalize_raster(raster, min_value, max_value)
         
     if normalize==True:
     # Overlay the raster with alpha for transparency using raster_transform for its extent
-        img = ax.imshow(raster, alpha=alpha_basemap, cmap=colormap, norm=norm,
-                    extent=rasterio.plot.plotting_extent(raster, transform=raster_transform))  # ensure correct transform
-    
+      
+        
+        img = ax.imshow(raster, alpha=alpha_basemap, cmap=colormap, norm=norm, 
+                    extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform))  # ensure correct transform
     if normalize==False:
         
         if min_value is None and max_value is None:
             min_value = np.nanmin(raster)
             max_value = np.nanmax(raster)
         else:
             min_value=min_value
             max_value=max_value
-        
-        # Overlay the raster with alpha for transparency using raster_transform for its extent
-        img = ax.imshow(raster, alpha=alpha_basemap, cmap=colormap, vmin=min_value , vmax=max_value,
-                    extent=rasterio.plot.plotting_extent(raster, transform=raster_transform))  # ensure correct transform
-        
+       
+      
+                 # Overlay the raster with alpha for transparency using raster_transform for its extent
+        img = ax.imshow(raster, alpha=alpha_basemap, cmap=colormap, vmin=min_value , vmax=max_value, 
+                        extent=rasterio.plot.plotting_extent(hillshade, transform=dem_transform))  # ensure correct transform
     if aspect_raster is not None:
         def aspect_to_uv(aspect):
             """
             Convert aspect data to U and V components for arrows.
             """
             aspect_rad = np.deg2rad(aspect)
             u = np.sin(aspect_rad)
             v = np.cos(aspect_rad)
             return u, v
-        # Load the raster file
-        with rasterio.open(aspect_raster) as dataset:
-            # Read the aspect data
-            aspect_data = dataset.read(1)
+        # # Load the raster file
+        # with rasterio.open(aspect_raster) as dataset:
+        #     # Read the aspect data
+        #     aspect_data = dataset.read(1)
             
-            # Get the geotransformation data
-            transform = dataset.transform
-
-            # Get the shape of the data
-            data_shape = aspect_data.shape
+        #     # Get the geotransformation data
+        #     transform = dataset.transform
 
+        #     # Get the shape of the data
+        #     data_shape = aspect_data.shape
+        aspect_data=aspect_raster
+        data_shape=aspect_data.shape
         # Generate a grid of points every 10 pixels
         step=step
         x_positions = np.arange(0, data_shape[1], step)
         y_positions = np.arange(0, data_shape[0], step)
         x_grid, y_grid = np.meshgrid(x_positions, y_positions)
 
         # Subset the aspect data to match the grid
         aspect_subset = aspect_data[y_positions[:, None], x_positions]
         aspect_subset, norm = _normalize_raster(aspect_subset, min_value=None, max_value=None)
         u_subset, v_subset = aspect_to_uv(aspect_subset)
 
         # Convert grid positions to real world coordinates
-        x_grid_world, y_grid_world = transform * (x_grid, y_grid)
+        x_grid_world, y_grid_world = dem_transform * (x_grid, y_grid)
         if cmap_aspect is None:
             cmap_aspect='hsv'
         quiver = ax.quiver(x_grid_world, y_grid_world, u_subset, v_subset, aspect_subset, scale=20, cmap=cmap_aspect , angles='xy', norm=norm, alpha=alpha)
         # Adding a second colorbar in a horizontal position
         cbar_ax2 = fig.add_axes([0.25, 0.04, 0.5, 0.02])  # Position for the horizontal colorbar
         cbar2 = fig.colorbar(quiver, cax=cbar_ax2, orientation='horizontal',  extend='both')  # Using the ScalarMappable created earlier
         cbar2.set_label('Aspect-Colorbar(degrees)')
@@ -282,25 +705,240 @@
         ax.set_ylabel('Northing')
 
     #ax.grid(True, which='major')
     ax.set_title(title)
 
    
         
-    scalebar = ScaleBar(dx=pixel_resolution_meters, location='lower right', units='m',
+    scalebar = ScaleBar(1, location='lower right', units='m',
                         frameon=True, scale_loc='bottom', dimension='si-length', box_color='white', color='k', border_pad=1, box_alpha=0.65)  # Adjust parameters as needed
    
     ax.add_artist(scalebar)
-      
+    
+
     # Save the plot
     plt.savefig(os.path.join(output_folder, output_file_name), dpi=100, bbox_inches='tight')
 
 
 
 
+
+from simplekml import Kml, OverlayXY, ScreenXY, Units, RotationXY, AltitudeMode, Camera
+
+def gearth_fig(west, south, east, north, pixels=1024):
+    aspect = np.cos(np.mean([south, north]) * np.pi/180.0)
+    xsize = np.ptp([east, west]) * aspect
+    ysize = np.ptp([north, south])
+    aspect = ysize / xsize
+
+    if aspect > 1.0:
+        figsize = (10.0 / aspect, 10.0)
+    else:
+        figsize = (10.0, 10.0 * aspect)
+
+    fig = plt.figure(figsize=figsize, frameon=False, dpi=pixels // 10)
+    ax = fig.add_axes([0, 0, 1, 1])
+    ax.set_xlim(west, east)
+    ax.set_ylim(south, north)
+    return fig, ax
+
+def make_kml(west, south, east, north,
+             figs, colorbar=None, **kw):
+    """TODO: LatLon bbox, list of figs, optional colorbar figure,
+    and several simplekml kw..."""
+
+    kml = Kml()
+    altitude = kw.pop('altitude', 2e7)
+    roll = kw.pop('roll', 0)
+    tilt = kw.pop('tilt', 0)
+    altitudemode = kw.pop('altitudemode', AltitudeMode.relativetoground)
+    camera = Camera(latitude=np.mean([north, south]),
+                    longitude=np.mean([east, west]),
+                    altitude=altitude, roll=roll, tilt=tilt,
+                    altitudemode=altitudemode)
+
+    #kml.document.camera = camera
+    draworder = 0
+    for fig in figs:  # NOTE: Overlays are limited to the same bbox.
+        draworder += 1
+        ground = kml.newgroundoverlay(name='GroundOverlay')
+        ground.draworder = draworder
+        # ground.visibility = kw.pop('visibility', 1)
+        # #ground.name = kw.pop('name', 'overlay')
+        ground.color = kw.pop('color', '9effffff')
+        ground.atomauthor = kw.pop('author', 'ocefpaf')
+        ground.latlonbox.rotation = kw.pop('rotation', 0)
+        ground.description = kw.pop('description', 'Matplotlib figure')
+        ground.gxaltitudemode = kw.pop('gxaltitudemode',
+                                       'clampToSeaFloor')
+        ground.icon.href = fig
+        ground.latlonbox.east = east
+        ground.latlonbox.south = south
+        ground.latlonbox.north = north
+        ground.latlonbox.west = west
+
+    if colorbar:  # Options for colorbar are hard-coded (to avoid a big mess).
+        screen = kml.newscreenoverlay(name='Legend')
+        screen.icon.href = colorbar
+        screen.overlayxy = OverlayXY(x=0, y=0,
+                                     xunits=Units.fraction,
+                                     yunits=Units.fraction)
+        screen.screenxy = ScreenXY(x=0.015, y=0.075,
+                                   xunits=Units.fraction,
+                                   yunits=Units.fraction)
+        screen.rotationXY = RotationXY(x=0.5, y=0.5,
+                                       xunits=Units.fraction,
+                                       yunits=Units.fraction)
+        screen.size.x = 0
+        screen.size.y = 0
+        screen.size.xunits = Units.fraction
+        screen.size.yunits = Units.fraction
+        screen.visibility = 1
+
+    kmzfile = kw.pop('kmzfile', 'overlay.kmz')
+    
+    
+    kml.savekmz(kmzfile)
+  
+
+def create_kmz_overlay(hillshade, raster, colormap, alpha, west, south, east, north, output_folder, output_file_name, pixels=2030, colorbar_label='colorbar_label',
+                       normalize=True, min_value= None, max_value=None, title='title', aspect_raster=None, step=10, cmap_aspect='hsv', transform=None):
+    
+    fig_ov, ax = gearth_fig(west, south, east, north, pixels)
+    ax.imshow(hillshade, alpha=0.85,cmap='gray', extent=[west, east, south, north])
+    
+   
+    if normalize:
+        raster, norm = _normalize_raster(raster, min_value, max_value)
+    img = ax.imshow(raster, cmap=colormap, alpha=0.75, extent=[west, east, south, north], norm=norm)
+    ax.set_axis_off()
+    fig_path = os.path.join(output_folder, 'overlay' + '.jpg')
+    
+    
+    ########ADD qquiver plot############
+    if aspect_raster is not None:
+        def aspect_to_uv(aspect):
+            """
+            Convert aspect data to U and V components for arrows.
+            """
+            aspect_rad = np.deg2rad(aspect)
+            u = np.sin(aspect_rad)
+            v = np.cos(aspect_rad)
+            return u, v
+        aspect_data=aspect_raster
+        data_shape=aspect_data.shape
+        # Generate a grid of points every 10 pixels
+        step=step
+        x_positions = np.arange(0, data_shape[1], step)
+        y_positions = np.arange(0, data_shape[0], step)
+        x_grid, y_grid = np.meshgrid(x_positions, y_positions)
+
+        # Subset the aspect data to match the grid
+        aspect_subset = aspect_data[y_positions[:, None], x_positions]
+        aspect_subset, norm = _normalize_raster(aspect_subset, min_value=None, max_value=None)
+        u_subset, v_subset = aspect_to_uv(aspect_subset)
+
+        # Convert grid positions to real world coordinates
+        x_grid_world, y_grid_world = transform * (x_grid, y_grid)
+        
+        if cmap_aspect is None:
+            cmap_aspect='hsv'
+    if aspect_raster is not None:
+        quiver = ax.quiver(x_grid_world, y_grid_world, u_subset, v_subset, aspect_subset, scale=20, cmap=cmap_aspect , angles='xy', norm=norm, alpha=1)
+        
+    
+    fig_ov.savefig(fig_path, dpi=fig_ov.dpi, transparent=False, bbox_inches='tight')
+    plt.close(fig_ov)
+        ##############################
+
+    if aspect_raster is not None:
+        figsize=(4.0, 2.0)
+        colorbar_path=os.path.join(output_folder, 'legend' + '.jpg')
+    else:
+        figsize=(4.0, 1.0)
+        colorbar_path=os.path.join(output_folder, 'legend' + '.jpg')
+        
+        
+        
+    if aspect_raster is not None:
+        
+        fig_cb = plt.figure(figsize=figsize, facecolor='white', frameon=True)
+
+        # First Colorbar
+        ax_cb1 = fig_cb.add_axes([0.05, 0.8, 0.9, 0.1])  # Adjusted the position of the axes for the first colorbar
+        cb1 = plt.colorbar(img, cax=ax_cb1, orientation='horizontal', extend='both')  # First colorbar
+        cb1.set_label(colorbar_label, color='k', labelpad=1)  # Adjusted labelpad
+        
+        # Second Colorbar
+        ax_cb2 = fig_cb.add_axes([0.05, 0.3, 0.9, 0.1])  # Adjusted the position of the axes for the second colorbar
+        cb2 = plt.colorbar(quiver, cax=ax_cb2, orientation='horizontal', extend='both')  # Second colorbar
+        cb2.set_label('Aspect-Colorbar(degrees)', color='k', labelpad=1)  # Adjusted labelpad
+        #plt.tight_layout()  # Ensures all elements are included with tight layout
+        fig_cb.savefig(colorbar_path, transparent=False)
+        plt.close(fig_cb)
+        make_kml(west, south, east, north, [fig_path], kmzfile=os.path.join(output_folder, output_file_name[:-4] + '.kmz'), colorbar=colorbar_path, name=title)
+    
+    else:
+        fig_cb = plt.figure(figsize=figsize, facecolor='white', frameon=True)
+        # First Colorbar
+        ax_cb1 = fig_cb.add_axes([0.05, 0.6, 0.9, 0.2])  # Adjusted the position of the axes for the first colorbar
+        cb1 = plt.colorbar(img, cax=ax_cb1, orientation='horizontal', extend='both')  # First colorbar
+        cb1.set_label(colorbar_label, color='k', labelpad=1)  # Adjusted labelpad
+        #plt.tight_layout()  # Ensures all elements are included with tight layout
+        fig_cb.savefig(colorbar_path, transparent=False) 
+        plt.close(fig_cb)
+        
+        make_kml(west, south, east, north, [fig_path], kmzfile=os.path.join(output_folder, output_file_name[:-4] + '.kmz'), colorbar=colorbar_path, name=title)
+        
+    #Delete temp files  
+    os.remove(fig_path)
+    os.remove(colorbar_path)
+        
+        
+        
+
+    
+       
+    
+    
+    
+    
+    
+    
+    # fig_cb = plt.figure(figsize=(4.0, 1.0), facecolor='white', frameon=True)
+    # ax_cb = fig_cb.add_axes([0.05, 0.6, 0.9, 0.2])  # Adjusted the position of the axes
+    # cb = plt.colorbar(img, cax=ax_cb, orientation='horizontal', extend='both')  # Changed orientation and extended both ends
+    # cb.set_label(colorbar_label, color='k', labelpad=10)  # Adjusted labelpad
+    
+    # ###second colorbar##
+    # if aspect_raster is not None:
+    #     # Adding a second colorbar in a horizontal position
+    #     cbar_ax2 = fig_cb.add_axes([0.25, 0.2, 0.5, 0.02])  # Position for the horizontal colorbar
+    #     cbar2 = fig_cb.colorbar(quiver, cax=cbar_ax2, orientation='horizontal',  extend='both')  # Using the ScalarMappable created earlier
+    #     cbar2.set_label('Aspect-Colorbar(degrees)')
+        
+    # plt.tight_layout()
+    # fig_cb.savefig(colorbar_path, transparent=False)
+    # plt.close(fig_cb)
+   
+    # fig_cb = plt.figure(figsize=(1.0, 4.0), facecolor='white', frameon=True)
+    # ax_cb = fig_cb.add_axes([0.0, 0.05, 0.2, 0.9])
+    # cb = plt.colorbar(img, cax=ax_cb)
+    # cb.set_label(colorbar_label, rotation=90, color='k', labelpad=20)
+    
+    # fig_cb.savefig(colorbar_path, transparent=False)
+    # plt.close(fig_cb)
+
+   
+
+    
+    
+   
+
+
 def plot_stackNetwork(src_folder="", output_folder="", cmap='tab20', date_plot_interval=(5, 30), marker_size=15):
     
     """
     Generates a scatter plot to visualize the time intervals between dates extracted from the filenames of .tif files.
     The function handles filenames containing single or multiple dates. For multiple dates, it calculates the interval 
     between the first and last date. For single dates, it calculates the interval between consecutive dates.
```

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Classification.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Classification.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Coreg.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Coreg.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_GOI.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_GOI.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_TS.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_TS.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Tools.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -2184,2620 +2184,2998 @@
 00008870: 2020 2020 2020 7265 7475 726e 2028 7261        return (ra
 00008880: 6e64 6f6d 2e75 6e69 666f 726d 2830 2c20  ndom.uniform(0, 
 00008890: 3129 2c20 7261 6e64 6f6d 2e75 6e69 666f  1), random.unifo
 000088a0: 726d 2830 2c20 3129 2c20 7261 6e64 6f6d  rm(0, 1), random
 000088b0: 2e75 6e69 666f 726d 2830 2c20 3129 290d  .uniform(0, 1)).
 000088c0: 0a0d 0a20 2020 2064 6566 2072 6561 645f  ...    def read_
 000088d0: 6465 6d28 6465 6d5f 6669 6c65 293a 0d0a  dem(dem_file):..
-000088e0: 2020 2020 2020 2020 6473 203d 2067 6461          ds = gda
-000088f0: 6c2e 4f70 656e 2864 656d 5f66 696c 6529  l.Open(dem_file)
-00008900: 0d0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
-00008910: 2064 732e 5265 6164 4173 4172 7261 7928   ds.ReadAsArray(
-00008920: 290d 0a20 2020 2020 2020 2074 7261 6e73  )..        trans
-00008930: 666f 726d 203d 2064 732e 4765 7447 656f  form = ds.GetGeo
-00008940: 5472 616e 7366 6f72 6d28 290d 0a20 2020  Transform()..   
-00008950: 2020 2020 2070 726f 6a65 6374 696f 6e20       projection 
-00008960: 3d20 6473 2e47 6574 5072 6f6a 6563 7469  = ds.GetProjecti
-00008970: 6f6e 2829 0d0a 2020 2020 2020 2020 6473  on()..        ds
-00008980: 203d 204e 6f6e 6520 2023 2043 6c6f 7365   = None  # Close
-00008990: 2074 6865 2064 6174 6173 6574 0d0a 2020   the dataset..  
-000089a0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
-000089b0: 612c 2074 7261 6e73 666f 726d 2c20 7072  a, transform, pr
-000089c0: 6f6a 6563 7469 6f6e 0d0a 2020 2020 0d0a  ojection..    ..
-000089d0: 2020 2020 6461 7461 2c20 7472 616e 7366      data, transf
-000089e0: 6f72 6d2c 2070 726f 6a65 6374 696f 6e20  orm, projection 
-000089f0: 3d20 7265 6164 5f64 656d 2864 656d 5f64  = read_dem(dem_d
-00008a00: 6174 6129 0d0a 2020 2020 0d0a 2020 2020  ata)..    ..    
-00008a10: 696d 706f 7274 206d 6174 680d 0a0d 0a20  import math.... 
-00008a20: 2020 2064 6566 2063 616c 6375 6c61 7465     def calculate
-00008a30: 5f64 6970 5f61 6e67 6c65 5f61 6e64 5f64  _dip_angle_and_d
-00008a40: 6972 6563 7469 6f6e 2841 2c20 4229 3a0d  irection(A, B):.
-00008a50: 0a20 2020 2020 2020 2023 2043 616c 6375  .        # Calcu
-00008a60: 6c61 7465 2074 6865 2064 6970 2061 6e67  late the dip ang
-00008a70: 6c65 2028 696e 636c 696e 6174 696f 6e29  le (inclination)
-00008a80: 0d0a 2020 2020 2020 2020 6469 705f 616e  ..        dip_an
-00008a90: 676c 6520 3d20 6d61 7468 2e64 6567 7265  gle = math.degre
-00008aa0: 6573 286d 6174 682e 6174 616e 286d 6174  es(math.atan(mat
-00008ab0: 682e 7371 7274 2841 2a2a 3220 2b20 422a  h.sqrt(A**2 + B*
-00008ac0: 2a32 2929 290d 0a20 2020 2020 2020 0d0a  *2)))..       ..
-00008ad0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00008ae0: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
-00008af0: 6520 6469 7020 6469 7265 6374 696f 6e20  e dip direction 
-00008b00: 2861 7a69 6d75 7468 290d 0a20 2020 2020  (azimuth)..     
-00008b10: 2020 2064 6970 5f64 6972 6563 7469 6f6e     dip_direction
-00008b20: 203d 206d 6174 682e 6465 6772 6565 7328   = math.degrees(
-00008b30: 6d61 7468 2e61 7461 6e32 282d 422c 202d  math.atan2(-B, -
-00008b40: 4129 290d 0a20 2020 2020 2020 200d 0a20  A))..        .. 
-00008b50: 2020 2020 2020 2023 2045 6e73 7572 6520         # Ensure 
-00008b60: 6469 705f 6469 7265 6374 696f 6e20 6973  dip_direction is
-00008b70: 2069 6e20 7468 6520 7261 6e67 6520 5b30   in the range [0
-00008b80: 2c20 3336 3029 0d0a 2020 2020 2020 2020  , 360)..        
-00008b90: 6469 705f 6469 7265 6374 696f 6e20 3d20  dip_direction = 
-00008ba0: 2864 6970 5f64 6972 6563 7469 6f6e 202b  (dip_direction +
-00008bb0: 2039 3029 2025 2033 3630 0d0a 2020 2020   90) % 360..    
-00008bc0: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-00008bd0: 7475 726e 2064 6970 5f61 6e67 6c65 2c20  turn dip_angle, 
-00008be0: 6469 705f 6469 7265 6374 696f 6e0d 0a20  dip_direction.. 
-00008bf0: 2020 200d 0a20 2020 2064 6566 2066 6974     ..    def fit
-00008c00: 5f70 6c61 6e65 2870 6f69 6e74 732c 2078  _plane(points, x
-00008c10: 782c 2079 7929 3a0d 0a20 2020 2020 2020  x, yy):..       
-00008c20: 206d 696e 5f72 616e 6765 203d 206e 702e   min_range = np.
-00008c30: 6e61 6e6d 696e 2864 6174 6129 0d0a 2020  nanmin(data)..  
-00008c40: 2020 2020 2020 6d61 785f 7261 6e67 6520        max_range 
-00008c50: 3d20 6e70 2e6e 616e 6d61 7828 6461 7461  = np.nanmax(data
-00008c60: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00008c70: 2020 2020 2023 2078 7820 3d20 2878 7820       # xx = (xx 
-00008c80: 2d20 6e70 2e6e 616e 6d69 6e28 7878 2929  - np.nanmin(xx))
-00008c90: 202f 2028 6e70 2e6e 616e 6d61 7828 7878   / (np.nanmax(xx
-00008ca0: 2920 2d20 6e70 2e6e 616e 6d69 6e28 7878  ) - np.nanmin(xx
-00008cb0: 2929 0d0a 2020 2020 2020 2020 2320 7878  ))..        # xx
-00008cc0: 203d 2078 7820 2a20 286d 6178 5f72 616e   = xx * (max_ran
-00008cd0: 6765 202d 206d 696e 5f72 616e 6765 2920  ge - min_range) 
-00008ce0: 2b20 6d69 6e5f 7261 6e67 650d 0a20 2020  + min_range..   
-00008cf0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00008d00: 2079 7920 3d20 2879 7920 2d20 6e70 2e6e   yy = (yy - np.n
-00008d10: 616e 6d69 6e28 7979 2929 202f 2028 6e70  anmin(yy)) / (np
-00008d20: 2e6e 616e 6d61 7828 7979 2920 2d20 6e70  .nanmax(yy) - np
-00008d30: 2e6e 616e 6d69 6e28 7979 2929 0d0a 2020  .nanmin(yy))..  
-00008d40: 2020 2020 2020 2320 7979 203d 2079 7920        # yy = yy 
-00008d50: 2a20 286d 6178 5f72 616e 6765 202d 206d  * (max_range - m
-00008d60: 696e 5f72 616e 6765 2920 2b20 6d69 6e5f  in_range) + min_
-00008d70: 7261 6e67 650d 0a20 2020 2020 2020 200d  range..        .
-00008d80: 0a20 2020 2020 2020 2078 5f76 616c 732c  .        x_vals,
-00008d90: 2079 5f76 616c 732c 207a 5f76 616c 7320   y_vals, z_vals 
-00008da0: 3d20 7a69 7028 2a70 6f69 6e74 7329 0d0a  = zip(*points)..
-00008db0: 2020 2020 0d0a 2020 2020 2020 2020 4120      ..        A 
-00008dc0: 3d20 6e70 2e76 7374 6163 6b28 5b78 5f76  = np.vstack([x_v
-00008dd0: 616c 732c 2079 5f76 616c 732c 206e 702e  als, y_vals, np.
-00008de0: 6f6e 6573 286c 656e 2878 5f76 616c 7329  ones(len(x_vals)
-00008df0: 295d 292e 540d 0a20 2020 2020 2020 2061  )]).T..        a
-00008e00: 2c20 622c 2063 203d 206e 702e 6c69 6e61  , b, c = np.lina
-00008e10: 6c67 2e6c 7374 7371 2841 2c20 7a5f 7661  lg.lstsq(A, z_va
-00008e20: 6c73 2c20 7263 6f6e 643d 4e6f 6e65 295b  ls, rcond=None)[
-00008e30: 305d 0d0a 2020 2020 2020 2020 0d0a 2020  0]..        ..  
-00008e40: 2020 2020 2020 7072 696e 7428 6622 506c        print(f"Pl
-00008e50: 616e 6520 6571 7561 7469 6f6e 3a20 7a20  ane equation: z 
-00008e60: 3d20 7b61 7d78 202b 207b 627d 7920 2b20  = {a}x + {b}y + 
-00008e70: 7b63 7d22 2920 2023 2044 6562 7567 6769  {c}")  # Debuggi
-00008e80: 6e67 206c 696e 650d 0a20 2020 2020 2020  ng line..       
-00008e90: 200d 0a20 2020 2020 2020 207a 7a20 3d20   ..        zz = 
-00008ea0: 6120 2a20 7878 202b 2062 202a 2079 7920  a * xx + b * yy 
-00008eb0: 2b20 630d 0a20 2020 2020 2020 2023 2323  + c..        ###
-00008ec0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00008ed0: 2323 2323 2323 2323 2323 2323 2323 230d  ###############.
-00008ee0: 0a20 2020 2020 2020 2023 2070 6f69 6e74  .        # point
-00008ef0: 7320 3d20 6e70 2e61 7272 6179 2870 6f69  s = np.array(poi
-00008f00: 6e74 7329 200d 0a20 2020 2020 2020 2023  nts) ..        #
-00008f10: 2023 2043 6f6d 7075 7465 2074 6865 2063   # Compute the c
-00008f20: 656e 7472 6f69 6420 6f66 2074 6865 2070  entroid of the p
-00008f30: 6f69 6e74 730d 0a20 2020 2020 2020 2023  oints..        #
-00008f40: 2063 656e 7472 6f69 6420 3d20 6e70 2e6d   centroid = np.m
-00008f50: 6561 6e28 706f 696e 7473 2c20 6178 6973  ean(points, axis
-00008f60: 3d30 290d 0a0d 0a20 2020 2020 2020 2023  =0)....        #
-00008f70: 2023 2053 7562 7472 6163 7420 7468 6520   # Subtract the 
-00008f80: 6365 6e74 726f 6964 2066 726f 6d20 7468  centroid from th
-00008f90: 6520 706f 696e 7473 2074 6f20 6365 6e74  e points to cent
-00008fa0: 6572 2074 6865 6d0d 0a20 2020 2020 2020  er them..       
-00008fb0: 2023 2063 656e 7465 7265 645f 706f 696e   # centered_poin
-00008fc0: 7473 203d 2070 6f69 6e74 7320 2d20 6365  ts = points - ce
-00008fd0: 6e74 726f 6964 0d0a 0d0a 2020 2020 2020  ntroid....      
-00008fe0: 2020 2320 2320 5065 7266 6f72 6d20 5356    # # Perform SV
-00008ff0: 4420 6f6e 2074 6865 2063 656e 7465 7265  D on the centere
-00009000: 6420 706f 696e 7473 0d0a 2020 2020 2020  d points..      
-00009010: 2020 2320 552c 2053 2c20 5674 203d 206e    # U, S, Vt = n
-00009020: 702e 6c69 6e61 6c67 2e73 7664 2863 656e  p.linalg.svd(cen
-00009030: 7465 7265 645f 706f 696e 7473 290d 0a0d  tered_points)...
-00009040: 0a20 2020 2020 2020 2023 2023 2054 6865  .        # # The
-00009050: 206e 6f72 6d61 6c20 7665 6374 6f72 206f   normal vector o
-00009060: 6620 7468 6520 706c 616e 6520 6973 2074  f the plane is t
-00009070: 6865 206c 6173 7420 726f 7720 6f66 2056  he last row of V
-00009080: 740d 0a20 2020 2020 2020 2023 206e 6f72  t..        # nor
-00009090: 6d61 6c5f 7665 6374 6f72 203d 2056 745b  mal_vector = Vt[
-000090a0: 2d31 2c20 3a5d 0d0a 0d0a 2020 2020 2020  -1, :]....      
-000090b0: 2020 2320 2320 4e6f 726d 616c 697a 6520    # # Normalize 
-000090c0: 7468 6520 6e6f 726d 616c 2076 6563 746f  the normal vecto
-000090d0: 720d 0a20 2020 2020 2020 2023 206e 6f72  r..        # nor
-000090e0: 6d61 6c5f 7665 6374 6f72 202f 3d20 6e70  mal_vector /= np
-000090f0: 2e6c 696e 616c 672e 6e6f 726d 286e 6f72  .linalg.norm(nor
-00009100: 6d61 6c5f 7665 6374 6f72 290d 0a0d 0a20  mal_vector).... 
-00009110: 2020 2020 2020 2023 2023 2054 6865 2065         # # The e
-00009120: 7175 6174 696f 6e20 6f66 2074 6865 2070  quation of the p
-00009130: 6c61 6e65 2069 733a 2061 7820 2b20 6279  lane is: ax + by
-00009140: 202b 2063 7a20 2b20 6420 3d20 302c 2077   + cz + d = 0, w
-00009150: 6865 7265 205b 612c 2062 2c20 635d 2069  here [a, b, c] i
-00009160: 7320 7468 6520 6e6f 726d 616c 2076 6563  s the normal vec
-00009170: 746f 720d 0a20 2020 2020 2020 2023 2061  tor..        # a
-00009180: 2c20 622c 2063 203d 206e 6f72 6d61 6c5f  , b, c = normal_
-00009190: 7665 6374 6f72 0d0a 0d0a 2020 2020 2020  vector....      
-000091a0: 2020 2320 2320 4361 6c63 756c 6174 6520    # # Calculate 
-000091b0: 6420 7573 696e 6720 7468 6520 706c 616e  d using the plan
-000091c0: 6520 6571 7561 7469 6f6e 2061 6e64 2074  e equation and t
-000091d0: 6865 2063 656e 7472 6f69 640d 0a20 2020  he centroid..   
-000091e0: 2020 2020 2023 2064 203d 202d 6e70 2e64       # d = -np.d
-000091f0: 6f74 286e 6f72 6d61 6c5f 7665 6374 6f72  ot(normal_vector
-00009200: 2c20 6365 6e74 726f 6964 290d 0a20 2020  , centroid)..   
-00009210: 2020 2020 2023 207a 7a20 3d20 282d 6120       # zz = (-a 
-00009220: 2a20 7878 202d 2062 202a 2079 7920 2d20  * xx - b * yy - 
-00009230: 6429 202f 2063 2020 2320 536f 6c76 6520  d) / c  # Solve 
-00009240: 666f 7220 7a0d 0a20 2020 2020 2020 200d  for z..        .
-00009250: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-00009260: 2020 6469 705f 616e 676c 652c 2064 6970    dip_angle, dip
-00009270: 5f64 6972 6563 7469 6f6e 203d 2063 616c  _direction = cal
-00009280: 6375 6c61 7465 5f64 6970 5f61 6e67 6c65  culate_dip_angle
-00009290: 5f61 6e64 5f64 6972 6563 7469 6f6e 2861  _and_direction(a
-000092a0: 2c20 6229 0d0a 0d0a 2020 2020 2020 2020  , b)....        
-000092b0: 7072 696e 7428 6622 4469 7020 416e 676c  print(f"Dip Angl
-000092c0: 6520 2849 6e63 6c69 6e61 7469 6f6e 293a  e (Inclination):
-000092d0: 207b 6469 705f 616e 676c 657d 2064 6567   {dip_angle} deg
-000092e0: 7265 6573 2229 0d0a 2020 2020 2020 2020  rees")..        
-000092f0: 7072 696e 7428 6622 4469 7020 4469 7265  print(f"Dip Dire
-00009300: 6374 696f 6e20 2841 7a69 6d75 7468 293a  ction (Azimuth):
-00009310: 207b 6469 705f 6469 7265 6374 696f 6e7d   {dip_direction}
-00009320: 2064 6567 7265 6573 2229 0d0a 2020 2020   degrees")..    
-00009330: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-00009340: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00009350: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00009360: 2020 2020 2023 2020 2320 436c 6970 2074       #  # Clip t
-00009370: 6865 2076 616c 7565 7320 746f 2074 6865  he values to the
-00009380: 2064 6573 6972 6564 2072 616e 6765 0d0a   desired range..
-00009390: 2020 2020 2020 2020 237a 7a20 3d20 6e70          #zz = np
-000093a0: 2e63 6c69 7028 7a7a 2c20 6d69 6e5f 7261  .clip(zz, min_ra
-000093b0: 6e67 652c 206d 6178 5f72 616e 6765 290d  nge, max_range).
-000093c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000093d0: 2020 207a 7a5b 7a7a 203c 206d 696e 5f72     zz[zz < min_r
-000093e0: 616e 6765 5d20 3d20 6e70 2e6e 616e 0d0a  ange] = np.nan..
-000093f0: 2020 2020 2020 2020 7a7a 5b7a 7a20 3e20          zz[zz > 
-00009400: 6d61 785f 7261 6e67 655d 203d 206e 702e  max_range] = np.
-00009410: 6e61 6e0d 0a20 2020 2020 2020 0d0a 2020  nan..       ..  
-00009420: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00009430: 2023 2044 6566 696e 6520 7468 6520 6465   # Define the de
-00009440: 7369 7265 6420 7261 6e67 6520 6261 7365  sired range base
-00009450: 6420 6f6e 2079 6f75 7220 2764 6174 6127  d on your 'data'
-00009460: 0d0a 2020 2020 2020 2020 2320 6966 206c  ..        # if l
-00009470: 696d 6974 5f65 7874 656e 643d 3d46 616c  imit_extend==Fal
-00009480: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00009490: 0d0a 2020 2020 2020 2020 2320 2320 2320  ..        # # # 
-000094a0: 2320 4e6f 726d 616c 697a 6520 277a 7a27  # Normalize 'zz'
-000094b0: 2074 6f20 6d61 7463 6820 7468 6520 276d   to match the 'm
-000094c0: 696e 5f72 616e 6765 2720 616e 6420 276d  in_range' and 'm
-000094d0: 6178 5f72 616e 6765 2720 6f66 2027 6461  ax_range' of 'da
-000094e0: 7461 270d 0a20 2020 2020 2020 2023 207a  ta'..        # z
-000094f0: 7a20 3d20 287a 7a20 2d20 6e70 2e6e 616e  z = (zz - np.nan
-00009500: 6d69 6e28 7a7a 2929 202f 2028 6e70 2e6e  min(zz)) / (np.n
-00009510: 616e 6d61 7828 7a7a 2920 2d20 6e70 2e6e  anmax(zz) - np.n
-00009520: 616e 6d69 6e28 7a7a 2929 0d0a 2020 2020  anmin(zz))..    
-00009530: 2020 2020 2320 7a7a 203d 207a 7a20 2a20      # zz = zz * 
-00009540: 286d 6178 5f72 616e 6765 202d 206d 696e  (max_range - min
-00009550: 5f72 616e 6765 2920 2b20 6d69 6e5f 7261  _range) + min_ra
-00009560: 6e67 650d 0a20 2020 2020 2020 200d 0a20  nge..        .. 
-00009570: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-00009580: 2020 2020 2020 2020 2320 7072 696e 7428          # print(
-00009590: 7a7a 2e73 6861 7065 290d 0a20 2020 2020  zz.shape)..     
-000095a0: 2020 2023 2070 7269 6e74 287a 7a29 0d0a     # print(zz)..
-000095b0: 2020 2020 2020 2020 7265 7475 726e 207a          return z
-000095c0: 7a2c 2061 2c20 622c 2063 2c20 6469 705f  z, a, b, c, dip_
-000095d0: 616e 676c 652c 2064 6970 5f64 6972 6563  angle, dip_direc
-000095e0: 7469 6f6e 0d0a 2020 2020 0d0a 2020 200d  tion..    ..   .
-000095f0: 0a20 2020 0d0a 2020 200d 0a0d 0a20 2020  .   ..   ....   
-00009600: 2064 6566 206f 6e63 6c69 636b 2865 7665   def onclick(eve
-00009610: 6e74 2c20 706f 696e 7473 2c20 6461 7461  nt, points, data
-00009620: 2c20 7472 616e 7366 6f72 6d29 3a0d 0a20  , transform):.. 
-00009630: 2020 2020 2020 2078 2c20 7920 3d20 6576         x, y = ev
-00009640: 656e 742e 7864 6174 612c 2065 7665 6e74  ent.xdata, event
-00009650: 2e79 6461 7461 0d0a 2020 2020 2020 2020  .ydata..        
-00009660: 636f 6c20 3d20 696e 7428 2878 202d 2074  col = int((x - t
-00009670: 7261 6e73 666f 726d 5b30 5d29 202f 2074  ransform[0]) / t
-00009680: 7261 6e73 666f 726d 5b31 5d29 0d0a 2020  ransform[1])..  
-00009690: 2020 2020 2020 726f 7720 3d20 696e 7428        row = int(
-000096a0: 2879 202d 2074 7261 6e73 666f 726d 5b33  (y - transform[3
-000096b0: 5d29 202f 2074 7261 6e73 666f 726d 5b35  ]) / transform[5
-000096c0: 5d29 0d0a 0d0a 2020 2020 2020 2020 6966  ])....        if
-000096d0: 2030 203c 3d20 636f 6c20 3c20 6461 7461   0 <= col < data
-000096e0: 2e73 6861 7065 5b31 5d20 616e 6420 3020  .shape[1] and 0 
-000096f0: 3c3d 2072 6f77 203c 2064 6174 612e 7368  <= row < data.sh
-00009700: 6170 655b 305d 3a0d 0a20 2020 2020 2020  ape[0]:..       
-00009710: 2020 2020 207a 203d 2064 6174 615b 726f       z = data[ro
-00009720: 772c 2063 6f6c 5d0d 0a20 2020 2020 2020  w, col]..       
-00009730: 2020 2020 2070 6f69 6e74 732e 6170 7065       points.appe
-00009740: 6e64 285b 782c 2079 2c20 7a5d 290d 0a20  nd([x, y, z]).. 
-00009750: 2020 2020 2020 2020 2020 2061 785f 3264             ax_2d
-00009760: 2e70 6c6f 7428 782c 2079 2c20 276f 272c  .plot(x, y, 'o',
-00009770: 2063 6f6c 6f72 3d27 626c 6163 6b27 290d   color='black').
-00009780: 0a20 2020 2020 2020 2020 2020 2063 616e  .            can
-00009790: 7661 735f 3264 2e64 7261 7728 290d 0a0d  vas_2d.draw()...
-000097a0: 0a20 2020 2020 2020 2020 2020 2070 6f69  .            poi
-000097b0: 6e74 5f73 7472 203d 2066 2278 3d7b 783a  nt_str = f"x={x:
-000097c0: 2e32 667d 2c20 793d 7b79 3a2e 3266 7d2c  .2f}, y={y:.2f},
-000097d0: 207a 3d7b 7a3a 2e32 667d 220d 0a20 2020   z={z:.2f}"..   
-000097e0: 2020 2020 2020 2020 2070 6f69 6e74 735f           points_
-000097f0: 6c69 7374 626f 782e 696e 7365 7274 2874  listbox.insert(t
-00009800: 6b2e 454e 442c 2070 6f69 6e74 5f73 7472  k.END, point_str
-00009810: 290d 0a0d 0a20 2020 2064 6566 206f 6e5f  )....    def on_
-00009820: 706f 696e 745f 646f 7562 6c65 5f63 6c69  point_double_cli
-00009830: 636b 2865 7665 6e74 293a 0d0a 2020 2020  ck(event):..    
-00009840: 2020 2020 676c 6f62 616c 2070 6f69 6e74      global point
-00009850: 732c 2061 785f 3264 2c20 706f 696e 7473  s, ax_2d, points
-00009860: 5f6c 6973 7462 6f78 2c20 6873 0d0a 2020  _listbox, hs..  
-00009870: 2020 2020 2020 6964 7820 3d20 706f 696e        idx = poin
-00009880: 7473 5f6c 6973 7462 6f78 2e63 7572 7365  ts_listbox.curse
-00009890: 6c65 6374 696f 6e28 295b 305d 2020 2320  lection()[0]  # 
-000098a0: 496e 6465 7820 6f66 2073 656c 6563 7465  Index of selecte
-000098b0: 6420 706f 696e 7420 696e 2074 6865 206c  d point in the l
-000098c0: 6973 7462 6f78 0d0a 2020 2020 2020 2020  istbox..        
-000098d0: 706f 696e 7420 3d20 706f 696e 7473 5b69  point = points[i
-000098e0: 6478 5d0d 0a20 2020 2020 2020 200d 0a20  dx]..        .. 
-000098f0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-00009900: 7468 6520 706f 696e 7420 6672 6f6d 206f  the point from o
-00009910: 7572 2064 6174 610d 0a20 2020 2020 2020  ur data..       
-00009920: 2070 6f69 6e74 732e 706f 7028 6964 7829   points.pop(idx)
-00009930: 0d0a 2020 2020 2020 2020 706f 696e 7473  ..        points
-00009940: 5f6c 6973 7462 6f78 2e64 656c 6574 6528  _listbox.delete(
-00009950: 6964 7829 0d0a 0d0a 2020 2020 2020 2020  idx)....        
-00009960: 2320 4964 656e 7469 6679 2061 6e64 2072  # Identify and r
-00009970: 656d 6f76 6520 7468 6520 636f 7272 6573  emove the corres
-00009980: 706f 6e64 696e 6720 706f 696e 7420 6672  ponding point fr
-00009990: 6f6d 2074 6865 2061 785f 3264 2070 6c6f  om the ax_2d plo
-000099a0: 740d 0a20 2020 2020 2020 2066 6f72 206c  t..        for l
-000099b0: 696e 6520 696e 2061 785f 3264 2e6c 696e  ine in ax_2d.lin
-000099c0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-000099d0: 2078 6461 7461 2c20 7964 6174 6120 3d20   xdata, ydata = 
-000099e0: 6c69 6e65 2e67 6574 5f78 6461 7461 2829  line.get_xdata()
-000099f0: 2c20 6c69 6e65 2e67 6574 5f79 6461 7461  , line.get_ydata
-00009a00: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00009a10: 6966 2078 6461 7461 5b30 5d20 3d3d 2070  if xdata[0] == p
-00009a20: 6f69 6e74 5b30 5d20 616e 6420 7964 6174  oint[0] and ydat
-00009a30: 615b 305d 203d 3d20 706f 696e 745b 315d  a[0] == point[1]
-00009a40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00009a50: 2020 206c 696e 652e 7265 6d6f 7665 2829     line.remove()
-00009a60: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009a70: 2020 6272 6561 6b0d 0a0d 0a20 2020 2020    break....     
-00009a80: 2020 2063 616e 7661 735f 3264 2e64 7261     canvas_2d.dra
-00009a90: 7728 290d 0a20 2020 2020 2020 200d 0a20  w()..        .. 
-00009aa0: 2020 2020 2020 200d 0a20 2020 200d 0a20         ..    .. 
-00009ab0: 2020 200d 0a20 2020 2064 6566 2070 6c6f     ..    def plo
-00009ac0: 745f 706c 616e 6573 2864 6970 5f6c 6973  t_planes(dip_lis
-00009ad0: 742c 2061 7a69 6d75 7468 5f6c 6973 742c  t, azimuth_list,
-00009ae0: 2072 6762 5f63 6f6c 6f72 732c 206f 7574   rgb_colors, out
-00009af0: 5f70 6c61 6e65 466f 6c64 6572 3d6f 7574  _planeFolder=out
-00009b00: 5f70 6c61 6e65 466f 6c64 6572 293a 0d0a  _planeFolder):..
-00009b10: 2020 2020 2020 2020 2366 726f 6d20 6d70          #from mp
-00009b20: 6c73 7465 7265 6f6e 6574 2069 6d70 6f72  lstereonet impor
-00009b30: 7420 5374 6572 656f 6e65 7441 7865 730d  t StereonetAxes.
-00009b40: 0a20 2020 2020 2020 2020 2320 4372 6561  .         # Crea
-00009b50: 7465 2061 2073 7465 7265 6f20 6e65 7420  te a stereo net 
-00009b60: 706c 6f74 0d0a 2020 2020 2020 2020 6669  plot..        fi
-00009b70: 6720 3d20 706c 742e 6669 6775 7265 2866  g = plt.figure(f
-00009b80: 6967 7369 7a65 3d28 3130 2c20 3130 292c  igsize=(10, 10),
-00009b90: 2064 7069 3d33 3030 290d 0a20 2020 2020   dpi=300)..     
-00009ba0: 2020 2023 6178 203d 2066 6967 2e61 6464     #ax = fig.add
-00009bb0: 5f73 7562 706c 6f74 2831 3231 2c20 7072  _subplot(121, pr
-00009bc0: 6f6a 6563 7469 6f6e 3d27 7374 6572 656f  ojection='stereo
-00009bd0: 6e65 7427 290d 0a20 2020 2020 2020 2061  net')..        a
-00009be0: 783d 6669 672e 6164 645f 7375 6270 6c6f  x=fig.add_subplo
-00009bf0: 7428 3132 312c 2070 6f6c 6172 3d54 7275  t(121, polar=Tru
-00009c00: 6529 0d0a 0d0a 2020 2020 2020 2020 666f  e)....        fo
-00009c10: 7220 6469 705f 616e 676c 6573 2c20 6469  r dip_angles, di
-00009c20: 705f 6469 7265 6374 696f 6e73 2c20 636f  p_directions, co
-00009c30: 6c6f 7220 696e 207a 6970 2864 6970 5f6c  lor in zip(dip_l
-00009c40: 6973 742c 2061 7a69 6d75 7468 5f6c 6973  ist, azimuth_lis
-00009c50: 742c 2072 6762 5f63 6f6c 6f72 7329 3a0d  t, rgb_colors):.
-00009c60: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
-00009c70: 6f6e 7665 7274 2064 6970 2064 6972 6563  onvert dip direc
-00009c80: 7469 6f6e 7320 616e 6420 6469 7020 616e  tions and dip an
-00009c90: 676c 6573 2074 6f20 7261 6469 616e 730d  gles to radians.
-00009ca0: 0a20 2020 2020 2020 2020 2020 2023 6469  .            #di
-00009cb0: 705f 6469 7265 6374 696f 6e73 203d 2028  p_directions = (
-00009cc0: 6469 705f 6469 7265 6374 696f 6e73 202b  dip_directions +
-00009cd0: 2039 3029 2025 2033 3630 2023 636f 6e76   90) % 360 #conv
-00009ce0: 6572 7465 6420 6469 7020 6469 7265 6374  erted dip direct
-00009cf0: 696f 6e20 746f 2073 7472 696b 650d 0a20  ion to strike.. 
-00009d00: 2020 2020 2020 2020 2020 2064 6970 5f61             dip_a
-00009d10: 6e67 6c65 7320 3d20 2839 3020 2d20 6e70  ngles = (90 - np
-00009d20: 2e61 7272 6179 2864 6970 5f61 6e67 6c65  .array(dip_angle
-00009d30: 7329 2920 2023 2043 6f6e 7665 7274 2064  s))  # Convert d
-00009d40: 6970 2061 6e67 6c65 7320 746f 2063 6f6d  ip angles to com
-00009d50: 706c 656d 656e 7461 7279 2061 6e67 6c65  plementary angle
-00009d60: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
-00009d70: 2320 436f 6e76 6572 7420 6469 7020 617a  # Convert dip az
-00009d80: 696d 7574 6873 2074 6f20 7261 6469 616e  imuths to radian
-00009d90: 730d 0a20 2020 2020 2020 2020 2020 2064  s..            d
-00009da0: 6970 5f61 7a69 6d75 7468 735f 7261 6420  ip_azimuths_rad 
-00009db0: 3d20 6e70 2e72 6164 6961 6e73 2864 6970  = np.radians(dip
-00009dc0: 5f64 6972 6563 7469 6f6e 7329 0d0a 2020  _directions)..  
-00009dd0: 2020 2020 2020 2020 2020 2320 506c 6f74            # Plot
-00009de0: 2074 6865 2070 6f6c 6573 206f 6620 706c   the poles of pl
-00009df0: 616e 6573 2061 7320 646f 7473 0d0a 2020  anes as dots..  
-00009e00: 2020 2020 2020 2020 2020 6178 2e73 6361            ax.sca
-00009e10: 7474 6572 2864 6970 5f61 7a69 6d75 7468  tter(dip_azimuth
-00009e20: 735f 7261 642c 2064 6970 5f61 6e67 6c65  s_rad, dip_angle
-00009e30: 732c 2063 6f6c 6f72 3d63 6f6c 6f72 2920  s, color=color) 
-00009e40: 2020 0d0a 0d0a 2020 2020 2020 2020 6178    ....        ax
-00009e50: 2e67 7269 6428 5472 7565 290d 0a20 2020  .grid(True)..   
-00009e60: 2020 2020 2061 782e 7365 745f 7468 6574       ax.set_thet
-00009e70: 615f 7a65 726f 5f6c 6f63 6174 696f 6e28  a_zero_location(
-00009e80: 274e 2729 2020 2320 5365 7420 3020 6465  'N')  # Set 0 de
-00009e90: 6772 6565 7320 6174 2074 6865 2074 6f70  grees at the top
-00009ea0: 0d0a 2020 2020 2020 2020 6178 2e73 6574  ..        ax.set
-00009eb0: 5f74 6865 7461 5f64 6972 6563 7469 6f6e  _theta_direction
-00009ec0: 282d 3129 2020 2320 5265 7665 7273 6520  (-1)  # Reverse 
-00009ed0: 7468 6520 6469 7265 6374 696f 6e20 6f66  the direction of
-00009ee0: 2074 6865 2061 6e67 6c65 730d 0a0d 0a20   the angles.... 
-00009ef0: 2020 2020 2020 2023 2053 6574 206c 6162         # Set lab
-00009f00: 656c 7320 666f 7220 6361 7264 696e 616c  els for cardinal
-00009f10: 2064 6972 6563 7469 6f6e 730d 0a20 2020   directions..   
-00009f20: 2020 2020 2061 782e 7365 745f 7874 6963       ax.set_xtic
-00009f30: 6b73 286e 702e 7261 6469 616e 7328 5b30  ks(np.radians([0
-00009f40: 2c20 3435 2c20 3930 2c20 3133 352c 2031  , 45, 90, 135, 1
-00009f50: 3830 2c20 3232 352c 2032 3730 2c20 3331  80, 225, 270, 31
-00009f60: 355d 2929 0d0a 2020 2020 2020 2020 6178  5]))..        ax
-00009f70: 2e73 6574 5f78 7469 636b 6c61 6265 6c73  .set_xticklabels
-00009f80: 285b 274e 272c 2027 4e45 272c 2027 4527  (['N', 'NE', 'E'
-00009f90: 2c20 2753 4527 2c20 2753 272c 2027 5357  , 'SE', 'S', 'SW
-00009fa0: 272c 2027 5727 2c20 274e 5727 5d29 0d0a  ', 'W', 'NW'])..
-00009fb0: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-00009fc0: 7468 6520 7261 6469 616c 2067 7269 6420  the radial grid 
-00009fd0: 616e 6420 6c61 6265 6c73 0d0a 2020 2020  and labels..    
-00009fe0: 2020 2020 6178 2e73 6574 5f72 6c61 6265      ax.set_rlabe
-00009ff0: 6c5f 706f 7369 7469 6f6e 2839 3029 0d0a  l_position(90)..
-0000a000: 2020 2020 2020 2020 6178 2e73 6574 5f79          ax.set_y
-0000a010: 7469 636b 7328 5b31 352c 2033 302c 2034  ticks([15, 30, 4
-0000a020: 352c 2036 302c 2037 355d 290d 0a20 2020  5, 60, 75])..   
-0000a030: 2020 2020 2061 782e 7365 745f 726d 6178       ax.set_rmax
-0000a040: 2839 3029 2020 2320 5365 7420 7468 6520  (90)  # Set the 
-0000a050: 6d61 7869 6d75 6d20 7261 6469 616c 2064  maximum radial d
-0000a060: 6973 7461 6e63 650d 0a20 2020 2020 2020  istance..       
-0000a070: 2061 782e 7365 745f 7469 746c 6528 2250   ax.set_title("P
-0000a080: 6f6c 6573 2074 6f20 506c 616e 6573 2229  oles to Planes")
-0000a090: 0d0a 2020 2020 2020 2020 2320 4375 7374  ..        # Cust
-0000a0a0: 6f6d 697a 6520 7469 636b 206d 6172 6b73  omize tick marks
-0000a0b0: 202d 2073 7065 6369 6679 2061 6e67 6c65   - specify angle
-0000a0c0: 7320 696e 2072 6164 6961 6e73 0d0a 2020  s in radians..  
-0000a0d0: 2020 2020 2020 2320 6178 2e73 6574 5f78        # ax.set_x
-0000a0e0: 7469 636b 7328 6e70 2e72 6164 6961 6e73  ticks(np.radians
-0000a0f0: 2872 616e 6765 2830 2c20 3336 302c 2031  (range(0, 360, 1
-0000a100: 3029 2929 2020 2320 3130 2d64 6567 7265  0)))  # 10-degre
-0000a110: 6520 696e 7465 7276 616c 730d 0a20 2020  e intervals..   
-0000a120: 2020 2020 2023 2061 782e 7365 745f 7974       # ax.set_yt
-0000a130: 6963 6b73 286e 702e 7261 6469 616e 7328  icks(np.radians(
-0000a140: 7261 6e67 6528 2d39 302c 2039 302c 2031  range(-90, 90, 1
-0000a150: 3029 2929 0d0a 0d0a 2020 2020 2020 2020  0)))....        
-0000a160: 7374 7269 6b65 733d 5b5d 0d0a 2020 2020  strikes=[]..    
-0000a170: 2020 2020 616c 6c5f 636f 6c6f 7273 3d5b      all_colors=[
-0000a180: 5d0d 0a20 2020 2020 2020 2066 6f72 2064  ]..        for d
-0000a190: 6970 5f61 6e67 6c65 732c 2064 6970 5f64  ip_angles, dip_d
-0000a1a0: 6972 6563 7469 6f6e 732c 2063 6f6c 6f72  irections, color
-0000a1b0: 2069 6e20 7a69 7028 6469 705f 6c69 7374   in zip(dip_list
-0000a1c0: 2c20 617a 696d 7574 685f 6c69 7374 2c20  , azimuth_list, 
-0000a1d0: 7267 625f 636f 6c6f 7273 293a 0d0a 2020  rgb_colors):..  
-0000a1e0: 2020 2020 2020 2020 2020 6469 705f 617a            dip_az
-0000a1f0: 696d 7574 6873 5f72 6164 203d 206e 702e  imuths_rad = np.
-0000a200: 7261 6469 616e 7328 6469 705f 6469 7265  radians(dip_dire
-0000a210: 6374 696f 6e73 290d 0a20 2020 2020 2020  ctions)..       
-0000a220: 2020 2020 2023 6469 705f 6469 7265 6374       #dip_direct
-0000a230: 696f 6e73 203d 2028 6469 705f 6469 7265  ions = (dip_dire
-0000a240: 6374 696f 6e73 202b 2039 3029 2025 2033  ctions + 90) % 3
-0000a250: 3630 0d0a 2020 2020 2020 2020 2020 2020  60..            
-0000a260: 6469 705f 616e 676c 6573 203d 2028 3930  dip_angles = (90
-0000a270: 202d 206e 702e 6172 7261 7928 6469 705f   - np.array(dip_
-0000a280: 616e 676c 6573 2929 2020 2320 436f 6e76  angles))  # Conv
-0000a290: 6572 7420 6469 7020 616e 676c 6573 2074  ert dip angles t
-0000a2a0: 6f20 636f 6d70 6c65 6d65 6e74 6172 7920  o complementary 
-0000a2b0: 616e 676c 6573 0d0a 2020 2020 2020 2020  angles..        
-0000a2c0: 2020 2020 7374 7269 6b65 732e 6170 7065      strikes.appe
-0000a2d0: 6e64 2828 6469 705f 617a 696d 7574 6873  nd((dip_azimuths
-0000a2e0: 5f72 6164 202b 2039 3029 2025 2033 3630  _rad + 90) % 360
-0000a2f0: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
-0000a300: 6c6c 5f63 6f6c 6f72 732e 6170 7065 6e64  ll_colors.append
-0000a310: 2863 6f6c 6f72 290d 0a20 2020 2020 2020  (color)..       
-0000a320: 200d 0a0d 0a20 2020 2020 2020 2020 2320   ....         # 
-0000a330: 4361 6c63 756c 6174 6520 7468 6520 6e75  Calculate the nu
-0000a340: 6d62 6572 206f 6620 6269 6e73 2075 7369  mber of bins usi
-0000a350: 6e67 2053 636f 7474 2773 2052 756c 650d  ng Scott's Rule.
-0000a360: 0a20 2020 2020 2020 206e 203d 206c 656e  .        n = len
-0000a370: 2873 7472 696b 6573 290d 0a0d 0a20 2020  (strikes)....   
-0000a380: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
-0000a390: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-0000a3a0: 7669 6174 696f 6e20 6f66 2074 6865 2064  viation of the d
-0000a3b0: 6174 610d 0a20 2020 2020 2020 2073 7464  ata..        std
-0000a3c0: 5f64 6576 203d 206e 702e 7374 6428 7374  _dev = np.std(st
-0000a3d0: 7269 6b65 7329 0d0a 0d0a 2020 2020 2020  rikes)....      
-0000a3e0: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
-0000a3f0: 6520 6269 6e20 7769 6474 6820 7573 696e  e bin width usin
-0000a400: 6720 5363 6f74 7427 7320 5275 6c65 2066  g Scott's Rule f
-0000a410: 6f72 6d75 6c61 2c20 656e 7375 7269 6e67  ormula, ensuring
-0000a420: 2069 7427 7320 6e6f 7420 7a65 726f 0d0a   it's not zero..
-0000a430: 2020 2020 2020 2020 6966 2073 7464 5f64          if std_d
-0000a440: 6576 2021 3d20 303a 0d0a 2020 2020 2020  ev != 0:..      
-0000a450: 2020 2020 2020 6269 6e5f 7769 6474 6820        bin_width 
-0000a460: 3d20 302e 3520 2a20 7374 645f 6465 7620  = 0.5 * std_dev 
-0000a470: 2f20 286e 2a2a 2831 2f33 2929 2020 2320  / (n**(1/3))  # 
-0000a480: 5363 6f74 7427 7320 5275 6c65 2066 6f72  Scott's Rule for
-0000a490: 6d75 6c61 0d0a 2020 2020 2020 2020 2020  mula..          
-0000a4a0: 2020 6e75 6d5f 6269 6e73 203d 206d 6178    num_bins = max
-0000a4b0: 2869 6e74 2828 6d61 7828 7374 7269 6b65  (int((max(strike
-0000a4c0: 7329 202d 206d 696e 2873 7472 696b 6573  s) - min(strikes
-0000a4d0: 2929 202f 2062 696e 5f77 6964 7468 292c  )) / bin_width),
-0000a4e0: 2031 2920 2023 2045 6e73 7572 6520 6e75   1)  # Ensure nu
-0000a4f0: 6d5f 6269 6e73 2069 7320 6174 206c 6561  m_bins is at lea
-0000a500: 7374 2031 0d0a 2020 2020 2020 2020 656c  st 1..        el
-0000a510: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0000a520: 206e 756d 5f62 696e 7320 3d20 3132 2020   num_bins = 12  
-0000a530: 2320 4120 6465 6661 756c 7420 6e75 6d62  # A default numb
-0000a540: 6572 206f 6620 6269 6e73 2069 6620 7374  er of bins if st
-0000a550: 645f 6465 7620 6973 207a 6572 6f0d 0a20  d_dev is zero.. 
-0000a560: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0000a570: 6120 726f 7365 2064 6961 6772 616d 2028  a rose diagram (
-0000a580: 6369 7263 756c 6172 2068 6973 746f 6772  circular histogr
-0000a590: 616d 290d 0a20 2020 2020 2020 2061 785f  am)..        ax_
-0000a5a0: 726f 7365 203d 2066 6967 2e61 6464 5f73  rose = fig.add_s
-0000a5b0: 7562 706c 6f74 2831 3232 2c20 706f 6c61  ubplot(122, pola
-0000a5c0: 723d 5472 7565 290d 0a0d 0a20 2020 2020  r=True)....     
-0000a5d0: 2020 2066 6f72 2064 6970 2c20 7374 7269     for dip, stri
-0000a5e0: 6b65 2c20 636f 6c6f 722c 2061 7a20 696e  ke, color, az in
-0000a5f0: 207a 6970 2864 6970 5f6c 6973 742c 2073   zip(dip_list, s
-0000a600: 7472 696b 6573 2c20 616c 6c5f 636f 6c6f  trikes, all_colo
-0000a610: 7273 2c20 617a 696d 7574 685f 6c69 7374  rs, azimuth_list
-0000a620: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0000a630: 2320 436f 6e76 6572 7420 6469 7020 617a  # Convert dip az
-0000a640: 696d 7574 6873 2074 6f20 7261 6469 616e  imuths to radian
-0000a650: 730d 0a20 2020 2020 2020 2020 2020 2064  s..            d
-0000a660: 6970 5f61 7a69 6d75 7468 735f 7261 6420  ip_azimuths_rad 
-0000a670: 3d20 6e70 2e72 6164 6961 6e73 2861 7a29  = np.radians(az)
-0000a680: 0d0a 2020 2020 2020 2020 2020 2020 6469  ..            di
-0000a690: 705f 616e 676c 6573 203d 2028 3930 202d  p_angles = (90 -
-0000a6a0: 206e 702e 6172 7261 7928 6469 705f 616e   np.array(dip_an
-0000a6b0: 676c 6573 2929 2020 2320 436f 6e76 6572  gles))  # Conver
-0000a6c0: 7420 6469 7020 616e 676c 6573 2074 6f20  t dip angles to 
-0000a6d0: 636f 6d70 6c65 6d65 6e74 6172 7920 616e  complementary an
-0000a6e0: 676c 6573 0d0a 2020 2020 2020 2020 2020  gles..          
-0000a6f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000a700: 2320 506c 6f74 2064 6970 2061 6e67 6c65  # Plot dip angle
-0000a710: 7320 6173 2072 6164 6969 2061 6e64 2064  s as radii and d
-0000a720: 6970 2061 7a69 6d75 7468 7320 6173 2061  ip azimuths as a
-0000a730: 6e67 6c65 730d 0a20 2020 2020 2020 2020  ngles..         
-0000a740: 2020 2023 6178 5f72 6f73 652e 7363 6174     #ax_rose.scat
-0000a750: 7465 7228 6469 705f 617a 696d 7574 6873  ter(dip_azimuths
-0000a760: 5f72 6164 2c20 6469 705f 616e 676c 6573  _rad, dip_angles
-0000a770: 2c20 633d 636f 6c6f 722c 2061 6c70 6861  , c=color, alpha
-0000a780: 3d30 2e35 290d 0a20 2020 2020 2020 2020  =0.5)..         
-0000a790: 2020 2023 2050 6c6f 7420 7468 6520 6f72     # Plot the or
-0000a7a0: 6965 6e74 6174 696f 6e20 6461 7461 2061  ientation data a
-0000a7b0: 7320 6120 726f 7365 2064 6961 6772 616d  s a rose diagram
-0000a7c0: 0d0a 2020 2020 2020 2020 2020 2020 6e2c  ..            n,
-0000a7d0: 2062 696e 732c 2070 6174 6368 6573 3d61   bins, patches=a
-0000a7e0: 785f 726f 7365 2e68 6973 7428 7374 7269  x_rose.hist(stri
-0000a7f0: 6b65 2c20 6269 6e73 3d6e 756d 5f62 696e  ke, bins=num_bin
-0000a800: 732c 2063 6f6c 6f72 3d63 6f6c 6f72 2c20  s, color=color, 
-0000a810: 616c 7068 613d 302e 3529 0d0a 2020 2020  alpha=0.5)..    
-0000a820: 2020 2020 2020 2020 2023 2041 6e6e 6f74           # Annot
-0000a830: 6174 6520 7468 6520 6e75 6d62 6572 206f  ate the number o
-0000a840: 6620 6461 7461 2070 6f69 6e74 7320 616e  f data points an
-0000a850: 6420 6269 6e20 6e75 6d62 6572 0d0a 2020  d bin number..  
-0000a860: 2020 2020 2020 2020 2020 6178 5f72 6f73            ax_ros
-0000a870: 652e 7465 7874 2830 2c20 2d30 2e31 2c20  e.text(0, -0.1, 
-0000a880: 6622 4461 7461 2050 6f69 6e74 733a 207b  f"Data Points: {
-0000a890: 6c65 6e28 7374 7269 6b65 7329 7d22 2c20  len(strikes)}", 
-0000a8a0: 6861 3d27 6365 6e74 6572 272c 2076 613d  ha='center', va=
-0000a8b0: 2763 656e 7465 7227 2c20 7472 616e 7366  'center', transf
-0000a8c0: 6f72 6d3d 6178 5f72 6f73 652e 7472 616e  orm=ax_rose.tran
-0000a8d0: 7341 7865 7329 0d0a 2020 2020 2020 2020  sAxes)..        
-0000a8e0: 2020 2020 6178 5f72 6f73 652e 7465 7874      ax_rose.text
-0000a8f0: 2830 2c20 2d30 2e31 352c 2066 2242 696e  (0, -0.15, f"Bin
-0000a900: 2043 6f75 6e74 3a20 7b6e 756d 5f62 696e   Count: {num_bin
-0000a910: 737d 222c 2068 613d 2763 656e 7465 7227  s}", ha='center'
-0000a920: 2c20 7661 3d27 6365 6e74 6572 272c 2074  , va='center', t
-0000a930: 7261 6e73 666f 726d 3d61 785f 726f 7365  ransform=ax_rose
-0000a940: 2e74 7261 6e73 4178 6573 290d 0a0d 0a20  .transAxes).... 
-0000a950: 2020 2020 2020 2023 2023 2043 7573 746f         # # Custo
-0000a960: 6d69 7a65 2074 6865 2072 6f73 6520 6469  mize the rose di
-0000a970: 6167 7261 6d0d 0a20 2020 2020 2020 2023  agram..        #
-0000a980: 2061 785f 726f 7365 2e73 6574 5f74 6865   ax_rose.set_the
-0000a990: 7461 5f7a 6572 6f5f 6c6f 6361 7469 6f6e  ta_zero_location
-0000a9a0: 2822 4e22 290d 0a20 2020 2020 2020 2023  ("N")..        #
-0000a9b0: 2061 785f 726f 7365 2e73 6574 5f74 6865   ax_rose.set_the
-0000a9c0: 7461 5f64 6972 6563 7469 6f6e 282d 3129  ta_direction(-1)
-0000a9d0: 0d0a 2020 2020 2020 2020 2320 4375 7374  ..        # Cust
-0000a9e0: 6f6d 697a 6520 7468 6520 706f 6c61 7220  omize the polar 
-0000a9f0: 706c 6f74 0d0a 2020 2020 2020 2020 6178  plot..        ax
-0000aa00: 5f72 6f73 652e 7365 745f 7468 6574 615f  _rose.set_theta_
-0000aa10: 7a65 726f 5f6c 6f63 6174 696f 6e28 274e  zero_location('N
-0000aa20: 2729 2020 2320 5365 7420 3020 6465 6772  ')  # Set 0 degr
-0000aa30: 6565 7320 6174 2074 6865 2074 6f70 0d0a  ees at the top..
-0000aa40: 2020 2020 2020 2020 6178 5f72 6f73 652e          ax_rose.
-0000aa50: 7365 745f 7468 6574 615f 6469 7265 6374  set_theta_direct
-0000aa60: 696f 6e28 2d31 2920 2023 2052 6576 6572  ion(-1)  # Rever
-0000aa70: 7365 2074 6865 2064 6972 6563 7469 6f6e  se the direction
-0000aa80: 206f 6620 7468 6520 616e 676c 6573 0d0a   of the angles..
-0000aa90: 0d0a 2020 2020 2020 2020 2320 5365 7420  ..        # Set 
-0000aaa0: 6c61 6265 6c73 2066 6f72 2063 6172 6469  labels for cardi
-0000aab0: 6e61 6c20 6469 7265 6374 696f 6e73 0d0a  nal directions..
-0000aac0: 2020 2020 2020 2020 6178 5f72 6f73 652e          ax_rose.
-0000aad0: 7365 745f 7874 6963 6b73 286e 702e 7261  set_xticks(np.ra
-0000aae0: 6469 616e 7328 5b30 2c20 3435 2c20 3930  dians([0, 45, 90
-0000aaf0: 2c20 3133 352c 2031 3830 2c20 3232 352c  , 135, 180, 225,
-0000ab00: 2032 3730 2c20 3331 355d 2929 0d0a 2020   270, 315]))..  
-0000ab10: 2020 2020 2020 6178 5f72 6f73 652e 7365        ax_rose.se
-0000ab20: 745f 7874 6963 6b6c 6162 656c 7328 5b27  t_xticklabels(['
-0000ab30: 4e27 2c20 274e 4527 2c20 2745 272c 2027  N', 'NE', 'E', '
-0000ab40: 5345 272c 2027 5327 2c20 2753 5727 2c20  SE', 'S', 'SW', 
-0000ab50: 2757 272c 2027 4e57 275d 290d 0a20 2020  'W', 'NW'])..   
-0000ab60: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0000ab70: 2320 5365 7420 7468 6520 7261 6469 616c  # Set the radial
-0000ab80: 2067 7269 6420 616e 6420 6c61 6265 6c73   grid and labels
-0000ab90: 0d0a 2020 2020 2020 2020 2320 6178 5f72  ..        # ax_r
-0000aba0: 6f73 652e 7365 745f 726c 6162 656c 5f70  ose.set_rlabel_p
-0000abb0: 6f73 6974 696f 6e28 3930 290d 0a20 2020  osition(90)..   
-0000abc0: 2020 2020 2023 2061 785f 726f 7365 2e73       # ax_rose.s
-0000abd0: 6574 5f79 7469 636b 7328 5b31 352c 2033  et_yticks([15, 3
-0000abe0: 302c 2034 352c 2036 302c 2037 355d 290d  0, 45, 60, 75]).
-0000abf0: 0a20 2020 2020 2020 2023 2061 785f 726f  .        # ax_ro
-0000ac00: 7365 2e73 6574 5f72 6d61 7828 3930 2920  se.set_rmax(90) 
-0000ac10: 2023 2053 6574 2074 6865 206d 6178 696d   # Set the maxim
-0000ac20: 756d 2072 6164 6961 6c20 6469 7374 616e  um radial distan
-0000ac30: 6365 0d0a 2020 2020 2020 2020 6178 5f72  ce..        ax_r
-0000ac40: 6f73 652e 7365 745f 7469 746c 6528 2252  ose.set_title("R
-0000ac50: 6f73 6520 4469 6167 7261 6d20 5374 7269  ose Diagram Stri
-0000ac60: 6b65 2229 0d0a 0d0a 2020 2020 2020 2020  ke")....        
-0000ac70: 2320 4164 6a75 7374 2073 7061 6369 6e67  # Adjust spacing
-0000ac80: 2062 6574 7765 656e 2073 7562 706c 6f74   between subplot
-0000ac90: 730d 0a20 2020 2020 2020 2070 6c74 2e73  s..        plt.s
-0000aca0: 7562 706c 6f74 735f 6164 6a75 7374 2877  ubplots_adjust(w
-0000acb0: 7370 6163 653d 302e 3229 0d0a 0d0a 2020  space=0.2)....  
-0000acc0: 2020 2020 2020 706c 742e 7361 7665 6669        plt.savefi
-0000acd0: 6728 6f75 745f 706c 616e 6546 6f6c 6465  g(out_planeFolde
-0000ace0: 7220 2b20 222f 2220 2b20 2273 7465 7265  r + "/" + "stere
-0000acf0: 6f70 6c6f 742e 706e 6722 2c20 6470 693d  oplot.png", dpi=
-0000ad00: 3330 3029 0d0a 2020 2020 2020 2020 706c  300)..        pl
-0000ad10: 742e 7469 6768 745f 6c61 796f 7574 0d0a  t.tight_layout..
-0000ad20: 2020 2020 2020 2020 2370 6c74 2e63 6c6f          #plt.clo
-0000ad30: 7365 2829 0d0a 2020 2020 2020 2020 706c  se()..        pl
-0000ad40: 742e 636c 6f73 6528 290d 0a20 2020 2020  t.close()..     
-0000ad50: 2020 200d 0a20 2020 200d 0a20 2020 200d     ..    ..    .
-0000ad60: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
-0000ad70: 6566 2064 7261 775f 706c 616e 6528 7878  ef draw_plane(xx
-0000ad80: 2c79 7929 3a0d 0a20 2020 2020 2020 200d  ,yy):..        .
-0000ad90: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-0000ada0: 706f 696e 7473 2920 3e3d 2033 3a0d 0a20  points) >= 3:.. 
-0000adb0: 2020 2020 2020 2020 2020 2066 6974 7465             fitte
-0000adc0: 645f 706c 616e 652c 2061 2c20 622c 2063  d_plane, a, b, c
-0000add0: 202c 2064 6970 5f61 6e67 6c65 2c20 6469   , dip_angle, di
-0000ade0: 705f 6469 7265 6374 696f 6e20 3d20 6669  p_direction = fi
-0000adf0: 745f 706c 616e 6528 706f 696e 7473 2c20  t_plane(points, 
-0000ae00: 7878 2c20 7979 290d 0a20 2020 2020 2020  xx, yy)..       
-0000ae10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000ae20: 2020 2064 6970 5f61 6e67 6c65 5f6c 6973     dip_angle_lis
-0000ae30: 742e 6170 7065 6e64 2864 6970 5f61 6e67  t.append(dip_ang
-0000ae40: 6c65 290d 0a20 2020 2020 2020 2020 2020  le)..           
-0000ae50: 2064 6970 5f64 6972 6563 7469 6f6e 5f6c   dip_direction_l
-0000ae60: 6973 742e 6170 7065 6e64 2864 6970 5f64  ist.append(dip_d
-0000ae70: 6972 6563 7469 6f6e 290d 0a20 2020 2020  irection)..     
-0000ae80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000ae90: 2020 2020 2023 2069 6620 6c69 6d69 745f       # if limit_
-0000aea0: 6578 7465 6e64 3a0d 0a20 2020 2020 2020  extend:..       
-0000aeb0: 2020 2020 2023 2020 2347 6574 2062 6f75       #  #Get bou
-0000aec0: 6e64 696e 6720 626f 7820 6f66 2074 6865  nding box of the
-0000aed0: 2073 656c 6563 7465 6420 706f 696e 7473   selected points
-0000aee0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000aef0: 2020 2020 786d 696e 2c20 786d 6178 2c20      xmin, xmax, 
-0000af00: 796d 696e 2c20 796d 6178 203d 2062 6f75  ymin, ymax = bou
-0000af10: 6e64 696e 675f 626f 7828 706f 696e 7473  nding_box(points
-0000af20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000af30: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000af40: 2023 2020 2020 206d 6173 6b20 3d20 2878   #     mask = (x
-0000af50: 7820 3e3d 2078 6d69 6e29 2026 2028 7878  x >= xmin) & (xx
-0000af60: 203c 3d20 786d 6178 2920 2620 2879 7920   <= xmax) & (yy 
-0000af70: 3e3d 2079 6d69 6e29 2026 2028 7979 203c  >= ymin) & (yy <
-0000af80: 3d20 796d 6178 290d 0a20 2020 2020 2020  = ymax)..       
-0000af90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000afa0: 2020 2020 2020 2023 2020 2020 2066 6f72         #     for
-0000afb0: 2069 2069 6e20 7261 6e67 6528 7878 2e73   i in range(xx.s
-0000afc0: 6861 7065 5b30 5d29 3a0d 0a20 2020 2020  hape[0]):..     
-0000afd0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
-0000afe0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0000aff0: 7878 2e73 6861 7065 5b31 5d29 3a0d 0a20  xx.shape[1]):.. 
-0000b000: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-0000b010: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000b020: 6d61 736b 5b69 2c20 6a5d 3a0d 0a20 2020  mask[i, j]:..   
-0000b030: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0000b040: 2020 2020 2020 2020 2020 2066 6974 7465             fitte
-0000b050: 645f 706c 616e 655b 692c 206a 5d20 3d20  d_plane[i, j] = 
-0000b060: 6e70 2e6e 616e 2020 2320 5365 7420 6f75  np.nan  # Set ou
-0000b070: 742d 6f66 2d62 6f75 6e64 7320 7661 6c75  t-of-bounds valu
-0000b080: 6573 2074 6f20 4e61 4e0d 0a20 2020 2020  es to NaN..     
-0000b090: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000b0a0: 2070 6c61 6e65 732e 6170 7065 6e64 2866   planes.append(f
-0000b0b0: 6974 7465 645f 706c 616e 6529 0d0a 2020  itted_plane)..  
-0000b0c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000b0d0: 2020 2020 2020 2020 2370 6c61 6e65 5f63          #plane_c
-0000b0e0: 6f6c 6f72 203d 2072 616e 646f 6d5f 636f  olor = random_co
-0000b0f0: 6c6f 7228 290d 0a20 2020 2020 2020 2020  lor()..         
-0000b100: 2020 2070 6c61 6e65 5f63 6f6c 6f72 3d63     plane_color=c
-0000b110: 6f6c 6f72 5f66 726f 6d5f 6469 705f 616e  olor_from_dip_an
-0000b120: 645f 6469 7265 6374 696f 6e28 6469 705f  d_direction(dip_
-0000b130: 616e 676c 652c 2064 6970 5f64 6972 6563  angle, dip_direc
-0000b140: 7469 6f6e 290d 0a20 2020 2020 2020 2020  tion)..         
-0000b150: 2020 2070 7269 6e74 2827 706c 616e 6520     print('plane 
-0000b160: 636f 6c6f 723a 2027 2c20 706c 616e 655f  color: ', plane_
-0000b170: 636f 6c6f 7229 0d0a 2020 2020 2020 2020  color)..        
-0000b180: 2020 2020 706c 616e 655f 636f 6c6f 7273      plane_colors
-0000b190: 2e61 7070 656e 6428 706c 616e 655f 636f  .append(plane_co
-0000b1a0: 6c6f 7229 0d0a 0d0a 2020 2020 2020 2020  lor)....        
-0000b1b0: 2020 2020 666f 7220 706f 696e 7420 2069      for point  i
-0000b1c0: 6e20 706f 696e 7473 3a0d 0a20 2020 2020  n points:..     
-0000b1d0: 2020 2020 2020 2020 2020 2061 785f 3264             ax_2d
-0000b1e0: 2e70 6c6f 7428 706f 696e 745b 305d 2c20  .plot(point[0], 
-0000b1f0: 706f 696e 745b 315d 2c20 276f 272c 2063  point[1], 'o', c
-0000b200: 6f6c 6f72 3d70 6c61 6e65 5f63 6f6c 6f72  olor=plane_color
-0000b210: 202c 2061 6c70 6861 3d30 2e37 290d 0a20   , alpha=0.7).. 
-0000b220: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000b230: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000b240: 200d 0a20 2020 2020 2020 2020 2020 2063   ..            c
-0000b250: 616e 7661 735f 3264 2e64 7261 7728 290d  anvas_2d.draw().
-0000b260: 0a20 2020 2020 2020 2020 2020 200d 0a0d  .            ...
-0000b270: 0a20 2020 2020 2020 2020 2020 2023 6178  .            #ax
-0000b280: 5f33 642e 636c 6561 7228 290d 0a20 2020  _3d.clear()..   
-0000b290: 2020 2020 2020 2020 2061 785f 3364 2e73           ax_3d.s
-0000b2a0: 6574 5f74 6974 6c65 2827 3344 2044 454d  et_title('3D DEM
-0000b2b0: 2077 6974 6820 4669 7474 6564 2050 6c61   with Fitted Pla
-0000b2c0: 6e65 7327 290d 0a20 2020 2020 2020 2020  nes')..         
-0000b2d0: 2020 2061 785f 3364 2e70 6c6f 745f 7375     ax_3d.plot_su
-0000b2e0: 7266 6163 6528 7878 2c20 7979 2c20 6461  rface(xx, yy, da
-0000b2f0: 7461 2c20 636d 6170 3d27 7465 7272 6169  ta, cmap='terrai
-0000b300: 6e27 2c20 6c69 6e65 7769 6474 683d 302c  n', linewidth=0,
-0000b310: 2061 6e74 6961 6c69 6173 6564 3d54 7275   antialiased=Tru
-0000b320: 652c 2061 6c70 6861 3d30 2e35 290d 0a20  e, alpha=0.5).. 
-0000b330: 2020 2020 2020 2020 2020 2023 666f 7220             #for 
-0000b340: 706c 616e 6520 696e 2070 6c61 6e65 733a  plane in planes:
-0000b350: 0d0a 2020 2020 2020 2020 2020 2020 7375  ..            su
-0000b360: 7266 3d61 785f 3364 2e70 6c6f 745f 7375  rf=ax_3d.plot_su
-0000b370: 7266 6163 6528 7878 2c20 7979 2c20 6669  rface(xx, yy, fi
-0000b380: 7474 6564 5f70 6c61 6e65 2c20 616c 7068  tted_plane, alph
-0000b390: 613d 302e 362c 206c 696e 6577 6964 7468  a=0.6, linewidth
-0000b3a0: 3d30 2c20 616e 7469 616c 6961 7365 643d  =0, antialiased=
-0000b3b0: 5472 7565 2c20 636f 6c6f 723d 706c 616e  True, color=plan
-0000b3c0: 655f 636f 6c6f 7229 0d0a 2020 2020 2020  e_color)..      
-0000b3d0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000b3e0: 2020 2020 2020 2020 2370 6c6f 7420 706f          #plot po
-0000b3f0: 696e 7473 2069 6e20 3344 0d0a 2020 2020  ints in 3D..    
-0000b400: 2020 2020 2020 2020 666f 7220 706f 696e          for poin
-0000b410: 7420 696e 2070 6f69 6e74 733a 0d0a 2020  t in points:..  
-0000b420: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0000b430: 5f33 642e 706c 6f74 2870 6f69 6e74 5b30  _3d.plot(point[0
-0000b440: 5d2c 2070 6f69 6e74 5b31 5d2c 2027 6f27  ], point[1], 'o'
-0000b450: 2c20 636f 6c6f 723d 706c 616e 655f 636f  , color=plane_co
-0000b460: 6c6f 7229 0d0a 2020 2020 2020 2020 2020  lor)..          
-0000b470: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000b480: 2020 2020 6361 6e76 6173 5f33 642e 6472      canvas_3d.dr
-0000b490: 6177 2829 0d0a 2020 2020 2020 2020 2020  aw()..          
-0000b4a0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000b4b0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000b4c0: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
-0000b4d0: 696e 7473 5f6c 6973 7462 6f78 2e64 656c  ints_listbox.del
-0000b4e0: 6574 6528 302c 2074 6b2e 454e 4429 0d0a  ete(0, tk.END)..
-0000b4f0: 2020 2020 2020 2020 2020 2020 706f 696e              poin
-0000b500: 7473 2e63 6c65 6172 2829 0d0a 2020 2020  ts.clear()..    
-0000b510: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000b520: 2020 2020 2020 706c 6f74 5f70 6c61 6e65        plot_plane
-0000b530: 7328 6469 705f 616e 676c 655f 6c69 7374  s(dip_angle_list
-0000b540: 2c20 6469 705f 6469 7265 6374 696f 6e5f  , dip_direction_
-0000b550: 6c69 7374 2c20 706c 616e 655f 636f 6c6f  list, plane_colo
-0000b560: 7273 290d 0a20 2020 2020 2020 2020 2020  rs)..           
-0000b570: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
-0000b580: 2041 7373 756d 696e 6720 796f 7520 6861   Assuming you ha
-0000b590: 7665 2061 2027 706c 616e 6573 2720 6c69  ve a 'planes' li
-0000b5a0: 7374 2c20 796f 7520 6361 6e20 6368 6563  st, you can chec
-0000b5b0: 6b20 6974 7320 666f 726d 6174 0d0a 2020  k its format..  
-0000b5c0: 2020 2020 2020 2020 2020 2320 666f 7220            # for 
-0000b5d0: 706c 616e 6520 696e 2070 6c61 6e65 733a  plane in planes:
-0000b5e0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000b5f0: 2020 2020 7072 696e 7428 7479 7065 2870      print(type(p
-0000b600: 6c61 6e65 2929 0d0a 2020 2020 2020 2020  lane))..        
-0000b610: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
-0000b620: 6c65 6e28 706c 616e 6529 2920 2023 2054  len(plane))  # T
-0000b630: 6869 7320 7769 6c6c 2067 6976 6520 796f  his will give yo
-0000b640: 7520 7468 6520 6c65 6e67 7468 206f 7220  u the length or 
-0000b650: 6e75 6d62 6572 206f 6620 656c 656d 656e  number of elemen
-0000b660: 7473 2069 6e20 7468 6520 706c 616e 650d  ts in the plane.
-0000b670: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-0000b680: 2020 2020 2023 2049 6620 6974 2773 2061       # If it's a
-0000b690: 204e 756d 5079 2061 7272 6179 2c20 796f   NumPy array, yo
-0000b6a0: 7520 6361 6e20 7072 696e 7420 6974 7320  u can print its 
-0000b6b0: 7368 6170 6520 746f 2073 6565 2074 6865  shape to see the
-0000b6c0: 2064 696d 656e 7369 6f6e 730d 0a20 2020   dimensions..   
-0000b6d0: 2020 2020 2020 2020 2023 2020 2020 2069           #     i
-0000b6e0: 6620 6973 696e 7374 616e 6365 2870 6c61  f isinstance(pla
-0000b6f0: 6e65 2c20 6e70 2e6e 6461 7272 6179 293a  ne, np.ndarray):
-0000b700: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000b710: 2020 2020 2020 2020 7072 696e 7428 706c          print(pl
-0000b720: 616e 652e 7368 6170 6529 0d0a 2020 2020  ane.shape)..    
-0000b730: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0000b740: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0000b750: 2320 5072 696e 7420 7468 6520 6669 7273  # Print the firs
-0000b760: 7420 656c 656d 656e 7420 2861 7373 756d  t element (assum
-0000b770: 696e 6720 6974 2773 2061 206c 6973 7420  ing it's a list 
-0000b780: 6f72 204e 756d 5079 2061 7272 6179 290d  or NumPy array).
-0000b790: 0a20 2020 2020 2020 2020 2020 2023 2020  .            #  
-0000b7a0: 2020 2070 7269 6e74 2870 6c61 6e65 5b30     print(plane[0
-0000b7b0: 5d29 0d0a 0d0a 2020 2020 2020 2020 2020  ])....          
-0000b7c0: 2020 2320 2320 5072 696e 7420 7468 6520    # # Print the 
-0000b7d0: 6c65 6e67 7468 206f 6620 7468 6520 2770  length of the 'p
-0000b7e0: 6c61 6e65 7327 206c 6973 740d 0a20 2020  lanes' list..   
-0000b7f0: 2020 2020 2020 2020 2023 2070 7269 6e74           # print
-0000b800: 286c 656e 2870 6c61 6e65 7329 290d 0a20  (len(planes)).. 
-0000b810: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000b820: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000b830: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000b840: 200d 0a0d 0a20 2020 2064 6566 2062 6f75   ....    def bou
-0000b850: 6e64 696e 675f 626f 7828 706f 696e 7473  nding_box(points
-0000b860: 293a 0d0a 2020 2020 2020 2020 2222 2246  ):..        """F
-0000b870: 696e 6420 7468 6520 626f 756e 6469 6e67  ind the bounding
-0000b880: 2062 6f78 2066 6f72 2061 2073 6574 206f   box for a set o
-0000b890: 6620 706f 696e 7473 2e22 2222 0d0a 2020  f points."""..  
-0000b8a0: 2020 2020 2020 785f 7661 6c73 2c20 795f        x_vals, y_
-0000b8b0: 7661 6c73 2c20 5f20 3d20 7a69 7028 2a70  vals, _ = zip(*p
-0000b8c0: 6f69 6e74 7329 0d0a 2020 2020 2020 2020  oints)..        
-0000b8d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0000b8e0: 2020 2020 7265 7475 726e 206d 696e 2878      return min(x
-0000b8f0: 5f76 616c 7329 202c 206d 6178 2878 5f76  _vals) , max(x_v
-0000b900: 616c 7329 2c20 6d69 6e28 795f 7661 6c73  als), min(y_vals
-0000b910: 292c 206d 6178 2879 5f76 616c 7329 0d0a  ), max(y_vals)..
-0000b920: 0d0a 2020 2020 2323 2323 2323 2323 0d0a  ..    ########..
-0000b930: 0d0a 2020 200d 0a20 2020 200d 0a20 2020  ..   ..    ..   
-0000b940: 2069 6d70 6f72 7420 657a 6478 660d 0a20   import ezdxf.. 
-0000b950: 2020 2066 726f 6d20 7363 6970 792e 7370     from scipy.sp
-0000b960: 6174 6961 6c20 696d 706f 7274 2044 656c  atial import Del
-0000b970: 6175 6e61 790d 0a20 2020 2069 6d70 6f72  aunay..    impor
-0000b980: 7420 6e75 6d70 7920 6173 206e 700d 0a20  t numpy as np.. 
-0000b990: 2020 2069 6d70 6f72 7420 6f73 0d0a 0d0a     import os....
-0000b9a0: 2020 2020 6465 6620 6c69 7374 5f78 797a      def list_xyz
-0000b9b0: 5f66 696c 6573 5f69 6e5f 666f 6c64 6572  _files_in_folder
-0000b9c0: 2866 6f6c 6465 725f 7061 7468 293a 0d0a  (folder_path):..
-0000b9d0: 2020 2020 2020 2020 7879 7a5f 6669 6c65          xyz_file
-0000b9e0: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0000b9f0: 666f 7220 6669 6c65 6e61 6d65 2069 6e20  for filename in 
-0000ba00: 6f73 2e6c 6973 7464 6972 2866 6f6c 6465  os.listdir(folde
-0000ba10: 725f 7061 7468 293a 0d0a 2020 2020 2020  r_path):..      
-0000ba20: 2020 2020 2020 6966 2066 696c 656e 616d        if filenam
-0000ba30: 652e 656e 6473 7769 7468 2822 2e78 797a  e.endswith(".xyz
-0000ba40: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-0000ba50: 2020 2020 2078 797a 5f66 696c 6573 2e61       xyz_files.a
-0000ba60: 7070 656e 6428 6f73 2e70 6174 682e 6a6f  ppend(os.path.jo
-0000ba70: 696e 2866 6f6c 6465 725f 7061 7468 2c20  in(folder_path, 
-0000ba80: 6669 6c65 6e61 6d65 2929 0d0a 2020 2020  filename))..    
-0000ba90: 2020 2020 7265 7475 726e 2078 797a 5f66      return xyz_f
-0000baa0: 696c 6573 0d0a 0d0a 2020 2020 6465 6620  iles....    def 
-0000bab0: 6372 6561 7465 5f64 7866 5f66 726f 6d5f  create_dxf_from_
-0000bac0: 7879 7a5f 6669 6c65 7328 7879 7a5f 6669  xyz_files(xyz_fi
-0000bad0: 6c65 732c 206f 7574 7075 745f 7061 7468  les, output_path
-0000bae0: 2c20 7369 6e67 6c65 3d4e 6f6e 6529 3a0d  , single=None):.
-0000baf0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000bb00: 2020 2069 6620 7369 6e67 6c65 2069 7320     if single is 
-0000bb10: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-0000bb20: 2020 2020 2320 4372 6561 7465 2061 206e      # Create a n
-0000bb30: 6577 2044 5846 2064 6f63 756d 656e 740d  ew DXF document.
-0000bb40: 0a20 2020 2020 2020 2020 2020 2064 6f63  .            doc
-0000bb50: 203d 2065 7a64 7866 2e6e 6577 2829 0d0a   = ezdxf.new()..
-0000bb60: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000bb70: 4372 6561 7465 2061 206e 6577 2044 5846  Create a new DXF
-0000bb80: 206d 6f64 656c 2073 7061 6365 0d0a 2020   model space..  
-0000bb90: 2020 2020 2020 2020 2020 6d73 7020 3d20            msp = 
-0000bba0: 646f 632e 6d6f 6465 6c73 7061 6365 2829  doc.modelspace()
-0000bbb0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000bbc0: 2020 2020 2020 2020 2020 200d 0a0d 0a20             .... 
-0000bbd0: 2020 2020 2020 2066 6f72 2078 797a 5f66         for xyz_f
-0000bbe0: 696c 6520 696e 2078 797a 5f66 696c 6573  ile in xyz_files
-0000bbf0: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-0000bc00: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000bc10: 7369 6e67 6c65 2069 7320 6e6f 7420 4e6f  single is not No
-0000bc20: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-0000bc30: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
-0000bc40: 6e65 7720 4458 4620 646f 6375 6d65 6e74  new DXF document
-0000bc50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bc60: 2020 646f 6320 3d20 657a 6478 662e 6e65    doc = ezdxf.ne
-0000bc70: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-0000bc80: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0000bc90: 6120 6e65 7720 4458 4620 6d6f 6465 6c20  a new DXF model 
-0000bca0: 7370 6163 650d 0a20 2020 2020 2020 2020  space..         
-0000bcb0: 2020 2020 2020 206d 7370 203d 2064 6f63         msp = doc
-0000bcc0: 2e6d 6f64 656c 7370 6163 6528 290d 0a20  .modelspace().. 
-0000bcd0: 2020 2020 2020 2020 2020 2023 204c 6f61             # Loa
-0000bce0: 6420 5859 5a20 6461 7461 2066 726f 6d20  d XYZ data from 
-0000bcf0: 6120 6669 6c65 0d0a 2020 2020 2020 2020  a file..        
-0000bd00: 2020 2020 6461 7461 203d 206e 702e 6c6f      data = np.lo
-0000bd10: 6164 7478 7428 7879 7a5f 6669 6c65 290d  adtxt(xyz_file).
-0000bd20: 0a20 2020 2020 2020 2020 2020 200d 0a0d  .            ...
-0000bd30: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-0000bd40: 6570 6172 6174 6520 7468 6520 5859 5a20  eparate the XYZ 
-0000bd50: 6461 7461 2069 6e74 6f20 696e 6469 7669  data into indivi
-0000bd60: 6475 616c 2061 7272 6179 730d 0a20 2020  dual arrays..   
-0000bd70: 2020 2020 2020 2020 2078 203d 2064 6174           x = dat
-0000bd80: 615b 3a2c 2030 5d0d 0a20 2020 2020 2020  a[:, 0]..       
-0000bd90: 2020 2020 2079 203d 2064 6174 615b 3a2c       y = data[:,
-0000bda0: 2031 5d0d 0a20 2020 2020 2020 2020 2020   1]..           
-0000bdb0: 207a 203d 2064 6174 615b 3a2c 2032 5d0d   z = data[:, 2].
-0000bdc0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
-0000bdd0: 2043 7265 6174 6520 6120 4465 6c61 756e   Create a Delaun
-0000bde0: 6179 2074 7269 616e 6775 6c61 7469 6f6e  ay triangulation
-0000bdf0: 206f 6620 7468 6520 706f 696e 7473 0d0a   of the points..
-0000be00: 2020 2020 2020 2020 2020 2020 7472 6920              tri 
-0000be10: 3d20 4465 6c61 756e 6179 286e 702e 636f  = Delaunay(np.co
-0000be20: 6c75 6d6e 5f73 7461 636b 2828 782c 2079  lumn_stack((x, y
-0000be30: 2929 290d 0a0d 0a20 2020 2020 2020 2020  )))....         
-0000be40: 2020 2023 2041 6464 2074 6865 2074 7269     # Add the tri
-0000be50: 616e 676c 6573 2074 6f20 7468 6520 6d6f  angles to the mo
-0000be60: 6465 6c20 7370 6163 650d 0a20 2020 2020  del space..     
-0000be70: 2020 2020 2020 2066 6f72 2073 696d 706c         for simpl
-0000be80: 6578 2069 6e20 7472 692e 7369 6d70 6c69  ex in tri.simpli
-0000be90: 6365 733a 0d0a 2020 2020 2020 2020 2020  ces:..          
-0000bea0: 2020 2020 2020 7665 7274 6963 6573 203d        vertices =
-0000beb0: 205b 2878 5b69 5d2c 2079 5b69 5d2c 207a   [(x[i], y[i], z
-0000bec0: 5b69 5d29 2066 6f72 2069 2069 6e20 7369  [i]) for i in si
-0000bed0: 6d70 6c65 785d 0d0a 2020 2020 2020 2020  mplex]..        
-0000bee0: 2020 2020 2020 2020 6d73 702e 6164 645f          msp.add_
-0000bef0: 3364 6661 6365 2870 6f69 6e74 733d 7665  3dface(points=ve
-0000bf00: 7274 6963 6573 290d 0a20 2020 2020 2020  rtices)..       
-0000bf10: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000bf20: 2020 2069 6620 7369 6e67 6c65 2069 7320     if single is 
-0000bf30: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
-0000bf40: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000bf50: 2053 6176 6520 7468 6520 4458 4620 6669   Save the DXF fi
-0000bf60: 6c65 0d0a 2020 2020 2020 2020 2020 2020  le..            
-0000bf70: 2020 2020 646f 632e 7361 7665 6173 286f      doc.saveas(o
-0000bf80: 7574 7075 745f 7061 7468 290d 0a20 2020  utput_path)..   
-0000bf90: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000bfa0: 2020 2069 6620 7369 6e67 6c65 2069 7320     if single is 
-0000bfb0: 4e6f 6e65 3a20 0d0a 0d0a 2020 2020 2020  None: ....      
-0000bfc0: 2020 2020 2020 2320 5361 7665 2074 6865        # Save the
-0000bfd0: 2044 5846 2066 696c 650d 0a20 2020 2020   DXF file..     
-0000bfe0: 2020 2020 2020 2064 6f63 2e73 6176 6561         doc.savea
-0000bff0: 7328 6f75 7470 7574 5f70 6174 6829 0d0a  s(output_path)..
-0000c000: 2020 2020 2020 2020 0d0a 2020 2020 0d0a          ..    ..
-0000c010: 2020 2020 6465 6620 7361 7665 5f70 6c61      def save_pla
-0000c020: 6e65 735f 746f 5f6f 626a 2829 3a0d 0a20  nes_to_obj():.. 
-0000c030: 2020 2020 2020 2078 5f63 6f6f 7264 7320         x_coords 
-0000c040: 3d20 6e70 2e6c 696e 7370 6163 6528 6c65  = np.linspace(le
-0000c050: 6674 2c20 7269 6768 742c 2064 6174 612e  ft, right, data.
-0000c060: 7368 6170 655b 315d 290d 0a20 2020 2020  shape[1])..     
-0000c070: 2020 2079 5f63 6f6f 7264 7320 3d20 6e70     y_coords = np
-0000c080: 2e6c 696e 7370 6163 6528 746f 702c 2062  .linspace(top, b
-0000c090: 6f74 746f 6d2c 2064 6174 612e 7368 6170  ottom, data.shap
-0000c0a0: 655b 305d 290d 0a20 2020 2020 2020 2078  e[0])..        x
-0000c0b0: 782c 2079 7920 3d20 6e70 2e6d 6573 6867  x, yy = np.meshg
-0000c0c0: 7269 6428 785f 636f 6f72 6473 2c20 795f  rid(x_coords, y_
-0000c0d0: 636f 6f72 6473 290d 0a20 2020 2020 2020  coords)..       
-0000c0e0: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0000c0f0: 2070 6c61 6e65 733a 0d0a 2020 2020 2020   planes:..      
-0000c100: 2020 2020 2020 7072 696e 7428 224e 6f20        print("No 
-0000c110: 706c 616e 6573 2074 6f20 7361 7665 2e22  planes to save."
-0000c120: 290d 0a20 2020 2020 2020 2020 2020 2072  )..            r
-0000c130: 6574 7572 6e0d 0a20 2020 2020 2020 200d  eturn..        .
-0000c140: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000c150: 2020 206f 7574 7075 745f 6669 6c65 6e61     output_filena
-0000c160: 6d65 5f64 7866 203d 2066 227b 6f75 745f  me_dxf = f"{out_
-0000c170: 706c 616e 6546 6f6c 6465 727d 2f70 6c61  planeFolder}/pla
-0000c180: 6e65 732e 6478 6622 0d0a 2020 2020 2020  nes.dxf"..      
-0000c190: 2020 666f 7220 6964 782c 2070 6c61 6e65    for idx, plane
-0000c1a0: 2069 6e20 656e 756d 6572 6174 6528 706c   in enumerate(pl
-0000c1b0: 616e 6573 293a 0d0a 2020 2020 2020 2020  anes):..        
-0000c1c0: 2020 2020 6f75 7470 7574 5f66 696c 656e      output_filen
-0000c1d0: 616d 6520 3d20 6622 7b6f 7574 5f70 6c61  ame = f"{out_pla
-0000c1e0: 6e65 466f 6c64 6572 7d2f 706c 616e 6573  neFolder}/planes
-0000c1f0: 5f7b 6964 787d 2e78 797a 220d 0a20 2020  _{idx}.xyz"..   
-0000c200: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000c210: 6669 6c65 6e61 6d65 5f69 6478 203d 2066  filename_idx = f
-0000c220: 227b 6f75 745f 706c 616e 6546 6f6c 6465  "{out_planeFolde
-0000c230: 727d 2f70 6c61 6e65 735f 7b69 6478 7d2e  r}/planes_{idx}.
-0000c240: 6478 6622 0d0a 2020 2020 2020 2020 2020  dxf"..          
-0000c250: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000c260: 2320 496e 6974 6961 6c69 7a65 206c 6973  # Initialize lis
-0000c270: 7473 2074 6f20 7374 6f72 6520 7665 7274  ts to store vert
-0000c280: 6963 6573 2061 6e64 2066 6163 6573 0d0a  ices and faces..
-0000c290: 2020 2020 2020 2020 2020 2020 7665 7274              vert
-0000c2a0: 6963 6573 203d 205b 5d0d 0a20 2020 2020  ices = []..     
-0000c2b0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000c2c0: 2020 2020 2023 2053 616d 706c 6564 2070       # Sampled p
-0000c2d0: 6f69 6e74 2069 6e74 6572 7661 6c0d 0a20  oint interval.. 
-0000c2e0: 2020 2020 2020 2020 2020 2073 616d 706c             sampl
-0000c2f0: 655f 696e 7465 7276 616c 203d 2032 3030  e_interval = 200
-0000c300: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000c310: 2020 2020 2020 2020 2020 2020 2320 4f70              # Op
-0000c320: 656e 2074 6865 2058 595a 2066 696c 6520  en the XYZ file 
-0000c330: 666f 7220 7772 6974 696e 670d 0a20 2020  for writing..   
-0000c340: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0000c350: 656e 286f 7574 7075 745f 6669 6c65 6e61  en(output_filena
-0000c360: 6d65 2c20 2777 2729 2061 7320 7879 7a5f  me, 'w') as xyz_
-0000c370: 6669 6c65 3a0d 0a20 2020 2020 2020 2020  file:..         
-0000c380: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0000c390: 7261 6e67 6528 302c 2070 6c61 6e65 2e73  range(0, plane.s
-0000c3a0: 6861 7065 5b30 5d2c 2073 616d 706c 655f  hape[0], sample_
-0000c3b0: 696e 7465 7276 616c 293a 0d0a 2020 2020  interval):..    
-0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3d0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-0000c3e0: 2c20 706c 616e 652e 7368 6170 655b 315d  , plane.shape[1]
-0000c3f0: 2c20 7361 6d70 6c65 5f69 6e74 6572 7661  , sample_interva
-0000c400: 6c29 3a0d 0a20 2020 2020 2020 2020 2020  l):..           
-0000c410: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000c420: 6920 3c20 7878 2e73 6861 7065 5b30 5d20  i < xx.shape[0] 
-0000c430: 616e 6420 6a20 3c20 7878 2e73 6861 7065  and j < xx.shape
-0000c440: 5b31 5d3a 0d0a 2020 2020 2020 2020 2020  [1]:..          
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 7820 3d20 7878 5b69 2c20 6a5d 0d0a    x = xx[i, j]..
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
-0000c490: 7979 5b69 2c20 6a5d 0d0a 2020 2020 2020  yy[i, j]..      
-0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 2020 2020 7a20 3d20 706c 616e 655b        z = plane[
-0000c4c0: 692c 206a 5d0d 0a0d 0a20 2020 2020 2020  i, j]....       
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4e0: 2020 2020 2023 2043 6865 636b 2066 6f72       # Check for
-0000c4f0: 204e 614e 2076 616c 7565 730d 0a20 2020   NaN values..   
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000c520: 6e70 2e69 736e 616e 2878 2920 616e 6420  np.isnan(x) and 
-0000c530: 6e6f 7420 6e70 2e69 736e 616e 2879 2920  not np.isnan(y) 
-0000c540: 616e 6420 6e6f 7420 6e70 2e69 736e 616e  and not np.isnan
-0000c550: 287a 293a 0d0a 2020 2020 2020 2020 2020  (z):..          
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2020 2020 2020 2320 4164 6420 7468 6520        # Add the 
-0000c580: 7665 7274 6578 2074 6f20 7468 6520 6c69  vertex to the li
-0000c590: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 2020 7665 7274 6963 6573 2e61 7070      vertices.app
-0000c5c0: 656e 6428 2878 2c20 792c 207a 2929 0d0a  end((x, y, z))..
-0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000c5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c610: 2023 2057 7269 7465 2076 6572 7465 7820   # Write vertex 
-0000c620: 6461 7461 2074 6f20 7468 6520 5859 5a20  data to the XYZ 
-0000c630: 6669 6c65 0d0a 2020 2020 2020 2020 2020  file..          
-0000c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c650: 2020 2020 2020 7879 7a5f 6669 6c65 2e77        xyz_file.w
-0000c660: 7269 7465 2866 277b 787d 207b 797d 207b  rite(f'{x} {y} {
-0000c670: 7a7d 5c6e 2729 0d0a 2020 2020 2020 2020  z}\n')..        
-0000c680: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0000c690: 2020 6372 6561 7465 5f64 7866 5f66 726f    create_dxf_fro
-0000c6a0: 6d5f 7879 7a5f 6669 6c65 7328 6c69 7374  m_xyz_files(list
-0000c6b0: 5f78 797a 5f66 696c 6573 5f69 6e5f 666f  _xyz_files_in_fo
-0000c6c0: 6c64 6572 286f 7574 5f70 6c61 6e65 466f  lder(out_planeFo
-0000c6d0: 6c64 6572 292c 206f 7574 7075 745f 6669  lder), output_fi
-0000c6e0: 6c65 6e61 6d65 5f69 6478 2c20 7369 6e67  lename_idx, sing
-0000c6f0: 6c65 3d69 6478 290d 0a20 2020 2020 2020  le=idx)..       
-0000c700: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c710: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0000c720: 2020 2070 7269 6e74 2866 277a 7a20 7661     print(f'zz va
-0000c730: 6c75 6573 2073 6176 6564 2074 6f20 7b6f  lues saved to {o
-0000c740: 7574 7075 745f 6669 6c65 6e61 6d65 7d27  utput_filename}'
-0000c750: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
-0000c760: 0a20 2020 2020 2020 200d 0a20 2020 0d0a  .        ..   ..
-0000c770: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0000c780: 2020 0d0a 2020 2020 6465 6620 636f 6c6c    ..    def coll
-0000c790: 6563 745f 706f 696e 7473 5f66 726f 6d5f  ect_points_from_
-0000c7a0: 6c69 6e65 2867 6466 293a 0d0a 2020 2020  line(gdf):..    
-0000c7b0: 2020 2020 2222 2243 6f6c 6c65 6374 2073      """Collect s
-0000c7c0: 7461 7274 2c20 6d69 6464 6c65 2c20 616e  tart, middle, an
-0000c7d0: 6420 656e 6420 706f 696e 7473 2066 726f  d end points fro
-0000c7e0: 6d20 6561 6368 206c 696e 6520 6665 6174  m each line feat
-0000c7f0: 7572 652e 2222 220d 0a20 2020 2020 2020  ure."""..       
-0000c800: 2063 6f6c 6c65 6374 6564 5f70 6f69 6e74   collected_point
-0000c810: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
-0000c820: 2020 666f 7220 6765 6f6d 6574 7279 2069    for geometry i
-0000c830: 6e20 6764 662e 6765 6f6d 6574 7279 3a0d  n gdf.geometry:.
-0000c840: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c850: 6765 6f6d 6574 7279 2e67 656f 6d5f 7479  geometry.geom_ty
-0000c860: 7065 203d 3d20 224c 696e 6553 7472 696e  pe == "LineStrin
-0000c870: 6722 3a0d 0a20 2020 2020 2020 2020 2020  g":..           
-0000c880: 2020 2020 2078 2c20 7920 3d20 6765 6f6d       x, y = geom
-0000c890: 6574 7279 2e78 790d 0a20 2020 2020 2020  etry.xy..       
-0000c8a0: 2020 2020 2020 2020 2073 7461 7274 203d           start =
-0000c8b0: 2028 785b 305d 2c20 795b 305d 290d 0a20   (x[0], y[0]).. 
-0000c8c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c8d0: 6e64 203d 2028 785b 2d31 5d2c 2079 5b2d  nd = (x[-1], y[-
-0000c8e0: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
-0000c8f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000c900: 2020 2020 2020 2023 7072 696e 7428 2773         #print('s
-0000c910: 7461 7274 3a20 2720 2c73 7461 7274 290d  tart: ' ,start).
-0000c920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c930: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000c940: 2020 2023 2023 2043 7265 6174 6520 6120     # # Create a 
-0000c950: 4c69 6e65 5374 7269 6e67 2066 726f 6d20  LineString from 
-0000c960: 636f 6f72 6469 6e61 7465 7320 746f 2065  coordinates to e
-0000c970: 6173 696c 7920 6765 7420 6120 706f 696e  asily get a poin
-0000c980: 7420 6174 2035 3025 2064 6973 7461 6e63  t at 50% distanc
-0000c990: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
-0000c9a0: 2020 206c 696e 6520 3d20 4c69 6e65 5374     line = LineSt
-0000c9b0: 7269 6e67 287a 6970 2878 2c20 7929 290d  ring(zip(x, y)).
-0000c9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c9d0: 2023 2069 6620 6c65 6e28 6c69 6e65 2e63   # if len(line.c
-0000c9e0: 6f6f 7264 7329 203e 3d20 333a 0d0a 2020  oords) >= 3:..  
-0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ca00: 2020 2020 2320 4966 2074 6865 206c 696e      # If the lin
-0000ca10: 6520 6861 7320 6d6f 7265 2074 6861 6e20  e has more than 
-0000ca20: 3220 7665 7274 6963 6573 2c20 636f 6c6c  2 vertices, coll
-0000ca30: 6563 7420 706f 696e 7473 2061 7420 7665  ect points at ve
-0000ca40: 7274 6963 6573 0d0a 2020 2020 2020 2020  rtices..        
-0000ca50: 2020 2020 2020 2020 2320 2020 2020 7665          #     ve
-0000ca60: 7274 6963 6573 203d 206c 6973 7428 6c69  rtices = list(li
-0000ca70: 6e65 2e63 6f6f 7264 7329 0d0a 2020 2020  ne.coords)..    
-0000ca80: 2020 2020 2020 2020 2020 2020 2320 2020              #   
-0000ca90: 2020 2370 7269 6e74 2827 7665 7274 6963    #print('vertic
-0000caa0: 733a 2027 2c20 7665 7274 6963 6573 290d  s: ', vertices).
-0000cab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cac0: 2023 2020 2020 2076 6572 7465 785f 6c69   #     vertex_li
-0000cad0: 7374 3d5b 6920 666f 7220 6920 696e 2076  st=[i for i in v
-0000cae0: 6572 7469 6365 735d 0d0a 2020 2020 2020  ertices]..      
-0000caf0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-0000cb00: 666f 7220 6b6a 2069 6e20 7665 7274 6578  for kj in vertex
-0000cb10: 5f6c 6973 743a 0d0a 2020 2020 2020 2020  _list:..        
-0000cb20: 2020 2020 2020 2020 2320 2020 2020 2020          #       
-0000cb30: 2020 636f 6c6c 6563 7465 645f 706f 696e    collected_poin
-0000cb40: 7473 2e61 7070 656e 6428 6b6a 290d 0a20  ts.append(kj).. 
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000cb60: 2020 2020 2023 636f 6c6c 6563 7465 645f       #collected_
-0000cb70: 706f 696e 7473 2e65 7874 656e 6428 7665  points.extend(ve
-0000cb80: 7274 6963 6573 290d 0a20 2020 2020 2020  rtices)..       
-0000cb90: 2020 2020 2020 2020 2023 2065 6c73 653a           # else:
-0000cba0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000cbb0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000cbc0: 2020 2020 2020 2020 6d69 6464 6c65 203d          middle =
-0000cbd0: 206c 696e 652e 696e 7465 7270 6f6c 6174   line.interpolat
-0000cbe0: 6528 302e 352c 206e 6f72 6d61 6c69 7a65  e(0.5, normalize
-0000cbf0: 643d 5472 7565 292e 636f 6f72 6473 5b30  d=True).coords[0
-0000cc00: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0000cc10: 2020 2070 3220 3d20 6c69 6e65 2e69 6e74     p2 = line.int
-0000cc20: 6572 706f 6c61 7465 2830 2e32 352c 206e  erpolate(0.25, n
-0000cc30: 6f72 6d61 6c69 7a65 643d 5472 7565 292e  ormalized=True).
-0000cc40: 636f 6f72 6473 5b30 5d0d 0a20 2020 2020  coords[0]..     
-0000cc50: 2020 2020 2020 2020 2020 2070 3120 3d20             p1 = 
-0000cc60: 6c69 6e65 2e69 6e74 6572 706f 6c61 7465  line.interpolate
-0000cc70: 2830 2e37 352c 206e 6f72 6d61 6c69 7a65  (0.75, normalize
-0000cc80: 643d 5472 7565 292e 636f 6f72 6473 5b30  d=True).coords[0
-0000cc90: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
-0000cca0: 2020 2020 2063 6f6c 6c65 6374 6564 5f70       collected_p
-0000ccb0: 6f69 6e74 732e 6170 7065 6e64 285b 7374  oints.append([st
-0000ccc0: 6172 742c 206d 6964 646c 652c 2065 6e64  art, middle, end
-0000ccd0: 2c20 7031 2c70 325d 290d 0a0d 0a20 2020  , p1,p2])....   
-0000cce0: 2020 2020 2072 6574 7572 6e20 636f 6c6c       return coll
-0000ccf0: 6563 7465 645f 706f 696e 7473 0d0a 0d0a  ected_points....
-0000cd00: 2020 2020 2320 6465 6620 636f 6c6c 6563      # def collec
-0000cd10: 745f 706f 696e 7473 5f66 726f 6d5f 6c69  t_points_from_li
-0000cd20: 6e65 2867 6466 293a 0d0a 2020 2020 2320  ne(gdf):..    # 
-0000cd30: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
-0000cd40: 2061 6e20 656d 7074 7920 6c69 7374 2074   an empty list t
-0000cd50: 6f20 7374 6f72 6520 7468 6520 636f 6f72  o store the coor
-0000cd60: 6469 6e61 7465 730d 0a20 2020 2023 2020  dinates..    #  
-0000cd70: 2020 2063 6f6c 6c65 6374 6564 5f70 6f69     collected_poi
-0000cd80: 6e74 7320 3d20 5b5d 0d0a 0d0a 2020 2020  nts = []....    
-0000cd90: 2320 2020 2020 2320 4974 6572 6174 6520  #     # Iterate 
-0000cda0: 7468 726f 7567 6820 7468 6520 4765 6f44  through the GeoD
-0000cdb0: 6174 6146 7261 6d65 0d0a 2020 2020 2320  ataFrame..    # 
-0000cdc0: 2020 2020 666f 7220 6765 6f6d 6574 7279      for geometry
-0000cdd0: 2069 6e20 6764 665b 2767 656f 6d65 7472   in gdf['geometr
-0000cde0: 7927 5d3a 0d0a 2020 2020 2320 2020 2020  y']:..    #     
-0000cdf0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-0000ce00: 6528 6765 6f6d 6574 7279 2c20 4c69 6e65  e(geometry, Line
-0000ce10: 5374 7269 6e67 293a 0d0a 2020 2020 2320  String):..    # 
-0000ce20: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
-0000ce30: 756e 7420 7468 6520 6e75 6d62 6572 206f  unt the number o
-0000ce40: 6620 7665 7274 6963 6573 2069 6e20 7468  f vertices in th
-0000ce50: 6520 4c69 6e65 5374 7269 6e67 0d0a 2020  e LineString..  
-0000ce60: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0000ce70: 6e75 6d5f 7665 7274 6963 6573 203d 206c  num_vertices = l
-0000ce80: 656e 2867 656f 6d65 7472 792e 636f 6f72  en(geometry.coor
-0000ce90: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
-0000cea0: 2020 2020 200d 0a20 2020 2023 2020 2020       ..    #    
-0000ceb0: 2020 2020 2020 2020 2023 2043 6865 636b           # Check
-0000cec0: 2069 6620 7468 6520 4c69 6e65 5374 7269   if the LineStri
-0000ced0: 6e67 2069 7320 7374 7261 6967 6874 2028  ng is straight (
-0000cee0: 3320 6f72 2066 6577 6572 2076 6572 7469  3 or fewer verti
-0000cef0: 6365 7329 0d0a 2020 2020 2320 2020 2020  ces)..    #     
-0000cf00: 2020 2020 2020 2020 6966 206e 756d 5f76          if num_v
-0000cf10: 6572 7469 6365 7320 3c3d 2033 3a0d 0a20  ertices <= 3:.. 
-0000cf20: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0000cf30: 2020 2020 2023 2046 6f72 2073 7472 6169       # For strai
-0000cf40: 6768 7420 6c69 6e65 732c 2074 616b 6520  ght lines, take 
-0000cf50: 636f 6f72 6469 6e61 7465 7320 6f66 2073  coordinates of s
-0000cf60: 7461 7274 2c20 656e 642c 2061 6e64 206d  tart, end, and m
-0000cf70: 6964 646c 650d 0a20 2020 2023 2020 2020  iddle..    #    
-0000cf80: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000cf90: 7274 5f70 6f69 6e74 203d 2067 656f 6d65  rt_point = geome
-0000cfa0: 7472 792e 636f 6f72 6473 5b30 5d0d 0a20  try.coords[0].. 
-0000cfb0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0000cfc0: 2020 2020 2065 6e64 5f70 6f69 6e74 203d       end_point =
-0000cfd0: 2067 656f 6d65 7472 792e 636f 6f72 6473   geometry.coords
-0000cfe0: 5b2d 315d 0d0a 2020 2020 2320 2020 2020  [-1]..    #     
-0000cff0: 2020 2020 2020 2020 2020 2020 6d69 6464              midd
-0000d000: 6c65 5f70 6f69 6e74 203d 2067 656f 6d65  le_point = geome
-0000d010: 7472 792e 696e 7465 7270 6f6c 6174 6528  try.interpolate(
-0000d020: 302e 352c 206e 6f72 6d61 6c69 7a65 643d  0.5, normalized=
-0000d030: 5472 7565 292e 636f 6f72 6473 5b30 5d0d  True).coords[0].
-0000d040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d050: 2020 2020 200d 0a20 2020 2023 2020 2020       ..    #    
-0000d060: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0000d070: 6c65 6374 6564 5f70 6f69 6e74 732e 6578  lected_points.ex
-0000d080: 7465 6e64 285b 7374 6172 745f 706f 696e  tend([start_poin
-0000d090: 742c 206d 6964 646c 655f 706f 696e 742c  t, middle_point,
-0000d0a0: 2065 6e64 5f70 6f69 6e74 5d29 0d0a 2020   end_point])..  
-0000d0b0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
-0000d0c0: 656c 7365 3a0d 0a20 2020 2023 2020 2020  else:..    #    
-0000d0d0: 2020 2020 2020 2020 2020 2020 2023 2046               # F
-0000d0e0: 6f72 2063 7572 7665 6420 6c69 6e65 732c  or curved lines,
-0000d0f0: 2074 616b 6520 636f 6f72 6469 6e61 7465   take coordinate
-0000d100: 7320 6f66 2061 6c6c 2076 6572 7469 6365  s of all vertice
-0000d110: 730d 0a20 2020 2023 2020 2020 2020 2020  s..    #        
-0000d120: 2020 2020 2020 2020 2066 6f72 2070 6f69           for poi
-0000d130: 6e74 2069 6e20 6765 6f6d 6574 7279 2e63  nt in geometry.c
-0000d140: 6f6f 7264 733a 0d0a 2020 2020 2320 2020  oords:..    #   
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 2020 782c 2079 203d 2070 6f69 6e74 0d0a    x, y = point..
-0000d170: 2020 2020 2320 2020 2020 2020 2020 2020      #           
-0000d180: 2020 2020 2020 2020 2020 636f 6c6c 6563            collec
-0000d190: 7465 645f 706f 696e 7473 2e61 7070 656e  ted_points.appen
-0000d1a0: 6428 2878 2c20 7929 290d 0a20 2020 2020  d((x, y))..     
-0000d1b0: 2020 200d 0a20 2020 2023 2020 2020 2072     ..    #     r
-0000d1c0: 6574 7572 6e20 636f 6c6c 6563 7465 645f  eturn collected_
-0000d1d0: 706f 696e 7473 0d0a 0d0a 2320 4e6f 772c  points....# Now,
-0000d1e0: 2063 6f6f 7264 696e 6174 6573 5f6c 6973   coordinates_lis
-0000d1f0: 7420 636f 6e74 6169 6e73 2074 6865 2063  t contains the c
-0000d200: 6f6f 7264 696e 6174 6573 206f 6620 7374  oordinates of st
-0000d210: 6172 742c 2065 6e64 2c20 6d69 6464 6c65  art, end, middle
-0000d220: 2c20 616e 6420 616c 6c20 7665 7274 6963  , and all vertic
-0000d230: 6573 0d0a 2320 6261 7365 6420 6f6e 2077  es..# based on w
-0000d240: 6865 7468 6572 2074 6865 206c 696e 6520  hether the line 
-0000d250: 6973 2073 7472 6169 6768 7420 2833 206f  is straight (3 o
-0000d260: 7220 6665 7765 7220 7665 7274 6963 6573  r fewer vertices
-0000d270: 2920 6f72 2063 7572 7665 640d 0a20 2020  ) or curved..   
-0000d280: 2020 2020 200d 0a20 2020 200d 0a0d 0a20       ..    .... 
-0000d290: 2020 2064 6566 2064 7261 775f 706c 616e     def draw_plan
-0000d2a0: 6573 5f66 726f 6d5f 6c69 6e65 7328 7878  es_from_lines(xx
-0000d2b0: 2c79 7929 3a0d 0a20 2020 2020 2020 2067  ,yy):..        g
-0000d2c0: 6c6f 6261 6c20 6178 5f32 642c 2061 785f  lobal ax_2d, ax_
-0000d2d0: 3364 2c20 6461 7461 2c20 7472 616e 7366  3d, data, transf
-0000d2e0: 6f72 6d2c 206c 6566 742c 2072 6967 6874  orm, left, right
-0000d2f0: 2c20 626f 7474 6f6d 2c20 746f 702c 2070  , bottom, top, p
-0000d300: 6c61 6e65 7320 0d0a 2020 2020 2020 2020  lanes ..        
-0000d310: 0d0a 2020 2020 2020 2020 6461 7461 2c20  ..        data, 
-0000d320: 7472 616e 7366 6f72 6d2c 2070 726f 6a65  transform, proje
-0000d330: 6374 696f 6e20 3d20 7265 6164 5f64 656d  ction = read_dem
-0000d340: 2864 656d 5f64 6174 6129 0d0a 0d0a 2020  (dem_data)....  
-0000d350: 2020 2020 2020 6764 6620 3d20 6770 642e        gdf = gpd.
-0000d360: 7265 6164 5f66 696c 6528 6c69 6e65 5f73  read_file(line_s
-0000d370: 6861 7065 6669 6c65 290d 0a20 2020 2020  hapefile)..     
-0000d380: 2020 2069 6620 6764 662e 6372 732e 746f     if gdf.crs.to
-0000d390: 5f73 7472 696e 6728 2920 213d 2070 726f  _string() != pro
-0000d3a0: 6a65 6374 696f 6e3a 0d0a 2020 2020 2020  jection:..      
-0000d3b0: 2020 2020 2020 6764 6620 3d20 6764 662e        gdf = gdf.
-0000d3c0: 746f 5f63 7273 2870 726f 6a65 6374 696f  to_crs(projectio
-0000d3d0: 6e29 0d0a 0d0a 2020 2020 2020 2020 706f  n)....        po
-0000d3e0: 696e 745f 7365 7473 203d 2063 6f6c 6c65  int_sets = colle
-0000d3f0: 6374 5f70 6f69 6e74 735f 6672 6f6d 5f6c  ct_points_from_l
-0000d400: 696e 6528 6764 6629 0d0a 2020 2020 2020  ine(gdf)..      
-0000d410: 2020 2320 785f 636f 6f72 6473 203d 206e    # x_coords = n
-0000d420: 702e 6c69 6e73 7061 6365 286c 6566 742c  p.linspace(left,
-0000d430: 2072 6967 6874 2c20 6461 7461 2e73 6861   right, data.sha
-0000d440: 7065 5b31 5d29 0d0a 2020 2020 2020 2020  pe[1])..        
-0000d450: 2320 795f 636f 6f72 6473 203d 206e 702e  # y_coords = np.
-0000d460: 6c69 6e73 7061 6365 2874 6f70 2c20 626f  linspace(top, bo
-0000d470: 7474 6f6d 2c20 6461 7461 2e73 6861 7065  ttom, data.shape
-0000d480: 5b30 5d29 0d0a 2020 2020 2020 2020 2320  [0])..        # 
-0000d490: 7878 2c20 7979 203d 206e 702e 6d65 7368  xx, yy = np.mesh
-0000d4a0: 6772 6964 2878 5f63 6f6f 7264 732c 2079  grid(x_coords, y
-0000d4b0: 5f63 6f6f 7264 7329 0d0a 2020 2020 2020  _coords)..      
-0000d4c0: 2020 0d0a 2020 2020 2020 2020 6672 6f6d    ..        from
-0000d4d0: 2074 7164 6d20 696d 706f 7274 2074 7164   tqdm import tqd
-0000d4e0: 6d0d 0a20 2020 2020 2020 2070 6c61 6e65  m..        plane
-0000d4f0: 733d 5b5d 0d0a 2020 2020 2020 2020 666f  s=[]..        fo
-0000d500: 7220 706f 696e 7473 2069 6e20 7471 646d  r points in tqdm
-0000d510: 2870 6f69 6e74 5f73 6574 732c 2064 6573  (point_sets, des
-0000d520: 633d 2250 726f 6365 7373 696e 6720 6669  c="Processing fi
-0000d530: 7474 6564 2070 6c61 6e65 7322 293a 0d0a  tted planes"):..
-0000d540: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-0000d550: 6e74 2827 706f 696e 7473 3a20 272c 2070  nt('points: ', p
-0000d560: 6f69 6e74 7329 0d0a 2020 2020 2020 2020  oints)..        
-0000d570: 2020 2020 237a 5f76 616c 7565 7320 3d20      #z_values = 
-0000d580: 5b64 6174 615b 696e 7428 2870 6f69 6e74  [data[int((point
-0000d590: 5b31 5d20 2d20 746f 7029 202f 2061 6273  [1] - top) / abs
-0000d5a0: 2874 7261 6e73 666f 726d 5b35 5d29 292c  (transform[5])),
-0000d5b0: 2069 6e74 2828 706f 696e 745b 305d 202d   int((point[0] -
-0000d5c0: 206c 6566 7429 202f 2074 7261 6e73 666f   left) / transfo
-0000d5d0: 726d 5b31 5d29 5d20 666f 7220 706f 696e  rm[1])] for poin
-0000d5e0: 7420 696e 2070 6f69 6e74 735d 0d0a 2020  t in points]..  
-0000d5f0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0000d600: 2020 2020 2020 2020 7a5f 7661 6c75 6573          z_values
-0000d610: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
-0000d620: 2020 2020 2066 6f72 2070 6f69 6e74 2069       for point i
-0000d630: 6e20 706f 696e 7473 3a0d 0a20 2020 2020  n points:..     
-0000d640: 2020 2020 2020 2020 2020 2079 5f69 6e64             y_ind
-0000d650: 6578 203d 2069 6e74 2828 706f 696e 745b  ex = int((point[
-0000d660: 315d 202d 2074 6f70 2920 2f20 6162 7328  1] - top) / abs(
-0000d670: 7472 616e 7366 6f72 6d5b 355d 2929 0d0a  transform[5]))..
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2320 795f 696e 6465 7820 3d20 696e 7428  # y_index = int(
-0000d6a0: 2870 6f69 6e74 5b31 5d20 2d20 746f 7029  (point[1] - top)
-0000d6b0: 202f 2061 6273 2874 7261 6e73 666f 726d   / abs(transform
-0000d6c0: 5b35 5d29 2920 6966 2069 7369 6e73 7461  [5])) if isinsta
-0000d6d0: 6e63 6528 706f 696e 745b 315d 2c20 2869  nce(point[1], (i
-0000d6e0: 6e74 2c20 666c 6f61 7429 2920 616e 6420  nt, float)) and 
-0000d6f0: 6973 696e 7374 616e 6365 2874 7261 6e73  isinstance(trans
-0000d700: 666f 726d 5b35 5d2c 2028 696e 742c 2066  form[5], (int, f
-0000d710: 6c6f 6174 2929 2065 6c73 6520 4e6f 6e65  loat)) else None
-0000d720: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000d730: 2020 2320 785f 696e 6465 7820 3d20 696e    # x_index = in
-0000d740: 7428 2870 6f69 6e74 5b30 5d20 2d20 746f  t((point[0] - to
-0000d750: 7029 202f 2061 6273 2874 7261 6e73 666f  p) / abs(transfo
-0000d760: 726d 5b31 5d29 2920 6966 2069 7369 6e73  rm[1])) if isins
-0000d770: 7461 6e63 6528 706f 696e 745b 305d 2c20  tance(point[0], 
-0000d780: 2869 6e74 2c20 666c 6f61 7429 2920 616e  (int, float)) an
-0000d790: 6420 6973 696e 7374 616e 6365 2874 7261  d isinstance(tra
-0000d7a0: 6e73 666f 726d 5b31 5d2c 2028 696e 742c  nsform[1], (int,
-0000d7b0: 2066 6c6f 6174 2929 2065 6c73 6520 4e6f   float)) else No
-0000d7c0: 6e65 0d0a 0d0a 2020 2020 2020 2020 2020  ne....          
-0000d7d0: 2020 2020 2020 785f 696e 6465 7820 3d20        x_index = 
-0000d7e0: 696e 7428 2870 6f69 6e74 5b30 5d20 2d20  int((point[0] - 
-0000d7f0: 6c65 6674 2920 2f20 7472 616e 7366 6f72  left) / transfor
-0000d800: 6d5b 315d 290d 0a20 2020 2020 2020 2020  m[1])..         
-0000d810: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d820: 2020 2020 2020 2020 207a 5f76 616c 7565           z_value
-0000d830: 203d 2064 6174 615b 795f 696e 6465 785d   = data[y_index]
-0000d840: 5b78 5f69 6e64 6578 5d0d 0a20 2020 2020  [x_index]..     
-0000d850: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000d860: 2020 2020 2020 2020 2020 2020 207a 5f76               z_v
-0000d870: 616c 7565 732e 6170 7065 6e64 287a 5f76  alues.append(z_v
-0000d880: 616c 7565 290d 0a0d 0a20 2020 2020 2020  alue)....       
-0000d890: 2020 2020 2078 797a 5f70 6f69 6e74 7320       xyz_points 
-0000d8a0: 3d20 5b70 6f69 6e74 735b 695d 202b 2028  = [points[i] + (
-0000d8b0: 7a5f 7661 6c75 6573 5b69 5d2c 2920 666f  z_values[i],) fo
-0000d8c0: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
-0000d8d0: 287a 5f76 616c 7565 7329 295d 0d0a 0d0a  (z_values))]....
-0000d8e0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000d8f0: 656e 2878 797a 5f70 6f69 6e74 7329 203e  en(xyz_points) >
-0000d900: 3d20 333a 0d0a 2020 2020 2020 2020 2020  = 3:..          
-0000d910: 2020 2020 2020 6669 7474 6564 5f70 6c61        fitted_pla
-0000d920: 6e65 2c20 612c 2062 2c20 632c 2064 6970  ne, a, b, c, dip
-0000d930: 5f61 6e67 6c65 2c20 6469 705f 6469 7265  _angle, dip_dire
-0000d940: 6374 696f 6e20 3d20 6669 745f 706c 616e  ction = fit_plan
-0000d950: 6528 7879 7a5f 706f 696e 7473 2c20 7878  e(xyz_points, xx
-0000d960: 2c20 7979 290d 0a20 2020 2020 2020 2020  , yy)..         
-0000d970: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0000d980: 2020 2020 2020 2020 2064 6970 5f61 6e67           dip_ang
-0000d990: 6c65 5f6c 6973 742e 6170 7065 6e64 2864  le_list.append(d
-0000d9a0: 6970 5f61 6e67 6c65 290d 0a20 2020 2020  ip_angle)..     
-0000d9b0: 2020 2020 2020 2020 2020 2064 6970 5f64             dip_d
-0000d9c0: 6972 6563 7469 6f6e 5f6c 6973 742e 6170  irection_list.ap
-0000d9d0: 7065 6e64 2864 6970 5f64 6972 6563 7469  pend(dip_directi
-0000d9e0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-0000d9f0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000da00: 2020 2023 2069 6620 6c69 6d69 745f 6578     # if limit_ex
-0000da10: 7465 6e64 3a0d 0a20 2020 2020 2020 2020  tend:..         
-0000da20: 2020 2020 2020 2023 2020 2020 2023 2047         #     # G
-0000da30: 6574 2062 6f75 6e64 696e 6720 626f 7820  et bounding box 
-0000da40: 6f66 2074 6865 2073 656c 6563 7465 6420  of the selected 
-0000da50: 706f 696e 7473 0d0a 2020 2020 2020 2020  points..        
-0000da60: 2020 2020 2020 2020 2320 2020 2020 786d          #     xm
-0000da70: 696e 2c20 786d 6178 2c20 796d 696e 2c20  in, xmax, ymin, 
-0000da80: 796d 6178 203d 2062 6f75 6e64 696e 675f  ymax = bounding_
-0000da90: 626f 7828 7879 7a5f 706f 696e 7473 290d  box(xyz_points).
-0000daa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dab0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0000dac0: 2020 2020 2020 2023 2020 2020 206d 6173         #     mas
-0000dad0: 6b20 3d20 2878 7820 3e3d 2078 6d69 6e29  k = (xx >= xmin)
-0000dae0: 2026 2028 7878 203c 3d20 786d 6178 2920   & (xx <= xmax) 
-0000daf0: 2620 2879 7920 3e3d 2079 6d69 6e29 2026  & (yy >= ymin) &
-0000db00: 2028 7979 203c 3d20 796d 6178 290d 0a20   (yy <= ymax).. 
-0000db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db20: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0000db30: 2020 2020 2023 2020 2020 2066 6f72 2069       #     for i
-0000db40: 2069 6e20 7261 6e67 6528 7878 2e73 6861   in range(xx.sha
-0000db50: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
-0000db60: 2020 2020 2020 2020 2023 2020 2020 2020           #      
-0000db70: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
-0000db80: 6528 7878 2e73 6861 7065 5b31 5d29 3a0d  e(xx.shape[1]):.
-0000db90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dba0: 2023 2020 2020 2020 2020 2020 2020 2069   #             i
-0000dbb0: 6620 6e6f 7420 6d61 736b 5b69 2c20 6a5d  f not mask[i, j]
-0000dbc0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000dbd0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
-0000dbe0: 2020 2020 2066 6974 7465 645f 706c 616e       fitted_plan
-0000dbf0: 655b 692c 206a 5d20 3d20 6e70 2e6e 616e  e[i, j] = np.nan
-0000dc00: 2020 2320 5365 7420 6f75 742d 6f66 2d62    # Set out-of-b
-0000dc10: 6f75 6e64 7320 7661 6c75 6573 2074 6f20  ounds values to 
-0000dc20: 4e61 4e0d 0a20 2020 2020 2020 2020 2020  NaN..           
-0000dc30: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
-0000dc40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000dc50: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0000dc60: 2020 2020 2323 2323 2323 2323 230d 0a20      #########.. 
-0000dc70: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0000dc80: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000dc90: 6e65 732e 6170 7065 6e64 2866 6974 7465  nes.append(fitte
-0000dca0: 645f 706c 616e 6529 0d0a 2020 2020 2020  d_plane)..      
-0000dcb0: 2020 2020 2020 2020 2020 2370 6c61 6e65            #plane
-0000dcc0: 5f63 6f6c 6f72 203d 2072 616e 646f 6d5f  _color = random_
-0000dcd0: 636f 6c6f 7228 290d 0a20 2020 2020 2020  color()..       
-0000dce0: 2020 2020 2020 2020 2070 6c61 6e65 5f63           plane_c
-0000dcf0: 6f6c 6f72 3d63 6f6c 6f72 5f66 726f 6d5f  olor=color_from_
-0000dd00: 6469 705f 616e 645f 6469 7265 6374 696f  dip_and_directio
-0000dd10: 6e28 6469 705f 616e 676c 652c 2064 6970  n(dip_angle, dip
-0000dd20: 5f64 6972 6563 7469 6f6e 290d 0a20 2020  _direction)..   
-0000dd30: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000dd40: 6e65 5f63 6f6c 6f72 732e 6170 7065 6e64  ne_colors.append
-0000dd50: 2870 6c61 6e65 5f63 6f6c 6f72 290d 0a20  (plane_color).. 
-0000dd60: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0000dd70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dd80: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-0000dd90: 2020 2020 2020 2020 2023 2323 230d 0a20           ####.. 
-0000dda0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ddb0: 6f72 2070 6f69 6e74 6e20 696e 2078 797a  or pointn in xyz
-0000ddc0: 5f70 6f69 6e74 733a 0d0a 2020 2020 2020  _points:..      
-0000ddd0: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-0000dde0: 5f32 642e 706c 6f74 2870 6f69 6e74 6e5b  _2d.plot(pointn[
-0000ddf0: 305d 2c20 706f 696e 746e 5b31 5d2c 2027  0], pointn[1], '
-0000de00: 6f27 2c20 636f 6c6f 723d 706c 616e 655f  o', color=plane_
-0000de10: 636f 6c6f 722c 2061 6c70 6861 3d30 2e37  color, alpha=0.7
-0000de20: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000de30: 2020 2063 616e 7661 735f 3264 2e64 7261     canvas_2d.dra
-0000de40: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
-0000de50: 2020 2020 2020 2023 6178 5f33 642e 636c         #ax_3d.cl
-0000de60: 6561 7228 290d 0a20 2020 2020 2020 2020  ear()..         
-0000de70: 2020 2020 2020 2061 785f 3364 2e73 6574         ax_3d.set
-0000de80: 5f74 6974 6c65 2827 3344 2044 454d 2077  _title('3D DEM w
-0000de90: 6974 6820 4669 7474 6564 2050 6c61 6e65  ith Fitted Plane
-0000dea0: 7327 290d 0a20 2020 2020 2020 2020 2020  s')..           
-0000deb0: 2020 2020 2061 785f 3364 2e70 6c6f 745f       ax_3d.plot_
-0000dec0: 7375 7266 6163 6528 7878 2c20 7979 2c20  surface(xx, yy, 
-0000ded0: 6461 7461 2c20 636d 6170 3d27 7465 7272  data, cmap='terr
-0000dee0: 6169 6e27 2c20 6c69 6e65 7769 6474 683d  ain', linewidth=
-0000def0: 302c 2061 6e74 6961 6c69 6173 6564 3d54  0, antialiased=T
-0000df00: 7275 652c 2061 6c70 6861 3d30 2e35 290d  rue, alpha=0.5).
-0000df10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df20: 2023 666f 7220 706c 616e 6520 696e 2070   #for plane in p
-0000df30: 6c61 6e65 733a 0d0a 2020 2020 2020 2020  lanes:..        
-0000df40: 2020 2020 2020 2020 6178 5f33 642e 706c          ax_3d.pl
-0000df50: 6f74 5f73 7572 6661 6365 2878 782c 2079  ot_surface(xx, y
-0000df60: 792c 2066 6974 7465 645f 706c 616e 652c  y, fitted_plane,
-0000df70: 2061 6c70 6861 3d30 2e36 2c20 6c69 6e65   alpha=0.6, line
-0000df80: 7769 6474 683d 302c 2061 6e74 6961 6c69  width=0, antiali
-0000df90: 6173 6564 3d54 7275 652c 2063 6f6c 6f72  ased=True, color
-0000dfa0: 3d70 6c61 6e65 5f63 6f6c 6f72 290d 0a20  =plane_color).. 
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000dfc0: 616e 7661 735f 3364 2e64 7261 7728 290d  anvas_3d.draw().
-0000dfd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dfe0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0000dff0: 2020 2070 6c6f 745f 706c 616e 6573 2864     plot_planes(d
-0000e000: 6970 5f61 6e67 6c65 5f6c 6973 742c 2064  ip_angle_list, d
-0000e010: 6970 5f64 6972 6563 7469 6f6e 5f6c 6973  ip_direction_lis
-0000e020: 742c 2070 6c61 6e65 5f63 6f6c 6f72 7329  t, plane_colors)
-0000e030: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
-0000e040: 2020 2020 2020 2020 0d0a 2020 2020 0d0a          ..    ..
-0000e050: 0d0a 2020 2020 6465 6620 706c 6f74 5f64  ..    def plot_d
-0000e060: 656d 2864 6174 612c 2074 7261 6e73 666f  em(data, transfo
-0000e070: 726d 2c20 7072 6f6a 6563 7469 6f6e 2c20  rm, projection, 
-0000e080: 7061 7468 5f74 6f5f 7368 6170 6566 696c  path_to_shapefil
-0000e090: 6529 3a0d 0a20 2020 2020 2020 2067 6c6f  e):..        glo
-0000e0a0: 6261 6c20 6178 5f32 642c 2061 785f 3364  bal ax_2d, ax_3d
-0000e0b0: 2c20 706f 696e 7473 2c20 6361 6e76 6173  , points, canvas
-0000e0c0: 5f32 642c 2063 616e 7661 735f 3364 2c20  _2d, canvas_3d, 
-0000e0d0: 706f 696e 7473 5f6c 6973 7462 6f78 2c20  points_listbox, 
-0000e0e0: 706c 616e 6573 2c20 706c 616e 655f 636f  planes, plane_co
-0000e0f0: 6c6f 7273 2c20 6873 2c20 6c65 6674 2c20  lors, hs, left, 
-0000e100: 7269 6768 742c 2062 6f74 746f 6d2c 2074  right, bottom, t
-0000e110: 6f70 0d0a 2020 2020 2020 2020 706f 696e  op..        poin
-0000e120: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
-0000e130: 2070 6c61 6e65 7320 3d20 5b5d 0d0a 2020   planes = []..  
-0000e140: 2020 2020 2020 706c 616e 655f 636f 6c6f        plane_colo
-0000e150: 7273 203d 205b 5d0d 0a20 2020 2020 2020  rs = []..       
-0000e160: 200d 0a20 2020 2020 2020 200d 0a0d 0a20   ..        .... 
-0000e170: 2020 2020 2020 2068 7320 3d20 6573 2e68         hs = es.h
-0000e180: 696c 6c73 6861 6465 2864 6174 6129 0d0a  illshade(data)..
-0000e190: 0d0a 2020 2020 2020 2020 726f 6f74 203d  ..        root =
-0000e1a0: 2074 6b2e 546b 2829 0d0a 2020 2020 2020   tk.Tk()..      
-0000e1b0: 2020 726f 6f74 2e74 6974 6c65 2822 416b    root.title("Ak
-0000e1c0: 6864 6566 6f5f 4669 7450 6c61 6e65 7322  hdefo_FitPlanes"
-0000e1d0: 290d 0a0d 0a20 2020 2020 2020 206c 6566  )....        lef
-0000e1e0: 742c 2063 656c 6c5f 7369 7a65 5f78 2c20  t, cell_size_x, 
-0000e1f0: 5f2c 2074 6f70 2c20 5f2c 2063 656c 6c5f  _, top, _, cell_
-0000e200: 7369 7a65 5f79 203d 2074 7261 6e73 666f  size_y = transfo
-0000e210: 726d 0d0a 2020 2020 2020 2020 0d0a 2020  rm..        ..  
-0000e220: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
-0000e230: 6967 6874 203d 206c 6566 7420 2b20 6365  ight = left + ce
-0000e240: 6c6c 5f73 697a 655f 7820 2a20 6461 7461  ll_size_x * data
-0000e250: 2e73 6861 7065 5b31 5d0d 0a20 2020 2020  .shape[1]..     
-0000e260: 2020 2062 6f74 746f 6d20 3d20 746f 7020     bottom = top 
-0000e270: 2b20 6365 6c6c 5f73 697a 655f 7920 2a20  + cell_size_y * 
-0000e280: 6461 7461 2e73 6861 7065 5b30 5d0d 0a0d  data.shape[0]...
-0000e290: 0a20 2020 2020 2020 2066 6967 3120 3d20  .        fig1 = 
-0000e2a0: 706c 742e 4669 6775 7265 2866 6967 7369  plt.Figure(figsi
-0000e2b0: 7a65 3d28 362c 2036 292c 2064 7069 3d31  ze=(6, 6), dpi=1
-0000e2c0: 3530 290d 0a20 2020 2020 2020 2061 785f  50)..        ax_
-0000e2d0: 3264 203d 2066 6967 312e 6164 645f 7375  2d = fig1.add_su
-0000e2e0: 6270 6c6f 7428 3131 3129 0d0a 2020 2020  bplot(111)..    
-0000e2f0: 2020 2020 6178 5f32 642e 696d 7368 6f77      ax_2d.imshow
-0000e300: 2868 732c 2063 6d61 703d 2767 7261 7927  (hs, cmap='gray'
-0000e310: 2c20 6578 7465 6e74 3d5b 6c65 6674 2c20  , extent=[left, 
-0000e320: 7269 6768 742c 2062 6f74 746f 6d2c 2074  right, bottom, t
-0000e330: 6f70 5d29 0d0a 2020 2020 2020 2020 6178  op])..        ax
-0000e340: 5f32 642e 7365 745f 7469 746c 6528 2748  _2d.set_title('H
-0000e350: 696c 6c73 6861 6465 272c 2066 6f6e 7477  illshade', fontw
-0000e360: 6569 6768 743d 2262 6f6c 6422 2c20 666f  eight="bold", fo
-0000e370: 6e74 7369 7a65 3d31 3429 0d0a 2020 2020  ntsize=14)..    
-0000e380: 2020 2020 6178 5f32 642e 7365 745f 786c      ax_2d.set_xl
-0000e390: 6162 656c 2822 4c6f 6e67 6974 7564 6522  abel("Longitude"
-0000e3a0: 2c20 666f 6e74 7369 7a65 3d31 3229 0d0a  , fontsize=12)..
-0000e3b0: 2020 2020 2020 2020 6178 5f32 642e 7365          ax_2d.se
-0000e3c0: 745f 796c 6162 656c 2822 4c61 7469 7475  t_ylabel("Latitu
-0000e3d0: 6465 222c 2066 6f6e 7473 697a 653d 3132  de", fontsize=12
-0000e3e0: 290d 0a20 2020 2020 2020 2061 785f 3264  )..        ax_2d
-0000e3f0: 2e67 7269 6428 5472 7565 2c20 7768 6963  .grid(True, whic
-0000e400: 683d 2762 6f74 6827 2c20 6c69 6e65 7374  h='both', linest
-0000e410: 796c 653d 272d 2d27 2c20 6c69 6e65 7769  yle='--', linewi
-0000e420: 6474 683d 302e 3529 0d0a 2020 2020 2020  dth=0.5)..      
-0000e430: 2020 6178 5f32 642e 7365 745f 6173 7065    ax_2d.set_aspe
-0000e440: 6374 2827 6571 7561 6c27 290d 0a20 2020  ct('equal')..   
-0000e450: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
-0000e460: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0000e470: 2020 2069 6620 7061 7468 5f74 6f5f 7368     if path_to_sh
-0000e480: 6170 6566 696c 6520 6973 206e 6f74 204e  apefile is not N
-0000e490: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-0000e4a0: 2020 6764 6620 3d20 6770 642e 7265 6164    gdf = gpd.read
-0000e4b0: 5f66 696c 6528 7061 7468 5f74 6f5f 7368  _file(path_to_sh
-0000e4c0: 6170 6566 696c 6529 0d0a 2020 2020 2020  apefile)..      
-0000e4d0: 2020 2020 2020 6966 2067 6466 2e63 7273        if gdf.crs
-0000e4e0: 2e74 6f5f 7374 7269 6e67 2829 2021 3d20  .to_string() != 
-0000e4f0: 7072 6f6a 6563 7469 6f6e 3a0d 0a20 2020  projection:..   
-0000e500: 2020 2020 2020 2020 2020 2020 2067 6466               gdf
-0000e510: 203d 2067 6466 2e74 6f5f 6372 7328 7072   = gdf.to_crs(pr
-0000e520: 6f6a 6563 7469 6f6e 290d 0a20 2020 2020  ojection)..     
-0000e530: 2020 2020 2020 2067 6466 2e70 6c6f 7428         gdf.plot(
-0000e540: 6178 3d61 785f 3264 2c20 636f 6c6f 723d  ax=ax_2d, color=
-0000e550: 2772 6564 272c 206c 6162 656c 3d22 4c69  'red', label="Li
-0000e560: 6e65 6172 2046 6561 7475 7265 7322 290d  near Features").
-0000e570: 0a20 2020 2020 2020 2020 2020 2061 785f  .            ax_
-0000e580: 3264 2e6c 6567 656e 6428 6c6f 633d 2275  2d.legend(loc="u
-0000e590: 7070 6572 206c 6566 7422 290d 0a20 2020  pper left")..   
-0000e5a0: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
-0000e5b0: 6967 3220 3d20 706c 742e 4669 6775 7265  ig2 = plt.Figure
-0000e5c0: 2866 6967 7369 7a65 3d28 362c 2036 292c  (figsize=(6, 6),
-0000e5d0: 2064 7069 3d31 3530 290d 0a20 2020 2020   dpi=150)..     
-0000e5e0: 2020 2023 2043 7265 6174 6520 6120 6669     # Create a fi
-0000e5f0: 6775 7265 2061 6e64 2061 7869 730d 0a20  gure and axis.. 
-0000e600: 2020 2020 2020 2061 785f 3364 203d 2066         ax_3d = f
-0000e610: 6967 322e 6164 645f 7375 6270 6c6f 7428  ig2.add_subplot(
-0000e620: 3131 312c 2070 726f 6a65 6374 696f 6e3d  111, projection=
-0000e630: 2733 6427 290d 0a20 2020 2020 2020 2061  '3d')..        a
-0000e640: 785f 3364 2e73 6574 5f74 6974 6c65 2827  x_3d.set_title('
-0000e650: 3344 2044 454d 2077 6974 6820 4669 7474  3D DEM with Fitt
-0000e660: 6564 2050 6c61 6e65 7327 2c20 666f 6e74  ed Planes', font
-0000e670: 7765 6967 6874 3d22 626f 6c64 222c 2066  weight="bold", f
-0000e680: 6f6e 7473 697a 653d 3134 290d 0a20 2020  ontsize=14)..   
-0000e690: 2020 2020 2061 785f 3364 2e73 6574 5f78       ax_3d.set_x
-0000e6a0: 6c61 6265 6c28 224c 6f6e 6769 7475 6465  label("Longitude
-0000e6b0: 222c 2066 6f6e 7473 697a 653d 3132 290d  ", fontsize=12).
-0000e6c0: 0a20 2020 2020 2020 2061 785f 3364 2e73  .        ax_3d.s
-0000e6d0: 6574 5f79 6c61 6265 6c28 224c 6174 6974  et_ylabel("Latit
-0000e6e0: 7564 6522 2c20 666f 6e74 7369 7a65 3d31  ude", fontsize=1
-0000e6f0: 3229 0d0a 2020 2020 2020 2020 6178 5f33  2)..        ax_3
-0000e700: 642e 7365 745f 7a6c 6162 656c 2822 456c  d.set_zlabel("El
-0000e710: 6576 6174 696f 6e22 2c20 666f 6e74 7369  evation", fontsi
-0000e720: 7a65 3d31 3229 0d0a 2020 2020 2020 2020  ze=12)..        
-0000e730: 785f 636f 6f72 6473 203d 206e 702e 6c69  x_coords = np.li
-0000e740: 6e73 7061 6365 286c 6566 742c 2072 6967  nspace(left, rig
-0000e750: 6874 2c20 6461 7461 2e73 6861 7065 5b31  ht, data.shape[1
-0000e760: 5d29 0d0a 2020 2020 2020 2020 795f 636f  ])..        y_co
-0000e770: 6f72 6473 203d 206e 702e 6c69 6e73 7061  ords = np.linspa
-0000e780: 6365 2874 6f70 2c20 626f 7474 6f6d 2c20  ce(top, bottom, 
-0000e790: 6461 7461 2e73 6861 7065 5b30 5d29 0d0a  data.shape[0])..
-0000e7a0: 2020 2020 2020 2020 7878 2c20 7979 203d          xx, yy =
-0000e7b0: 206e 702e 6d65 7368 6772 6964 2878 5f63   np.meshgrid(x_c
-0000e7c0: 6f6f 7264 732c 2079 5f63 6f6f 7264 7329  oords, y_coords)
-0000e7d0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-0000e7e0: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
-0000e7f0: 0d0a 2020 2020 2020 2020 0d0a 0d0a 2020  ..        ....  
-0000e800: 2020 2020 2020 2320 6178 5f33 642e 7365        # ax_3d.se
-0000e810: 745f 786c 696d 285b 6c65 6674 2c20 7269  t_xlim([left, ri
-0000e820: 6768 745d 290d 0a20 2020 2020 2020 2023  ght])..        #
-0000e830: 2061 785f 3364 2e73 6574 5f79 6c69 6d28   ax_3d.set_ylim(
-0000e840: 5b62 6f74 746f 6d2c 2074 6f70 5d29 0d0a  [bottom, top])..
-0000e850: 2020 2020 2020 2020 2320 6178 5f33 642e          # ax_3d.
-0000e860: 7365 745f 7a6c 696d 285b 7a6d 696e 2c20  set_zlim([zmin, 
-0000e870: 7a6d 6178 5d29 0d0a 0d0a 2020 2020 2020  zmax])....      
-0000e880: 2020 6672 616d 655f 3264 203d 2074 6b2e    frame_2d = tk.
-0000e890: 4672 616d 6528 726f 6f74 290d 0a20 2020  Frame(root)..   
-0000e8a0: 2020 2020 2066 7261 6d65 5f32 642e 6772       frame_2d.gr
-0000e8b0: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
-0000e8c0: 3d30 2c20 7374 6963 6b79 3d27 6e73 6577  =0, sticky='nsew
-0000e8d0: 2729 0d0a 2020 2020 2020 2020 2320 6361  ')..        # ca
-0000e8e0: 6e76 6173 5f32 6420 3d20 4669 6775 7265  nvas_2d = Figure
-0000e8f0: 4361 6e76 6173 546b 4167 6728 6669 6731  CanvasTkAgg(fig1
-0000e900: 2c20 6d61 7374 6572 3d66 7261 6d65 5f32  , master=frame_2
-0000e910: 6429 0d0a 2020 2020 2020 2020 2320 6361  d)..        # ca
-0000e920: 6e76 6173 5f32 642e 6765 745f 746b 5f77  nvas_2d.get_tk_w
-0000e930: 6964 6765 7428 292e 7061 636b 2866 696c  idget().pack(fil
-0000e940: 6c3d 746b 2e42 4f54 482c 2065 7870 616e  l=tk.BOTH, expan
-0000e950: 643d 4661 6c73 6529 0d0a 2020 2020 2020  d=False)..      
-0000e960: 2020 2320 746f 6f6c 6261 725f 3264 203d    # toolbar_2d =
-0000e970: 204e 6176 6967 6174 696f 6e54 6f6f 6c62   NavigationToolb
-0000e980: 6172 3254 6b28 6361 6e76 6173 5f32 642c  ar2Tk(canvas_2d,
-0000e990: 2066 7261 6d65 5f32 6429 0d0a 2020 2020   frame_2d)..    
-0000e9a0: 2020 2020 2320 746f 6f6c 6261 725f 3264      # toolbar_2d
-0000e9b0: 2e75 7064 6174 6528 290d 0a20 2020 2020  .update()..     
-0000e9c0: 2020 2023 2043 7265 6174 6520 7468 6520     # Create the 
-0000e9d0: 6361 6e76 6173 2066 6f72 2074 6865 2070  canvas for the p
-0000e9e0: 6c6f 740d 0a20 2020 2020 2020 2063 616e  lot..        can
-0000e9f0: 7661 735f 3264 203d 2046 6967 7572 6543  vas_2d = FigureC
-0000ea00: 616e 7661 7354 6b41 6767 2866 6967 312c  anvasTkAgg(fig1,
-0000ea10: 206d 6173 7465 723d 6672 616d 655f 3264   master=frame_2d
-0000ea20: 290d 0a20 2020 2020 2020 2063 616e 7661  )..        canva
-0000ea30: 735f 3264 2e67 6574 5f74 6b5f 7769 6467  s_2d.get_tk_widg
-0000ea40: 6574 2829 2e70 6163 6b28 6669 6c6c 3d74  et().pack(fill=t
-0000ea50: 6b2e 424f 5448 2c20 6578 7061 6e64 3d54  k.BOTH, expand=T
-0000ea60: 7275 6529 2020 2320 4669 6c6c 2074 6865  rue)  # Fill the
-0000ea70: 2066 7261 6d65 0d0a 2020 2020 2020 2020   frame..        
-0000ea80: 2320 4372 6561 7465 2074 6865 2074 6f6f  # Create the too
-0000ea90: 6c62 6172 2061 6e64 2070 6c61 6365 2069  lbar and place i
-0000eaa0: 7420 6174 2074 6865 2074 6f70 206f 6620  t at the top of 
-0000eab0: 7468 6520 6361 6e76 6173 0d0a 2020 2020  the canvas..    
-0000eac0: 2020 2020 746f 6f6c 6261 725f 3264 203d      toolbar_2d =
-0000ead0: 204e 6176 6967 6174 696f 6e54 6f6f 6c62   NavigationToolb
-0000eae0: 6172 3254 6b28 6361 6e76 6173 5f32 642c  ar2Tk(canvas_2d,
-0000eaf0: 2066 7261 6d65 5f32 6429 0d0a 2020 2020   frame_2d)..    
-0000eb00: 2020 2020 746f 6f6c 6261 725f 3264 2e75      toolbar_2d.u
-0000eb10: 7064 6174 6528 290d 0a20 2020 2020 2020  pdate()..       
-0000eb20: 2074 6f6f 6c62 6172 5f32 642e 7061 636b   toolbar_2d.pack
-0000eb30: 2873 6964 653d 746b 2e54 4f50 2c20 6669  (side=tk.TOP, fi
-0000eb40: 6c6c 3d74 6b2e 5829 2020 2320 5061 636b  ll=tk.X)  # Pack
-0000eb50: 2074 6865 2074 6f6f 6c62 6172 2061 7420   the toolbar at 
-0000eb60: 7468 6520 746f 700d 0a20 2020 2020 2020  the top..       
-0000eb70: 200d 0a20 2020 2020 2020 2023 2323 2323   ..        #####
-0000eb80: 2323 6164 6420 636f 6c6f 7262 6172 2066  ##add colorbar f
-0000eb90: 6967 7572 6520 746f 2043 616e 7661 730d  igure to Canvas.
-0000eba0: 0a20 2020 2020 2020 200d 0a0d 0a0d 0a0d  .        .......
-0000ebb0: 0a20 2020 2020 2020 2066 7261 6d65 5f33  .        frame_3
-0000ebc0: 6420 3d20 746b 2e46 7261 6d65 2872 6f6f  d = tk.Frame(roo
-0000ebd0: 7429 0d0a 2020 2020 2020 2020 6672 616d  t)..        fram
-0000ebe0: 655f 3364 2e67 7269 6428 726f 773d 302c  e_3d.grid(row=0,
-0000ebf0: 2063 6f6c 756d 6e3d 312c 2073 7469 636b   column=1, stick
-0000ec00: 793d 276e 7365 7727 290d 0a20 2020 2020  y='nsew')..     
-0000ec10: 2020 2023 2063 616e 7661 735f 3364 203d     # canvas_3d =
-0000ec20: 2046 6967 7572 6543 616e 7661 7354 6b41   FigureCanvasTkA
-0000ec30: 6767 2866 6967 322c 206d 6173 7465 723d  gg(fig2, master=
-0000ec40: 6672 616d 655f 3364 290d 0a20 2020 2020  frame_3d)..     
-0000ec50: 2020 2023 2063 616e 7661 735f 3364 2e67     # canvas_3d.g
-0000ec60: 6574 5f74 6b5f 7769 6467 6574 2829 2e70  et_tk_widget().p
-0000ec70: 6163 6b28 6669 6c6c 3d74 6b2e 424f 5448  ack(fill=tk.BOTH
-0000ec80: 2c20 6578 7061 6e64 3d46 616c 7365 290d  , expand=False).
-0000ec90: 0a20 2020 2020 2020 2023 2074 6f6f 6c62  .        # toolb
-0000eca0: 6172 5f33 6420 3d20 4e61 7669 6761 7469  ar_3d = Navigati
-0000ecb0: 6f6e 546f 6f6c 6261 7232 546b 2863 616e  onToolbar2Tk(can
-0000ecc0: 7661 735f 3364 2c20 6672 616d 655f 3364  vas_3d, frame_3d
-0000ecd0: 290d 0a20 2020 2020 2020 2023 2074 6f6f  )..        # too
-0000ece0: 6c62 6172 5f33 642e 7570 6461 7465 2829  lbar_3d.update()
-0000ecf0: 0d0a 2020 2020 2020 2020 6361 6e76 6173  ..        canvas
-0000ed00: 5f33 6420 3d20 4669 6775 7265 4361 6e76  _3d = FigureCanv
-0000ed10: 6173 546b 4167 6728 6669 6732 2c20 6d61  asTkAgg(fig2, ma
-0000ed20: 7374 6572 3d66 7261 6d65 5f33 6429 0d0a  ster=frame_3d)..
-0000ed30: 2020 2020 2020 2020 6361 6e76 6173 5f33          canvas_3
-0000ed40: 642e 6765 745f 746b 5f77 6964 6765 7428  d.get_tk_widget(
-0000ed50: 292e 7061 636b 2866 696c 6c3d 746b 2e42  ).pack(fill=tk.B
-0000ed60: 4f54 482c 2065 7870 616e 643d 5472 7565  OTH, expand=True
-0000ed70: 2920 2023 2046 696c 6c20 7468 6520 6672  )  # Fill the fr
-0000ed80: 616d 650d 0a20 2020 2020 2020 2023 2043  ame..        # C
-0000ed90: 7265 6174 6520 7468 6520 746f 6f6c 6261  reate the toolba
-0000eda0: 7220 616e 6420 706c 6163 6520 6974 2061  r and place it a
-0000edb0: 7420 7468 6520 746f 7020 6f66 2074 6865  t the top of the
-0000edc0: 2063 616e 7661 730d 0a20 2020 2020 2020   canvas..       
-0000edd0: 2074 6f6f 6c62 6172 5f33 6420 3d20 4e61   toolbar_3d = Na
-0000ede0: 7669 6761 7469 6f6e 546f 6f6c 6261 7232  vigationToolbar2
-0000edf0: 546b 2863 616e 7661 735f 3364 2c20 6672  Tk(canvas_3d, fr
-0000ee00: 616d 655f 3364 290d 0a20 2020 2020 2020  ame_3d)..       
-0000ee10: 2074 6f6f 6c62 6172 5f33 642e 7570 6461   toolbar_3d.upda
-0000ee20: 7465 2829 0d0a 2020 2020 2020 2020 746f  te()..        to
-0000ee30: 6f6c 6261 725f 3364 2e70 6163 6b28 7369  olbar_3d.pack(si
-0000ee40: 6465 3d74 6b2e 544f 502c 2066 696c 6c3d  de=tk.TOP, fill=
-0000ee50: 746b 2e58 2920 2023 2050 6163 6b20 7468  tk.X)  # Pack th
-0000ee60: 6520 746f 6f6c 6261 7220 6174 2074 6865  e toolbar at the
-0000ee70: 2074 6f70 0d0a 0d0a 2020 2020 2020 2020   top....        
-0000ee80: 2320 4372 6561 7465 2061 2066 7261 6d65  # Create a frame
-0000ee90: 206f 6e20 7468 6520 7269 6768 7420 746f   on the right to
-0000eea0: 2068 6f6c 6420 636f 6e74 726f 6c73 0d0a   hold controls..
-0000eeb0: 2020 2020 2020 2020 636f 6e74 726f 6c73          controls
-0000eec0: 5f66 7261 6d65 203d 2074 6b2e 4672 616d  _frame = tk.Fram
-0000eed0: 6528 726f 6f74 290d 0a20 2020 2020 2020  e(root)..       
-0000eee0: 2063 6f6e 7472 6f6c 735f 6672 616d 652e   controls_frame.
-0000eef0: 6772 6964 2872 6f77 3d30 2c20 636f 6c75  grid(row=0, colu
-0000ef00: 6d6e 3d33 2c20 726f 7773 7061 6e3d 312c  mn=3, rowspan=1,
-0000ef10: 2073 7469 636b 793d 276e 7365 7727 290d   sticky='nsew').
-0000ef20: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
-0000ef30: 2020 2020 2023 204e 6f77 2070 7574 2061       # Now put a
-0000ef40: 6c6c 2062 7574 746f 6e73 2061 6e64 204c  ll buttons and L
-0000ef50: 6973 7462 6f78 2069 6e73 6964 6520 7468  istbox inside th
-0000ef60: 6973 2063 6f6e 7472 6f6c 735f 6672 616d  is controls_fram
-0000ef70: 650d 0a20 2020 2020 2020 2064 7261 775f  e..        draw_
-0000ef80: 6275 7474 6f6e 203d 2074 746b 2e42 7574  button = ttk.But
-0000ef90: 746f 6e28 636f 6e74 726f 6c73 5f66 7261  ton(controls_fra
-0000efa0: 6d65 2c20 7465 7874 3d22 4472 6177 2050  me, text="Draw P
-0000efb0: 6c61 6e65 222c 2063 6f6d 6d61 6e64 3d6c  lane", command=l
-0000efc0: 616d 6264 613a 2064 7261 775f 706c 616e  ambda: draw_plan
-0000efd0: 6528 7878 2c79 7929 290d 0a20 2020 2020  e(xx,yy))..     
-0000efe0: 2020 2064 7261 775f 6275 7474 6f6e 2e70     draw_button.p
-0000eff0: 6163 6b28 7061 6479 3d32 2c20 7061 6478  ack(pady=2, padx
-0000f000: 3d32 290d 0a0d 0a20 2020 2020 2020 206c  =2)....        l
-0000f010: 696e 655f 706c 616e 655f 6275 7474 6f6e  ine_plane_button
-0000f020: 203d 2074 746b 2e42 7574 746f 6e28 636f   = ttk.Button(co
-0000f030: 6e74 726f 6c73 5f66 7261 6d65 2c20 7465  ntrols_frame, te
-0000f040: 7874 3d22 4372 6561 7465 2050 6c61 6e65  xt="Create Plane
-0000f050: 7320 6672 6f6d 204c 696e 6573 222c 2063  s from Lines", c
-0000f060: 6f6d 6d61 6e64 3d6c 616d 6264 613a 2064  ommand=lambda: d
-0000f070: 7261 775f 706c 616e 6573 5f66 726f 6d5f  raw_planes_from_
-0000f080: 6c69 6e65 7328 7878 2c79 7929 290d 0a20  lines(xx,yy)).. 
-0000f090: 2020 2020 2020 206c 696e 655f 706c 616e         line_plan
-0000f0a0: 655f 6275 7474 6f6e 2e70 6163 6b28 7061  e_button.pack(pa
-0000f0b0: 6479 3d32 2c20 7061 6478 3d32 290d 0a0d  dy=2, padx=2)...
-0000f0c0: 0a20 2020 2020 2020 2073 6176 655f 706c  .        save_pl
-0000f0d0: 616e 655f 6275 7474 6f6e 203d 2074 746b  ane_button = ttk
-0000f0e0: 2e42 7574 746f 6e28 636f 6e74 726f 6c73  .Button(controls
-0000f0f0: 5f66 7261 6d65 2c20 7465 7874 3d22 5361  _frame, text="Sa
-0000f100: 7665 2050 6c61 6e65 7320 746f 204f 424a  ve Planes to OBJ
-0000f110: 222c 2063 6f6d 6d61 6e64 3d73 6176 655f  ", command=save_
-0000f120: 706c 616e 6573 5f74 6f5f 6f62 6a29 2023  planes_to_obj) #
-0000f130: 7361 7665 5f66 6974 7465 645f 706c 616e  save_fitted_plan
-0000f140: 6573 5f61 735f 6478 660d 0a20 2020 2020  es_as_dxf..     
-0000f150: 2020 2073 6176 655f 706c 616e 655f 6275     save_plane_bu
-0000f160: 7474 6f6e 2e70 6163 6b28 7061 6479 3d32  tton.pack(pady=2
-0000f170: 2c20 7061 6478 3d32 290d 0a20 2020 2020  , padx=2)..     
-0000f180: 2020 2023 2073 6176 655f 706c 616e 655f     # save_plane_
-0000f190: 6275 7474 6f6e 5f64 7866 203d 2074 746b  button_dxf = ttk
-0000f1a0: 2e42 7574 746f 6e28 636f 6e74 726f 6c73  .Button(controls
-0000f1b0: 5f66 7261 6d65 2c20 7465 7874 3d22 5361  _frame, text="Sa
-0000f1c0: 7665 2050 6c61 6e65 7320 746f 2044 5846  ve Planes to DXF
-0000f1d0: 222c 2063 6f6d 6d61 6e64 3d73 6176 655f  ", command=save_
-0000f1e0: 6669 7474 6564 5f70 6c61 6e65 735f 6173  fitted_planes_as
-0000f1f0: 5f64 7866 290d 0a20 2020 2020 2020 2023  _dxf)..        #
-0000f200: 2073 6176 655f 706c 616e 655f 6275 7474   save_plane_butt
-0000f210: 6f6e 5f64 7866 2e70 6163 6b28 7061 6479  on_dxf.pack(pady
-0000f220: 3d31 302c 2070 6164 783d 3130 290d 0a0d  =10, padx=10)...
-0000f230: 0a20 2020 2020 2020 2070 6f69 6e74 735f  .        points_
-0000f240: 6c69 7374 626f 7820 3d20 746b 2e4c 6973  listbox = tk.Lis
-0000f250: 7462 6f78 2863 6f6e 7472 6f6c 735f 6672  tbox(controls_fr
-0000f260: 616d 652c 2068 6569 6768 743d 352c 2077  ame, height=5, w
-0000f270: 6964 7468 3d34 302c 2065 7870 6f72 7473  idth=40, exports
-0000f280: 656c 6563 7469 6f6e 3d46 616c 7365 290d  election=False).
-0000f290: 0a20 2020 2020 2020 2070 6f69 6e74 735f  .        points_
-0000f2a0: 6c69 7374 626f 782e 7061 636b 2870 6164  listbox.pack(pad
-0000f2b0: 793d 322c 2070 6164 783d 322c 2066 696c  y=2, padx=2, fil
-0000f2c0: 6c3d 2762 6f74 6827 2c20 6578 7061 6e64  l='both', expand
-0000f2d0: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
-0000f2e0: 0d0a 2020 2020 2020 2020 7363 726f 6c6c  ..        scroll
-0000f2f0: 6261 7220 3d20 7474 6b2e 5363 726f 6c6c  bar = ttk.Scroll
-0000f300: 6261 7228 636f 6e74 726f 6c73 5f66 7261  bar(controls_fra
-0000f310: 6d65 2c20 6f72 6965 6e74 3d22 7665 7274  me, orient="vert
-0000f320: 6963 616c 222c 2063 6f6d 6d61 6e64 3d70  ical", command=p
-0000f330: 6f69 6e74 735f 6c69 7374 626f 782e 7976  oints_listbox.yv
-0000f340: 6965 7729 0d0a 2020 2020 2020 2020 7363  iew)..        sc
-0000f350: 726f 6c6c 6261 722e 7061 636b 2873 6964  rollbar.pack(sid
-0000f360: 653d 746b 2e52 4947 4854 2c20 6669 6c6c  e=tk.RIGHT, fill
-0000f370: 3d74 6b2e 5929 0d0a 2020 2020 2020 2020  =tk.Y)..        
-0000f380: 0d0a 2020 2020 2020 2020 706f 696e 7473  ..        points
-0000f390: 5f6c 6973 7462 6f78 2e63 6f6e 6669 6728  _listbox.config(
-0000f3a0: 7973 6372 6f6c 6c63 6f6d 6d61 6e64 3d73  yscrollcommand=s
-0000f3b0: 6372 6f6c 6c62 6172 2e73 6574 290d 0a20  crollbar.set).. 
-0000f3c0: 2020 2020 2020 2070 6f69 6e74 735f 6c69         points_li
-0000f3d0: 7374 626f 782e 6269 6e64 2822 3c44 6f75  stbox.bind("<Dou
-0000f3e0: 626c 652d 4275 7474 6f6e 2d31 3e22 2c20  ble-Button-1>", 
-0000f3f0: 6f6e 5f70 6f69 6e74 5f64 6f75 626c 655f  on_point_double_
-0000f400: 636c 6963 6b29 0d0a 2020 2020 2020 2020  click)..        
-0000f410: 2323 2323 0d0a 2020 2020 0d0a 2020 2020  ####..    ..    
-0000f420: 2020 2020 0d0a 2020 2020 2020 2020 2323      ..        ##
-0000f430: 2323 0d0a 0d0a 2020 2020 2020 2020 6669  ##....        fi
-0000f440: 6731 2e63 616e 7661 732e 6d70 6c5f 636f  g1.canvas.mpl_co
-0000f450: 6e6e 6563 7428 2762 7574 746f 6e5f 7072  nnect('button_pr
-0000f460: 6573 735f 6576 656e 7427 2c20 6c61 6d62  ess_event', lamb
-0000f470: 6461 2065 7665 6e74 3a20 6f6e 636c 6963  da event: onclic
-0000f480: 6b28 6576 656e 742c 2070 6f69 6e74 732c  k(event, points,
-0000f490: 2064 6174 612c 2074 7261 6e73 666f 726d   data, transform
-0000f4a0: 2929 0d0a 2020 2020 2020 2020 0d0a 2020  ))..        ..  
-0000f4b0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0000f4c0: 2320 4164 6469 6e67 2074 6865 2073 697a  # Adding the siz
-0000f4d0: 6520 6772 6970 2066 6f72 2077 696e 646f  e grip for windo
-0000f4e0: 7720 7265 7369 7a69 6e67 0d0a 2020 2020  w resizing..    
-0000f4f0: 2020 2020 7369 7a65 6772 6970 203d 2074      sizegrip = t
-0000f500: 746b 2e53 697a 6567 7269 7028 726f 6f74  tk.Sizegrip(root
-0000f510: 290d 0a20 2020 2020 2020 2073 697a 6567  )..        sizeg
-0000f520: 7269 702e 6772 6964 2872 6f77 3d33 2c20  rip.grid(row=3, 
-0000f530: 636f 6c75 6d6e 3d31 2c20 7374 6963 6b79  column=1, sticky
-0000f540: 3d27 6e73 6577 2729 0d0a 0d0a 2020 2020  ='nsew')....    
-0000f550: 2020 2020 2320 4d61 6b69 6e67 2074 6865      # Making the
-0000f560: 2064 6573 6967 6e20 7265 7370 6f6e 7369   design responsi
-0000f570: 7665 0d0a 2020 2020 2020 2020 726f 6f74  ve..        root
-0000f580: 2e67 7269 645f 726f 7763 6f6e 6669 6775  .grid_rowconfigu
-0000f590: 7265 2830 2c20 7765 6967 6874 3d31 2920  re(0, weight=1) 
-0000f5a0: 2023 2043 616e 7661 7320 726f 770d 0a20   # Canvas row.. 
-0000f5b0: 2020 2020 2020 2072 6f6f 742e 6772 6964         root.grid
-0000f5c0: 5f72 6f77 636f 6e66 6967 7572 6528 312c  _rowconfigure(1,
-0000f5d0: 2077 6569 6768 743d 3029 2020 2320 546f   weight=0)  # To
-0000f5e0: 6f6c 6261 7220 726f 770d 0a20 2020 2020  olbar row..     
-0000f5f0: 2020 2072 6f6f 742e 6772 6964 5f72 6f77     root.grid_row
-0000f600: 636f 6e66 6967 7572 6528 322c 2077 6569  configure(2, wei
-0000f610: 6768 743d 3029 2020 2320 4275 7474 6f6e  ght=0)  # Button
-0000f620: 2072 6f77 0d0a 2020 2020 2020 2020 726f   row..        ro
-0000f630: 6f74 2e67 7269 645f 636f 6c75 6d6e 636f  ot.grid_columnco
-0000f640: 6e66 6967 7572 6528 302c 2077 6569 6768  nfigure(0, weigh
-0000f650: 743d 3129 2020 2320 3244 2070 6c6f 7420  t=1)  # 2D plot 
-0000f660: 636f 6c75 6d6e 0d0a 2020 2020 2020 2020  column..        
-0000f670: 726f 6f74 2e67 7269 645f 636f 6c75 6d6e  root.grid_column
-0000f680: 636f 6e66 6967 7572 6528 312c 2077 6569  configure(1, wei
-0000f690: 6768 743d 3129 2020 2320 3344 2070 6c6f  ght=1)  # 3D plo
-0000f6a0: 7420 636f 6c75 6d6e 0d0a 2020 2020 2020  t column..      
-0000f6b0: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0000f6d0: 2020 2020 2020 2020 726f 6f74 2e6d 6169          root.mai
-0000f6e0: 6e6c 6f6f 7028 290d 0a0d 0a0d 0a20 2020  nloop()......   
-0000f6f0: 200d 0a20 2020 2070 6c6f 745f 6465 6d28   ..    plot_dem(
-0000f700: 6461 7461 2c20 7472 616e 7366 6f72 6d2c  data, transform,
-0000f710: 2070 726f 6a65 6374 696f 6e2c 206c 696e   projection, lin
-0000f720: 655f 7368 6170 6566 696c 6529 0d0a 2020  e_shapefile)..  
-0000f730: 200d 0a20 2020 200d 0a23 616b 6864 6566   ..    ..#akhdef
-0000f740: 6f5f 6669 7450 6c61 6e65 2864 656d 5f64  o_fitPlane(dem_d
-0000f750: 6174 613d 2763 7572 7269 652f 6465 6d5f  ata='currie/dem_
-0000f760: 316d 2e74 6966 272c 206c 696e 655f 7368  1m.tif', line_sh
-0000f770: 6170 6566 696c 653d 2763 7572 7269 652f  apefile='currie/
-0000f780: 6c69 6e65 732e 7368 7027 2c20 6f75 745f  lines.shp', out_
-0000f790: 706c 616e 6546 6f6c 6465 723d 2750 6c61  planeFolder='Pla
-0000f7a0: 6e65 735f 6f75 742f 6e65 7727 2c20 6c69  nes_out/new', li
-0000f7b0: 6d69 745f 6578 7465 6e64 3d46 616c 7365  mit_extend=False
-0000f7c0: 290d 0a0d 0a69 6d70 6f72 7420 6f73 0d0a  )....import os..
-0000f7d0: 696d 706f 7274 2073 6875 7469 6c0d 0a0d  import shutil...
-0000f7e0: 0a64 6566 206d 6f76 655f 6669 6c65 735f  .def move_files_
-0000f7f0: 7769 7468 5f73 7472 696e 6728 736f 7572  with_string(sour
-0000f800: 6365 5f64 6972 3a20 7374 7220 3d22 222c  ce_dir: str ="",
-0000f810: 2064 6573 745f 6469 723a 2073 7472 203d   dest_dir: str =
-0000f820: 2222 2c20 7365 6172 6368 5f73 7472 696e  "", search_strin
-0000f830: 673a 2073 7472 203d 222e 7469 6622 293a  g: str =".tif"):
-0000f840: 0d0a 2020 2020 2222 220d 0a20 2020 204d  ..    """..    M
-0000f850: 6f76 6520 6669 6c65 7320 6672 6f6d 2061  ove files from a
-0000f860: 2073 6f75 7263 6520 6469 7265 6374 6f72   source director
-0000f870: 7920 746f 2061 2064 6573 7469 6e61 7469  y to a destinati
-0000f880: 6f6e 2064 6972 6563 746f 7279 2062 6173  on directory bas
-0000f890: 6564 206f 6e20 6120 7365 6172 6368 2073  ed on a search s
-0000f8a0: 7472 696e 6720 7072 6573 656e 7420 696e  tring present in
-0000f8b0: 2074 6865 6972 2070 6174 6873 2e0d 0a0d   their paths....
-0000f8c0: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
-0000f8d0: 0d0a 2020 2020 2d20 736f 7572 6365 5f64  ..    - source_d
-0000f8e0: 6972 2028 7374 7229 3a20 5468 6520 6469  ir (str): The di
-0000f8f0: 7265 6374 6f72 7920 6672 6f6d 2077 6869  rectory from whi
-0000f900: 6368 2066 696c 6573 2061 7265 2074 6f20  ch files are to 
-0000f910: 6265 206d 6f76 6564 2e0d 0a20 2020 202d  be moved...    -
-0000f920: 2064 6573 745f 6469 7220 2873 7472 293a   dest_dir (str):
-0000f930: 2054 6865 2064 6573 7469 6e61 7469 6f6e   The destination
-0000f940: 2064 6972 6563 746f 7279 2077 6865 7265   directory where
-0000f950: 2066 696c 6573 2077 696c 6c20 6265 206d   files will be m
-0000f960: 6f76 6564 2e0d 0a20 2020 202d 2073 6561  oved...    - sea
-0000f970: 7263 685f 7374 7269 6e67 2028 7374 7229  rch_string (str)
-0000f980: 3a20 5468 6520 7374 7269 6e67 2074 6f20  : The string to 
-0000f990: 7365 6172 6368 2066 6f72 2069 6e20 7468  search for in th
-0000f9a0: 6520 6669 6c65 2070 6174 6873 2e0d 0a0d  e file paths....
-0000f9b0: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
-0000f9c0: 6f6e 2074 7261 7665 7273 6573 2074 6865  on traverses the
-0000f9d0: 2073 6f75 7263 6520 6469 7265 6374 6f72   source director
-0000f9e0: 792c 2069 6e63 6c75 6469 6e67 2069 7473  y, including its
-0000f9f0: 2073 7562 6469 7265 6374 6f72 6965 732e   subdirectories.
-0000fa00: 200d 0a20 2020 2046 696c 6573 2077 686f   ..    Files who
-0000fa10: 7365 2070 6174 6873 2063 6f6e 7461 696e  se paths contain
-0000fa20: 2074 6865 2073 6561 7263 6820 7374 7269   the search stri
-0000fa30: 6e67 2061 7265 206d 6f76 6564 2074 6f20  ng are moved to 
-0000fa40: 7468 6520 6465 7374 696e 6174 696f 6e20  the destination 
-0000fa50: 6469 7265 6374 6f72 792e 200d 0a20 2020  directory. ..   
-0000fa60: 2049 6620 6120 6669 6c65 2077 6974 6820   If a file with 
-0000fa70: 7468 6520 7361 6d65 206e 616d 6520 6578  the same name ex
-0000fa80: 6973 7473 2069 6e20 7468 6520 6465 7374  ists in the dest
-0000fa90: 696e 6174 696f 6e2c 2069 7427 7320 7265  ination, it's re
-0000faa0: 6e61 6d65 6420 746f 2061 766f 6964 206f  named to avoid o
-0000fab0: 7665 7277 7269 7469 6e67 2e0d 0a0d 0a20  verwriting..... 
-0000fac0: 2020 2045 7272 6f72 7320 6475 7269 6e67     Errors during
-0000fad0: 2066 696c 6520 6d6f 7665 6d65 6e74 2028   file movement (
-0000fae0: 652e 672e 2c20 7065 726d 6973 7369 6f6e  e.g., permission
-0000faf0: 2069 7373 7565 732c 206e 6f6e 2d65 7869   issues, non-exi
-0000fb00: 7374 656e 7420 6469 7265 6374 6f72 6965  stent directorie
-0000fb10: 7329 2061 7265 206c 6f67 6765 6420 6275  s) are logged bu
-0000fb20: 7420 646f 206e 6f74 2073 746f 7020 7468  t do not stop th
-0000fb30: 6520 7072 6f63 6573 732e 0d0a 2020 2020  e process...    
-0000fb40: 2222 220d 0a0d 0a20 2020 2069 6620 6e6f  """....    if no
-0000fb50: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
-0000fb60: 2873 6f75 7263 655f 6469 7229 3a0d 0a20  (source_dir):.. 
-0000fb70: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0000fb80: 7565 4572 726f 7228 6622 536f 7572 6365  ueError(f"Source
-0000fb90: 2064 6972 6563 746f 7279 2027 7b73 6f75   directory '{sou
-0000fba0: 7263 655f 6469 727d 2720 646f 6573 206e  rce_dir}' does n
-0000fbb0: 6f74 2065 7869 7374 2e22 290d 0a0d 0a20  ot exist.").... 
-0000fbc0: 2020 2023 2043 7265 6174 6520 7468 6520     # Create the 
-0000fbd0: 6465 7374 696e 6174 696f 6e20 6469 7265  destination dire
-0000fbe0: 6374 6f72 7920 6966 2069 7420 646f 6573  ctory if it does
-0000fbf0: 6e27 7420 6578 6973 740d 0a20 2020 2069  n't exist..    i
-0000fc00: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
-0000fc10: 6973 7473 2864 6573 745f 6469 7229 3a0d  ists(dest_dir):.
-0000fc20: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
-0000fc30: 6469 7273 2864 6573 745f 6469 7229 0d0a  dirs(dest_dir)..
-0000fc40: 0d0a 2020 2020 666f 7220 726f 6f74 2c20  ..    for root, 
-0000fc50: 6469 7273 2c20 6669 6c65 7320 696e 206f  dirs, files in o
-0000fc60: 732e 7761 6c6b 2873 6f75 7263 655f 6469  s.walk(source_di
-0000fc70: 7229 3a0d 0a20 2020 2020 2020 2066 6f72  r):..        for
-0000fc80: 2066 696c 6520 696e 2066 696c 6573 3a0d   file in files:.
-0000fc90: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-0000fca0: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
-0000fcb0: 2e6a 6f69 6e28 726f 6f74 2c20 6669 6c65  .join(root, file
-0000fcc0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000fcd0: 6620 7365 6172 6368 5f73 7472 696e 6720  f search_string 
-0000fce0: 696e 2066 696c 655f 7061 7468 3a0d 0a20  in file_path:.. 
-0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000fd00: 6573 745f 6669 6c65 5f70 6174 6820 3d20  est_file_path = 
-0000fd10: 6f73 2e70 6174 682e 6a6f 696e 2864 6573  os.path.join(des
-0000fd20: 745f 6469 722c 2066 696c 6529 0d0a 0d0a  t_dir, file)....
-0000fd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd40: 2320 4368 6563 6b20 6966 2074 6865 2066  # Check if the f
-0000fd50: 696c 6520 616c 7265 6164 7920 6578 6973  ile already exis
-0000fd60: 7473 2069 6e20 6465 7374 696e 6174 696f  ts in destinatio
-0000fd70: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
-0000fd80: 2020 2063 6f75 6e74 6572 203d 2031 0d0a     counter = 1..
-0000fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fda0: 7768 696c 6520 6f73 2e70 6174 682e 6578  while os.path.ex
-0000fdb0: 6973 7473 2864 6573 745f 6669 6c65 5f70  ists(dest_file_p
-0000fdc0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
-0000fdd0: 2020 2020 2020 2020 2020 2023 2053 706c             # Spl
-0000fde0: 6974 2066 696c 656e 616d 6520 616e 6420  it filename and 
-0000fdf0: 6578 7465 6e73 696f 6e0d 0a20 2020 2020  extension..     
-0000fe00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000fe10: 696c 655f 6261 7365 2c20 6669 6c65 5f65  ile_base, file_e
-0000fe20: 7874 656e 7369 6f6e 203d 206f 732e 7061  xtension = os.pa
-0000fe30: 7468 2e73 706c 6974 6578 7428 6669 6c65  th.splitext(file
-0000fe40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000fe50: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-0000fe60: 6120 6e65 7720 6669 6c65 6e61 6d65 2077  a new filename w
-0000fe70: 6974 6820 6120 636f 756e 7465 7220 746f  ith a counter to
-0000fe80: 2061 766f 6964 206f 7665 7277 7269 7469   avoid overwriti
-0000fe90: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
-0000fea0: 2020 2020 2020 2020 6465 7374 5f66 696c          dest_fil
-0000feb0: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
-0000fec0: 2e6a 6f69 6e28 6465 7374 5f64 6972 2c20  .join(dest_dir, 
-0000fed0: 6622 7b66 696c 655f 6261 7365 7d5f 7b63  f"{file_base}_{c
-0000fee0: 6f75 6e74 6572 7d7b 6669 6c65 5f65 7874  ounter}{file_ext
-0000fef0: 656e 7369 6f6e 7d22 290d 0a20 2020 2020  ension}")..     
-0000ff00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000ff10: 6f75 6e74 6572 202b 3d20 310d 0a0d 0a20  ounter += 1.... 
-0000ff20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000ff30: 204d 6f76 6520 7468 6520 6669 6c65 2074   Move the file t
-0000ff40: 6f20 7468 6520 6465 7374 696e 6174 696f  o the destinatio
-0000ff50: 6e20 6469 7265 6374 6f72 790d 0a20 2020  n directory..   
-0000ff60: 2020 2020 2020 2020 2020 2020 2074 7279               try
-0000ff70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0000ff80: 2020 2020 2020 2073 6875 7469 6c2e 6d6f         shutil.mo
-0000ff90: 7665 2866 696c 655f 7061 7468 2c20 6465  ve(file_path, de
-0000ffa0: 7374 5f66 696c 655f 7061 7468 290d 0a20  st_file_path).. 
-0000ffb0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000ffc0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-0000ffd0: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
-0000ffe0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000fff0: 2866 2245 7272 6f72 206d 6f76 696e 6720  (f"Error moving 
-00010000: 6669 6c65 207b 6669 6c65 5f70 6174 687d  file {file_path}
-00010010: 2074 6f20 7b64 6573 745f 6669 6c65 5f70   to {dest_file_p
-00010020: 6174 687d 3a20 7b65 7d22 290d 0a0d 0a23  ath}: {e}")....#
-00010030: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010040: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010050: 2323 2323 2323 2323 2323 2323 0d0a 2354  ############..#T
-00010060: 6869 7320 7061 7274 2069 7320 7374 696c  his part is stil
-00010070: 6c20 756e 6465 7220 636f 6e73 7472 7563  l under construc
-00010080: 7469 6f6e 0d0a 0d0a 696d 706f 7274 206e  tion....import n
-00010090: 756d 7079 2061 7320 6e70 0d0a 0d0a 6465  umpy as np....de
-000100a0: 6620 7061 7274 6961 6c5f 6465 7269 7661  f partial_deriva
-000100b0: 7469 7665 2866 2c20 6478 2c20 6479 293a  tive(f, dx, dy):
-000100c0: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
-000100d0: 616c 6375 6c61 7465 2074 6865 2063 656e  alculate the cen
-000100e0: 7472 616c 2064 6966 6665 7265 6e63 6520  tral difference 
-000100f0: 6170 7072 6f78 696d 6174 696f 6e20 666f  approximation fo
-00010100: 7220 7468 6520 7061 7274 6961 6c20 6465  r the partial de
-00010110: 7269 7661 7469 7665 730d 0a20 2020 206f  rivatives..    o
-00010120: 6620 6120 3244 2066 756e 6374 696f 6e20  f a 2D function 
-00010130: 7769 7468 2072 6573 7065 6374 2074 6f20  with respect to 
-00010140: 7820 616e 6420 792e 0d0a 0d0a 2020 2020  x and y.....    
-00010150: 3a70 6172 616d 2066 3a20 3244 206e 756d  :param f: 2D num
-00010160: 7079 2061 7272 6179 206f 6620 6675 6e63  py array of func
-00010170: 7469 6f6e 2076 616c 7565 732c 2072 6570  tion values, rep
-00010180: 7265 7365 6e74 696e 6720 7468 6520 7261  resenting the ra
-00010190: 7374 6572 0d0a 2020 2020 3a70 6172 616d  ster..    :param
-000101a0: 2064 783a 2053 7061 6369 6e67 2069 6e20   dx: Spacing in 
-000101b0: 7468 6520 782d 6469 7265 6374 696f 6e20  the x-direction 
-000101c0: 2861 7373 756d 6564 2074 6f20 6265 2063  (assumed to be c
-000101d0: 6f6e 7374 616e 7429 0d0a 2020 2020 3a70  onstant)..    :p
-000101e0: 6172 616d 2064 793a 2053 7061 6369 6e67  aram dy: Spacing
-000101f0: 2069 6e20 7468 6520 792d 6469 7265 6374   in the y-direct
-00010200: 696f 6e20 2861 7373 756d 6564 2074 6f20  ion (assumed to 
-00010210: 6265 2063 6f6e 7374 616e 7429 0d0a 2020  be constant)..  
-00010220: 2020 3a72 6574 7572 6e3a 2054 776f 2032    :return: Two 2
-00010230: 4420 6e75 6d70 7920 6172 7261 7973 2c20  D numpy arrays, 
-00010240: 6f6e 6520 666f 7220 7468 6520 7061 7274  one for the part
-00010250: 6961 6c20 6465 7269 7661 7469 7665 2077  ial derivative w
-00010260: 6974 6820 7265 7370 6563 7420 746f 2078  ith respect to x
-00010270: 2028 6466 5f64 7829 0d0a 2020 2020 2020   (df_dx)..      
-00010280: 2020 2020 2020 2061 6e64 206f 6e65 2066         and one f
-00010290: 6f72 2074 6865 2070 6172 7469 616c 2064  or the partial d
-000102a0: 6572 6976 6174 6976 6520 7769 7468 2072  erivative with r
-000102b0: 6573 7065 6374 2074 6f20 7920 2864 665f  espect to y (df_
-000102c0: 6479 290d 0a20 2020 2022 2222 0d0a 2020  dy)..    """..  
-000102d0: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
-000102e0: 6172 7261 7973 2074 6f20 7374 6f72 6520  arrays to store 
-000102f0: 7468 6520 7061 7274 6961 6c20 6465 7269  the partial deri
-00010300: 7661 7469 7665 730d 0a20 2020 2064 665f  vatives..    df_
-00010310: 6478 203d 206e 702e 7a65 726f 735f 6c69  dx = np.zeros_li
-00010320: 6b65 2866 290d 0a20 2020 2064 665f 6479  ke(f)..    df_dy
-00010330: 203d 206e 702e 7a65 726f 735f 6c69 6b65   = np.zeros_like
-00010340: 2866 290d 0a0d 0a20 2020 2023 2043 6f6d  (f)....    # Com
-00010350: 7075 7465 2074 6865 2070 6172 7469 616c  pute the partial
-00010360: 2064 6572 6976 6174 6976 6573 2066 6f72   derivatives for
-00010370: 2074 6865 2069 6e74 6572 6e61 6c20 706f   the internal po
-00010380: 696e 7473 0d0a 2020 2020 666f 7220 7869  ints..    for xi
-00010390: 2069 6e20 7261 6e67 6528 312c 2066 2e73   in range(1, f.s
-000103a0: 6861 7065 5b30 5d20 2d20 3129 3a0d 0a20  hape[0] - 1):.. 
-000103b0: 2020 2020 2020 2066 6f72 2079 6a20 696e         for yj in
-000103c0: 2072 616e 6765 2831 2c20 662e 7368 6170   range(1, f.shap
-000103d0: 655b 315d 202d 2031 293a 0d0a 2020 2020  e[1] - 1):..    
-000103e0: 2020 2020 2020 2020 6466 5f64 785b 7869          df_dx[xi
-000103f0: 2c20 796a 5d20 3d20 2866 5b78 6920 2b20  , yj] = (f[xi + 
-00010400: 312c 2079 6a5d 202d 2066 5b78 6920 2d20  1, yj] - f[xi - 
-00010410: 312c 2079 6a5d 2920 2f20 2832 202a 2064  1, yj]) / (2 * d
-00010420: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
-00010430: 6466 5f64 795b 7869 2c20 796a 5d20 3d20  df_dy[xi, yj] = 
-00010440: 2866 5b78 692c 2079 6a20 2b20 315d 202d  (f[xi, yj + 1] -
-00010450: 2066 5b78 692c 2079 6a20 2d20 315d 2920   f[xi, yj - 1]) 
-00010460: 2f20 2832 202a 2064 7929 0d0a 0d0a 2020  / (2 * dy)....  
-00010470: 2020 2320 4861 6e64 6c65 2074 6865 2062    # Handle the b
-00010480: 6f75 6e64 6172 6965 7320 6279 2073 6574  oundaries by set
-00010490: 7469 6e67 2074 6865 2064 6572 6976 6174  ting the derivat
-000104a0: 6976 6520 746f 207a 6572 6f20 6f72 2075  ive to zero or u
-000104b0: 7369 6e67 206f 6e65 2d73 6964 6564 2064  sing one-sided d
-000104c0: 6966 6665 7265 6e63 6573 0d0a 2020 2020  ifferences..    
-000104d0: 2320 4865 7265 2077 6520 6368 6f6f 7365  # Here we choose
-000104e0: 2074 6f20 7365 7420 7468 6520 626f 756e   to set the boun
-000104f0: 6461 7279 2064 6572 6976 6174 6976 6520  dary derivative 
-00010500: 746f 207a 6572 6f0d 0a20 2020 2023 2041  to zero..    # A
-00010510: 6c74 6572 6e61 7469 7665 6c79 2c20 7573  lternatively, us
-00010520: 6520 666f 7277 6172 642f 6261 636b 7761  e forward/backwa
-00010530: 7264 2064 6966 6665 7265 6e63 6520 6174  rd difference at
-00010540: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
-00010550: 6966 206e 6565 6465 640d 0a0d 0a20 2020  if needed....   
-00010560: 2072 6574 7572 6e20 6466 5f64 782c 2064   return df_dx, d
-00010570: 665f 6479 0d0a 0d0a 0d0a 696d 706f 7274  f_dy......import
-00010580: 206e 756d 7079 2061 7320 6e70 0d0a 696d   numpy as np..im
-00010590: 706f 7274 2072 6173 7465 7269 6f0d 0a0d  port rasterio...
-000105a0: 0a64 6566 2063 616c 6375 6c61 7465 5f73  .def calculate_s
-000105b0: 6c6f 7065 2864 656d 2c20 6173 7065 6374  lope(dem, aspect
-000105c0: 2c20 6478 202c 2064 7929 3a0d 0a20 2020  , dx , dy):..   
-000105d0: 2022 2222 0d0a 2020 2020 4361 6c63 756c   """..    Calcul
-000105e0: 6174 6520 7468 6520 736c 6f70 6520 6174  ate the slope at
-000105f0: 2065 6163 6820 7069 7865 6c20 7573 696e   each pixel usin
-00010600: 6720 7468 6520 6173 7065 6374 2074 6f20  g the aspect to 
-00010610: 6465 7465 726d 696e 6520 6469 7265 6374  determine direct
-00010620: 696f 6e2e 0d0a 0d0a 2020 2020 5061 7261  ion.....    Para
-00010630: 6d65 7465 7273 3a0d 0a20 2020 2064 656d  meters:..    dem
-00010640: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-00010650: 3a20 4469 6769 7461 6c20 456c 6576 6174  : Digital Elevat
-00010660: 696f 6e20 4d6f 6465 6c20 2844 454d 2920  ion Model (DEM) 
-00010670: 6172 7261 792e 0d0a 2020 2020 6173 7065  array...    aspe
-00010680: 6374 2028 6e75 6d70 792e 6e64 6172 7261  ct (numpy.ndarra
-00010690: 7929 3a20 4173 7065 6374 2061 7272 6179  y): Aspect array
-000106a0: 2e0d 0a20 2020 2064 7820 2866 6c6f 6174  ...    dx (float
-000106b0: 293a 2020 7820 5370 6174 6961 6c20 7265  ):  x Spatial re
-000106c0: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
-000106d0: 7261 7374 6572 2028 6469 7374 616e 6365  raster (distance
-000106e0: 2062 6574 7765 656e 2070 6978 656c 7329   between pixels)
-000106f0: 2e0d 0a20 2020 2064 7920 2866 6c6f 6174  ...    dy (float
-00010700: 293a 2020 7920 5370 6174 6961 6c20 7265  ):  y Spatial re
-00010710: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
-00010720: 7261 7374 6572 2028 6469 7374 616e 6365  raster (distance
-00010730: 2062 6574 7765 656e 2070 6978 656c 7329   between pixels)
-00010740: 2e0d 0a0d 0a20 2020 2052 6574 7572 6e73  .....    Returns
-00010750: 3a0d 0a20 2020 206e 756d 7079 2e6e 6461  :..    numpy.nda
-00010760: 7272 6179 3a20 4172 7261 7920 6f66 2073  rray: Array of s
-00010770: 6c6f 7065 2076 616c 7565 7320 696e 2064  lope values in d
-00010780: 6567 7265 6573 2e0d 0a20 2020 2022 2222  egrees...    """
-00010790: 0d0a 2020 2020 0d0a 2020 2020 2320 6772  ..    ..    # gr
-000107a0: 6164 5f79 2c20 6772 6164 5f78 203d 206e  ad_y, grad_x = n
-000107b0: 702e 6772 6164 6965 6e74 2864 656d 2c20  p.gradient(dem, 
-000107c0: 6478 2c20 6479 290d 0a20 2020 200d 0a20  dx, dy)..    .. 
-000107d0: 2020 200d 0a20 2020 2023 2041 7373 756d     ..    # Assum
-000107e0: 696e 6720 2764 656d 2720 616e 6420 2761  ing 'dem' and 'a
-000107f0: 7370 6563 7427 2061 7265 2079 6f75 7220  spect' are your 
-00010800: 6578 6973 7469 6e67 206e 756d 7079 2061  existing numpy a
-00010810: 7272 6179 730d 0a20 2020 2023 2043 6865  rrays..    # Che
-00010820: 636b 2069 6620 7468 6520 7368 6170 6573  ck if the shapes
-00010830: 2061 7265 2064 6966 6665 7265 6e74 0d0a   are different..
-00010840: 2020 2020 2320 6966 2064 656d 2e73 6861      # if dem.sha
-00010850: 7065 2021 3d20 6173 7065 6374 2e73 6861  pe != aspect.sha
-00010860: 7065 3a0d 0a20 2020 2023 2020 2020 2023  pe:..    #     #
-00010870: 2052 6573 697a 6520 2764 656d 2720 746f   Resize 'dem' to
-00010880: 206d 6174 6368 2074 6865 2073 6861 7065   match the shape
-00010890: 206f 6620 2761 7370 6563 7427 0d0a 2020   of 'aspect'..  
-000108a0: 2020 2320 2020 2020 6173 7065 6374 203d    #     aspect =
-000108b0: 206e 702e 7265 7369 7a65 2861 7370 6563   np.resize(aspec
-000108c0: 742c 2064 656d 2e73 6861 7065 290d 0a20  t, dem.shape).. 
-000108d0: 2020 2023 2065 6c73 653a 0d0a 2020 2020     # else:..    
-000108e0: 2320 2020 2020 6173 7065 6374 203d 2061  #     aspect = a
-000108f0: 7370 6563 740d 0a0d 0a0d 0a0d 0a20 2020  spect........   
-00010900: 2067 7261 645f 792c 2067 7261 645f 7820   grad_y, grad_x 
-00010910: 3d20 6e70 2e67 7261 6469 656e 7428 6465  = np.gradient(de
-00010920: 6d2c 2064 782c 2064 7929 0d0a 2020 2020  m, dx, dy)..    
-00010930: 2367 7261 645f 792c 2067 7261 645f 783d  #grad_y, grad_x=
-00010940: 7061 7274 6961 6c5f 6465 7269 7661 7469  partial_derivati
-00010950: 7665 2864 656d 2c20 6478 2c20 6479 290d  ve(dem, dx, dy).
-00010960: 0a0d 0a20 2020 2069 6620 6772 6164 5f78  ...    if grad_x
-00010970: 2e73 6861 7065 2021 3d20 6772 6164 5f79  .shape != grad_y
-00010980: 2e73 6861 7065 3a0d 0a20 2020 2020 2020  .shape:..       
-00010990: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-000109a0: 7228 2247 7261 6469 656e 7420 6172 7261  r("Gradient arra
-000109b0: 7973 2068 6176 6520 6d69 736d 6174 6368  ys have mismatch
-000109c0: 6564 2073 6861 7065 732e 2229 0d0a 2020  ed shapes.")..  
-000109d0: 2020 0d0a 2020 2020 6173 7065 6374 5f72    ..    aspect_r
-000109e0: 6164 6961 6e73 203d 206e 702e 6465 6732  adians = np.deg2
-000109f0: 7261 6428 6173 7065 6374 290d 0a20 2020  rad(aspect)..   
-00010a00: 2064 6972 6563 7469 6f6e 616c 5f67 7261   directional_gra
-00010a10: 6420 3d20 6e70 2e63 6f73 2861 7370 6563  d = np.cos(aspec
-00010a20: 745f 7261 6469 616e 7329 202a 2067 7261  t_radians) * gra
-00010a30: 645f 7820 2b20 6e70 2e73 696e 2861 7370  d_x + np.sin(asp
-00010a40: 6563 745f 7261 6469 616e 7329 202a 2067  ect_radians) * g
-00010a50: 7261 645f 790d 0a20 2020 2023 736c 6f70  rad_y..    #slop
-00010a60: 655f 6465 6772 6565 7320 3d20 6e70 2e72  e_degrees = np.r
-00010a70: 6164 3264 6567 286e 702e 6172 6374 616e  ad2deg(np.arctan
-00010a80: 2864 6972 6563 7469 6f6e 616c 5f67 7261  (directional_gra
-00010a90: 6429 290d 0a20 2020 0d0a 2020 2020 2320  d))..   ..    # 
-00010aa0: 4361 6c63 756c 6174 6520 736c 6f70 6520  Calculate slope 
-00010ab0: 696e 2072 6164 6961 6e73 0d0a 2020 2020  in radians..    
-00010ac0: 736c 6f70 655f 7261 6469 616e 7320 3d20  slope_radians = 
-00010ad0: 6e70 2e61 7263 7461 6e28 6469 7265 6374  np.arctan(direct
-00010ae0: 696f 6e61 6c5f 6772 6164 290d 0a0d 0a20  ional_grad).... 
-00010af0: 2020 2023 2045 6e73 7572 6520 736c 6f70     # Ensure slop
-00010b00: 6520 6973 2077 6974 6869 6e20 3020 746f  e is within 0 to
-00010b10: 20cf 802f 3220 7261 6469 616e 7320 2830   ../2 radians (0
-00010b20: 2074 6f20 3930 2064 6567 7265 6573 2920   to 90 degrees) 
-00010b30: 7261 6e67 650d 0a20 2020 2023 736c 6f70  range..    #slop
-00010b40: 655f 7261 6469 616e 7320 3d20 736c 6f70  e_radians = slop
-00010b50: 655f 7261 6469 616e 7320 2520 286e 702e  e_radians % (np.
-00010b60: 7069 202f 2032 290d 0a0d 0a20 2020 2023  pi / 2)....    #
-00010b70: 2043 6f6e 7665 7274 2073 6c6f 7065 2074   Convert slope t
-00010b80: 6f20 6465 6772 6565 730d 0a20 2020 2073  o degrees..    s
-00010b90: 6c6f 7065 5f64 6567 7265 6573 203d 2028  lope_degrees = (
-00010ba0: 6e70 2e72 6164 3264 6567 2873 6c6f 7065  np.rad2deg(slope
-00010bb0: 5f72 6164 6961 6e73 2929 2025 2039 3020  _radians)) % 90 
-00010bc0: 0d0a 2020 2020 2373 6c6f 7065 5f64 6567  ..    #slope_deg
-00010bd0: 7265 6573 3d20 2831 3335 2d73 6c6f 7065  rees= (135-slope
-00010be0: 5f64 6567 7265 6573 2925 2039 3020 0d0a  _degrees)% 90 ..
-00010bf0: 2020 2020 0d0a 2020 200d 0a20 2020 200d      ..   ..    .
-00010c00: 0a20 2020 2072 6574 7572 6e20 736c 6f70  .    return slop
-00010c10: 655f 6465 6772 6565 732c 2064 6972 6563  e_degrees, direc
-00010c20: 7469 6f6e 616c 5f67 7261 640d 0a0d 0a64  tional_grad....d
-00010c30: 6566 2063 616c 6375 6c61 7465 5f68 6569  ef calculate_hei
-00010c40: 6768 745f 6368 616e 6765 2873 6c6f 7065  ght_change(slope
-00010c50: 2c20 6469 7374 616e 6365 2c20 6465 6d29  , distance, dem)
-00010c60: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00010c70: 4361 6c63 756c 6174 6520 7468 6520 6865  Calculate the he
-00010c80: 6967 6874 2063 6861 6e67 6520 7573 696e  ight change usin
-00010c90: 6720 7468 6520 736c 6f70 6520 616e 6420  g the slope and 
-00010ca0: 6469 7374 616e 6365 2066 6f72 2065 6163  distance for eac
-00010cb0: 6820 7069 7865 6c2e 0d0a 0d0a 2020 2020  h pixel.....    
-00010cc0: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
-00010cd0: 2073 6c6f 7065 2028 6e75 6d70 792e 6e64   slope (numpy.nd
-00010ce0: 6172 7261 7929 3a20 4172 7261 7920 6f66  array): Array of
-00010cf0: 2073 6c6f 7065 2076 616c 7565 7320 696e   slope values in
-00010d00: 2064 6567 7265 6573 2e0d 0a20 2020 2064   degrees...    d
-00010d10: 6973 7461 6e63 6520 286e 756d 7079 2e6e  istance (numpy.n
-00010d20: 6461 7272 6179 293a 2041 7272 6179 206f  darray): Array o
-00010d30: 6620 6469 7374 616e 6365 2076 616c 7565  f distance value
-00010d40: 732e 0d0a 0d0a 2020 2020 5265 7475 726e  s.....    Return
-00010d50: 733a 0d0a 2020 2020 6e75 6d70 792e 6e64  s:..    numpy.nd
-00010d60: 6172 7261 793a 2041 7272 6179 206f 6620  array: Array of 
-00010d70: 6865 6967 6874 2063 6861 6e67 6573 2e0d  height changes..
-00010d80: 0a20 2020 2022 2222 0d0a 2020 2020 736c  .    """..    sl
-00010d90: 6f70 655f 7261 6469 616e 7320 3d20 6e70  ope_radians = np
-00010da0: 2e64 6567 3272 6164 2873 6c6f 7065 290d  .deg2rad(slope).
-00010db0: 0a20 2020 2068 6569 6768 745f 6368 616e  .    height_chan
-00010dc0: 6765 203d 206e 702e 7461 6e28 736c 6f70  ge = np.tan(slop
-00010dd0: 655f 7261 6469 616e 7329 202a 2064 6973  e_radians) * dis
-00010de0: 7461 6e63 650d 0a20 2020 200d 0a20 2020  tance..    ..   
-00010df0: 200d 0a20 2020 200d 0a20 2020 2072 6574   ..    ..    ret
-00010e00: 7572 6e20 6865 6967 6874 5f63 6861 6e67  urn height_chang
-00010e10: 6520 0d0a 0d0a 6465 6620 6361 6c63 756c  e ....def calcul
-00010e20: 6174 655f 766f 6c75 6d65 5f63 6861 6e67  ate_volume_chang
-00010e30: 6528 6865 6967 6874 5f63 6861 6e67 652c  e(height_change,
-00010e40: 2070 6978 656c 5f61 7265 6129 3a0d 0a20   pixel_area):.. 
-00010e50: 2020 2022 2222 0d0a 2020 2020 4361 6c63     """..    Calc
-00010e60: 756c 6174 6520 7468 6520 766f 6c75 6d65  ulate the volume
-00010e70: 2063 6861 6e67 6520 666f 7220 6561 6368   change for each
-00010e80: 2070 6978 656c 2e0d 0a0d 0a20 2020 2050   pixel.....    P
-00010e90: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
-00010ea0: 6865 6967 6874 5f63 6861 6e67 6520 286e  height_change (n
-00010eb0: 756d 7079 2e6e 6461 7272 6179 293a 2041  umpy.ndarray): A
-00010ec0: 7272 6179 206f 6620 6865 6967 6874 2063  rray of height c
-00010ed0: 6861 6e67 6573 2e0d 0a20 2020 2070 6978  hanges...    pix
-00010ee0: 656c 5f61 7265 6120 2866 6c6f 6174 293a  el_area (float):
-00010ef0: 2041 7265 6120 6f66 2061 2073 696e 676c   Area of a singl
-00010f00: 6520 7069 7865 6c2e 0d0a 2020 2020 0d0a  e pixel...    ..
-00010f10: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
-00010f20: 2020 6e75 6d70 792e 6e64 6172 7261 793a    numpy.ndarray:
-00010f30: 2041 7272 6179 206f 6620 766f 6c75 6d65   Array of volume
-00010f40: 2063 6861 6e67 6573 2e0d 0a20 2020 2022   changes...    "
-00010f50: 2222 0d0a 2020 2020 766f 6c75 6d65 5f63  ""..    volume_c
-00010f60: 6861 6e67 6520 3d20 6865 6967 6874 5f63  hange = height_c
-00010f70: 6861 6e67 6520 2a20 7069 7865 6c5f 6172  hange * pixel_ar
-00010f80: 6561 0d0a 2020 2020 7072 696e 7420 2866  ea..    print (f
-00010f90: 2754 6f74 616c 2056 6f6c 756d 653a 207b  'Total Volume: {
-00010fa0: 6e70 2e6e 616e 7375 6d28 766f 6c75 6d65  np.nansum(volume
-00010fb0: 5f63 6861 6e67 6529 7d20 6375 6269 6320  _change)} cubic 
-00010fc0: 6d65 7465 7227 290d 0a20 2020 2072 6574  meter')..    ret
-00010fd0: 7572 6e20 766f 6c75 6d65 5f63 6861 6e67  urn volume_chang
-00010fe0: 650d 0a0d 0a66 726f 6d20 736b 696d 6167  e....from skimag
-00010ff0: 652e 6669 6c74 6572 7320 696d 706f 7274  e.filters import
-00011000: 2067 6175 7373 6961 6e0d 0a0d 0a64 6566   gaussian....def
-00011010: 2064 6973 706c 6163 656d 656e 745f 746f   displacement_to
-00011020: 5f76 6f6c 756d 6528 6465 6d5f 7061 7468  _volume(dem_path
-00011030: 3d22 222c 2061 7370 6563 745f 7061 7468  ="", aspect_path
-00011040: 3d22 222c 2064 6973 706c 6163 656d 656e  ="", displacemen
-00011050: 745f 7061 7468 3d22 222c 2073 6c6f 7065  t_path="", slope
-00011060: 5f6f 7574 7075 745f 7061 7468 3d22 222c  _output_path="",
-00011070: 2068 6569 6768 745f 6f75 7470 7574 5f70   height_output_p
-00011080: 6174 683d 2222 2c20 766f 6c75 6d65 5f6f  ath="", volume_o
-00011090: 7574 7075 745f 7061 7468 3d22 222c 2064  utput_path="", d
-000110a0: 783d 4e6f 6e65 202c 2064 793d 4e6f 6e65  x=None , dy=None
-000110b0: 202c 2070 6978 656c 5f61 7265 613d 4e6f   , pixel_area=No
-000110c0: 6e65 293a 0d0a 2020 2020 2222 220d 0a20  ne):..    """.. 
-000110d0: 2020 2050 726f 6365 7373 2074 6865 2044     Process the D
-000110e0: 454d 2c20 6173 7065 6374 2c20 616e 6420  EM, aspect, and 
-000110f0: 6469 7370 6c61 6365 6d65 6e74 2072 6173  displacement ras
-00011100: 7465 7273 2074 6f20 6361 6c63 756c 6174  ters to calculat
-00011110: 6520 616e 6420 6578 706f 7274 2074 6865  e and export the
-00011120: 2073 6c6f 7065 2c20 6865 6967 6874 2063   slope, height c
-00011130: 6861 6e67 652c 2061 6e64 2076 6f6c 756d  hange, and volum
-00011140: 6520 6368 616e 6765 2e0d 0a0d 0a20 2020  e change.....   
-00011150: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-00011160: 2020 6465 6d5f 7061 7468 2028 7374 7229    dem_path (str)
-00011170: 3a20 5061 7468 2074 6f20 7468 6520 4445  : Path to the DE
-00011180: 4d20 7261 7374 6572 2066 696c 652e 0d0a  M raster file...
-00011190: 2020 2020 6173 7065 6374 5f70 6174 6820      aspect_path 
-000111a0: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
-000111b0: 6865 2061 7370 6563 7420 7261 7374 6572  he aspect raster
-000111c0: 2066 696c 652e 0d0a 2020 2020 6469 7370   file...    disp
-000111d0: 6c61 6365 6d65 6e74 5f70 6174 6820 2873  lacement_path (s
-000111e0: 7472 293a 2050 6174 6820 746f 2074 6865  tr): Path to the
-000111f0: 2064 6973 706c 6163 656d 656e 7420 7261   displacement ra
-00011200: 7374 6572 2066 696c 652e 0d0a 2020 2020  ster file...    
-00011210: 736c 6f70 655f 6f75 7470 7574 5f70 6174  slope_output_pat
-00011220: 6820 2873 7472 293a 2050 6174 6820 666f  h (str): Path fo
-00011230: 7220 7468 6520 736c 6f70 6520 6f75 7470  r the slope outp
-00011240: 7574 2047 656f 5449 4646 2066 696c 652e  ut GeoTIFF file.
-00011250: 0d0a 2020 2020 6865 6967 6874 5f6f 7574  ..    height_out
-00011260: 7075 745f 7061 7468 2028 7374 7229 3a20  put_path (str): 
-00011270: 5061 7468 2066 6f72 2074 6865 2068 6569  Path for the hei
-00011280: 6768 7420 6368 616e 6765 206f 7574 7075  ght change outpu
-00011290: 7420 4765 6f54 4946 4620 6669 6c65 2e0d  t GeoTIFF file..
-000112a0: 0a20 2020 2076 6f6c 756d 655f 6f75 7470  .    volume_outp
-000112b0: 7574 5f70 6174 6820 2873 7472 293a 2050  ut_path (str): P
-000112c0: 6174 6820 666f 7220 7468 6520 766f 6c75  ath for the volu
-000112d0: 6d65 2063 6861 6e67 6520 6f75 7470 7574  me change output
-000112e0: 2047 656f 5449 4646 2066 696c 652e 0d0a   GeoTIFF file...
-000112f0: 2020 2020 6478 2028 666c 6f61 7429 3a20      dx (float): 
-00011300: 2078 2053 7061 7469 616c 2072 6573 6f6c   x Spatial resol
-00011310: 7574 696f 6e20 6f66 2074 6865 2072 6173  ution of the ras
-00011320: 7465 7220 2864 6973 7461 6e63 6520 6265  ter (distance be
-00011330: 7477 6565 6e20 7069 7865 6c73 292e 0d0a  tween pixels)...
-00011340: 2020 2020 6479 2028 666c 6f61 7429 3a20      dy (float): 
-00011350: 2079 2053 7061 7469 616c 2072 6573 6f6c   y Spatial resol
-00011360: 7574 696f 6e20 6f66 2074 6865 2072 6173  ution of the ras
-00011370: 7465 7220 2864 6973 7461 6e63 6520 6265  ter (distance be
-00011380: 7477 6565 6e20 7069 7865 6c73 292e 0d0a  tween pixels)...
-00011390: 2020 2020 7069 7865 6c5f 6172 6561 2028      pixel_area (
-000113a0: 666c 6f61 7429 3a20 4172 6561 206f 6620  float): Area of 
-000113b0: 6120 7369 6e67 6c65 2070 6978 656c 2e0d  a single pixel..
-000113c0: 0a0d 0a20 2020 2052 6574 7572 6e73 3a0d  ...    Returns:.
-000113d0: 0a20 2020 204e 6f6e 653a 204f 7574 7075  .    None: Outpu
-000113e0: 7473 2047 656f 5449 4646 2066 696c 6573  ts GeoTIFF files
-000113f0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
-00011400: 6420 6f75 7470 7574 2070 6174 6873 2e0d  d output paths..
-00011410: 0a20 2020 2022 2222 0d0a 2020 2020 7769  .    """..    wi
-00011420: 7468 2072 6173 7465 7269 6f2e 6f70 656e  th rasterio.open
-00011430: 2864 656d 5f70 6174 6829 2061 7320 6465  (dem_path) as de
-00011440: 6d5f 7261 7374 6572 2c20 5c0d 0a20 2020  m_raster, \..   
-00011450: 2020 2020 2020 7261 7374 6572 696f 2e6f        rasterio.o
-00011460: 7065 6e28 6173 7065 6374 5f70 6174 6829  pen(aspect_path)
-00011470: 2061 7320 6173 7065 6374 5f72 6173 7465   as aspect_raste
-00011480: 722c 205c 0d0a 2020 2020 2020 2020 2072  r, \..         r
-00011490: 6173 7465 7269 6f2e 6f70 656e 2864 6973  asterio.open(dis
-000114a0: 706c 6163 656d 656e 745f 7061 7468 2920  placement_path) 
-000114b0: 6173 2064 6973 706c 6163 656d 656e 745f  as displacement_
-000114c0: 7261 7374 6572 3a0d 0a0d 0a20 2020 2020  raster:....     
-000114d0: 2020 2064 656d 203d 2064 656d 5f72 6173     dem = dem_ras
-000114e0: 7465 722e 7265 6164 2831 2c20 206d 6173  ter.read(1,  mas
-000114f0: 6b65 643d 5472 7565 290d 0a20 2020 2020  ked=True)..     
-00011500: 2020 2061 7370 6563 7420 3d20 6173 7065     aspect = aspe
-00011510: 6374 5f72 6173 7465 722e 7265 6164 2831  ct_raster.read(1
-00011520: 2c20 206d 6173 6b65 643d 5472 7565 290d  ,  masked=True).
-00011530: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
-00011540: 656d 656e 7420 3d20 6469 7370 6c61 6365  ement = displace
-00011550: 6d65 6e74 5f72 6173 7465 722e 7265 6164  ment_raster.read
-00011560: 2831 2c20 206d 6173 6b65 643d 5472 7565  (1,  masked=True
-00011570: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00011580: 2020 2020 2078 5f72 6573 6f6c 7574 696f       x_resolutio
-00011590: 6e2c 2079 5f72 6573 6f6c 7574 696f 6e20  n, y_resolution 
-000115a0: 3d20 6469 7370 6c61 6365 6d65 6e74 5f72  = displacement_r
-000115b0: 6173 7465 722e 7265 730d 0a20 2020 2020  aster.res..     
-000115c0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-000115d0: 6478 2069 7320 4e6f 6e65 3a0d 0a20 2020  dx is None:..   
-000115e0: 2020 2020 2020 2020 2064 783d 785f 7265           dx=x_re
-000115f0: 736f 6c75 7469 6f6e 0d0a 2020 2020 2020  solution..      
-00011600: 2020 6966 2064 7920 6973 204e 6f6e 653a    if dy is None:
-00011610: 0d0a 2020 2020 2020 2020 2020 2020 6479  ..            dy
-00011620: 3d79 5f72 6573 6f6c 7574 696f 6e0d 0a20  =y_resolution.. 
-00011630: 2020 2020 2020 2069 6620 7069 7865 6c5f         if pixel_
-00011640: 6172 6561 2069 7320 4e6f 6e65 3a0d 0a20  area is None:.. 
-00011650: 2020 2020 2020 2020 2020 2070 6978 656c             pixel
-00011660: 5f61 7265 613d 6478 202a 2064 790d 0a20  _area=dx * dy.. 
-00011670: 2020 2020 2020 2066 726f 6d20 7363 6970         from scip
-00011680: 792e 6e64 696d 6167 6520 696d 706f 7274  y.ndimage import
-00011690: 207a 6f6f 6d0d 0a0d 0a20 2020 2020 2020   zoom....       
-000116a0: 2023 2045 7861 6d70 6c65 2064 696d 656e   # Example dimen
-000116b0: 7369 6f6e 7320 2d20 7265 706c 6163 6520  sions - replace 
-000116c0: 7468 6573 6520 7769 7468 2061 6374 7561  these with actua
-000116d0: 6c20 6469 6d65 6e73 696f 6e73 0d0a 2020  l dimensions..  
-000116e0: 2020 2020 2020 6465 6d5f 7368 6170 6520        dem_shape 
-000116f0: 3d20 6465 6d2e 7368 6170 650d 0a20 2020  = dem.shape..   
-00011700: 2020 2020 2061 7370 6563 745f 7368 6170       aspect_shap
-00011710: 6520 3d20 6173 7065 6374 2e73 6861 7065  e = aspect.shape
-00011720: 0d0a 2020 2020 2020 2020 6469 7370 6c61  ..        displa
-00011730: 6365 6d65 6e74 5f73 6861 7065 203d 2064  cement_shape = d
-00011740: 6973 706c 6163 656d 656e 742e 7368 6170  isplacement.shap
-00011750: 650d 0a0d 0a20 2020 2020 2020 2023 2043  e....        # C
-00011760: 616c 6375 6c61 7469 6e67 207a 6f6f 6d20  alculating zoom 
-00011770: 6661 6374 6f72 730d 0a20 2020 2020 2020  factors..       
-00011780: 207a 6f6f 6d5f 6661 6374 6f72 5f61 7370   zoom_factor_asp
-00011790: 6563 7420 3d20 5b64 656d 5f64 696d 202f  ect = [dem_dim /
-000117a0: 2061 7370 6563 745f 6469 6d20 666f 7220   aspect_dim for 
-000117b0: 6465 6d5f 6469 6d2c 2061 7370 6563 745f  dem_dim, aspect_
-000117c0: 6469 6d20 696e 207a 6970 2864 656d 5f73  dim in zip(dem_s
-000117d0: 6861 7065 2c20 6173 7065 6374 5f73 6861  hape, aspect_sha
-000117e0: 7065 295d 0d0a 2020 2020 2020 2020 7a6f  pe)]..        zo
-000117f0: 6f6d 5f66 6163 746f 725f 6469 7370 6c61  om_factor_displa
-00011800: 6365 6d65 6e74 203d 205b 6465 6d5f 6469  cement = [dem_di
-00011810: 6d20 2f20 6469 7370 6c61 6365 6d65 6e74  m / displacement
-00011820: 5f64 696d 2066 6f72 2064 656d 5f64 696d  _dim for dem_dim
-00011830: 2c20 6469 7370 6c61 6365 6d65 6e74 5f64  , displacement_d
-00011840: 696d 2069 6e20 7a69 7028 6465 6d5f 7368  im in zip(dem_sh
-00011850: 6170 652c 2064 6973 706c 6163 656d 656e  ape, displacemen
-00011860: 745f 7368 6170 6529 5d0d 0a0d 0a20 2020  t_shape)]....   
-00011870: 2020 2020 2023 2052 6573 697a 696e 6720       # Resizing 
-00011880: 6173 7065 6374 2061 6e64 2064 6973 706c  aspect and displ
-00011890: 6163 656d 656e 7420 6172 7261 7973 0d0a  acement arrays..
-000118a0: 2020 2020 2020 2020 6173 7065 6374 203d          aspect =
-000118b0: 207a 6f6f 6d28 6173 7065 6374 2c20 7a6f   zoom(aspect, zo
-000118c0: 6f6d 5f66 6163 746f 725f 6173 7065 6374  om_factor_aspect
-000118d0: 2c20 6f72 6465 723d 3129 2020 2320 6375  , order=1)  # cu
-000118e0: 6269 6320 696e 7465 7270 6f6c 6174 696f  bic interpolatio
-000118f0: 6e0d 0a20 2020 2020 2020 2064 6973 706c  n..        displ
-00011900: 6163 656d 656e 7420 3d20 7a6f 6f6d 2864  acement = zoom(d
-00011910: 6973 706c 6163 656d 656e 742c 207a 6f6f  isplacement, zoo
-00011920: 6d5f 6661 6374 6f72 5f64 6973 706c 6163  m_factor_displac
-00011930: 656d 656e 742c 206f 7264 6572 3d31 2920  ement, order=1) 
-00011940: 2023 2063 7562 6963 2069 6e74 6572 706f   # cubic interpo
-00011950: 6c61 7469 6f6e 0d0a 2020 2020 2020 2020  lation..        
-00011960: 0d0a 2020 2020 2020 2020 2320 6173 7065  ..        # aspe
-00011970: 6374 203d 206e 702e 7265 7369 7a65 2861  ct = np.resize(a
-00011980: 7370 6563 742c 2064 656d 2e73 6861 7065  spect, dem.shape
-00011990: 290d 0a20 2020 2020 2020 2023 2064 6973  )..        # dis
-000119a0: 706c 6163 656d 656e 7420 3d20 6e70 2e72  placement = np.r
-000119b0: 6573 697a 6528 6469 7370 6c61 6365 6d65  esize(displaceme
-000119c0: 6e74 2c20 6465 6d2e 7368 6170 6529 0d0a  nt, dem.shape)..
-000119d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-000119e0: 2020 736c 6f70 652c 2064 6972 6563 7469    slope, directi
-000119f0: 6f6e 616c 5f67 7261 6420 3d20 6361 6c63  onal_grad = calc
-00011a00: 756c 6174 655f 736c 6f70 6528 6465 6d2c  ulate_slope(dem,
-00011a10: 2061 7370 6563 742c 2064 7820 2c20 6479   aspect, dx , dy
-00011a20: 2029 0d0a 2020 2020 2020 2020 6865 6967   )..        heig
-00011a30: 6874 5f63 6861 6e67 6520 203d 2063 616c  ht_change  = cal
-00011a40: 6375 6c61 7465 5f68 6569 6768 745f 6368  culate_height_ch
-00011a50: 616e 6765 2873 6c6f 7065 2c20 6469 7265  ange(slope, dire
-00011a60: 6374 696f 6e61 6c5f 6772 6164 2c20 6465  ctional_grad, de
-00011a70: 6d29 0d0a 2020 2020 2020 2020 2368 6569  m)..        #hei
-00011a80: 6768 745f 6368 616e 6765 3d67 6175 7373  ght_change=gauss
-00011a90: 6961 6e28 6865 6967 6874 5f63 6861 6e67  ian(height_chang
-00011aa0: 652c 2073 6967 6d61 3d33 290d 0a20 2020  e, sigma=3)..   
-00011ab0: 2020 2020 2076 6f6c 756d 655f 6368 616e       volume_chan
-00011ac0: 6765 203d 2063 616c 6375 6c61 7465 5f76  ge = calculate_v
-00011ad0: 6f6c 756d 655f 6368 616e 6765 2868 6569  olume_change(hei
-00011ae0: 6768 745f 6368 616e 6765 2c20 7069 7865  ght_change, pixe
-00011af0: 6c5f 6172 6561 290d 0a20 2020 2020 2020  l_area)..       
-00011b00: 0d0a 2020 2020 2020 200d 0a0d 0a20 2020  ..       ....   
-00011b10: 2020 2020 2023 2044 6566 696e 6520 6120       # Define a 
-00011b20: 6675 6e63 7469 6f6e 2074 6f20 6578 706f  function to expo
-00011b30: 7274 2064 6174 6120 746f 2061 2047 656f  rt data to a Geo
-00011b40: 5449 4646 0d0a 2020 2020 2020 2020 6465  TIFF..        de
-00011b50: 6620 6578 706f 7274 5f74 6f5f 6765 6f74  f export_to_geot
-00011b60: 6966 6628 6461 7461 2c20 6f75 7470 7574  iff(data, output
-00011b70: 5f70 6174 682c 2072 6566 6572 656e 6365  _path, reference
-00011b80: 5f72 6173 7465 7229 3a0d 0a20 2020 2020  _raster):..     
-00011b90: 2020 2020 2020 2077 6974 6820 7261 7374         with rast
-00011ba0: 6572 696f 2e6f 7065 6e28 0d0a 2020 2020  erio.open(..    
-00011bb0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00011bc0: 7574 5f70 6174 682c 2027 7727 2c0d 0a20  ut_path, 'w',.. 
-00011bd0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00011be0: 7269 7665 723d 2747 5469 6666 272c 0d0a  river='GTiff',..
-00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c00: 6865 6967 6874 3d64 6174 612e 7368 6170  height=data.shap
-00011c10: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
-00011c20: 2020 2020 2020 2077 6964 7468 3d64 6174         width=dat
-00011c30: 612e 7368 6170 655b 315d 2c0d 0a20 2020  a.shape[1],..   
-00011c40: 2020 2020 2020 2020 2020 2020 2063 6f75               cou
-00011c50: 6e74 3d31 2c0d 0a20 2020 2020 2020 2020  nt=1,..         
-00011c60: 2020 2020 2020 2064 7479 7065 3d6e 702e         dtype=np.
-00011c70: 666c 6f61 7433 322c 0d0a 2020 2020 2020  float32,..      
-00011c80: 2020 2020 2020 2020 2020 6372 733d 7265            crs=re
-00011c90: 6665 7265 6e63 655f 7261 7374 6572 2e63  ference_raster.c
-00011ca0: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
-00011cb0: 2020 2020 2074 7261 6e73 666f 726d 3d72       transform=r
-00011cc0: 6566 6572 656e 6365 5f72 6173 7465 722e  eference_raster.
-00011cd0: 7472 616e 7366 6f72 6d2c 206e 6f64 6174  transform, nodat
-00011ce0: 613d 6e70 2e6e 616e 0d0a 2020 2020 2020  a=np.nan..      
-00011cf0: 2020 2020 2020 2920 6173 206f 7574 7075        ) as outpu
-00011d00: 745f 7261 7374 6572 3a0d 0a20 2020 2020  t_raster:..     
-00011d10: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00011d20: 745f 7261 7374 6572 2e77 7269 7465 2864  t_raster.write(d
-00011d30: 6174 612c 2031 290d 0a0d 0a20 2020 2020  ata, 1)....     
-00011d40: 2020 2023 2045 7870 6f72 7469 6e67 2073     # Exporting s
-00011d50: 6c6f 7065 2c20 6865 6967 6874 2063 6861  lope, height cha
-00011d60: 6e67 652c 2061 6e64 2076 6f6c 756d 6520  nge, and volume 
-00011d70: 6368 616e 6765 2074 6f20 4765 6f54 4946  change to GeoTIF
-00011d80: 4673 0d0a 2020 2020 2020 2020 6578 706f  Fs..        expo
-00011d90: 7274 5f74 6f5f 6765 6f74 6966 6628 736c  rt_to_geotiff(sl
-00011da0: 6f70 652c 2073 6c6f 7065 5f6f 7574 7075  ope, slope_outpu
-00011db0: 745f 7061 7468 2c20 6465 6d5f 7261 7374  t_path, dem_rast
-00011dc0: 6572 290d 0a20 2020 2020 2020 2065 7870  er)..        exp
-00011dd0: 6f72 745f 746f 5f67 656f 7469 6666 2868  ort_to_geotiff(h
-00011de0: 6569 6768 745f 6368 616e 6765 2c20 6865  eight_change, he
-00011df0: 6967 6874 5f6f 7574 7075 745f 7061 7468  ight_output_path
-00011e00: 2c20 6465 6d5f 7261 7374 6572 290d 0a20  , dem_raster).. 
-00011e10: 2020 2020 2020 2065 7870 6f72 745f 746f         export_to
-00011e20: 5f67 656f 7469 6666 2876 6f6c 756d 655f  _geotiff(volume_
-00011e30: 6368 616e 6765 2c20 766f 6c75 6d65 5f6f  change, volume_o
-00011e40: 7574 7075 745f 7061 7468 2c20 6465 6d5f  utput_path, dem_
-00011e50: 7261 7374 6572 290d 0a20 2020 2020 2020  raster)..       
-00011e60: 0d0a 0d0a 0d0a 0d0a 696d 706f 7274 206e  ........import n
-00011e70: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
-00011e80: 206f 7367 656f 2069 6d70 6f72 7420 6764   osgeo import gd
-00011e90: 616c 0d0a 0d0a 6465 6620 6361 6c63 756c  al....def calcul
-00011ea0: 6174 655f 616e 645f 7361 7665 5f61 7370  ate_and_save_asp
-00011eb0: 6563 745f 7261 7374 6572 2865 775f 7261  ect_raster(ew_ra
-00011ec0: 7374 6572 5f70 6174 683a 2073 7472 203d  ster_path: str =
-00011ed0: 2222 2c20 6e73 5f72 6173 7465 725f 7061  "", ns_raster_pa
-00011ee0: 7468 3a20 7374 7220 3d22 222c 206f 7574  th: str ="", out
-00011ef0: 7075 745f 7261 7374 6572 5f70 6174 683a  put_raster_path:
-00011f00: 2073 7472 203d 2222 293a 0d0a 2020 2020   str =""):..    
-00011f10: 2222 220d 0a20 2020 2043 616c 6375 6c61  """..    Calcula
-00011f20: 7465 2074 6865 2061 7370 6563 7420 7261  te the aspect ra
-00011f30: 7374 6572 2066 726f 6d20 6561 7374 2d77  ster from east-w
-00011f40: 6573 7420 616e 6420 6e6f 7274 682d 736f  est and north-so
-00011f50: 7574 6820 6469 7370 6c61 6365 6d65 6e74  uth displacement
-00011f60: 2072 6173 7465 7273 2061 6e64 2073 6176   rasters and sav
-00011f70: 6520 6974 2e0d 0a0d 0a20 2020 2054 6869  e it.....    Thi
-00011f80: 7320 6675 6e63 7469 6f6e 2072 6561 6473  s function reads
-00011f90: 2074 776f 2072 6173 7465 7220 6669 6c65   two raster file
-00011fa0: 7320 7265 7072 6573 656e 7469 6e67 2065  s representing e
-00011fb0: 6173 742d 7765 7374 2028 4557 2920 616e  ast-west (EW) an
-00011fc0: 6420 6e6f 7274 682d 736f 7574 6820 284e  d north-south (N
-00011fd0: 5329 200d 0a20 2020 2064 6973 706c 6163  S) ..    displac
-00011fe0: 656d 656e 7473 2c20 6361 6c63 756c 6174  ements, calculat
-00011ff0: 6573 2074 6865 2061 7370 6563 7420 6f66  es the aspect of
-00012000: 2065 6163 6820 7069 7865 6c2c 2061 6e64   each pixel, and
-00012010: 2073 6176 6573 2074 6865 2072 6573 756c   saves the resul
-00012020: 7420 6173 2061 206e 6577 2072 6173 7465  t as a new raste
-00012030: 7220 6669 6c65 2e0d 0a20 2020 2041 7370  r file...    Asp
-00012040: 6563 7420 6973 2063 616c 6375 6c61 7465  ect is calculate
-00012050: 6420 696e 2064 6567 7265 6573 2066 726f  d in degrees fro
-00012060: 6d20 6e6f 7274 6820 2830 2064 6567 7265  m north (0 degre
-00012070: 6573 292c 2065 6173 7420 2839 3020 6465  es), east (90 de
-00012080: 6772 6565 7329 2c20 736f 7574 6820 2831  grees), south (1
-00012090: 3830 2064 6567 7265 6573 292c 0d0a 2020  80 degrees),..  
-000120a0: 2020 616e 6420 7765 7374 2028 3237 3020    and west (270 
-000120b0: 6465 6772 6565 7329 2e0d 0a0d 0a20 2020  degrees).....   
-000120c0: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
-000120d0: 2020 2d20 6577 5f72 6173 7465 725f 7061    - ew_raster_pa
-000120e0: 7468 2028 7374 7229 3a20 4669 6c65 2070  th (str): File p
-000120f0: 6174 6820 666f 7220 7468 6520 6561 7374  ath for the east
-00012100: 2d77 6573 7420 6469 7370 6c61 6365 6d65  -west displaceme
-00012110: 6e74 2072 6173 7465 722e 0d0a 2020 2020  nt raster...    
-00012120: 2d20 6e73 5f72 6173 7465 725f 7061 7468  - ns_raster_path
-00012130: 2028 7374 7229 3a20 4669 6c65 2070 6174   (str): File pat
-00012140: 6820 666f 7220 7468 6520 6e6f 7274 682d  h for the north-
-00012150: 736f 7574 6820 6469 7370 6c61 6365 6d65  south displaceme
-00012160: 6e74 2072 6173 7465 722e 0d0a 2020 2020  nt raster...    
-00012170: 2d20 6f75 7470 7574 5f72 6173 7465 725f  - output_raster_
-00012180: 7061 7468 2028 7374 7229 3a20 4669 6c65  path (str): File
-00012190: 2070 6174 6820 666f 7220 7468 6520 6f75   path for the ou
-000121a0: 7470 7574 2061 7370 6563 7420 7261 7374  tput aspect rast
-000121b0: 6572 2e0d 0a0d 0a20 2020 2052 6574 7572  er.....    Retur
-000121c0: 6e73 3a0d 0a20 2020 204e 6f6e 652e 2054  ns:..    None. T
-000121d0: 6865 2072 6573 756c 7420 6973 2073 6176  he result is sav
-000121e0: 6564 2061 7320 6120 6e65 7720 7261 7374  ed as a new rast
-000121f0: 6572 2066 696c 6520 6174 2074 6865 2073  er file at the s
-00012200: 7065 6369 6669 6564 206f 7574 7075 7420  pecified output 
-00012210: 7061 7468 2e0d 0a20 2020 200d 0a20 2020  path...    ..   
-00012220: 2022 2222 0d0a 2020 2020 6465 6620 7265   """..    def re
-00012230: 6164 5f72 6173 7465 7228 6669 6c65 5f70  ad_raster(file_p
-00012240: 6174 6829 3a0d 0a20 2020 2020 2020 2022  ath):..        "
-00012250: 2222 5265 6164 2061 2072 6173 7465 7220  ""Read a raster 
-00012260: 6669 6c65 2061 6e64 2072 6574 7572 6e20  file and return 
-00012270: 7468 6520 6461 7461 2061 7272 6179 2061  the data array a
-00012280: 6e64 2067 656f 7472 616e 7366 6f72 6d2e  nd geotransform.
-00012290: 2222 220d 0a0d 0a20 2020 2020 2020 2023  """....        #
-000122a0: 204f 7065 6e20 7468 6520 6461 7461 7365   Open the datase
-000122b0: 740d 0a20 2020 2020 2020 2064 6174 6173  t..        datas
-000122c0: 6574 203d 2067 6461 6c2e 4f70 656e 2866  et = gdal.Open(f
-000122d0: 696c 655f 7061 7468 290d 0a20 2020 2020  ile_path)..     
-000122e0: 2020 2069 6620 6461 7461 7365 7420 6973     if dataset is
-000122f0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00012300: 2020 2020 7261 6973 6520 494f 4572 726f      raise IOErro
-00012310: 7228 2243 6f75 6c64 206e 6f74 206f 7065  r("Could not ope
-00012320: 6e20 6669 6c65 2061 7420 7b7d 222e 666f  n file at {}".fo
-00012330: 726d 6174 2866 696c 655f 7061 7468 2929  rmat(file_path))
-00012340: 0d0a 0d0a 2020 2020 2020 2020 2320 4765  ....        # Ge
-00012350: 7420 7468 6520 6669 7273 7420 7261 7374  t the first rast
-00012360: 6572 2062 616e 640d 0a20 2020 2020 2020  er band..       
-00012370: 2062 616e 6420 3d20 6461 7461 7365 742e   band = dataset.
-00012380: 4765 7452 6173 7465 7242 616e 6428 3129  GetRasterBand(1)
-00012390: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
-000123a0: 6164 2074 6865 2064 6174 6120 6173 2061  ad the data as a
-000123b0: 206e 756d 7079 2061 7272 6179 0d0a 2020   numpy array..  
-000123c0: 2020 2020 2020 6461 7461 203d 2062 616e        data = ban
-000123d0: 642e 5265 6164 4173 4172 7261 7928 290d  d.ReadAsArray().
-000123e0: 0a0d 0a20 2020 2020 2020 2023 2047 6574  ...        # Get
-000123f0: 206e 6f2d 6461 7461 2076 616c 7565 2066   no-data value f
-00012400: 726f 6d20 7468 6520 6261 6e64 0d0a 2020  rom the band..  
-00012410: 2020 2020 2020 6e6f 6461 7461 5f76 616c        nodata_val
-00012420: 7565 203d 2062 616e 642e 4765 744e 6f44  ue = band.GetNoD
-00012430: 6174 6156 616c 7565 2829 0d0a 0d0a 2020  ataValue()....  
-00012440: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
-00012450: 2074 6865 7265 2069 7320 6120 6e6f 2d64   there is a no-d
-00012460: 6174 6120 7661 6c75 6520 6465 6669 6e65  ata value define
-00012470: 640d 0a20 2020 2020 2020 2069 6620 6e6f  d..        if no
-00012480: 6461 7461 5f76 616c 7565 2069 7320 6e6f  data_value is no
-00012490: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
-000124a0: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
-000124b0: 6d61 736b 2074 6861 7420 6973 2054 7275  mask that is Tru
-000124c0: 6520 666f 7220 7661 6c69 6420 7069 7865  e for valid pixe
-000124d0: 6c73 0d0a 2020 2020 2020 2020 2020 2020  ls..            
-000124e0: 6d61 736b 203d 2064 6174 6120 213d 206e  mask = data != n
-000124f0: 6f64 6174 615f 7661 6c75 650d 0a0d 0a20  odata_value.... 
-00012500: 2020 2020 2020 2020 2020 2023 2041 7070             # App
-00012510: 6c79 2074 6865 206d 6173 6b20 746f 2066  ly the mask to f
-00012520: 696c 7465 7220 6f75 7420 6e6f 2d64 6174  ilter out no-dat
-00012530: 6120 7069 7865 6c73 0d0a 2020 2020 2020  a pixels..      
-00012540: 2020 2020 2020 7661 6c69 645f 6461 7461        valid_data
-00012550: 203d 206e 702e 7768 6572 6528 6d61 736b   = np.where(mask
-00012560: 2c20 6461 7461 2c20 6e70 2e6e 616e 2920  , data, np.nan) 
-00012570: 2023 2052 6570 6c61 6365 206e 6f2d 6461   # Replace no-da
-00012580: 7461 2077 6974 6820 4e61 4e0d 0a20 2020  ta with NaN..   
-00012590: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
-000125a0: 2020 2020 2020 2020 7661 6c69 645f 6461          valid_da
-000125b0: 7461 203d 2064 6174 6120 2023 2041 6c6c  ta = data  # All
-000125c0: 2064 6174 6120 6973 2076 616c 6964 2069   data is valid i
-000125d0: 6620 7468 6572 6520 6973 206e 6f20 6e6f  f there is no no
-000125e0: 2d64 6174 6120 7661 6c75 650d 0a0d 0a20  -data value.... 
-000125f0: 2020 2020 2020 2023 2052 6574 7269 6576         # Retriev
-00012600: 6520 6765 6f74 7261 6e73 666f 726d 6174  e geotransformat
-00012610: 696f 6e0d 0a20 2020 2020 2020 2067 656f  ion..        geo
-00012620: 7472 616e 7366 6f72 6d20 3d20 6461 7461  transform = data
-00012630: 7365 742e 4765 7447 656f 5472 616e 7366  set.GetGeoTransf
-00012640: 6f72 6d28 290d 0a0d 0a20 2020 2020 2020  orm()....       
-00012650: 2023 2043 6c6f 7365 2074 6865 2064 6174   # Close the dat
-00012660: 6173 6574 0d0a 2020 2020 2020 2020 2364  aset..        #d
-00012670: 6174 6173 6574 203d 204e 6f6e 650d 0a0d  ataset = None...
-00012680: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012690: 7661 6c69 645f 6461 7461 2c20 6765 6f74  valid_data, geot
-000126a0: 7261 6e73 666f 726d 2c20 6461 7461 7365  ransform, datase
-000126b0: 740d 0a0d 0a20 2020 2064 6566 2063 616c  t....    def cal
-000126c0: 6375 6c61 7465 5f61 7370 6563 7428 6577  culate_aspect(ew
-000126d0: 5f64 6174 612c 206e 735f 6461 7461 293a  _data, ns_data):
-000126e0: 0d0a 2020 2020 2020 2020 2222 2243 616c  ..        """Cal
-000126f0: 6375 6c61 7465 2074 6865 2061 7370 6563  culate the aspec
-00012700: 7420 6672 6f6d 2045 5720 616e 6420 4e53  t from EW and NS
-00012710: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
-00012720: 7461 2e22 2222 0d0a 2020 2020 2020 2020  ta."""..        
-00012730: 7769 7468 206e 702e 6572 7273 7461 7465  with np.errstate
-00012740: 2864 6976 6964 653d 2769 676e 6f72 6527  (divide='ignore'
-00012750: 2c20 696e 7661 6c69 643d 2769 676e 6f72  , invalid='ignor
-00012760: 6527 293a 0d0a 2020 2020 2020 2020 2020  e'):..          
-00012770: 2020 6173 7065 6374 203d 206e 702e 6172    aspect = np.ar
-00012780: 6374 616e 3228 6577 5f64 6174 612c 206e  ctan2(ew_data, n
-00012790: 735f 6461 7461 290d 0a20 2020 2020 2020  s_data)..       
-000127a0: 2020 2020 2061 7370 6563 745f 6465 673d       aspect_deg=
-000127b0: 6e70 2e64 6567 7265 6573 2861 7370 6563  np.degrees(aspec
-000127c0: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
-000127d0: 6173 7065 6374 5f64 6567 203d 2028 3435  aspect_deg = (45
-000127e0: 3020 2d61 7370 6563 745f 6465 6720 2920  0 -aspect_deg ) 
-000127f0: 2520 3336 300d 0a20 2020 2020 2020 2072  % 360..        r
-00012800: 6574 7572 6e20 6173 7065 6374 5f64 6567  eturn aspect_deg
-00012810: 0d0a 0d0a 2020 2020 6465 6620 7361 7665  ....    def save
-00012820: 5f72 6173 7465 7228 6f75 7470 7574 5f70  _raster(output_p
-00012830: 6174 682c 2064 6174 612c 2067 656f 5f74  ath, data, geo_t
-00012840: 7261 6e73 666f 726d 2c20 7265 6665 7265  ransform, refere
-00012850: 6e63 655f 6461 7461 7365 7429 3a0d 0a20  nce_dataset):.. 
-00012860: 2020 2020 2020 2022 2222 5361 7665 2074         """Save t
-00012870: 6865 2064 6174 6120 6173 2061 2072 6173  he data as a ras
-00012880: 7465 7220 6669 6c65 2e22 2222 0d0a 2020  ter file."""..  
-00012890: 2020 2020 2020 6472 6976 6572 203d 2067        driver = g
-000128a0: 6461 6c2e 4765 7444 7269 7665 7242 794e  dal.GetDriverByN
-000128b0: 616d 6528 2747 5469 6666 2729 0d0a 2020  ame('GTiff')..  
-000128c0: 2020 2020 2020 726f 7773 2c20 636f 6c73        rows, cols
-000128d0: 203d 2064 6174 612e 7368 6170 650d 0a20   = data.shape.. 
-000128e0: 2020 2020 2020 206f 7574 5f72 6173 7465         out_raste
-000128f0: 7220 3d20 6472 6976 6572 2e43 7265 6174  r = driver.Creat
-00012900: 6528 6f75 7470 7574 5f70 6174 682c 2063  e(output_path, c
-00012910: 6f6c 732c 2072 6f77 732c 2031 2c20 6764  ols, rows, 1, gd
-00012920: 616c 2e47 4454 5f46 6c6f 6174 3332 290d  al.GDT_Float32).
-00012930: 0a20 2020 2020 2020 206f 7574 5f72 6173  .        out_ras
-00012940: 7465 722e 5365 7447 656f 5472 616e 7366  ter.SetGeoTransf
-00012950: 6f72 6d28 6765 6f5f 7472 616e 7366 6f72  orm(geo_transfor
-00012960: 6d29 0d0a 2020 2020 2020 2020 6f75 745f  m)..        out_
-00012970: 6261 6e64 203d 206f 7574 5f72 6173 7465  band = out_raste
-00012980: 722e 4765 7452 6173 7465 7242 616e 6428  r.GetRasterBand(
-00012990: 3129 0d0a 2020 2020 2020 2020 6f75 745f  1)..        out_
-000129a0: 6261 6e64 2e57 7269 7465 4172 7261 7928  band.WriteArray(
-000129b0: 6461 7461 290d 0a20 2020 2020 2020 206f  data)..        o
-000129c0: 7574 5f72 6173 7465 722e 5365 7450 726f  ut_raster.SetPro
-000129d0: 6a65 6374 696f 6e28 7265 6665 7265 6e63  jection(referenc
-000129e0: 655f 6461 7461 7365 742e 4765 7450 726f  e_dataset.GetPro
-000129f0: 6a65 6374 696f 6e28 2929 0d0a 2020 2020  jection())..    
-00012a00: 2020 2020 6f75 745f 6261 6e64 2e46 6c75      out_band.Flu
-00012a10: 7368 4361 6368 6528 290d 0a0d 0a20 2020  shCache()....   
-00012a20: 2023 2052 6561 6420 7468 6520 4557 2061   # Read the EW a
-00012a30: 6e64 204e 5320 7261 7374 6572 2064 6174  nd NS raster dat
-00012a40: 610d 0a20 2020 2065 775f 6461 7461 2c20  a..    ew_data, 
-00012a50: 6765 6f5f 7472 616e 7366 6f72 6d2c 2064  geo_transform, d
-00012a60: 6174 6173 6574 203d 2072 6561 645f 7261  ataset = read_ra
-00012a70: 7374 6572 2865 775f 7261 7374 6572 5f70  ster(ew_raster_p
-00012a80: 6174 6829 0d0a 2020 2020 6e73 5f64 6174  ath)..    ns_dat
-00012a90: 612c 205f 2c20 5f20 3d20 7265 6164 5f72  a, _, _ = read_r
-00012aa0: 6173 7465 7228 6e73 5f72 6173 7465 725f  aster(ns_raster_
-00012ab0: 7061 7468 290d 0a0d 0a20 2020 2023 2043  path)....    # C
-00012ac0: 616c 6375 6c61 7465 2074 6865 2061 7370  alculate the asp
-00012ad0: 6563 7420 616e 6420 7361 7665 2074 6865  ect and save the
-00012ae0: 2072 6573 756c 740d 0a20 2020 2061 7370   result..    asp
-00012af0: 6563 745f 6461 7461 203d 2063 616c 6375  ect_data = calcu
-00012b00: 6c61 7465 5f61 7370 6563 7428 6577 5f64  late_aspect(ew_d
-00012b10: 6174 612c 206e 735f 6461 7461 290d 0a20  ata, ns_data).. 
-00012b20: 2020 2073 6176 655f 7261 7374 6572 286f     save_raster(o
-00012b30: 7574 7075 745f 7261 7374 6572 5f70 6174  utput_raster_pat
-00012b40: 682c 2061 7370 6563 745f 6461 7461 2c20  h, aspect_data, 
-00012b50: 6765 6f5f 7472 616e 7366 6f72 6d2c 2064  geo_transform, d
-00012b60: 6174 6173 6574 290d 0a0d 0a23 2045 7861  ataset)....# Exa
-00012b70: 6d70 6c65 2075 7361 6765 3a0d 0a23 2063  mple usage:..# c
-00012b80: 616c 6375 6c61 7465 5f61 6e64 5f73 6176  alculate_and_sav
-00012b90: 655f 6173 7065 6374 5f72 6173 7465 7228  e_aspect_raster(
-00012ba0: 2770 6174 685f 746f 5f65 775f 7261 7374  'path_to_ew_rast
-00012bb0: 6572 2e74 6966 272c 2027 7061 7468 5f74  er.tif', 'path_t
-00012bc0: 6f5f 6e73 5f72 6173 7465 722e 7469 6627  o_ns_raster.tif'
-00012bd0: 2c20 2770 6174 685f 746f 5f6f 7574 7075  , 'path_to_outpu
-00012be0: 745f 6173 7065 6374 5f72 6173 7465 722e  t_aspect_raster.
-00012bf0: 7469 6627 290d 0a0d 0a0d 0a0d 0a23 2323  tif')........###
-00012c00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012c10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00012c20: 2323 2323 2323 2323 2323 230d 0a0d 0a    ###########....
+000088e0: 2020 2020 2020 2020 2320 4f70 656e 2074          # Open t
+000088f0: 6865 2044 454d 2066 696c 6520 7573 696e  he DEM file usin
+00008900: 6720 4744 414c 0d0a 2020 2020 2020 2020  g GDAL..        
+00008910: 6473 203d 2067 6461 6c2e 4f70 656e 2864  ds = gdal.Open(d
+00008920: 656d 5f66 696c 6529 0d0a 2020 2020 2020  em_file)..      
+00008930: 2020 6966 2064 7320 6973 204e 6f6e 653a    if ds is None:
+00008940: 0d0a 2020 2020 2020 2020 2020 2020 7261  ..            ra
+00008950: 6973 6520 4669 6c65 4e6f 7446 6f75 6e64  ise FileNotFound
+00008960: 4572 726f 7228 6622 4669 6c65 206e 6f74  Error(f"File not
+00008970: 2066 6f75 6e64 3a20 7b64 656d 5f66 696c   found: {dem_fil
+00008980: 657d 2229 0d0a 0d0a 2020 2020 2020 2020  e}")....        
+00008990: 2320 4163 6365 7373 2074 6865 2066 6972  # Access the fir
+000089a0: 7374 2072 6173 7465 7220 6261 6e64 2066  st raster band f
+000089b0: 726f 6d20 7468 6520 6461 7461 7365 740d  rom the dataset.
+000089c0: 0a20 2020 2020 2020 2062 616e 6420 3d20  .        band = 
+000089d0: 6473 2e47 6574 5261 7374 6572 4261 6e64  ds.GetRasterBand
+000089e0: 2831 290d 0a0d 0a20 2020 2020 2020 2023  (1)....        #
+000089f0: 2052 6574 7269 6576 6520 7468 6520 6e6f   Retrieve the no
+00008a00: 2064 6174 6120 7661 6c75 6520 6672 6f6d   data value from
+00008a10: 2074 6865 2062 616e 640d 0a20 2020 2020   the band..     
+00008a20: 2020 206e 6f5f 6461 7461 5f76 616c 7565     no_data_value
+00008a30: 203d 2062 616e 642e 4765 744e 6f44 6174   = band.GetNoDat
+00008a40: 6156 616c 7565 2829 0d0a 0d0a 2020 2020  aValue()....    
+00008a50: 2020 2020 2320 5265 6164 2074 6865 2064      # Read the d
+00008a60: 6174 6120 696e 746f 2061 204e 756d 5079  ata into a NumPy
+00008a70: 2061 7272 6179 0d0a 2020 2020 2020 2020   array..        
+00008a80: 6461 7461 203d 2062 616e 642e 5265 6164  data = band.Read
+00008a90: 4173 4172 7261 7928 290d 0a0d 0a20 2020  AsArray()....   
+00008aa0: 2020 2020 2023 2043 6865 636b 2069 6620       # Check if 
+00008ab0: 7468 6572 6520 6973 2061 206e 6f20 6461  there is a no da
+00008ac0: 7461 2076 616c 7565 2064 6566 696e 6564  ta value defined
+00008ad0: 2061 6e64 2072 6570 6c61 6365 2069 7420   and replace it 
+00008ae0: 7769 7468 204e 614e 0d0a 2020 2020 2020  with NaN..      
+00008af0: 2020 6966 206e 6f5f 6461 7461 5f76 616c    if no_data_val
+00008b00: 7565 2069 7320 6e6f 7420 4e6f 6e65 3a0d  ue is not None:.
+00008b10: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00008b20: 615b 6461 7461 203d 3d20 6e6f 5f64 6174  a[data == no_dat
+00008b30: 615f 7661 6c75 655d 203d 206e 702e 6e61  a_value] = np.na
+00008b40: 6e0d 0a0d 0a20 2020 2020 2020 2023 2047  n....        # G
+00008b50: 6574 2067 656f 7472 616e 7366 6f72 6d61  et geotransforma
+00008b60: 7469 6f6e 2061 6e64 2070 726f 6a65 6374  tion and project
+00008b70: 696f 6e20 696e 666f 726d 6174 696f 6e0d  ion information.
+00008b80: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
+00008b90: 726d 203d 2064 732e 4765 7447 656f 5472  rm = ds.GetGeoTr
+00008ba0: 616e 7366 6f72 6d28 290d 0a20 2020 2020  ansform()..     
+00008bb0: 2020 2070 726f 6a65 6374 696f 6e20 3d20     projection = 
+00008bc0: 6473 2e47 6574 5072 6f6a 6563 7469 6f6e  ds.GetProjection
+00008bd0: 2829 0d0a 0d0a 2020 2020 2020 2020 2320  ()....        # 
+00008be0: 436c 6561 6e20 7570 2062 7920 636c 6f73  Clean up by clos
+00008bf0: 696e 6720 7468 6520 6461 7461 7365 740d  ing the dataset.
+00008c00: 0a20 2020 2020 2020 2064 7320 3d20 4e6f  .        ds = No
+00008c10: 6e65 0d0a 2020 2020 2020 2020 7265 7475  ne..        retu
+00008c20: 726e 2064 6174 612c 2074 7261 6e73 666f  rn data, transfo
+00008c30: 726d 2c20 7072 6f6a 6563 7469 6f6e 0d0a  rm, projection..
+00008c40: 2020 2020 0d0a 2020 2020 6461 7461 2c20      ..    data, 
+00008c50: 7472 616e 7366 6f72 6d2c 2070 726f 6a65  transform, proje
+00008c60: 6374 696f 6e20 3d20 7265 6164 5f64 656d  ction = read_dem
+00008c70: 2864 656d 5f64 6174 6129 0d0a 2020 2020  (dem_data)..    
+00008c80: 0d0a 2020 2020 696d 706f 7274 206d 6174  ..    import mat
+00008c90: 680d 0a0d 0a20 2020 2064 6566 2063 616c  h....    def cal
+00008ca0: 6375 6c61 7465 5f64 6970 5f61 6e67 6c65  culate_dip_angle
+00008cb0: 5f61 6e64 5f64 6972 6563 7469 6f6e 2841  _and_direction(A
+00008cc0: 2c20 4229 3a0d 0a20 2020 2020 2020 2023  , B):..        #
+00008cd0: 2043 616c 6375 6c61 7465 2074 6865 2064   Calculate the d
+00008ce0: 6970 2061 6e67 6c65 2028 696e 636c 696e  ip angle (inclin
+00008cf0: 6174 696f 6e29 0d0a 2020 2020 2020 2020  ation)..        
+00008d00: 6469 705f 616e 676c 6520 3d20 6d61 7468  dip_angle = math
+00008d10: 2e64 6567 7265 6573 286d 6174 682e 6174  .degrees(math.at
+00008d20: 616e 286d 6174 682e 7371 7274 2841 2a2a  an(math.sqrt(A**
+00008d30: 3220 2b20 422a 2a32 2929 290d 0a20 2020  2 + B**2)))..   
+00008d40: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+00008d50: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
+00008d60: 6174 6520 7468 6520 6469 7020 6469 7265  ate the dip dire
+00008d70: 6374 696f 6e20 2861 7a69 6d75 7468 290d  ction (azimuth).
+00008d80: 0a20 2020 2020 2020 2064 6970 5f64 6972  .        dip_dir
+00008d90: 6563 7469 6f6e 203d 206d 6174 682e 6465  ection = math.de
+00008da0: 6772 6565 7328 6d61 7468 2e61 7461 6e32  grees(math.atan2
+00008db0: 282d 422c 202d 4129 290d 0a20 2020 2020  (-B, -A))..     
+00008dc0: 2020 200d 0a20 2020 2020 2020 2023 2045     ..        # E
+00008dd0: 6e73 7572 6520 6469 705f 6469 7265 6374  nsure dip_direct
+00008de0: 696f 6e20 6973 2069 6e20 7468 6520 7261  ion is in the ra
+00008df0: 6e67 6520 5b30 2c20 3336 3029 0d0a 2020  nge [0, 360)..  
+00008e00: 2020 2020 2020 6469 705f 6469 7265 6374        dip_direct
+00008e10: 696f 6e20 3d20 2864 6970 5f64 6972 6563  ion = (dip_direc
+00008e20: 7469 6f6e 202b 2039 3029 2025 2033 3630  tion + 90) % 360
+00008e30: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00008e40: 2020 2020 7265 7475 726e 2064 6970 5f61      return dip_a
+00008e50: 6e67 6c65 2c20 6469 705f 6469 7265 6374  ngle, dip_direct
+00008e60: 696f 6e0d 0a20 2020 200d 0a20 2020 2064  ion..    ..    d
+00008e70: 6566 2066 6974 5f70 6c61 6e65 2870 6f69  ef fit_plane(poi
+00008e80: 6e74 732c 2078 782c 2079 7929 3a0d 0a20  nts, xx, yy):.. 
+00008e90: 2020 2020 2020 206d 696e 5f72 616e 6765         min_range
+00008ea0: 203d 206e 702e 6e61 6e6d 696e 2864 6174   = np.nanmin(dat
+00008eb0: 6129 0d0a 2020 2020 2020 2020 6d61 785f  a)..        max_
+00008ec0: 7261 6e67 6520 3d20 6e70 2e6e 616e 6d61  range = np.nanma
+00008ed0: 7828 6461 7461 290d 0a20 2020 2020 2020  x(data)..       
+00008ee0: 200d 0a20 2020 2020 2020 2023 2078 7820   ..        # xx 
+00008ef0: 3d20 2878 7820 2d20 6e70 2e6e 616e 6d69  = (xx - np.nanmi
+00008f00: 6e28 7878 2929 202f 2028 6e70 2e6e 616e  n(xx)) / (np.nan
+00008f10: 6d61 7828 7878 2920 2d20 6e70 2e6e 616e  max(xx) - np.nan
+00008f20: 6d69 6e28 7878 2929 0d0a 2020 2020 2020  min(xx))..      
+00008f30: 2020 2320 7878 203d 2078 7820 2a20 286d    # xx = xx * (m
+00008f40: 6178 5f72 616e 6765 202d 206d 696e 5f72  ax_range - min_r
+00008f50: 616e 6765 2920 2b20 6d69 6e5f 7261 6e67  ange) + min_rang
+00008f60: 650d 0a20 2020 2020 2020 200d 0a20 2020  e..        ..   
+00008f70: 2020 2020 2023 2079 7920 3d20 2879 7920       # yy = (yy 
+00008f80: 2d20 6e70 2e6e 616e 6d69 6e28 7979 2929  - np.nanmin(yy))
+00008f90: 202f 2028 6e70 2e6e 616e 6d61 7828 7979   / (np.nanmax(yy
+00008fa0: 2920 2d20 6e70 2e6e 616e 6d69 6e28 7979  ) - np.nanmin(yy
+00008fb0: 2929 0d0a 2020 2020 2020 2020 2320 7979  ))..        # yy
+00008fc0: 203d 2079 7920 2a20 286d 6178 5f72 616e   = yy * (max_ran
+00008fd0: 6765 202d 206d 696e 5f72 616e 6765 2920  ge - min_range) 
+00008fe0: 2b20 6d69 6e5f 7261 6e67 650d 0a20 2020  + min_range..   
+00008ff0: 2020 2020 200d 0a20 2020 2020 2020 2078       ..        x
+00009000: 5f76 616c 732c 2079 5f76 616c 732c 207a  _vals, y_vals, z
+00009010: 5f76 616c 7320 3d20 7a69 7028 2a70 6f69  _vals = zip(*poi
+00009020: 6e74 7329 0d0a 2020 2020 0d0a 2020 2020  nts)..    ..    
+00009030: 2020 2020 4120 3d20 6e70 2e76 7374 6163      A = np.vstac
+00009040: 6b28 5b78 5f76 616c 732c 2079 5f76 616c  k([x_vals, y_val
+00009050: 732c 206e 702e 6f6e 6573 286c 656e 2878  s, np.ones(len(x
+00009060: 5f76 616c 7329 295d 292e 540d 0a20 2020  _vals))]).T..   
+00009070: 2020 2020 2061 2c20 622c 2063 203d 206e       a, b, c = n
+00009080: 702e 6c69 6e61 6c67 2e6c 7374 7371 2841  p.linalg.lstsq(A
+00009090: 2c20 7a5f 7661 6c73 2c20 7263 6f6e 643d  , z_vals, rcond=
+000090a0: 4e6f 6e65 295b 305d 0d0a 2020 2020 2020  None)[0]..      
+000090b0: 2020 0d0a 2020 2020 2020 2020 7072 696e    ..        prin
+000090c0: 7428 6622 506c 616e 6520 6571 7561 7469  t(f"Plane equati
+000090d0: 6f6e 3a20 7a20 3d20 7b61 7d78 202b 207b  on: z = {a}x + {
+000090e0: 627d 7920 2b20 7b63 7d22 2920 2023 2044  b}y + {c}")  # D
+000090f0: 6562 7567 6769 6e67 206c 696e 650d 0a20  ebugging line.. 
+00009100: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00009110: 207a 7a20 3d20 6120 2a20 7878 202b 2062   zz = a * xx + b
+00009120: 202a 2079 7920 2b20 630d 0a20 2020 2020   * yy + c..     
+00009130: 2020 2023 2323 2323 2323 2323 2323 2323     #############
+00009140: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009150: 2323 2323 230d 0a20 2020 2020 2020 2023  #####..        #
+00009160: 2070 6f69 6e74 7320 3d20 6e70 2e61 7272   points = np.arr
+00009170: 6179 2870 6f69 6e74 7329 200d 0a20 2020  ay(points) ..   
+00009180: 2020 2020 2023 2023 2043 6f6d 7075 7465       # # Compute
+00009190: 2074 6865 2063 656e 7472 6f69 6420 6f66   the centroid of
+000091a0: 2074 6865 2070 6f69 6e74 730d 0a20 2020   the points..   
+000091b0: 2020 2020 2023 2063 656e 7472 6f69 6420       # centroid 
+000091c0: 3d20 6e70 2e6d 6561 6e28 706f 696e 7473  = np.mean(points
+000091d0: 2c20 6178 6973 3d30 290d 0a0d 0a20 2020  , axis=0)....   
+000091e0: 2020 2020 2023 2023 2053 7562 7472 6163       # # Subtrac
+000091f0: 7420 7468 6520 6365 6e74 726f 6964 2066  t the centroid f
+00009200: 726f 6d20 7468 6520 706f 696e 7473 2074  rom the points t
+00009210: 6f20 6365 6e74 6572 2074 6865 6d0d 0a20  o center them.. 
+00009220: 2020 2020 2020 2023 2063 656e 7465 7265         # centere
+00009230: 645f 706f 696e 7473 203d 2070 6f69 6e74  d_points = point
+00009240: 7320 2d20 6365 6e74 726f 6964 0d0a 0d0a  s - centroid....
+00009250: 2020 2020 2020 2020 2320 2320 5065 7266          # # Perf
+00009260: 6f72 6d20 5356 4420 6f6e 2074 6865 2063  orm SVD on the c
+00009270: 656e 7465 7265 6420 706f 696e 7473 0d0a  entered points..
+00009280: 2020 2020 2020 2020 2320 552c 2053 2c20          # U, S, 
+00009290: 5674 203d 206e 702e 6c69 6e61 6c67 2e73  Vt = np.linalg.s
+000092a0: 7664 2863 656e 7465 7265 645f 706f 696e  vd(centered_poin
+000092b0: 7473 290d 0a0d 0a20 2020 2020 2020 2023  ts)....        #
+000092c0: 2023 2054 6865 206e 6f72 6d61 6c20 7665   # The normal ve
+000092d0: 6374 6f72 206f 6620 7468 6520 706c 616e  ctor of the plan
+000092e0: 6520 6973 2074 6865 206c 6173 7420 726f  e is the last ro
+000092f0: 7720 6f66 2056 740d 0a20 2020 2020 2020  w of Vt..       
+00009300: 2023 206e 6f72 6d61 6c5f 7665 6374 6f72   # normal_vector
+00009310: 203d 2056 745b 2d31 2c20 3a5d 0d0a 0d0a   = Vt[-1, :]....
+00009320: 2020 2020 2020 2020 2320 2320 4e6f 726d          # # Norm
+00009330: 616c 697a 6520 7468 6520 6e6f 726d 616c  alize the normal
+00009340: 2076 6563 746f 720d 0a20 2020 2020 2020   vector..       
+00009350: 2023 206e 6f72 6d61 6c5f 7665 6374 6f72   # normal_vector
+00009360: 202f 3d20 6e70 2e6c 696e 616c 672e 6e6f   /= np.linalg.no
+00009370: 726d 286e 6f72 6d61 6c5f 7665 6374 6f72  rm(normal_vector
+00009380: 290d 0a0d 0a20 2020 2020 2020 2023 2023  )....        # #
+00009390: 2054 6865 2065 7175 6174 696f 6e20 6f66   The equation of
+000093a0: 2074 6865 2070 6c61 6e65 2069 733a 2061   the plane is: a
+000093b0: 7820 2b20 6279 202b 2063 7a20 2b20 6420  x + by + cz + d 
+000093c0: 3d20 302c 2077 6865 7265 205b 612c 2062  = 0, where [a, b
+000093d0: 2c20 635d 2069 7320 7468 6520 6e6f 726d  , c] is the norm
+000093e0: 616c 2076 6563 746f 720d 0a20 2020 2020  al vector..     
+000093f0: 2020 2023 2061 2c20 622c 2063 203d 206e     # a, b, c = n
+00009400: 6f72 6d61 6c5f 7665 6374 6f72 0d0a 0d0a  ormal_vector....
+00009410: 2020 2020 2020 2020 2320 2320 4361 6c63          # # Calc
+00009420: 756c 6174 6520 6420 7573 696e 6720 7468  ulate d using th
+00009430: 6520 706c 616e 6520 6571 7561 7469 6f6e  e plane equation
+00009440: 2061 6e64 2074 6865 2063 656e 7472 6f69   and the centroi
+00009450: 640d 0a20 2020 2020 2020 2023 2064 203d  d..        # d =
+00009460: 202d 6e70 2e64 6f74 286e 6f72 6d61 6c5f   -np.dot(normal_
+00009470: 7665 6374 6f72 2c20 6365 6e74 726f 6964  vector, centroid
+00009480: 290d 0a20 2020 2020 2020 2023 207a 7a20  )..        # zz 
+00009490: 3d20 282d 6120 2a20 7878 202d 2062 202a  = (-a * xx - b *
+000094a0: 2079 7920 2d20 6429 202f 2063 2020 2320   yy - d) / c  # 
+000094b0: 536f 6c76 6520 666f 7220 7a0d 0a20 2020  Solve for z..   
+000094c0: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
+000094d0: 2020 2020 2020 2020 6469 705f 616e 676c          dip_angl
+000094e0: 652c 2064 6970 5f64 6972 6563 7469 6f6e  e, dip_direction
+000094f0: 203d 2063 616c 6375 6c61 7465 5f64 6970   = calculate_dip
+00009500: 5f61 6e67 6c65 5f61 6e64 5f64 6972 6563  _angle_and_direc
+00009510: 7469 6f6e 2861 2c20 6229 0d0a 0d0a 2020  tion(a, b)....  
+00009520: 2020 2020 2020 7072 696e 7428 6622 4469        print(f"Di
+00009530: 7020 416e 676c 6520 2849 6e63 6c69 6e61  p Angle (Inclina
+00009540: 7469 6f6e 293a 207b 6469 705f 616e 676c  tion): {dip_angl
+00009550: 657d 2064 6567 7265 6573 2229 0d0a 2020  e} degrees")..  
+00009560: 2020 2020 2020 7072 696e 7428 6622 4469        print(f"Di
+00009570: 7020 4469 7265 6374 696f 6e20 2841 7a69  p Direction (Azi
+00009580: 6d75 7468 293a 207b 6469 705f 6469 7265  muth): {dip_dire
+00009590: 6374 696f 6e7d 2064 6567 7265 6573 2229  ction} degrees")
+000095a0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000095b0: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+000095c0: 6465 6620 6e6f 726d 616c 697a 655f 6172  def normalize_ar
+000095d0: 7261 7928 6172 722c 206e 6577 5f6d 696e  ray(arr, new_min
+000095e0: 2c20 6e65 775f 6d61 7829 3a0d 0a20 2020  , new_max):..   
+000095f0: 2020 2020 2023 2020 2020 206d 696e 5f76       #     min_v
+00009600: 616c 203d 206e 702e 6d69 6e28 6172 7229  al = np.min(arr)
+00009610: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+00009620: 6d61 785f 7661 6c20 3d20 6e70 2e6d 6178  max_val = np.max
+00009630: 2861 7272 290d 0a20 2020 2020 2020 2023  (arr)..        #
+00009640: 2020 2020 206e 6f72 6d61 6c69 7a65 6420       normalized 
+00009650: 3d20 6e65 775f 6d69 6e20 2b20 2861 7272  = new_min + (arr
+00009660: 202d 206d 696e 5f76 616c 2920 2a20 286e   - min_val) * (n
+00009670: 6577 5f6d 6178 202d 206e 6577 5f6d 696e  ew_max - new_min
+00009680: 2920 2f20 286d 6178 5f76 616c 202d 206d  ) / (max_val - m
+00009690: 696e 5f76 616c 290d 0a20 2020 2020 2020  in_val)..       
+000096a0: 2023 2020 2020 2072 6574 7572 6e20 6e6f   #     return no
+000096b0: 726d 616c 697a 6564 0d0a 2020 2020 2020  rmalized..      
+000096c0: 2020 2320 7a7a 203d 206e 6f72 6d61 6c69    # zz = normali
+000096d0: 7a65 5f61 7272 6179 287a 7a2c 206d 696e  ze_array(zz, min
+000096e0: 5f72 616e 6765 2c20 6d61 785f 7261 6e67  _range, max_rang
+000096f0: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
+00009700: 2020 2020 2020 2320 2023 2043 6c69 7020        #  # Clip 
+00009710: 7468 6520 7661 6c75 6573 2074 6f20 7468  the values to th
+00009720: 6520 6465 7369 7265 6420 7261 6e67 650d  e desired range.
+00009730: 0a20 2020 2020 2020 2023 7a7a 203d 206e  .        #zz = n
+00009740: 702e 636c 6970 287a 7a2c 206d 696e 5f72  p.clip(zz, min_r
+00009750: 616e 6765 2c20 6d61 785f 7261 6e67 6529  ange, max_range)
+00009760: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00009770: 2020 2020 7a7a 5b7a 7a20 3c20 6d69 6e5f      zz[zz < min_
+00009780: 7261 6e67 655d 203d 206e 702e 6e61 6e0d  range] = np.nan.
+00009790: 0a20 2020 2020 2020 207a 7a5b 7a7a 203e  .        zz[zz >
+000097a0: 206d 6178 5f72 616e 6765 5d20 3d20 6e70   max_range] = np
+000097b0: 2e6e 616e 0d0a 2020 2020 2020 200d 0a20  .nan..       .. 
+000097c0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+000097d0: 2320 2320 4465 6669 6e65 2074 6865 2064  # # Define the d
+000097e0: 6573 6972 6564 2072 616e 6765 2062 6173  esired range bas
+000097f0: 6564 206f 6e20 796f 7572 2027 6461 7461  ed on your 'data
+00009800: 270d 0a20 2020 2020 2020 2023 2069 6620  '..        # if 
+00009810: 6c69 6d69 745f 6578 7465 6e64 3d3d 4661  limit_extend==Fa
+00009820: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00009830: 200d 0a20 2020 2020 2020 2023 2023 2023   ..        # # #
+00009840: 2023 204e 6f72 6d61 6c69 7a65 2027 7a7a   # Normalize 'zz
+00009850: 2720 746f 206d 6174 6368 2074 6865 2027  ' to match the '
+00009860: 6d69 6e5f 7261 6e67 6527 2061 6e64 2027  min_range' and '
+00009870: 6d61 785f 7261 6e67 6527 206f 6620 2764  max_range' of 'd
+00009880: 6174 6127 0d0a 2020 2020 2020 2020 2320  ata'..        # 
+00009890: 7a7a 203d 2028 7a7a 202d 206e 702e 6e61  zz = (zz - np.na
+000098a0: 6e6d 696e 287a 7a29 2920 2f20 286e 702e  nmin(zz)) / (np.
+000098b0: 6e61 6e6d 6178 287a 7a29 202d 206e 702e  nanmax(zz) - np.
+000098c0: 6e61 6e6d 696e 287a 7a29 290d 0a20 2020  nanmin(zz))..   
+000098d0: 2020 2020 2023 207a 7a20 3d20 7a7a 202a       # zz = zz *
+000098e0: 2028 6d61 785f 7261 6e67 6520 2d20 6d69   (max_range - mi
+000098f0: 6e5f 7261 6e67 6529 202b 206d 696e 5f72  n_range) + min_r
+00009900: 616e 6765 0d0a 2020 2020 2020 2020 0d0a  ange..        ..
+00009910: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00009920: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
+00009930: 287a 7a2e 7368 6170 6529 0d0a 2020 2020  (zz.shape)..    
+00009940: 2020 2020 2320 7072 696e 7428 7a7a 290d      # print(zz).
+00009950: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009960: 7a7a 2c20 612c 2062 2c20 632c 2064 6970  zz, a, b, c, dip
+00009970: 5f61 6e67 6c65 2c20 6469 705f 6469 7265  _angle, dip_dire
+00009980: 6374 696f 6e0d 0a20 2020 200d 0a20 2020  ction..    ..   
+00009990: 0d0a 2020 200d 0a20 2020 0d0a 0d0a 2020  ..   ..   ....  
+000099a0: 2020 6465 6620 6f6e 636c 6963 6b28 6576    def onclick(ev
+000099b0: 656e 742c 2070 6f69 6e74 732c 2064 6174  ent, points, dat
+000099c0: 612c 2074 7261 6e73 666f 726d 293a 0d0a  a, transform):..
+000099d0: 2020 2020 2020 2020 782c 2079 203d 2065          x, y = e
+000099e0: 7665 6e74 2e78 6461 7461 2c20 6576 656e  vent.xdata, even
+000099f0: 742e 7964 6174 610d 0a20 2020 2020 2020  t.ydata..       
+00009a00: 2063 6f6c 203d 2069 6e74 2828 7820 2d20   col = int((x - 
+00009a10: 7472 616e 7366 6f72 6d5b 305d 2920 2f20  transform[0]) / 
+00009a20: 7472 616e 7366 6f72 6d5b 315d 290d 0a20  transform[1]).. 
+00009a30: 2020 2020 2020 2072 6f77 203d 2069 6e74         row = int
+00009a40: 2828 7920 2d20 7472 616e 7366 6f72 6d5b  ((y - transform[
+00009a50: 335d 2920 2f20 7472 616e 7366 6f72 6d5b  3]) / transform[
+00009a60: 355d 290d 0a0d 0a20 2020 2020 2020 2069  5])....        i
+00009a70: 6620 3020 3c3d 2063 6f6c 203c 2064 6174  f 0 <= col < dat
+00009a80: 612e 7368 6170 655b 315d 2061 6e64 2030  a.shape[1] and 0
+00009a90: 203c 3d20 726f 7720 3c20 6461 7461 2e73   <= row < data.s
+00009aa0: 6861 7065 5b30 5d3a 0d0a 2020 2020 2020  hape[0]:..      
+00009ab0: 2020 2020 2020 7a20 3d20 6461 7461 5b72        z = data[r
+00009ac0: 6f77 2c20 636f 6c5d 0d0a 2020 2020 2020  ow, col]..      
+00009ad0: 2020 2020 2020 706f 696e 7473 2e61 7070        points.app
+00009ae0: 656e 6428 5b78 2c20 792c 207a 5d29 0d0a  end([x, y, z])..
+00009af0: 2020 2020 2020 2020 2020 2020 6178 5f32              ax_2
+00009b00: 642e 706c 6f74 2878 2c20 792c 2027 6f27  d.plot(x, y, 'o'
+00009b10: 2c20 636f 6c6f 723d 2762 6c61 636b 2729  , color='black')
+00009b20: 0d0a 2020 2020 2020 2020 2020 2020 6361  ..            ca
+00009b30: 6e76 6173 5f32 642e 6472 6177 2829 0d0a  nvas_2d.draw()..
+00009b40: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00009b50: 696e 745f 7374 7220 3d20 6622 783d 7b78  int_str = f"x={x
+00009b60: 3a2e 3266 7d2c 2079 3d7b 793a 2e32 667d  :.2f}, y={y:.2f}
+00009b70: 2c20 7a3d 7b7a 3a2e 3266 7d22 0d0a 2020  , z={z:.2f}"..  
+00009b80: 2020 2020 2020 2020 2020 706f 696e 7473            points
+00009b90: 5f6c 6973 7462 6f78 2e69 6e73 6572 7428  _listbox.insert(
+00009ba0: 746b 2e45 4e44 2c20 706f 696e 745f 7374  tk.END, point_st
+00009bb0: 7229 0d0a 0d0a 2020 2020 6465 6620 6f6e  r)....    def on
+00009bc0: 5f70 6f69 6e74 5f64 6f75 626c 655f 636c  _point_double_cl
+00009bd0: 6963 6b28 6576 656e 7429 3a0d 0a20 2020  ick(event):..   
+00009be0: 2020 2020 2067 6c6f 6261 6c20 706f 696e       global poin
+00009bf0: 7473 2c20 6178 5f32 642c 2070 6f69 6e74  ts, ax_2d, point
+00009c00: 735f 6c69 7374 626f 782c 2068 730d 0a20  s_listbox, hs.. 
+00009c10: 2020 2020 2020 2069 6478 203d 2070 6f69         idx = poi
+00009c20: 6e74 735f 6c69 7374 626f 782e 6375 7273  nts_listbox.curs
+00009c30: 656c 6563 7469 6f6e 2829 5b30 5d20 2023  election()[0]  #
+00009c40: 2049 6e64 6578 206f 6620 7365 6c65 6374   Index of select
+00009c50: 6564 2070 6f69 6e74 2069 6e20 7468 6520  ed point in the 
+00009c60: 6c69 7374 626f 780d 0a20 2020 2020 2020  listbox..       
+00009c70: 2070 6f69 6e74 203d 2070 6f69 6e74 735b   point = points[
+00009c80: 6964 785d 0d0a 2020 2020 2020 2020 0d0a  idx]..        ..
+00009c90: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
+00009ca0: 2074 6865 2070 6f69 6e74 2066 726f 6d20   the point from 
+00009cb0: 6f75 7220 6461 7461 0d0a 2020 2020 2020  our data..      
+00009cc0: 2020 706f 696e 7473 2e70 6f70 2869 6478    points.pop(idx
+00009cd0: 290d 0a20 2020 2020 2020 2070 6f69 6e74  )..        point
+00009ce0: 735f 6c69 7374 626f 782e 6465 6c65 7465  s_listbox.delete
+00009cf0: 2869 6478 290d 0a0d 0a20 2020 2020 2020  (idx)....       
+00009d00: 2023 2049 6465 6e74 6966 7920 616e 6420   # Identify and 
+00009d10: 7265 6d6f 7665 2074 6865 2063 6f72 7265  remove the corre
+00009d20: 7370 6f6e 6469 6e67 2070 6f69 6e74 2066  sponding point f
+00009d30: 726f 6d20 7468 6520 6178 5f32 6420 706c  rom the ax_2d pl
+00009d40: 6f74 0d0a 2020 2020 2020 2020 666f 7220  ot..        for 
+00009d50: 6c69 6e65 2069 6e20 6178 5f32 642e 6c69  line in ax_2d.li
+00009d60: 6e65 733a 0d0a 2020 2020 2020 2020 2020  nes:..          
+00009d70: 2020 7864 6174 612c 2079 6461 7461 203d    xdata, ydata =
+00009d80: 206c 696e 652e 6765 745f 7864 6174 6128   line.get_xdata(
+00009d90: 292c 206c 696e 652e 6765 745f 7964 6174  ), line.get_ydat
+00009da0: 6128 290d 0a20 2020 2020 2020 2020 2020  a()..           
+00009db0: 2069 6620 7864 6174 615b 305d 203d 3d20   if xdata[0] == 
+00009dc0: 706f 696e 745b 305d 2061 6e64 2079 6461  point[0] and yda
+00009dd0: 7461 5b30 5d20 3d3d 2070 6f69 6e74 5b31  ta[0] == point[1
+00009de0: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+00009df0: 2020 2020 6c69 6e65 2e72 656d 6f76 6528      line.remove(
+00009e00: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00009e10: 2020 2062 7265 616b 0d0a 0d0a 2020 2020     break....    
+00009e20: 2020 2020 6361 6e76 6173 5f32 642e 6472      canvas_2d.dr
+00009e30: 6177 2829 0d0a 2020 2020 2020 2020 0d0a  aw()..        ..
+00009e40: 2020 2020 2020 2020 0d0a 2020 2020 0d0a          ..    ..
+00009e50: 2020 2020 0d0a 2020 2020 6465 6620 706c      ..    def pl
+00009e60: 6f74 5f70 6c61 6e65 7328 6469 705f 6c69  ot_planes(dip_li
+00009e70: 7374 2c20 617a 696d 7574 685f 6c69 7374  st, azimuth_list
+00009e80: 2c20 7267 625f 636f 6c6f 7273 2c20 6f75  , rgb_colors, ou
+00009e90: 745f 706c 616e 6546 6f6c 6465 723d 6f75  t_planeFolder=ou
+00009ea0: 745f 706c 616e 6546 6f6c 6465 7229 3a0d  t_planeFolder):.
+00009eb0: 0a20 2020 2020 2020 2023 6672 6f6d 206d  .        #from m
+00009ec0: 706c 7374 6572 656f 6e65 7420 696d 706f  plstereonet impo
+00009ed0: 7274 2053 7465 7265 6f6e 6574 4178 6573  rt StereonetAxes
+00009ee0: 0d0a 2020 2020 2020 2020 2023 2043 7265  ..         # Cre
+00009ef0: 6174 6520 6120 7374 6572 656f 206e 6574  ate a stereo net
+00009f00: 2070 6c6f 740d 0a20 2020 2020 2020 2066   plot..        f
+00009f10: 6967 203d 2070 6c74 2e66 6967 7572 6528  ig = plt.figure(
+00009f20: 6669 6773 697a 653d 2831 302c 2031 3029  figsize=(10, 10)
+00009f30: 2c20 6470 693d 3330 3029 0d0a 2020 2020  , dpi=300)..    
+00009f40: 2020 2020 2361 7820 3d20 6669 672e 6164      #ax = fig.ad
+00009f50: 645f 7375 6270 6c6f 7428 3132 312c 2070  d_subplot(121, p
+00009f60: 726f 6a65 6374 696f 6e3d 2773 7465 7265  rojection='stere
+00009f70: 6f6e 6574 2729 0d0a 2020 2020 2020 2020  onet')..        
+00009f80: 6178 3d66 6967 2e61 6464 5f73 7562 706c  ax=fig.add_subpl
+00009f90: 6f74 2831 3231 2c20 706f 6c61 723d 5472  ot(121, polar=Tr
+00009fa0: 7565 290d 0a0d 0a20 2020 2020 2020 2066  ue)....        f
+00009fb0: 6f72 2064 6970 5f61 6e67 6c65 732c 2064  or dip_angles, d
+00009fc0: 6970 5f64 6972 6563 7469 6f6e 732c 2063  ip_directions, c
+00009fd0: 6f6c 6f72 2069 6e20 7a69 7028 6469 705f  olor in zip(dip_
+00009fe0: 6c69 7374 2c20 617a 696d 7574 685f 6c69  list, azimuth_li
+00009ff0: 7374 2c20 7267 625f 636f 6c6f 7273 293a  st, rgb_colors):
+0000a000: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000a010: 436f 6e76 6572 7420 6469 7020 6469 7265  Convert dip dire
+0000a020: 6374 696f 6e73 2061 6e64 2064 6970 2061  ctions and dip a
+0000a030: 6e67 6c65 7320 746f 2072 6164 6961 6e73  ngles to radians
+0000a040: 0d0a 2020 2020 2020 2020 2020 2020 2364  ..            #d
+0000a050: 6970 5f64 6972 6563 7469 6f6e 7320 3d20  ip_directions = 
+0000a060: 2864 6970 5f64 6972 6563 7469 6f6e 7320  (dip_directions 
+0000a070: 2b20 3930 2920 2520 3336 3020 2363 6f6e  + 90) % 360 #con
+0000a080: 7665 7274 6564 2064 6970 2064 6972 6563  verted dip direc
+0000a090: 7469 6f6e 2074 6f20 7374 7269 6b65 0d0a  tion to strike..
+0000a0a0: 2020 2020 2020 2020 2020 2020 6469 705f              dip_
+0000a0b0: 616e 676c 6573 203d 2028 3930 202d 206e  angles = (90 - n
+0000a0c0: 702e 6172 7261 7928 6469 705f 616e 676c  p.array(dip_angl
+0000a0d0: 6573 2929 2020 2320 436f 6e76 6572 7420  es))  # Convert 
+0000a0e0: 6469 7020 616e 676c 6573 2074 6f20 636f  dip angles to co
+0000a0f0: 6d70 6c65 6d65 6e74 6172 7920 616e 676c  mplementary angl
+0000a100: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+0000a110: 2023 2043 6f6e 7665 7274 2064 6970 2061   # Convert dip a
+0000a120: 7a69 6d75 7468 7320 746f 2072 6164 6961  zimuths to radia
+0000a130: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
+0000a140: 6469 705f 617a 696d 7574 6873 5f72 6164  dip_azimuths_rad
+0000a150: 203d 206e 702e 7261 6469 616e 7328 6469   = np.radians(di
+0000a160: 705f 6469 7265 6374 696f 6e73 290d 0a20  p_directions).. 
+0000a170: 2020 2020 2020 2020 2020 2023 2050 6c6f             # Plo
+0000a180: 7420 7468 6520 706f 6c65 7320 6f66 2070  t the poles of p
+0000a190: 6c61 6e65 7320 6173 2064 6f74 730d 0a20  lanes as dots.. 
+0000a1a0: 2020 2020 2020 2020 2020 2061 782e 7363             ax.sc
+0000a1b0: 6174 7465 7228 6469 705f 617a 696d 7574  atter(dip_azimut
+0000a1c0: 6873 5f72 6164 2c20 6469 705f 616e 676c  hs_rad, dip_angl
+0000a1d0: 6573 2c20 636f 6c6f 723d 636f 6c6f 7229  es, color=color)
+0000a1e0: 2020 200d 0a0d 0a20 2020 2020 2020 2061     ....        a
+0000a1f0: 782e 6772 6964 2854 7275 6529 0d0a 2020  x.grid(True)..  
+0000a200: 2020 2020 2020 6178 2e73 6574 5f74 6865        ax.set_the
+0000a210: 7461 5f7a 6572 6f5f 6c6f 6361 7469 6f6e  ta_zero_location
+0000a220: 2827 4e27 2920 2023 2053 6574 2030 2064  ('N')  # Set 0 d
+0000a230: 6567 7265 6573 2061 7420 7468 6520 746f  egrees at the to
+0000a240: 700d 0a20 2020 2020 2020 2061 782e 7365  p..        ax.se
+0000a250: 745f 7468 6574 615f 6469 7265 6374 696f  t_theta_directio
+0000a260: 6e28 2d31 2920 2023 2052 6576 6572 7365  n(-1)  # Reverse
+0000a270: 2074 6865 2064 6972 6563 7469 6f6e 206f   the direction o
+0000a280: 6620 7468 6520 616e 676c 6573 0d0a 0d0a  f the angles....
+0000a290: 2020 2020 2020 2020 2320 5365 7420 6c61          # Set la
+0000a2a0: 6265 6c73 2066 6f72 2063 6172 6469 6e61  bels for cardina
+0000a2b0: 6c20 6469 7265 6374 696f 6e73 0d0a 2020  l directions..  
+0000a2c0: 2020 2020 2020 6178 2e73 6574 5f78 7469        ax.set_xti
+0000a2d0: 636b 7328 6e70 2e72 6164 6961 6e73 285b  cks(np.radians([
+0000a2e0: 302c 2034 352c 2039 302c 2031 3335 2c20  0, 45, 90, 135, 
+0000a2f0: 3138 302c 2032 3235 2c20 3237 302c 2033  180, 225, 270, 3
+0000a300: 3135 5d29 290d 0a20 2020 2020 2020 2061  15]))..        a
+0000a310: 782e 7365 745f 7874 6963 6b6c 6162 656c  x.set_xticklabel
+0000a320: 7328 5b27 4e27 2c20 274e 4527 2c20 2745  s(['N', 'NE', 'E
+0000a330: 272c 2027 5345 272c 2027 5327 2c20 2753  ', 'SE', 'S', 'S
+0000a340: 5727 2c20 2757 272c 2027 4e57 275d 290d  W', 'W', 'NW']).
+0000a350: 0a0d 0a20 2020 2020 2020 2023 2053 6574  ...        # Set
+0000a360: 2074 6865 2072 6164 6961 6c20 6772 6964   the radial grid
+0000a370: 2061 6e64 206c 6162 656c 730d 0a20 2020   and labels..   
+0000a380: 2020 2020 2061 782e 7365 745f 726c 6162       ax.set_rlab
+0000a390: 656c 5f70 6f73 6974 696f 6e28 3930 290d  el_position(90).
+0000a3a0: 0a20 2020 2020 2020 2061 782e 7365 745f  .        ax.set_
+0000a3b0: 7974 6963 6b73 285b 3135 2c20 3330 2c20  yticks([15, 30, 
+0000a3c0: 3435 2c20 3630 2c20 3735 5d29 0d0a 2020  45, 60, 75])..  
+0000a3d0: 2020 2020 2020 6178 2e73 6574 5f72 6d61        ax.set_rma
+0000a3e0: 7828 3930 2920 2023 2053 6574 2074 6865  x(90)  # Set the
+0000a3f0: 206d 6178 696d 756d 2072 6164 6961 6c20   maximum radial 
+0000a400: 6469 7374 616e 6365 0d0a 2020 2020 2020  distance..      
+0000a410: 2020 6178 2e73 6574 5f74 6974 6c65 2822    ax.set_title("
+0000a420: 506f 6c65 7320 746f 2050 6c61 6e65 7322  Poles to Planes"
+0000a430: 290d 0a20 2020 2020 2020 2023 2043 7573  )..        # Cus
+0000a440: 746f 6d69 7a65 2074 6963 6b20 6d61 726b  tomize tick mark
+0000a450: 7320 2d20 7370 6563 6966 7920 616e 676c  s - specify angl
+0000a460: 6573 2069 6e20 7261 6469 616e 730d 0a20  es in radians.. 
+0000a470: 2020 2020 2020 2023 2061 782e 7365 745f         # ax.set_
+0000a480: 7874 6963 6b73 286e 702e 7261 6469 616e  xticks(np.radian
+0000a490: 7328 7261 6e67 6528 302c 2033 3630 2c20  s(range(0, 360, 
+0000a4a0: 3130 2929 2920 2023 2031 302d 6465 6772  10)))  # 10-degr
+0000a4b0: 6565 2069 6e74 6572 7661 6c73 0d0a 2020  ee intervals..  
+0000a4c0: 2020 2020 2020 2320 6178 2e73 6574 5f79        # ax.set_y
+0000a4d0: 7469 636b 7328 6e70 2e72 6164 6961 6e73  ticks(np.radians
+0000a4e0: 2872 616e 6765 282d 3930 2c20 3930 2c20  (range(-90, 90, 
+0000a4f0: 3130 2929 290d 0a0d 0a20 2020 2020 2020  10)))....       
+0000a500: 2073 7472 696b 6573 3d5b 5d0d 0a20 2020   strikes=[]..   
+0000a510: 2020 2020 2061 6c6c 5f63 6f6c 6f72 733d       all_colors=
+0000a520: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+0000a530: 6469 705f 616e 676c 6573 2c20 6469 705f  dip_angles, dip_
+0000a540: 6469 7265 6374 696f 6e73 2c20 636f 6c6f  directions, colo
+0000a550: 7220 696e 207a 6970 2864 6970 5f6c 6973  r in zip(dip_lis
+0000a560: 742c 2061 7a69 6d75 7468 5f6c 6973 742c  t, azimuth_list,
+0000a570: 2072 6762 5f63 6f6c 6f72 7329 3a0d 0a20   rgb_colors):.. 
+0000a580: 2020 2020 2020 2020 2020 2064 6970 5f61             dip_a
+0000a590: 7a69 6d75 7468 735f 7261 6420 3d20 6e70  zimuths_rad = np
+0000a5a0: 2e72 6164 6961 6e73 2864 6970 5f64 6972  .radians(dip_dir
+0000a5b0: 6563 7469 6f6e 7329 0d0a 2020 2020 2020  ections)..      
+0000a5c0: 2020 2020 2020 2364 6970 5f64 6972 6563        #dip_direc
+0000a5d0: 7469 6f6e 7320 3d20 2864 6970 5f64 6972  tions = (dip_dir
+0000a5e0: 6563 7469 6f6e 7320 2b20 3930 2920 2520  ections + 90) % 
+0000a5f0: 3336 300d 0a20 2020 2020 2020 2020 2020  360..           
+0000a600: 2064 6970 5f61 6e67 6c65 7320 3d20 2839   dip_angles = (9
+0000a610: 3020 2d20 6e70 2e61 7272 6179 2864 6970  0 - np.array(dip
+0000a620: 5f61 6e67 6c65 7329 2920 2023 2043 6f6e  _angles))  # Con
+0000a630: 7665 7274 2064 6970 2061 6e67 6c65 7320  vert dip angles 
+0000a640: 746f 2063 6f6d 706c 656d 656e 7461 7279  to complementary
+0000a650: 2061 6e67 6c65 730d 0a20 2020 2020 2020   angles..       
+0000a660: 2020 2020 2073 7472 696b 6573 2e61 7070       strikes.app
+0000a670: 656e 6428 2864 6970 5f61 7a69 6d75 7468  end((dip_azimuth
+0000a680: 735f 7261 6420 2b20 3930 2920 2520 3336  s_rad + 90) % 36
+0000a690: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
+0000a6a0: 616c 6c5f 636f 6c6f 7273 2e61 7070 656e  all_colors.appen
+0000a6b0: 6428 636f 6c6f 7229 0d0a 2020 2020 2020  d(color)..      
+0000a6c0: 2020 0d0a 0d0a 2020 2020 2020 2020 2023    ....         #
+0000a6d0: 2043 616c 6375 6c61 7465 2074 6865 206e   Calculate the n
+0000a6e0: 756d 6265 7220 6f66 2062 696e 7320 7573  umber of bins us
+0000a6f0: 696e 6720 5363 6f74 7427 7320 5275 6c65  ing Scott's Rule
+0000a700: 0d0a 2020 2020 2020 2020 6e20 3d20 6c65  ..        n = le
+0000a710: 6e28 7374 7269 6b65 7329 0d0a 0d0a 2020  n(strikes)....  
+0000a720: 2020 2020 2020 2320 4361 6c63 756c 6174        # Calculat
+0000a730: 6520 7468 6520 7374 616e 6461 7264 2064  e the standard d
+0000a740: 6576 6961 7469 6f6e 206f 6620 7468 6520  eviation of the 
+0000a750: 6461 7461 0d0a 2020 2020 2020 2020 7374  data..        st
+0000a760: 645f 6465 7620 3d20 6e70 2e6e 616e 7374  d_dev = np.nanst
+0000a770: 6428 7374 7269 6b65 7329 0d0a 2020 2020  d(strikes)..    
+0000a780: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+0000a790: 6d61 7820 616e 6420 6d69 6e2c 2069 676e  max and min, ign
+0000a7a0: 6f72 696e 6720 4e61 4e20 7661 6c75 6573  oring NaN values
+0000a7b0: 0d0a 2020 2020 2020 2020 6d61 785f 7374  ..        max_st
+0000a7c0: 7269 6b65 203d 206e 702e 6e61 6e6d 6178  rike = np.nanmax
+0000a7d0: 2873 7472 696b 6573 290d 0a20 2020 2020  (strikes)..     
+0000a7e0: 2020 206d 696e 5f73 7472 696b 6520 3d20     min_strike = 
+0000a7f0: 6e70 2e6e 616e 6d69 6e28 7374 7269 6b65  np.nanmin(strike
+0000a800: 7329 0d0a 2020 2020 2020 2020 2320 4361  s)..        # Ca
+0000a810: 6c63 756c 6174 6520 7468 6520 6269 6e20  lculate the bin 
+0000a820: 7769 6474 6820 7573 696e 6720 5363 6f74  width using Scot
+0000a830: 7427 7320 5275 6c65 2066 6f72 6d75 6c61  t's Rule formula
+0000a840: 2c20 656e 7375 7269 6e67 2069 7427 7320  , ensuring it's 
+0000a850: 6e6f 7420 7a65 726f 0d0a 2020 2020 2020  not zero..      
+0000a860: 2020 6966 2073 7464 5f64 6576 2021 3d20    if std_dev != 
+0000a870: 303a 0d0a 2020 2020 2020 2020 2020 2020  0:..            
+0000a880: 6269 6e5f 7769 6474 6820 3d20 302e 3520  bin_width = 0.5 
+0000a890: 2a20 7374 645f 6465 7620 2f20 286e 2a2a  * std_dev / (n**
+0000a8a0: 2831 2f33 2929 2020 2320 5363 6f74 7427  (1/3))  # Scott'
+0000a8b0: 7320 5275 6c65 2066 6f72 6d75 6c61 0d0a  s Rule formula..
+0000a8c0: 2020 2020 2020 2020 2020 2020 236e 756d              #num
+0000a8d0: 5f62 696e 7320 3d20 6d61 7828 696e 7428  _bins = max(int(
+0000a8e0: 286d 6178 2873 7472 696b 6573 2920 2d20  (max(strikes) - 
+0000a8f0: 6d69 6e28 7374 7269 6b65 7329 2920 2f20  min(strikes)) / 
+0000a900: 6269 6e5f 7769 6474 6829 2c20 3129 2020  bin_width), 1)  
+0000a910: 2320 456e 7375 7265 206e 756d 5f62 696e  # Ensure num_bin
+0000a920: 7320 6973 2061 7420 6c65 6173 7420 310d  s is at least 1.
+0000a930: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+0000a940: 5f62 696e 7320 3d20 6d61 7828 696e 7428  _bins = max(int(
+0000a950: 286d 6178 5f73 7472 696b 6520 2d20 6d69  (max_strike - mi
+0000a960: 6e5f 7374 7269 6b65 2920 2f20 6269 6e5f  n_strike) / bin_
+0000a970: 7769 6474 6829 2c20 3129 2020 2320 456e  width), 1)  # En
+0000a980: 7375 7265 206e 756d 5f62 696e 7320 6973  sure num_bins is
+0000a990: 2061 7420 6c65 6173 7420 310d 0a20 2020   at least 1..   
+0000a9a0: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0000a9b0: 2020 2020 2020 2020 6e75 6d5f 6269 6e73          num_bins
+0000a9c0: 203d 2031 3220 2023 2041 2064 6566 6175   = 12  # A defau
+0000a9d0: 6c74 206e 756d 6265 7220 6f66 2062 696e  lt number of bin
+0000a9e0: 7320 6966 2073 7464 5f64 6576 2069 7320  s if std_dev is 
+0000a9f0: 7a65 726f 0d0a 2020 2020 2020 2020 2320  zero..        # 
+0000aa00: 4372 6561 7465 2061 2072 6f73 6520 6469  Create a rose di
+0000aa10: 6167 7261 6d20 2863 6972 6375 6c61 7220  agram (circular 
+0000aa20: 6869 7374 6f67 7261 6d29 0d0a 2020 2020  histogram)..    
+0000aa30: 2020 2020 6178 5f72 6f73 6520 3d20 6669      ax_rose = fi
+0000aa40: 672e 6164 645f 7375 6270 6c6f 7428 3132  g.add_subplot(12
+0000aa50: 322c 2070 6f6c 6172 3d54 7275 6529 0d0a  2, polar=True)..
+0000aa60: 0d0a 2020 2020 2020 2020 666f 7220 6469  ..        for di
+0000aa70: 702c 2073 7472 696b 652c 2063 6f6c 6f72  p, strike, color
+0000aa80: 2c20 617a 2069 6e20 7a69 7028 6469 705f  , az in zip(dip_
+0000aa90: 6c69 7374 2c20 7374 7269 6b65 732c 2061  list, strikes, a
+0000aaa0: 6c6c 5f63 6f6c 6f72 732c 2061 7a69 6d75  ll_colors, azimu
+0000aab0: 7468 5f6c 6973 7429 3a0d 0a20 2020 2020  th_list):..     
+0000aac0: 2020 2020 2020 2023 2043 6f6e 7665 7274         # Convert
+0000aad0: 2064 6970 2061 7a69 6d75 7468 7320 746f   dip azimuths to
+0000aae0: 2072 6164 6961 6e73 0d0a 2020 2020 2020   radians..      
+0000aaf0: 2020 2020 2020 6469 705f 617a 696d 7574        dip_azimut
+0000ab00: 6873 5f72 6164 203d 206e 702e 7261 6469  hs_rad = np.radi
+0000ab10: 616e 7328 617a 290d 0a20 2020 2020 2020  ans(az)..       
+0000ab20: 2020 2020 2064 6970 5f61 6e67 6c65 7320       dip_angles 
+0000ab30: 3d20 2839 3020 2d20 6e70 2e61 7272 6179  = (90 - np.array
+0000ab40: 2864 6970 5f61 6e67 6c65 7329 2920 2023  (dip_angles))  #
+0000ab50: 2043 6f6e 7665 7274 2064 6970 2061 6e67   Convert dip ang
+0000ab60: 6c65 7320 746f 2063 6f6d 706c 656d 656e  les to complemen
+0000ab70: 7461 7279 2061 6e67 6c65 730d 0a20 2020  tary angles..   
+0000ab80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000ab90: 2020 2020 2020 2023 2050 6c6f 7420 6469         # Plot di
+0000aba0: 7020 616e 676c 6573 2061 7320 7261 6469  p angles as radi
+0000abb0: 6920 616e 6420 6469 7020 617a 696d 7574  i and dip azimut
+0000abc0: 6873 2061 7320 616e 676c 6573 0d0a 2020  hs as angles..  
+0000abd0: 2020 2020 2020 2020 2020 2361 785f 726f            #ax_ro
+0000abe0: 7365 2e73 6361 7474 6572 2864 6970 5f61  se.scatter(dip_a
+0000abf0: 7a69 6d75 7468 735f 7261 642c 2064 6970  zimuths_rad, dip
+0000ac00: 5f61 6e67 6c65 732c 2063 3d63 6f6c 6f72  _angles, c=color
+0000ac10: 2c20 616c 7068 613d 302e 3529 0d0a 2020  , alpha=0.5)..  
+0000ac20: 2020 2020 2020 2020 2020 2320 506c 6f74            # Plot
+0000ac30: 2074 6865 206f 7269 656e 7461 7469 6f6e   the orientation
+0000ac40: 2064 6174 6120 6173 2061 2072 6f73 6520   data as a rose 
+0000ac50: 6469 6167 7261 6d0d 0a20 2020 2020 2020  diagram..       
+0000ac60: 2020 2020 206e 2c20 6269 6e73 2c20 7061       n, bins, pa
+0000ac70: 7463 6865 733d 6178 5f72 6f73 652e 6869  tches=ax_rose.hi
+0000ac80: 7374 2873 7472 696b 652c 2062 696e 733d  st(strike, bins=
+0000ac90: 6e75 6d5f 6269 6e73 2c20 636f 6c6f 723d  num_bins, color=
+0000aca0: 636f 6c6f 722c 2061 6c70 6861 3d30 2e35  color, alpha=0.5
+0000acb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000acc0: 2320 416e 6e6f 7461 7465 2074 6865 206e  # Annotate the n
+0000acd0: 756d 6265 7220 6f66 2064 6174 6120 706f  umber of data po
+0000ace0: 696e 7473 2061 6e64 2062 696e 206e 756d  ints and bin num
+0000acf0: 6265 720d 0a20 2020 2020 2020 2020 2020  ber..           
+0000ad00: 2061 785f 726f 7365 2e74 6578 7428 302c   ax_rose.text(0,
+0000ad10: 202d 302e 312c 2066 2244 6174 6120 506f   -0.1, f"Data Po
+0000ad20: 696e 7473 3a20 7b6c 656e 2873 7472 696b  ints: {len(strik
+0000ad30: 6573 297d 222c 2068 613d 2763 656e 7465  es)}", ha='cente
+0000ad40: 7227 2c20 7661 3d27 6365 6e74 6572 272c  r', va='center',
+0000ad50: 2074 7261 6e73 666f 726d 3d61 785f 726f   transform=ax_ro
+0000ad60: 7365 2e74 7261 6e73 4178 6573 290d 0a20  se.transAxes).. 
+0000ad70: 2020 2020 2020 2020 2020 2061 785f 726f             ax_ro
+0000ad80: 7365 2e74 6578 7428 302c 202d 302e 3135  se.text(0, -0.15
+0000ad90: 2c20 6622 4269 6e20 436f 756e 743a 207b  , f"Bin Count: {
+0000ada0: 6e75 6d5f 6269 6e73 7d22 2c20 6861 3d27  num_bins}", ha='
+0000adb0: 6365 6e74 6572 272c 2076 613d 2763 656e  center', va='cen
+0000adc0: 7465 7227 2c20 7472 616e 7366 6f72 6d3d  ter', transform=
+0000add0: 6178 5f72 6f73 652e 7472 616e 7341 7865  ax_rose.transAxe
+0000ade0: 7329 0d0a 0d0a 2020 2020 2020 2020 2320  s)....        # 
+0000adf0: 2320 4375 7374 6f6d 697a 6520 7468 6520  # Customize the 
+0000ae00: 726f 7365 2064 6961 6772 616d 0d0a 2020  rose diagram..  
+0000ae10: 2020 2020 2020 2320 6178 5f72 6f73 652e        # ax_rose.
+0000ae20: 7365 745f 7468 6574 615f 7a65 726f 5f6c  set_theta_zero_l
+0000ae30: 6f63 6174 696f 6e28 224e 2229 0d0a 2020  ocation("N")..  
+0000ae40: 2020 2020 2020 2320 6178 5f72 6f73 652e        # ax_rose.
+0000ae50: 7365 745f 7468 6574 615f 6469 7265 6374  set_theta_direct
+0000ae60: 696f 6e28 2d31 290d 0a20 2020 2020 2020  ion(-1)..       
+0000ae70: 2023 2043 7573 746f 6d69 7a65 2074 6865   # Customize the
+0000ae80: 2070 6f6c 6172 2070 6c6f 740d 0a20 2020   polar plot..   
+0000ae90: 2020 2020 2061 785f 726f 7365 2e73 6574       ax_rose.set
+0000aea0: 5f74 6865 7461 5f7a 6572 6f5f 6c6f 6361  _theta_zero_loca
+0000aeb0: 7469 6f6e 2827 4e27 2920 2023 2053 6574  tion('N')  # Set
+0000aec0: 2030 2064 6567 7265 6573 2061 7420 7468   0 degrees at th
+0000aed0: 6520 746f 700d 0a20 2020 2020 2020 2061  e top..        a
+0000aee0: 785f 726f 7365 2e73 6574 5f74 6865 7461  x_rose.set_theta
+0000aef0: 5f64 6972 6563 7469 6f6e 282d 3129 2020  _direction(-1)  
+0000af00: 2320 5265 7665 7273 6520 7468 6520 6469  # Reverse the di
+0000af10: 7265 6374 696f 6e20 6f66 2074 6865 2061  rection of the a
+0000af20: 6e67 6c65 730d 0a0d 0a20 2020 2020 2020  ngles....       
+0000af30: 2023 2053 6574 206c 6162 656c 7320 666f   # Set labels fo
+0000af40: 7220 6361 7264 696e 616c 2064 6972 6563  r cardinal direc
+0000af50: 7469 6f6e 730d 0a20 2020 2020 2020 2061  tions..        a
+0000af60: 785f 726f 7365 2e73 6574 5f78 7469 636b  x_rose.set_xtick
+0000af70: 7328 6e70 2e72 6164 6961 6e73 285b 302c  s(np.radians([0,
+0000af80: 2034 352c 2039 302c 2031 3335 2c20 3138   45, 90, 135, 18
+0000af90: 302c 2032 3235 2c20 3237 302c 2033 3135  0, 225, 270, 315
+0000afa0: 5d29 290d 0a20 2020 2020 2020 2061 785f  ]))..        ax_
+0000afb0: 726f 7365 2e73 6574 5f78 7469 636b 6c61  rose.set_xtickla
+0000afc0: 6265 6c73 285b 274e 272c 2027 4e45 272c  bels(['N', 'NE',
+0000afd0: 2027 4527 2c20 2753 4527 2c20 2753 272c   'E', 'SE', 'S',
+0000afe0: 2027 5357 272c 2027 5727 2c20 274e 5727   'SW', 'W', 'NW'
+0000aff0: 5d29 0d0a 2020 2020 2020 200d 0a0d 0a20  ])..       .... 
+0000b000: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
+0000b010: 2072 6164 6961 6c20 6772 6964 2061 6e64   radial grid and
+0000b020: 206c 6162 656c 730d 0a20 2020 2020 2020   labels..       
+0000b030: 2023 2061 785f 726f 7365 2e73 6574 5f72   # ax_rose.set_r
+0000b040: 6c61 6265 6c5f 706f 7369 7469 6f6e 2839  label_position(9
+0000b050: 3029 0d0a 2020 2020 2020 2020 2320 6178  0)..        # ax
+0000b060: 5f72 6f73 652e 7365 745f 7974 6963 6b73  _rose.set_yticks
+0000b070: 285b 3135 2c20 3330 2c20 3435 2c20 3630  ([15, 30, 45, 60
+0000b080: 2c20 3735 5d29 0d0a 2020 2020 2020 2020  , 75])..        
+0000b090: 2320 6178 5f72 6f73 652e 7365 745f 726d  # ax_rose.set_rm
+0000b0a0: 6178 2839 3029 2020 2320 5365 7420 7468  ax(90)  # Set th
+0000b0b0: 6520 6d61 7869 6d75 6d20 7261 6469 616c  e maximum radial
+0000b0c0: 2064 6973 7461 6e63 650d 0a20 2020 2020   distance..     
+0000b0d0: 2020 2061 785f 726f 7365 2e73 6574 5f74     ax_rose.set_t
+0000b0e0: 6974 6c65 2822 526f 7365 2044 6961 6772  itle("Rose Diagr
+0000b0f0: 616d 2053 7472 696b 6522 290d 0a0d 0a20  am Strike").... 
+0000b100: 2020 2020 2020 2023 2041 646a 7573 7420         # Adjust 
+0000b110: 7370 6163 696e 6720 6265 7477 6565 6e20  spacing between 
+0000b120: 7375 6270 6c6f 7473 0d0a 2020 2020 2020  subplots..      
+0000b130: 2020 706c 742e 7375 6270 6c6f 7473 5f61    plt.subplots_a
+0000b140: 646a 7573 7428 7773 7061 6365 3d30 2e32  djust(wspace=0.2
+0000b150: 290d 0a0d 0a20 2020 2020 2020 2070 6c74  )....        plt
+0000b160: 2e73 6176 6566 6967 286f 7574 5f70 6c61  .savefig(out_pla
+0000b170: 6e65 466f 6c64 6572 202b 2022 2f22 202b  neFolder + "/" +
+0000b180: 2022 7374 6572 656f 706c 6f74 2e70 6e67   "stereoplot.png
+0000b190: 222c 2064 7069 3d33 3030 290d 0a20 2020  ", dpi=300)..   
+0000b1a0: 2020 2020 2070 6c74 2e74 6967 6874 5f6c       plt.tight_l
+0000b1b0: 6179 6f75 740d 0a20 2020 2020 2020 2023  ayout..        #
+0000b1c0: 706c 742e 636c 6f73 6528 290d 0a20 2020  plt.close()..   
+0000b1d0: 2020 2020 2070 6c74 2e63 6c6f 7365 2829       plt.close()
+0000b1e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000b1f0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
+0000b200: 0d0a 2020 2020 6465 6620 6472 6177 5f70  ..    def draw_p
+0000b210: 6c61 6e65 2878 782c 7979 293a 0d0a 2020  lane(xx,yy):..  
+0000b220: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000b230: 6966 206c 656e 2870 6f69 6e74 7329 203e  if len(points) >
+0000b240: 3d20 333a 0d0a 2020 2020 2020 2020 2020  = 3:..          
+0000b250: 2020 6669 7474 6564 5f70 6c61 6e65 2c20    fitted_plane, 
+0000b260: 612c 2062 2c20 6320 2c20 6469 705f 616e  a, b, c , dip_an
+0000b270: 676c 652c 2064 6970 5f64 6972 6563 7469  gle, dip_directi
+0000b280: 6f6e 203d 2066 6974 5f70 6c61 6e65 2870  on = fit_plane(p
+0000b290: 6f69 6e74 732c 2078 782c 2079 7929 0d0a  oints, xx, yy)..
+0000b2a0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000b2b0: 2020 2020 2020 2020 2020 6469 705f 616e            dip_an
+0000b2c0: 676c 655f 6c69 7374 2e61 7070 656e 6428  gle_list.append(
+0000b2d0: 6469 705f 616e 676c 6529 0d0a 2020 2020  dip_angle)..    
+0000b2e0: 2020 2020 2020 2020 6469 705f 6469 7265          dip_dire
+0000b2f0: 6374 696f 6e5f 6c69 7374 2e61 7070 656e  ction_list.appen
+0000b300: 6428 6469 705f 6469 7265 6374 696f 6e29  d(dip_direction)
+0000b310: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000b320: 2020 2020 2020 2020 2020 2020 2320 6966              # if
+0000b330: 206c 696d 6974 5f65 7874 656e 643a 0d0a   limit_extend:..
+0000b340: 2020 2020 2020 2020 2020 2020 2320 2023              #  #
+0000b350: 4765 7420 626f 756e 6469 6e67 2062 6f78  Get bounding box
+0000b360: 206f 6620 7468 6520 7365 6c65 6374 6564   of the selected
+0000b370: 2070 6f69 6e74 730d 0a20 2020 2020 2020   points..       
+0000b380: 2020 2020 2023 2020 2020 2078 6d69 6e2c       #     xmin,
+0000b390: 2078 6d61 782c 2079 6d69 6e2c 2079 6d61   xmax, ymin, yma
+0000b3a0: 7820 3d20 626f 756e 6469 6e67 5f62 6f78  x = bounding_box
+0000b3b0: 2870 6f69 6e74 7329 0d0a 2020 2020 2020  (points)..      
+0000b3c0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000b3d0: 2020 2020 2020 2020 2320 2020 2020 6d61          #     ma
+0000b3e0: 736b 203d 2028 7878 203e 3d20 786d 696e  sk = (xx >= xmin
+0000b3f0: 2920 2620 2878 7820 3c3d 2078 6d61 7829  ) & (xx <= xmax)
+0000b400: 2026 2028 7979 203e 3d20 796d 696e 2920   & (yy >= ymin) 
+0000b410: 2620 2879 7920 3c3d 2079 6d61 7829 0d0a  & (yy <= ymax)..
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000b440: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0000b450: 6765 2878 782e 7368 6170 655b 305d 293a  ge(xx.shape[0]):
+0000b460: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000b470: 2020 2020 2020 2020 666f 7220 6a20 696e          for j in
+0000b480: 2072 616e 6765 2878 782e 7368 6170 655b   range(xx.shape[
+0000b490: 315d 293a 0d0a 2020 2020 2020 2020 2020  1]):..          
+0000b4a0: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0000b4b0: 6966 206e 6f74 206d 6173 6b5b 692c 206a  if not mask[i, j
+0000b4c0: 5d3a 0d0a 2020 2020 2020 2020 2020 2020  ]:..            
+0000b4d0: 2320 2020 2020 2020 2020 2020 2020 2020  #               
+0000b4e0: 2020 6669 7474 6564 5f70 6c61 6e65 5b69    fitted_plane[i
+0000b4f0: 2c20 6a5d 203d 206e 702e 6e61 6e20 2023  , j] = np.nan  #
+0000b500: 2053 6574 206f 7574 2d6f 662d 626f 756e   Set out-of-boun
+0000b510: 6473 2076 616c 7565 7320 746f 204e 614e  ds values to NaN
+0000b520: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000b530: 2020 2020 2020 2020 706c 616e 6573 2e61          planes.a
+0000b540: 7070 656e 6428 6669 7474 6564 5f70 6c61  ppend(fitted_pla
+0000b550: 6e65 290d 0a20 2020 2020 2020 2020 2020  ne)..           
+0000b560: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
+0000b570: 706c 616e 655f 636f 6c6f 7220 3d20 7261  plane_color = ra
+0000b580: 6e64 6f6d 5f63 6f6c 6f72 2829 0d0a 2020  ndom_color()..  
+0000b590: 2020 2020 2020 2020 2020 706c 616e 655f            plane_
+0000b5a0: 636f 6c6f 723d 636f 6c6f 725f 6672 6f6d  color=color_from
+0000b5b0: 5f64 6970 5f61 6e64 5f64 6972 6563 7469  _dip_and_directi
+0000b5c0: 6f6e 2864 6970 5f61 6e67 6c65 2c20 6469  on(dip_angle, di
+0000b5d0: 705f 6469 7265 6374 696f 6e29 0d0a 2020  p_direction)..  
+0000b5e0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+0000b5f0: 2770 6c61 6e65 2063 6f6c 6f72 3a20 272c  'plane color: ',
+0000b600: 2070 6c61 6e65 5f63 6f6c 6f72 290d 0a20   plane_color).. 
+0000b610: 2020 2020 2020 2020 2020 2070 6c61 6e65             plane
+0000b620: 5f63 6f6c 6f72 732e 6170 7065 6e64 2870  _colors.append(p
+0000b630: 6c61 6e65 5f63 6f6c 6f72 290d 0a0d 0a20  lane_color).... 
+0000b640: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+0000b650: 6f69 6e74 2020 696e 2070 6f69 6e74 733a  oint  in points:
+0000b660: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000b670: 2020 6178 5f32 642e 706c 6f74 2870 6f69    ax_2d.plot(poi
+0000b680: 6e74 5b30 5d2c 2070 6f69 6e74 5b31 5d2c  nt[0], point[1],
+0000b690: 2027 6f27 2c20 636f 6c6f 723d 706c 616e   'o', color=plan
+0000b6a0: 655f 636f 6c6f 7220 2c20 616c 7068 613d  e_color , alpha=
+0000b6b0: 302e 3729 0d0a 2020 2020 2020 2020 2020  0.7)..          
+0000b6c0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000b6d0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000b6e0: 2020 2020 2020 6361 6e76 6173 5f32 642e        canvas_2d.
+0000b6f0: 6472 6177 2829 0d0a 2020 2020 2020 2020  draw()..        
+0000b700: 2020 2020 6672 6f6d 206d 6174 706c 6f74      from matplot
+0000b710: 6c69 622e 636f 6c6f 7273 2069 6d70 6f72  lib.colors impor
+0000b720: 7420 4c69 6768 7453 6f75 7263 650d 0a20  t LightSource.. 
+0000b730: 2020 2020 2020 2020 2020 206c 7320 3d20             ls = 
+0000b740: 4c69 6768 7453 6f75 7263 6528 3237 302c  LightSource(270,
+0000b750: 2034 3529 0d0a 2020 2020 2020 2020 2020   45)..          
+0000b760: 2020 2320 546f 2075 7365 2061 2063 7573    # To use a cus
+0000b770: 746f 6d20 6869 6c6c 7368 6164 696e 6720  tom hillshading 
+0000b780: 6d6f 6465 2c20 6f76 6572 7269 6465 2074  mode, override t
+0000b790: 6865 2062 7569 6c74 2d69 6e20 7368 6164  he built-in shad
+0000b7a0: 696e 6720 616e 6420 7061 7373 0d0a 2020  ing and pass..  
+0000b7b0: 2020 2020 2020 2020 2020 2320 696e 2074            # in t
+0000b7c0: 6865 2072 6762 2063 6f6c 6f72 7320 6f66  he rgb colors of
+0000b7d0: 2074 6865 2073 6861 6465 6420 7375 7266   the shaded surf
+0000b7e0: 6163 6520 6361 6c63 756c 6174 6564 2066  ace calculated f
+0000b7f0: 726f 6d20 2273 6861 6465 222e 0d0a 2020  rom "shade"...  
+0000b800: 2020 2020 2020 2020 2020 7267 6220 3d20            rgb = 
+0000b810: 6c73 2e73 6861 6465 2864 6174 612c 2063  ls.shade(data, c
+0000b820: 6d61 703d 706c 742e 636d 2e67 7261 792c  map=plt.cm.gray,
+0000b830: 2076 6572 745f 6578 6167 3d31 2c20 626c   vert_exag=1, bl
+0000b840: 656e 645f 6d6f 6465 3d27 6f76 6572 6c61  end_mode='overla
+0000b850: 7927 290d 0a0d 0a20 2020 2020 2020 2020  y')....         
+0000b860: 2020 2023 6178 5f33 642e 636c 6561 7228     #ax_3d.clear(
+0000b870: 290d 0a20 2020 2020 2020 2020 2020 2061  )..            a
+0000b880: 785f 3364 2e73 6574 5f74 6974 6c65 2827  x_3d.set_title('
+0000b890: 3344 2044 454d 2077 6974 6820 4669 7474  3D DEM with Fitt
+0000b8a0: 6564 2050 6c61 6e65 7327 290d 0a20 2020  ed Planes')..   
+0000b8b0: 2020 2020 2020 2020 2061 785f 3364 2e70           ax_3d.p
+0000b8c0: 6c6f 745f 7375 7266 6163 6528 7878 2c20  lot_surface(xx, 
+0000b8d0: 7979 2c20 6461 7461 2c63 6d61 703d 2767  yy, data,cmap='g
+0000b8e0: 7261 7927 2c0d 0a20 2020 2020 2020 2020  ray',..         
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+0000b900: 6e65 7769 6474 683d 302c 2061 6e74 6961  newidth=0, antia
+0000b910: 6c69 6173 6564 3d54 7275 652c 2073 6861  liased=True, sha
+0000b920: 6465 3d46 616c 7365 2c20 616c 7068 613d  de=False, alpha=
+0000b930: 302e 342c 2066 6163 6563 6f6c 6f72 733d  0.4, facecolors=
+0000b940: 7267 6229 0d0a 2020 2020 2020 2020 2020  rgb)..          
+0000b950: 2020 2366 6f72 2070 6c61 6e65 2069 6e20    #for plane in 
+0000b960: 706c 616e 6573 3a0d 0a20 2020 2020 2020  planes:..       
+0000b970: 2020 2020 2073 7572 663d 6178 5f33 642e       surf=ax_3d.
+0000b980: 706c 6f74 5f73 7572 6661 6365 2878 782c  plot_surface(xx,
+0000b990: 2079 792c 2066 6974 7465 645f 706c 616e   yy, fitted_plan
+0000b9a0: 652c 2061 6c70 6861 3d30 2e36 2c20 6c69  e, alpha=0.6, li
+0000b9b0: 6e65 7769 6474 683d 302c 2061 6e74 6961  newidth=0, antia
+0000b9c0: 6c69 6173 6564 3d54 7275 652c 2063 6f6c  liased=True, col
+0000b9d0: 6f72 3d70 6c61 6e65 5f63 6f6c 6f72 290d  or=plane_color).
+0000b9e0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000ba00: 706c 6f74 2070 6f69 6e74 7320 696e 2033  plot points in 3
+0000ba10: 440d 0a20 2020 2020 2020 2020 2020 2066  D..            f
+0000ba20: 6f72 2070 6f69 6e74 2069 6e20 706f 696e  or point in poin
+0000ba30: 7473 3a0d 0a20 2020 2020 2020 2020 2020  ts:..           
+0000ba40: 2020 2020 2061 785f 3364 2e70 6c6f 7428       ax_3d.plot(
+0000ba50: 706f 696e 745b 305d 2c20 706f 696e 745b  point[0], point[
+0000ba60: 315d 2c20 276f 272c 2063 6f6c 6f72 3d70  1], 'o', color=p
+0000ba70: 6c61 6e65 5f63 6f6c 6f72 290d 0a20 2020  lane_color)..   
+0000ba80: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000ba90: 2020 2020 2020 2020 2020 2063 616e 7661             canva
+0000baa0: 735f 3364 2e64 7261 7728 290d 0a20 2020  s_3d.draw()..   
+0000bab0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000bac0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000bad0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
+0000bae0: 2020 2020 2070 6f69 6e74 735f 6c69 7374       points_list
+0000baf0: 626f 782e 6465 6c65 7465 2830 2c20 746b  box.delete(0, tk
+0000bb00: 2e45 4e44 290d 0a20 2020 2020 2020 2020  .END)..         
+0000bb10: 2020 2070 6f69 6e74 732e 636c 6561 7228     points.clear(
+0000bb20: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+0000bb30: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
+0000bb40: 745f 706c 616e 6573 2864 6970 5f61 6e67  t_planes(dip_ang
+0000bb50: 6c65 5f6c 6973 742c 2064 6970 5f64 6972  le_list, dip_dir
+0000bb60: 6563 7469 6f6e 5f6c 6973 742c 2070 6c61  ection_list, pla
+0000bb70: 6e65 5f63 6f6c 6f72 7329 0d0a 2020 2020  ne_colors)..    
+0000bb80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000bb90: 2020 2020 2020 2320 4173 7375 6d69 6e67        # Assuming
+0000bba0: 2079 6f75 2068 6176 6520 6120 2770 6c61   you have a 'pla
+0000bbb0: 6e65 7327 206c 6973 742c 2079 6f75 2063  nes' list, you c
+0000bbc0: 616e 2063 6865 636b 2069 7473 2066 6f72  an check its for
+0000bbd0: 6d61 740d 0a20 2020 2020 2020 2020 2020  mat..           
+0000bbe0: 2023 2066 6f72 2070 6c61 6e65 2069 6e20   # for plane in 
+0000bbf0: 706c 616e 6573 3a0d 0a20 2020 2020 2020  planes:..       
+0000bc00: 2020 2020 2023 2020 2020 2070 7269 6e74       #     print
+0000bc10: 2874 7970 6528 706c 616e 6529 290d 0a20  (type(plane)).. 
+0000bc20: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+0000bc30: 2070 7269 6e74 286c 656e 2870 6c61 6e65   print(len(plane
+0000bc40: 2929 2020 2320 5468 6973 2077 696c 6c20  ))  # This will 
+0000bc50: 6769 7665 2079 6f75 2074 6865 206c 656e  give you the len
+0000bc60: 6774 6820 6f72 206e 756d 6265 7220 6f66  gth or number of
+0000bc70: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
+0000bc80: 2070 6c61 6e65 0d0a 0d0a 2020 2020 2020   plane....      
+0000bc90: 2020 2020 2020 2320 2020 2020 2320 4966        #     # If
+0000bca0: 2069 7427 7320 6120 4e75 6d50 7920 6172   it's a NumPy ar
+0000bcb0: 7261 792c 2079 6f75 2063 616e 2070 7269  ray, you can pri
+0000bcc0: 6e74 2069 7473 2073 6861 7065 2074 6f20  nt its shape to 
+0000bcd0: 7365 6520 7468 6520 6469 6d65 6e73 696f  see the dimensio
+0000bce0: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
+0000bcf0: 2320 2020 2020 6966 2069 7369 6e73 7461  #     if isinsta
+0000bd00: 6e63 6528 706c 616e 652c 206e 702e 6e64  nce(plane, np.nd
+0000bd10: 6172 7261 7929 3a0d 0a20 2020 2020 2020  array):..       
+0000bd20: 2020 2020 2023 2020 2020 2020 2020 2070       #         p
+0000bd30: 7269 6e74 2870 6c61 6e65 2e73 6861 7065  rint(plane.shape
+0000bd40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000bd50: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000bd60: 2023 2020 2020 2023 2050 7269 6e74 2074   #     # Print t
+0000bd70: 6865 2066 6972 7374 2065 6c65 6d65 6e74  he first element
+0000bd80: 2028 6173 7375 6d69 6e67 2069 7427 7320   (assuming it's 
+0000bd90: 6120 6c69 7374 206f 7220 4e75 6d50 7920  a list or NumPy 
+0000bda0: 6172 7261 7929 0d0a 2020 2020 2020 2020  array)..        
+0000bdb0: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
+0000bdc0: 706c 616e 655b 305d 290d 0a0d 0a20 2020  plane[0])....   
+0000bdd0: 2020 2020 2020 2020 2023 2023 2050 7269           # # Pri
+0000bde0: 6e74 2074 6865 206c 656e 6774 6820 6f66  nt the length of
+0000bdf0: 2074 6865 2027 706c 616e 6573 2720 6c69   the 'planes' li
+0000be00: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
+0000be10: 2320 7072 696e 7428 6c65 6e28 706c 616e  # print(len(plan
+0000be20: 6573 2929 0d0a 2020 2020 2020 2020 2020  es))..          
+0000be30: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000be40: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000be50: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0000be60: 6465 6620 626f 756e 6469 6e67 5f62 6f78  def bounding_box
+0000be70: 2870 6f69 6e74 7329 3a0d 0a20 2020 2020  (points):..     
+0000be80: 2020 2022 2222 4669 6e64 2074 6865 2062     """Find the b
+0000be90: 6f75 6e64 696e 6720 626f 7820 666f 7220  ounding box for 
+0000bea0: 6120 7365 7420 6f66 2070 6f69 6e74 732e  a set of points.
+0000beb0: 2222 220d 0a20 2020 2020 2020 2078 5f76  """..        x_v
+0000bec0: 616c 732c 2079 5f76 616c 732c 205f 203d  als, y_vals, _ =
+0000bed0: 207a 6970 282a 706f 696e 7473 290d 0a20   zip(*points).. 
+0000bee0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000bef0: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0000bf00: 6e20 6d69 6e28 785f 7661 6c73 2920 2c20  n min(x_vals) , 
+0000bf10: 6d61 7828 785f 7661 6c73 292c 206d 696e  max(x_vals), min
+0000bf20: 2879 5f76 616c 7329 2c20 6d61 7828 795f  (y_vals), max(y_
+0000bf30: 7661 6c73 290d 0a0d 0a20 2020 2023 2323  vals)....    ###
+0000bf40: 2323 2323 230d 0a0d 0a20 2020 0d0a 2020  #####....   ..  
+0000bf50: 2020 0d0a 2020 2020 696d 706f 7274 2065    ..    import e
+0000bf60: 7a64 7866 0d0a 2020 2020 6672 6f6d 2073  zdxf..    from s
+0000bf70: 6369 7079 2e73 7061 7469 616c 2069 6d70  cipy.spatial imp
+0000bf80: 6f72 7420 4465 6c61 756e 6179 0d0a 2020  ort Delaunay..  
+0000bf90: 2020 696d 706f 7274 206e 756d 7079 2061    import numpy a
+0000bfa0: 7320 6e70 0d0a 2020 2020 696d 706f 7274  s np..    import
+0000bfb0: 206f 730d 0a0d 0a20 2020 2064 6566 206c   os....    def l
+0000bfc0: 6973 745f 7879 7a5f 6669 6c65 735f 696e  ist_xyz_files_in
+0000bfd0: 5f66 6f6c 6465 7228 666f 6c64 6572 5f70  _folder(folder_p
+0000bfe0: 6174 6829 3a0d 0a20 2020 2020 2020 2078  ath):..        x
+0000bff0: 797a 5f66 696c 6573 203d 205b 5d0d 0a20  yz_files = [].. 
+0000c000: 2020 2020 2020 2066 6f72 2066 696c 656e         for filen
+0000c010: 616d 6520 696e 206f 732e 6c69 7374 6469  ame in os.listdi
+0000c020: 7228 666f 6c64 6572 5f70 6174 6829 3a0d  r(folder_path):.
+0000c030: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000c040: 6669 6c65 6e61 6d65 2e65 6e64 7377 6974  filename.endswit
+0000c050: 6828 222e 7879 7a22 293a 0d0a 2020 2020  h(".xyz"):..    
+0000c060: 2020 2020 2020 2020 2020 2020 7879 7a5f              xyz_
+0000c070: 6669 6c65 732e 6170 7065 6e64 286f 732e  files.append(os.
+0000c080: 7061 7468 2e6a 6f69 6e28 666f 6c64 6572  path.join(folder
+0000c090: 5f70 6174 682c 2066 696c 656e 616d 6529  _path, filename)
+0000c0a0: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+0000c0b0: 6e20 7879 7a5f 6669 6c65 730d 0a0d 0a20  n xyz_files.... 
+0000c0c0: 2020 2064 6566 2063 7265 6174 655f 6478     def create_dx
+0000c0d0: 665f 6672 6f6d 5f78 797a 5f66 696c 6573  f_from_xyz_files
+0000c0e0: 2878 797a 5f66 696c 6573 2c20 6f75 7470  (xyz_files, outp
+0000c0f0: 7574 5f70 6174 682c 2073 696e 676c 653d  ut_path, single=
+0000c100: 4e6f 6e65 293a 0d0a 2020 2020 2020 2020  None):..        
+0000c110: 2369 6d70 6f72 7420 6f70 656e 3364 2061  #import open3d a
+0000c120: 7320 6f33 640d 0a20 2020 2020 2020 2069  s o3d..        i
+0000c130: 6d70 6f72 7420 7079 6d65 7368 6c61 620d  mport pymeshlab.
+0000c140: 0a0d 0a20 2020 2020 2020 2066 6f72 2078  ...        for x
+0000c150: 797a 5f66 696c 6520 696e 2078 797a 5f66  yz_file in xyz_f
+0000c160: 696c 6573 3a0d 0a20 2020 2020 2020 2020  iles:..         
+0000c170: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000c180: 206d 7320 3d20 7079 6d65 7368 6c61 622e   ms = pymeshlab.
+0000c190: 4d65 7368 5365 7428 290d 0a20 2020 2020  MeshSet()..     
+0000c1a0: 2020 2020 2020 206d 732e 6c6f 6164 5f6e         ms.load_n
+0000c1b0: 6577 5f6d 6573 6828 7879 7a5f 6669 6c65  ew_mesh(xyz_file
+0000c1c0: 290d 0a20 2020 2020 2020 2020 2020 206d  )..            m
+0000c1d0: 732e 636f 6d70 7574 655f 6e6f 726d 616c  s.compute_normal
+0000c1e0: 5f66 6f72 5f70 6f69 6e74 5f63 6c6f 7564  _for_point_cloud
+0000c1f0: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+0000c200: 2023 6d73 2e67 656e 6572 6174 655f 7375   #ms.generate_su
+0000c210: 7266 6163 655f 7265 636f 6e73 7472 7563  rface_reconstruc
+0000c220: 7469 6f6e 5f62 616c 6c5f 7069 766f 7469  tion_ball_pivoti
+0000c230: 6e67 2829 0d0a 2020 2020 2020 2020 2020  ng()..          
+0000c240: 2020 6d73 2e67 656e 6572 6174 655f 7375    ms.generate_su
+0000c250: 7266 6163 655f 7265 636f 6e73 7472 7563  rface_reconstruc
+0000c260: 7469 6f6e 5f73 6372 6565 6e65 645f 706f  tion_screened_po
+0000c270: 6973 736f 6e28 290d 0a20 2020 2020 2020  isson()..       
+0000c280: 2020 2020 206d 732e 6d65 7368 696e 675f       ms.meshing_
+0000c290: 7265 6d6f 7665 5f75 6e72 6566 6572 656e  remove_unreferen
+0000c2a0: 6365 645f 7665 7274 6963 6573 2829 0d0a  ced_vertices()..
+0000c2b0: 2020 2020 2020 2020 2020 2020 6d73 5f31              ms_1
+0000c2c0: 3d6d 730d 0a20 2020 2020 2020 2020 2020  =ms..           
+0000c2d0: 2023 6d73 2e73 6176 655f 6375 7272 656e   #ms.save_curren
+0000c2e0: 745f 6d65 7368 286f 7574 7075 745f 7061  t_mesh(output_pa
+0000c2f0: 7468 5b3a 2d34 5d2b 272e 6f62 6a27 290d  th[:-4]+'.obj').
+0000c300: 0a20 2020 2020 2020 2020 2020 206d 735f  .            ms_
+0000c310: 312e 7361 7665 5f63 7572 7265 6e74 5f6d  1.save_current_m
+0000c320: 6573 6828 6f75 7470 7574 5f70 6174 685b  esh(output_path[
+0000c330: 3a2d 345d 2b27 2e70 6c79 272c 2062 696e  :-4]+'.ply', bin
+0000c340: 6172 793d 5472 7565 290d 0a20 2020 2020  ary=True)..     
+0000c350: 2020 2020 2020 2023 2070 6364 203d 206f         # pcd = o
+0000c360: 3364 2e69 6f2e 7265 6164 5f70 6f69 6e74  3d.io.read_point
+0000c370: 5f63 6c6f 7564 2878 797a 5f66 696c 6529  _cloud(xyz_file)
+0000c380: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000c390: 7063 642e 6573 7469 6d61 7465 5f6e 6f72  pcd.estimate_nor
+0000c3a0: 6d61 6c73 2829 0d0a 0d0a 2020 2020 2020  mals()....      
+0000c3b0: 2020 2020 2020 2320 2320 746f 206f 6274        # # to obt
+0000c3c0: 6169 6e20 6120 636f 6e73 6973 7465 6e74  ain a consistent
+0000c3d0: 206e 6f72 6d61 6c20 6f72 6965 6e74 6174   normal orientat
+0000c3e0: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+0000c3f0: 2023 2070 6364 2e6f 7269 656e 745f 6e6f   # pcd.orient_no
+0000c400: 726d 616c 735f 746f 7761 7264 735f 6361  rmals_towards_ca
+0000c410: 6d65 7261 5f6c 6f63 6174 696f 6e28 7063  mera_location(pc
+0000c420: 642e 6765 745f 6365 6e74 6572 2829 290d  d.get_center()).
+0000c430: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+0000c440: 2023 206f 7220 796f 7520 6d69 6768 7420   # or you might 
+0000c450: 7761 6e74 2074 6f20 666c 6970 2074 6865  want to flip the
+0000c460: 206e 6f72 6d61 6c73 2074 6f20 6d61 6b65   normals to make
+0000c470: 2074 6865 6d20 706f 696e 7420 6f75 7477   them point outw
+0000c480: 6172 642c 206e 6f74 206d 616e 6461 746f  ard, not mandato
+0000c490: 7279 0d0a 2020 2020 2020 2020 2020 2020  ry..            
+0000c4a0: 2320 7063 642e 6e6f 726d 616c 7320 3d20  # pcd.normals = 
+0000c4b0: 6f33 642e 7574 696c 6974 792e 5665 6374  o3d.utility.Vect
+0000c4c0: 6f72 3364 5665 6374 6f72 2820 2d20 6e70  or3dVector( - np
+0000c4d0: 2e61 7361 7272 6179 2870 6364 2e6e 6f72  .asarray(pcd.nor
+0000c4e0: 6d61 6c73 2929 0d0a 0d0a 2020 2020 2020  mals))....      
+0000c4f0: 2020 2020 2020 2320 2320 7375 7266 6163        # # surfac
+0000c500: 6520 7265 636f 6e73 7472 7563 7469 6f6e  e reconstruction
+0000c510: 2075 7369 6e67 2050 6f69 7373 6f6e 2072   using Poisson r
+0000c520: 6563 6f6e 7374 7275 6374 696f 6e0d 0a20  econstruction.. 
+0000c530: 2020 2020 2020 2020 2020 2023 206d 6573             # mes
+0000c540: 682c 205f 203d 206f 3364 2e67 656f 6d65  h, _ = o3d.geome
+0000c550: 7472 792e 5472 6961 6e67 6c65 4d65 7368  try.TriangleMesh
+0000c560: 2e63 7265 6174 655f 6672 6f6d 5f70 6f69  .create_from_poi
+0000c570: 6e74 5f63 6c6f 7564 5f70 6f69 7373 6f6e  nt_cloud_poisson
+0000c580: 2870 6364 2c20 6465 7074 683d 3929 0d0a  (pcd, depth=9)..
+0000c590: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0000c5a0: 2320 7061 696e 7420 756e 6966 6f72 6d20  # paint uniform 
+0000c5b0: 636f 6c6f 7220 746f 2062 6574 7465 7220  color to better 
+0000c5c0: 7669 7375 616c 697a 652c 206e 6f74 206d  visualize, not m
+0000c5d0: 616e 6461 746f 7279 0d0a 2020 2020 2020  andatory..      
+0000c5e0: 2020 2020 2020 2320 6d65 7368 2e70 6169        # mesh.pai
+0000c5f0: 6e74 5f75 6e69 666f 726d 5f63 6f6c 6f72  nt_uniform_color
+0000c600: 286e 702e 6172 7261 7928 5b30 2e37 2c20  (np.array([0.7, 
+0000c610: 302e 372c 2030 2e37 5d29 290d 0a0d 0a20  0.7, 0.7])).... 
+0000c620: 2020 2020 2020 2020 2020 2023 206f 3364             # o3d
+0000c630: 2e69 6f2e 7772 6974 655f 7472 6961 6e67  .io.write_triang
+0000c640: 6c65 5f6d 6573 6828 6f75 7470 7574 5f70  le_mesh(output_p
+0000c650: 6174 685b 3a2d 345d 2b27 2e70 6c79 272c  ath[:-4]+'.ply',
+0000c660: 206d 6573 6829 0d0a 2020 2020 2020 2020   mesh)..        
+0000c670: 2320 646f 6320 3d20 4e6f 6e65 0d0a 2020  # doc = None..  
+0000c680: 2020 2020 2020 2320 6d73 7020 3d20 4e6f        # msp = No
+0000c690: 6e65 0d0a 0d0a 2020 2020 2020 2020 2320  ne....        # 
+0000c6a0: 2320 4675 6e63 7469 6f6e 2074 6f20 696e  # Function to in
+0000c6b0: 6974 6961 6c69 7a65 2044 5846 2064 6f63  itialize DXF doc
+0000c6c0: 756d 656e 740d 0a20 2020 2020 2020 2023  ument..        #
+0000c6d0: 2064 6566 2069 6e69 7469 616c 697a 655f   def initialize_
+0000c6e0: 6478 6628 293a 0d0a 2020 2020 2020 2020  dxf():..        
+0000c6f0: 2320 2020 2020 6e6f 6e6c 6f63 616c 2064  #     nonlocal d
+0000c700: 6f63 2c20 6d73 700d 0a20 2020 2020 2020  oc, msp..       
+0000c710: 2023 2020 2020 2064 6f63 203d 2065 7a64   #     doc = ezd
+0000c720: 7866 2e6e 6577 2827 5232 3031 3027 2920  xf.new('R2010') 
+0000c730: 2023 2053 7065 6369 6679 2074 6865 2044   # Specify the D
+0000c740: 5846 2066 6f72 6d61 742c 2065 2e67 2e2c  XF format, e.g.,
+0000c750: 2027 5232 3031 3027 2066 6f72 2063 6f6d   'R2010' for com
+0000c760: 7061 7469 6269 6c69 7479 0d0a 2020 2020  patibility..    
+0000c770: 2020 2020 2320 2020 2020 6d73 7020 3d20      #     msp = 
+0000c780: 646f 632e 6d6f 6465 6c73 7061 6365 2829  doc.modelspace()
+0000c790: 0d0a 0d0a 2020 2020 2020 2020 2320 6966  ....        # if
+0000c7a0: 2073 696e 676c 6520 6973 204e 6f6e 653a   single is None:
+0000c7b0: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0000c7c0: 696e 6974 6961 6c69 7a65 5f64 7866 2829  initialize_dxf()
+0000c7d0: 0d0a 0d0a 2020 2020 2020 2020 2320 666f  ....        # fo
+0000c7e0: 7220 7879 7a5f 6669 6c65 2069 6e20 7879  r xyz_file in xy
+0000c7f0: 7a5f 6669 6c65 733a 0d0a 2020 2020 2020  z_files:..      
+0000c800: 2020 2320 2020 2020 6966 2073 696e 676c    #     if singl
+0000c810: 6520 6973 206e 6f74 204e 6f6e 653a 0d0a  e is not None:..
+0000c820: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0000c830: 2020 696e 6974 6961 6c69 7a65 5f64 7866    initialize_dxf
+0000c840: 2829 0d0a 0d0a 2020 2020 2020 2020 2320  ()....        # 
+0000c850: 2020 2020 6461 7461 203d 206e 702e 6c6f      data = np.lo
+0000c860: 6164 7478 7428 7879 7a5f 6669 6c65 290d  adtxt(xyz_file).
+0000c870: 0a20 2020 2020 2020 2023 2020 2020 2069  .        #     i
+0000c880: 6620 6461 7461 2e73 697a 6520 3d3d 2030  f data.size == 0
+0000c890: 206f 7220 6461 7461 2e73 6861 7065 5b31   or data.shape[1
+0000c8a0: 5d20 3c20 333a 0d0a 2020 2020 2020 2020  ] < 3:..        
+0000c8b0: 2320 2020 2020 2020 2020 7072 696e 7428  #         print(
+0000c8c0: 6622 536b 6970 7069 6e67 207b 7879 7a5f  f"Skipping {xyz_
+0000c8d0: 6669 6c65 7d20 6475 6520 746f 2069 6e73  file} due to ins
+0000c8e0: 7566 6669 6369 656e 7420 6461 7461 2229  ufficient data")
+0000c8f0: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0000c900: 2020 2020 636f 6e74 696e 7565 0d0a 2020      continue..  
+0000c910: 2020 2020 2020 2320 2020 2020 6966 2064        #     if d
+0000c920: 6174 612e 6e64 696d 203d 3d20 313a 0d0a  ata.ndim == 1:..
+0000c930: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0000c940: 2020 6461 7461 203d 2064 6174 615b 6e70    data = data[np
+0000c950: 2e6e 6577 6178 6973 2c20 3a5d 0d0a 0d0a  .newaxis, :]....
+0000c960: 2020 2020 2020 2020 2320 2020 2020 782c          #     x,
+0000c970: 2079 2c20 7a20 3d20 6461 7461 5b3a 2c20   y, z = data[:, 
+0000c980: 305d 2c20 6461 7461 5b3a 2c20 315d 2c20  0], data[:, 1], 
+0000c990: 6461 7461 5b3a 2c20 325d 0d0a 2020 2020  data[:, 2]..    
+0000c9a0: 2020 2020 2320 2020 2020 706f 696e 7473      #     points
+0000c9b0: 203d 206e 702e 636f 6c75 6d6e 5f73 7461   = np.column_sta
+0000c9c0: 636b 2828 782c 2079 2c20 7a29 290d 0a0d  ck((x, y, z))...
+0000c9d0: 0a20 2020 2020 2020 2023 2020 2020 2074  .        #     t
+0000c9e0: 7279 3a0d 0a20 2020 2020 2020 2023 2020  ry:..        #  
+0000c9f0: 2020 2020 2020 2074 7269 203d 2044 656c         tri = Del
+0000ca00: 6175 6e61 7928 706f 696e 7473 2c20 6675  aunay(points, fu
+0000ca10: 7274 6865 7374 5f73 6974 653d 4661 6c73  rthest_site=Fals
+0000ca20: 652c 2069 6e63 7265 6d65 6e74 616c 3d54  e, incremental=T
+0000ca30: 7275 652c 2071 6875 6c6c 5f6f 7074 696f  rue, qhull_optio
+0000ca40: 6e73 3d27 5163 2729 0d0a 2020 2020 2020  ns='Qc')..      
+0000ca50: 2020 2320 2020 2020 2020 2020 666f 7220    #         for 
+0000ca60: 7369 6d70 6c65 7820 696e 2074 7269 2e73  simplex in tri.s
+0000ca70: 696d 706c 6963 6573 3a0d 0a20 2020 2020  implices:..     
+0000ca80: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000ca90: 2076 6572 7469 6365 7320 3d20 5b74 7570   vertices = [tup
+0000caa0: 6c65 2870 6f69 6e74 735b 695d 2920 666f  le(points[i]) fo
+0000cab0: 7220 6920 696e 2073 696d 706c 6578 5d20  r i in simplex] 
+0000cac0: 2023 2045 6e73 7572 6520 7665 7274 6963   # Ensure vertic
+0000cad0: 6573 2061 7265 2074 7570 6c65 730d 0a20  es are tuples.. 
+0000cae0: 2020 2020 2020 2023 2020 2020 2020 2020         #        
+0000caf0: 2020 2020 206d 7370 2e61 6464 5f33 6466       msp.add_3df
+0000cb00: 6163 6528 7665 7274 6963 6573 290d 0a20  ace(vertices).. 
+0000cb10: 2020 2020 2020 2023 2020 2020 2065 7863         #     exc
+0000cb20: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
+0000cb30: 2065 3a0d 0a20 2020 2020 2020 2023 2020   e:..        #  
+0000cb40: 2020 2020 2020 2070 7269 6e74 2866 2246         print(f"F
+0000cb50: 6169 6c65 6420 746f 2070 726f 6365 7373  ailed to process
+0000cb60: 207b 7879 7a5f 6669 6c65 7d3a 207b 657d   {xyz_file}: {e}
+0000cb70: 2229 0d0a 2020 2020 2020 2020 2320 2020  ")..        #   
+0000cb80: 2020 2020 2020 636f 6e74 696e 7565 0d0a        continue..
+0000cb90: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0000cba0: 6966 2073 696e 676c 6520 6973 206e 6f74  if single is not
+0000cbb0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+0000cbc0: 2320 2020 2020 2020 2020 6669 6c65 6e61  #         filena
+0000cbd0: 6d65 203d 206f 732e 7061 7468 2e6a 6f69  me = os.path.joi
+0000cbe0: 6e28 6f75 7470 7574 5f70 6174 682c 2066  n(output_path, f
+0000cbf0: 227b 6f73 2e70 6174 682e 7370 6c69 7465  "{os.path.splite
+0000cc00: 7874 286f 732e 7061 7468 2e62 6173 656e  xt(os.path.basen
+0000cc10: 616d 6528 7879 7a5f 6669 6c65 2929 5b30  ame(xyz_file))[0
+0000cc20: 5d7d 2e64 7866 2229 0d0a 2020 2020 2020  ]}.dxf")..      
+0000cc30: 2020 2320 2020 2020 2020 2020 7472 793a    #         try:
+0000cc40: 0d0a 2020 2020 2020 2020 2320 2020 2020  ..        #     
+0000cc50: 2020 2020 2020 2020 646f 632e 7361 7665          doc.save
+0000cc60: 6173 2866 696c 656e 616d 6529 0d0a 2020  as(filename)..  
+0000cc70: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+0000cc80: 2020 2020 7072 696e 7428 6622 5361 7665      print(f"Save
+0000cc90: 643a 207b 6669 6c65 6e61 6d65 7d22 290d  d: {filename}").
+0000cca0: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0000ccb0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+0000ccc0: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+0000ccd0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000cce0: 2070 7269 6e74 2866 2245 7272 6f72 2073   print(f"Error s
+0000ccf0: 6176 696e 6720 7b66 696c 656e 616d 657d  aving {filename}
+0000cd00: 3a20 7b65 7d22 290d 0a0d 0a20 2020 2020  : {e}")....     
+0000cd10: 2020 2023 2069 6620 7369 6e67 6c65 2069     # if single i
+0000cd20: 7320 4e6f 6e65 2061 6e64 2064 6f63 2069  s None and doc i
+0000cd30: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
+0000cd40: 2020 2020 2023 2020 2020 2074 7279 3a0d       #     try:.
+0000cd50: 0a20 2020 2020 2020 2023 2020 2020 2020  .        #      
+0000cd60: 2020 2064 6f63 2e73 6176 6561 7328 6f75     doc.saveas(ou
+0000cd70: 7470 7574 5f70 6174 6829 0d0a 2020 2020  tput_path)..    
+0000cd80: 2020 2020 2320 2020 2020 2020 2020 7072      #         pr
+0000cd90: 696e 7428 6622 5361 7665 6420 636f 6d62  int(f"Saved comb
+0000cda0: 696e 6564 2044 5846 2066 696c 653a 207b  ined DXF file: {
+0000cdb0: 6f75 7470 7574 5f70 6174 687d 2229 0d0a  output_path}")..
+0000cdc0: 2020 2020 2020 2020 2320 2020 2020 6578          #     ex
+0000cdd0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+0000cde0: 7320 653a 0d0a 2020 2020 2020 2020 2320  s e:..        # 
+0000cdf0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+0000ce00: 4572 726f 7220 7361 7669 6e67 2063 6f6d  Error saving com
+0000ce10: 6269 6e65 6420 4458 4620 6669 6c65 3a20  bined DXF file: 
+0000ce20: 7b65 7d22 290d 0a20 2020 2020 2020 200d  {e}")..        .
+0000ce30: 0a20 2020 200d 0a20 2020 2064 6566 2073  .    ..    def s
+0000ce40: 6176 655f 706c 616e 6573 5f74 6f5f 6f62  ave_planes_to_ob
+0000ce50: 6a28 293a 0d0a 2020 2020 2020 2020 785f  j():..        x_
+0000ce60: 636f 6f72 6473 203d 206e 702e 6c69 6e73  coords = np.lins
+0000ce70: 7061 6365 286c 6566 742c 2072 6967 6874  pace(left, right
+0000ce80: 2c20 6461 7461 2e73 6861 7065 5b31 5d29  , data.shape[1])
+0000ce90: 0d0a 2020 2020 2020 2020 795f 636f 6f72  ..        y_coor
+0000cea0: 6473 203d 206e 702e 6c69 6e73 7061 6365  ds = np.linspace
+0000ceb0: 2874 6f70 2c20 626f 7474 6f6d 2c20 6461  (top, bottom, da
+0000cec0: 7461 2e73 6861 7065 5b30 5d29 0d0a 2020  ta.shape[0])..  
+0000ced0: 2020 2020 2020 7878 2c20 7979 203d 206e        xx, yy = n
+0000cee0: 702e 6d65 7368 6772 6964 2878 5f63 6f6f  p.meshgrid(x_coo
+0000cef0: 7264 732c 2079 5f63 6f6f 7264 7329 0d0a  rds, y_coords)..
+0000cf00: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000cf10: 2069 6620 6e6f 7420 706c 616e 6573 3a0d   if not planes:.
+0000cf20: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+0000cf30: 6e74 2822 4e6f 2070 6c61 6e65 7320 746f  nt("No planes to
+0000cf40: 2073 6176 652e 2229 0d0a 2020 2020 2020   save.")..      
+0000cf50: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+0000cf60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000cf70: 0d0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
+0000cf80: 5f66 696c 656e 616d 655f 6478 6620 3d20  _filename_dxf = 
+0000cf90: 6622 7b6f 7574 5f70 6c61 6e65 466f 6c64  f"{out_planeFold
+0000cfa0: 6572 7d2f 706c 616e 6573 2e64 7866 220d  er}/planes.dxf".
+0000cfb0: 0a20 2020 2020 2020 2066 6f72 2069 6478  .        for idx
+0000cfc0: 2c20 706c 616e 6520 696e 2065 6e75 6d65  , plane in enume
+0000cfd0: 7261 7465 2870 6c61 6e65 7329 3a0d 0a20  rate(planes):.. 
+0000cfe0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000cff0: 745f 6669 6c65 6e61 6d65 203d 2066 227b  t_filename = f"{
+0000d000: 6f75 745f 706c 616e 6546 6f6c 6465 727d  out_planeFolder}
+0000d010: 2f70 6c61 6e65 735f 7b69 6478 7d2e 7879  /planes_{idx}.xy
+0000d020: 7a22 0d0a 2020 2020 2020 2020 2020 2020  z"..            
+0000d030: 6f75 7470 7574 5f66 696c 656e 616d 655f  output_filename_
+0000d040: 6964 7820 3d20 6622 7b6f 7574 5f70 6c61  idx = f"{out_pla
+0000d050: 6e65 466f 6c64 6572 7d2f 706c 616e 6573  neFolder}/planes
+0000d060: 5f7b 6964 787d 2e64 7866 220d 0a20 2020  _{idx}.dxf"..   
+0000d070: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0000d080: 2020 2020 2020 2023 2049 6e69 7469 616c         # Initial
+0000d090: 697a 6520 6c69 7374 7320 746f 2073 746f  ize lists to sto
+0000d0a0: 7265 2076 6572 7469 6365 7320 616e 6420  re vertices and 
+0000d0b0: 6661 6365 730d 0a20 2020 2020 2020 2020  faces..         
+0000d0c0: 2020 2076 6572 7469 6365 7320 3d20 5b5d     vertices = []
+0000d0d0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000d0e0: 2020 2020 2020 2020 2020 2020 2320 5361              # Sa
+0000d0f0: 6d70 6c65 6420 706f 696e 7420 696e 7465  mpled point inte
+0000d100: 7276 616c 0d0a 2020 2020 2020 2020 2020  rval..          
+0000d110: 2020 7361 6d70 6c65 5f69 6e74 6572 7661    sample_interva
+0000d120: 6c20 3d20 3230 300d 0a20 2020 2020 2020  l = 200..       
+0000d130: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000d140: 2020 2023 204f 7065 6e20 7468 6520 5859     # Open the XY
+0000d150: 5a20 6669 6c65 2066 6f72 2077 7269 7469  Z file for writi
+0000d160: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
+0000d170: 7769 7468 206f 7065 6e28 6f75 7470 7574  with open(output
+0000d180: 5f66 696c 656e 616d 652c 2027 7727 2920  _filename, 'w') 
+0000d190: 6173 2078 797a 5f66 696c 653a 0d0a 2020  as xyz_file:..  
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000d1b0: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+0000d1c0: 706c 616e 652e 7368 6170 655b 305d 2c20  plane.shape[0], 
+0000d1d0: 7361 6d70 6c65 5f69 6e74 6572 7661 6c29  sample_interval)
+0000d1e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000d1f0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0000d200: 7261 6e67 6528 302c 2070 6c61 6e65 2e73  range(0, plane.s
+0000d210: 6861 7065 5b31 5d2c 2073 616d 706c 655f  hape[1], sample_
+0000d220: 696e 7465 7276 616c 293a 0d0a 2020 2020  interval):..    
+0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d240: 2020 2020 6966 2069 203c 2078 782e 7368      if i < xx.sh
+0000d250: 6170 655b 305d 2061 6e64 206a 203c 2078  ape[0] and j < x
+0000d260: 782e 7368 6170 655b 315d 3a0d 0a20 2020  x.shape[1]:..   
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2078 203d 2078 785b           x = xx[
+0000d290: 692c 206a 5d0d 0a20 2020 2020 2020 2020  i, j]..         
+0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2b0: 2020 2079 203d 2079 795b 692c 206a 5d0d     y = yy[i, j].
+0000d2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d2d0: 2020 2020 2020 2020 2020 2020 207a 203d               z =
+0000d2e0: 2070 6c61 6e65 5b69 2c20 6a5d 0d0a 0d0a   plane[i, j]....
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2020 2020 2020 2020 2320 4368              # Ch
+0000d310: 6563 6b20 666f 7220 4e61 4e20 7661 6c75  eck for NaN valu
+0000d320: 6573 0d0a 2020 2020 2020 2020 2020 2020  es..            
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 6966 206e 6f74 206e 702e 6973 6e61 6e28  if not np.isnan(
+0000d350: 7829 2061 6e64 206e 6f74 206e 702e 6973  x) and not np.is
+0000d360: 6e61 6e28 7929 2061 6e64 206e 6f74 206e  nan(y) and not n
+0000d370: 702e 6973 6e61 6e28 7a29 3a0d 0a20 2020  p.isnan(z):..   
+0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d390: 2020 2020 2020 2020 2020 2020 2023 2041               # A
+0000d3a0: 6464 2074 6865 2076 6572 7465 7820 746f  dd the vertex to
+0000d3b0: 2074 6865 206c 6973 740d 0a20 2020 2020   the list..     
+0000d3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3d0: 2020 2020 2020 2020 2020 2076 6572 7469             verti
+0000d3e0: 6365 732e 6170 7065 6e64 2828 782c 2079  ces.append((x, y
+0000d3f0: 2c20 7a29 290d 0a20 2020 2020 2020 2020  , z))..         
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d410: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d430: 2020 2020 2020 2020 2320 5772 6974 6520          # Write 
+0000d440: 7665 7274 6578 2064 6174 6120 746f 2074  vertex data to t
+0000d450: 6865 2058 595a 2066 696c 650d 0a20 2020  he XYZ file..   
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d470: 2020 2020 2020 2020 2020 2020 2078 797a               xyz
+0000d480: 5f66 696c 652e 7772 6974 6528 6627 7b78  _file.write(f'{x
+0000d490: 7d20 7b79 7d20 7b7a 7d5c 6e27 290d 0a20  } {y} {z}\n').. 
+0000d4a0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000d4b0: 2020 2020 2020 2020 2063 7265 6174 655f           create_
+0000d4c0: 6478 665f 6672 6f6d 5f78 797a 5f66 696c  dxf_from_xyz_fil
+0000d4d0: 6573 286c 6973 745f 7879 7a5f 6669 6c65  es(list_xyz_file
+0000d4e0: 735f 696e 5f66 6f6c 6465 7228 6f75 745f  s_in_folder(out_
+0000d4f0: 706c 616e 6546 6f6c 6465 7229 2c20 6f75  planeFolder), ou
+0000d500: 7470 7574 5f66 696c 656e 616d 655f 6964  tput_filename_id
+0000d510: 782c 2073 696e 676c 653d 6964 7829 0d0a  x, single=idx)..
+0000d520: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d540: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
+0000d550: 6627 7a7a 2076 616c 7565 7320 7361 7665  f'zz values save
+0000d560: 6420 746f 207b 6f75 7470 7574 5f66 696c  d to {output_fil
+0000d570: 656e 616d 657d 2729 0d0a 2020 2020 2020  ename}')..      
+0000d580: 2020 2020 2020 0d0a 2020 2020 0d0a 2020        ..    ..  
+0000d590: 2020 2320 696d 706f 7274 206f 7065 6e33    # import open3
+0000d5a0: 6420 6173 206f 3364 0d0a 0d0a 2020 2020  d as o3d....    
+0000d5b0: 2320 6465 6620 7361 7665 5f70 6c61 6e65  # def save_plane
+0000d5c0: 735f 746f 5f6f 626a 2829 3a0d 0a20 2020  s_to_obj():..   
+0000d5d0: 2023 2020 2020 2078 5f63 6f6f 7264 7320   #     x_coords 
+0000d5e0: 3d20 6e70 2e6c 696e 7370 6163 6528 6c65  = np.linspace(le
+0000d5f0: 6674 2c20 7269 6768 742c 2064 6174 612e  ft, right, data.
+0000d600: 7368 6170 655b 315d 290d 0a20 2020 2023  shape[1])..    #
+0000d610: 2020 2020 2079 5f63 6f6f 7264 7320 3d20       y_coords = 
+0000d620: 6e70 2e6c 696e 7370 6163 6528 746f 702c  np.linspace(top,
+0000d630: 2062 6f74 746f 6d2c 2064 6174 612e 7368   bottom, data.sh
+0000d640: 6170 655b 305d 290d 0a20 2020 2023 2020  ape[0])..    #  
+0000d650: 2020 2078 782c 2079 7920 3d20 6e70 2e6d     xx, yy = np.m
+0000d660: 6573 6867 7269 6428 785f 636f 6f72 6473  eshgrid(x_coords
+0000d670: 2c20 795f 636f 6f72 6473 290d 0a20 2020  , y_coords)..   
+0000d680: 2020 2020 200d 0a20 2020 2023 2020 2020       ..    #    
+0000d690: 2069 6620 6e6f 7420 706c 616e 6573 3a0d   if not planes:.
+0000d6a0: 0a20 2020 2023 2020 2020 2020 2020 2070  .    #         p
+0000d6b0: 7269 6e74 2822 4e6f 2070 6c61 6e65 7320  rint("No planes 
+0000d6c0: 746f 2073 6176 652e 2229 0d0a 2020 2020  to save.")..    
+0000d6d0: 2320 2020 2020 2020 2020 7265 7475 726e  #         return
+0000d6e0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000d6f0: 2320 2020 2020 6f75 7470 7574 5f66 696c  #     output_fil
+0000d700: 656e 616d 655f 6478 6620 3d20 6622 7b6f  ename_dxf = f"{o
+0000d710: 7574 5f70 6c61 6e65 466f 6c64 6572 7d2f  ut_planeFolder}/
+0000d720: 706c 616e 6573 2e64 7866 220d 0a20 2020  planes.dxf"..   
+0000d730: 2023 2020 2020 2066 6f72 2069 6478 2c20   #     for idx, 
+0000d740: 706c 616e 6520 696e 2065 6e75 6d65 7261  plane in enumera
+0000d750: 7465 2870 6c61 6e65 7329 3a0d 0a20 2020  te(planes):..   
+0000d760: 2023 2020 2020 2020 2020 206f 7574 7075   #         outpu
+0000d770: 745f 6669 6c65 6e61 6d65 5f78 797a 203d  t_filename_xyz =
+0000d780: 2066 227b 6f75 745f 706c 616e 6546 6f6c   f"{out_planeFol
+0000d790: 6465 727d 2f70 6c61 6e65 735f 7b69 6478  der}/planes_{idx
+0000d7a0: 7d2e 7879 7a22 0d0a 2020 2020 2320 2020  }.xyz"..    #   
+0000d7b0: 2020 2020 2020 6f75 7470 7574 5f66 696c        output_fil
+0000d7c0: 656e 616d 655f 6f62 6a20 3d20 6622 7b6f  ename_obj = f"{o
+0000d7d0: 7574 5f70 6c61 6e65 466f 6c64 6572 7d2f  ut_planeFolder}/
+0000d7e0: 706c 616e 6573 5f7b 6964 787d 2e6f 626a  planes_{idx}.obj
+0000d7f0: 220d 0a20 2020 2020 2020 2020 2020 200d  "..            .
+0000d800: 0a20 2020 2023 2020 2020 2020 2020 2023  .    #         #
+0000d810: 2049 6e69 7469 616c 697a 6520 6c69 7374   Initialize list
+0000d820: 7320 746f 2073 746f 7265 2076 6572 7469  s to store verti
+0000d830: 6365 7320 616e 6420 6661 6365 730d 0a20  ces and faces.. 
+0000d840: 2020 2023 2020 2020 2020 2020 2076 6572     #         ver
+0000d850: 7469 6365 7320 3d20 5b5d 0d0a 2020 2020  tices = []..    
+0000d860: 2020 2020 2020 2020 0d0a 2020 2020 2320          ..    # 
+0000d870: 2020 2020 2020 2020 2320 5361 6d70 6c65          # Sample
+0000d880: 6420 706f 696e 7420 696e 7465 7276 616c  d point interval
+0000d890: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
+0000d8a0: 7361 6d70 6c65 5f69 6e74 6572 7661 6c20  sample_interval 
+0000d8b0: 3d20 3230 300d 0a20 2020 2020 2020 2020  = 200..         
+0000d8c0: 2020 200d 0a20 2020 2023 2020 2020 2020     ..    #      
+0000d8d0: 2020 2023 204f 7065 6e20 7468 6520 5859     # Open the XY
+0000d8e0: 5a20 6669 6c65 2066 6f72 2077 7269 7469  Z file for writi
+0000d8f0: 6e67 0d0a 2020 2020 2320 2020 2020 2020  ng..    #       
+0000d900: 2020 7769 7468 206f 7065 6e28 6f75 7470    with open(outp
+0000d910: 7574 5f66 696c 656e 616d 655f 7879 7a2c  ut_filename_xyz,
+0000d920: 2027 7727 2920 6173 2078 797a 5f66 696c   'w') as xyz_fil
+0000d930: 653a 0d0a 2020 2020 2320 2020 2020 2020  e:..    #       
+0000d940: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+0000d950: 616e 6765 2830 2c20 706c 616e 652e 7368  ange(0, plane.sh
+0000d960: 6170 655b 305d 2c20 7361 6d70 6c65 5f69  ape[0], sample_i
+0000d970: 6e74 6572 7661 6c29 3a0d 0a20 2020 2023  nterval):..    #
+0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d990: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
+0000d9a0: 302c 2070 6c61 6e65 2e73 6861 7065 5b31  0, plane.shape[1
+0000d9b0: 5d2c 2073 616d 706c 655f 696e 7465 7276  ], sample_interv
+0000d9c0: 616c 293a 0d0a 2020 2020 2320 2020 2020  al):..    #     
+0000d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9e0: 6966 2069 203c 2078 782e 7368 6170 655b  if i < xx.shape[
+0000d9f0: 305d 2061 6e64 206a 203c 2078 782e 7368  0] and j < xx.sh
+0000da00: 6170 655b 315d 3a0d 0a20 2020 2023 2020  ape[1]:..    #  
+0000da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da20: 2020 2020 2020 2078 203d 2078 785b 692c         x = xx[i,
+0000da30: 206a 5d0d 0a20 2020 2023 2020 2020 2020   j]..    #      
+0000da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da50: 2020 2079 203d 2079 795b 692c 206a 5d0d     y = yy[i, j].
+0000da60: 0a20 2020 2023 2020 2020 2020 2020 2020  .    #          
+0000da70: 2020 2020 2020 2020 2020 2020 2020 207a                 z
+0000da80: 203d 2070 6c61 6e65 5b69 2c20 6a5d 0d0a   = plane[i, j]..
+0000da90: 0d0a 2020 2020 2320 2020 2020 2020 2020  ..    #         
+0000daa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dab0: 2320 4368 6563 6b20 666f 7220 4e61 4e20  # Check for NaN 
+0000dac0: 7661 6c75 6573 0d0a 2020 2020 2320 2020  values..    #   
+0000dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dae0: 2020 2020 2020 6966 206e 6f74 206e 702e        if not np.
+0000daf0: 6973 6e61 6e28 7829 2061 6e64 206e 6f74  isnan(x) and not
+0000db00: 206e 702e 6973 6e61 6e28 7929 2061 6e64   np.isnan(y) and
+0000db10: 206e 6f74 206e 702e 6973 6e61 6e28 7a29   not np.isnan(z)
+0000db20: 3a0d 0a20 2020 2023 2020 2020 2020 2020  :..    #        
+0000db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db40: 2020 2020 2023 2041 6464 2074 6865 2076       # Add the v
+0000db50: 6572 7465 7820 746f 2074 6865 206c 6973  ertex to the lis
+0000db60: 740d 0a20 2020 2023 2020 2020 2020 2020  t..    #        
+0000db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db80: 2020 2020 2076 6572 7469 6365 732e 6170       vertices.ap
+0000db90: 7065 6e64 2828 782c 2079 2c20 7a29 290d  pend((x, y, z)).
+0000dba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dbb0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+0000dbc0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2023 2057 7269 7465 2076 6572 7465 7820   # Write vertex 
+0000dbf0: 6461 7461 2074 6f20 7468 6520 5859 5a20  data to the XYZ 
+0000dc00: 6669 6c65 0d0a 2020 2020 2320 2020 2020  file..    #     
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc20: 2020 2020 2020 2020 7879 7a5f 6669 6c65          xyz_file
+0000dc30: 2e77 7269 7465 2866 277b 787d 207b 797d  .write(f'{x} {y}
+0000dc40: 207b 7a7d 5c6e 2729 0d0a 2020 2020 2020   {z}\n')..      
+0000dc50: 2020 2020 2020 0d0a 2020 2020 2320 2020        ..    #   
+0000dc60: 2020 2020 2020 2320 4c6f 6164 2074 6865        # Load the
+0000dc70: 2058 595a 2066 696c 6520 6173 2061 2070   XYZ file as a p
+0000dc80: 6f69 6e74 2063 6c6f 7564 0d0a 2020 2020  oint cloud..    
+0000dc90: 2320 2020 2020 2020 2020 7063 6420 3d20  #         pcd = 
+0000dca0: 6f33 642e 696f 2e72 6561 645f 706f 696e  o3d.io.read_poin
+0000dcb0: 745f 636c 6f75 6428 6f75 7470 7574 5f66  t_cloud(output_f
+0000dcc0: 696c 656e 616d 655f 7879 7a2c 2066 6f72  ilename_xyz, for
+0000dcd0: 6d61 743d 2778 797a 2729 0d0a 2020 2020  mat='xyz')..    
+0000dce0: 2020 2020 2020 2020 0d0a 2020 2020 2320          ..    # 
+0000dcf0: 2020 2020 2020 2020 2320 4f70 7469 6f6e          # Option
+0000dd00: 616c 6c79 2065 7374 696d 6174 6520 6e6f  ally estimate no
+0000dd10: 726d 616c 730d 0a20 2020 2023 2020 2020  rmals..    #    
+0000dd20: 2020 2020 2070 6364 2e65 7374 696d 6174       pcd.estimat
+0000dd30: 655f 6e6f 726d 616c 7328 290d 0a20 2020  e_normals()..   
+0000dd40: 2020 2020 2020 2020 200d 0a20 2020 2023           ..    #
+0000dd50: 2020 2020 2020 2020 2023 2043 7265 6174           # Creat
+0000dd60: 6520 6120 6d65 7368 2075 7369 6e67 2074  e a mesh using t
+0000dd70: 6865 2070 6f69 6e74 2063 6c6f 7564 2028  he point cloud (
+0000dd80: 7573 696e 6720 506f 6973 736f 6e20 7265  using Poisson re
+0000dd90: 636f 6e73 7472 7563 7469 6f6e 2061 7320  construction as 
+0000dda0: 616e 2065 7861 6d70 6c65 290d 0a20 2020  an example)..   
+0000ddb0: 2023 2020 2020 2020 2020 2072 6164 6975   #         radiu
+0000ddc0: 7320 3d20 3130 2020 2320 796f 7520 6d61  s = 10  # you ma
+0000ddd0: 7920 6e65 6564 2074 6f20 6164 6a75 7374  y need to adjust
+0000dde0: 2074 6869 7320 6261 7365 6420 6f6e 2079   this based on y
+0000ddf0: 6f75 7220 6461 7461 2073 6361 6c65 0d0a  our data scale..
+0000de00: 2020 2020 2320 2020 2020 2020 2020 6d65      #         me
+0000de10: 7368 203d 206f 3364 2e67 656f 6d65 7472  sh = o3d.geometr
+0000de20: 792e 5472 6961 6e67 6c65 4d65 7368 2e63  y.TriangleMesh.c
+0000de30: 7265 6174 655f 6672 6f6d 5f70 6f69 6e74  reate_from_point
+0000de40: 5f63 6c6f 7564 5f62 616c 6c5f 7069 766f  _cloud_ball_pivo
+0000de50: 7469 6e67 280d 0a20 2020 2023 2020 2020  ting(..    #    
+0000de60: 2020 2020 2020 2020 2070 6364 2c20 6f33           pcd, o3
+0000de70: 642e 7574 696c 6974 792e 446f 7562 6c65  d.utility.Double
+0000de80: 5665 6374 6f72 285b 7261 6469 7573 2c20  Vector([radius, 
+0000de90: 7261 6469 7573 202a 2032 5d29 290d 0a20  radius * 2])).. 
+0000dea0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000deb0: 2023 2020 2020 2020 2020 2023 2053 6176   #         # Sav
+0000dec0: 6520 6d65 7368 2061 7320 4f42 4a0d 0a20  e mesh as OBJ.. 
+0000ded0: 2020 2023 2020 2020 206f 3364 2e69 6f2e     #     o3d.io.
+0000dee0: 7772 6974 655f 7472 6961 6e67 6c65 5f6d  write_triangle_m
+0000def0: 6573 6828 6f75 7470 7574 5f66 696c 656e  esh(output_filen
+0000df00: 616d 655f 6f62 6a2c 206d 6573 6829 0d0a  ame_obj, mesh)..
+0000df10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0000df20: 2020 0d0a 2020 2020 6465 6620 636f 6c6c    ..    def coll
+0000df30: 6563 745f 706f 696e 7473 5f66 726f 6d5f  ect_points_from_
+0000df40: 6c69 6e65 2867 6466 293a 0d0a 2020 2020  line(gdf):..    
+0000df50: 2020 2020 2222 2243 6f6c 6c65 6374 2073      """Collect s
+0000df60: 7461 7274 2c20 6d69 6464 6c65 2c20 616e  tart, middle, an
+0000df70: 6420 656e 6420 706f 696e 7473 2066 726f  d end points fro
+0000df80: 6d20 6561 6368 206c 696e 6520 6665 6174  m each line feat
+0000df90: 7572 652e 2222 220d 0a20 2020 2020 2020  ure."""..       
+0000dfa0: 2063 6f6c 6c65 6374 6564 5f70 6f69 6e74   collected_point
+0000dfb0: 7320 3d20 5b5d 0d0a 0d0a 2020 2020 2020  s = []....      
+0000dfc0: 2020 666f 7220 6765 6f6d 6574 7279 2069    for geometry i
+0000dfd0: 6e20 6764 662e 6765 6f6d 6574 7279 3a0d  n gdf.geometry:.
+0000dfe0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000dff0: 6765 6f6d 6574 7279 2e67 656f 6d5f 7479  geometry.geom_ty
+0000e000: 7065 203d 3d20 224c 696e 6553 7472 696e  pe == "LineStrin
+0000e010: 6722 3a0d 0a20 2020 2020 2020 2020 2020  g":..           
+0000e020: 2020 2020 2078 2c20 7920 3d20 6765 6f6d       x, y = geom
+0000e030: 6574 7279 2e78 790d 0a20 2020 2020 2020  etry.xy..       
+0000e040: 2020 2020 2020 2020 2073 7461 7274 203d           start =
+0000e050: 2028 785b 305d 2c20 795b 305d 290d 0a20   (x[0], y[0]).. 
+0000e060: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000e070: 6e64 203d 2028 785b 2d31 5d2c 2079 5b2d  nd = (x[-1], y[-
+0000e080: 315d 290d 0a20 2020 2020 2020 2020 2020  1])..           
+0000e090: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000e0a0: 2020 2020 2020 2023 7072 696e 7428 2773         #print('s
+0000e0b0: 7461 7274 3a20 2720 2c73 7461 7274 290d  tart: ' ,start).
+0000e0c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e0d0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000e0e0: 2020 2023 2023 2043 7265 6174 6520 6120     # # Create a 
+0000e0f0: 4c69 6e65 5374 7269 6e67 2066 726f 6d20  LineString from 
+0000e100: 636f 6f72 6469 6e61 7465 7320 746f 2065  coordinates to e
+0000e110: 6173 696c 7920 6765 7420 6120 706f 696e  asily get a poin
+0000e120: 7420 6174 2035 3025 2064 6973 7461 6e63  t at 50% distanc
+0000e130: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+0000e140: 2020 206c 696e 6520 3d20 4c69 6e65 5374     line = LineSt
+0000e150: 7269 6e67 287a 6970 2878 2c20 7929 290d  ring(zip(x, y)).
+0000e160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e170: 2023 2069 6620 6c65 6e28 6c69 6e65 2e63   # if len(line.c
+0000e180: 6f6f 7264 7329 203e 3d20 333a 0d0a 2020  oords) >= 3:..  
+0000e190: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e1a0: 2020 2020 2320 4966 2074 6865 206c 696e      # If the lin
+0000e1b0: 6520 6861 7320 6d6f 7265 2074 6861 6e20  e has more than 
+0000e1c0: 3220 7665 7274 6963 6573 2c20 636f 6c6c  2 vertices, coll
+0000e1d0: 6563 7420 706f 696e 7473 2061 7420 7665  ect points at ve
+0000e1e0: 7274 6963 6573 0d0a 2020 2020 2020 2020  rtices..        
+0000e1f0: 2020 2020 2020 2020 2320 2020 2020 7665          #     ve
+0000e200: 7274 6963 6573 203d 206c 6973 7428 6c69  rtices = list(li
+0000e210: 6e65 2e63 6f6f 7264 7329 0d0a 2020 2020  ne.coords)..    
+0000e220: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+0000e230: 2020 2370 7269 6e74 2827 7665 7274 6963    #print('vertic
+0000e240: 733a 2027 2c20 7665 7274 6963 6573 290d  s: ', vertices).
+0000e250: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e260: 2023 2020 2020 2076 6572 7465 785f 6c69   #     vertex_li
+0000e270: 7374 3d5b 6920 666f 7220 6920 696e 2076  st=[i for i in v
+0000e280: 6572 7469 6365 735d 0d0a 2020 2020 2020  ertices]..      
+0000e290: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+0000e2a0: 666f 7220 6b6a 2069 6e20 7665 7274 6578  for kj in vertex
+0000e2b0: 5f6c 6973 743a 0d0a 2020 2020 2020 2020  _list:..        
+0000e2c0: 2020 2020 2020 2020 2320 2020 2020 2020          #       
+0000e2d0: 2020 636f 6c6c 6563 7465 645f 706f 696e    collected_poin
+0000e2e0: 7473 2e61 7070 656e 6428 6b6a 290d 0a20  ts.append(kj).. 
+0000e2f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000e300: 2020 2020 2023 636f 6c6c 6563 7465 645f       #collected_
+0000e310: 706f 696e 7473 2e65 7874 656e 6428 7665  points.extend(ve
+0000e320: 7274 6963 6573 290d 0a20 2020 2020 2020  rtices)..       
+0000e330: 2020 2020 2020 2020 2023 2065 6c73 653a           # else:
+0000e340: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e350: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0000e360: 2020 2020 2020 2020 6d69 6464 6c65 203d          middle =
+0000e370: 206c 696e 652e 696e 7465 7270 6f6c 6174   line.interpolat
+0000e380: 6528 302e 352c 206e 6f72 6d61 6c69 7a65  e(0.5, normalize
+0000e390: 643d 5472 7565 292e 636f 6f72 6473 5b30  d=True).coords[0
+0000e3a0: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000e3b0: 2020 2070 3220 3d20 6c69 6e65 2e69 6e74     p2 = line.int
+0000e3c0: 6572 706f 6c61 7465 2830 2e32 352c 206e  erpolate(0.25, n
+0000e3d0: 6f72 6d61 6c69 7a65 643d 5472 7565 292e  ormalized=True).
+0000e3e0: 636f 6f72 6473 5b30 5d0d 0a20 2020 2020  coords[0]..     
+0000e3f0: 2020 2020 2020 2020 2020 2070 3120 3d20             p1 = 
+0000e400: 6c69 6e65 2e69 6e74 6572 706f 6c61 7465  line.interpolate
+0000e410: 2830 2e37 352c 206e 6f72 6d61 6c69 7a65  (0.75, normalize
+0000e420: 643d 5472 7565 292e 636f 6f72 6473 5b30  d=True).coords[0
+0000e430: 5d0d 0a0d 0a20 2020 2020 2020 2020 2020  ]....           
+0000e440: 2020 2020 2063 6f6c 6c65 6374 6564 5f70       collected_p
+0000e450: 6f69 6e74 732e 6170 7065 6e64 285b 7374  oints.append([st
+0000e460: 6172 742c 206d 6964 646c 652c 2065 6e64  art, middle, end
+0000e470: 2c20 7031 2c70 325d 290d 0a0d 0a20 2020  , p1,p2])....   
+0000e480: 2020 2020 2072 6574 7572 6e20 636f 6c6c       return coll
+0000e490: 6563 7465 645f 706f 696e 7473 0d0a 0d0a  ected_points....
+0000e4a0: 2020 2020 2320 6465 6620 636f 6c6c 6563      # def collec
+0000e4b0: 745f 706f 696e 7473 5f66 726f 6d5f 6c69  t_points_from_li
+0000e4c0: 6e65 2867 6466 293a 0d0a 2020 2020 2320  ne(gdf):..    # 
+0000e4d0: 2020 2020 2320 496e 6974 6961 6c69 7a65      # Initialize
+0000e4e0: 2061 6e20 656d 7074 7920 6c69 7374 2074   an empty list t
+0000e4f0: 6f20 7374 6f72 6520 7468 6520 636f 6f72  o store the coor
+0000e500: 6469 6e61 7465 730d 0a20 2020 2023 2020  dinates..    #  
+0000e510: 2020 2063 6f6c 6c65 6374 6564 5f70 6f69     collected_poi
+0000e520: 6e74 7320 3d20 5b5d 0d0a 0d0a 2020 2020  nts = []....    
+0000e530: 2320 2020 2020 2320 4974 6572 6174 6520  #     # Iterate 
+0000e540: 7468 726f 7567 6820 7468 6520 4765 6f44  through the GeoD
+0000e550: 6174 6146 7261 6d65 0d0a 2020 2020 2320  ataFrame..    # 
+0000e560: 2020 2020 666f 7220 6765 6f6d 6574 7279      for geometry
+0000e570: 2069 6e20 6764 665b 2767 656f 6d65 7472   in gdf['geometr
+0000e580: 7927 5d3a 0d0a 2020 2020 2320 2020 2020  y']:..    #     
+0000e590: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+0000e5a0: 6528 6765 6f6d 6574 7279 2c20 4c69 6e65  e(geometry, Line
+0000e5b0: 5374 7269 6e67 293a 0d0a 2020 2020 2320  String):..    # 
+0000e5c0: 2020 2020 2020 2020 2020 2020 2320 436f              # Co
+0000e5d0: 756e 7420 7468 6520 6e75 6d62 6572 206f  unt the number o
+0000e5e0: 6620 7665 7274 6963 6573 2069 6e20 7468  f vertices in th
+0000e5f0: 6520 4c69 6e65 5374 7269 6e67 0d0a 2020  e LineString..  
+0000e600: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0000e610: 6e75 6d5f 7665 7274 6963 6573 203d 206c  num_vertices = l
+0000e620: 656e 2867 656f 6d65 7472 792e 636f 6f72  en(geometry.coor
+0000e630: 6473 290d 0a20 2020 2020 2020 2020 2020  ds)..           
+0000e640: 2020 2020 200d 0a20 2020 2023 2020 2020       ..    #    
+0000e650: 2020 2020 2020 2020 2023 2043 6865 636b           # Check
+0000e660: 2069 6620 7468 6520 4c69 6e65 5374 7269   if the LineStri
+0000e670: 6e67 2069 7320 7374 7261 6967 6874 2028  ng is straight (
+0000e680: 3320 6f72 2066 6577 6572 2076 6572 7469  3 or fewer verti
+0000e690: 6365 7329 0d0a 2020 2020 2320 2020 2020  ces)..    #     
+0000e6a0: 2020 2020 2020 2020 6966 206e 756d 5f76          if num_v
+0000e6b0: 6572 7469 6365 7320 3c3d 2033 3a0d 0a20  ertices <= 3:.. 
+0000e6c0: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000e6d0: 2020 2020 2023 2046 6f72 2073 7472 6169       # For strai
+0000e6e0: 6768 7420 6c69 6e65 732c 2074 616b 6520  ght lines, take 
+0000e6f0: 636f 6f72 6469 6e61 7465 7320 6f66 2073  coordinates of s
+0000e700: 7461 7274 2c20 656e 642c 2061 6e64 206d  tart, end, and m
+0000e710: 6964 646c 650d 0a20 2020 2023 2020 2020  iddle..    #    
+0000e720: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000e730: 7274 5f70 6f69 6e74 203d 2067 656f 6d65  rt_point = geome
+0000e740: 7472 792e 636f 6f72 6473 5b30 5d0d 0a20  try.coords[0].. 
+0000e750: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000e760: 2020 2020 2065 6e64 5f70 6f69 6e74 203d       end_point =
+0000e770: 2067 656f 6d65 7472 792e 636f 6f72 6473   geometry.coords
+0000e780: 5b2d 315d 0d0a 2020 2020 2320 2020 2020  [-1]..    #     
+0000e790: 2020 2020 2020 2020 2020 2020 6d69 6464              midd
+0000e7a0: 6c65 5f70 6f69 6e74 203d 2067 656f 6d65  le_point = geome
+0000e7b0: 7472 792e 696e 7465 7270 6f6c 6174 6528  try.interpolate(
+0000e7c0: 302e 352c 206e 6f72 6d61 6c69 7a65 643d  0.5, normalized=
+0000e7d0: 5472 7565 292e 636f 6f72 6473 5b30 5d0d  True).coords[0].
+0000e7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e7f0: 2020 2020 200d 0a20 2020 2023 2020 2020       ..    #    
+0000e800: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0000e810: 6c65 6374 6564 5f70 6f69 6e74 732e 6578  lected_points.ex
+0000e820: 7465 6e64 285b 7374 6172 745f 706f 696e  tend([start_poin
+0000e830: 742c 206d 6964 646c 655f 706f 696e 742c  t, middle_point,
+0000e840: 2065 6e64 5f70 6f69 6e74 5d29 0d0a 2020   end_point])..  
+0000e850: 2020 2320 2020 2020 2020 2020 2020 2020    #             
+0000e860: 656c 7365 3a0d 0a20 2020 2023 2020 2020  else:..    #    
+0000e870: 2020 2020 2020 2020 2020 2020 2023 2046               # F
+0000e880: 6f72 2063 7572 7665 6420 6c69 6e65 732c  or curved lines,
+0000e890: 2074 616b 6520 636f 6f72 6469 6e61 7465   take coordinate
+0000e8a0: 7320 6f66 2061 6c6c 2076 6572 7469 6365  s of all vertice
+0000e8b0: 730d 0a20 2020 2023 2020 2020 2020 2020  s..    #        
+0000e8c0: 2020 2020 2020 2020 2066 6f72 2070 6f69           for poi
+0000e8d0: 6e74 2069 6e20 6765 6f6d 6574 7279 2e63  nt in geometry.c
+0000e8e0: 6f6f 7264 733a 0d0a 2020 2020 2320 2020  oords:..    #   
+0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e900: 2020 782c 2079 203d 2070 6f69 6e74 0d0a    x, y = point..
+0000e910: 2020 2020 2320 2020 2020 2020 2020 2020      #           
+0000e920: 2020 2020 2020 2020 2020 636f 6c6c 6563            collec
+0000e930: 7465 645f 706f 696e 7473 2e61 7070 656e  ted_points.appen
+0000e940: 6428 2878 2c20 7929 290d 0a20 2020 2020  d((x, y))..     
+0000e950: 2020 200d 0a20 2020 2023 2020 2020 2072     ..    #     r
+0000e960: 6574 7572 6e20 636f 6c6c 6563 7465 645f  eturn collected_
+0000e970: 706f 696e 7473 0d0a 0d0a 2320 4e6f 772c  points....# Now,
+0000e980: 2063 6f6f 7264 696e 6174 6573 5f6c 6973   coordinates_lis
+0000e990: 7420 636f 6e74 6169 6e73 2074 6865 2063  t contains the c
+0000e9a0: 6f6f 7264 696e 6174 6573 206f 6620 7374  oordinates of st
+0000e9b0: 6172 742c 2065 6e64 2c20 6d69 6464 6c65  art, end, middle
+0000e9c0: 2c20 616e 6420 616c 6c20 7665 7274 6963  , and all vertic
+0000e9d0: 6573 0d0a 2320 6261 7365 6420 6f6e 2077  es..# based on w
+0000e9e0: 6865 7468 6572 2074 6865 206c 696e 6520  hether the line 
+0000e9f0: 6973 2073 7472 6169 6768 7420 2833 206f  is straight (3 o
+0000ea00: 7220 6665 7765 7220 7665 7274 6963 6573  r fewer vertices
+0000ea10: 2920 6f72 2063 7572 7665 640d 0a20 2020  ) or curved..   
+0000ea20: 2020 2020 200d 0a20 2020 200d 0a0d 0a20       ..    .... 
+0000ea30: 2020 2064 6566 2064 7261 775f 706c 616e     def draw_plan
+0000ea40: 6573 5f66 726f 6d5f 6c69 6e65 7328 7878  es_from_lines(xx
+0000ea50: 2c79 7929 3a0d 0a20 2020 2020 2020 2067  ,yy):..        g
+0000ea60: 6c6f 6261 6c20 6178 5f32 642c 2061 785f  lobal ax_2d, ax_
+0000ea70: 3364 2c20 6461 7461 2c20 7472 616e 7366  3d, data, transf
+0000ea80: 6f72 6d2c 206c 6566 742c 2072 6967 6874  orm, left, right
+0000ea90: 2c20 626f 7474 6f6d 2c20 746f 702c 2070  , bottom, top, p
+0000eaa0: 6c61 6e65 7320 0d0a 2020 2020 2020 2020  lanes ..        
+0000eab0: 0d0a 2020 2020 2020 2020 6461 7461 2c20  ..        data, 
+0000eac0: 7472 616e 7366 6f72 6d2c 2070 726f 6a65  transform, proje
+0000ead0: 6374 696f 6e20 3d20 7265 6164 5f64 656d  ction = read_dem
+0000eae0: 2864 656d 5f64 6174 6129 0d0a 0d0a 2020  (dem_data)....  
+0000eaf0: 2020 2020 2020 6764 6620 3d20 6770 642e        gdf = gpd.
+0000eb00: 7265 6164 5f66 696c 6528 6c69 6e65 5f73  read_file(line_s
+0000eb10: 6861 7065 6669 6c65 290d 0a20 2020 2020  hapefile)..     
+0000eb20: 2020 2069 6620 6764 662e 6372 732e 746f     if gdf.crs.to
+0000eb30: 5f73 7472 696e 6728 2920 213d 2070 726f  _string() != pro
+0000eb40: 6a65 6374 696f 6e3a 0d0a 2020 2020 2020  jection:..      
+0000eb50: 2020 2020 2020 6764 6620 3d20 6764 662e        gdf = gdf.
+0000eb60: 746f 5f63 7273 2870 726f 6a65 6374 696f  to_crs(projectio
+0000eb70: 6e29 0d0a 0d0a 2020 2020 2020 2020 706f  n)....        po
+0000eb80: 696e 745f 7365 7473 203d 2063 6f6c 6c65  int_sets = colle
+0000eb90: 6374 5f70 6f69 6e74 735f 6672 6f6d 5f6c  ct_points_from_l
+0000eba0: 696e 6528 6764 6629 0d0a 2020 2020 2020  ine(gdf)..      
+0000ebb0: 2020 2320 785f 636f 6f72 6473 203d 206e    # x_coords = n
+0000ebc0: 702e 6c69 6e73 7061 6365 286c 6566 742c  p.linspace(left,
+0000ebd0: 2072 6967 6874 2c20 6461 7461 2e73 6861   right, data.sha
+0000ebe0: 7065 5b31 5d29 0d0a 2020 2020 2020 2020  pe[1])..        
+0000ebf0: 2320 795f 636f 6f72 6473 203d 206e 702e  # y_coords = np.
+0000ec00: 6c69 6e73 7061 6365 2874 6f70 2c20 626f  linspace(top, bo
+0000ec10: 7474 6f6d 2c20 6461 7461 2e73 6861 7065  ttom, data.shape
+0000ec20: 5b30 5d29 0d0a 2020 2020 2020 2020 2320  [0])..        # 
+0000ec30: 7878 2c20 7979 203d 206e 702e 6d65 7368  xx, yy = np.mesh
+0000ec40: 6772 6964 2878 5f63 6f6f 7264 732c 2079  grid(x_coords, y
+0000ec50: 5f63 6f6f 7264 7329 0d0a 2020 2020 2020  _coords)..      
+0000ec60: 2020 0d0a 2020 2020 2020 2020 6672 6f6d    ..        from
+0000ec70: 2074 7164 6d20 696d 706f 7274 2074 7164   tqdm import tqd
+0000ec80: 6d0d 0a20 2020 2020 2020 2070 6c61 6e65  m..        plane
+0000ec90: 733d 5b5d 0d0a 2020 2020 2020 2020 666f  s=[]..        fo
+0000eca0: 7220 706f 696e 7473 2069 6e20 7471 646d  r points in tqdm
+0000ecb0: 2870 6f69 6e74 5f73 6574 732c 2064 6573  (point_sets, des
+0000ecc0: 633d 2250 726f 6365 7373 696e 6720 6669  c="Processing fi
+0000ecd0: 7474 6564 2070 6c61 6e65 7322 293a 0d0a  tted planes"):..
+0000ece0: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+0000ecf0: 6e74 2827 706f 696e 7473 3a20 272c 2070  nt('points: ', p
+0000ed00: 6f69 6e74 7329 0d0a 2020 2020 2020 2020  oints)..        
+0000ed10: 2020 2020 237a 5f76 616c 7565 7320 3d20      #z_values = 
+0000ed20: 5b64 6174 615b 696e 7428 2870 6f69 6e74  [data[int((point
+0000ed30: 5b31 5d20 2d20 746f 7029 202f 2061 6273  [1] - top) / abs
+0000ed40: 2874 7261 6e73 666f 726d 5b35 5d29 292c  (transform[5])),
+0000ed50: 2069 6e74 2828 706f 696e 745b 305d 202d   int((point[0] -
+0000ed60: 206c 6566 7429 202f 2074 7261 6e73 666f   left) / transfo
+0000ed70: 726d 5b31 5d29 5d20 666f 7220 706f 696e  rm[1])] for poin
+0000ed80: 7420 696e 2070 6f69 6e74 735d 0d0a 2020  t in points]..  
+0000ed90: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0000eda0: 2020 2020 2020 2020 7a5f 7661 6c75 6573          z_values
+0000edb0: 203d 205b 5d0d 0a0d 0a20 2020 2020 2020   = []....       
+0000edc0: 2020 2020 2066 6f72 2070 6f69 6e74 2069       for point i
+0000edd0: 6e20 706f 696e 7473 3a0d 0a20 2020 2020  n points:..     
+0000ede0: 2020 2020 2020 2020 2020 2079 5f69 6e64             y_ind
+0000edf0: 6578 203d 2069 6e74 2828 706f 696e 745b  ex = int((point[
+0000ee00: 315d 202d 2074 6f70 2920 2f20 6162 7328  1] - top) / abs(
+0000ee10: 7472 616e 7366 6f72 6d5b 355d 2929 0d0a  transform[5]))..
+0000ee20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 2320 795f 696e 6465 7820 3d20 696e 7428  # y_index = int(
+0000ee40: 2870 6f69 6e74 5b31 5d20 2d20 746f 7029  (point[1] - top)
+0000ee50: 202f 2061 6273 2874 7261 6e73 666f 726d   / abs(transform
+0000ee60: 5b35 5d29 2920 6966 2069 7369 6e73 7461  [5])) if isinsta
+0000ee70: 6e63 6528 706f 696e 745b 315d 2c20 2869  nce(point[1], (i
+0000ee80: 6e74 2c20 666c 6f61 7429 2920 616e 6420  nt, float)) and 
+0000ee90: 6973 696e 7374 616e 6365 2874 7261 6e73  isinstance(trans
+0000eea0: 666f 726d 5b35 5d2c 2028 696e 742c 2066  form[5], (int, f
+0000eeb0: 6c6f 6174 2929 2065 6c73 6520 4e6f 6e65  loat)) else None
+0000eec0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000eed0: 2020 2320 785f 696e 6465 7820 3d20 696e    # x_index = in
+0000eee0: 7428 2870 6f69 6e74 5b30 5d20 2d20 746f  t((point[0] - to
+0000eef0: 7029 202f 2061 6273 2874 7261 6e73 666f  p) / abs(transfo
+0000ef00: 726d 5b31 5d29 2920 6966 2069 7369 6e73  rm[1])) if isins
+0000ef10: 7461 6e63 6528 706f 696e 745b 305d 2c20  tance(point[0], 
+0000ef20: 2869 6e74 2c20 666c 6f61 7429 2920 616e  (int, float)) an
+0000ef30: 6420 6973 696e 7374 616e 6365 2874 7261  d isinstance(tra
+0000ef40: 6e73 666f 726d 5b31 5d2c 2028 696e 742c  nsform[1], (int,
+0000ef50: 2066 6c6f 6174 2929 2065 6c73 6520 4e6f   float)) else No
+0000ef60: 6e65 0d0a 0d0a 2020 2020 2020 2020 2020  ne....          
+0000ef70: 2020 2020 2020 785f 696e 6465 7820 3d20        x_index = 
+0000ef80: 696e 7428 2870 6f69 6e74 5b30 5d20 2d20  int((point[0] - 
+0000ef90: 6c65 6674 2920 2f20 7472 616e 7366 6f72  left) / transfor
+0000efa0: 6d5b 315d 290d 0a20 2020 2020 2020 2020  m[1])..         
+0000efb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000efc0: 2020 2020 2020 2020 207a 5f76 616c 7565           z_value
+0000efd0: 203d 2064 6174 615b 795f 696e 6465 785d   = data[y_index]
+0000efe0: 5b78 5f69 6e64 6578 5d0d 0a20 2020 2020  [x_index]..     
+0000eff0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f000: 2020 2020 2020 2020 2020 2020 207a 5f76               z_v
+0000f010: 616c 7565 732e 6170 7065 6e64 287a 5f76  alues.append(z_v
+0000f020: 616c 7565 290d 0a0d 0a20 2020 2020 2020  alue)....       
+0000f030: 2020 2020 2078 797a 5f70 6f69 6e74 7320       xyz_points 
+0000f040: 3d20 5b70 6f69 6e74 735b 695d 202b 2028  = [points[i] + (
+0000f050: 7a5f 7661 6c75 6573 5b69 5d2c 2920 666f  z_values[i],) fo
+0000f060: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+0000f070: 287a 5f76 616c 7565 7329 295d 0d0a 0d0a  (z_values))]....
+0000f080: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0000f090: 656e 2878 797a 5f70 6f69 6e74 7329 203e  en(xyz_points) >
+0000f0a0: 3d20 333a 0d0a 2020 2020 2020 2020 2020  = 3:..          
+0000f0b0: 2020 2020 2020 6669 7474 6564 5f70 6c61        fitted_pla
+0000f0c0: 6e65 2c20 612c 2062 2c20 632c 2064 6970  ne, a, b, c, dip
+0000f0d0: 5f61 6e67 6c65 2c20 6469 705f 6469 7265  _angle, dip_dire
+0000f0e0: 6374 696f 6e20 3d20 6669 745f 706c 616e  ction = fit_plan
+0000f0f0: 6528 7879 7a5f 706f 696e 7473 2c20 7878  e(xyz_points, xx
+0000f100: 2c20 7979 290d 0a20 2020 2020 2020 2020  , yy)..         
+0000f110: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0000f120: 2020 2020 2020 2020 2064 6970 5f61 6e67           dip_ang
+0000f130: 6c65 5f6c 6973 742e 6170 7065 6e64 2864  le_list.append(d
+0000f140: 6970 5f61 6e67 6c65 290d 0a20 2020 2020  ip_angle)..     
+0000f150: 2020 2020 2020 2020 2020 2064 6970 5f64             dip_d
+0000f160: 6972 6563 7469 6f6e 5f6c 6973 742e 6170  irection_list.ap
+0000f170: 7065 6e64 2864 6970 5f64 6972 6563 7469  pend(dip_directi
+0000f180: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
+0000f190: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f1a0: 2020 2023 2069 6620 6c69 6d69 745f 6578     # if limit_ex
+0000f1b0: 7465 6e64 3a0d 0a20 2020 2020 2020 2020  tend:..         
+0000f1c0: 2020 2020 2020 2023 2020 2020 2023 2047         #     # G
+0000f1d0: 6574 2062 6f75 6e64 696e 6720 626f 7820  et bounding box 
+0000f1e0: 6f66 2074 6865 2073 656c 6563 7465 6420  of the selected 
+0000f1f0: 706f 696e 7473 0d0a 2020 2020 2020 2020  points..        
+0000f200: 2020 2020 2020 2020 2320 2020 2020 786d          #     xm
+0000f210: 696e 2c20 786d 6178 2c20 796d 696e 2c20  in, xmax, ymin, 
+0000f220: 796d 6178 203d 2062 6f75 6e64 696e 675f  ymax = bounding_
+0000f230: 626f 7828 7879 7a5f 706f 696e 7473 290d  box(xyz_points).
+0000f240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f250: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0000f260: 2020 2020 2020 2023 2020 2020 206d 6173         #     mas
+0000f270: 6b20 3d20 2878 7820 3e3d 2078 6d69 6e29  k = (xx >= xmin)
+0000f280: 2026 2028 7878 203c 3d20 786d 6178 2920   & (xx <= xmax) 
+0000f290: 2620 2879 7920 3e3d 2079 6d69 6e29 2026  & (yy >= ymin) &
+0000f2a0: 2028 7979 203c 3d20 796d 6178 290d 0a20   (yy <= ymax).. 
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0000f2d0: 2020 2020 2023 2020 2020 2066 6f72 2069       #     for i
+0000f2e0: 2069 6e20 7261 6e67 6528 7878 2e73 6861   in range(xx.sha
+0000f2f0: 7065 5b30 5d29 3a0d 0a20 2020 2020 2020  pe[0]):..       
+0000f300: 2020 2020 2020 2020 2023 2020 2020 2020           #      
+0000f310: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+0000f320: 6528 7878 2e73 6861 7065 5b31 5d29 3a0d  e(xx.shape[1]):.
+0000f330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f340: 2023 2020 2020 2020 2020 2020 2020 2069   #             i
+0000f350: 6620 6e6f 7420 6d61 736b 5b69 2c20 6a5d  f not mask[i, j]
+0000f360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0000f370: 2020 2023 2020 2020 2020 2020 2020 2020     #            
+0000f380: 2020 2020 2066 6974 7465 645f 706c 616e       fitted_plan
+0000f390: 655b 692c 206a 5d20 3d20 6e70 2e6e 616e  e[i, j] = np.nan
+0000f3a0: 2020 2320 5365 7420 6f75 742d 6f66 2d62    # Set out-of-b
+0000f3b0: 6f75 6e64 7320 7661 6c75 6573 2074 6f20  ounds values to 
+0000f3c0: 4e61 4e0d 0a20 2020 2020 2020 2020 2020  NaN..           
+0000f3d0: 2020 2020 2023 2323 2323 2323 2323 2323       ###########
+0000f3e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000f3f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0000f400: 2020 2020 2323 2323 2323 2323 230d 0a20      #########.. 
+0000f410: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0000f420: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000f430: 6e65 732e 6170 7065 6e64 2866 6974 7465  nes.append(fitte
+0000f440: 645f 706c 616e 6529 0d0a 2020 2020 2020  d_plane)..      
+0000f450: 2020 2020 2020 2020 2020 2370 6c61 6e65            #plane
+0000f460: 5f63 6f6c 6f72 203d 2072 616e 646f 6d5f  _color = random_
+0000f470: 636f 6c6f 7228 290d 0a20 2020 2020 2020  color()..       
+0000f480: 2020 2020 2020 2020 2070 6c61 6e65 5f63           plane_c
+0000f490: 6f6c 6f72 3d63 6f6c 6f72 5f66 726f 6d5f  olor=color_from_
+0000f4a0: 6469 705f 616e 645f 6469 7265 6374 696f  dip_and_directio
+0000f4b0: 6e28 6469 705f 616e 676c 652c 2064 6970  n(dip_angle, dip
+0000f4c0: 5f64 6972 6563 7469 6f6e 290d 0a20 2020  _direction)..   
+0000f4d0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000f4e0: 6e65 5f63 6f6c 6f72 732e 6170 7065 6e64  ne_colors.append
+0000f4f0: 2870 6c61 6e65 5f63 6f6c 6f72 290d 0a20  (plane_color).. 
+0000f500: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+0000f510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f520: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
+0000f530: 2020 2020 2020 2020 2023 2323 230d 0a20           ####.. 
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000f550: 6f72 2070 6f69 6e74 6e20 696e 2078 797a  or pointn in xyz
+0000f560: 5f70 6f69 6e74 733a 0d0a 2020 2020 2020  _points:..      
+0000f570: 2020 2020 2020 2020 2020 2020 2020 6178                ax
+0000f580: 5f32 642e 706c 6f74 2870 6f69 6e74 6e5b  _2d.plot(pointn[
+0000f590: 305d 2c20 706f 696e 746e 5b31 5d2c 2027  0], pointn[1], '
+0000f5a0: 6f27 2c20 636f 6c6f 723d 706c 616e 655f  o', color=plane_
+0000f5b0: 636f 6c6f 722c 2061 6c70 6861 3d30 2e37  color, alpha=0.7
+0000f5c0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000f5d0: 2020 2063 616e 7661 735f 3264 2e64 7261     canvas_2d.dra
+0000f5e0: 7728 290d 0a0d 0a20 2020 2020 2020 2020  w()....         
+0000f5f0: 2020 2020 2020 2023 6178 5f33 642e 636c         #ax_3d.cl
+0000f600: 6561 7228 290d 0a20 2020 2020 2020 2020  ear()..         
+0000f610: 2020 2020 2020 2061 785f 3364 2e73 6574         ax_3d.set
+0000f620: 5f74 6974 6c65 2827 3344 2044 454d 2077  _title('3D DEM w
+0000f630: 6974 6820 4669 7474 6564 2050 6c61 6e65  ith Fitted Plane
+0000f640: 7327 290d 0a20 2020 2020 2020 2020 2020  s')..           
+0000f650: 2020 2020 2061 785f 3364 2e70 6c6f 745f       ax_3d.plot_
+0000f660: 7375 7266 6163 6528 7878 2c20 7979 2c20  surface(xx, yy, 
+0000f670: 6461 7461 2c20 636d 6170 3d27 7465 7272  data, cmap='terr
+0000f680: 6169 6e27 2c20 6c69 6e65 7769 6474 683d  ain', linewidth=
+0000f690: 302c 2061 6e74 6961 6c69 6173 6564 3d54  0, antialiased=T
+0000f6a0: 7275 652c 2061 6c70 6861 3d30 2e35 290d  rue, alpha=0.5).
+0000f6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f6c0: 2023 666f 7220 706c 616e 6520 696e 2070   #for plane in p
+0000f6d0: 6c61 6e65 733a 0d0a 2020 2020 2020 2020  lanes:..        
+0000f6e0: 2020 2020 2020 2020 6178 5f33 642e 706c          ax_3d.pl
+0000f6f0: 6f74 5f73 7572 6661 6365 2878 782c 2079  ot_surface(xx, y
+0000f700: 792c 2066 6974 7465 645f 706c 616e 652c  y, fitted_plane,
+0000f710: 2061 6c70 6861 3d30 2e36 2c20 6c69 6e65   alpha=0.6, line
+0000f720: 7769 6474 683d 302c 2061 6e74 6961 6c69  width=0, antiali
+0000f730: 6173 6564 3d54 7275 652c 2063 6f6c 6f72  ased=True, color
+0000f740: 3d70 6c61 6e65 5f63 6f6c 6f72 290d 0a20  =plane_color).. 
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f760: 616e 7661 735f 3364 2e64 7261 7728 290d  anvas_3d.draw().
+0000f770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f780: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0000f790: 2020 2070 6c6f 745f 706c 616e 6573 2864     plot_planes(d
+0000f7a0: 6970 5f61 6e67 6c65 5f6c 6973 742c 2064  ip_angle_list, d
+0000f7b0: 6970 5f64 6972 6563 7469 6f6e 5f6c 6973  ip_direction_lis
+0000f7c0: 742c 2070 6c61 6e65 5f63 6f6c 6f72 7329  t, plane_colors)
+0000f7d0: 0d0a 2020 2020 2020 2020 2020 2020 0d0a  ..            ..
+0000f7e0: 2020 2020 2020 2020 0d0a 2020 2020 0d0a          ..    ..
+0000f7f0: 0d0a 2020 2020 6465 6620 706c 6f74 5f64  ..    def plot_d
+0000f800: 656d 2864 6174 612c 2074 7261 6e73 666f  em(data, transfo
+0000f810: 726d 2c20 7072 6f6a 6563 7469 6f6e 2c20  rm, projection, 
+0000f820: 7061 7468 5f74 6f5f 7368 6170 6566 696c  path_to_shapefil
+0000f830: 6529 3a0d 0a20 2020 2020 2020 2067 6c6f  e):..        glo
+0000f840: 6261 6c20 6178 5f32 642c 2061 785f 3364  bal ax_2d, ax_3d
+0000f850: 2c20 706f 696e 7473 2c20 6361 6e76 6173  , points, canvas
+0000f860: 5f32 642c 2063 616e 7661 735f 3364 2c20  _2d, canvas_3d, 
+0000f870: 706f 696e 7473 5f6c 6973 7462 6f78 2c20  points_listbox, 
+0000f880: 706c 616e 6573 2c20 706c 616e 655f 636f  planes, plane_co
+0000f890: 6c6f 7273 2c20 6873 2c20 6c65 6674 2c20  lors, hs, left, 
+0000f8a0: 7269 6768 742c 2062 6f74 746f 6d2c 2074  right, bottom, t
+0000f8b0: 6f70 0d0a 2020 2020 2020 2020 706f 696e  op..        poin
+0000f8c0: 7473 203d 205b 5d0d 0a20 2020 2020 2020  ts = []..       
+0000f8d0: 2070 6c61 6e65 7320 3d20 5b5d 0d0a 2020   planes = []..  
+0000f8e0: 2020 2020 2020 706c 616e 655f 636f 6c6f        plane_colo
+0000f8f0: 7273 203d 205b 5d0d 0a20 2020 2020 2020  rs = []..       
+0000f900: 200d 0a20 2020 2020 2020 200d 0a0d 0a20   ..        .... 
+0000f910: 2020 2020 2020 2068 7320 3d20 6573 2e68         hs = es.h
+0000f920: 696c 6c73 6861 6465 2864 6174 6129 0d0a  illshade(data)..
+0000f930: 0d0a 2020 2020 2020 2020 726f 6f74 203d  ..        root =
+0000f940: 2074 6b2e 546b 2829 0d0a 2020 2020 2020   tk.Tk()..      
+0000f950: 2020 726f 6f74 2e74 6974 6c65 2822 416b    root.title("Ak
+0000f960: 6864 6566 6f5f 4669 7450 6c61 6e65 7322  hdefo_FitPlanes"
+0000f970: 290d 0a0d 0a20 2020 2020 2020 206c 6566  )....        lef
+0000f980: 742c 2063 656c 6c5f 7369 7a65 5f78 2c20  t, cell_size_x, 
+0000f990: 5f2c 2074 6f70 2c20 5f2c 2063 656c 6c5f  _, top, _, cell_
+0000f9a0: 7369 7a65 5f79 203d 2074 7261 6e73 666f  size_y = transfo
+0000f9b0: 726d 0d0a 2020 2020 2020 2020 0d0a 2020  rm..        ..  
+0000f9c0: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+0000f9d0: 6967 6874 203d 206c 6566 7420 2b20 6365  ight = left + ce
+0000f9e0: 6c6c 5f73 697a 655f 7820 2a20 6461 7461  ll_size_x * data
+0000f9f0: 2e73 6861 7065 5b31 5d0d 0a20 2020 2020  .shape[1]..     
+0000fa00: 2020 2062 6f74 746f 6d20 3d20 746f 7020     bottom = top 
+0000fa10: 2b20 6365 6c6c 5f73 697a 655f 7920 2a20  + cell_size_y * 
+0000fa20: 6461 7461 2e73 6861 7065 5b30 5d0d 0a0d  data.shape[0]...
+0000fa30: 0a20 2020 2020 2020 2066 6967 3120 3d20  .        fig1 = 
+0000fa40: 706c 742e 4669 6775 7265 2866 6967 7369  plt.Figure(figsi
+0000fa50: 7a65 3d28 362c 2036 292c 2064 7069 3d31  ze=(6, 6), dpi=1
+0000fa60: 3530 290d 0a20 2020 2020 2020 2061 785f  50)..        ax_
+0000fa70: 3264 203d 2066 6967 312e 6164 645f 7375  2d = fig1.add_su
+0000fa80: 6270 6c6f 7428 3131 3129 0d0a 2020 2020  bplot(111)..    
+0000fa90: 2020 2020 6178 5f32 642e 696d 7368 6f77      ax_2d.imshow
+0000faa0: 2868 732c 2063 6d61 703d 2767 7261 7927  (hs, cmap='gray'
+0000fab0: 2c20 6578 7465 6e74 3d5b 6c65 6674 2c20  , extent=[left, 
+0000fac0: 7269 6768 742c 2062 6f74 746f 6d2c 2074  right, bottom, t
+0000fad0: 6f70 5d29 0d0a 2020 2020 2020 2020 6178  op])..        ax
+0000fae0: 5f32 642e 7365 745f 7469 746c 6528 2748  _2d.set_title('H
+0000faf0: 696c 6c73 6861 6465 272c 2066 6f6e 7477  illshade', fontw
+0000fb00: 6569 6768 743d 2262 6f6c 6422 2c20 666f  eight="bold", fo
+0000fb10: 6e74 7369 7a65 3d31 3429 0d0a 2020 2020  ntsize=14)..    
+0000fb20: 2020 2020 6178 5f32 642e 7365 745f 786c      ax_2d.set_xl
+0000fb30: 6162 656c 2822 4c6f 6e67 6974 7564 6522  abel("Longitude"
+0000fb40: 2c20 666f 6e74 7369 7a65 3d31 3229 0d0a  , fontsize=12)..
+0000fb50: 2020 2020 2020 2020 6178 5f32 642e 7365          ax_2d.se
+0000fb60: 745f 796c 6162 656c 2822 4c61 7469 7475  t_ylabel("Latitu
+0000fb70: 6465 222c 2066 6f6e 7473 697a 653d 3132  de", fontsize=12
+0000fb80: 290d 0a20 2020 2020 2020 2061 785f 3264  )..        ax_2d
+0000fb90: 2e67 7269 6428 5472 7565 2c20 7768 6963  .grid(True, whic
+0000fba0: 683d 2762 6f74 6827 2c20 6c69 6e65 7374  h='both', linest
+0000fbb0: 796c 653d 272d 2d27 2c20 6c69 6e65 7769  yle='--', linewi
+0000fbc0: 6474 683d 302e 3529 0d0a 2020 2020 2020  dth=0.5)..      
+0000fbd0: 2020 6178 5f32 642e 7365 745f 6173 7065    ax_2d.set_aspe
+0000fbe0: 6374 2827 6571 7561 6c27 290d 0a20 2020  ct('equal')..   
+0000fbf0: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+0000fc00: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+0000fc10: 2020 2069 6620 7061 7468 5f74 6f5f 7368     if path_to_sh
+0000fc20: 6170 6566 696c 6520 6973 206e 6f74 204e  apefile is not N
+0000fc30: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+0000fc40: 2020 6764 6620 3d20 6770 642e 7265 6164    gdf = gpd.read
+0000fc50: 5f66 696c 6528 7061 7468 5f74 6f5f 7368  _file(path_to_sh
+0000fc60: 6170 6566 696c 6529 0d0a 2020 2020 2020  apefile)..      
+0000fc70: 2020 2020 2020 6966 2067 6466 2e63 7273        if gdf.crs
+0000fc80: 2e74 6f5f 7374 7269 6e67 2829 2021 3d20  .to_string() != 
+0000fc90: 7072 6f6a 6563 7469 6f6e 3a0d 0a20 2020  projection:..   
+0000fca0: 2020 2020 2020 2020 2020 2020 2067 6466               gdf
+0000fcb0: 203d 2067 6466 2e74 6f5f 6372 7328 7072   = gdf.to_crs(pr
+0000fcc0: 6f6a 6563 7469 6f6e 290d 0a20 2020 2020  ojection)..     
+0000fcd0: 2020 2020 2020 2067 6466 2e70 6c6f 7428         gdf.plot(
+0000fce0: 6178 3d61 785f 3264 2c20 636f 6c6f 723d  ax=ax_2d, color=
+0000fcf0: 2772 6564 272c 206c 6162 656c 3d22 4c69  'red', label="Li
+0000fd00: 6e65 6172 2046 6561 7475 7265 7322 290d  near Features").
+0000fd10: 0a20 2020 2020 2020 2020 2020 2061 785f  .            ax_
+0000fd20: 3264 2e6c 6567 656e 6428 6c6f 633d 2275  2d.legend(loc="u
+0000fd30: 7070 6572 206c 6566 7422 290d 0a20 2020  pper left")..   
+0000fd40: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
+0000fd50: 6967 3220 3d20 706c 742e 4669 6775 7265  ig2 = plt.Figure
+0000fd60: 2866 6967 7369 7a65 3d28 362c 2036 292c  (figsize=(6, 6),
+0000fd70: 2064 7069 3d31 3530 290d 0a20 2020 2020   dpi=150)..     
+0000fd80: 2020 2023 2043 7265 6174 6520 6120 6669     # Create a fi
+0000fd90: 6775 7265 2061 6e64 2061 7869 730d 0a20  gure and axis.. 
+0000fda0: 2020 2020 2020 2061 785f 3364 203d 2066         ax_3d = f
+0000fdb0: 6967 322e 6164 645f 7375 6270 6c6f 7428  ig2.add_subplot(
+0000fdc0: 3131 312c 2070 726f 6a65 6374 696f 6e3d  111, projection=
+0000fdd0: 2733 6427 290d 0a20 2020 2020 2020 2061  '3d')..        a
+0000fde0: 785f 3364 2e73 6574 5f74 6974 6c65 2827  x_3d.set_title('
+0000fdf0: 3344 2044 454d 2077 6974 6820 4669 7474  3D DEM with Fitt
+0000fe00: 6564 2050 6c61 6e65 7327 2c20 666f 6e74  ed Planes', font
+0000fe10: 7765 6967 6874 3d22 626f 6c64 222c 2066  weight="bold", f
+0000fe20: 6f6e 7473 697a 653d 3134 290d 0a20 2020  ontsize=14)..   
+0000fe30: 2020 2020 2061 785f 3364 2e73 6574 5f78       ax_3d.set_x
+0000fe40: 6c61 6265 6c28 224c 6f6e 6769 7475 6465  label("Longitude
+0000fe50: 222c 2066 6f6e 7473 697a 653d 3132 290d  ", fontsize=12).
+0000fe60: 0a20 2020 2020 2020 2061 785f 3364 2e73  .        ax_3d.s
+0000fe70: 6574 5f79 6c61 6265 6c28 224c 6174 6974  et_ylabel("Latit
+0000fe80: 7564 6522 2c20 666f 6e74 7369 7a65 3d31  ude", fontsize=1
+0000fe90: 3229 0d0a 2020 2020 2020 2020 6178 5f33  2)..        ax_3
+0000fea0: 642e 7365 745f 7a6c 6162 656c 2822 456c  d.set_zlabel("El
+0000feb0: 6576 6174 696f 6e22 2c20 666f 6e74 7369  evation", fontsi
+0000fec0: 7a65 3d31 3229 0d0a 2020 2020 2020 2020  ze=12)..        
+0000fed0: 785f 636f 6f72 6473 203d 206e 702e 6c69  x_coords = np.li
+0000fee0: 6e73 7061 6365 286c 6566 742c 2072 6967  nspace(left, rig
+0000fef0: 6874 2c20 6461 7461 2e73 6861 7065 5b31  ht, data.shape[1
+0000ff00: 5d29 0d0a 2020 2020 2020 2020 795f 636f  ])..        y_co
+0000ff10: 6f72 6473 203d 206e 702e 6c69 6e73 7061  ords = np.linspa
+0000ff20: 6365 2874 6f70 2c20 626f 7474 6f6d 2c20  ce(top, bottom, 
+0000ff30: 6461 7461 2e73 6861 7065 5b30 5d29 0d0a  data.shape[0])..
+0000ff40: 2020 2020 2020 2020 7878 2c20 7979 203d          xx, yy =
+0000ff50: 206e 702e 6d65 7368 6772 6964 2878 5f63   np.meshgrid(x_c
+0000ff60: 6f6f 7264 732c 2079 5f63 6f6f 7264 7329  oords, y_coords)
+0000ff70: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0000ff80: 2020 2020 0d0a 2020 2020 2020 2020 0d0a      ..        ..
+0000ff90: 0d0a 2020 2020 2020 2020 0d0a 0d0a 2020  ..        ....  
+0000ffa0: 2020 2020 2020 2320 6178 5f33 642e 7365        # ax_3d.se
+0000ffb0: 745f 786c 696d 285b 6c65 6674 2c20 7269  t_xlim([left, ri
+0000ffc0: 6768 745d 290d 0a20 2020 2020 2020 2023  ght])..        #
+0000ffd0: 2061 785f 3364 2e73 6574 5f79 6c69 6d28   ax_3d.set_ylim(
+0000ffe0: 5b62 6f74 746f 6d2c 2074 6f70 5d29 0d0a  [bottom, top])..
+0000fff0: 2020 2020 2020 2020 2320 6178 5f33 642e          # ax_3d.
+00010000: 7365 745f 7a6c 696d 285b 7a6d 696e 2c20  set_zlim([zmin, 
+00010010: 7a6d 6178 5d29 0d0a 0d0a 2020 2020 2020  zmax])....      
+00010020: 2020 6672 616d 655f 3264 203d 2074 6b2e    frame_2d = tk.
+00010030: 4672 616d 6528 726f 6f74 290d 0a20 2020  Frame(root)..   
+00010040: 2020 2020 2066 7261 6d65 5f32 642e 6772       frame_2d.gr
+00010050: 6964 2872 6f77 3d30 2c20 636f 6c75 6d6e  id(row=0, column
+00010060: 3d30 2c20 7374 6963 6b79 3d27 6e73 6577  =0, sticky='nsew
+00010070: 2729 0d0a 2020 2020 2020 2020 2320 6361  ')..        # ca
+00010080: 6e76 6173 5f32 6420 3d20 4669 6775 7265  nvas_2d = Figure
+00010090: 4361 6e76 6173 546b 4167 6728 6669 6731  CanvasTkAgg(fig1
+000100a0: 2c20 6d61 7374 6572 3d66 7261 6d65 5f32  , master=frame_2
+000100b0: 6429 0d0a 2020 2020 2020 2020 2320 6361  d)..        # ca
+000100c0: 6e76 6173 5f32 642e 6765 745f 746b 5f77  nvas_2d.get_tk_w
+000100d0: 6964 6765 7428 292e 7061 636b 2866 696c  idget().pack(fil
+000100e0: 6c3d 746b 2e42 4f54 482c 2065 7870 616e  l=tk.BOTH, expan
+000100f0: 643d 4661 6c73 6529 0d0a 2020 2020 2020  d=False)..      
+00010100: 2020 2320 746f 6f6c 6261 725f 3264 203d    # toolbar_2d =
+00010110: 204e 6176 6967 6174 696f 6e54 6f6f 6c62   NavigationToolb
+00010120: 6172 3254 6b28 6361 6e76 6173 5f32 642c  ar2Tk(canvas_2d,
+00010130: 2066 7261 6d65 5f32 6429 0d0a 2020 2020   frame_2d)..    
+00010140: 2020 2020 2320 746f 6f6c 6261 725f 3264      # toolbar_2d
+00010150: 2e75 7064 6174 6528 290d 0a20 2020 2020  .update()..     
+00010160: 2020 2023 2043 7265 6174 6520 7468 6520     # Create the 
+00010170: 6361 6e76 6173 2066 6f72 2074 6865 2070  canvas for the p
+00010180: 6c6f 740d 0a20 2020 2020 2020 2063 616e  lot..        can
+00010190: 7661 735f 3264 203d 2046 6967 7572 6543  vas_2d = FigureC
+000101a0: 616e 7661 7354 6b41 6767 2866 6967 312c  anvasTkAgg(fig1,
+000101b0: 206d 6173 7465 723d 6672 616d 655f 3264   master=frame_2d
+000101c0: 290d 0a20 2020 2020 2020 2063 616e 7661  )..        canva
+000101d0: 735f 3264 2e67 6574 5f74 6b5f 7769 6467  s_2d.get_tk_widg
+000101e0: 6574 2829 2e70 6163 6b28 6669 6c6c 3d74  et().pack(fill=t
+000101f0: 6b2e 424f 5448 2c20 6578 7061 6e64 3d54  k.BOTH, expand=T
+00010200: 7275 6529 2020 2320 4669 6c6c 2074 6865  rue)  # Fill the
+00010210: 2066 7261 6d65 0d0a 2020 2020 2020 2020   frame..        
+00010220: 2320 4372 6561 7465 2074 6865 2074 6f6f  # Create the too
+00010230: 6c62 6172 2061 6e64 2070 6c61 6365 2069  lbar and place i
+00010240: 7420 6174 2074 6865 2074 6f70 206f 6620  t at the top of 
+00010250: 7468 6520 6361 6e76 6173 0d0a 2020 2020  the canvas..    
+00010260: 2020 2020 746f 6f6c 6261 725f 3264 203d      toolbar_2d =
+00010270: 204e 6176 6967 6174 696f 6e54 6f6f 6c62   NavigationToolb
+00010280: 6172 3254 6b28 6361 6e76 6173 5f32 642c  ar2Tk(canvas_2d,
+00010290: 2066 7261 6d65 5f32 6429 0d0a 2020 2020   frame_2d)..    
+000102a0: 2020 2020 746f 6f6c 6261 725f 3264 2e75      toolbar_2d.u
+000102b0: 7064 6174 6528 290d 0a20 2020 2020 2020  pdate()..       
+000102c0: 2074 6f6f 6c62 6172 5f32 642e 7061 636b   toolbar_2d.pack
+000102d0: 2873 6964 653d 746b 2e54 4f50 2c20 6669  (side=tk.TOP, fi
+000102e0: 6c6c 3d74 6b2e 5829 2020 2320 5061 636b  ll=tk.X)  # Pack
+000102f0: 2074 6865 2074 6f6f 6c62 6172 2061 7420   the toolbar at 
+00010300: 7468 6520 746f 700d 0a20 2020 2020 2020  the top..       
+00010310: 200d 0a20 2020 2020 2020 2023 2323 2323   ..        #####
+00010320: 2323 6164 6420 636f 6c6f 7262 6172 2066  ##add colorbar f
+00010330: 6967 7572 6520 746f 2043 616e 7661 730d  igure to Canvas.
+00010340: 0a20 2020 2020 2020 200d 0a0d 0a0d 0a0d  .        .......
+00010350: 0a20 2020 2020 2020 2066 7261 6d65 5f33  .        frame_3
+00010360: 6420 3d20 746b 2e46 7261 6d65 2872 6f6f  d = tk.Frame(roo
+00010370: 7429 0d0a 2020 2020 2020 2020 6672 616d  t)..        fram
+00010380: 655f 3364 2e67 7269 6428 726f 773d 302c  e_3d.grid(row=0,
+00010390: 2063 6f6c 756d 6e3d 312c 2073 7469 636b   column=1, stick
+000103a0: 793d 276e 7365 7727 290d 0a20 2020 2020  y='nsew')..     
+000103b0: 2020 2023 2063 616e 7661 735f 3364 203d     # canvas_3d =
+000103c0: 2046 6967 7572 6543 616e 7661 7354 6b41   FigureCanvasTkA
+000103d0: 6767 2866 6967 322c 206d 6173 7465 723d  gg(fig2, master=
+000103e0: 6672 616d 655f 3364 290d 0a20 2020 2020  frame_3d)..     
+000103f0: 2020 2023 2063 616e 7661 735f 3364 2e67     # canvas_3d.g
+00010400: 6574 5f74 6b5f 7769 6467 6574 2829 2e70  et_tk_widget().p
+00010410: 6163 6b28 6669 6c6c 3d74 6b2e 424f 5448  ack(fill=tk.BOTH
+00010420: 2c20 6578 7061 6e64 3d46 616c 7365 290d  , expand=False).
+00010430: 0a20 2020 2020 2020 2023 2074 6f6f 6c62  .        # toolb
+00010440: 6172 5f33 6420 3d20 4e61 7669 6761 7469  ar_3d = Navigati
+00010450: 6f6e 546f 6f6c 6261 7232 546b 2863 616e  onToolbar2Tk(can
+00010460: 7661 735f 3364 2c20 6672 616d 655f 3364  vas_3d, frame_3d
+00010470: 290d 0a20 2020 2020 2020 2023 2074 6f6f  )..        # too
+00010480: 6c62 6172 5f33 642e 7570 6461 7465 2829  lbar_3d.update()
+00010490: 0d0a 2020 2020 2020 2020 6361 6e76 6173  ..        canvas
+000104a0: 5f33 6420 3d20 4669 6775 7265 4361 6e76  _3d = FigureCanv
+000104b0: 6173 546b 4167 6728 6669 6732 2c20 6d61  asTkAgg(fig2, ma
+000104c0: 7374 6572 3d66 7261 6d65 5f33 6429 0d0a  ster=frame_3d)..
+000104d0: 2020 2020 2020 2020 6361 6e76 6173 5f33          canvas_3
+000104e0: 642e 6765 745f 746b 5f77 6964 6765 7428  d.get_tk_widget(
+000104f0: 292e 7061 636b 2866 696c 6c3d 746b 2e42  ).pack(fill=tk.B
+00010500: 4f54 482c 2065 7870 616e 643d 5472 7565  OTH, expand=True
+00010510: 2920 2023 2046 696c 6c20 7468 6520 6672  )  # Fill the fr
+00010520: 616d 650d 0a20 2020 2020 2020 2023 2043  ame..        # C
+00010530: 7265 6174 6520 7468 6520 746f 6f6c 6261  reate the toolba
+00010540: 7220 616e 6420 706c 6163 6520 6974 2061  r and place it a
+00010550: 7420 7468 6520 746f 7020 6f66 2074 6865  t the top of the
+00010560: 2063 616e 7661 730d 0a20 2020 2020 2020   canvas..       
+00010570: 2074 6f6f 6c62 6172 5f33 6420 3d20 4e61   toolbar_3d = Na
+00010580: 7669 6761 7469 6f6e 546f 6f6c 6261 7232  vigationToolbar2
+00010590: 546b 2863 616e 7661 735f 3364 2c20 6672  Tk(canvas_3d, fr
+000105a0: 616d 655f 3364 290d 0a20 2020 2020 2020  ame_3d)..       
+000105b0: 2074 6f6f 6c62 6172 5f33 642e 7570 6461   toolbar_3d.upda
+000105c0: 7465 2829 0d0a 2020 2020 2020 2020 746f  te()..        to
+000105d0: 6f6c 6261 725f 3364 2e70 6163 6b28 7369  olbar_3d.pack(si
+000105e0: 6465 3d74 6b2e 544f 502c 2066 696c 6c3d  de=tk.TOP, fill=
+000105f0: 746b 2e58 2920 2023 2050 6163 6b20 7468  tk.X)  # Pack th
+00010600: 6520 746f 6f6c 6261 7220 6174 2074 6865  e toolbar at the
+00010610: 2074 6f70 0d0a 0d0a 2020 2020 2020 2020   top....        
+00010620: 2320 4372 6561 7465 2061 2066 7261 6d65  # Create a frame
+00010630: 206f 6e20 7468 6520 7269 6768 7420 746f   on the right to
+00010640: 2068 6f6c 6420 636f 6e74 726f 6c73 0d0a   hold controls..
+00010650: 2020 2020 2020 2020 636f 6e74 726f 6c73          controls
+00010660: 5f66 7261 6d65 203d 2074 6b2e 4672 616d  _frame = tk.Fram
+00010670: 6528 726f 6f74 290d 0a20 2020 2020 2020  e(root)..       
+00010680: 2063 6f6e 7472 6f6c 735f 6672 616d 652e   controls_frame.
+00010690: 6772 6964 2872 6f77 3d30 2c20 636f 6c75  grid(row=0, colu
+000106a0: 6d6e 3d33 2c20 726f 7773 7061 6e3d 312c  mn=3, rowspan=1,
+000106b0: 2073 7469 636b 793d 276e 7365 7727 290d   sticky='nsew').
+000106c0: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
+000106d0: 2020 2020 2023 204e 6f77 2070 7574 2061       # Now put a
+000106e0: 6c6c 2062 7574 746f 6e73 2061 6e64 204c  ll buttons and L
+000106f0: 6973 7462 6f78 2069 6e73 6964 6520 7468  istbox inside th
+00010700: 6973 2063 6f6e 7472 6f6c 735f 6672 616d  is controls_fram
+00010710: 650d 0a20 2020 2020 2020 2064 7261 775f  e..        draw_
+00010720: 6275 7474 6f6e 203d 2074 746b 2e42 7574  button = ttk.But
+00010730: 746f 6e28 636f 6e74 726f 6c73 5f66 7261  ton(controls_fra
+00010740: 6d65 2c20 7465 7874 3d22 4472 6177 2050  me, text="Draw P
+00010750: 6c61 6e65 222c 2063 6f6d 6d61 6e64 3d6c  lane", command=l
+00010760: 616d 6264 613a 2064 7261 775f 706c 616e  ambda: draw_plan
+00010770: 6528 7878 2c79 7929 290d 0a20 2020 2020  e(xx,yy))..     
+00010780: 2020 2064 7261 775f 6275 7474 6f6e 2e70     draw_button.p
+00010790: 6163 6b28 7061 6479 3d32 2c20 7061 6478  ack(pady=2, padx
+000107a0: 3d32 290d 0a0d 0a20 2020 2020 2020 206c  =2)....        l
+000107b0: 696e 655f 706c 616e 655f 6275 7474 6f6e  ine_plane_button
+000107c0: 203d 2074 746b 2e42 7574 746f 6e28 636f   = ttk.Button(co
+000107d0: 6e74 726f 6c73 5f66 7261 6d65 2c20 7465  ntrols_frame, te
+000107e0: 7874 3d22 4372 6561 7465 2050 6c61 6e65  xt="Create Plane
+000107f0: 7320 6672 6f6d 204c 696e 6573 222c 2063  s from Lines", c
+00010800: 6f6d 6d61 6e64 3d6c 616d 6264 613a 2064  ommand=lambda: d
+00010810: 7261 775f 706c 616e 6573 5f66 726f 6d5f  raw_planes_from_
+00010820: 6c69 6e65 7328 7878 2c79 7929 290d 0a20  lines(xx,yy)).. 
+00010830: 2020 2020 2020 206c 696e 655f 706c 616e         line_plan
+00010840: 655f 6275 7474 6f6e 2e70 6163 6b28 7061  e_button.pack(pa
+00010850: 6479 3d32 2c20 7061 6478 3d32 290d 0a0d  dy=2, padx=2)...
+00010860: 0a20 2020 2020 2020 2073 6176 655f 706c  .        save_pl
+00010870: 616e 655f 6275 7474 6f6e 203d 2074 746b  ane_button = ttk
+00010880: 2e42 7574 746f 6e28 636f 6e74 726f 6c73  .Button(controls
+00010890: 5f66 7261 6d65 2c20 7465 7874 3d22 5361  _frame, text="Sa
+000108a0: 7665 2050 6c61 6e65 7320 746f 204f 424a  ve Planes to OBJ
+000108b0: 222c 2063 6f6d 6d61 6e64 3d73 6176 655f  ", command=save_
+000108c0: 706c 616e 6573 5f74 6f5f 6f62 6a29 2023  planes_to_obj) #
+000108d0: 7361 7665 5f66 6974 7465 645f 706c 616e  save_fitted_plan
+000108e0: 6573 5f61 735f 6478 660d 0a20 2020 2020  es_as_dxf..     
+000108f0: 2020 2073 6176 655f 706c 616e 655f 6275     save_plane_bu
+00010900: 7474 6f6e 2e70 6163 6b28 7061 6479 3d32  tton.pack(pady=2
+00010910: 2c20 7061 6478 3d32 290d 0a20 2020 2020  , padx=2)..     
+00010920: 2020 2023 2073 6176 655f 706c 616e 655f     # save_plane_
+00010930: 6275 7474 6f6e 5f64 7866 203d 2074 746b  button_dxf = ttk
+00010940: 2e42 7574 746f 6e28 636f 6e74 726f 6c73  .Button(controls
+00010950: 5f66 7261 6d65 2c20 7465 7874 3d22 5361  _frame, text="Sa
+00010960: 7665 2050 6c61 6e65 7320 746f 2044 5846  ve Planes to DXF
+00010970: 222c 2063 6f6d 6d61 6e64 3d73 6176 655f  ", command=save_
+00010980: 6669 7474 6564 5f70 6c61 6e65 735f 6173  fitted_planes_as
+00010990: 5f64 7866 290d 0a20 2020 2020 2020 2023  _dxf)..        #
+000109a0: 2073 6176 655f 706c 616e 655f 6275 7474   save_plane_butt
+000109b0: 6f6e 5f64 7866 2e70 6163 6b28 7061 6479  on_dxf.pack(pady
+000109c0: 3d31 302c 2070 6164 783d 3130 290d 0a0d  =10, padx=10)...
+000109d0: 0a20 2020 2020 2020 2070 6f69 6e74 735f  .        points_
+000109e0: 6c69 7374 626f 7820 3d20 746b 2e4c 6973  listbox = tk.Lis
+000109f0: 7462 6f78 2863 6f6e 7472 6f6c 735f 6672  tbox(controls_fr
+00010a00: 616d 652c 2068 6569 6768 743d 352c 2077  ame, height=5, w
+00010a10: 6964 7468 3d34 302c 2065 7870 6f72 7473  idth=40, exports
+00010a20: 656c 6563 7469 6f6e 3d46 616c 7365 290d  election=False).
+00010a30: 0a20 2020 2020 2020 2070 6f69 6e74 735f  .        points_
+00010a40: 6c69 7374 626f 782e 7061 636b 2870 6164  listbox.pack(pad
+00010a50: 793d 322c 2070 6164 783d 322c 2066 696c  y=2, padx=2, fil
+00010a60: 6c3d 2762 6f74 6827 2c20 6578 7061 6e64  l='both', expand
+00010a70: 3d54 7275 6529 0d0a 2020 2020 2020 2020  =True)..        
+00010a80: 0d0a 2020 2020 2020 2020 7363 726f 6c6c  ..        scroll
+00010a90: 6261 7220 3d20 7474 6b2e 5363 726f 6c6c  bar = ttk.Scroll
+00010aa0: 6261 7228 636f 6e74 726f 6c73 5f66 7261  bar(controls_fra
+00010ab0: 6d65 2c20 6f72 6965 6e74 3d22 7665 7274  me, orient="vert
+00010ac0: 6963 616c 222c 2063 6f6d 6d61 6e64 3d70  ical", command=p
+00010ad0: 6f69 6e74 735f 6c69 7374 626f 782e 7976  oints_listbox.yv
+00010ae0: 6965 7729 0d0a 2020 2020 2020 2020 7363  iew)..        sc
+00010af0: 726f 6c6c 6261 722e 7061 636b 2873 6964  rollbar.pack(sid
+00010b00: 653d 746b 2e52 4947 4854 2c20 6669 6c6c  e=tk.RIGHT, fill
+00010b10: 3d74 6b2e 5929 0d0a 2020 2020 2020 2020  =tk.Y)..        
+00010b20: 0d0a 2020 2020 2020 2020 706f 696e 7473  ..        points
+00010b30: 5f6c 6973 7462 6f78 2e63 6f6e 6669 6728  _listbox.config(
+00010b40: 7973 6372 6f6c 6c63 6f6d 6d61 6e64 3d73  yscrollcommand=s
+00010b50: 6372 6f6c 6c62 6172 2e73 6574 290d 0a20  crollbar.set).. 
+00010b60: 2020 2020 2020 2070 6f69 6e74 735f 6c69         points_li
+00010b70: 7374 626f 782e 6269 6e64 2822 3c44 6f75  stbox.bind("<Dou
+00010b80: 626c 652d 4275 7474 6f6e 2d31 3e22 2c20  ble-Button-1>", 
+00010b90: 6f6e 5f70 6f69 6e74 5f64 6f75 626c 655f  on_point_double_
+00010ba0: 636c 6963 6b29 0d0a 2020 2020 2020 2020  click)..        
+00010bb0: 2323 2323 0d0a 2020 2020 0d0a 2020 2020  ####..    ..    
+00010bc0: 2020 2020 0d0a 2020 2020 2020 2020 2323      ..        ##
+00010bd0: 2323 0d0a 0d0a 2020 2020 2020 2020 6669  ##....        fi
+00010be0: 6731 2e63 616e 7661 732e 6d70 6c5f 636f  g1.canvas.mpl_co
+00010bf0: 6e6e 6563 7428 2762 7574 746f 6e5f 7072  nnect('button_pr
+00010c00: 6573 735f 6576 656e 7427 2c20 6c61 6d62  ess_event', lamb
+00010c10: 6461 2065 7665 6e74 3a20 6f6e 636c 6963  da event: onclic
+00010c20: 6b28 6576 656e 742c 2070 6f69 6e74 732c  k(event, points,
+00010c30: 2064 6174 612c 2074 7261 6e73 666f 726d   data, transform
+00010c40: 2929 0d0a 2020 2020 2020 2020 0d0a 2020  ))..        ..  
+00010c50: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00010c60: 2320 4164 6469 6e67 2074 6865 2073 697a  # Adding the siz
+00010c70: 6520 6772 6970 2066 6f72 2077 696e 646f  e grip for windo
+00010c80: 7720 7265 7369 7a69 6e67 0d0a 2020 2020  w resizing..    
+00010c90: 2020 2020 7369 7a65 6772 6970 203d 2074      sizegrip = t
+00010ca0: 746b 2e53 697a 6567 7269 7028 726f 6f74  tk.Sizegrip(root
+00010cb0: 290d 0a20 2020 2020 2020 2073 697a 6567  )..        sizeg
+00010cc0: 7269 702e 6772 6964 2872 6f77 3d33 2c20  rip.grid(row=3, 
+00010cd0: 636f 6c75 6d6e 3d31 2c20 7374 6963 6b79  column=1, sticky
+00010ce0: 3d27 6e73 6577 2729 0d0a 0d0a 2020 2020  ='nsew')....    
+00010cf0: 2020 2020 2320 4d61 6b69 6e67 2074 6865      # Making the
+00010d00: 2064 6573 6967 6e20 7265 7370 6f6e 7369   design responsi
+00010d10: 7665 0d0a 2020 2020 2020 2020 726f 6f74  ve..        root
+00010d20: 2e67 7269 645f 726f 7763 6f6e 6669 6775  .grid_rowconfigu
+00010d30: 7265 2830 2c20 7765 6967 6874 3d31 2920  re(0, weight=1) 
+00010d40: 2023 2043 616e 7661 7320 726f 770d 0a20   # Canvas row.. 
+00010d50: 2020 2020 2020 2072 6f6f 742e 6772 6964         root.grid
+00010d60: 5f72 6f77 636f 6e66 6967 7572 6528 312c  _rowconfigure(1,
+00010d70: 2077 6569 6768 743d 3029 2020 2320 546f   weight=0)  # To
+00010d80: 6f6c 6261 7220 726f 770d 0a20 2020 2020  olbar row..     
+00010d90: 2020 2072 6f6f 742e 6772 6964 5f72 6f77     root.grid_row
+00010da0: 636f 6e66 6967 7572 6528 322c 2077 6569  configure(2, wei
+00010db0: 6768 743d 3029 2020 2320 4275 7474 6f6e  ght=0)  # Button
+00010dc0: 2072 6f77 0d0a 2020 2020 2020 2020 726f   row..        ro
+00010dd0: 6f74 2e67 7269 645f 636f 6c75 6d6e 636f  ot.grid_columnco
+00010de0: 6e66 6967 7572 6528 302c 2077 6569 6768  nfigure(0, weigh
+00010df0: 743d 3129 2020 2320 3244 2070 6c6f 7420  t=1)  # 2D plot 
+00010e00: 636f 6c75 6d6e 0d0a 2020 2020 2020 2020  column..        
+00010e10: 726f 6f74 2e67 7269 645f 636f 6c75 6d6e  root.grid_column
+00010e20: 636f 6e66 6967 7572 6528 312c 2077 6569  configure(1, wei
+00010e30: 6768 743d 3129 2020 2320 3344 2070 6c6f  ght=1)  # 3D plo
+00010e40: 7420 636f 6c75 6d6e 0d0a 2020 2020 2020  t column..      
+00010e50: 2020 0d0a 2020 2020 2020 2020 0d0a 2020    ..        ..  
+00010e60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00010e70: 2020 2020 2020 2020 726f 6f74 2e6d 6169          root.mai
+00010e80: 6e6c 6f6f 7028 290d 0a0d 0a0d 0a20 2020  nloop()......   
+00010e90: 200d 0a20 2020 2070 6c6f 745f 6465 6d28   ..    plot_dem(
+00010ea0: 6461 7461 2c20 7472 616e 7366 6f72 6d2c  data, transform,
+00010eb0: 2070 726f 6a65 6374 696f 6e2c 206c 696e   projection, lin
+00010ec0: 655f 7368 6170 6566 696c 6529 0d0a 2020  e_shapefile)..  
+00010ed0: 200d 0a20 2020 200d 0a23 616b 6864 6566   ..    ..#akhdef
+00010ee0: 6f5f 6669 7450 6c61 6e65 2864 656d 5f64  o_fitPlane(dem_d
+00010ef0: 6174 613d 2763 7572 7269 652f 6465 6d5f  ata='currie/dem_
+00010f00: 316d 2e74 6966 272c 206c 696e 655f 7368  1m.tif', line_sh
+00010f10: 6170 6566 696c 653d 2763 7572 7269 652f  apefile='currie/
+00010f20: 6c69 6e65 732e 7368 7027 2c20 6f75 745f  lines.shp', out_
+00010f30: 706c 616e 6546 6f6c 6465 723d 2750 6c61  planeFolder='Pla
+00010f40: 6e65 735f 6f75 742f 6e65 7727 2c20 6c69  nes_out/new', li
+00010f50: 6d69 745f 6578 7465 6e64 3d46 616c 7365  mit_extend=False
+00010f60: 290d 0a0d 0a69 6d70 6f72 7420 6f73 0d0a  )....import os..
+00010f70: 696d 706f 7274 2073 6875 7469 6c0d 0a0d  import shutil...
+00010f80: 0a64 6566 206d 6f76 655f 6669 6c65 735f  .def move_files_
+00010f90: 7769 7468 5f73 7472 696e 6728 736f 7572  with_string(sour
+00010fa0: 6365 5f64 6972 3a20 7374 7220 3d22 222c  ce_dir: str ="",
+00010fb0: 2064 6573 745f 6469 723a 2073 7472 203d   dest_dir: str =
+00010fc0: 2222 2c20 7365 6172 6368 5f73 7472 696e  "", search_strin
+00010fd0: 673a 2073 7472 203d 222e 7469 6622 293a  g: str =".tif"):
+00010fe0: 0d0a 2020 2020 2222 220d 0a20 2020 204d  ..    """..    M
+00010ff0: 6f76 6520 6669 6c65 7320 6672 6f6d 2061  ove files from a
+00011000: 2073 6f75 7263 6520 6469 7265 6374 6f72   source director
+00011010: 7920 746f 2061 2064 6573 7469 6e61 7469  y to a destinati
+00011020: 6f6e 2064 6972 6563 746f 7279 2062 6173  on directory bas
+00011030: 6564 206f 6e20 6120 7365 6172 6368 2073  ed on a search s
+00011040: 7472 696e 6720 7072 6573 656e 7420 696e  tring present in
+00011050: 2074 6865 6972 2070 6174 6873 2e0d 0a0d   their paths....
+00011060: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
+00011070: 0d0a 2020 2020 2d20 736f 7572 6365 5f64  ..    - source_d
+00011080: 6972 2028 7374 7229 3a20 5468 6520 6469  ir (str): The di
+00011090: 7265 6374 6f72 7920 6672 6f6d 2077 6869  rectory from whi
+000110a0: 6368 2066 696c 6573 2061 7265 2074 6f20  ch files are to 
+000110b0: 6265 206d 6f76 6564 2e0d 0a20 2020 202d  be moved...    -
+000110c0: 2064 6573 745f 6469 7220 2873 7472 293a   dest_dir (str):
+000110d0: 2054 6865 2064 6573 7469 6e61 7469 6f6e   The destination
+000110e0: 2064 6972 6563 746f 7279 2077 6865 7265   directory where
+000110f0: 2066 696c 6573 2077 696c 6c20 6265 206d   files will be m
+00011100: 6f76 6564 2e0d 0a20 2020 202d 2073 6561  oved...    - sea
+00011110: 7263 685f 7374 7269 6e67 2028 7374 7229  rch_string (str)
+00011120: 3a20 5468 6520 7374 7269 6e67 2074 6f20  : The string to 
+00011130: 7365 6172 6368 2066 6f72 2069 6e20 7468  search for in th
+00011140: 6520 6669 6c65 2070 6174 6873 2e0d 0a0d  e file paths....
+00011150: 0a20 2020 2054 6869 7320 6675 6e63 7469  .    This functi
+00011160: 6f6e 2074 7261 7665 7273 6573 2074 6865  on traverses the
+00011170: 2073 6f75 7263 6520 6469 7265 6374 6f72   source director
+00011180: 792c 2069 6e63 6c75 6469 6e67 2069 7473  y, including its
+00011190: 2073 7562 6469 7265 6374 6f72 6965 732e   subdirectories.
+000111a0: 200d 0a20 2020 2046 696c 6573 2077 686f   ..    Files who
+000111b0: 7365 2070 6174 6873 2063 6f6e 7461 696e  se paths contain
+000111c0: 2074 6865 2073 6561 7263 6820 7374 7269   the search stri
+000111d0: 6e67 2061 7265 206d 6f76 6564 2074 6f20  ng are moved to 
+000111e0: 7468 6520 6465 7374 696e 6174 696f 6e20  the destination 
+000111f0: 6469 7265 6374 6f72 792e 200d 0a20 2020  directory. ..   
+00011200: 2049 6620 6120 6669 6c65 2077 6974 6820   If a file with 
+00011210: 7468 6520 7361 6d65 206e 616d 6520 6578  the same name ex
+00011220: 6973 7473 2069 6e20 7468 6520 6465 7374  ists in the dest
+00011230: 696e 6174 696f 6e2c 2069 7427 7320 7265  ination, it's re
+00011240: 6e61 6d65 6420 746f 2061 766f 6964 206f  named to avoid o
+00011250: 7665 7277 7269 7469 6e67 2e0d 0a0d 0a20  verwriting..... 
+00011260: 2020 2045 7272 6f72 7320 6475 7269 6e67     Errors during
+00011270: 2066 696c 6520 6d6f 7665 6d65 6e74 2028   file movement (
+00011280: 652e 672e 2c20 7065 726d 6973 7369 6f6e  e.g., permission
+00011290: 2069 7373 7565 732c 206e 6f6e 2d65 7869   issues, non-exi
+000112a0: 7374 656e 7420 6469 7265 6374 6f72 6965  stent directorie
+000112b0: 7329 2061 7265 206c 6f67 6765 6420 6275  s) are logged bu
+000112c0: 7420 646f 206e 6f74 2073 746f 7020 7468  t do not stop th
+000112d0: 6520 7072 6f63 6573 732e 0d0a 2020 2020  e process...    
+000112e0: 2222 220d 0a0d 0a20 2020 2069 6620 6e6f  """....    if no
+000112f0: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
+00011300: 2873 6f75 7263 655f 6469 7229 3a0d 0a20  (source_dir):.. 
+00011310: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00011320: 7565 4572 726f 7228 6622 536f 7572 6365  ueError(f"Source
+00011330: 2064 6972 6563 746f 7279 2027 7b73 6f75   directory '{sou
+00011340: 7263 655f 6469 727d 2720 646f 6573 206e  rce_dir}' does n
+00011350: 6f74 2065 7869 7374 2e22 290d 0a0d 0a20  ot exist.").... 
+00011360: 2020 2023 2043 7265 6174 6520 7468 6520     # Create the 
+00011370: 6465 7374 696e 6174 696f 6e20 6469 7265  destination dire
+00011380: 6374 6f72 7920 6966 2069 7420 646f 6573  ctory if it does
+00011390: 6e27 7420 6578 6973 740d 0a20 2020 2069  n't exist..    i
+000113a0: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
+000113b0: 6973 7473 2864 6573 745f 6469 7229 3a0d  ists(dest_dir):.
+000113c0: 0a20 2020 2020 2020 206f 732e 6d61 6b65  .        os.make
+000113d0: 6469 7273 2864 6573 745f 6469 7229 0d0a  dirs(dest_dir)..
+000113e0: 0d0a 2020 2020 666f 7220 726f 6f74 2c20  ..    for root, 
+000113f0: 6469 7273 2c20 6669 6c65 7320 696e 206f  dirs, files in o
+00011400: 732e 7761 6c6b 2873 6f75 7263 655f 6469  s.walk(source_di
+00011410: 7229 3a0d 0a20 2020 2020 2020 2066 6f72  r):..        for
+00011420: 2066 696c 6520 696e 2066 696c 6573 3a0d   file in files:.
+00011430: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00011440: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
+00011450: 2e6a 6f69 6e28 726f 6f74 2c20 6669 6c65  .join(root, file
+00011460: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00011470: 6620 7365 6172 6368 5f73 7472 696e 6720  f search_string 
+00011480: 696e 2066 696c 655f 7061 7468 3a0d 0a20  in file_path:.. 
+00011490: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000114a0: 6573 745f 6669 6c65 5f70 6174 6820 3d20  est_file_path = 
+000114b0: 6f73 2e70 6174 682e 6a6f 696e 2864 6573  os.path.join(des
+000114c0: 745f 6469 722c 2066 696c 6529 0d0a 0d0a  t_dir, file)....
+000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000114e0: 2320 4368 6563 6b20 6966 2074 6865 2066  # Check if the f
+000114f0: 696c 6520 616c 7265 6164 7920 6578 6973  ile already exis
+00011500: 7473 2069 6e20 6465 7374 696e 6174 696f  ts in destinatio
+00011510: 6e0d 0a20 2020 2020 2020 2020 2020 2020  n..             
+00011520: 2020 2063 6f75 6e74 6572 203d 2031 0d0a     counter = 1..
+00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011540: 7768 696c 6520 6f73 2e70 6174 682e 6578  while os.path.ex
+00011550: 6973 7473 2864 6573 745f 6669 6c65 5f70  ists(dest_file_p
+00011560: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
+00011570: 2020 2020 2020 2020 2020 2023 2053 706c             # Spl
+00011580: 6974 2066 696c 656e 616d 6520 616e 6420  it filename and 
+00011590: 6578 7465 6e73 696f 6e0d 0a20 2020 2020  extension..     
+000115a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000115b0: 696c 655f 6261 7365 2c20 6669 6c65 5f65  ile_base, file_e
+000115c0: 7874 656e 7369 6f6e 203d 206f 732e 7061  xtension = os.pa
+000115d0: 7468 2e73 706c 6974 6578 7428 6669 6c65  th.splitext(file
+000115e0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+000115f0: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00011600: 6120 6e65 7720 6669 6c65 6e61 6d65 2077  a new filename w
+00011610: 6974 6820 6120 636f 756e 7465 7220 746f  ith a counter to
+00011620: 2061 766f 6964 206f 7665 7277 7269 7469   avoid overwriti
+00011630: 6e67 0d0a 2020 2020 2020 2020 2020 2020  ng..            
+00011640: 2020 2020 2020 2020 6465 7374 5f66 696c          dest_fil
+00011650: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
+00011660: 2e6a 6f69 6e28 6465 7374 5f64 6972 2c20  .join(dest_dir, 
+00011670: 6622 7b66 696c 655f 6261 7365 7d5f 7b63  f"{file_base}_{c
+00011680: 6f75 6e74 6572 7d7b 6669 6c65 5f65 7874  ounter}{file_ext
+00011690: 656e 7369 6f6e 7d22 290d 0a20 2020 2020  ension}")..     
+000116a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000116b0: 6f75 6e74 6572 202b 3d20 310d 0a0d 0a20  ounter += 1.... 
+000116c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000116d0: 204d 6f76 6520 7468 6520 6669 6c65 2074   Move the file t
+000116e0: 6f20 7468 6520 6465 7374 696e 6174 696f  o the destinatio
+000116f0: 6e20 6469 7265 6374 6f72 790d 0a20 2020  n directory..   
+00011700: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00011710: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00011720: 2020 2020 2020 2073 6875 7469 6c2e 6d6f         shutil.mo
+00011730: 7665 2866 696c 655f 7061 7468 2c20 6465  ve(file_path, de
+00011740: 7374 5f66 696c 655f 7061 7468 290d 0a20  st_file_path).. 
+00011750: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00011760: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+00011770: 6173 2065 3a0d 0a20 2020 2020 2020 2020  as e:..         
+00011780: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00011790: 2866 2245 7272 6f72 206d 6f76 696e 6720  (f"Error moving 
+000117a0: 6669 6c65 207b 6669 6c65 5f70 6174 687d  file {file_path}
+000117b0: 2074 6f20 7b64 6573 745f 6669 6c65 5f70   to {dest_file_p
+000117c0: 6174 687d 3a20 7b65 7d22 290d 0a0d 0a23  ath}: {e}")....#
+000117d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000117e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000117f0: 2323 2323 2323 2323 2323 2323 0d0a 2354  ############..#T
+00011800: 6869 7320 7061 7274 2069 7320 7374 696c  his part is stil
+00011810: 6c20 756e 6465 7220 636f 6e73 7472 7563  l under construc
+00011820: 7469 6f6e 0d0a 0d0a 696d 706f 7274 206e  tion....import n
+00011830: 756d 7079 2061 7320 6e70 0d0a 0d0a 6465  umpy as np....de
+00011840: 6620 7061 7274 6961 6c5f 6465 7269 7661  f partial_deriva
+00011850: 7469 7665 2866 2c20 6478 2c20 6479 293a  tive(f, dx, dy):
+00011860: 0d0a 2020 2020 2222 220d 0a20 2020 2043  ..    """..    C
+00011870: 616c 6375 6c61 7465 2074 6865 2063 656e  alculate the cen
+00011880: 7472 616c 2064 6966 6665 7265 6e63 6520  tral difference 
+00011890: 6170 7072 6f78 696d 6174 696f 6e20 666f  approximation fo
+000118a0: 7220 7468 6520 7061 7274 6961 6c20 6465  r the partial de
+000118b0: 7269 7661 7469 7665 730d 0a20 2020 206f  rivatives..    o
+000118c0: 6620 6120 3244 2066 756e 6374 696f 6e20  f a 2D function 
+000118d0: 7769 7468 2072 6573 7065 6374 2074 6f20  with respect to 
+000118e0: 7820 616e 6420 792e 0d0a 0d0a 2020 2020  x and y.....    
+000118f0: 3a70 6172 616d 2066 3a20 3244 206e 756d  :param f: 2D num
+00011900: 7079 2061 7272 6179 206f 6620 6675 6e63  py array of func
+00011910: 7469 6f6e 2076 616c 7565 732c 2072 6570  tion values, rep
+00011920: 7265 7365 6e74 696e 6720 7468 6520 7261  resenting the ra
+00011930: 7374 6572 0d0a 2020 2020 3a70 6172 616d  ster..    :param
+00011940: 2064 783a 2053 7061 6369 6e67 2069 6e20   dx: Spacing in 
+00011950: 7468 6520 782d 6469 7265 6374 696f 6e20  the x-direction 
+00011960: 2861 7373 756d 6564 2074 6f20 6265 2063  (assumed to be c
+00011970: 6f6e 7374 616e 7429 0d0a 2020 2020 3a70  onstant)..    :p
+00011980: 6172 616d 2064 793a 2053 7061 6369 6e67  aram dy: Spacing
+00011990: 2069 6e20 7468 6520 792d 6469 7265 6374   in the y-direct
+000119a0: 696f 6e20 2861 7373 756d 6564 2074 6f20  ion (assumed to 
+000119b0: 6265 2063 6f6e 7374 616e 7429 0d0a 2020  be constant)..  
+000119c0: 2020 3a72 6574 7572 6e3a 2054 776f 2032    :return: Two 2
+000119d0: 4420 6e75 6d70 7920 6172 7261 7973 2c20  D numpy arrays, 
+000119e0: 6f6e 6520 666f 7220 7468 6520 7061 7274  one for the part
+000119f0: 6961 6c20 6465 7269 7661 7469 7665 2077  ial derivative w
+00011a00: 6974 6820 7265 7370 6563 7420 746f 2078  ith respect to x
+00011a10: 2028 6466 5f64 7829 0d0a 2020 2020 2020   (df_dx)..      
+00011a20: 2020 2020 2020 2061 6e64 206f 6e65 2066         and one f
+00011a30: 6f72 2074 6865 2070 6172 7469 616c 2064  or the partial d
+00011a40: 6572 6976 6174 6976 6520 7769 7468 2072  erivative with r
+00011a50: 6573 7065 6374 2074 6f20 7920 2864 665f  espect to y (df_
+00011a60: 6479 290d 0a20 2020 2022 2222 0d0a 2020  dy)..    """..  
+00011a70: 2020 2023 2049 6e69 7469 616c 697a 6520     # Initialize 
+00011a80: 6172 7261 7973 2074 6f20 7374 6f72 6520  arrays to store 
+00011a90: 7468 6520 7061 7274 6961 6c20 6465 7269  the partial deri
+00011aa0: 7661 7469 7665 730d 0a20 2020 2064 665f  vatives..    df_
+00011ab0: 6478 203d 206e 702e 7a65 726f 735f 6c69  dx = np.zeros_li
+00011ac0: 6b65 2866 290d 0a20 2020 2064 665f 6479  ke(f)..    df_dy
+00011ad0: 203d 206e 702e 7a65 726f 735f 6c69 6b65   = np.zeros_like
+00011ae0: 2866 290d 0a0d 0a20 2020 2023 2043 6f6d  (f)....    # Com
+00011af0: 7075 7465 2074 6865 2070 6172 7469 616c  pute the partial
+00011b00: 2064 6572 6976 6174 6976 6573 2066 6f72   derivatives for
+00011b10: 2074 6865 2069 6e74 6572 6e61 6c20 706f   the internal po
+00011b20: 696e 7473 0d0a 2020 2020 666f 7220 7869  ints..    for xi
+00011b30: 2069 6e20 7261 6e67 6528 312c 2066 2e73   in range(1, f.s
+00011b40: 6861 7065 5b30 5d20 2d20 3129 3a0d 0a20  hape[0] - 1):.. 
+00011b50: 2020 2020 2020 2066 6f72 2079 6a20 696e         for yj in
+00011b60: 2072 616e 6765 2831 2c20 662e 7368 6170   range(1, f.shap
+00011b70: 655b 315d 202d 2031 293a 0d0a 2020 2020  e[1] - 1):..    
+00011b80: 2020 2020 2020 2020 6466 5f64 785b 7869          df_dx[xi
+00011b90: 2c20 796a 5d20 3d20 2866 5b78 6920 2b20  , yj] = (f[xi + 
+00011ba0: 312c 2079 6a5d 202d 2066 5b78 6920 2d20  1, yj] - f[xi - 
+00011bb0: 312c 2079 6a5d 2920 2f20 2832 202a 2064  1, yj]) / (2 * d
+00011bc0: 7829 0d0a 2020 2020 2020 2020 2020 2020  x)..            
+00011bd0: 6466 5f64 795b 7869 2c20 796a 5d20 3d20  df_dy[xi, yj] = 
+00011be0: 2866 5b78 692c 2079 6a20 2b20 315d 202d  (f[xi, yj + 1] -
+00011bf0: 2066 5b78 692c 2079 6a20 2d20 315d 2920   f[xi, yj - 1]) 
+00011c00: 2f20 2832 202a 2064 7929 0d0a 0d0a 2020  / (2 * dy)....  
+00011c10: 2020 2320 4861 6e64 6c65 2074 6865 2062    # Handle the b
+00011c20: 6f75 6e64 6172 6965 7320 6279 2073 6574  oundaries by set
+00011c30: 7469 6e67 2074 6865 2064 6572 6976 6174  ting the derivat
+00011c40: 6976 6520 746f 207a 6572 6f20 6f72 2075  ive to zero or u
+00011c50: 7369 6e67 206f 6e65 2d73 6964 6564 2064  sing one-sided d
+00011c60: 6966 6665 7265 6e63 6573 0d0a 2020 2020  ifferences..    
+00011c70: 2320 4865 7265 2077 6520 6368 6f6f 7365  # Here we choose
+00011c80: 2074 6f20 7365 7420 7468 6520 626f 756e   to set the boun
+00011c90: 6461 7279 2064 6572 6976 6174 6976 6520  dary derivative 
+00011ca0: 746f 207a 6572 6f0d 0a20 2020 2023 2041  to zero..    # A
+00011cb0: 6c74 6572 6e61 7469 7665 6c79 2c20 7573  lternatively, us
+00011cc0: 6520 666f 7277 6172 642f 6261 636b 7761  e forward/backwa
+00011cd0: 7264 2064 6966 6665 7265 6e63 6520 6174  rd difference at
+00011ce0: 2074 6865 2062 6f75 6e64 6172 6965 7320   the boundaries 
+00011cf0: 6966 206e 6565 6465 640d 0a0d 0a20 2020  if needed....   
+00011d00: 2072 6574 7572 6e20 6466 5f64 782c 2064   return df_dx, d
+00011d10: 665f 6479 0d0a 0d0a 0d0a 696d 706f 7274  f_dy......import
+00011d20: 206e 756d 7079 2061 7320 6e70 0d0a 696d   numpy as np..im
+00011d30: 706f 7274 2072 6173 7465 7269 6f0d 0a0d  port rasterio...
+00011d40: 0a64 6566 2063 616c 6375 6c61 7465 5f73  .def calculate_s
+00011d50: 6c6f 7065 2864 656d 2c20 6173 7065 6374  lope(dem, aspect
+00011d60: 2c20 6478 202c 2064 7929 3a0d 0a20 2020  , dx , dy):..   
+00011d70: 2022 2222 0d0a 2020 2020 4361 6c63 756c   """..    Calcul
+00011d80: 6174 6520 7468 6520 736c 6f70 6520 6174  ate the slope at
+00011d90: 2065 6163 6820 7069 7865 6c20 7573 696e   each pixel usin
+00011da0: 6720 7468 6520 6173 7065 6374 2074 6f20  g the aspect to 
+00011db0: 6465 7465 726d 696e 6520 6469 7265 6374  determine direct
+00011dc0: 696f 6e2e 0d0a 0d0a 2020 2020 5061 7261  ion.....    Para
+00011dd0: 6d65 7465 7273 3a0d 0a20 2020 2064 656d  meters:..    dem
+00011de0: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
+00011df0: 3a20 4469 6769 7461 6c20 456c 6576 6174  : Digital Elevat
+00011e00: 696f 6e20 4d6f 6465 6c20 2844 454d 2920  ion Model (DEM) 
+00011e10: 6172 7261 792e 0d0a 2020 2020 6173 7065  array...    aspe
+00011e20: 6374 2028 6e75 6d70 792e 6e64 6172 7261  ct (numpy.ndarra
+00011e30: 7929 3a20 4173 7065 6374 2061 7272 6179  y): Aspect array
+00011e40: 2e0d 0a20 2020 2064 7820 2866 6c6f 6174  ...    dx (float
+00011e50: 293a 2020 7820 5370 6174 6961 6c20 7265  ):  x Spatial re
+00011e60: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
+00011e70: 7261 7374 6572 2028 6469 7374 616e 6365  raster (distance
+00011e80: 2062 6574 7765 656e 2070 6978 656c 7329   between pixels)
+00011e90: 2e0d 0a20 2020 2064 7920 2866 6c6f 6174  ...    dy (float
+00011ea0: 293a 2020 7920 5370 6174 6961 6c20 7265  ):  y Spatial re
+00011eb0: 736f 6c75 7469 6f6e 206f 6620 7468 6520  solution of the 
+00011ec0: 7261 7374 6572 2028 6469 7374 616e 6365  raster (distance
+00011ed0: 2062 6574 7765 656e 2070 6978 656c 7329   between pixels)
+00011ee0: 2e0d 0a0d 0a20 2020 2052 6574 7572 6e73  .....    Returns
+00011ef0: 3a0d 0a20 2020 206e 756d 7079 2e6e 6461  :..    numpy.nda
+00011f00: 7272 6179 3a20 4172 7261 7920 6f66 2073  rray: Array of s
+00011f10: 6c6f 7065 2076 616c 7565 7320 696e 2064  lope values in d
+00011f20: 6567 7265 6573 2e0d 0a20 2020 2022 2222  egrees...    """
+00011f30: 0d0a 2020 2020 0d0a 2020 2020 2320 6772  ..    ..    # gr
+00011f40: 6164 5f79 2c20 6772 6164 5f78 203d 206e  ad_y, grad_x = n
+00011f50: 702e 6772 6164 6965 6e74 2864 656d 2c20  p.gradient(dem, 
+00011f60: 6478 2c20 6479 290d 0a20 2020 200d 0a20  dx, dy)..    .. 
+00011f70: 2020 200d 0a20 2020 2023 2041 7373 756d     ..    # Assum
+00011f80: 696e 6720 2764 656d 2720 616e 6420 2761  ing 'dem' and 'a
+00011f90: 7370 6563 7427 2061 7265 2079 6f75 7220  spect' are your 
+00011fa0: 6578 6973 7469 6e67 206e 756d 7079 2061  existing numpy a
+00011fb0: 7272 6179 730d 0a20 2020 2023 2043 6865  rrays..    # Che
+00011fc0: 636b 2069 6620 7468 6520 7368 6170 6573  ck if the shapes
+00011fd0: 2061 7265 2064 6966 6665 7265 6e74 0d0a   are different..
+00011fe0: 2020 2020 2320 6966 2064 656d 2e73 6861      # if dem.sha
+00011ff0: 7065 2021 3d20 6173 7065 6374 2e73 6861  pe != aspect.sha
+00012000: 7065 3a0d 0a20 2020 2023 2020 2020 2023  pe:..    #     #
+00012010: 2052 6573 697a 6520 2764 656d 2720 746f   Resize 'dem' to
+00012020: 206d 6174 6368 2074 6865 2073 6861 7065   match the shape
+00012030: 206f 6620 2761 7370 6563 7427 0d0a 2020   of 'aspect'..  
+00012040: 2020 2320 2020 2020 6173 7065 6374 203d    #     aspect =
+00012050: 206e 702e 7265 7369 7a65 2861 7370 6563   np.resize(aspec
+00012060: 742c 2064 656d 2e73 6861 7065 290d 0a20  t, dem.shape).. 
+00012070: 2020 2023 2065 6c73 653a 0d0a 2020 2020     # else:..    
+00012080: 2320 2020 2020 6173 7065 6374 203d 2061  #     aspect = a
+00012090: 7370 6563 740d 0a0d 0a0d 0a0d 0a20 2020  spect........   
+000120a0: 2067 7261 645f 792c 2067 7261 645f 7820   grad_y, grad_x 
+000120b0: 3d20 6e70 2e67 7261 6469 656e 7428 6465  = np.gradient(de
+000120c0: 6d2c 2064 782c 2064 7929 0d0a 2020 2020  m, dx, dy)..    
+000120d0: 2367 7261 645f 792c 2067 7261 645f 783d  #grad_y, grad_x=
+000120e0: 7061 7274 6961 6c5f 6465 7269 7661 7469  partial_derivati
+000120f0: 7665 2864 656d 2c20 6478 2c20 6479 290d  ve(dem, dx, dy).
+00012100: 0a0d 0a20 2020 2069 6620 6772 6164 5f78  ...    if grad_x
+00012110: 2e73 6861 7065 2021 3d20 6772 6164 5f79  .shape != grad_y
+00012120: 2e73 6861 7065 3a0d 0a20 2020 2020 2020  .shape:..       
+00012130: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00012140: 7228 2247 7261 6469 656e 7420 6172 7261  r("Gradient arra
+00012150: 7973 2068 6176 6520 6d69 736d 6174 6368  ys have mismatch
+00012160: 6564 2073 6861 7065 732e 2229 0d0a 2020  ed shapes.")..  
+00012170: 2020 0d0a 2020 2020 6173 7065 6374 5f72    ..    aspect_r
+00012180: 6164 6961 6e73 203d 206e 702e 6465 6732  adians = np.deg2
+00012190: 7261 6428 6173 7065 6374 290d 0a20 2020  rad(aspect)..   
+000121a0: 2064 6972 6563 7469 6f6e 616c 5f67 7261   directional_gra
+000121b0: 6420 3d20 6e70 2e63 6f73 2861 7370 6563  d = np.cos(aspec
+000121c0: 745f 7261 6469 616e 7329 202a 2067 7261  t_radians) * gra
+000121d0: 645f 7820 2b20 6e70 2e73 696e 2861 7370  d_x + np.sin(asp
+000121e0: 6563 745f 7261 6469 616e 7329 202a 2067  ect_radians) * g
+000121f0: 7261 645f 790d 0a20 2020 2023 736c 6f70  rad_y..    #slop
+00012200: 655f 6465 6772 6565 7320 3d20 6e70 2e72  e_degrees = np.r
+00012210: 6164 3264 6567 286e 702e 6172 6374 616e  ad2deg(np.arctan
+00012220: 2864 6972 6563 7469 6f6e 616c 5f67 7261  (directional_gra
+00012230: 6429 290d 0a20 2020 0d0a 2020 2020 2320  d))..   ..    # 
+00012240: 4361 6c63 756c 6174 6520 736c 6f70 6520  Calculate slope 
+00012250: 696e 2072 6164 6961 6e73 0d0a 2020 2020  in radians..    
+00012260: 736c 6f70 655f 7261 6469 616e 7320 3d20  slope_radians = 
+00012270: 6e70 2e61 7263 7461 6e28 6469 7265 6374  np.arctan(direct
+00012280: 696f 6e61 6c5f 6772 6164 290d 0a0d 0a20  ional_grad).... 
+00012290: 2020 2023 2045 6e73 7572 6520 736c 6f70     # Ensure slop
+000122a0: 6520 6973 2077 6974 6869 6e20 3020 746f  e is within 0 to
+000122b0: 20cf 802f 3220 7261 6469 616e 7320 2830   ../2 radians (0
+000122c0: 2074 6f20 3930 2064 6567 7265 6573 2920   to 90 degrees) 
+000122d0: 7261 6e67 650d 0a20 2020 2023 736c 6f70  range..    #slop
+000122e0: 655f 7261 6469 616e 7320 3d20 736c 6f70  e_radians = slop
+000122f0: 655f 7261 6469 616e 7320 2520 286e 702e  e_radians % (np.
+00012300: 7069 202f 2032 290d 0a0d 0a20 2020 2023  pi / 2)....    #
+00012310: 2043 6f6e 7665 7274 2073 6c6f 7065 2074   Convert slope t
+00012320: 6f20 6465 6772 6565 730d 0a20 2020 2073  o degrees..    s
+00012330: 6c6f 7065 5f64 6567 7265 6573 203d 2028  lope_degrees = (
+00012340: 6e70 2e72 6164 3264 6567 2873 6c6f 7065  np.rad2deg(slope
+00012350: 5f72 6164 6961 6e73 2929 2025 2039 3020  _radians)) % 90 
+00012360: 0d0a 2020 2020 2373 6c6f 7065 5f64 6567  ..    #slope_deg
+00012370: 7265 6573 3d20 2831 3335 2d73 6c6f 7065  rees= (135-slope
+00012380: 5f64 6567 7265 6573 2925 2039 3020 0d0a  _degrees)% 90 ..
+00012390: 2020 2020 0d0a 2020 200d 0a20 2020 200d      ..   ..    .
+000123a0: 0a20 2020 2072 6574 7572 6e20 736c 6f70  .    return slop
+000123b0: 655f 6465 6772 6565 732c 2064 6972 6563  e_degrees, direc
+000123c0: 7469 6f6e 616c 5f67 7261 640d 0a0d 0a64  tional_grad....d
+000123d0: 6566 2063 616c 6375 6c61 7465 5f68 6569  ef calculate_hei
+000123e0: 6768 745f 6368 616e 6765 2873 6c6f 7065  ght_change(slope
+000123f0: 2c20 6469 7374 616e 6365 2c20 6465 6d29  , distance, dem)
+00012400: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
+00012410: 4361 6c63 756c 6174 6520 7468 6520 6865  Calculate the he
+00012420: 6967 6874 2063 6861 6e67 6520 7573 696e  ight change usin
+00012430: 6720 7468 6520 736c 6f70 6520 616e 6420  g the slope and 
+00012440: 6469 7374 616e 6365 2066 6f72 2065 6163  distance for eac
+00012450: 6820 7069 7865 6c2e 0d0a 0d0a 2020 2020  h pixel.....    
+00012460: 5061 7261 6d65 7465 7273 3a0d 0a20 2020  Parameters:..   
+00012470: 2073 6c6f 7065 2028 6e75 6d70 792e 6e64   slope (numpy.nd
+00012480: 6172 7261 7929 3a20 4172 7261 7920 6f66  array): Array of
+00012490: 2073 6c6f 7065 2076 616c 7565 7320 696e   slope values in
+000124a0: 2064 6567 7265 6573 2e0d 0a20 2020 2064   degrees...    d
+000124b0: 6973 7461 6e63 6520 286e 756d 7079 2e6e  istance (numpy.n
+000124c0: 6461 7272 6179 293a 2041 7272 6179 206f  darray): Array o
+000124d0: 6620 6469 7374 616e 6365 2076 616c 7565  f distance value
+000124e0: 732e 0d0a 0d0a 2020 2020 5265 7475 726e  s.....    Return
+000124f0: 733a 0d0a 2020 2020 6e75 6d70 792e 6e64  s:..    numpy.nd
+00012500: 6172 7261 793a 2041 7272 6179 206f 6620  array: Array of 
+00012510: 6865 6967 6874 2063 6861 6e67 6573 2e0d  height changes..
+00012520: 0a20 2020 2022 2222 0d0a 2020 2020 736c  .    """..    sl
+00012530: 6f70 655f 7261 6469 616e 7320 3d20 6e70  ope_radians = np
+00012540: 2e64 6567 3272 6164 2873 6c6f 7065 290d  .deg2rad(slope).
+00012550: 0a20 2020 2068 6569 6768 745f 6368 616e  .    height_chan
+00012560: 6765 203d 206e 702e 7461 6e28 736c 6f70  ge = np.tan(slop
+00012570: 655f 7261 6469 616e 7329 202a 2064 6973  e_radians) * dis
+00012580: 7461 6e63 650d 0a20 2020 200d 0a20 2020  tance..    ..   
+00012590: 200d 0a20 2020 200d 0a20 2020 2072 6574   ..    ..    ret
+000125a0: 7572 6e20 6865 6967 6874 5f63 6861 6e67  urn height_chang
+000125b0: 6520 0d0a 0d0a 6465 6620 6361 6c63 756c  e ....def calcul
+000125c0: 6174 655f 766f 6c75 6d65 5f63 6861 6e67  ate_volume_chang
+000125d0: 6528 6865 6967 6874 5f63 6861 6e67 652c  e(height_change,
+000125e0: 2070 6978 656c 5f61 7265 6129 3a0d 0a20   pixel_area):.. 
+000125f0: 2020 2022 2222 0d0a 2020 2020 4361 6c63     """..    Calc
+00012600: 756c 6174 6520 7468 6520 766f 6c75 6d65  ulate the volume
+00012610: 2063 6861 6e67 6520 666f 7220 6561 6368   change for each
+00012620: 2070 6978 656c 2e0d 0a0d 0a20 2020 2050   pixel.....    P
+00012630: 6172 616d 6574 6572 733a 0d0a 2020 2020  arameters:..    
+00012640: 6865 6967 6874 5f63 6861 6e67 6520 286e  height_change (n
+00012650: 756d 7079 2e6e 6461 7272 6179 293a 2041  umpy.ndarray): A
+00012660: 7272 6179 206f 6620 6865 6967 6874 2063  rray of height c
+00012670: 6861 6e67 6573 2e0d 0a20 2020 2070 6978  hanges...    pix
+00012680: 656c 5f61 7265 6120 2866 6c6f 6174 293a  el_area (float):
+00012690: 2041 7265 6120 6f66 2061 2073 696e 676c   Area of a singl
+000126a0: 6520 7069 7865 6c2e 0d0a 2020 2020 0d0a  e pixel...    ..
+000126b0: 2020 2020 5265 7475 726e 733a 0d0a 2020      Returns:..  
+000126c0: 2020 6e75 6d70 792e 6e64 6172 7261 793a    numpy.ndarray:
+000126d0: 2041 7272 6179 206f 6620 766f 6c75 6d65   Array of volume
+000126e0: 2063 6861 6e67 6573 2e0d 0a20 2020 2022   changes...    "
+000126f0: 2222 0d0a 2020 2020 766f 6c75 6d65 5f63  ""..    volume_c
+00012700: 6861 6e67 6520 3d20 6865 6967 6874 5f63  hange = height_c
+00012710: 6861 6e67 6520 2a20 7069 7865 6c5f 6172  hange * pixel_ar
+00012720: 6561 0d0a 2020 2020 7072 696e 7420 2866  ea..    print (f
+00012730: 2754 6f74 616c 2056 6f6c 756d 653a 207b  'Total Volume: {
+00012740: 6e70 2e6e 616e 7375 6d28 766f 6c75 6d65  np.nansum(volume
+00012750: 5f63 6861 6e67 6529 7d20 6375 6269 6320  _change)} cubic 
+00012760: 6d65 7465 7227 290d 0a20 2020 2072 6574  meter')..    ret
+00012770: 7572 6e20 766f 6c75 6d65 5f63 6861 6e67  urn volume_chang
+00012780: 650d 0a0d 0a66 726f 6d20 736b 696d 6167  e....from skimag
+00012790: 652e 6669 6c74 6572 7320 696d 706f 7274  e.filters import
+000127a0: 2067 6175 7373 6961 6e0d 0a0d 0a64 6566   gaussian....def
+000127b0: 2064 6973 706c 6163 656d 656e 745f 746f   displacement_to
+000127c0: 5f76 6f6c 756d 6528 6465 6d5f 7061 7468  _volume(dem_path
+000127d0: 3d22 222c 2061 7370 6563 745f 7061 7468  ="", aspect_path
+000127e0: 3d22 222c 2064 6973 706c 6163 656d 656e  ="", displacemen
+000127f0: 745f 7061 7468 3d22 222c 2073 6c6f 7065  t_path="", slope
+00012800: 5f6f 7574 7075 745f 7061 7468 3d22 222c  _output_path="",
+00012810: 2068 6569 6768 745f 6f75 7470 7574 5f70   height_output_p
+00012820: 6174 683d 2222 2c20 766f 6c75 6d65 5f6f  ath="", volume_o
+00012830: 7574 7075 745f 7061 7468 3d22 222c 2064  utput_path="", d
+00012840: 783d 4e6f 6e65 202c 2064 793d 4e6f 6e65  x=None , dy=None
+00012850: 202c 2070 6978 656c 5f61 7265 613d 4e6f   , pixel_area=No
+00012860: 6e65 293a 0d0a 2020 2020 2222 220d 0a20  ne):..    """.. 
+00012870: 2020 2050 726f 6365 7373 2074 6865 2044     Process the D
+00012880: 454d 2c20 6173 7065 6374 2c20 616e 6420  EM, aspect, and 
+00012890: 6469 7370 6c61 6365 6d65 6e74 2072 6173  displacement ras
+000128a0: 7465 7273 2074 6f20 6361 6c63 756c 6174  ters to calculat
+000128b0: 6520 616e 6420 6578 706f 7274 2074 6865  e and export the
+000128c0: 2073 6c6f 7065 2c20 6865 6967 6874 2063   slope, height c
+000128d0: 6861 6e67 652c 2061 6e64 2076 6f6c 756d  hange, and volum
+000128e0: 6520 6368 616e 6765 2e0d 0a0d 0a20 2020  e change.....   
+000128f0: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
+00012900: 2020 6465 6d5f 7061 7468 2028 7374 7229    dem_path (str)
+00012910: 3a20 5061 7468 2074 6f20 7468 6520 4445  : Path to the DE
+00012920: 4d20 7261 7374 6572 2066 696c 652e 0d0a  M raster file...
+00012930: 2020 2020 6173 7065 6374 5f70 6174 6820      aspect_path 
+00012940: 2873 7472 293a 2050 6174 6820 746f 2074  (str): Path to t
+00012950: 6865 2061 7370 6563 7420 7261 7374 6572  he aspect raster
+00012960: 2066 696c 652e 0d0a 2020 2020 6469 7370   file...    disp
+00012970: 6c61 6365 6d65 6e74 5f70 6174 6820 2873  lacement_path (s
+00012980: 7472 293a 2050 6174 6820 746f 2074 6865  tr): Path to the
+00012990: 2064 6973 706c 6163 656d 656e 7420 7261   displacement ra
+000129a0: 7374 6572 2066 696c 652e 0d0a 2020 2020  ster file...    
+000129b0: 736c 6f70 655f 6f75 7470 7574 5f70 6174  slope_output_pat
+000129c0: 6820 2873 7472 293a 2050 6174 6820 666f  h (str): Path fo
+000129d0: 7220 7468 6520 736c 6f70 6520 6f75 7470  r the slope outp
+000129e0: 7574 2047 656f 5449 4646 2066 696c 652e  ut GeoTIFF file.
+000129f0: 0d0a 2020 2020 6865 6967 6874 5f6f 7574  ..    height_out
+00012a00: 7075 745f 7061 7468 2028 7374 7229 3a20  put_path (str): 
+00012a10: 5061 7468 2066 6f72 2074 6865 2068 6569  Path for the hei
+00012a20: 6768 7420 6368 616e 6765 206f 7574 7075  ght change outpu
+00012a30: 7420 4765 6f54 4946 4620 6669 6c65 2e0d  t GeoTIFF file..
+00012a40: 0a20 2020 2076 6f6c 756d 655f 6f75 7470  .    volume_outp
+00012a50: 7574 5f70 6174 6820 2873 7472 293a 2050  ut_path (str): P
+00012a60: 6174 6820 666f 7220 7468 6520 766f 6c75  ath for the volu
+00012a70: 6d65 2063 6861 6e67 6520 6f75 7470 7574  me change output
+00012a80: 2047 656f 5449 4646 2066 696c 652e 0d0a   GeoTIFF file...
+00012a90: 2020 2020 6478 2028 666c 6f61 7429 3a20      dx (float): 
+00012aa0: 2078 2053 7061 7469 616c 2072 6573 6f6c   x Spatial resol
+00012ab0: 7574 696f 6e20 6f66 2074 6865 2072 6173  ution of the ras
+00012ac0: 7465 7220 2864 6973 7461 6e63 6520 6265  ter (distance be
+00012ad0: 7477 6565 6e20 7069 7865 6c73 292e 0d0a  tween pixels)...
+00012ae0: 2020 2020 6479 2028 666c 6f61 7429 3a20      dy (float): 
+00012af0: 2079 2053 7061 7469 616c 2072 6573 6f6c   y Spatial resol
+00012b00: 7574 696f 6e20 6f66 2074 6865 2072 6173  ution of the ras
+00012b10: 7465 7220 2864 6973 7461 6e63 6520 6265  ter (distance be
+00012b20: 7477 6565 6e20 7069 7865 6c73 292e 0d0a  tween pixels)...
+00012b30: 2020 2020 7069 7865 6c5f 6172 6561 2028      pixel_area (
+00012b40: 666c 6f61 7429 3a20 4172 6561 206f 6620  float): Area of 
+00012b50: 6120 7369 6e67 6c65 2070 6978 656c 2e0d  a single pixel..
+00012b60: 0a0d 0a20 2020 2052 6574 7572 6e73 3a0d  ...    Returns:.
+00012b70: 0a20 2020 204e 6f6e 653a 204f 7574 7075  .    None: Outpu
+00012b80: 7473 2047 656f 5449 4646 2066 696c 6573  ts GeoTIFF files
+00012b90: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
+00012ba0: 6420 6f75 7470 7574 2070 6174 6873 2e0d  d output paths..
+00012bb0: 0a20 2020 2022 2222 0d0a 2020 2020 7769  .    """..    wi
+00012bc0: 7468 2072 6173 7465 7269 6f2e 6f70 656e  th rasterio.open
+00012bd0: 2864 656d 5f70 6174 6829 2061 7320 6465  (dem_path) as de
+00012be0: 6d5f 7261 7374 6572 2c20 5c0d 0a20 2020  m_raster, \..   
+00012bf0: 2020 2020 2020 7261 7374 6572 696f 2e6f        rasterio.o
+00012c00: 7065 6e28 6173 7065 6374 5f70 6174 6829  pen(aspect_path)
+00012c10: 2061 7320 6173 7065 6374 5f72 6173 7465   as aspect_raste
+00012c20: 722c 205c 0d0a 2020 2020 2020 2020 2072  r, \..         r
+00012c30: 6173 7465 7269 6f2e 6f70 656e 2864 6973  asterio.open(dis
+00012c40: 706c 6163 656d 656e 745f 7061 7468 2920  placement_path) 
+00012c50: 6173 2064 6973 706c 6163 656d 656e 745f  as displacement_
+00012c60: 7261 7374 6572 3a0d 0a0d 0a20 2020 2020  raster:....     
+00012c70: 2020 2064 656d 203d 2064 656d 5f72 6173     dem = dem_ras
+00012c80: 7465 722e 7265 6164 2831 2c20 206d 6173  ter.read(1,  mas
+00012c90: 6b65 643d 5472 7565 290d 0a20 2020 2020  ked=True)..     
+00012ca0: 2020 2061 7370 6563 7420 3d20 6173 7065     aspect = aspe
+00012cb0: 6374 5f72 6173 7465 722e 7265 6164 2831  ct_raster.read(1
+00012cc0: 2c20 206d 6173 6b65 643d 5472 7565 290d  ,  masked=True).
+00012cd0: 0a20 2020 2020 2020 2064 6973 706c 6163  .        displac
+00012ce0: 656d 656e 7420 3d20 6469 7370 6c61 6365  ement = displace
+00012cf0: 6d65 6e74 5f72 6173 7465 722e 7265 6164  ment_raster.read
+00012d00: 2831 2c20 206d 6173 6b65 643d 5472 7565  (1,  masked=True
+00012d10: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00012d20: 2020 2020 2078 5f72 6573 6f6c 7574 696f       x_resolutio
+00012d30: 6e2c 2079 5f72 6573 6f6c 7574 696f 6e20  n, y_resolution 
+00012d40: 3d20 6469 7370 6c61 6365 6d65 6e74 5f72  = displacement_r
+00012d50: 6173 7465 722e 7265 730d 0a20 2020 2020  aster.res..     
+00012d60: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+00012d70: 6478 2069 7320 4e6f 6e65 3a0d 0a20 2020  dx is None:..   
+00012d80: 2020 2020 2020 2020 2064 783d 785f 7265           dx=x_re
+00012d90: 736f 6c75 7469 6f6e 0d0a 2020 2020 2020  solution..      
+00012da0: 2020 6966 2064 7920 6973 204e 6f6e 653a    if dy is None:
+00012db0: 0d0a 2020 2020 2020 2020 2020 2020 6479  ..            dy
+00012dc0: 3d79 5f72 6573 6f6c 7574 696f 6e0d 0a20  =y_resolution.. 
+00012dd0: 2020 2020 2020 2069 6620 7069 7865 6c5f         if pixel_
+00012de0: 6172 6561 2069 7320 4e6f 6e65 3a0d 0a20  area is None:.. 
+00012df0: 2020 2020 2020 2020 2020 2070 6978 656c             pixel
+00012e00: 5f61 7265 613d 6478 202a 2064 790d 0a20  _area=dx * dy.. 
+00012e10: 2020 2020 2020 2066 726f 6d20 7363 6970         from scip
+00012e20: 792e 6e64 696d 6167 6520 696d 706f 7274  y.ndimage import
+00012e30: 207a 6f6f 6d0d 0a0d 0a20 2020 2020 2020   zoom....       
+00012e40: 2023 2045 7861 6d70 6c65 2064 696d 656e   # Example dimen
+00012e50: 7369 6f6e 7320 2d20 7265 706c 6163 6520  sions - replace 
+00012e60: 7468 6573 6520 7769 7468 2061 6374 7561  these with actua
+00012e70: 6c20 6469 6d65 6e73 696f 6e73 0d0a 2020  l dimensions..  
+00012e80: 2020 2020 2020 6465 6d5f 7368 6170 6520        dem_shape 
+00012e90: 3d20 6465 6d2e 7368 6170 650d 0a20 2020  = dem.shape..   
+00012ea0: 2020 2020 2061 7370 6563 745f 7368 6170       aspect_shap
+00012eb0: 6520 3d20 6173 7065 6374 2e73 6861 7065  e = aspect.shape
+00012ec0: 0d0a 2020 2020 2020 2020 6469 7370 6c61  ..        displa
+00012ed0: 6365 6d65 6e74 5f73 6861 7065 203d 2064  cement_shape = d
+00012ee0: 6973 706c 6163 656d 656e 742e 7368 6170  isplacement.shap
+00012ef0: 650d 0a0d 0a20 2020 2020 2020 2023 2043  e....        # C
+00012f00: 616c 6375 6c61 7469 6e67 207a 6f6f 6d20  alculating zoom 
+00012f10: 6661 6374 6f72 730d 0a20 2020 2020 2020  factors..       
+00012f20: 207a 6f6f 6d5f 6661 6374 6f72 5f61 7370   zoom_factor_asp
+00012f30: 6563 7420 3d20 5b64 656d 5f64 696d 202f  ect = [dem_dim /
+00012f40: 2061 7370 6563 745f 6469 6d20 666f 7220   aspect_dim for 
+00012f50: 6465 6d5f 6469 6d2c 2061 7370 6563 745f  dem_dim, aspect_
+00012f60: 6469 6d20 696e 207a 6970 2864 656d 5f73  dim in zip(dem_s
+00012f70: 6861 7065 2c20 6173 7065 6374 5f73 6861  hape, aspect_sha
+00012f80: 7065 295d 0d0a 2020 2020 2020 2020 7a6f  pe)]..        zo
+00012f90: 6f6d 5f66 6163 746f 725f 6469 7370 6c61  om_factor_displa
+00012fa0: 6365 6d65 6e74 203d 205b 6465 6d5f 6469  cement = [dem_di
+00012fb0: 6d20 2f20 6469 7370 6c61 6365 6d65 6e74  m / displacement
+00012fc0: 5f64 696d 2066 6f72 2064 656d 5f64 696d  _dim for dem_dim
+00012fd0: 2c20 6469 7370 6c61 6365 6d65 6e74 5f64  , displacement_d
+00012fe0: 696d 2069 6e20 7a69 7028 6465 6d5f 7368  im in zip(dem_sh
+00012ff0: 6170 652c 2064 6973 706c 6163 656d 656e  ape, displacemen
+00013000: 745f 7368 6170 6529 5d0d 0a0d 0a20 2020  t_shape)]....   
+00013010: 2020 2020 2023 2052 6573 697a 696e 6720       # Resizing 
+00013020: 6173 7065 6374 2061 6e64 2064 6973 706c  aspect and displ
+00013030: 6163 656d 656e 7420 6172 7261 7973 0d0a  acement arrays..
+00013040: 2020 2020 2020 2020 6173 7065 6374 203d          aspect =
+00013050: 207a 6f6f 6d28 6173 7065 6374 2c20 7a6f   zoom(aspect, zo
+00013060: 6f6d 5f66 6163 746f 725f 6173 7065 6374  om_factor_aspect
+00013070: 2c20 6f72 6465 723d 3129 2020 2320 6375  , order=1)  # cu
+00013080: 6269 6320 696e 7465 7270 6f6c 6174 696f  bic interpolatio
+00013090: 6e0d 0a20 2020 2020 2020 2064 6973 706c  n..        displ
+000130a0: 6163 656d 656e 7420 3d20 7a6f 6f6d 2864  acement = zoom(d
+000130b0: 6973 706c 6163 656d 656e 742c 207a 6f6f  isplacement, zoo
+000130c0: 6d5f 6661 6374 6f72 5f64 6973 706c 6163  m_factor_displac
+000130d0: 656d 656e 742c 206f 7264 6572 3d31 2920  ement, order=1) 
+000130e0: 2023 2063 7562 6963 2069 6e74 6572 706f   # cubic interpo
+000130f0: 6c61 7469 6f6e 0d0a 2020 2020 2020 2020  lation..        
+00013100: 0d0a 2020 2020 2020 2020 2320 6173 7065  ..        # aspe
+00013110: 6374 203d 206e 702e 7265 7369 7a65 2861  ct = np.resize(a
+00013120: 7370 6563 742c 2064 656d 2e73 6861 7065  spect, dem.shape
+00013130: 290d 0a20 2020 2020 2020 2023 2064 6973  )..        # dis
+00013140: 706c 6163 656d 656e 7420 3d20 6e70 2e72  placement = np.r
+00013150: 6573 697a 6528 6469 7370 6c61 6365 6d65  esize(displaceme
+00013160: 6e74 2c20 6465 6d2e 7368 6170 6529 0d0a  nt, dem.shape)..
+00013170: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00013180: 2020 736c 6f70 652c 2064 6972 6563 7469    slope, directi
+00013190: 6f6e 616c 5f67 7261 6420 3d20 6361 6c63  onal_grad = calc
+000131a0: 756c 6174 655f 736c 6f70 6528 6465 6d2c  ulate_slope(dem,
+000131b0: 2061 7370 6563 742c 2064 7820 2c20 6479   aspect, dx , dy
+000131c0: 2029 0d0a 2020 2020 2020 2020 6865 6967   )..        heig
+000131d0: 6874 5f63 6861 6e67 6520 203d 2063 616c  ht_change  = cal
+000131e0: 6375 6c61 7465 5f68 6569 6768 745f 6368  culate_height_ch
+000131f0: 616e 6765 2873 6c6f 7065 2c20 6469 7265  ange(slope, dire
+00013200: 6374 696f 6e61 6c5f 6772 6164 2c20 6465  ctional_grad, de
+00013210: 6d29 0d0a 2020 2020 2020 2020 2368 6569  m)..        #hei
+00013220: 6768 745f 6368 616e 6765 3d67 6175 7373  ght_change=gauss
+00013230: 6961 6e28 6865 6967 6874 5f63 6861 6e67  ian(height_chang
+00013240: 652c 2073 6967 6d61 3d33 290d 0a20 2020  e, sigma=3)..   
+00013250: 2020 2020 2076 6f6c 756d 655f 6368 616e       volume_chan
+00013260: 6765 203d 2063 616c 6375 6c61 7465 5f76  ge = calculate_v
+00013270: 6f6c 756d 655f 6368 616e 6765 2868 6569  olume_change(hei
+00013280: 6768 745f 6368 616e 6765 2c20 7069 7865  ght_change, pixe
+00013290: 6c5f 6172 6561 290d 0a20 2020 2020 2020  l_area)..       
+000132a0: 0d0a 2020 2020 2020 200d 0a0d 0a20 2020  ..       ....   
+000132b0: 2020 2020 2023 2044 6566 696e 6520 6120       # Define a 
+000132c0: 6675 6e63 7469 6f6e 2074 6f20 6578 706f  function to expo
+000132d0: 7274 2064 6174 6120 746f 2061 2047 656f  rt data to a Geo
+000132e0: 5449 4646 0d0a 2020 2020 2020 2020 6465  TIFF..        de
+000132f0: 6620 6578 706f 7274 5f74 6f5f 6765 6f74  f export_to_geot
+00013300: 6966 6628 6461 7461 2c20 6f75 7470 7574  iff(data, output
+00013310: 5f70 6174 682c 2072 6566 6572 656e 6365  _path, reference
+00013320: 5f72 6173 7465 7229 3a0d 0a20 2020 2020  _raster):..     
+00013330: 2020 2020 2020 2077 6974 6820 7261 7374         with rast
+00013340: 6572 696f 2e6f 7065 6e28 0d0a 2020 2020  erio.open(..    
+00013350: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00013360: 7574 5f70 6174 682c 2027 7727 2c0d 0a20  ut_path, 'w',.. 
+00013370: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00013380: 7269 7665 723d 2747 5469 6666 272c 0d0a  river='GTiff',..
+00013390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133a0: 6865 6967 6874 3d64 6174 612e 7368 6170  height=data.shap
+000133b0: 655b 305d 2c0d 0a20 2020 2020 2020 2020  e[0],..         
+000133c0: 2020 2020 2020 2077 6964 7468 3d64 6174         width=dat
+000133d0: 612e 7368 6170 655b 315d 2c0d 0a20 2020  a.shape[1],..   
+000133e0: 2020 2020 2020 2020 2020 2020 2063 6f75               cou
+000133f0: 6e74 3d31 2c0d 0a20 2020 2020 2020 2020  nt=1,..         
+00013400: 2020 2020 2020 2064 7479 7065 3d6e 702e         dtype=np.
+00013410: 666c 6f61 7433 322c 0d0a 2020 2020 2020  float32,..      
+00013420: 2020 2020 2020 2020 2020 6372 733d 7265            crs=re
+00013430: 6665 7265 6e63 655f 7261 7374 6572 2e63  ference_raster.c
+00013440: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+00013450: 2020 2020 2074 7261 6e73 666f 726d 3d72       transform=r
+00013460: 6566 6572 656e 6365 5f72 6173 7465 722e  eference_raster.
+00013470: 7472 616e 7366 6f72 6d2c 206e 6f64 6174  transform, nodat
+00013480: 613d 6e70 2e6e 616e 0d0a 2020 2020 2020  a=np.nan..      
+00013490: 2020 2020 2020 2920 6173 206f 7574 7075        ) as outpu
+000134a0: 745f 7261 7374 6572 3a0d 0a20 2020 2020  t_raster:..     
+000134b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+000134c0: 745f 7261 7374 6572 2e77 7269 7465 2864  t_raster.write(d
+000134d0: 6174 612c 2031 290d 0a0d 0a20 2020 2020  ata, 1)....     
+000134e0: 2020 2023 2045 7870 6f72 7469 6e67 2073     # Exporting s
+000134f0: 6c6f 7065 2c20 6865 6967 6874 2063 6861  lope, height cha
+00013500: 6e67 652c 2061 6e64 2076 6f6c 756d 6520  nge, and volume 
+00013510: 6368 616e 6765 2074 6f20 4765 6f54 4946  change to GeoTIF
+00013520: 4673 0d0a 2020 2020 2020 2020 6578 706f  Fs..        expo
+00013530: 7274 5f74 6f5f 6765 6f74 6966 6628 736c  rt_to_geotiff(sl
+00013540: 6f70 652c 2073 6c6f 7065 5f6f 7574 7075  ope, slope_outpu
+00013550: 745f 7061 7468 2c20 6465 6d5f 7261 7374  t_path, dem_rast
+00013560: 6572 290d 0a20 2020 2020 2020 2065 7870  er)..        exp
+00013570: 6f72 745f 746f 5f67 656f 7469 6666 2868  ort_to_geotiff(h
+00013580: 6569 6768 745f 6368 616e 6765 2c20 6865  eight_change, he
+00013590: 6967 6874 5f6f 7574 7075 745f 7061 7468  ight_output_path
+000135a0: 2c20 6465 6d5f 7261 7374 6572 290d 0a20  , dem_raster).. 
+000135b0: 2020 2020 2020 2065 7870 6f72 745f 746f         export_to
+000135c0: 5f67 656f 7469 6666 2876 6f6c 756d 655f  _geotiff(volume_
+000135d0: 6368 616e 6765 2c20 766f 6c75 6d65 5f6f  change, volume_o
+000135e0: 7574 7075 745f 7061 7468 2c20 6465 6d5f  utput_path, dem_
+000135f0: 7261 7374 6572 290d 0a20 2020 2020 2020  raster)..       
+00013600: 0d0a 0d0a 0d0a 0d0a 696d 706f 7274 206e  ........import n
+00013610: 756d 7079 2061 7320 6e70 0d0a 6672 6f6d  umpy as np..from
+00013620: 206f 7367 656f 2069 6d70 6f72 7420 6764   osgeo import gd
+00013630: 616c 0d0a 0d0a 6465 6620 6361 6c63 756c  al....def calcul
+00013640: 6174 655f 616e 645f 7361 7665 5f61 7370  ate_and_save_asp
+00013650: 6563 745f 7261 7374 6572 2865 775f 7261  ect_raster(ew_ra
+00013660: 7374 6572 5f70 6174 683a 2073 7472 203d  ster_path: str =
+00013670: 2222 2c20 6e73 5f72 6173 7465 725f 7061  "", ns_raster_pa
+00013680: 7468 3a20 7374 7220 3d22 222c 206f 7574  th: str ="", out
+00013690: 7075 745f 7261 7374 6572 5f70 6174 683a  put_raster_path:
+000136a0: 2073 7472 203d 2222 293a 0d0a 2020 2020   str =""):..    
+000136b0: 2222 220d 0a20 2020 2043 616c 6375 6c61  """..    Calcula
+000136c0: 7465 2074 6865 2061 7370 6563 7420 7261  te the aspect ra
+000136d0: 7374 6572 2066 726f 6d20 6561 7374 2d77  ster from east-w
+000136e0: 6573 7420 616e 6420 6e6f 7274 682d 736f  est and north-so
+000136f0: 7574 6820 6469 7370 6c61 6365 6d65 6e74  uth displacement
+00013700: 2072 6173 7465 7273 2061 6e64 2073 6176   rasters and sav
+00013710: 6520 6974 2e0d 0a0d 0a20 2020 2054 6869  e it.....    Thi
+00013720: 7320 6675 6e63 7469 6f6e 2072 6561 6473  s function reads
+00013730: 2074 776f 2072 6173 7465 7220 6669 6c65   two raster file
+00013740: 7320 7265 7072 6573 656e 7469 6e67 2065  s representing e
+00013750: 6173 742d 7765 7374 2028 4557 2920 616e  ast-west (EW) an
+00013760: 6420 6e6f 7274 682d 736f 7574 6820 284e  d north-south (N
+00013770: 5329 200d 0a20 2020 2064 6973 706c 6163  S) ..    displac
+00013780: 656d 656e 7473 2c20 6361 6c63 756c 6174  ements, calculat
+00013790: 6573 2074 6865 2061 7370 6563 7420 6f66  es the aspect of
+000137a0: 2065 6163 6820 7069 7865 6c2c 2061 6e64   each pixel, and
+000137b0: 2073 6176 6573 2074 6865 2072 6573 756c   saves the resul
+000137c0: 7420 6173 2061 206e 6577 2072 6173 7465  t as a new raste
+000137d0: 7220 6669 6c65 2e0d 0a20 2020 2041 7370  r file...    Asp
+000137e0: 6563 7420 6973 2063 616c 6375 6c61 7465  ect is calculate
+000137f0: 6420 696e 2064 6567 7265 6573 2066 726f  d in degrees fro
+00013800: 6d20 6e6f 7274 6820 2830 2064 6567 7265  m north (0 degre
+00013810: 6573 292c 2065 6173 7420 2839 3020 6465  es), east (90 de
+00013820: 6772 6565 7329 2c20 736f 7574 6820 2831  grees), south (1
+00013830: 3830 2064 6567 7265 6573 292c 0d0a 2020  80 degrees),..  
+00013840: 2020 616e 6420 7765 7374 2028 3237 3020    and west (270 
+00013850: 6465 6772 6565 7329 2e0d 0a0d 0a20 2020  degrees).....   
+00013860: 2050 6172 616d 6574 6572 733a 0d0a 2020   Parameters:..  
+00013870: 2020 2d20 6577 5f72 6173 7465 725f 7061    - ew_raster_pa
+00013880: 7468 2028 7374 7229 3a20 4669 6c65 2070  th (str): File p
+00013890: 6174 6820 666f 7220 7468 6520 6561 7374  ath for the east
+000138a0: 2d77 6573 7420 6469 7370 6c61 6365 6d65  -west displaceme
+000138b0: 6e74 2072 6173 7465 722e 0d0a 2020 2020  nt raster...    
+000138c0: 2d20 6e73 5f72 6173 7465 725f 7061 7468  - ns_raster_path
+000138d0: 2028 7374 7229 3a20 4669 6c65 2070 6174   (str): File pat
+000138e0: 6820 666f 7220 7468 6520 6e6f 7274 682d  h for the north-
+000138f0: 736f 7574 6820 6469 7370 6c61 6365 6d65  south displaceme
+00013900: 6e74 2072 6173 7465 722e 0d0a 2020 2020  nt raster...    
+00013910: 2d20 6f75 7470 7574 5f72 6173 7465 725f  - output_raster_
+00013920: 7061 7468 2028 7374 7229 3a20 4669 6c65  path (str): File
+00013930: 2070 6174 6820 666f 7220 7468 6520 6f75   path for the ou
+00013940: 7470 7574 2061 7370 6563 7420 7261 7374  tput aspect rast
+00013950: 6572 2e0d 0a0d 0a20 2020 2052 6574 7572  er.....    Retur
+00013960: 6e73 3a0d 0a20 2020 204e 6f6e 652e 2054  ns:..    None. T
+00013970: 6865 2072 6573 756c 7420 6973 2073 6176  he result is sav
+00013980: 6564 2061 7320 6120 6e65 7720 7261 7374  ed as a new rast
+00013990: 6572 2066 696c 6520 6174 2074 6865 2073  er file at the s
+000139a0: 7065 6369 6669 6564 206f 7574 7075 7420  pecified output 
+000139b0: 7061 7468 2e0d 0a20 2020 200d 0a20 2020  path...    ..   
+000139c0: 2022 2222 0d0a 2020 2020 6465 6620 7265   """..    def re
+000139d0: 6164 5f72 6173 7465 7228 6669 6c65 5f70  ad_raster(file_p
+000139e0: 6174 6829 3a0d 0a20 2020 2020 2020 2022  ath):..        "
+000139f0: 2222 5265 6164 2061 2072 6173 7465 7220  ""Read a raster 
+00013a00: 6669 6c65 2061 6e64 2072 6574 7572 6e20  file and return 
+00013a10: 7468 6520 6461 7461 2061 7272 6179 2061  the data array a
+00013a20: 6e64 2067 656f 7472 616e 7366 6f72 6d2e  nd geotransform.
+00013a30: 2222 220d 0a0d 0a20 2020 2020 2020 2023  """....        #
+00013a40: 204f 7065 6e20 7468 6520 6461 7461 7365   Open the datase
+00013a50: 740d 0a20 2020 2020 2020 2064 6174 6173  t..        datas
+00013a60: 6574 203d 2067 6461 6c2e 4f70 656e 2866  et = gdal.Open(f
+00013a70: 696c 655f 7061 7468 290d 0a20 2020 2020  ile_path)..     
+00013a80: 2020 2069 6620 6461 7461 7365 7420 6973     if dataset is
+00013a90: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00013aa0: 2020 2020 7261 6973 6520 494f 4572 726f      raise IOErro
+00013ab0: 7228 2243 6f75 6c64 206e 6f74 206f 7065  r("Could not ope
+00013ac0: 6e20 6669 6c65 2061 7420 7b7d 222e 666f  n file at {}".fo
+00013ad0: 726d 6174 2866 696c 655f 7061 7468 2929  rmat(file_path))
+00013ae0: 0d0a 0d0a 2020 2020 2020 2020 2320 4765  ....        # Ge
+00013af0: 7420 7468 6520 6669 7273 7420 7261 7374  t the first rast
+00013b00: 6572 2062 616e 640d 0a20 2020 2020 2020  er band..       
+00013b10: 2062 616e 6420 3d20 6461 7461 7365 742e   band = dataset.
+00013b20: 4765 7452 6173 7465 7242 616e 6428 3129  GetRasterBand(1)
+00013b30: 0d0a 0d0a 2020 2020 2020 2020 2320 5265  ....        # Re
+00013b40: 6164 2074 6865 2064 6174 6120 6173 2061  ad the data as a
+00013b50: 206e 756d 7079 2061 7272 6179 0d0a 2020   numpy array..  
+00013b60: 2020 2020 2020 6461 7461 203d 2062 616e        data = ban
+00013b70: 642e 5265 6164 4173 4172 7261 7928 290d  d.ReadAsArray().
+00013b80: 0a0d 0a20 2020 2020 2020 2023 2047 6574  ...        # Get
+00013b90: 206e 6f2d 6461 7461 2076 616c 7565 2066   no-data value f
+00013ba0: 726f 6d20 7468 6520 6261 6e64 0d0a 2020  rom the band..  
+00013bb0: 2020 2020 2020 6e6f 6461 7461 5f76 616c        nodata_val
+00013bc0: 7565 203d 2062 616e 642e 4765 744e 6f44  ue = band.GetNoD
+00013bd0: 6174 6156 616c 7565 2829 0d0a 0d0a 2020  ataValue()....  
+00013be0: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
+00013bf0: 2074 6865 7265 2069 7320 6120 6e6f 2d64   there is a no-d
+00013c00: 6174 6120 7661 6c75 6520 6465 6669 6e65  ata value define
+00013c10: 640d 0a20 2020 2020 2020 2069 6620 6e6f  d..        if no
+00013c20: 6461 7461 5f76 616c 7565 2069 7320 6e6f  data_value is no
+00013c30: 7420 4e6f 6e65 3a0d 0a20 2020 2020 2020  t None:..       
+00013c40: 2020 2020 2023 2043 7265 6174 6520 6120       # Create a 
+00013c50: 6d61 736b 2074 6861 7420 6973 2054 7275  mask that is Tru
+00013c60: 6520 666f 7220 7661 6c69 6420 7069 7865  e for valid pixe
+00013c70: 6c73 0d0a 2020 2020 2020 2020 2020 2020  ls..            
+00013c80: 6d61 736b 203d 2064 6174 6120 213d 206e  mask = data != n
+00013c90: 6f64 6174 615f 7661 6c75 650d 0a0d 0a20  odata_value.... 
+00013ca0: 2020 2020 2020 2020 2020 2023 2041 7070             # App
+00013cb0: 6c79 2074 6865 206d 6173 6b20 746f 2066  ly the mask to f
+00013cc0: 696c 7465 7220 6f75 7420 6e6f 2d64 6174  ilter out no-dat
+00013cd0: 6120 7069 7865 6c73 0d0a 2020 2020 2020  a pixels..      
+00013ce0: 2020 2020 2020 7661 6c69 645f 6461 7461        valid_data
+00013cf0: 203d 206e 702e 7768 6572 6528 6d61 736b   = np.where(mask
+00013d00: 2c20 6461 7461 2c20 6e70 2e6e 616e 2920  , data, np.nan) 
+00013d10: 2023 2052 6570 6c61 6365 206e 6f2d 6461   # Replace no-da
+00013d20: 7461 2077 6974 6820 4e61 4e0d 0a20 2020  ta with NaN..   
+00013d30: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00013d40: 2020 2020 2020 2020 7661 6c69 645f 6461          valid_da
+00013d50: 7461 203d 2064 6174 6120 2023 2041 6c6c  ta = data  # All
+00013d60: 2064 6174 6120 6973 2076 616c 6964 2069   data is valid i
+00013d70: 6620 7468 6572 6520 6973 206e 6f20 6e6f  f there is no no
+00013d80: 2d64 6174 6120 7661 6c75 650d 0a0d 0a20  -data value.... 
+00013d90: 2020 2020 2020 2023 2052 6574 7269 6576         # Retriev
+00013da0: 6520 6765 6f74 7261 6e73 666f 726d 6174  e geotransformat
+00013db0: 696f 6e0d 0a20 2020 2020 2020 2067 656f  ion..        geo
+00013dc0: 7472 616e 7366 6f72 6d20 3d20 6461 7461  transform = data
+00013dd0: 7365 742e 4765 7447 656f 5472 616e 7366  set.GetGeoTransf
+00013de0: 6f72 6d28 290d 0a0d 0a20 2020 2020 2020  orm()....       
+00013df0: 2023 2043 6c6f 7365 2074 6865 2064 6174   # Close the dat
+00013e00: 6173 6574 0d0a 2020 2020 2020 2020 2364  aset..        #d
+00013e10: 6174 6173 6574 203d 204e 6f6e 650d 0a0d  ataset = None...
+00013e20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013e30: 7661 6c69 645f 6461 7461 2c20 6765 6f74  valid_data, geot
+00013e40: 7261 6e73 666f 726d 2c20 6461 7461 7365  ransform, datase
+00013e50: 740d 0a0d 0a20 2020 2064 6566 2063 616c  t....    def cal
+00013e60: 6375 6c61 7465 5f61 7370 6563 7428 6577  culate_aspect(ew
+00013e70: 5f64 6174 612c 206e 735f 6461 7461 293a  _data, ns_data):
+00013e80: 0d0a 2020 2020 2020 2020 2222 2243 616c  ..        """Cal
+00013e90: 6375 6c61 7465 2074 6865 2061 7370 6563  culate the aspec
+00013ea0: 7420 6672 6f6d 2045 5720 616e 6420 4e53  t from EW and NS
+00013eb0: 2064 6973 706c 6163 656d 656e 7420 6461   displacement da
+00013ec0: 7461 2e22 2222 0d0a 2020 2020 2020 2020  ta."""..        
+00013ed0: 7769 7468 206e 702e 6572 7273 7461 7465  with np.errstate
+00013ee0: 2864 6976 6964 653d 2769 676e 6f72 6527  (divide='ignore'
+00013ef0: 2c20 696e 7661 6c69 643d 2769 676e 6f72  , invalid='ignor
+00013f00: 6527 293a 0d0a 2020 2020 2020 2020 2020  e'):..          
+00013f10: 2020 6173 7065 6374 203d 206e 702e 6172    aspect = np.ar
+00013f20: 6374 616e 3228 6577 5f64 6174 612c 206e  ctan2(ew_data, n
+00013f30: 735f 6461 7461 290d 0a20 2020 2020 2020  s_data)..       
+00013f40: 2020 2020 2061 7370 6563 745f 6465 673d       aspect_deg=
+00013f50: 6e70 2e64 6567 7265 6573 2861 7370 6563  np.degrees(aspec
+00013f60: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00013f70: 6173 7065 6374 5f64 6567 203d 2028 3435  aspect_deg = (45
+00013f80: 3020 2d61 7370 6563 745f 6465 6720 2920  0 -aspect_deg ) 
+00013f90: 2520 3336 300d 0a20 2020 2020 2020 2072  % 360..        r
+00013fa0: 6574 7572 6e20 6173 7065 6374 5f64 6567  eturn aspect_deg
+00013fb0: 0d0a 0d0a 2020 2020 6465 6620 7361 7665  ....    def save
+00013fc0: 5f72 6173 7465 7228 6f75 7470 7574 5f70  _raster(output_p
+00013fd0: 6174 682c 2064 6174 612c 2067 656f 5f74  ath, data, geo_t
+00013fe0: 7261 6e73 666f 726d 2c20 7265 6665 7265  ransform, refere
+00013ff0: 6e63 655f 6461 7461 7365 7429 3a0d 0a20  nce_dataset):.. 
+00014000: 2020 2020 2020 2022 2222 5361 7665 2074         """Save t
+00014010: 6865 2064 6174 6120 6173 2061 2072 6173  he data as a ras
+00014020: 7465 7220 6669 6c65 2e22 2222 0d0a 2020  ter file."""..  
+00014030: 2020 2020 2020 6472 6976 6572 203d 2067        driver = g
+00014040: 6461 6c2e 4765 7444 7269 7665 7242 794e  dal.GetDriverByN
+00014050: 616d 6528 2747 5469 6666 2729 0d0a 2020  ame('GTiff')..  
+00014060: 2020 2020 2020 726f 7773 2c20 636f 6c73        rows, cols
+00014070: 203d 2064 6174 612e 7368 6170 650d 0a20   = data.shape.. 
+00014080: 2020 2020 2020 206f 7574 5f72 6173 7465         out_raste
+00014090: 7220 3d20 6472 6976 6572 2e43 7265 6174  r = driver.Creat
+000140a0: 6528 6f75 7470 7574 5f70 6174 682c 2063  e(output_path, c
+000140b0: 6f6c 732c 2072 6f77 732c 2031 2c20 6764  ols, rows, 1, gd
+000140c0: 616c 2e47 4454 5f46 6c6f 6174 3332 290d  al.GDT_Float32).
+000140d0: 0a20 2020 2020 2020 206f 7574 5f72 6173  .        out_ras
+000140e0: 7465 722e 5365 7447 656f 5472 616e 7366  ter.SetGeoTransf
+000140f0: 6f72 6d28 6765 6f5f 7472 616e 7366 6f72  orm(geo_transfor
+00014100: 6d29 0d0a 2020 2020 2020 2020 6f75 745f  m)..        out_
+00014110: 6261 6e64 203d 206f 7574 5f72 6173 7465  band = out_raste
+00014120: 722e 4765 7452 6173 7465 7242 616e 6428  r.GetRasterBand(
+00014130: 3129 0d0a 2020 2020 2020 2020 6f75 745f  1)..        out_
+00014140: 6261 6e64 2e57 7269 7465 4172 7261 7928  band.WriteArray(
+00014150: 6461 7461 290d 0a20 2020 2020 2020 206f  data)..        o
+00014160: 7574 5f72 6173 7465 722e 5365 7450 726f  ut_raster.SetPro
+00014170: 6a65 6374 696f 6e28 7265 6665 7265 6e63  jection(referenc
+00014180: 655f 6461 7461 7365 742e 4765 7450 726f  e_dataset.GetPro
+00014190: 6a65 6374 696f 6e28 2929 0d0a 2020 2020  jection())..    
+000141a0: 2020 2020 6f75 745f 6261 6e64 2e46 6c75      out_band.Flu
+000141b0: 7368 4361 6368 6528 290d 0a0d 0a20 2020  shCache()....   
+000141c0: 2023 2052 6561 6420 7468 6520 4557 2061   # Read the EW a
+000141d0: 6e64 204e 5320 7261 7374 6572 2064 6174  nd NS raster dat
+000141e0: 610d 0a20 2020 2065 775f 6461 7461 2c20  a..    ew_data, 
+000141f0: 6765 6f5f 7472 616e 7366 6f72 6d2c 2064  geo_transform, d
+00014200: 6174 6173 6574 203d 2072 6561 645f 7261  ataset = read_ra
+00014210: 7374 6572 2865 775f 7261 7374 6572 5f70  ster(ew_raster_p
+00014220: 6174 6829 0d0a 2020 2020 6e73 5f64 6174  ath)..    ns_dat
+00014230: 612c 205f 2c20 5f20 3d20 7265 6164 5f72  a, _, _ = read_r
+00014240: 6173 7465 7228 6e73 5f72 6173 7465 725f  aster(ns_raster_
+00014250: 7061 7468 290d 0a0d 0a20 2020 2023 2043  path)....    # C
+00014260: 616c 6375 6c61 7465 2074 6865 2061 7370  alculate the asp
+00014270: 6563 7420 616e 6420 7361 7665 2074 6865  ect and save the
+00014280: 2072 6573 756c 740d 0a20 2020 2061 7370   result..    asp
+00014290: 6563 745f 6461 7461 203d 2063 616c 6375  ect_data = calcu
+000142a0: 6c61 7465 5f61 7370 6563 7428 6577 5f64  late_aspect(ew_d
+000142b0: 6174 612c 206e 735f 6461 7461 290d 0a20  ata, ns_data).. 
+000142c0: 2020 2073 6176 655f 7261 7374 6572 286f     save_raster(o
+000142d0: 7574 7075 745f 7261 7374 6572 5f70 6174  utput_raster_pat
+000142e0: 682c 2061 7370 6563 745f 6461 7461 2c20  h, aspect_data, 
+000142f0: 6765 6f5f 7472 616e 7366 6f72 6d2c 2064  geo_transform, d
+00014300: 6174 6173 6574 290d 0a0d 0a23 2045 7861  ataset)....# Exa
+00014310: 6d70 6c65 2075 7361 6765 3a0d 0a23 2063  mple usage:..# c
+00014320: 616c 6375 6c61 7465 5f61 6e64 5f73 6176  alculate_and_sav
+00014330: 655f 6173 7065 6374 5f72 6173 7465 7228  e_aspect_raster(
+00014340: 2770 6174 685f 746f 5f65 775f 7261 7374  'path_to_ew_rast
+00014350: 6572 2e74 6966 272c 2027 7061 7468 5f74  er.tif', 'path_t
+00014360: 6f5f 6e73 5f72 6173 7465 722e 7469 6627  o_ns_raster.tif'
+00014370: 2c20 2770 6174 685f 746f 5f6f 7574 7075  , 'path_to_outpu
+00014380: 745f 6173 7065 6374 5f72 6173 7465 722e  t_aspect_raster.
+00014390: 7469 6627 290d 0a0d 0a0d 0a0d 0a23 2323  tif')........###
+000143a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000143b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000143c0: 2323 2323 2323 2323 2323 230d 0a0d 0a    ###########....
```

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Akhdefo_Utilities.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Akhdefo_Utilities.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Filter_PreProc.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Filter_PreProc.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Mosaic_Crop.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Mosaic_Crop.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/OpticalFlow.py` & `akhdefo_functions-2.5.4/akhdefo_functions/OpticalFlow.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Stacked_Velocity.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Stacked_Velocity.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Unzip_CopyFiles.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Unzip_CopyFiles.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/Video_Streamer.py` & `akhdefo_functions-2.5.4/akhdefo_functions/Video_Streamer.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/__init__.py` & `akhdefo_functions-2.5.4/akhdefo_functions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 akhdefo_functions
 
 collection of python modules performs geospatial image processing to moniter land deformation
 """
 
-__version__ = "2.5.3"
+__version__ = "2.5.4"
 __author__ = 'Mahmud Mustafa Muhammad: mahmud.muhamm1@gmail.com'
 __credits__ = 'Simon Fraser university-Department of Earth Sciences'
 
 
 
 
 from  .backend import*
```

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions/backend.py` & `akhdefo_functions-2.5.4/akhdefo_functions/backend.py`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions.egg-info/PKG-INFO` & `akhdefo_functions-2.5.4/akhdefo_functions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akhdefo-functions
-Version: 2.5.3
+Version: 2.5.4
 Summary: Land Deformation Monitoring Using Optical and SAR Satellite Imagery
 Home-page: https://github.com/mahmudsfu/AkhDefo
 Author: Mahmud Mustafa Muhammad
 Author-email: mahmud.muhamm1@gmail.com
 License: Academic Free License (AFL)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `akhdefo_functions-2.5.3/akhdefo_functions.egg-info/SOURCES.txt` & `akhdefo_functions-2.5.4/akhdefo_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akhdefo_functions-2.5.3/setup.py` & `akhdefo_functions-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # Read the long description from the README file
 with open("./README_pypi.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # Setup configuration
 setup(
     name='akhdefo_functions',
-    version='2.5.3',
+    version='2.5.4',
     description='Land Deformation Monitoring Using Optical and SAR Satellite Imagery',
     url='https://github.com/mahmudsfu/AkhDefo',
     author='Mahmud Mustafa Muhammad',
     author_email='mahmud.muhamm1@gmail.com',
     license='Academic Free License (AFL)',
     packages=['akhdefo_functions'],
     long_description=long_description,
```

