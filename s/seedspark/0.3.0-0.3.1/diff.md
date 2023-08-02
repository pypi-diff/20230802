# Comparing `tmp/seedspark-0.3.0.tar.gz` & `tmp/seedspark-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedspark-0.3.0.tar", max compression
+gzip compressed data, was "seedspark-0.3.1.tar", max compression
```

## Comparing `seedspark-0.3.0.tar` & `seedspark-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0     2621 2023-06-04 17:57:38.018059 seedspark-0.3.0/README.MD
--rw-r--r--   0        0        0     4175 2023-08-02 09:48:09.974418 seedspark-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/__init__.py
--rw-r--r--   0        0        0       93 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/configs/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/configs/configs.py
--rw-r--r--   0        0        0      118 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/__init__.py
--rw-r--r--   0        0        0      212 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/__init__.py
--rw-r--r--   0        0        0     3361 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/base_airflow_test.py
--rw-r--r--   0        0        0     6639 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/base_spark_test.py
--rw-r--r--   0        0        0      110 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/ge.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/service.py
--rw-r--r--   0        0        0      215 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/spark/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/spark/dataframe/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/__init__.py
--rw-r--r--   0        0        0    17049 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/df_compare.py
--rw-r--r--   0        0        0     9456 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/schema_comparer.py
--rw-r--r--   0        0        0     2338 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/utils.py
--rw-r--r--   0        0        0      150 2023-08-02 09:40:36.654423 seedspark-0.3.0/seedspark/spark/db/__init__.py
--rw-r--r--   0        0        0     7786 2023-08-02 09:40:36.654423 seedspark-0.3.0/seedspark/spark/sparkapp.py
--rw-r--r--   0        0        0      100 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/__init__.py
--rw-r--r--   0        0        0     2989 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/_datetime.py
--rw-r--r--   0        0        0     1719 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/json.py
--rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 seedspark-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2621 2023-06-04 17:57:38.018059 seedspark-0.3.1/README.MD
+-rw-r--r--   0        0        0     4175 2023-08-02 15:43:52.475086 seedspark-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/__init__.py
+-rw-r--r--   0        0        0       93 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/configs/__init__.py
+-rw-r--r--   0        0        0     1173 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/configs/configs.py
+-rw-r--r--   0        0        0      118 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/contrib/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/contrib/test/__init__.py
+-rw-r--r--   0        0        0     3361 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/contrib/test/base_airflow_test.py
+-rw-r--r--   0        0        0     6639 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/contrib/test/base_spark_test.py
+-rw-r--r--   0        0        0      110 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/dataquality/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/dataquality/ge.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/dataquality/service.py
+-rw-r--r--   0        0        0      774 2023-08-02 15:43:52.475086 seedspark-0.3.1/seedspark/spark/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.1/seedspark/spark/dataframe/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/spark/dataframe/compare/__init__.py
+-rw-r--r--   0        0        0    17049 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/spark/dataframe/compare/df_compare.py
+-rw-r--r--   0        0        0     9456 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/spark/dataframe/compare/schema_comparer.py
+-rw-r--r--   0        0        0     2338 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/spark/dataframe/utils.py
+-rw-r--r--   0        0        0       24 2023-08-02 15:43:52.475086 seedspark-0.3.1/seedspark/spark/db/__init__.py
+-rw-r--r--   0        0        0     3494 2023-08-02 15:43:52.475086 seedspark-0.3.1/seedspark/spark/db/onetl.py
+-rw-r--r--   0        0        0     7786 2023-08-02 09:40:36.654423 seedspark-0.3.1/seedspark/spark/sparkapp.py
+-rw-r--r--   0        0        0      100 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/utils/__init__.py
+-rw-r--r--   0        0        0     2989 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/utils/_datetime.py
+-rw-r--r--   0        0        0     1719 2023-06-04 17:57:38.028059 seedspark-0.3.1/seedspark/utils/json.py
+-rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 seedspark-0.3.1/PKG-INFO
```

### Comparing `seedspark-0.3.0/README.MD` & `seedspark-0.3.1/README.MD`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/pyproject.toml` & `seedspark-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seedspark"
-version = "0.3.0"
+version = "0.3.1"
 description = "SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments"
 authors = ["ChethanUK <chethanuk@outlook.com>"]
 maintainers = ["ChethanUK <chethanuk@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.MD"
 homepage = "https://github.com/ChethanUK/"
 repository = "https://github.com/ChethanUK/seedspark"
```

### Comparing `seedspark-0.3.0/seedspark/configs/configs.py` & `seedspark-0.3.1/seedspark/configs/configs.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/contrib/test/base_airflow_test.py` & `seedspark-0.3.1/seedspark/contrib/test/base_airflow_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/contrib/test/base_spark_test.py` & `seedspark-0.3.1/seedspark/contrib/test/base_spark_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/dataquality/ge.py` & `seedspark-0.3.1/seedspark/dataquality/ge.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/spark/dataframe/compare/df_compare.py` & `seedspark-0.3.1/seedspark/spark/dataframe/compare/df_compare.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/spark/dataframe/compare/schema_comparer.py` & `seedspark-0.3.1/seedspark/spark/dataframe/compare/schema_comparer.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/spark/dataframe/utils.py` & `seedspark-0.3.1/seedspark/spark/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/spark/sparkapp.py` & `seedspark-0.3.1/seedspark/spark/sparkapp.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/utils/_datetime.py` & `seedspark-0.3.1/seedspark/utils/_datetime.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/seedspark/utils/json.py` & `seedspark-0.3.1/seedspark/utils/json.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.3.0/PKG-INFO` & `seedspark-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedspark
-Version: 0.3.0
+Version: 0.3.1
 Summary: SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments
 Home-page: https://github.com/ChethanUK/
 License: Apache-2.0
 Keywords: PySpark,data-ops,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers,data-engineer,best-practices,big-data
 Author: ChethanUK
 Author-email: chethanuk@outlook.com
 Maintainer: ChethanUK
```

