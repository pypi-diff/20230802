# Comparing `tmp/magnetocaloric-1.2.1.tar.gz` & `tmp/magnetocaloric-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnetocaloric-1.2.1.tar", last modified: Mon Jul 31 06:25:36 2023, max compression
+gzip compressed data, was "magnetocaloric-1.2.2.tar", last modified: Wed Aug  2 12:17:55 2023, max compression
```

## Comparing `magnetocaloric-1.2.1.tar` & `magnetocaloric-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/
--rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.1/Licence.txt
--rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3969 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3222 2023-07-31 06:24:49.000000 magnetocaloric-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.565530 magnetocaloric-1.2.1/magnetocaloric/
--rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.1/magnetocaloric/Color_marker.py
--rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.1/magnetocaloric/M_H_reshaping.py
--rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.1/magnetocaloric/RCP_plot.py
--rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.1/magnetocaloric/T_FWHM_RCP.py
--rw-rw-rw-   0        0        0      831 2023-07-30 12:08:19.000000 magnetocaloric-1.2.1/magnetocaloric/__init__.py
--rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.1/magnetocaloric/arrott_plot.py
--rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.1/magnetocaloric/collect_from_database.py
--rw-rw-rw-   0        0        0     5564 2023-07-31 06:14:23.000000 magnetocaloric-1.2.1/magnetocaloric/data_visualization.py
--rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.1/magnetocaloric/entropy_change01.py
--rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.1/magnetocaloric/entropy_change02.py
--rw-rw-rw-   0        0        0     3943 2023-07-31 06:24:52.000000 magnetocaloric-1.2.1/magnetocaloric/mcepy.py
--rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.1/magnetocaloric/modified_arrott_plot.py
--rw-rw-rw-   0        0        0     2164 2023-07-30 11:39:58.000000 magnetocaloric-1.2.1/magnetocaloric/store_to_database.py
--rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.1/magnetocaloric/take_temp.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/magnetocaloric.egg-info/
--rw-rw-rw-   0        0        0     3969 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-31 06:25:36.000000 magnetocaloric-1.2.1/magnetocaloric.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 06:25:36.596790 magnetocaloric-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1180 2023-07-31 06:24:46.000000 magnetocaloric-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/
+-rw-rw-rw-   0        0        0       84 2022-04-14 07:58:46.000000 magnetocaloric-1.2.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1057 2023-07-27 08:24:00.000000 magnetocaloric-1.2.2/Licence.txt
+-rw-rw-rw-   0        0        0       81 2022-04-14 07:58:45.000000 magnetocaloric-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3969 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3222 2023-08-02 12:16:03.000000 magnetocaloric-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.122312 magnetocaloric-1.2.2/magnetocaloric/
+-rw-rw-rw-   0        0        0      560 2023-07-31 06:14:28.000000 magnetocaloric-1.2.2/magnetocaloric/Color_marker.py
+-rw-rw-rw-   0        0        0     1397 2023-07-30 11:40:32.000000 magnetocaloric-1.2.2/magnetocaloric/M_H_reshaping.py
+-rw-rw-rw-   0        0        0     2059 2023-07-30 11:43:59.000000 magnetocaloric-1.2.2/magnetocaloric/RCP_plot.py
+-rw-rw-rw-   0        0        0     3548 2023-07-30 11:43:19.000000 magnetocaloric-1.2.2/magnetocaloric/T_FWHM_RCP.py
+-rw-rw-rw-   0        0        0      831 2023-07-30 12:08:19.000000 magnetocaloric-1.2.2/magnetocaloric/__init__.py
+-rw-rw-rw-   0        0        0     1487 2023-07-30 11:41:26.000000 magnetocaloric-1.2.2/magnetocaloric/arrott_plot.py
+-rw-rw-rw-   0        0        0     1424 2023-07-30 11:37:12.000000 magnetocaloric-1.2.2/magnetocaloric/collect_from_database.py
+-rw-rw-rw-   0        0        0     5564 2023-07-31 06:14:23.000000 magnetocaloric-1.2.2/magnetocaloric/data_visualization.py
+-rw-rw-rw-   0        0        0     2433 2023-07-31 06:15:05.000000 magnetocaloric-1.2.2/magnetocaloric/entropy_change01.py
+-rw-rw-rw-   0        0        0     1229 2023-07-30 11:38:43.000000 magnetocaloric-1.2.2/magnetocaloric/entropy_change02.py
+-rw-rw-rw-   0        0        0     5644 2023-08-02 12:12:35.000000 magnetocaloric-1.2.2/magnetocaloric/mcepy.py
+-rw-rw-rw-   0        0        0     2434 2023-07-30 11:42:47.000000 magnetocaloric-1.2.2/magnetocaloric/modified_arrott_plot.py
+-rw-rw-rw-   0        0        0     2164 2023-07-30 11:39:58.000000 magnetocaloric-1.2.2/magnetocaloric/store_to_database.py
+-rw-rw-rw-   0        0        0      930 2023-07-30 11:36:24.000000 magnetocaloric-1.2.2/magnetocaloric/take_temp.py
+drwxrwxrwx   0        0        0        0 2023-08-02 12:17:55.137944 magnetocaloric-1.2.2/magnetocaloric.egg-info/
+-rw-rw-rw-   0        0        0     3969 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-02 12:17:54.000000 magnetocaloric-1.2.2/magnetocaloric.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 12:17:55.153573 magnetocaloric-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1190 2023-08-02 12:15:29.000000 magnetocaloric-1.2.2/setup.py
```

### Comparing `magnetocaloric-1.2.1/Licence.txt` & `magnetocaloric-1.2.2/Licence.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/PKG-INFO` & `magnetocaloric-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.1
+Version: 1.2.2
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.1
+# magnetocaloric 1.2.2
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.1
+ pip install magnetocaloric==1.2.2
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.1/README.md` & `magnetocaloric-1.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# magnetocaloric 1.2.1
+# magnetocaloric 1.2.2
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -21,15 +21,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.1
+ pip install magnetocaloric==1.2.2
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.1/magnetocaloric/Color_marker.py` & `magnetocaloric-1.2.2/magnetocaloric/Color_marker.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/M_H_reshaping.py` & `magnetocaloric-1.2.2/magnetocaloric/M_H_reshaping.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/RCP_plot.py` & `magnetocaloric-1.2.2/magnetocaloric/RCP_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/T_FWHM_RCP.py` & `magnetocaloric-1.2.2/magnetocaloric/T_FWHM_RCP.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/__init__.py` & `magnetocaloric-1.2.2/magnetocaloric/__init__.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/arrott_plot.py` & `magnetocaloric-1.2.2/magnetocaloric/arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/collect_from_database.py` & `magnetocaloric-1.2.2/magnetocaloric/collect_from_database.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/data_visualization.py` & `magnetocaloric-1.2.2/magnetocaloric/data_visualization.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/entropy_change01.py` & `magnetocaloric-1.2.2/magnetocaloric/entropy_change01.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/entropy_change02.py` & `magnetocaloric-1.2.2/magnetocaloric/entropy_change02.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/modified_arrott_plot.py` & `magnetocaloric-1.2.2/magnetocaloric/modified_arrott_plot.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/store_to_database.py` & `magnetocaloric-1.2.2/magnetocaloric/store_to_database.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric/take_temp.py` & `magnetocaloric-1.2.2/magnetocaloric/take_temp.py`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/magnetocaloric.egg-info/PKG-INFO` & `magnetocaloric-1.2.2/magnetocaloric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnetocaloric
-Version: 1.2.1
+Version: 1.2.2
 Summary: Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python
 Home-page: https://github.com/supratimdasinfo/Magnetocaloric-Effect
 Author: Supratim Das
 Author-email: supratim0707@gmail.com
 License: MIT
 Keywords: magnetocaloric,mcepy,magnetic,programming,code,python,supratim,das,bhaskar,biswas,physics
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,15 +12,15 @@
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: Licence.txt
 
 
-# magnetocaloric 1.2.1
+# magnetocaloric 1.2.2
 #### Developed by Supratim Das
 
 ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?)
 
 Effective approach to determine magnetocaloric performance of any magnetic material using python programming. From isotherm M(H) curves, using the Maxwell Relation the magnetocaloric performance of a material can be calculated with the help of this module.
 
 ## What's New
@@ -38,15 +38,15 @@
 
 ### 1. Installation 
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install magnetocaloric package.
 
 ```bash
 
