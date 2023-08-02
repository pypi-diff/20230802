# Comparing `tmp/chartart-0.0.3.dev21.tar.gz` & `tmp/chartart-0.0.3.dev22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartart-0.0.3.dev21.tar", last modified: Fri Jul 28 13:06:56 2023, max compression
+gzip compressed data, was "chartart-0.0.3.dev22.tar", last modified: Wed Aug  2 08:13:58 2023, max compression
```

## Comparing `chartart-0.0.3.dev21.tar` & `chartart-0.0.3.dev22.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.704010 chartart-0.0.3.dev21/
--rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/LICENSE
--rw-r--r--   0 dhananjay   (504) staff       (20)     2788 2023-07-28 13:06:56.704252 chartart-0.0.3.dev21/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)     2266 2023-07-28 13:05:48.000000 chartart-0.0.3.dev21/README.md
--rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/pyproject.toml
--rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-07-28 13:06:56.705463 chartart-0.0.3.dev21/setup.cfg
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.682018 chartart-0.0.3.dev21/src/
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.693149 chartart-0.0.3.dev21/src/chartart/
--rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/conftest.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/helpers.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    87504 2023-07-28 13:01:20.000000 chartart-0.0.3.dev21/src/chartart/plot.py
--rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/simple_eda_template.py
--rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/test_plot.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.702185 chartart-0.0.3.dev21/src/chartart/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/tests/__init__.py
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/src/chartart/tests/test_simple.py
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.699994 chartart-0.0.3.dev21/src/chartart.egg-info/
--rw-r--r--   0 dhananjay   (504) staff       (20)     2788 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/PKG-INFO
--rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/requires.txt
--rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-07-28 13:06:56.000000 chartart-0.0.3.dev21/src/chartart.egg-info/top_level.txt
-drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-07-28 13:06:56.703091 chartart-0.0.3.dev21/tests/
--rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev21/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.988657 chartart-0.0.3.dev22/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1059 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/LICENSE
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2846 2023-08-02 08:13:58.989050 chartart-0.0.3.dev22/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2324 2023-08-02 08:12:46.000000 chartart-0.0.3.dev22/README.md
+-rw-r--r--   0 dhananjay   (504) staff       (20)      103 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/pyproject.toml
+-rw-r--r--   0 dhananjay   (504) staff       (20)      714 2023-08-02 08:13:58.991735 chartart-0.0.3.dev22/setup.cfg
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.936402 chartart-0.0.3.dev22/src/
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.959720 chartart-0.0.3.dev22/src/chartart/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      577 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     1923 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/conftest.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2402 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/helpers.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    87470 2023-08-02 06:55:51.000000 chartart-0.0.3.dev22/src/chartart/plot.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2088 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/simple_eda_template.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)    47684 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/test_plot.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.983384 chartart-0.0.3.dev22/src/chartart/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      208 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/tests/__init__.py
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/src/chartart/tests/test_simple.py
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.980856 chartart-0.0.3.dev22/src/chartart.egg-info/
+-rw-r--r--   0 dhananjay   (504) staff       (20)     2846 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjay   (504) staff       (20)      464 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        1 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)       41 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/requires.txt
+-rw-r--r--   0 dhananjay   (504) staff       (20)        9 2023-08-02 08:13:58.000000 chartart-0.0.3.dev22/src/chartart.egg-info/top_level.txt
+drwxr-xr-x   0 dhananjay   (504) staff       (20)        0 2023-08-02 08:13:58.987207 chartart-0.0.3.dev22/tests/
+-rw-r--r--   0 dhananjay   (504) staff       (20)      417 2023-03-28 07:08:28.000000 chartart-0.0.3.dev22/tests/test_simple.py
```

### Comparing `chartart-0.0.3.dev21/LICENSE` & `chartart-0.0.3.dev22/LICENSE`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/PKG-INFO` & `chartart-0.0.3.dev22/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: chartart
-Version: 0.0.3.dev21
-Summary: ChartArt python package
-Home-page: https://github.com/pypa/sampleproject
-Author: BR-Advisers
-Author-email: info@br-advisers.com
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Keywords: chartart,NLP
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChartArt Package is under development
 
 Use 
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 Change Log 
@@ -83,7 +67,10 @@
 - Made default bin interval is 0 . 0 means syncfusion will calculate internally.
 
 0.0.3.dev20
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
 
 - 0.0.3.dev21
 Fix for communicate with Jupyter kernel
+
+- 0.0.3.dev22
+Fix for setting axis type on figure object
```

