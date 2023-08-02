# Comparing `tmp/gender_definer-0.0.2.tar.gz` & `tmp/gender_definer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gender_definer-0.0.2.tar", max compression
+gzip compressed data, was "gender_definer-0.0.3.tar", max compression
```

## Comparing `gender_definer-0.0.2.tar` & `gender_definer-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      480 2023-08-02 13:23:49.235691 gender_definer-0.0.2/README.md
--rw-r--r--   0        0        0       58 2023-08-02 13:12:25.895358 gender_definer-0.0.2/genderdefiner/__init__.py
--rw-r--r--   0        0        0      106 2023-08-02 12:44:32.946817 gender_definer-0.0.2/genderdefiner/enums.py
--rw-r--r--   0        0        0     1574 2023-08-02 13:22:48.274818 gender_definer-0.0.2/genderdefiner/genderdefiner.py
--rw-r--r--   0        0        0      149 2023-08-02 12:47:32.506558 gender_definer-0.0.2/genderdefiner/types.py
--rw-r--r--   0        0        0      435 2023-08-02 16:36:12.286406 gender_definer-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 gender_definer-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      475 2023-08-02 16:48:34.614710 gender_definer-0.0.3/README.md
+-rw-r--r--   0        0        0       58 2023-08-02 13:12:25.895358 gender_definer-0.0.3/genderdefiner/__init__.py
+-rw-r--r--   0        0        0      106 2023-08-02 12:44:32.946817 gender_definer-0.0.3/genderdefiner/enums.py
+-rw-r--r--   0        0        0     1574 2023-08-02 13:22:48.274818 gender_definer-0.0.3/genderdefiner/genderdefiner.py
+-rw-r--r--   0        0        0      149 2023-08-02 12:47:32.506558 gender_definer-0.0.3/genderdefiner/types.py
+-rw-r--r--   0        0        0      435 2023-08-02 16:49:24.861923 gender_definer-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 gender_definer-0.0.3/PKG-INFO
```

### Comparing `gender_definer-0.0.2/genderdefiner/genderdefiner.py` & `gender_definer-0.0.3/genderdefiner/genderdefiner.py`

 * *Files identical despite different names*

### Comparing `gender_definer-0.0.2/PKG-INFO` & `gender_definer-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gender-definer
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python packege for define a gender by cyrillic and latin names
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,16 @@
 ```
 
 ### Example
 
 ```python
 from genderdefiner import GenderDefiner
 
-definer = GenderDefiner()
+gd = GenderDefiner()
 
-print(definer.define('Юля'))
+print(gd.define('Юля'))
 
-# output
+# output:
+#
 # SubjectGender(gender='female', probability=0.7646426652337452)
+#
 ```
```

