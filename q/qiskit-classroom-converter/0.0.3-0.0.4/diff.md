# Comparing `tmp/qiskit-classroom-converter-0.0.3.tar.gz` & `tmp/qiskit-classroom-converter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-classroom-converter-0.0.3.tar", last modified: Mon Jul 31 10:46:27 2023, max compression
+gzip compressed data, was "qiskit-classroom-converter-0.0.4.tar", last modified: Wed Aug  2 12:19:44 2023, max compression
```

## Comparing `qiskit-classroom-converter-0.0.3.tar` & `qiskit-classroom-converter-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.009857 qiskit-classroom-converter-0.0.3/
--rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/LICENSE
--rw-r--r--   0 minwook-shin   (501) staff       (20)       36 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.3/MANIFEST.in
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-31 10:46:27.010008 qiskit-classroom-converter-0.0.3/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.3/README.md
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1188 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.3/pyproject.toml
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.002976 qiskit-classroom-converter-0.0.3/qiskit_class_converter/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1653 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/__init__.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.006780 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/base.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     3710 2023-07-28 05:39:05.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/braket_notation_to_matrix.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.007692 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/
--rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/__init__.py
--rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/converter_service.py
-drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-07-31 10:46:27.009588 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/
--rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/PKG-INFO
--rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/SOURCES.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/dependency_links.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)      165 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/requires.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-07-31 10:46:26.000000 qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/top_level.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       88 2023-07-30 00:19:08.000000 qiskit-classroom-converter-0.0.3/requirements.txt
--rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-07-31 10:46:27.010441 qiskit-classroom-converter-0.0.3/setup.cfg
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.049006 qiskit-classroom-converter-0.0.4/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)    11350 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/LICENSE
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       36 2023-07-31 10:43:34.000000 qiskit-classroom-converter-0.0.4/MANIFEST.in
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 12:19:44.049226 qiskit-classroom-converter-0.0.4/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1958 2023-07-28 06:54:58.000000 qiskit-classroom-converter-0.0.4/README.md
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1233 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/pyproject.toml
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.042342 qiskit-classroom-converter-0.0.4/qiskit_class_converter/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2761 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/__init__.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.045564 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1629 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/base.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     3679 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/braket_notation_to_matrix.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1409 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/matrix_to_quantum_circuit.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2440 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     1526 2023-07-28 05:38:56.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_matrix.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.046549 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        0 2023-05-26 12:59:36.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/__init__.py
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     4310 2023-07-28 06:43:21.000000 qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/converter_service.py
+drwxr-xr-x   0 minwook-shin   (501) staff       (20)        0 2023-08-02 12:19:44.048717 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/
+-rw-r--r--   0 minwook-shin   (501) staff       (20)     2565 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/PKG-INFO
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      801 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)        1 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      206 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/requires.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       23 2023-08-02 12:19:44.000000 qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/top_level.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)      126 2023-08-02 12:13:57.000000 qiskit-classroom-converter-0.0.4/requirements.txt
+-rw-r--r--   0 minwook-shin   (501) staff       (20)       79 2023-08-02 12:19:44.049706 qiskit-classroom-converter-0.0.4/setup.cfg
```

### Comparing `qiskit-classroom-converter-0.0.3/LICENSE` & `qiskit-classroom-converter-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/PKG-INFO` & `qiskit-classroom-converter-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.3
+Version: 0.0.4
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.3/README.md` & `qiskit-classroom-converter-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/pyproject.toml` & `qiskit-classroom-converter-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools.packages.find]
 include = ['qiskit_class_converter*']
 exclude = ['qiskit_class_converter*tests']
 
 [project]
 name = "qiskit-classroom-converter"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "KMU-quantum-classroom" },
 ]
 description = "extend the Qiskit classroom applications."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -26,15 +26,16 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "qiskit==0.44.0",
     "qiskit-aer==0.12.2",
     "loguru==0.7.0",
     "sympy==1.12",
-    "antlr4-python3-runtime==4.11"
+    "antlr4-python3-runtime==4.11",
+    "tomli==2.0.1; python_version < '3.11'"
 ]
 
 [project.optional-dependencies]
 dev = [
     "coverage==7.2.7",
     "pylint==2.17.5",
     "tox==4.6.4",
```

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/__init__.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/matrix_to_quantum_circuit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,9 @@
 """
-# qiskit-classroom-converter API Documents
-
-Convert quantum circuits, matrices, and bra-ket strings.
-
-# How to Install
-
-```
-pip install qiskit-classroom-converter
-```
-
-# Support convert method
-
-* quantum circuit to bra-ket notation
-* quantum circuit to matrix
-* matrix to quantum circuit
-* bra-ket notation to matrix
-
-# Options
-
-| convert method    | option                                   |
-|-------------------|------------------------------------------|
-| QC_TO_BRA_KET     | expression{simplify, expand}, print{raw} |
-| QC_TO_MATRIX      | -                                        |
-| MATRIX_TO_QC      | label{str}                               |
-| BRA_KET_TO_MATRIX | -                                        |
-
+Matrix to Quantum Circuit Converter
 """
 #  Licensed to the Apache Software Foundation (ASF) under one
 #  or more contributor license agreements.  See the NOTICE file
 #  distributed with this work for additional information
 #  regarding copyright ownership.  The ASF licenses this file
 #  to you under the Apache License, Version 2.0 (the
 #  "License"); you may not use this file except in compliance
@@ -39,10 +14,24 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-from .services.converter_service import ConversionService, ConversionType
+from qiskit_class_converter.converters.base import BaseConverter
+
 
-__all__ = ["ConversionService", "ConversionType"]
+class MatrixToQuantumCircuitConverter(BaseConverter):
+    """
+    Converter class
+    """
+
+    def actual_convert_action(self):
+        self.logger.debug("matrix to quantum circuit")
+        gate = self.qiskit.extensions.UnitaryGate(self.input_value)
+        # parse by unitary circuit. can't describe what circuit is.
+        if self.option.get("label", False):
+            gate.label = self.option.get("label", "")
+        else:
+            gate.label = str(self.input_value)
+        return gate
```

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/base.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/braket_notation_to_matrix.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/braket_notation_to_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,10 +113,9 @@
             expr_str = expr_str.replace(local_dict_str[key], key,1)
         expr = parse_expr(expr_str, evaluate=False, transformations='all', local_dict=local_dict)
         return expr
 
     def actual_convert_action(self):
         self.logger.debug("bra-ket notation to matrix")
         expr = self.parse_braket(self.input_value)
-        self.logger.info(expr)
         return expr
```

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_braket_notation.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/converters/quantum_circuit_to_matrix.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/converters/quantum_circuit_to_matrix.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_class_converter/services/converter_service.py` & `qiskit-classroom-converter-0.0.4/qiskit_class_converter/services/converter_service.py`

 * *Files identical despite different names*

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/PKG-INFO` & `qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-classroom-converter
-Version: 0.0.3
+Version: 0.0.4
 Summary: extend the Qiskit classroom applications.
 Author: KMU-quantum-classroom
 Project-URL: Homepage, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter
 Project-URL: Bug Tracker, https://github.com/KMU-quantum-classroom/qiskit-classroom-converter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `qiskit-classroom-converter-0.0.3/qiskit_classroom_converter.egg-info/SOURCES.txt` & `qiskit-classroom-converter-0.0.4/qiskit_classroom_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

