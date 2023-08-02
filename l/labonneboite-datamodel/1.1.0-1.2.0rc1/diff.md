# Comparing `tmp/labonneboite_datamodel-1.1.0.tar.gz` & `tmp/labonneboite_datamodel-1.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labonneboite_datamodel-1.1.0.tar", max compression
+gzip compressed data, was "labonneboite_datamodel-1.2.0rc1.tar", max compression
```

## Comparing `labonneboite_datamodel-1.1.0.tar` & `labonneboite_datamodel-1.2.0rc1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      240 2023-06-08 16:40:46.304772 labonneboite_datamodel-1.1.0/labonneboite_datamodel/__init__.py
--rw-r--r--   0        0        0      941 2023-06-29 04:35:09.561863 labonneboite_datamodel-1.1.0/labonneboite_datamodel/base.py
--rw-r--r--   0        0        0     2945 2023-06-08 16:40:46.304772 labonneboite_datamodel-1.1.0/labonneboite_datamodel/job.py
--rw-r--r--   0        0        0     7718 2023-06-08 16:40:46.304772 labonneboite_datamodel-1.1.0/labonneboite_datamodel/office.py
--rw-r--r--   0        0        0        0 2023-06-08 16:40:46.304772 labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/__init__.py
--rw-r--r--   0        0        0     3589 2023-06-08 16:40:46.304772 labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/data/test.csv
--rw-r--r--   0        0        0      449 2023-06-29 04:35:09.561863 labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/test_base.py
--rw-r--r--   0        0        0     1271 2023-06-29 04:35:09.561863 labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/test_job.py
--rw-r--r--   0        0        0     4814 2023-06-29 04:35:09.561863 labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/test_office.py
--rw-r--r--   0        0        0     1282 2023-06-29 04:36:44.083097 labonneboite_datamodel-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      299 2023-08-02 10:21:55.951567 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/__init__.py
+-rw-r--r--   0        0        0      941 2023-06-29 04:34:33.625392 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/base.py
+-rw-r--r--   0        0        0     2945 2023-06-08 16:40:14.792338 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/job.py
+-rw-r--r--   0        0        0     7843 2023-07-13 13:03:26.312464 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/office.py
+-rw-r--r--   0        0        0     1328 2023-08-02 10:21:55.951567 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/rome.py
+-rw-r--r--   0        0        0        0 2023-04-04 13:24:31.560952 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/__init__.py
+-rw-r--r--   0        0        0     3589 2023-04-06 09:30:27.400471 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/data/test.csv
+-rw-r--r--   0        0        0      449 2023-06-29 04:34:33.625392 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_base.py
+-rw-r--r--   0        0        0     1271 2023-06-29 04:34:33.625392 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_job.py
+-rw-r--r--   0        0        0     4814 2023-06-29 04:34:33.625392 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_office.py
+-rw-r--r--   0        0        0     1343 2023-08-02 10:21:55.951567 labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_rome.py
+-rw-r--r--   0        0        0     1287 2023-08-02 10:40:41.657285 labonneboite_datamodel-1.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 labonneboite_datamodel-1.2.0rc1/PKG-INFO
```

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/base.py` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/base.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/job.py` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/job.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/office.py` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/office.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,19 @@
         street: Street name of the company. (Optional)
         postcode: Postal code of the city where the company is, this may not be unique in France. (Optional)
         citycode: INSEE code of the city where the company is, this may is unique in France. (Optional)
         email: Email of the branch company. (Optional)
         phone: Phone of the branch company. (Optional)
         website: Website of the branch / main company. (Optional)
         headcount_range: Number of employees in the branch company. (Optional)
-        flag_pmsmp:
-        flag_poe_afpr:
-        flag_junior:
-        flag_senior:
-        flag_handicap:
+        flag_pmsmp: To be removed (Optional)
+        flag_poe_afpr: To be removed (Optional)
+        flag_junior: To be removed (Optional)
+        flag_senior: To be removed (Optional)
+        flag_handicap: To be removed (Optional)
     """
 
     naf: str
     company_name: str
     office_name: str
     streetnumber: str = Field(default="", nullable=True)
     street: str = Field(default="", nullable=True)
```

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/data/test.csv` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/data/test.csv`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/test_job.py` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.1.0/labonneboite_datamodel/tests/test_office.py` & `labonneboite_datamodel-1.2.0rc1/labonneboite_datamodel/tests/test_office.py`

 * *Files identical despite different names*

### Comparing `labonneboite_datamodel-1.1.0/pyproject.toml` & `labonneboite_datamodel-1.2.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "labonneboite-datamodel"
-version = "1.1.0"
+version = "1.2.0-rc.1"
 description = "Datamodel for labonneboite"
 authors = ["Sylvain Touret"]
 license = "MIT"
 packages = [{include = "labonneboite_datamodel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

