# Comparing `tmp/seedspark-0.1.9.tar.gz` & `tmp/seedspark-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seedspark-0.1.9.tar", max compression
+gzip compressed data, was "seedspark-0.3.0.tar", max compression
```

## Comparing `seedspark-0.1.9.tar` & `seedspark-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     2621 2023-06-04 17:57:38.018059 seedspark-0.1.9/README.MD
--rw-r--r--   0        0        0     3941 2023-06-04 17:59:22.668079 seedspark-0.1.9/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/__init__.py
--rw-r--r--   0        0        0       93 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/configs/__init__.py
--rw-r--r--   0        0        0     1173 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/configs/configs.py
--rw-r--r--   0        0        0      118 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/__init__.py
--rw-r--r--   0        0        0      212 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/__init__.py
--rw-r--r--   0        0        0     3361 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/base_airflow_test.py
--rw-r--r--   0        0        0     6639 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/contrib/test/base_spark_test.py
--rw-r--r--   0        0        0      110 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/ge.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/dataquality/service.py
--rw-r--r--   0        0        0      215 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/spark/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.1.9/seedspark/spark/dataframe/__init__.py
--rw-r--r--   0        0        0        0 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/__init__.py
--rw-r--r--   0        0        0    17049 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/df_compare.py
--rw-r--r--   0        0        0     9456 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/compare/schema_comparer.py
--rw-r--r--   0        0        0     2338 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/dataframe/utils.py
--rw-r--r--   0        0        0     7924 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/spark/sparkapp.py
--rw-r--r--   0        0        0      100 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/__init__.py
--rw-r--r--   0        0        0     2989 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/_datetime.py
--rw-r--r--   0        0        0     1719 2023-06-04 17:57:38.028059 seedspark-0.1.9/seedspark/utils/json.py
--rw-r--r--   0        0        0     4163 1970-01-01 00:00:00.000000 seedspark-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2621 2023-06-04 17:57:38.018059 seedspark-0.3.0/README.MD
+-rw-r--r--   0        0        0     4175 2023-08-02 09:48:09.974418 seedspark-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/__init__.py
+-rw-r--r--   0        0        0       93 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/configs/__init__.py
+-rw-r--r--   0        0        0     1173 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/configs/configs.py
+-rw-r--r--   0        0        0      118 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/__init__.py
+-rw-r--r--   0        0        0     3361 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/base_airflow_test.py
+-rw-r--r--   0        0        0     6639 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/contrib/test/base_spark_test.py
+-rw-r--r--   0        0        0      110 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/ge.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/dataquality/service.py
+-rw-r--r--   0        0        0      215 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/spark/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.018059 seedspark-0.3.0/seedspark/spark/dataframe/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/__init__.py
+-rw-r--r--   0        0        0    17049 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/df_compare.py
+-rw-r--r--   0        0        0     9456 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/compare/schema_comparer.py
+-rw-r--r--   0        0        0     2338 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/spark/dataframe/utils.py
+-rw-r--r--   0        0        0      150 2023-08-02 09:40:36.654423 seedspark-0.3.0/seedspark/spark/db/__init__.py
+-rw-r--r--   0        0        0     7786 2023-08-02 09:40:36.654423 seedspark-0.3.0/seedspark/spark/sparkapp.py
+-rw-r--r--   0        0        0      100 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/__init__.py
+-rw-r--r--   0        0        0     2989 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/_datetime.py
+-rw-r--r--   0        0        0     1719 2023-06-04 17:57:38.028059 seedspark-0.3.0/seedspark/utils/json.py
+-rw-r--r--   0        0        0     4349 1970-01-01 00:00:00.000000 seedspark-0.3.0/PKG-INFO
```

### Comparing `seedspark-0.1.9/README.MD` & `seedspark-0.3.0/README.MD`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/pyproject.toml` & `seedspark-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seedspark"
-version = "0.1.9"
+version = "0.3.0"
 description = "SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments"
 authors = ["ChethanUK <chethanuk@outlook.com>"]
 maintainers = ["ChethanUK <chethanuk@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.MD"
 homepage = "https://github.com/ChethanUK/"
 repository = "https://github.com/ChethanUK/seedspark"
@@ -26,28 +26,34 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",    
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Software Development :: Testing"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 pyspark = { version = ">=2.4.7", extras = ["sql"], optional = true }
 pyarrow = { version = ">=2.0.0", optional = true }  # "^4.0.1"
 lognub = "^0.1.3"
+pytest-postgresql = {version = "^5.0.0", optional = true}
+onetl = {version = "^0.8.1", extras = ["s3"], optional = true}
+sqlglot = {version = "^17.8.0", optional = true}
+
+[tool.poetry.extras]
+database = ["onetl", "sqlglot", "pytest-postgresql"]
+spark = ["pyspark", "onetl"]
 
 [tool.poetry.dev-dependencies]
 pytest-lazy-fixture = "^0.6.3"
 pytest-ordering = "^0.6"
 pytest-tldr = "^0.2.4"
 pytest-picked = "^0.4.6"
 pytest-instafail = "^0.4.2"
```

