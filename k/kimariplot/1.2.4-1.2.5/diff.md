# Comparing `tmp/kimariplot-1.2.4.tar.gz` & `tmp/kimariplot-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.2.4.tar", last modified: Wed Aug  2 16:49:41 2023, max compression
+gzip compressed data, was "kimariplot-1.2.5.tar", last modified: Wed Aug  2 16:50:55 2023, max compression
```

## Comparing `kimariplot-1.2.4.tar` & `kimariplot-1.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 16:49:41.716515 kimariplot-1.2.4/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.4/LICENSE
--rw-rw-rw-   0        0        0     4398 2023-08-02 16:49:41.664046 kimariplot-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 16:49:41.654044 kimariplot-1.2.4/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.4/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     9494 2023-08-02 16:48:12.000000 kimariplot-1.2.4/kimariplot/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-02 16:49:41.662043 kimariplot-1.2.4/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-08-02 16:49:41.000000 kimariplot-1.2.4/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-02 16:49:41.000000 kimariplot-1.2.4/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 16:49:41.000000 kimariplot-1.2.4/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-08-02 16:49:41.000000 kimariplot-1.2.4/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-02 16:49:41.000000 kimariplot-1.2.4/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 16:49:41.717267 kimariplot-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-08-02 13:25:55.000000 kimariplot-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.960501 kimariplot-1.2.5/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0     4398 2023-08-02 16:50:55.960501 kimariplot-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.946605 kimariplot-1.2.5/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.5/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     9452 2023-08-02 16:50:29.000000 kimariplot-1.2.5/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:50:55.958502 kimariplot-1.2.5/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 16:50:55.000000 kimariplot-1.2.5/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 16:50:55.961536 kimariplot-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-02 16:50:29.000000 kimariplot-1.2.5/setup.py
```

### Comparing `kimariplot-1.2.4/LICENSE` & `kimariplot-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.4/PKG-INFO` & `kimariplot-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.4
+Version: 1.2.5
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.4/README.md` & `kimariplot-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.4/kimariplot/plotter.py` & `kimariplot-1.2.5/kimariplot/plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     except Exception as e:
         raise Exception(f"An error occurred while plotting the graph: {e}")
 
 
 def main():
     # 定义版本信息
     version_info = {
-        'version': 'v1.2.4',
+        'version': 'v1.2.5',
         'release_date': 'Aug-3-2023',
         'developer': 'Kimariyb, Ryan Hsiun',
         'address': 'XiaMen University, School of Electronic Science and Engineering',
         'website': 'https://github.com/kimariyb/kimariPlot',
     }
 
     # 创建 ArgumentParser 对象
@@ -233,10 +233,7 @@
     now = datetime.datetime.now().strftime("%b-%d-%Y, 00:45:%S")
     # 程序结束后提示版权信息和问候语
     print(f"Thank you for using our plotting tool! Have a great day!")
     print("Copyright © 2023 Kimariyb. All rights reserved.")
     print(f"Currently timeline: {now}")
     print("============================================================================")
 
-
-if __name__ == '__main__':
-    main()
```

### Comparing `kimariplot-1.2.4/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.2.5/kimariplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.4
+Version: 1.2.5
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.4/setup.py` & `kimariplot-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.2.4",
+    version="1.2.5",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
```

