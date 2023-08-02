# Comparing `tmp/terragrunt-generator-0.6.5.tar.gz` & `tmp/terragrunt-generator-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.6.5.tar", last modified: Tue Aug  1 20:25:50 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.6.6.tar", last modified: Wed Aug  2 16:25:35 2023, max compression
```

## Comparing `terragrunt-generator-0.6.5.tar` & `terragrunt-generator-0.6.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 20:25:38.000000 terragrunt-generator-0.6.5/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-01 20:25:38.000000 terragrunt-generator-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21326 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 20:25:50.000000 terragrunt-generator-0.6.5/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:50.156776 terragrunt-generator-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-01 20:25:27.000000 terragrunt-generator-0.6.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.964164 terragrunt-generator-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21241 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-02 16:25:23.000000 terragrunt-generator-0.6.6/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-02 16:25:23.000000 terragrunt-generator-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:25:35.964164 terragrunt-generator-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21492 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:25:35.000000 terragrunt-generator-0.6.6/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:35.960163 terragrunt-generator-0.6.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-02 16:25:13.000000 terragrunt-generator-0.6.6/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.6.5/COPYING` & `terragrunt-generator-0.6.6/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.5/PKG-INFO` & `terragrunt-generator-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.5
+Version: 0.6.6
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
 # terragrunt-generator
 
+[![codecov](https://codecov.io/gh/goabonga/terragrunt-generator/branch/main/graph/badge.svg?token=LZYOP61FF7)](https://codecov.io/gh/goabonga/terragrunt-generator)
+
+
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
 - python3.6+
```

### Comparing `terragrunt-generator-0.6.5/README.md` & `terragrunt-generator-0.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # terragrunt-generator
 
+[![codecov](https://codecov.io/gh/goabonga/terragrunt-generator/branch/main/graph/badge.svg?token=LZYOP61FF7)](https://codecov.io/gh/goabonga/terragrunt-generator)
+
+
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
 - python3.6+
```

### Comparing `terragrunt-generator-0.6.5/generator/generate.py` & `terragrunt-generator-0.6.6/generator/generate.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.5/generator/main.py` & `terragrunt-generator-0.6.6/generator/main.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.5/pyproject.toml` & `terragrunt-generator-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.5"
+version = "0.6.6"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.6.5/setup.py` & `terragrunt-generator-0.6.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     author_email='goabonga@pm.me',
     description='generate terragrunt manifest from terraform module.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'python-hcl2==3.0.5',
-        'GitPython==3.1.27',
+        'GitPython==3.1.30',
     ],
     extras_require={
         'dev': [
             'pytest==7.1.3',
+            'pytest-cov==4.1.0',
             'black==23.3.0',
             'isort==5.12.0',
             'commitizen==2.42.1',
             'flake8==6.0.0',
             'pre-commit==3.2.2',
         ]
     },
```

### Comparing `terragrunt-generator-0.6.5/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt-generator-0.6.6/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.6.5
+Version: 0.6.6
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
 
 # terragrunt-generator
 
+[![codecov](https://codecov.io/gh/goabonga/terragrunt-generator/branch/main/graph/badge.svg?token=LZYOP61FF7)](https://codecov.io/gh/goabonga/terragrunt-generator)
+
+
 **terragrunt-generator** provide a way to generate a ```terragrunt.hcl``` file with documented inputs who's coming from variables exposed by terraform module.
 
 The result is easily configurable with a **yaml** file.
 ## Requirements
 
 - python3.6+
```

### Comparing `terragrunt-generator-0.6.5/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.6.6/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.5/tests/test_generate.py` & `terragrunt-generator-0.6.6/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.6.5/tests/test_reader.py` & `terragrunt-generator-0.6.6/tests/test_reader.py`

 * *Files identical despite different names*

