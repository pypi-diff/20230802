# Comparing `tmp/centerline-width-1.1.0.tar.gz` & `tmp/centerline-width-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/centerline-width-1.1.0.tar", last modified: Mon Jul 31 06:52:33 2023, max compression
+gzip compressed data, was "dist/centerline-width-1.2.0.tar", last modified: Wed Aug  2 21:47:36 2023, max compression
```

## Comparing `centerline-width-1.1.0.tar` & `centerline-width-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.573910 centerline-width-1.1.0/
--rw-rw-r--   0 user      (1000) user      (1000)    53316 2023-07-31 06:52:33.573910 centerline-width-1.1.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    46958 2023-07-31 06:34:46.000000 centerline-width-1.1.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.569910 centerline-width-1.1.0/centerline_width/
--rw-rw-r--   0 user      (1000) user      (1000)     1949 2023-07-28 21:06:35.000000 centerline-width-1.1.0/centerline_width/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    28929 2023-07-28 21:33:59.000000 centerline-width-1.1.0/centerline_width/centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)    19456 2023-07-28 21:35:26.000000 centerline-width-1.1.0/centerline_width/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.1.0/centerline_width/getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    13110 2023-07-28 21:27:12.000000 centerline-width-1.1.0/centerline_width/plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.1.0/centerline_width/preprocessing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.573910 centerline-width-1.1.0/centerline_width/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)    17125 2023-07-29 22:22:33.000000 centerline-width-1.1.0/centerline_width/pytests/test_centerline.py
--rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.1.0/centerline_width/pytests/test_getCoordinatesKML.py
--rw-rw-r--   0 user      (1000) user      (1000)    15156 2023-07-29 22:17:03.000000 centerline-width-1.1.0/centerline_width/pytests/test_plotDiagrams.py
--rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.1.0/centerline_width/pytests/test_preprocessing.py
--rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.1.0/centerline_width/pytests/test_riverCenterlineClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     3486 2023-07-28 21:11:22.000000 centerline-width-1.1.0/centerline_width/relativeDistance.py
--rw-rw-r--   0 user      (1000) user      (1000)     9334 2023-07-28 21:36:14.000000 centerline-width-1.1.0/centerline_width/riverCenterlineClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 06:52:33.569910 centerline-width-1.1.0/centerline_width.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    53316 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      737 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      160 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       17 2023-07-31 06:52:33.000000 centerline-width-1.1.0/centerline_width.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 06:52:33.573910 centerline-width-1.1.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-07-31 06:41:29.000000 centerline-width-1.1.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.907874 centerline-width-1.2.0/
+-rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 21:47:36.903874 centerline-width-1.2.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    47490 2023-08-01 21:45:39.000000 centerline-width-1.2.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.899874 centerline-width-1.2.0/centerline_width/
+-rw-rw-r--   0 user      (1000) user      (1000)     1981 2023-08-01 00:12:16.000000 centerline-width-1.2.0/centerline_width/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    24559 2023-08-02 21:33:19.000000 centerline-width-1.2.0/centerline_width/centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19456 2023-08-01 21:47:42.000000 centerline-width-1.2.0/centerline_width/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1854 2023-05-18 02:15:59.000000 centerline-width-1.2.0/centerline_width/getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    12626 2023-08-02 20:44:38.000000 centerline-width-1.2.0/centerline_width/plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6759 2023-06-01 21:17:09.000000 centerline-width-1.2.0/centerline_width/preprocessing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.903874 centerline-width-1.2.0/centerline_width/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6529 2023-08-01 21:54:02.000000 centerline-width-1.2.0/centerline_width/pytests/test_centerline.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4472 2023-05-24 19:31:02.000000 centerline-width-1.2.0/centerline_width/pytests/test_getCoordinatesKML.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15156 2023-08-01 21:54:05.000000 centerline-width-1.2.0/centerline_width/pytests/test_plotDiagrams.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2457 2023-05-17 04:21:46.000000 centerline-width-1.2.0/centerline_width/pytests/test_preprocessing.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5105 2023-06-24 07:13:29.000000 centerline-width-1.2.0/centerline_width/pytests/test_riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11472 2023-08-01 21:54:49.000000 centerline-width-1.2.0/centerline_width/pytests/test_saveOutput.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3516 2023-08-02 20:45:43.000000 centerline-width-1.2.0/centerline_width/relativeDistance.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9334 2023-08-02 05:58:57.000000 centerline-width-1.2.0/centerline_width/riverCenterlineClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5833 2023-08-01 22:05:26.000000 centerline-width-1.2.0/centerline_width/saveOutput.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 21:47:36.903874 centerline-width-1.2.0/centerline_width.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    53896 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      812 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      160 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       17 2023-08-02 21:47:36.000000 centerline-width-1.2.0/centerline_width.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 21:47:36.907874 centerline-width-1.2.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1846 2023-08-02 21:45:52.000000 centerline-width-1.2.0/setup.py
```

### Comparing `centerline-width-1.1.0/PKG-INFO` & `centerline-width-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -71,28 +71,34 @@
         ```
         Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
         
         ```python
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
-        To plot the centerline, run the `plotCenterline()` function from `river_object` created
+        To plot the centerline, run the `plotCenterline()` function from `river_object` created. By default, will display with `Decimal Degrees` (latitude/longitude) coordinates
         ```python
         river_object.plotCenterline()
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
         
         To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
         
         While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
+        It is possible to also display all the coordinates as a `Relative Distance`, where all the coordinates are converted to a relative distance (in meters) from the first point on the left bank
+        ```python
+        river_object.plotCenterline(coordinate_unit="Relative Distance")
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_relative_distance_coords_centerline.png)
+        
         For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
         
         For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
         
         ## Preprocessing
         ### Generating KML files from Google Earth Pro
         Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
@@ -254,16 +260,16 @@
         * starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
         * bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
-        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
+        * x_voronoi_ridge_point_relative (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+        * y_voronoi_ridge_point_relative (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
         * interpolate_data (boolean): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
@@ -327,42 +333,42 @@
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
-        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
         * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
-        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
         * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -389,24 +395,24 @@
         plotCenterline(centerline_type="Voronoi",
         		marker_type="line",
         		centerline_color="black",
         		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False,
-        		coordinate_type="Decimal Degrees")
+        		coordinate_unit="Decimal Degrees")
         ```
         * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
         * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline()
         ```
         Output:
@@ -421,24 +427,24 @@
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
         		remove_intersections=False,
-        		coordinate_type="Decimal Degrees")
+        		coordinate_unit="Decimal Degrees")
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
@@ -459,19 +465,19 @@
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
-        **coordinate_type**
+        **coordinate_unit**
         
         Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
         
-        | coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+        | coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
         | ------------- | ------------- |
         | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
@@ -482,21 +488,21 @@
         
         Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
-        			coordinate_type="Decimal Degrees",
+        			coordinate_unit="Decimal Degrees",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.1.0/README.md` & `centerline-width-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -63,28 +63,34 @@
 ```
 Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
 
 ```python
 river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
 ```
 
-To plot the centerline, run the `plotCenterline()` function from `river_object` created
+To plot the centerline, run the `plotCenterline()` function from `river_object` created. By default, will display with `Decimal Degrees` (latitude/longitude) coordinates
 ```python
 river_object.plotCenterline()
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
 
 To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
 
 While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
 ```python
 river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
 ```
 ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
 
+It is possible to also display all the coordinates as a `Relative Distance`, where all the coordinates are converted to a relative distance (in meters) from the first point on the left bank
+```python
+river_object.plotCenterline(coordinate_unit="Relative Distance")
+```
+![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_relative_distance_coords_centerline.png)
+
 For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
 
 For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
 
 ## Preprocessing
 ### Generating KML files from Google Earth Pro
 Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
@@ -246,16 +252,16 @@
 * starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
 * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
 * ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
 * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
 * bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
 * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
 * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-* x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