- pip install magnetocaloric==1.2.1
+ pip install magnetocaloric==1.2.2
 
 ```
 ### 2. Manage Excel Spreadsheet
 -  Check the main excel spreadsheet from where the M-H data will be fetched by the program, data must be arranged in this format given below. 
 
 ![](https://raw.githubusercontent.com/supratimdasinfo/magnetocaloric.mcepy/main/Screenshot%20(229).png?raw=True)
```

### Comparing `magnetocaloric-1.2.1/magnetocaloric.egg-info/SOURCES.txt` & `magnetocaloric-1.2.2/magnetocaloric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magnetocaloric-1.2.1/setup.py` & `magnetocaloric-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='magnetocaloric',
-  version='1.2.1',
+  version='1.2.2',
   description='Effective Approach To Calculate Magnetocaloric Effect Of Any Magnetic Material Using Python',
   long_description=long_description,
   long_description_content_type="text/markdown",
   url='https://github.com/supratimdasinfo/Magnetocaloric-Effect',  
   author='Supratim Das',
   author_email='supratim0707@gmail.com',
   license='MIT', 
   classifiers=classifiers,
   keywords=['magnetocaloric', 'mcepy', 'magnetic', 'programming', 'code', 'python','supratim', 'das', 'bhaskar', 'biswas', 'physics'],
   include_package_data=True, 
   packages=['magnetocaloric'],
-  install_requires=['num2words', 'matplotlib','xlrd==1.2.0','openpyxl','tableprint','XlsxWriter','numpy'] 
+  install_requires=['num2words', 'matplotlib','xlrd==1.2.0','openpyxl','tableprint','XlsxWriter','numpy', 'bcrypt'] 
 )
```