### Comparing `chartart-0.0.3.dev21/setup.cfg` & `chartart-0.0.3.dev22/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chartart
-version = 0.0.3.dev21
+version = 0.0.3.dev22
 author = BR-Advisers
 author_email = info@br-advisers.com
 description = ChartArt python package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `chartart-0.0.3.dev21/src/chartart/__init__.py` & `chartart-0.0.3.dev22/src/chartart/__init__.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/src/chartart/conftest.py` & `chartart-0.0.3.dev22/src/chartart/conftest.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/src/chartart/helpers.py` & `chartart-0.0.3.dev22/src/chartart/helpers.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/src/chartart/plot.py` & `chartart-0.0.3.dev22/src/chartart/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
     
     def set_xAxisType(self, xAxisType: str):
          """
          Used to override axis type internally decided by library. Flow : create Figure create chart and then set axis type. 
          Usefull in case of bar/column chart where seris is numeric but to look better in zoom we will make it catagorical.
          :param xAxisType  numeric OR datetime OR category/categorical OR datetimeCategory OR logarithmic
          """
-         self.xAxisProperties['xAxisType'] = xAxisType
+         self.x_axis_type = xAxisType
 
     def set_yAxisMaximum(self, yAxisMaximum: Union[int, float, str]):
          self.yAxisProperties['maximum'] = yAxisMaximum
 
     def set_yAxisMinimum(self, yAxisMinimum: Union[int, float, str]):
          self.yAxisProperties['minimum'] = yAxisMinimum
 
@@ -388,15 +388,15 @@
 
     def set_yAxisType(self, yAxisType: str):
          """
          Used to override axis type internally decided by library. Flow : create Figure create chart and then set axis type. 
          Usefull in case of bar/column chart where seris is numeric but to look better in zoom we will make it catagorical.
          :param xAxisType  numeric OR datetime OR category/categorical OR datetimeCategory OR logarithmic
          """
-         self.yAxisProperties['yAxisType'] = yAxisType
+         self.y_axis_type = yAxisType
 
     def set_annotation(self, htmlText: str, x: Optional[Union[int, float, str]] = None, y: Optional[Union[int, float, str]] = None, radius: Optional[str] = None):
         """
         Use this method to add annotation on cartesian or circular chart
         Call this method multiple times to add multiple annotations
         :param htmlText: Annotation content in the form of html text
         :param x: x axis % or value in case of cartesian chart
```

### Comparing `chartart-0.0.3.dev21/src/chartart/simple_eda_template.py` & `chartart-0.0.3.dev22/src/chartart/simple_eda_template.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/src/chartart/test_plot.py` & `chartart-0.0.3.dev22/src/chartart/test_plot.py`

 * *Files identical despite different names*

### Comparing `chartart-0.0.3.dev21/src/chartart.egg-info/PKG-INFO` & `chartart-0.0.3.dev22/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartart
-Version: 0.0.3.dev21
+Version: 0.0.3.dev22
 Summary: ChartArt python package
 Home-page: https://github.com/pypa/sampleproject
 Author: BR-Advisers
 Author-email: info@br-advisers.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: chartart,NLP
 Classifier: Programming Language :: Python :: 3
@@ -83,7 +83,10 @@
 - Made default bin interval is 0 . 0 means syncfusion will calculate internally.
 
 0.0.3.dev20
 - preview and previewPost url should route should start with /  e.g  earlier http://localhost:port/#preview  now http://localhost:port/#/preview
 
 - 0.0.3.dev21
 Fix for communicate with Jupyter kernel
+
+- 0.0.3.dev22
+Fix for setting axis type on figure object
```