-* y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
+* x_voronoi_ridge_point_relative (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+* y_voronoi_ridge_point_relative (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
 * interpolate_data (boolean): if interpolating between existing data, defaults to False
 * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
 * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
@@ -319,42 +325,42 @@
 ```
 Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
 
 ### Save Centerline Coordinates to a .CSV File
 Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
 
 ```
-saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
 ```
 * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
 * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
 * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
-* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+* [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
 ```
 Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
 
 Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
 
 ### Save Centerline Coordinates to a .MAT File
 Save the centerline coordinates to a .mat file with columns for latitude and longitude
 
 ```
-saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
 ```
 * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
 * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
 * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
-* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+* [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
 ```
 Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -381,24 +387,24 @@
 plotCenterline(centerline_type="Voronoi",
 		marker_type="line",
 		centerline_color="black",
 		display_all_possible_paths=False, 
 		plot_title=None, 
 		save_plot_name=None, 
 		display_voronoi=False,
-		coordinate_type="Decimal Degrees")
+		coordinate_unit="Decimal Degrees")
 ```
 * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
 * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
 * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
 * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
-* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+* [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterline()
 ```
 Output:
@@ -413,24 +419,24 @@
 plotCenterlineWidth(plot_title=None, 
 		save_plot_name=None, 
 		display_true_centerline=True,
 		transect_span_distance=3,
 		apply_smoothing=False,
 		flag_intersections=True,
 		remove_intersections=False,
-		coordinate_type="Decimal Degrees")
+		coordinate_unit="Decimal Degrees")
 ```
 * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
 * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
 * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
 * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
-* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+* [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 
 **apply_smoothing**
 
 apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
 
 | apply_smoothing=False | apply_smoothing=True |
 | ------------- | ------------- |
@@ -451,19 +457,19 @@
 
 Intersecting lines are flagged in red by default (flag_intersections=True)
 
 | remove_intersections=False | remove_intersections=True |
 | ------------- | ------------- |
 | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
 
-**coordinate_type**
+**coordinate_unit**
 
 Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
 
-| coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+| coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
 | ------------- | ------------- |
 | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
 river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
@@ -474,21 +480,21 @@
 
 Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
 
 ```
 riverWidthFromCenterline(transect_span_distance=3,
 			apply_smoothing=True,
 			remove_intersections=False,
-			coordinate_type="Decimal Degrees",
+			coordinate_unit="Decimal Degrees",
 			save_to_csv=None)
 ```
 * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
 * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
 * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-* [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+* [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
 * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
 
 Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
 
 ```python
 import centerline_width
 river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.1.0/centerline_width/__init__.py` & `centerline-width-1.2.0/centerline_width/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,18 @@
 from .centerline import networkXGraphShortestPath
 from .centerline import centerlineLength
 from .centerline import equalDistanceCenterline
 from .centerline import evenlySpacedCenterline
 from .centerline import smoothedCoordinates
 from .centerline import riverWidthFromCenterlineCoordinates
 from .centerline import riverWidthFromCenterline
-from .centerline import saveCenterlineCSV
-from .centerline import saveCenterlineMAT
+
+# saveOutput.py function calls
+from .saveOutput import saveCenterlineCSV
+from .saveOutput import saveCenterlineMAT
 
 # plotDiagrams.py function calls
 from .plotDiagrams import plotCenterline
 from .plotDiagrams import plotCenterlineWidth
 
 # error_handling.py function calls
 from .error_handling import errrorHandlingConvertColumnsToCSV
```

### Comparing `centerline-width-1.1.0/centerline_width/centerline.py` & `centerline-width-1.2.0/centerline_width/centerline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # Built in Python functions
 import math
 import logging
-import csv
 
 # External Python libraries (installed via pip install)
 import numpy as np
 import networkx as nx
 from scipy import interpolate
-from scipy.io import savemat
 from shapely.geometry import Point, LineString
 from shapely.ops import split
 import pyproj
 import geopy.distance
 
 # Internal centerline_width reference to access functions, global variables, and error handling
 import centerline_width
@@ -198,15 +196,15 @@
 
 	return smoothed_coordinates
 
 def riverWidthFromCenterlineCoordinates(river_object=None,
 										centerline_coordinates=None,
 										transect_span_distance=3,
 										remove_intersections=False,
-										coordinate_type="Decimal Degrees",
+										coordinate_unit="Decimal Degrees",
 										save_to_csv=None):
 	# Return the left/right coordinates of width centerlines
 	right_width_coordinates = {}
 	left_width_coordinates = {}
 	num_intersection_coordinates = {}
 	x = []
 	y = []
@@ -225,15 +223,15 @@
 					slope_sum += (dy / dx)
 					total_slopes += 1
 		if slope_sum != 0:
 			slope_avg = slope_sum / total_slopes
 			normal_of_slope = -1 / slope_avg
 			middle_of_list = len(group_points) // 2 # set centerline point to be the middle point being averaged
 			centerline_slope[group_points[middle_of_list]] = normal_of_slope
-
+	
 	def intersectsTopOrBottomOfBank(point1, point2):
 		# returns True/False if the points lie on the 'false' top/bottom of the river
 		points_intersect_false_edges = False
 
 		# avoiding floating point precession errors when determining if point lies within the line
 		# if point is within a small distance of a line it is considered to intersect
 		if river_object.top_bank.distance(point1) < 1e-8 or river_object.bottom_bank.distance(point1) < 1e-8:
@@ -250,37 +248,39 @@
 		# draw a max line that extends the entire distance of the available space, will be trimmed below to just within polygon
 		left_y = slope * (min_x - centerline_point[0]) + centerline_point[1]
 		right_y = slope * (max_x - centerline_point[0]) + centerline_point[1]
 
 		# Save the points where they intersect the polygon
 		sloped_line = LineString([(min_x, left_y), (max_x, right_y)]) # sloped line from the centerpoint
 		line_intersection_points = river_object.bank_polygon.exterior.intersection(sloped_line) # points where the line intersects the polygon
+
 		# if the line only intersects in two places (does not intersect polygon any additional times)
-		if len(line_intersection_points.geoms) == 2:
-			 # only save width lines that do not touch the artifical top/bottom
-			if not intersectsTopOrBottomOfBank(line_intersection_points.geoms[0], line_intersection_points.geoms[1]):
-				left_width_coordinates[centerline_point] = (line_intersection_points.geoms[0].x, line_intersection_points.geoms[0].y)
-				right_width_coordinates[centerline_point] = (line_intersection_points.geoms[1].x, line_intersection_points.geoms[1].y)
-		else:
-			# line intersects to polygon at multiple points
-			if river_object.bank_polygon.contains(Point(centerline_point)): # width line made by centering centerline point, skip this width line if the centerline is outside of the polygon due to smoothing
-				all_linestring = split(sloped_line, river_object.bank_polygon) # split linestring where it intersects the polygon
-				left_point = None
-				right_point = None
-				for i, possible_linestring in enumerate(all_linestring.geoms): # iterate through all linestrings
-					if possible_linestring.distance(Point(centerline_point)) < 1e-8: # select linestring that contains the centerline point
-						left_point = Point(possible_linestring.coords[0])
-						right_point = Point(possible_linestring.coords[1])
-
-				# linestring contains the centerline, save coordinates
-				if left_point is not None and right_point is not None:
-					 # only save width lines that do not touch the artifical top/bottom
-					if not intersectsTopOrBottomOfBank(left_point, right_point):
-						left_width_coordinates[centerline_point] = (left_point.x, left_point.y)
-						right_width_coordinates[centerline_point] = (right_point.x, right_point.y)
+		if str(line_intersection_points) != "LINESTRING Z EMPTY": # if linestring has intersect (not empty)
+			if len(line_intersection_points.geoms) == 2:
+				 # only save width lines that do not touch the artifical top/bottom
+				if not intersectsTopOrBottomOfBank(line_intersection_points.geoms[0], line_intersection_points.geoms[1]):
+					left_width_coordinates[centerline_point] = (line_intersection_points.geoms[0].x, line_intersection_points.geoms[0].y)
+					right_width_coordinates[centerline_point] = (line_intersection_points.geoms[1].x, line_intersection_points.geoms[1].y)
+			else:
+				# line intersects to polygon at multiple points
+				if river_object.bank_polygon.contains(Point(centerline_point)): # width line made by centering centerline point, skip this width line if the centerline is outside of the polygon due to smoothing
+					all_linestring = split(sloped_line, river_object.bank_polygon) # split linestring where it intersects the polygon
+					left_point = None
+					right_point = None
+					for i, possible_linestring in enumerate(all_linestring.geoms): # iterate through all linestrings
+						if possible_linestring.distance(Point(centerline_point)) < 1e-8: # select linestring that contains the centerline point
+							left_point = Point(possible_linestring.coords[0])
+							right_point = Point(possible_linestring.coords[1])
+
+					# linestring contains the centerline, save coordinates
+					if left_point is not None and right_point is not None:
+						 # only save width lines that do not touch the artifical top/bottom
+						if not intersectsTopOrBottomOfBank(left_point, right_point):
+							left_width_coordinates[centerline_point] = (left_point.x, left_point.y)
+							right_width_coordinates[centerline_point] = (right_point.x, right_point.y)
 
 	# Determine lines that intersect with other lines in multiple places to flag/remove
 	all_linestrings = []
 	linestring_with_centerlines = {} # linestring with associated centerline: {linestring : centerline coordinate}
 	linestring_with_linestrings_that_intersect = {} # dictionary of all the linestrings that a linestring intersects with
 	# Generate a list of linestrings
 	for centerline_coord in right_width_coordinates.keys():
@@ -340,72 +340,82 @@
 
 		# Delete all width lines that have been flagged for removal
 		for centerline_coord in centerline_coordinates_to_be_removed:
 			del right_width_coordinates[centerline_coord]
 			del left_width_coordinates[centerline_coord]
 		logger.info("[SUCCESS] Intersection lines removed")
 
+	if coordinate_unit == "Relative Distance":
+		right_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], right_width_coordinates, river_object.ellipsoid)
+		left_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], left_width_coordinates, river_object.ellipsoid)
+		num_intersection_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], num_intersection_coordinates, river_object.ellipsoid)
+	
 	return right_width_coordinates, left_width_coordinates, num_intersection_coordinates
 
 def riverWidthFromCenterline(river_object=None,
 							transect_span_distance=3,
 							apply_smoothing=True,
 							remove_intersections=False,
-							coordinate_type="Decimal Degrees",
+							coordinate_unit="Decimal Degrees",
 							save_to_csv=None):
 	# Return river width: centerline and width at centerline
 	# Width is measured to the bank, relative to the center point (normal of the centerline)
 	# { [centerline latitude, centerline longitude] : widthValue }
 
 	centerline_width.errorHandlingRiverWidthFromCenterline(river_object=river_object,
 															transect_span_distance=transect_span_distance,
 															apply_smoothing=apply_smoothing,
 															remove_intersections=remove_intersections,
-															coordinate_type=coordinate_type,
+															coordinate_unit=coordinate_unit,
 															save_to_csv=save_to_csv)
 
-	coordinate_type = coordinate_type.title()
+	coordinate_unit = coordinate_unit.title()
 
 	if river_object.centerlineVoronoi is None:
 		logger.critical("\nCRITICAL ERROR, unable to find width without a valid centerline")
 		return None
 
-	# recreate the centerline with evenly spaced points
-	defined_centerline_coordinates = centerline_width.evenlySpacedCenterline(centerline_coordinates=river_object.centerlineVoronoi,
-																			number_of_fixed_points=river_object.interpolate_n_centerpoints)
+	# Run all as "Decimal Degrees" to be able to calculate width below
 	if apply_smoothing:
-		defined_centerline_coordinates = centerline_width.smoothedCoordinates(river_object=river_object,
-																				centerline_coordinates=river_object.centerlineVoronoi,
-																				interprolate_num=river_object.interpolate_n_centerpoints)
-	# if using smoothing, replace left/right coordinates with the smoothed variation
-	right_width_coord, left_width_coord, _ = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
-																								centerline_coordinates=defined_centerline_coordinates,
-																								transect_span_distance=transect_span_distance,
-																								remove_intersections=remove_intersections)
-
+		# if using smoothing, replace left/right coordinates with the smoothed variation
+		right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
+																																			centerline_coordinates=river_object.centerlineSmoothed,
+																																			transect_span_distance=transect_span_distance,
+																																			remove_intersections=remove_intersections,
+																																			coordinate_unit="Decimal Degrees")
+	else:
+		right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
+																																			centerline_coordinates=river_object.centerlineEvenlySpaced,
+																																			transect_span_distance=transect_span_distance,
+																																			remove_intersections=remove_intersections,
+																																			coordinate_unit="Decimal Degrees")
 	width_dict = {}
 
 	geodesic = pyproj.Geod(ellps=river_object.ellipsoid)
 
