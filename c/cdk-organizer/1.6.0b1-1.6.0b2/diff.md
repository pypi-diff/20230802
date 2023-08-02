# Comparing `tmp/cdk_organizer-1.6.0b1.tar.gz` & `tmp/cdk_organizer-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk_organizer-1.6.0b1.tar", max compression
+gzip compressed data, was "cdk_organizer-1.6.0b2.tar", max compression
```

## Comparing `cdk_organizer-1.6.0b1.tar` & `cdk_organizer-1.6.0b2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6748 2022-10-05 17:16:36.644081 cdk_organizer-1.6.0b1/README.md
--rw-r--r--   0        0        0      194 2022-09-09 12:39:05.760295 cdk_organizer-1.6.0b1/cdk_organizer/__init__.py
--rw-r--r--   0        0        0       22 2022-09-09 12:39:05.762815 cdk_organizer-1.6.0b1/cdk_organizer/aws/__init__.py
--rw-r--r--   0        0        0     1168 2022-09-09 12:39:05.764895 cdk_organizer-1.6.0b1/cdk_organizer/aws/stack.py
--rw-r--r--   0        0        0      509 2022-09-09 12:39:05.766124 cdk_organizer-1.6.0b1/cdk_organizer/aws/stack_group.py
--rw-r--r--   0        0        0       27 2022-09-09 12:39:05.766813 cdk_organizer-1.6.0b1/cdk_organizer/decorators/__init__.py
--rw-r--r--   0        0        0     1129 2022-09-09 12:39:05.768384 cdk_organizer-1.6.0b1/cdk_organizer/decorators/catch_exceptions.py
--rw-r--r--   0        0        0       22 2022-09-09 12:39:05.769040 cdk_organizer-1.6.0b1/cdk_organizer/loaders/__init__.py
--rw-r--r--   0        0        0     4058 2022-09-09 12:39:05.770652 cdk_organizer-1.6.0b1/cdk_organizer/loaders/config_loader.py
--rw-r--r--   0        0        0       28 2022-09-09 12:39:05.771365 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/__init__.py
--rw-r--r--   0        0        0     1652 2022-09-09 12:39:05.772921 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/logging.py
--rw-r--r--   0        0        0       31 2022-09-09 12:39:05.774140 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/__init__.py
--rw-r--r--   0        0        0     1111 2022-09-09 12:39:05.777863 cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py
--rw-r--r--   0        0        0     4834 2022-09-09 12:39:05.778749 cdk_organizer-1.6.0b1/cdk_organizer/stack.py
--rw-r--r--   0        0        0    12127 2023-06-02 22:04:03.712277 cdk_organizer-1.6.0b1/cdk_organizer/stack_group.py
--rw-r--r--   0        0        0       28 2022-09-09 12:39:05.780694 cdk_organizer-1.6.0b1/cdk_organizer/terraform/__init__.py
--rw-r--r--   0        0        0     1388 2022-09-13 21:00:59.686116 cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack.py
--rw-r--r--   0        0        0      519 2022-09-09 12:39:05.784357 cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack_group.py
--rw-r--r--   0        0        0     1095 2023-08-02 14:12:24.540866 cdk_organizer-1.6.0b1/pyproject.toml
--rw-r--r--   0        0        0     7482 1970-01-01 00:00:00.000000 cdk_organizer-1.6.0b1/PKG-INFO
+-rw-r--r--   0        0        0     6748 2022-10-05 17:16:36.644081 cdk_organizer-1.6.0b2/README.md
+-rw-r--r--   0        0        0      194 2022-09-09 12:39:05.760295 cdk_organizer-1.6.0b2/cdk_organizer/__init__.py
+-rw-r--r--   0        0        0       22 2022-09-09 12:39:05.762815 cdk_organizer-1.6.0b2/cdk_organizer/aws/__init__.py
+-rw-r--r--   0        0        0     1168 2022-09-09 12:39:05.764895 cdk_organizer-1.6.0b2/cdk_organizer/aws/stack.py
+-rw-r--r--   0        0        0      509 2022-09-09 12:39:05.766124 cdk_organizer-1.6.0b2/cdk_organizer/aws/stack_group.py
+-rw-r--r--   0        0        0       27 2022-09-09 12:39:05.766813 cdk_organizer-1.6.0b2/cdk_organizer/decorators/__init__.py
+-rw-r--r--   0        0        0     1129 2022-09-09 12:39:05.768384 cdk_organizer-1.6.0b2/cdk_organizer/decorators/catch_exceptions.py
+-rw-r--r--   0        0        0       22 2022-09-09 12:39:05.769040 cdk_organizer-1.6.0b2/cdk_organizer/loaders/__init__.py
+-rw-r--r--   0        0        0     4058 2022-09-09 12:39:05.770652 cdk_organizer-1.6.0b2/cdk_organizer/loaders/config_loader.py
+-rw-r--r--   0        0        0       28 2022-09-09 12:39:05.771365 cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/__init__.py
+-rw-r--r--   0        0        0     1652 2022-09-09 12:39:05.772921 cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/logging.py
+-rw-r--r--   0        0        0       31 2022-09-09 12:39:05.774140 cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/yaml_tags/__init__.py
+-rw-r--r--   0        0        0     1111 2022-09-09 12:39:05.777863 cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py
+-rw-r--r--   0        0        0     4834 2022-09-09 12:39:05.778749 cdk_organizer-1.6.0b2/cdk_organizer/stack.py
+-rw-r--r--   0        0        0    12127 2023-06-02 22:04:03.712277 cdk_organizer-1.6.0b2/cdk_organizer/stack_group.py
+-rw-r--r--   0        0        0       28 2022-09-09 12:39:05.780694 cdk_organizer-1.6.0b2/cdk_organizer/terraform/__init__.py
+-rw-r--r--   0        0        0     1388 2022-09-13 21:00:59.686116 cdk_organizer-1.6.0b2/cdk_organizer/terraform/stack.py
+-rw-r--r--   0        0        0      519 2022-09-09 12:39:05.784357 cdk_organizer-1.6.0b2/cdk_organizer/terraform/stack_group.py
+-rw-r--r--   0        0        0     1094 2023-08-02 14:19:40.768788 cdk_organizer-1.6.0b2/pyproject.toml
+-rw-r--r--   0        0        0     7481 1970-01-01 00:00:00.000000 cdk_organizer-1.6.0b2/PKG-INFO
```

### Comparing `cdk_organizer-1.6.0b1/README.md` & `cdk_organizer-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/aws/stack.py` & `cdk_organizer-1.6.0b2/cdk_organizer/aws/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/decorators/catch_exceptions.py` & `cdk_organizer-1.6.0b2/cdk_organizer/decorators/catch_exceptions.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/loaders/config_loader.py` & `cdk_organizer-1.6.0b2/cdk_organizer/loaders/config_loader.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/logging.py` & `cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/logging.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py` & `cdk_organizer-1.6.0b2/cdk_organizer/miscellaneous/yaml_tags/merge_yaml.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/stack.py` & `cdk_organizer-1.6.0b2/cdk_organizer/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/stack_group.py` & `cdk_organizer-1.6.0b2/cdk_organizer/stack_group.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack.py` & `cdk_organizer-1.6.0b2/cdk_organizer/terraform/stack.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/cdk_organizer/terraform/stack_group.py` & `cdk_organizer-1.6.0b2/cdk_organizer/terraform/stack_group.py`

 * *Files identical despite different names*

### Comparing `cdk_organizer-1.6.0b1/pyproject.toml` & `cdk_organizer-1.6.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 show_missing = true
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-fail-under=100 --cov-report html:'../../coverage/packages/framework-python/html' --cov-report xml:'../../coverage/packages/framework-python/coverage.xml' --junitxml='../../reports/packages/framework-python/unittests/junit.xml' --html='../../reports/packages/framework-python/unittests/html/index.html'"
 
 [tool.poetry]
 name = "cdk-organizer"
-version = "1.6.0b1"
+version = "1.6.0b2"
 description = "CDK Organizer"
 authors = [ ]
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "cdk_organizer"
 
   [tool.poetry.dependencies]
-  python = ">=3.7,<=3.10"
+  python = ">=3.7,<3.11"
   PyYAML = "^6.0"
   dacite = "^1.6.0"
   pyhumps = "^3.7.2"
   constructs = "^10.1.49"
   cdktf = { version = "^0.15.0", optional = true }
   "aws-cdk-lib" = { version = "^2.32.1", optional = true }
```

### Comparing `cdk_organizer-1.6.0b1/PKG-INFO` & `cdk_organizer-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cdk-organizer
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: CDK Organizer
-Requires-Python: >=3.7,<=3.10
+Requires-Python: >=3.7,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: aws
 Provides-Extra: terraform
```

