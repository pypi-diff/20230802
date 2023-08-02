# Comparing `tmp/qiskit-classroom-converter-0.0.4.tar.gz` & `tmp/qiskit-classroom-converter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.0.4.tar", last modified: Wed Aug  2 12:19:44 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.0.5.tar", last modified: Wed Aug  2 13:21:26 2023, max compression
```

## Comparing `qiskit-classroom-converter-0.0.4.tar` & `qiskit-classroom-converter-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.049006 qiskit-classroom-converter-0.0.4/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)       36 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.4/MANIFEST.in
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 12:19:44.049226 qiskit-classroom-converter-0.0.4/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.4/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1233 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/pyproject.toml
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.042342 qiskit-classroom-converter-0.0.4/qiskit_class_converter/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2761 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.045564 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/base.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3679 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/braket_notation_to_matrix.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.046549 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.048717 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      206 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      126 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/requirements.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-08-02 12:19:44.049706 qiskit-classroom-converter-0.0.4/setup.cfg
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.678543 qiskit-classroom-converter-0.0.5/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.5/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       59 2023-08-02 12:35:39.000000 qiskit-classroom-converter-0.0.5/MANIFEST.in
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 13:21:26.678673 qiskit-classroom-converter-0.0.5/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.5/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1233 2023-08-02 13:10:51.000000 qiskit-classroom-converter-0.0.5/pyproject.toml
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.673936 qiskit-classroom-converter-0.0.5/qiskit_class_converter/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2166 2023-08-02 13:10:51.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.676072 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3679 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/braket_notation_to_matrix.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.676655 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-08-02 12:36:25.000000 qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 13:21:26.678270 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      206 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-08-02 13:21:26.000000 qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      126 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.5/requirements.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-08-02 13:21:26.679100 qiskit-classroom-converter-0.0.5/setup.cfg
```

### Comparing `qiskit-classroom-converter-0.0.4/LICENSE` & `qiskit-classroom-converter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/PKG-INFO` & `qiskit-classroom-converter-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.4
+Version: 0.0.5
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.4/README.md` & `qiskit-classroom-converter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/pyproject.toml` & `qiskit-classroom-converter-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools.packages.find]
 include = ['qiskit_class_converter*']
 exclude = ['qiskit_class_converter*tests']
 
 [project]
 name = "qiskit-classroom-converter"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "KMU-quantum-classroom" },
 ]
 description = "extend the Qiskit classroom applications."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/braket_notation_to_matrix.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/braket_notation_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/matrix_to_quantum_circuit.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_matrix.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/converters/quantum_circuit_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.0.5/qiskit_class_converter/services/converter_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.4
+Version: 0.0.5
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.0.5/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