-	for centerline_coord, _ in right_width_coord.items():
+	for centerline_coord, _ in right_width_coordinates.items():
 		# store the distance between the lat/lon position of the right/left bank
-		lon1, lat1 = right_width_coord[centerline_coord]
-		lon2, lat2 = left_width_coord[centerline_coord]
+		lon1, lat1 = right_width_coordinates[centerline_coord]
+		lon2, lat2 = left_width_coordinates[centerline_coord]
 		_, _, distance_between_right_and_left_m = geodesic.inv(lon1, lat1, lon2, lat2)
 		width_dict[centerline_coord] = distance_between_right_and_left_m/1000
 
+	# Convert to Relative Distance after accounting for the width dictionary
+	if coordinate_unit == "Relative Distance":
+		right_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], right_width_coordinates, river_object.ellipsoid)
+		left_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], left_width_coordinates, river_object.ellipsoid)
+		width_dict = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], width_dict, river_object.ellipsoid)
+
 	# Set headers and conver to Relative Distance if needed
-	if coordinate_type == "Decimal Degrees":
+	if coordinate_unit == "Decimal Degrees":
 		latitude_header= "Centerline Latitude (Deg)"
 		longitude_header = "Centerline Longitude (Deg)"
-	if coordinate_type == "Relative Distance":
+	if coordinate_unit == "Relative Distance":
 		latitude_header= "Relative Distance Y (from Latitude) (m)"
 		longitude_header = "Relative Distance X (from Longitude) (m)"
-		# Convert from Decimal Degrees to Relative Distance
-		width_dict = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], width_dict, river_object.ellipsoid)
 
 	# Save width dictionary to a csv file (Latitude, Longtiude, Width)
 	if save_to_csv:
 		with open(save_to_csv, "w") as csv_file_output:
 			writer = csv.writer(csv_file_output)
 			writer.writerow([latitude_header,longitude_header, "Width (km)"])
 			for coordinate_key, width_value in width_dict.items():
@@ -427,109 +437,7 @@
 			previous_pair = xy_pair
 		else:
 			lon1, lon2 = previous_pair[0], xy_pair[0]
 			lat1, lat2 = previous_pair[1], xy_pair[1]
 			_, _, distance_between_meters = geodesic.inv(lon1, lat1, lon2, lat2)
 			total_length += distance_between_meters
 	return total_length/1000
-
-def saveCenterlineCSV(river_object=None,
-					save_to_csv=None,
-					latitude_header=None,
-					longitude_header=None,
-					centerline_type="Voronoi",
-					coordinate_type="Decimal Degrees"):
-	# Save Centerline Coordinates generated by Voronoi Diagram to .CSV
-	centerline_width.errorHandlingSaveCenterlineCSV(river_object=river_object,
-													save_to_csv=save_to_csv, 
-													latitude_header=latitude_header,
-													longitude_header=longitude_header,
-													centerline_type=centerline_type,
-													coordinate_type=coordinate_type)
-	centerline_type = centerline_type.title()
-	coordinate_type = coordinate_type.title()
-
-	if coordinate_type == "Decimal Degrees":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
-	if coordinate_type == "Relative Distance":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
-
-	if coordinate_type == "Decimal Degrees":
-		if latitude_header is None:
-			latitude_header = "{0} Centerline Latitude (Deg)".format(centerline_type)
-		if longitude_header is None:
-			longitude_header = "{0} Centerline Longitude (Deg)".format(centerline_type)
-	if coordinate_type == "Relative Distance":
-		if latitude_header is None:
-			latitude_header = "{0} Relative Distance Y (from Latitude) (m)".format(centerline_type)
-		if longitude_header is None:
-			longitude_header = "{0} Relative Distance X (from Longitude) (m)".format(centerline_type)
-
-	with open(save_to_csv, "w") as csv_file_output:
-		writer = csv.writer(csv_file_output)
-		writer.writerow([latitude_header, longitude_header])
-		if centerline_coordinates_by_type is not None:
-			for latitude_longitude in centerline_coordinates_by_type:
-				writer.writerow([latitude_longitude[1], latitude_longitude[0]])
-		else:
-			logger.warn("\nWARNING, no {0} centerline coordinates found, {1} file generated will be empty".format(centerline_type, save_to_csv))
-
-def saveCenterlineMAT(river_object=None,
-					save_to_mat=None,
-					latitude_header=None,
-					longitude_header=None,
-					centerline_type="Voronoi",
-					coordinate_type="Decimal Degrees"):
-	# Save Centerline Coordinates generated by Voronoi Diagram to .MAT
-	centerline_width.errorHandlingSaveCenterlineMAT(river_object=river_object,
-													save_to_mat=save_to_mat, 
-													latitude_header=latitude_header,
-													longitude_header=longitude_header,
-													centerline_type=centerline_type,
-													coordinate_type=coordinate_type)
-	centerline_type = centerline_type.title()
-	coordinate_type = coordinate_type.title()
-
-	if coordinate_type == "Decimal Degrees":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoi
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothed
-	if coordinate_type == "Relative Distance":
-		if centerline_type == "Voronoi": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
-		if centerline_type == "Equal Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
-		if centerline_type == "Evenly Spaced": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
-		if centerline_type == "Smoothed": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
-
-	# .mat files do not allow for spaces or special characters in the header
-	if coordinate_type == "Decimal Degrees":
-		if latitude_header is None:
-			latitude_header = "{0}_Centerline_Latitude_Deg".format(centerline_type.replace(" ", "_"))
-		if longitude_header is None:
-			longitude_header = "{0}_Centerline_Longitude_Deg".format(centerline_type.replace(" ", "_"))
-	if coordinate_type == "Relative Distance":
-		if latitude_header is None:
-			latitude_header = "{0}_Relative_Distance_Y_From_Latitude_m".format(centerline_type.replace(" ", "_"))
-		if longitude_header is None:
-			longitude_header = "{0}_Relative_Distance_X_From_Longitude_m".format(centerline_type.replace(" ", "_"))		
-
-	latitude_lst = []
-	longtiude_lst = []
-
-	if centerline_coordinates_by_type is not None:
-		for latitude_longitude in centerline_coordinates_by_type:
-			longtiude_lst.append(latitude_longitude[0])
-			latitude_lst.append(latitude_longitude[1])
-	else:
-		logger.warn("\nWARNING, no {0} centerline coordinates found, {1} file generated will be empty".format(centerline_type, save_to_mat))
-	
-	# Centerline dictionary of latitude and longtiude centerline coordinates
-	centerline_dict = {latitude_header: np.asarray(latitude_lst), longitude_header: np.asarray(longtiude_lst)}
-
-	# Save to matlab format (.mat)
-	savemat(save_to_mat, mdict=centerline_dict)
```

### Comparing `centerline-width-1.1.0/centerline_width/error_handling.py` & `centerline-width-1.2.0/centerline_width/error_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 								centerline_type=None,
 								marker_type=None,
 								centerline_color=None,
 								display_all_possible_paths=None,
 								plot_title=None,
 								save_plot_name=None,
 								display_voronoi=None,
-								coordinate_type=None):
+								coordinate_unit=None):
 	# Error handling for plotCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -89,32 +89,32 @@
 		logger.critical("\nCRITICAL ERROR, [save_plot_name]: Must be a str, current type = '{0}'".format(type(save_plot_name)))
 		exit()
 
 	if type(display_voronoi) != bool:
 		logger.critical("\nCRITICAL ERROR, [display_voronoi]: Must be a bool, current type = '{0}'".format(type(display_voronoi)))
 		exit()
 
