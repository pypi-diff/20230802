# Comparing `tmp/SliceCommander-0.1.post2.tar.gz` & `tmp/SliceCommander-0.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SliceCommander-0.1.post2.tar", last modified: Wed Aug  2 20:00:04 2023, max compression
+gzip compressed data, was "SliceCommander-0.1.post3.tar", last modified: Wed Aug  2 20:02:44 2023, max compression
```

## Comparing `SliceCommander-0.1.post2.tar` & `SliceCommander-0.1.post3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2023-08-02 19:58:53.000000 SliceCommander-0.1.post2/LICENSE
--rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2023-08-02 19:58:57.000000 SliceCommander-0.1.post2/MANIFEST.in
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1060 2022-12-20 19:23:00.000000 SliceCommander-0.1.post2/README.md
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/SliceCommander.egg-info/
--rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/PKG-INFO
--rw-r--r--   0 ezra      (1000) ezra      (1000)      380 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/SOURCES.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/dependency_links.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       55 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/entry_points.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/requires.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       10 2023-08-02 20:00:04.000000 SliceCommander-0.1.post2/SliceCommander.egg-info/top_level.txt
-drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/commander/
--rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/__init__.py
--rwxr-xr-x   0 ezra      (1000) ezra      (1000)    15746 2023-08-02 19:42:52.000000 SliceCommander-0.1.post2/commander/cli.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)      865 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/spinner.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2565 2023-08-02 17:06:40.000000 SliceCommander-0.1.post2/commander/ssh.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2970 2022-12-19 19:11:09.000000 SliceCommander-0.1.post2/commander/util.py
--rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 19:54:26.000000 SliceCommander-0.1.post2/requirements.txt
--rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-08-02 20:00:04.577834 SliceCommander-0.1.post2/setup.cfg
--rw-r--r--   0 ezra      (1000) ezra      (1000)     2650 2023-08-02 19:56:14.000000 SliceCommander-0.1.post2/setup.py
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:02:44.853000 SliceCommander-0.1.post3/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1513 2023-08-02 19:58:53.000000 SliceCommander-0.1.post3/LICENSE
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       41 2023-08-02 19:58:57.000000 SliceCommander-0.1.post3/MANIFEST.in
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:02:44.853000 SliceCommander-0.1.post3/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1060 2022-12-20 19:23:00.000000 SliceCommander-0.1.post3/README.md
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:02:44.853000 SliceCommander-0.1.post3/SliceCommander.egg-info/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     1609 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/PKG-INFO
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      380 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/SOURCES.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        1 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/dependency_links.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       55 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/entry_points.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/requires.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       10 2023-08-02 20:02:44.000000 SliceCommander-0.1.post3/SliceCommander.egg-info/top_level.txt
+drwxr-xr-x   0 ezra      (1000) ezra      (1000)        0 2023-08-02 20:02:44.853000 SliceCommander-0.1.post3/commander/
+-rw-r--r--   0 ezra      (1000) ezra      (1000)        0 2022-12-19 19:11:09.000000 SliceCommander-0.1.post3/commander/__init__.py
+-rwxr-xr-x   0 ezra      (1000) ezra      (1000)    15746 2023-08-02 19:42:52.000000 SliceCommander-0.1.post3/commander/cli.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)      865 2022-12-19 19:11:09.000000 SliceCommander-0.1.post3/commander/spinner.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2565 2023-08-02 17:06:40.000000 SliceCommander-0.1.post3/commander/ssh.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2970 2022-12-19 19:11:09.000000 SliceCommander-0.1.post3/commander/util.py
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       67 2023-08-02 19:54:26.000000 SliceCommander-0.1.post3/requirements.txt
+-rw-r--r--   0 ezra      (1000) ezra      (1000)       38 2023-08-02 20:02:44.853000 SliceCommander-0.1.post3/setup.cfg
+-rw-r--r--   0 ezra      (1000) ezra      (1000)     2650 2023-08-02 20:02:09.000000 SliceCommander-0.1.post3/setup.py
```

### Comparing `SliceCommander-0.1.post2/LICENSE` & `SliceCommander-0.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/PKG-INFO` & `SliceCommander-0.1.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: SliceCommander
-Version: 0.1.post2
+Version: 0.1.post3
 Summary: FABRIC Slice Commander
 Home-page: https://github.com/fabric-testbed/slice-commander
 Author: Ezra Kissel
 Keywords: fabric slice command
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SliceCommander
 Tool for manipulating FABRIC slices on the command line.
```

### Comparing `SliceCommander-0.1.post2/README.md` & `SliceCommander-0.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/SliceCommander.egg-info/PKG-INFO` & `SliceCommander-0.1.post3/SliceCommander.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: SliceCommander
-Version: 0.1.post2
+Version: 0.1.post3
 Summary: FABRIC Slice Commander
 Home-page: https://github.com/fabric-testbed/slice-commander
 Author: Ezra Kissel
 Keywords: fabric slice command
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SliceCommander
 Tool for manipulating FABRIC slices on the command line.
```

### Comparing `SliceCommander-0.1.post2/commander/cli.py` & `SliceCommander-0.1.post3/commander/cli.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/commander/spinner.py` & `SliceCommander-0.1.post3/commander/spinner.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/commander/ssh.py` & `SliceCommander-0.1.post3/commander/ssh.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/commander/util.py` & `SliceCommander-0.1.post3/commander/util.py`

 * *Files identical despite different names*

### Comparing `SliceCommander-0.1.post2/setup.py` & `SliceCommander-0.1.post3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,25 +37,25 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fh:
     requirements = fh.read()
 
 setup(
     name='SliceCommander',
-    version='0.1-post2',
+    version='0.1-post3',
     description='FABRIC Slice Commander',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/fabric-testbed/slice-commander',
     author='Ezra Kissel',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
-        'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: BSD License',
         'Programming Language :: Python :: 3',
     ],
     keywords='fabric slice command',
     packages=find_packages(),
     setup_requires=requirements,
     install_requires=requirements,
     entry_points = {
```