### Comparing `seedspark-0.1.9/seedspark/configs/configs.py` & `seedspark-0.3.0/seedspark/configs/configs.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/contrib/test/base_airflow_test.py` & `seedspark-0.3.0/seedspark/contrib/test/base_airflow_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/contrib/test/base_spark_test.py` & `seedspark-0.3.0/seedspark/contrib/test/base_spark_test.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/dataquality/ge.py` & `seedspark-0.3.0/seedspark/dataquality/ge.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/spark/dataframe/compare/df_compare.py` & `seedspark-0.3.0/seedspark/spark/dataframe/compare/df_compare.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/spark/dataframe/compare/schema_comparer.py` & `seedspark-0.3.0/seedspark/spark/dataframe/compare/schema_comparer.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/spark/dataframe/utils.py` & `seedspark-0.3.0/seedspark/spark/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/spark/sparkapp.py` & `seedspark-0.3.0/seedspark/spark/sparkapp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 import copy
+from abc import ABC, abstractmethod
 from dataclasses import field
 from typing import Any, Dict, List, Tuple
 
 # Import Logger object
 from lognub import log
 from pyspark import SparkConf, SparkContext
 from pyspark.sql import SparkSession
 
 
-class SparkApps:
+class SparkApps(ABC):
     spark = None
     sc = None
 
     def __init__(
         self,
         app_name: str,
         extra_configs: Dict[Any, Any] = None,
@@ -38,39 +39,36 @@
         # spark.sql.inMemorycolumnarStorage.compressed
         # spark.sql.sources.partitionColumnTypeInference.enabled
         # spark.sql.parquet.mergeSchema
         # spark.sql.extensions
 
         _base_spark_conf = (
             SparkConf()
-            .set("spark.ui.showConsoleProgress", "false")
             .set("spark.ui.enabled", "true")
             .set("spark.network.timeout", "1200000")
             .set("spark.rpc.numRetries", "20")
-            .set("spark.dynamicAllocation.enabled", "true")
             .set("spark.task.maxFailures", "100")
             .set("spark.cleaner.periodicGC.interval", "1min")
             .set("spark.unsafe.exceptionOnMemoryLeak", "true")
             .set("spark.sql.broadcastTimeout", "3600")  # SQL
-            .set("spark.sql.shuffle.partitions", "10")
+            .set("spark.dynamicAllocation.enabled", "true")
             .set("spark.sql.parquet.filterPushdown", "true")
             .set("spark.sql.parquet.recordLevelFilter.enabled", "true")
-            .set("spark.sql.session.timeZone", "Asia/Kolkata")
             .set("spark.sql.adaptive.enabled", "true")
             .set("spark.sql.optimizer.nestedSchemaPruning.enabled", "true")
             .set("spark.sql.optimizer.dynamicPartitionPruning", "true")
             .set("spark.sql.optimizer.dynamicPartitionPruning", "true")
             .set("spark.sql.ansi.enabled", "true")
             .set("spark.sql.cbo.enabled", "true")
             .set("spark.sql.hive.metastorePartitionPruning", "true")
             .set("spark.sql.execution.arrow.pyspark.enabled", "true")  # Arrow
-            .set("spark.sql.execution.arrow.maxRecordsPerBatch", "50000")
-            .set("spark.sql.execution.arrow.pyspark.maxRecordsPerBatch", "50000")
             .set("spark.sql.execution.arrow.pyspark.fallback.enabled", "true")
             .set("spark.sql.execution.pandas.convertToArrowArraySafely", "true")
+            .set("spark.sql.execution.arrow.maxRecordsPerBatch", "50000")
+            .set("spark.sql.execution.arrow.pyspark.maxRecordsPerBatch", "50000")
         )
 
         return _base_spark_conf
 
     @staticmethod
     def _py4j_logger(sc: SparkContext):
         log4j_logger = sc._jvm.org.apache.log4j  # pylint: disable=W0212
@@ -168,17 +166,17 @@
         java_version = subprocess.check_output(["java", "-version"], stderr=subprocess.STDOUT)
         log.info(f"Java Version: {java_version}")
         import pkg_resources
 
         installed_packages_list = sorted([f"{i.key}=={i.version}" for i in pkg_resources.working_set])
         log.info(f"installed_packages_list: {installed_packages_list}")
 
-    # @abstractmethod
-    # def execute(self):
-    #     raise SparkAppsException("No Implementation has found for init()", NotImplementedError)
+    @abstractmethod
+    def execute(self):
+        raise SparkAppsException("No Implementation has found for execute()", NotImplementedError)
 
 
 class SparkAppsException(Exception):
     """
     SparkAppsException Common base class for all non-exit EasySpark exceptions
 
     Parameters
```

### Comparing `seedspark-0.1.9/seedspark/utils/_datetime.py` & `seedspark-0.3.0/seedspark/utils/_datetime.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/seedspark/utils/json.py` & `seedspark-0.3.0/seedspark/utils/json.py`

 * *Files identical despite different names*

### Comparing `seedspark-0.1.9/PKG-INFO` & `seedspark-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seedspark
-Version: 0.1.9
+Version: 0.3.0
 Summary: SeedSpark is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments
 Home-page: https://github.com/ChethanUK/
 License: Apache-2.0
 Keywords: PySpark,data-ops,data-engineering,data-quality,data-profiling,dataquality,dataunittest,data-unit-tests,data-profilers,data-engineer,best-practices,big-data
 Author: ChethanUK
 Author-email: chethanuk@outlook.com
 Maintainer: ChethanUK
@@ -17,20 +17,23 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Testing
+Provides-Extra: database
+Provides-Extra: spark
 Requires-Dist: lognub (>=0.1.3,<0.2.0)
+Requires-Dist: onetl[s3] (>=0.8.1,<0.9.0) ; extra == "database" or extra == "spark"
 Requires-Dist: pyarrow (>=2.0.0)
-Requires-Dist: pyspark[sql] (>=2.4.7)
+Requires-Dist: pyspark[sql] (>=2.4.7) ; extra == "spark"
+Requires-Dist: pytest-postgresql (>=5.0.0,<6.0.0) ; extra == "database"
+Requires-Dist: sqlglot (>=17.8.0,<18.0.0) ; extra == "database"
 Project-URL: Documentation, https://github.com/ChethanUK/seedspark#readme
 Project-URL: Repository, https://github.com/ChethanUK/seedspark
 Description-Content-Type: text/plain
 
 # SeedSpark
 
 **SeedSpark** is an open-source is an Extensible PySpark utility package to create production spark pipelines and dev-test them in dev environments or to perform end to end tests. The goal is to enable rapid development of Spark pipelines via PySpark on Spark clusters and locally test the pipeline by using various utilities.
```