-	if type(coordinate_type) != str:
-		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+	if type(coordinate_unit) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(type(coordinate_unit)))
 		exit()
 	else:
-		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
-		if coordinate_type.title() not in coordinate_type_options:
-			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+		coordinate_unit_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_unit.title() not in coordinate_unit_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in {0}, current option = '{1}'".format(coordinate_unit_options, coordinate_unit))
 			exit()
 
 def errorHandlingPlotCenterlineWidth(river_object=None,
 									plot_title=None,
 									save_plot_name=None,
 									display_true_centerline=None,
 									transect_span_distance=None,
 									apply_smoothing=None,
 									flag_intersections=None,
 									remove_intersections=None,
-									coordinate_type=None):
+									coordinate_unit=None):
 	# Error handling for plotCenterlineWidth()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -149,29 +149,29 @@
 		logger.critical("\nCRITICAL ERROR, [flag_intersections]: Must be a bool, current type = '{0}'".format(type(flag_intersections)))
 		exit()
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
-	if type(coordinate_type) != str:
-		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+	if type(coordinate_unit) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(type(coordinate_unit)))
 		exit()
 	else:
-		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
-		if coordinate_type.title() not in coordinate_type_options:
-			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+		coordinate_unit_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_unit.title() not in coordinate_unit_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in {0}, current option = '{1}'".format(coordinate_unit_options, coordinate_unit))
 			exit()
 
 ## Error Handling: centerline.py
 def errorHandlingRiverWidthFromCenterline(river_object=None,
 										transect_span_distance=None,
 										apply_smoothing=None,
 										remove_intersections=None,
-										coordinate_type=None,
+										coordinate_unit=None,
 										save_to_csv=None):
 	# Error Handling for riverWidthFromCenterline()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
@@ -191,21 +191,21 @@
 		logger.critical("\nCRITICAL ERROR, [apply_smoothing]: Must be a bool, current type = '{0}'".format(type(apply_smoothing)))
 		exit()
 
 	if type(remove_intersections) != bool:
 		logger.critical("\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(type(remove_intersections)))
 		exit()
 
-	if type(coordinate_type) != str:
-		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+	if type(coordinate_unit) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(type(coordinate_unit)))
 		exit()
 	else:
-		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
-		if coordinate_type.title() not in coordinate_type_options:
-			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+		coordinate_unit_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_unit.title() not in coordinate_unit_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in {0}, current option = '{1}'".format(coordinate_unit_options, coordinate_unit))
 			exit()
 
 	if save_to_csv is not None:
 		if type(save_to_csv) != str:
 			logger.critical("\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(type(save_to_csv)))
 			exit()
 		if not save_to_csv.lower().endswith(".csv"):
@@ -213,15 +213,15 @@
 			exit()
 
 def errorHandlingSaveCenterlineCSV(river_object=None,
 								latitude_header=None,
 								longitude_header=None,
 								save_to_csv=None,
 								centerline_type=None,
-								coordinate_type=None):
+								coordinate_unit=None):
 	# Error Handling for saveCenterlineCSV()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -251,29 +251,29 @@
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
 
-	if type(coordinate_type) != str:
-		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+	if type(coordinate_unit) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(type(coordinate_unit)))
 		exit()
 	else:
-		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
-		if coordinate_type.title() not in coordinate_type_options:
-			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+		coordinate_unit_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_unit.title() not in coordinate_unit_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in {0}, current option = '{1}'".format(coordinate_unit_options, coordinate_unit))
 			exit()
 
 def errorHandlingSaveCenterlineMAT(river_object=None,
 								latitude_header=None,
 								longitude_header=None,
 								save_to_mat=None,
 								centerline_type=None,
-								coordinate_type=None):
+								coordinate_unit=None):
 	# Error Handling for saveCenterlineMAT()
 	if river_object is None:
 		logger.critical("\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)")
 		exit()
 	else:
 		if not isinstance(river_object, centerline_width.riverCenterline):
 			logger.critical("\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(type(river_object)))
@@ -311,21 +311,21 @@
 		logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be a str, current type = '{0}'".format(type(centerline_type)))
 		exit()
 	else:
 		if centerline_type.title() not in centerline_type_options:
 			logger.critical("\nCRITICAL ERROR, [centerline_type]: Must be an available option in {0}, current option = '{1}'".format(centerline_type_options, centerline_type))
 			exit()
 
-	if type(coordinate_type) != str:
-		logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(type(coordinate_type)))
+	if type(coordinate_unit) != str:
+		logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(type(coordinate_unit)))
 		exit()
 	else:
-		coordinate_type_options = ["Decimal Degrees", "Relative Distance"]
-		if coordinate_type.title() not in coordinate_type_options:
-			logger.critical("\nCRITICAL ERROR, [coordinate_type]: Must be an available option in {0}, current option = '{1}'".format(coordinate_type_options, coordinate_type))
+		coordinate_unit_options = ["Decimal Degrees", "Relative Distance"]
+		if coordinate_unit.title() not in coordinate_unit_options:
+			logger.critical("\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in {0}, current option = '{1}'".format(coordinate_unit_options, coordinate_unit))
 			exit()
 
 # Error Handling: getCoordinatesKML.py
 def errorHandlingExtractPointsToTextFile(left_kml=None, right_kml=None, text_output_name=None):
 	# Error Handling for extractPointsToTextFile()
 	if left_kml is None:
 		logger.critical("\nCRITICAL ERROR, [left_kml]: Requires left_kml file")
```

### Comparing `centerline-width-1.1.0/centerline_width/getCoordinatesKML.py` & `centerline-width-1.2.0/centerline_width/getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.1.0/centerline_width/plotDiagrams.py` & `centerline-width-1.2.0/centerline_width/plotDiagrams.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,36 +16,36 @@
 logger.addHandler(stream_handler)
 
 def plotCenterlineBackend(river_object=None,
 						display_true_centerline=True,
 						centerline_type="Voronoi",
 						marker_type="line",
 						centerline_color="black",
-						coordinate_type=None):
+						coordinate_unit=None):
 	# Shared components between plotCenterline and plotCenterlineWidth
 	fig = plt.figure(figsize=(10,10))
 	ax = fig.add_subplot(111)
 	scatter_plot_size = 4
 	
-	coordinate_type = coordinate_type.title()
+	coordinate_unit = coordinate_unit.title()
 	# Plot River as a Polygon
-	if coordinate_type == "Decimal Degrees":
+	if coordinate_unit == "Decimal Degrees":
 		plt.plot(*river_object.bank_polygon.exterior.xy, c="gainsboro")
 		plt.plot(*river_object.top_bank.xy, c="forestgreen")
 		plt.plot(*river_object.bottom_bank.xy, c="lightcoral")
-	if coordinate_type == "Relative Distance":
+	if coordinate_unit == "Relative Distance":
 		plt.plot(*river_object.bank_polygon_relative.exterior.xy, c="gainsboro")
 		plt.plot(*river_object.top_bank_relative.xy, c="forestgreen")
 		plt.plot(*river_object.bottom_bank_relative.xy, c="lightcoral")
 
 	# Choose between Decimal Degrees and Relative Distances for X, Y coordinates
-	if coordinate_type == "Decimal Degrees":
+	if coordinate_unit == "Decimal Degrees":
 		right_coords =  river_object.right_bank_coordinates
 		left_coords =  river_object.left_bank_coordinates
-	if coordinate_type == "Relative Distance":
+	if coordinate_unit == "Relative Distance":
 		right_coords =  river_object.right_bank_relative_coordinates
 		left_coords =  river_object.left_bank_relative_coordinates
 
 	x = [i[0] for i in right_coords]
 	y = [i[1] for i in right_coords]
 	plt.scatter(x, y, c="dodgerblue", s=scatter_plot_size, label="Right Bank")
 	x = [i[0] for i in left_coords]
@@ -57,31 +57,31 @@
 
 	centerline_type = centerline_type.title()
 	marker_type = marker_type.title()
 
 	# Choose btween Decimal Degrees and Centerline Type
 	if centerline_type == "Voronoi": 
 		centerline_legend = "Voronoi Centerline Coordinates"
-		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineVoronoi
-		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
+		if coordinate_unit == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineVoronoi
+		if coordinate_unit == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineVoronoiRelative
 
 	if centerline_type == "Equal Distance": 
 		centerline_legend = "Equal Distance Centerline Coordinates"
-		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEqualDistance
-		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
+		if coordinate_unit == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEqualDistance
+		if coordinate_unit == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEqualDistanceRelative
 
 	if centerline_type == "Evenly Spaced": 
 		centerline_legend = "Evenly Spaced Centerline Coordiantes"
-		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
-		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
+		if coordinate_unit == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineEvenlySpaced
+		if coordinate_unit == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineEvenlySpacedRelative
 
 	if centerline_type == "Smoothed": 
 		centerline_legend = "Smoothed Centerlined Coordiantes"
-		if coordinate_type == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineSmoothed
-		if coordinate_type == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
+		if coordinate_unit == "Decimal Degrees": centerline_coordinates_by_type = river_object.centerlineSmoothed
+		if coordinate_unit == "Relative Distance": centerline_coordinates_by_type = river_object.centerlineSmoothedRelative
 
 	# Plot the centerline coordinates
 	if centerline_coordinates_by_type:
 		valid_path_through = True
 		if display_true_centerline:
 			if marker_type == "Line":
 				plt.plot(*zip(*centerline_coordinates_by_type), c=centerline_color, label=centerline_legend, zorder=10)
