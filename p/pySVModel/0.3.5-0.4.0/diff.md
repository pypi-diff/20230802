# Comparing `tmp/pySVModel-0.3.5.tar.gz` & `tmp/pySVModel-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySVModel-0.3.5.tar", last modified: Sun Jan 16 13:42:39 2022, max compression
+gzip compressed data, was "pySVModel-0.4.0.tar", last modified: Tue Aug  1 22:12:35 2023, max compression
```

## Comparing `pySVModel-0.3.5.tar` & `pySVModel-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:42:39.535710 pySVModel-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)    10571 2022-01-16 13:42:29.000000 pySVModel-0.3.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-01-16 13:42:39.535710 pySVModel-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4477 2022-01-16 13:42:29.000000 pySVModel-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:42:39.535710 pySVModel-0.3.5/pySVModel/
--rw-r--r--   0 runner    (1001) docker     (121)     7175 2022-01-16 13:42:29.000000 pySVModel-0.3.5/pySVModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 13:42:39.535710 pySVModel-0.3.5/pySVModel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-01-16 13:42:39.000000 pySVModel-0.3.5/pySVModel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-01-16 13:42:39.000000 pySVModel-0.3.5/pySVModel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 13:42:39.000000 pySVModel-0.3.5/pySVModel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-01-16 13:42:39.000000 pySVModel-0.3.5/pySVModel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-01-16 13:42:39.000000 pySVModel-0.3.5/pySVModel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-01-16 13:42:29.000000 pySVModel-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 13:42:39.535710 pySVModel-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-01-16 13:42:29.000000 pySVModel-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:35.651587 pySVModel-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-08-01 22:12:24.000000 pySVModel-0.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-01 22:12:35.651587 pySVModel-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-08-01 22:12:24.000000 pySVModel-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:35.647587 pySVModel-0.4.0/pySVModel/
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-08-01 22:12:24.000000 pySVModel-0.4.0/pySVModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 22:12:35.647587 pySVModel-0.4.0/pySVModel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-08-01 22:12:35.000000 pySVModel-0.4.0/pySVModel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-01 22:12:35.000000 pySVModel-0.4.0/pySVModel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 22:12:35.000000 pySVModel-0.4.0/pySVModel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-01 22:12:35.000000 pySVModel-0.4.0/pySVModel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 22:12:35.000000 pySVModel-0.4.0/pySVModel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-01 22:12:24.000000 pySVModel-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 22:12:35.651587 pySVModel-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-01 22:12:24.000000 pySVModel-0.4.0/setup.py
```

### Comparing `pySVModel-0.3.5/LICENSE.md` & `pySVModel-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pySVModel-0.3.5/PKG-INFO` & `pySVModel-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pySVModel
-Version: 0.3.5
+Version: 0.4.0
 Summary: An abstract SystemVerilog language model (incl. Verilog).
 Home-page: https://GitHub.com/edaa-org/pySVModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pySVModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pySVModel
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pySVModel/issues
 Keywords: Python3 Verilog SystemVerilog Language Model Abstract
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 <p align="center">
   <a title="edaa-org.github.io/pySVModel" href="https://edaa-org.github.io/pySVModel"><img height="80px" src="doc/_static/logo.svg"/></a>
@@ -97,9 +96,7 @@
 # License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pySVModel-0.3.5/README.md` & `pySVModel-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pySVModel-0.3.5/pySVModel.egg-info/PKG-INFO` & `pySVModel-0.4.0/pySVModel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pySVModel
-Version: 0.3.5
+Version: 0.4.0
 Summary: An abstract SystemVerilog language model (incl. Verilog).
 Home-page: https://GitHub.com/edaa-org/pySVModel
 Author: Patrick Lehmann
 Author-email: Paebbels@gmail.com
 License: Apache-2.0
 Project-URL: Documentation, https://edaa-org.GitHub.io/pySVModel
 Project-URL: Source Code, https://GitHub.com/edaa-org/pySVModel
 Project-URL: Issue Tracker, https://GitHub.com/edaa-org/pySVModel/issues
 Keywords: Python3 Verilog SystemVerilog Language Model Abstract
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Compilers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: all
 License-File: LICENSE.md
 
 <p align="center">
   <a title="edaa-org.github.io/pySVModel" href="https://edaa-org.github.io/pySVModel"><img height="80px" src="doc/_static/logo.svg"/></a>
@@ -97,9 +96,7 @@
 # License
 
 This Python package (source code) licensed under [Apache License 2.0](LICENSE.md).  
 The accompanying documentation is licensed under [Creative Commons - Attribution 4.0 (CC-BY 4.0)](doc/Doc-License.rst).
 
 -------------------------
 SPDX-License-Identifier: Apache-2.0
-
-
```

### Comparing `pySVModel-0.3.5/setup.py` & `pySVModel-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # |_|    |___/                                                                                                         #
 # ==================================================================================================================== #
 # Authors:                                                                                                             #
 #   Patrick Lehmann                                                                                                    #
 #                                                                                                                      #
 # License:                                                                                                             #
 # ==================================================================================================================== #
-# Copyright 2021-2022 Patrick Lehmann - Boetzingen, Germany                                                            #
+# Copyright 2021-2023 Patrick Lehmann - Boetzingen, Germany                                                            #
 #                                                                                                                      #
 # Licensed under the Apache License, Version 2.0 (the "License");                                                      #
 # you may not use this file except in compliance with the License.                                                     #
 # You may obtain a copy of the License at                                                                              #
 #                                                                                                                      #
 #   http://www.apache.org/licenses/LICENSE-2.0                                                                         #
 #                                                                                                                      #
@@ -39,14 +39,14 @@
 
 DescribePythonPackageHostedOnGitHub(
 	packageName=packageName,
 	description="An abstract SystemVerilog language model (incl. Verilog).",
 	gitHubNamespace=gitHubNamespace,
 	keywords="Python3 Verilog SystemVerilog Language Model Abstract",
 	sourceFileWithVersion=packageInformationFile,
-	developmentStatus="beta",
+	developmentStatus="alpha",
 	classifiers=list(DEFAULT_CLASSIFIERS) + [
 		"Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
 		"Topic :: Software Development :: Code Generators",
 		"Topic :: Software Development :: Compilers"
 	]
 )
```