@@ -92,78 +92,78 @@
 					x.append(k)
 					y.append(v)
 				plt.scatter(x, y, c=centerline_color, label=centerline_legend, s=8, zorder=10)
 
 	# Dynamically assign the starting and ending
 	if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 		ss = 45 # scatter size
-		if coordinate_type == "Decimal Degrees":
+		if coordinate_unit == "Decimal Degrees":
 			plt.scatter(river_object.starting_node[0], river_object.starting_node[1], c="green", label="Starting Node", s=ss)
 			plt.scatter(river_object.ending_node[0], river_object.ending_node[1], c="red", label="Ending Node", s=ss)
-		if coordinate_type == "Relative Distance":
+		if coordinate_unit == "Relative Distance":
 			plt.scatter(river_object.starting_node_relative[0], river_object.starting_node_relative[1], c="green", label="Starting Node", s=ss)
 			plt.scatter(river_object.ending_node_relative[0], river_object.ending_node_relative[1], c="red", label="Ending Node", s=ss)
 
 	return fig, ax, valid_path_through
 
 def plotCenterline(river_object=None,
 					centerline_type="Voronoi",
 					marker_type="line",
 					centerline_color="black",
 					display_all_possible_paths=False, 
 					plot_title=None, 
 					save_plot_name=None, 
 					display_voronoi=False,
-					coordinate_type="Decimal Degrees"):
+					coordinate_unit="Decimal Degrees"):
 	# Plot Centerline of River
 	centerline_width.errorHandlingPlotCenterline(river_object=river_object,
 												centerline_type=centerline_type,
 												marker_type=marker_type,
 												centerline_color=centerline_color,
 												display_all_possible_paths=display_all_possible_paths,
 												plot_title=plot_title,
 												save_plot_name=save_plot_name,
 												display_voronoi=display_voronoi,
-												coordinate_type=coordinate_type)
+												coordinate_unit=coordinate_unit)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object,
 														display_true_centerline=True,
 														centerline_type=centerline_type,
 														marker_type=marker_type,
 														centerline_color=centerline_color,
-														coordinate_type=coordinate_type)
+														coordinate_unit=coordinate_unit)
 
-	coordinate_type = coordinate_type.title()
+	coordinate_unit = coordinate_unit.title()
 
 	# Display the Voronoi Diagram
 	if display_voronoi:
-		if coordinate_type == "Decimal Degrees":
+		if coordinate_unit == "Decimal Degrees":
 			voronoi_plot_2d(river_object.bank_voronoi, show_points=True, point_size=1, ax=ax)
-		if coordinate_type == "Relative Distance":
+		if coordinate_unit == "Relative Distance":
 			voronoi_plot_2d(river_object.bank_voronoi_relative, show_points=True, point_size=1, ax=ax)
 
 	# Plot all possible paths with text for positions
 	if display_all_possible_paths:
-		if coordinate_type == "Decimal Degrees":
+		if coordinate_unit == "Decimal Degrees":
 			for i in range(len(river_object.x_voronoi_ridge_point)):
 				plt.plot(river_object.x_voronoi_ridge_point[i], river_object.y_voronoi_ridge_point[i], 'cyan', linewidth=1, zorder=1)
-		if coordinate_type == "Relative Distance":
+		if coordinate_unit == "Relative Distance":
 			for i in range(len(river_object.x_voronoi_ridge_point_relative)):
 				plt.plot(river_object.x_voronoi_ridge_point_relative[i], river_object.y_voronoi_ridge_point_relative[i], 'cyan', linewidth=1, zorder=1)
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Coordinates: Valid Centerline = {0}, Valid Polygon = {1}, Interpolated = {2}".format(valid_path_through, river_object.bank_polygon.is_valid, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 
-	if coordinate_type == "Decimal Degrees":
+	if coordinate_unit == "Decimal Degrees":
 		plt.xlabel("Longitude (°)")
 		plt.ylabel("Latitude (°)")
-	if coordinate_type == "Relative Distance":
+	if coordinate_unit == "Relative Distance":
 		plt.xlabel("Relative Distance X (m)")
 		plt.ylabel("Relative Distance Y (m)")
 
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
 
@@ -171,69 +171,65 @@
 						plot_title=None, 
 						save_plot_name=None, 
 						display_true_centerline=True,
 						transect_span_distance=3,
 						apply_smoothing=False,
 						flag_intersections=True,
 						remove_intersections=False,
-						coordinate_type="Decimal Degrees"):
+						coordinate_unit="Decimal Degrees"):
 	# Plot Width Lines based on Centerline
 	centerline_width.errorHandlingPlotCenterlineWidth(river_object=river_object,
 													plot_title=plot_title, 
 													save_plot_name=save_plot_name, 
 													display_true_centerline=display_true_centerline,
 													transect_span_distance=transect_span_distance,
 													apply_smoothing=apply_smoothing,
 													flag_intersections=flag_intersections,
 													remove_intersections=remove_intersections,
-													coordinate_type=coordinate_type)
+													coordinate_unit=coordinate_unit)
 
 	fig, ax, valid_path_through = plotCenterlineBackend(river_object=river_object, 
 														display_true_centerline=display_true_centerline,
 														centerline_type="Voronoi",
 														marker_type="line",
 														centerline_color="black",
-														coordinate_type=coordinate_type)
+														coordinate_unit=coordinate_unit)
 
-	coordinate_type = coordinate_type.title()
+	coordinate_unit = coordinate_unit.title()
 	# Determine the Width of River
 	number_of_evenly_spaced_points = ""
 
 	if river_object.centerlineVoronoi is not None:
 		number_of_evenly_spaced_points = "\nCenterline made of {0} Fixed Points, width lines generated every {1} points".format(river_object.interpolate_n_centerpoints, transect_span_distance)
 		if river_object.starting_node is not None: # error handling for when data is too small to generate centerline coordiantes
 
 			# if using smoothing, replace left/right coordinates with the smoothed variation
 			if apply_smoothing:
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object,
 																																					centerline_coordinates=river_object.centerlineSmoothed,
 																																					transect_span_distance=transect_span_distance,
-																																					remove_intersections=remove_intersections)
+																																					remove_intersections=remove_intersections,
+																																					coordinate_unit=coordinate_unit)
 				x = []
 				y = []
-				if coordinate_type == "Decimal Degrees":
+				if coordinate_unit == "Decimal Degrees":
 					smoothed_coords = river_object.centerlineSmoothed
-				if coordinate_type == "Relative Distance":
+				if coordinate_unit == "Relative Distance":
 					smoothed_coords = river_object.centerlineSmoothedRelative
 				for k, v in smoothed_coords:
 					x.append(k)
 					y.append(v)
 				plt.scatter(x, y, c="blue", label="Smoothed Centerline Coordinates", s=5)
 			else:
 				# recreate the centerline with evenly spaced points
 				right_width_coordinates, left_width_coordinates, num_intersection_coordinates = centerline_width.riverWidthFromCenterlineCoordinates(river_object=river_object, 
 																														centerline_coordinates=river_object.centerlineEvenlySpaced,
 																														transect_span_distance=transect_span_distance,
-																														remove_intersections=remove_intersections)
-
-			if coordinate_type == "Relative Distance":
-				# by default, sets up width with Decimal Degree, convert to Relative Distance
-				right_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], right_width_coordinates, river_object.ellipsoid)
-				left_width_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], left_width_coordinates, river_object.ellipsoid)
-				num_intersection_coordinates = centerline_width.relativeWidthCoordinates(river_object.left_bank_coordinates[0], num_intersection_coordinates, river_object.ellipsoid)
+																														remove_intersections=remove_intersections,
+																														coordinate_unit=coordinate_unit)
 
 			invalid_label_added = False # prevent legend for width lines from being generated more than once (because is inside a loop)
 			valid_label_added = False  # prevent legend for width lines from being generated more than once (because is inside a loop)
 			# plot width lines
 			for center_coord, edge_coord in right_width_coordinates.items():
 				x_points = (right_width_coordinates[center_coord][0], left_width_coordinates[center_coord][0])
 				y_points = (right_width_coordinates[center_coord][1], left_width_coordinates[center_coord][1])
@@ -261,17 +257,17 @@
 
 	# Plot Title, Legends, and Axis Labels
 	if not plot_title:
 		plt.title("River Width Coordinates: Valid Centerline = {0}, Valid Polygon = {1}{2}, Interpolated = {3}".format(valid_path_through, river_object.bank_polygon.is_valid, number_of_evenly_spaced_points, river_object.interpolate_data))
 	else:
 		plt.title(plot_title)
 
-	if coordinate_type == "Decimal Degrees":
+	if coordinate_unit == "Decimal Degrees":
 		plt.xlabel("Longitude (°)")
 		plt.ylabel("Latitude (°)")
-	if coordinate_type == "Relative Distance":
+	if coordinate_unit == "Relative Distance":
 		plt.xlabel("Relative Distance X (m)")
 		plt.ylabel("Distance Distance Y (m)")
 
 	plt.legend(loc="upper right")
 	plt.show()
 	if save_plot_name: fig.savefig(save_plot_name)
```

### Comparing `centerline-width-1.1.0/centerline_width/preprocessing.py` & `centerline-width-1.2.0/centerline_width/preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.1.0/centerline_width/pytests/test_centerline.py` & `centerline-width-1.2.0/centerline_width/pytests/test_saveOutput.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,14 @@
 
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal centerline-width reference to access functions, global variables, and error handling
 import centerline_width
 
-invalid_non_bool_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						("testing_string", "<class 'str'>")]
-
-invalid_non_class_options = [(1961, "<class 'int'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						("testing_string", "<class 'str'>"),
-						(False, "<class 'bool'>")]
-
-invalid_non_int_options = [("testing_string", "<class 'str'>"),
-						(3.1415, "<class 'float'>"),
-						([], "<class 'list'>"),
-						(False, "<class 'bool'>")]
-
 invalid_non_str_options = [(1961, "<class 'int'>"),
 						(3.1415, "<class 'float'>"),
 						([], "<class 'list'>"),
 						(False, "<class 'bool'>")]
 
 def river_class_object():
 	csv_example = StringIO()
@@ -37,92 +21,14 @@
 	csv_example.write("30.137581,-92.868569,30.037441,-92.867476\n")
 	csv_example.write("30.237581,-92.868569,30.037441,-92.867476\n")
 	csv_example.seek(0)
 	return centerline_width.riverCenterline(csv_data=csv_example)
 
 river_class_example = river_class_object()
 
-## riverWidthFromCenterlineCoordinates() #####################################################
-def test_riverWidthFromCenterline_riverObjectRequired(caplog):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)"
-
-@pytest.mark.parametrize("river_object_invalid, river_object_error_output", invalid_non_class_options)
-def test_riverWidthFromCenterline_riverObjectInvalidTypes(caplog, river_object_invalid, river_object_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_object_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Must be a river object (see: centerline_width.riverCenterline), current type = '{0}'".format(river_object_error_output)
-
-@pytest.mark.parametrize("transect_span_distance_invalid, transect_span_distance_error_output", invalid_non_int_options)
-def test_riverWidthFromCenterline_transectSpanDistanceInvalidTypes(caplog, transect_span_distance_invalid, transect_span_distance_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											transect_span_distance=transect_span_distance_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [transect_span_distance]: Must be a int, current type = '{0}'".format(transect_span_distance_error_output)
-
-@pytest.mark.parametrize("apply_smoothing_invalid, apply_smoothing_error_output", invalid_non_bool_options)
-def test_riverWidthFromCenterline_applySmoothingInvalidTypes(caplog, apply_smoothing_invalid, apply_smoothing_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											apply_smoothing=apply_smoothing_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [apply_smoothing]: Must be a bool, current type = '{0}'".format(apply_smoothing_error_output)
-
-@pytest.mark.parametrize("remove_intersections_invalid, remove_intersections_error_output", invalid_non_bool_options)
-def test_riverWidthFromCenterline_removeIntersectionsInvalidTypes(caplog, remove_intersections_invalid, remove_intersections_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											remove_intersections=remove_intersections_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(remove_intersections_error_output)
-
-@pytest.mark.parametrize("save_to_csv_invalid, save_to_csv_error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_saveToCSVInvalidTypes(caplog, save_to_csv_invalid, save_to_csv_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-											save_to_csv=save_to_csv_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(save_to_csv_error_output)
-
-def test_riverWidthFromCenterline_csvInvalidExtension(caplog):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-												save_to_csv="filename.txt")
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [save_to_csv]: Extension must be a .csv file, current extension = 'txt'"
-
-def test_riverWidthFromCenterline_coordinateTypeInvalidOption(caplog):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-										coordinate_type="Invalid Option")
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
-
-@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
-def test_riverWidthFromCenterline_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
-	with pytest.raises(SystemExit):
-		centerline_width.riverWidthFromCenterline(river_object=river_class_example,
-										coordinate_type=coordinate_type_name_invalid)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
-
-
 ## saveCenterlineCSV() #####################################################
 def test_saveCenterlineCSV_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineCSV(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [river_object]: Requires a river object (see: centerline_width.riverCenterline)"
@@ -176,32 +82,32 @@
 		centerline_width.saveCenterlineCSV(river_object=river_class_example,
 											save_to_csv="testing.csv",
 											centerline_type="not valid")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
 
-def test_saveCenterlineCSV_coordinateTypeInvalidOption(caplog):
+def test_saveCenterlineCSV_coordinateUnitInvalidOption(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineCSV(river_object=river_class_example,
 										save_to_csv="testing.csv",
-										coordinate_type="Invalid Option")
+										coordinate_unit="Invalid Option")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
 
-@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
-def test_saveCenterlineCSV_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+@pytest.mark.parametrize("coordinate_unit_name_invalid, coordinate_unit_error_output", invalid_non_str_options)
+def test_saveCenterlineCSV_coordinateTypeInvalidTypes(caplog, coordinate_unit_name_invalid, coordinate_unit_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineCSV(river_object=river_class_example,
 										save_to_csv="testing.csv",
-										coordinate_type=coordinate_type_name_invalid)
+										coordinate_unit=coordinate_unit_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(coordinate_unit_error_output)
 
 ## saveCenterlineMAT() #####################################################
 def test_saveCenterlineMAT_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineMAT(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
@@ -274,25 +180,25 @@
 		centerline_width.saveCenterlineMAT(river_object=river_class_example,
 											save_to_mat="testing.mat",
 											centerline_type="not valid")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [centerline_type]: Must be an available option in ['Voronoi', 'Evenly Spaced', 'Smoothed', 'Equal Distance'], current option = 'not valid'"
 
-def test_saveCenterlineMAT_coordinateTypeInvalidOption(caplog):
+def test_saveCenterlineMAT_coordinateUnitInvalidOption(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineMAT(river_object=river_class_example,
 										save_to_mat="testing.mat",
-										coordinate_type="Invalid Option")
+										coordinate_unit="Invalid Option")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
 
-@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
-def test_saveCenterlineMAT_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+@pytest.mark.parametrize("coordinate_unit_name_invalid, coordinate_unit_error_output", invalid_non_str_options)
+def test_saveCenterlineMAT_coordinateUnitInvalidTypes(caplog, coordinate_unit_name_invalid, coordinate_unit_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.saveCenterlineMAT(river_object=river_class_example,
 										save_to_mat="testing.mat",
-										coordinate_type=coordinate_type_name_invalid)
+										coordinate_unit=coordinate_unit_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(coordinate_unit_error_output)
```

### Comparing `centerline-width-1.1.0/centerline_width/pytests/test_getCoordinatesKML.py` & `centerline-width-1.2.0/centerline_width/pytests/test_getCoordinatesKML.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.1.0/centerline_width/pytests/test_plotDiagrams.py` & `centerline-width-1.2.0/centerline_width/pytests/test_plotDiagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,30 +133,30 @@
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_class_example,
 										display_voronoi=display_voronoi_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [display_voronoi]: Must be a bool, current type = '{0}'".format(display_voronoi_error_output)
 
-def test_plotCenterline_coordinateTypeInvalidOption(caplog):
+def test_plotCenterline_coordinateUnitInvalidOption(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_class_example,
-										coordinate_type="Invalid Option")
+										coordinate_unit="Invalid Option")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
 
-@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
-def test_plotCenterline_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+@pytest.mark.parametrize("coordinate_unit_name_invalid, coordinate_unit_error_output", invalid_non_str_options)
+def test_plotCenterline_coordinateUnitInvalidTypes(caplog, coordinate_unit_name_invalid, coordinate_unit_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterline(river_object=river_class_example,
-										coordinate_type=coordinate_type_name_invalid)
+										coordinate_unit=coordinate_unit_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(coordinate_unit_error_output)
 
 ## plotCenterlineWidth() #####################################################
 def test_plotCenterlineWidth_riverObjectRequired(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=None)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
@@ -229,23 +229,23 @@
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
 											remove_intersections=remove_intersections_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
 	assert log_record.message == "\nCRITICAL ERROR, [remove_intersections]: Must be a bool, current type = '{0}'".format(remove_intersections_error_output)
 
-def test_plotCenterlineWidth_coordinateTypeInvalidOption(caplog):
+def test_plotCenterlineWidth_coordinateUnitInvalidOption(caplog):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
-										coordinate_type="Invalid Option")
+										coordinate_unit="Invalid Option")
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be an available option in ['Decimal Degrees', 'Relative Distance'], current option = 'Invalid Option'"
 
-@pytest.mark.parametrize("coordinate_type_name_invalid, coordinate_type_error_output", invalid_non_str_options)
-def test_plotCenterlineWidth_coordinateTypeInvalidTypes(caplog, coordinate_type_name_invalid, coordinate_type_error_output):
+@pytest.mark.parametrize("coordinate_unit_name_invalid, coordinate_unit_error_output", invalid_non_str_options)
+def test_plotCenterlineWidth_coordinateUnitInvalidTypes(caplog, coordinate_unit_name_invalid, coordinate_unit_error_output):
 	with pytest.raises(SystemExit):
 		centerline_width.plotCenterlineWidth(river_object=river_class_example,
-										coordinate_type=coordinate_type_name_invalid)
+										coordinate_unit=coordinate_unit_name_invalid)
 	log_record = caplog.records[0]
 	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [coordinate_type]: Must be a str, current type = '{0}'".format(coordinate_type_error_output)
+	assert log_record.message == "\nCRITICAL ERROR, [coordinate_unit]: Must be a str, current type = '{0}'".format(coordinate_unit_error_output)
```

### Comparing `centerline-width-1.1.0/centerline_width/pytests/test_preprocessing.py` & `centerline-width-1.2.0/centerline_width/pytests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.1.0/centerline_width/pytests/test_riverCenterlineClass.py` & `centerline-width-1.2.0/centerline_width/pytests/test_riverCenterlineClass.py`

 * *Files identical despite different names*

### Comparing `centerline-width-1.1.0/centerline_width/relativeDistance.py` & `centerline-width-1.2.0/centerline_width/relativeDistance.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 	# Convert bank latitude/longtiude coordinates to relative coordinates
 	first_point = left_lon_lat_coordinates[0] # first point is the first point on the left bank
 
 	if left_lon_lat_coordinates is None or right_lon_lat_coordinates is None:
 		return None, None
 
 	left_relative_coordinates = []
-	for left_point in left_lon_lat_coordinates[1:]: # skip the bottom left most value
-		coord_pair = relativeSingleCoordinate(first_point, left_point, ellipsoid)
+	for left_point in left_lon_lat_coordinates:
+		if left_point == first_point:
+			coord_pair = (0.0, 0.0)
+		else:
+			coord_pair = relativeSingleCoordinate(first_point, left_point, ellipsoid)
 		left_relative_coordinates.append(coord_pair)
 
 	right_relative_coordinates = []
 	for right_point in right_lon_lat_coordinates:
 		coord_pair = relativeSingleCoordinate(first_point, right_point, ellipsoid)
 		right_relative_coordinates.append(coord_pair)
```

### Comparing `centerline-width-1.1.0/centerline_width/riverCenterlineClass.py` & `centerline-width-1.2.0/centerline_width/riverCenterlineClass.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,75 +107,75 @@
 						centerline_type="Voronoi",
 						marker_type="line",
 						centerline_color="black",
 						display_all_possible_paths=False,
 						plot_title=None,
 						save_plot_name=None,
 						display_voronoi=False,
-						coordinate_type="Decimal Degrees"):
+						coordinate_unit="Decimal Degrees"):
 		centerline_width.plotCenterline(river_object=self,
 										centerline_type=centerline_type,
 										marker_type=marker_type,
 										centerline_color=centerline_color,
 										display_all_possible_paths=display_all_possible_paths, 
 										plot_title=plot_title, 
 										save_plot_name=save_plot_name, 
 										display_voronoi=display_voronoi,
-										coordinate_type=coordinate_type)
+										coordinate_unit=coordinate_unit)
 
 	def plotCenterlineWidth(self,
 							plot_title=None, 
 							save_plot_name=None, 
 							display_true_centerline=True,
 							transect_span_distance=3,
 							apply_smoothing=False,
 							flag_intersections=True,
 							remove_intersections=False,
-							coordinate_type="Decimal Degrees"):
+							coordinate_unit="Decimal Degrees"):
 		centerline_width.plotCenterlineWidth(river_object=self,
 											plot_title=plot_title, 
 											save_plot_name=save_plot_name, 
 											display_true_centerline=display_true_centerline,
 											transect_span_distance=transect_span_distance,
 											apply_smoothing=apply_smoothing,
 											flag_intersections=flag_intersections,
 											remove_intersections=remove_intersections,
-											coordinate_type=coordinate_type)
+											coordinate_unit=coordinate_unit)
 
 	def riverWidthFromCenterline(self,
 								transect_span_distance=3,
 								apply_smoothing=True,
 								remove_intersections=False,
-								coordinate_type="Decimal Degrees",
+								coordinate_unit="Decimal Degrees",
 								save_to_csv=None):
 		return centerline_width.riverWidthFromCenterline(river_object=self,
 														transect_span_distance=transect_span_distance,
 														apply_smoothing=apply_smoothing,
 														remove_intersections=remove_intersections,
-														coordinate_type=coordinate_type,
+														coordinate_unit=coordinate_unit,
 														save_to_csv=save_to_csv)
 
 	def saveCenterlineCSV(self, 
 						save_to_csv=None,
 						latitude_header=None,
 						longitude_header=None, 
 						centerline_type="Voronoi",
-						coordinate_type="Decimal Degrees"):
+						coordinate_unit="Decimal Degrees"):
 		return centerline_width.saveCenterlineCSV(river_object=self,
 												save_to_csv=save_to_csv,
 												latitude_header=latitude_header, 
 												longitude_header=longitude_header, 
 												centerline_type=centerline_type,
-												coordinate_type=coordinate_type)
+												coordinate_unit=coordinate_unit)
 
 	def saveCenterlineMAT(self,
 						save_to_mat=None, 
 						latitude_header=None,
 						longitude_header=None, 
 						centerline_type="Voronoi",
-						coordinate_type="Decimal Degrees"):
+						coordinate_unit="Decimal Degrees"):
 		return centerline_width.saveCenterlineMAT(river_object=self,
 												save_to_mat=save_to_mat,
 												latitude_header=latitude_header,
 												longitude_header=longitude_header,
 												centerline_type=centerline_type,
-												coordinate_type=coordinate_type)
+												coordinate_unit=coordinate_unit)
```

### Comparing `centerline-width-1.1.0/centerline_width.egg-info/PKG-INFO` & `centerline-width-1.2.0/centerline_width.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: centerline-width
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank
 Home-page: https://github.com/cyschneck/centerline-width
 Author: Una Schneck (unaschneck), Cora Schneck (cyschneck)
 License: MIT
-Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.1.0.tar.gz
+Download-URL: https://github.com/cyschneck/centerline-width/archive/refs/tags/v1.2.0.tar.gz
 Description: # Centerline-Width
          <p align="center">
           <img src="https://raw.githubusercontent.com/cyschneck/centerline-width/main/assets/centerline_logo.jpg" />
         </p>
         
         ![PyPi](https://img.shields.io/pypi/v/centerline-width)
         ![license](https://img.shields.io/github/license/cyschneck/centerline-width)
@@ -71,28 +71,34 @@
         ```
         Then once the .csv file is created, in order to run the centerline-width functions, generate a river object from the `river_coordinates_output.csv`
         
         ```python
         river_object = centerline_width.riverCenterline(csv_data="river_coordinates_output.csv")
         ```
         
-        To plot the centerline, run the `plotCenterline()` function from `river_object` created
+        To plot the centerline, run the `plotCenterline()` function from `river_object` created. By default, will display with `Decimal Degrees` (latitude/longitude) coordinates
         ```python
         river_object.plotCenterline()
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_centerline.png)
         
         To plot the width of the river at intervals along the bank, run `plotCenterlineWidth`
         
         While `apply_smoothing`, `remove_intersections`, and `display_true_centerline` are optional, they are recommended to generate a minimal width diagram
         ```python
         river.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
         ```
         ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width.png)
         
+        It is possible to also display all the coordinates as a `Relative Distance`, where all the coordinates are converted to a relative distance (in meters) from the first point on the left bank
+        ```python
+        river_object.plotCenterline(coordinate_unit="Relative Distance")
+        ```
+        ![river_coords_centerline+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_relative_distance_coords_centerline.png)
+        
         For more details to fix unexpected behavior or error code: [Debugging, Error Handling, and Edge Cases](#debugging-error-handling-and-edge-cases)
         
         For a complete example script to run centerline-width: [centerline_width_example_script.py](https://github.com/cyschneck/centerline-width/blob/main/data/example_script_outputs/centerline_width_example_script.py) with [example outputs](https://github.com/cyschneck/centerline-width/tree/main/data/example_script_outputs)
         
         ## Preprocessing
         ### Generating KML files from Google Earth Pro
         Riverbanks can be defined here as the high-contrast boundary between active/recently-active flow and the surrounding landscape. We will be mapping the right and left bank separately
@@ -254,16 +260,16 @@
         * starting_node_relative (tuple): Tuple of the starting position (relative distance x and relative distance y) of the centerline path
         * ending_node (tuple): Tuple of the end position (latitude and longitude) of the centerline path
         * ending_node_relative (tuple): Tuple of the end position (relative distance x and relative distance y) of the centerline path
         * bank_voronoi (scipy Voronoi object): Voronoi generated by left/right banks of the latitude/longitude coordinate system
         * bank_voronoi_relative (scipy Voronoi object): Voronoi generated by left/right banks of the relative distance coordinate system
         * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Latitude position to ending Latitude position)
         * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Longitude position to ending Longitude position)
-        * x_voronoi_ridge_point (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
-        * y_voronoi_ridge_point (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
+        * x_voronoi_ridge_point_relative (list of tuples): X positions on Voronoi ridge (starting Relative Distance X position to ending Relative Distance X position)
+        * y_voronoi_ridge_point_relative (list of tuples): Y position on Voronoi ridge (starting Relative Distance Y position to ending Relative Distance Y position)
         * interpolate_data (boolean): if interpolating between existing data, defaults to False
         * interpolate_n (int): specifies how many additional points will be added between points along the riverbank when interpolating data, defaults to 5
         * interpolate_n_centerpoints (int): specifies how many points will be used to interpolate the Voronoi centerline, defaults to the length of the data frame (df_len)
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
@@ -327,42 +333,42 @@
         ```
         Output is a list of tuples: (example) `[(-92.86788596499872, 30.03786596717931), (-92.86789573751797, 30.037834641974108), (-92.8679141386283, 30.037789636848878), (-92.8679251193248, 30.037756853899904), (-92.86796903819089, 30.03765423778148), (-92.86797335733262, 30.037643336049054), (-92.8679920356456, 30.037592224469797), (-92.86800576063828, 30.037555441489403), (-92.86800841510367, 30.037546512833107), (-92.8680119498663, 30.03753043193875)]`
         
         ### Save Centerline Coordinates to a .CSV File
         Save the centerline coordinates to a csv file with columns for latitude and longitude. This is the file format for a table of (latitude,longitude) pairs accepted to import back into Google Earth Pro.
         
         ```
-        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+        saveCenterlineCSV(save_to_csv=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_csv (string): CSV filename, requires a .csv extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to CSV (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type> Centerline Latitude (Deg)` or `<centerline_type> Relative Distance Y (from Latitude) (m)`
         * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type> Centerline Longitude (Deg)` or `<centerline_type> Relative Distance X (from Longitude) (m)`
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineCSV(save_to_csv="centerline_coordinates.csv", centerline_type="Smoothed")
         ```
         Returns a csv with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed Centerline Latitude (Deg), Smoothed Centerline Longitude (Deg)`
         
         Note: it is best practice to plot the centerline with `plotCenterline()` to ensure that the results saved are as expected
         
         ### Save Centerline Coordinates to a .MAT File
         Save the centerline coordinates to a .mat file with columns for latitude and longitude
         
         ```
-        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_type="Decimal Degrees")
+        saveCenterlineMAT(save_to_mat=None, centerline_type="Voronoi", coordinate_unit="Decimal Degrees")
         ```
         * **[REQUIRED]** save_to_mat (string): MAT filename, requires a .mat extension
         * [OPTIONAL] centerline_type (string): Centerline type to save to MAT (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] latitude_header (string): Column header for latitude values, defaults to `<centerline_type>_Centerline_Latitude_(Deg)` or `<centerline_type>_Relative_Distance_Y_From_Latitude_m` (cannot include spaces or special characters)
         * [OPTIONAL] longitude_header (string): Column header for Longitude values, defaults to `<centerline_type>_Centerline_Longitude_(Deg)` or `<centerline_type>_Relative_Distance_X_From_Longitude_m` (cannot include spaces or special characters)
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.saveCenterlineMAT(save_to_mat="centerline_coordinates.mat", centerline_type="Smoothed")
         ```
         Returns a .mat file with the Latitude and Longitude coordinates of the specified centerline with column headers with centerline type: `Smoothed_Centerline_Latitude_(Deg), Smoothed_Centerline_Longitude_(Deg)`
@@ -389,24 +395,24 @@
         plotCenterline(centerline_type="Voronoi",
         		marker_type="line",
         		centerline_color="black",
         		display_all_possible_paths=False, 
         		plot_title=None, 
         		save_plot_name=None, 
         		display_voronoi=False,
-        		coordinate_type="Decimal Degrees")
+        		coordinate_unit="Decimal Degrees")
         ```
         * [OPTIONAL] centerline_type (string): Centerline type graph within river (not case-sensitive), options: ["Voronoi", "Evenly Spaced", "Smoothed", "Equal Distance"], defaults to "Voronoi"
         * [OPTIONAL] marker_type (string): Graph type (not case-sensitive), options: ["Line", "Scatter"], defaults to "Line"
         * [OPTIONAL] centerline_color (string): Color of centerline coordinates on graph (not case-sensitive), options: [matplotlib named colors](https://matplotlib.org/stable/gallery/color/named_colors.html), defaults to "black"
         * [OPTIONAL] display_all_possible_paths (boolean): Display all possible paths, not just the centerline (useful for debugging), defaults to False
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_voronoi (boolean): Overlay Voronoi diagram used to generate centerline, defaults to False
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterline()
         ```
         Output:
@@ -421,24 +427,24 @@
         plotCenterlineWidth(plot_title=None, 
         		save_plot_name=None, 
         		display_true_centerline=True,
         		transect_span_distance=3,
         		apply_smoothing=False,
         		flag_intersections=True,
         		remove_intersections=False,
-        		coordinate_type="Decimal Degrees")
+        		coordinate_unit="Decimal Degrees")
         ```
         * [OPTIONAL] plot_title (string): Change plot title, defaults to "River Coordinates: Valid Centerline = True/False, Valid Polygon = True/False"
         * [OPTIONAL] save_plot_name (string): Save the plot with a given name and location
         * [OPTIONAL] display_true_centerline (boolean): Display generated true centerline based on Voronoi diagrams
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] flag_intersections (boolean): Display intersecting width lines as red in graph, defaults to True
         * [OPTIONAL] remove_intersections (boolean): Remove intersecting lines (but maintain the most width lines as possible) and only return non-intersecting width lines, defaults to False
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         
         **apply_smoothing**
         
         apply_smoothing applies a spline to smooth the centerline points created by the Voronoi vertices. This reduces the noise of the slopes and can create width lines that are less susceptible to small changes in the bank
         
         | apply_smoothing=False | apply_smoothing=True |
         | ------------- | ------------- |
@@ -459,19 +465,19 @@
         
         Intersecting lines are flagged in red by default (flag_intersections=True)
         
         | remove_intersections=False | remove_intersections=True |
         | ------------- | ------------- |
         | ![river_keep+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_keep_intersections.png) | ![river_remove+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_remove_intersections.png)|
         
-        **coordinate_type**
+        **coordinate_unit**
         
         Two options for measuring and displaying coordinates. The two options are "Decimal Degrees" and "Relative Distance". "Decimal Degrees" is the default option that uses the original data coordinate system with latitude/longitude. "Relative Distance" changes the coordinates of each point to be the distance (in meters) from the first point on the left bank
         
-        | coordinate_type="Decimal Degrees" | remove_intersections="Relative Distance" |
+        | coordinate_unit="Decimal Degrees" | remove_intersections="Relative Distance" |
         | ------------- | ------------- |
         | ![dd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_decimal_degrees.png) | ![rd_coords+png](https://raw.githubusercontent.com/cyschneck/centerline-width/main/data/doc_examples/river_coords_width_relative_distance.png)|
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
         river_object.plotCenterlineWidth(apply_smoothing=True, remove_intersections=True, display_true_centerline=False)
@@ -482,21 +488,21 @@
         
         Return the width of the river at each (evenly spaced or smoothed) centerline coordinates as `(Longitude, Latitude) : width` in meters
         
         ```
         riverWidthFromCenterline(transect_span_distance=3,
         			apply_smoothing=True,
         			remove_intersections=False,
-        			coordinate_type="Decimal Degrees",
+        			coordinate_unit="Decimal Degrees",
         			save_to_csv=None)
         ```
         * [OPTIONAL] transect_span_distance (int): Sum up n number of points around a center point to determine the slope (increase to decrease the impact of sudden changes), defaults to 6, must be greater than 2 (since the slope is found from the difference in position between two points), measured orthogonal to the centerline
         * [OPTIONAL] apply_smoothing (boolean): Apply a B-spline smoothing to centerline
         * [OPTIONAL] remove_intersections (boolean): Iterative remove intersecting lines, to maintain the most width lines, but return only non-intersecting width lines, defaults to True
-        * [OPTIONAL] coordinate_type (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
+        * [OPTIONAL] coordinate_unit (string): Coordinates of the river are return as "Decimal Degrees" (latitude/longtidue) or converted to a distance from the first point on the left bank as "Relative Distance", defaults to "Decimal Degree"
         * [OPTIONAL] save_to_csv (string): CSV filename to output width, defaults to None (no file is saved), requires a .csv extension (Column Headers: `Centerline Latitude (Deg)", "Centerline Longitude (Deg)", "Width (km)`)
         
         Important note, when using `apply_smoothing=True`, the centerline generated is the result of evenly spaced coordinates generated from the original Voronoi coordinates, so the smoothed coordinates may not match exactly to the original centerline coordinates. When `apply_smoothing=False`, width lines are generated from the evenly spaced centerline coordinates
         
         ```python
         import centerline_width
         river_object = centerline_width.riverCenterline(csv_data="data/river_coords.csv")
```

### Comparing `centerline-width-1.1.0/centerline_width.egg-info/SOURCES.txt` & `centerline-width-1.2.0/centerline_width.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 centerline_width/centerline.py
 centerline_width/error_handling.py
 centerline_width/getCoordinatesKML.py
 centerline_width/plotDiagrams.py
 centerline_width/preprocessing.py
 centerline_width/relativeDistance.py
 centerline_width/riverCenterlineClass.py
+centerline_width/saveOutput.py
 centerline_width.egg-info/PKG-INFO
 centerline_width.egg-info/SOURCES.txt
 centerline_width.egg-info/dependency_links.txt
 centerline_width.egg-info/requires.txt
 centerline_width.egg-info/top_level.txt
 centerline_width/pytests/test_centerline.py
 centerline_width/pytests/test_getCoordinatesKML.py
 centerline_width/pytests/test_plotDiagrams.py
 centerline_width/pytests/test_preprocessing.py
-centerline_width/pytests/test_riverCenterlineClass.py
+centerline_width/pytests/test_riverCenterlineClass.py
+centerline_width/pytests/test_saveOutput.py
```

### Comparing `centerline-width-1.1.0/setup.py` & `centerline-width-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.1.0"
+VERSION="1.2.0"
 DESCRIPTION="A Python package to find the centerline and width of rivers based on the latitude and longitude of the right and left bank"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="centerline-width",
```

