# Comparing `tmp/constava-0.1.0.tar.gz` & `tmp/constava-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constava-0.1.0.tar", last modified: Wed Aug  2 14:46:05 2023, max compression
+gzip compressed data, was "constava-0.1.0b3.tar", last modified: Mon Jul 24 15:18:53 2023, max compression
```

## Comparing `constava-0.1.0.tar` & `constava-0.1.0b3.tar`

### file list

```diff
@@ -1,37 +1,31 @@
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.870815 constava-0.1.0/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        3 2023-06-21 10:18:15.000000 constava-0.1.0/LICENSE
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-06-29 10:54:47.000000 constava-0.1.0/MANIFEST.in
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9751 2023-08-02 14:46:05.870198 constava-0.1.0/PKG-INFO
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     8353 2023-07-24 15:43:25.000000 constava-0.1.0/README.md
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.827174 constava-0.1.0/constava/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       44 2023-08-02 14:06:42.000000 constava-0.1.0/constava/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     7878 2023-08-02 12:25:18.000000 constava-0.1.0/constava/__main__.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.834365 constava-0.1.0/constava/calc/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 12:25:18.000000 constava-0.1.0/constava/calc/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2544 2023-08-02 14:06:42.000000 constava-0.1.0/constava/calc/calculator.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)    10393 2023-08-02 12:25:18.000000 constava-0.1.0/constava/calc/pdfestimators.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)    10006 2023-08-02 12:25:18.000000 constava-0.1.0/constava/calc/subsampling.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      659 2023-08-02 12:25:18.000000 constava-0.1.0/constava/constants.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.835201 constava-0.1.0/constava/data/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20) 13337025 2023-07-11 12:57:23.000000 constava-0.1.0/constava/data/constava_default_training_data.json
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.863221 constava-0.1.0/constava/datautils/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 12:25:18.000000 constava-0.1.0/constava/datautils/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4581 2023-08-02 12:25:18.000000 constava-0.1.0/constava/datautils/ensembles.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1211 2023-08-02 14:06:42.000000 constava-0.1.0/constava/datautils/results.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4675 2023-08-02 12:25:18.000000 constava-0.1.0/constava/dihedrals.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.867383 constava-0.1.0/constava/io/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 12:25:18.000000 constava-0.1.0/constava/io/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)    12572 2023-08-02 12:25:18.000000 constava-0.1.0/constava/io/ensemblereader.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     3972 2023-08-02 14:06:42.000000 constava-0.1.0/constava/io/resultswriter.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.869231 constava-0.1.0/constava/wrapper/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:06:42.000000 constava-0.1.0/constava/wrapper/__init__.py
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     7548 2023-08-02 14:06:42.000000 constava-0.1.0/constava/wrapper/wrapper_utils.py
-drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-08-02 14:46:05.831371 constava-0.1.0/constava.egg-info/
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9751 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/PKG-INFO
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      721 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/SOURCES.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/dependency_links.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       53 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/entry_points.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       37 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/requires.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        9 2023-08-02 14:46:05.000000 constava-0.1.0/constava.egg-info/top_level.txt
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-08-02 14:46:05.870980 constava-0.1.0/setup.cfg
--rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1898 2023-08-02 14:46:00.000000 constava-0.1.0/setup.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-07-24 15:18:53.725190 constava-0.1.0b3/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        3 2023-06-21 10:18:15.000000 constava-0.1.0b3/LICENSE
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-06-29 10:54:47.000000 constava-0.1.0b3/MANIFEST.in
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9733 2023-07-24 15:18:53.723063 constava-0.1.0b3/PKG-INFO
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     8353 2023-07-24 15:18:10.000000 constava-0.1.0b3/README.md
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-07-24 15:18:53.665861 constava-0.1.0b3/constava/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       44 2023-06-21 13:38:32.000000 constava-0.1.0b3/constava/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     7733 2023-06-29 12:27:54.000000 constava-0.1.0b3/constava/__main__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1189 2023-06-29 10:54:47.000000 constava-0.1.0b3/constava/calculator.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      588 2023-06-29 10:54:47.000000 constava-0.1.0b3/constava/constants.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-07-24 15:18:53.672633 constava-0.1.0b3/constava/data/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20) 13337025 2023-07-11 12:57:23.000000 constava-0.1.0b3/constava/data/constava_default_training_data.json
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     2442 2023-06-21 10:18:15.000000 constava-0.1.0b3/constava/dihedrals.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5501 2023-06-21 13:38:27.000000 constava-0.1.0b3/constava/ensemblereader.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     4475 2023-06-21 13:38:27.000000 constava-0.1.0b3/constava/ensembles.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     3393 2023-06-29 11:26:43.000000 constava-0.1.0b3/constava/methods.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     5286 2023-06-29 12:27:54.000000 constava-0.1.0b3/constava/pdfestimators.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      833 2023-06-21 10:18:15.000000 constava-0.1.0b3/constava/results.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     3865 2023-06-21 10:18:15.000000 constava-0.1.0b3/constava/resultswriter.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-07-24 15:18:53.719933 constava-0.1.0b3/constava/wrapper_source/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        0 2023-06-21 13:38:32.000000 constava-0.1.0b3/constava/wrapper_source/__init__.py
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     7510 2023-06-29 12:38:03.000000 constava-0.1.0b3/constava/wrapper_source/wrapper_utils.py
+drwxr-xr-x   0 josegavaldagarcia   (501) staff       (20)        0 2023-07-24 15:18:53.671380 constava-0.1.0b3/constava.egg-info/
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     9733 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/PKG-INFO
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)      609 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/SOURCES.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        1 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/dependency_links.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       53 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/entry_points.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       37 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/requires.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)        9 2023-07-24 15:18:53.000000 constava-0.1.0b3/constava.egg-info/top_level.txt
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)       38 2023-07-24 15:18:53.725404 constava-0.1.0b3/setup.cfg
+-rw-r--r--   0 josegavaldagarcia   (501) staff       (20)     1880 2023-07-24 15:14:39.000000 constava-0.1.0b3/setup.py
```

### Comparing `constava-0.1.0/PKG-INFO` & `constava-0.1.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constava
-Version: 0.1.0
+Version: 0.1.0b3
 Summary: This software is used to calculate conformational states probability & conformational state variability from a protein structure ensemble.
 Home-page: https://bitbucket.org/bio2byte/constava/
 Author: Wim Vranken
 Author-email: wim.vranken@vub.be
 Maintainer: Jose Gavalda-Garcia, David Bickel, Adrian Diaz, Wim Vranken
 Maintainer-email: jose.gavalda.garcia@vub.be, david.bickel@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,16 +18,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="readme-top"></a>
 
 <!-- PROJECT LOGO -->
 <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constava Version: 0.1.0 Summary: This software is
+Metadata-Version: 2.1 Name: constava Version: 0.1.0b3 Summary: This software is
 used to calculate conformational states probability & conformational state
 variability from a protein structure ensemble. Home-page: https://
 bitbucket.org/bio2byte/constava/ Author: Wim Vranken Author-email:
 wim.vranken@vub.be Maintainer: Jose Gavalda-Garcia, David Bickel, Adrian Diaz,
 Wim Vranken Maintainer-email: jose.gavalda.garcia@vub.be, david.bickel@vub.be,
 adrian.diaz@vub.be, wim.vranken@vub.be License: OSI Approved :: GNU General
 Public License v3 (GPLv3) Platform: UNKNOWN Classifier: Natural Language ::
@@ -11,16 +11,16 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
 Independent Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Education Classifier: Development
-Status :: 5 - Production/Stable Requires-Python: >=3.6, <3.11 Description-
-Content-Type: text/markdown License-File: LICENSE
+Status :: 4 - Beta Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 [https://pbs.twimg.com/profile_images/1247824923546079232/B9b_Yg7n_400x400.jpg]
                                   # Constava
 ## Description This software is used to calculate conformational states
 propensities & conformational state variability from a protein structure
 ensemble. This is done by calculating the propensities for each conformational
 state for each residue in a protein ensemble. Then, conformational state
 variability is calculated from the change among conformational states, inferred
```

### Comparing `constava-0.1.0/README.md` & `constava-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `constava-0.1.0/constava/__main__.py` & `constava-0.1.0b3/constava/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-"""constava.__main__ is the executable for the command line functionality of 
-the tool."""
-
 import sys, os
 import argparse
 from warnings import warn
 
+from constava.calculator import ConfStateCalculator
 from constava.constants import DEFAULT_KDE_PATH, DEFAULT_TRAINING_DATA_PATH
-from constava.calc.calculator import ConfStateCalculator
-from constava.calc.subsampling import SubsamplingBootstrap, SubsamplingWindow
-from constava.calc.pdfestimators import KDEStatePdf, GridStatePdf
-from constava.io.ensemblereader import EnsembleReader
-from constava.io.resultswriter import ResultWriter
-
+from constava.ensemblereader import EnsembleReader
+from constava.methods import ConstavaBootstrap, ConstavaWindow
+from constava.resultswriter import ResultWriter
+from constava.pdfestimators import KDEStatePdf, GridStatePdf
 
 
 def parse_commandline_arguments(arguments):
 
     # Required for the description to consider return characters \n
     class CustomFormatter(argparse.RawDescriptionHelpFormatter, argparse.ArgumentDefaultsHelpFormatter):
         pass
@@ -66,15 +62,15 @@
     #                       help="Load KDEs used in publication. This requires sklearn version x.x.xx")
 
     misc_group = parser.add_argument_group("Miscellaneous Options")
     misc_group.add_argument("--window", metavar="<int>", type=int, nargs='+', help="Do inference using a moving reading-frame of <int> consecutive samples.")
     misc_group.add_argument("--bootstrap", metavar="<int>", type=int, nargs='+', help="Do inference using <Int> samples obtained through bootstrapping. (By default a run with 3 and 25 is performed.)")
     misc_group.add_argument("--bootstrap-samples", metavar="<int>", type=int, default=500, help="If bootstrap, sample <Int> times from the input data (default: 500)")
     misc_group.add_argument("--seed", metavar="<int>", type=int, default=None, required=False, help="Set random seed for bootstrap sampling (default: None)")
-    misc_group.add_argument("--quick", action="store_true", help="Use grid-interpolation instead of KDEs")
+    #misc_group.add_argument("--quick", action="store_true", help="Use grid-interpolation instead of KDEs")
     misc_group.add_argument("--precision", type=int, default=4, help='Sets de number of decimals in the output files. By default, 4 decimal.')
 
     # Do actual parameter parsing
     args = parser.parse_args(arguments)
 
     # Some validity checks for Input/output
     if args.input_file is not None and args.output_file is None:
@@ -131,17 +127,17 @@
     # IF dump_kdes, THEN save the KDEs
     if args.dump_kdes is not None:
         pdfestimator.dump_pickle(args.dump_kdes)
 
     # Load the calculation methods
     cscalc = ConfStateCalculator(pdfestimator)
     for window_size in args.window:
-        cscalc.add_method(SubsamplingWindow(window_size))
+        cscalc.add_method(ConstavaWindow(window_size))
     for sample_size in args.bootstrap:
-        cscalc.add_method(SubsamplingBootstrap(sample_size, args.bootstrap_samples, seed=args.seed))
+        cscalc.add_method(ConstavaBootstrap(sample_size, args.bootstrap_samples))
 
     # Do the inference
     results = cscalc.calculate(ensemble)
 
     # Write output
     writer = ResultWriter(args.output_format, args.precision)
     writer.writeToFile(results, args.output_file)
```

### Comparing `constava-0.1.0/constava/data/constava_default_training_data.json` & `constava-0.1.0b3/constava/data/constava_default_training_data.json`

 * *Files identical despite different names*

### Comparing `constava-0.1.0/constava/datautils/ensembles.py` & `constava-0.1.0b3/constava/ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-"""constava.ensembles contains classes describing the input data from the 
-conformational ensemble.
-"""
-
 from dataclasses import dataclass
 from typing import List, Generator
 import numpy as np
 
-from ..constants import aminoacids3to1
+from .constants import aminoacids3to1
 
 
 @dataclass
 class ResidueEnsemble:
     """ 
     Dataclass to hold information on a given residue in a conformational ensemble:
```

### Comparing `constava-0.1.0/constava/io/resultswriter.py` & `constava-0.1.0b3/constava/resultswriter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-"""constava.resultswriter contains classes the write the output to different 
-data formats."""
-
 import abc
 import csv
 import json
 import os 
 from typing import List
 import numpy as np
-from ..datautils.results import ConfStateResults, ConfStateResultsEntry
+from .results import ConfStateResults, ConfStateResultsEntry
 
 
 class WriterABC(metaclass=abc.ABCMeta):
 
     def __init__(self, float_precision: int = 4):
         self.float_precision = float_precision
```

### Comparing `constava-0.1.0/constava/wrapper/wrapper_utils.py` & `constava-0.1.0b3/constava/wrapper_source/wrapper_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # import sys
 # import argparse
 import os
 import glob
 from typing import List, Union, Optional, Literal
 
+from constava.calculator import ConfStateCalculator
 from constava.constants import DEFAULT_KDE_PATH, DEFAULT_TRAINING_DATA_PATH
-from constava.calc.calculator import ConfStateCalculator
-from constava.calc.subsampling import SubsamplingBootstrap, SubsamplingWindow
-from constava.calc.pdfestimators import KDEStatePdf, GridStatePdf
-from constava.io.ensemblereader import EnsembleReader
-from constava.io.resultswriter import ResultWriter
-
+from constava.ensemblereader import EnsembleReader
+from constava.methods import ConstavaBootstrap, ConstavaWindow
+from constava.resultswriter import ResultWriter
+from constava.pdfestimators import KDEStatePdf, GridStatePdf
 
 
 class ConStaVa:
 	"""
 	Initializes all the variables in required for the fitting and calculation of the Conformational State Variability.
 	It also stores all relevant information to train, save and load Kernel Density Estimators (KDE) as well as to
 	calculate and save Conformational State Variability for different windows and bootstrap parameters.
@@ -186,19 +185,19 @@
 		cscalc = ConfStateCalculator(self.pdfestimator)
 
 		if self.window is None and self.bootstrap is None:
 			self.bootstrap = [3, 25]
 
 		if self.window is not None:
 			for window_size in self.window:
-				cscalc.add_method(SubsamplingWindow(window_size))
+				cscalc.add_method(ConstavaWindow(window_size))
 
 		if self.bootstrap is not None:
 			for sample_size in self.bootstrap:
-				cscalc.add_method(SubsamplingBootstrap(sample_size, self.bootstrap_samples, seed=self.bootstrap_seed))
+				cscalc.add_method(ConstavaBootstrap(sample_size, self.bootstrap_samples, seed=self.bootstrap_seed))
 
 		# Do the inference
 		self.results = cscalc.calculate(self.ensemble)
 
 	def save_results(self, output_file: str, output_format: Literal['auto', 'csv', 'json'] = 'auto',
 	                 precision: int = 4):
 		"""
```

### Comparing `constava-0.1.0/constava.egg-info/PKG-INFO` & `constava-0.1.0b3/constava.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constava
-Version: 0.1.0
+Version: 0.1.0b3
 Summary: This software is used to calculate conformational states probability & conformational state variability from a protein structure ensemble.
 Home-page: https://bitbucket.org/bio2byte/constava/
 Author: Wim Vranken
 Author-email: wim.vranken@vub.be
 Maintainer: Jose Gavalda-Garcia, David Bickel, Adrian Diaz, Wim Vranken
 Maintainer-email: jose.gavalda.garcia@vub.be, david.bickel@vub.be, adrian.diaz@vub.be, wim.vranken@vub.be
 License: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,16 +18,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6, <3.11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="readme-top"></a>
 
 <!-- PROJECT LOGO -->
 <br />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: constava Version: 0.1.0 Summary: This software is
+Metadata-Version: 2.1 Name: constava Version: 0.1.0b3 Summary: This software is
 used to calculate conformational states probability & conformational state
 variability from a protein structure ensemble. Home-page: https://
 bitbucket.org/bio2byte/constava/ Author: Wim Vranken Author-email:
 wim.vranken@vub.be Maintainer: Jose Gavalda-Garcia, David Bickel, Adrian Diaz,
 Wim Vranken Maintainer-email: jose.gavalda.garcia@vub.be, david.bickel@vub.be,
 adrian.diaz@vub.be, wim.vranken@vub.be License: OSI Approved :: GNU General
 Public License v3 (GPLv3) Platform: UNKNOWN Classifier: Natural Language ::
@@ -11,16 +11,16 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Operating System :: OS
 Independent Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry Classifier: Topic ::
 Scientific/Engineering :: Physics Classifier: Intended Audience :: Science/
 Research Classifier: Intended Audience :: Education Classifier: Development
-Status :: 5 - Production/Stable Requires-Python: >=3.6, <3.11 Description-
-Content-Type: text/markdown License-File: LICENSE
+Status :: 4 - Beta Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
 [https://pbs.twimg.com/profile_images/1247824923546079232/B9b_Yg7n_400x400.jpg]
                                   # Constava
 ## Description This software is used to calculate conformational states
 propensities & conformational state variability from a protein structure
 ensemble. This is done by calculating the propensities for each conformational
 state for each residue in a protein ensemble. Then, conformational state
 variability is calculated from the change among conformational states, inferred
```

### Comparing `constava-0.1.0/constava.egg-info/SOURCES.txt` & `constava-0.1.0b3/constava.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 constava/__init__.py
 constava/__main__.py
+constava/calculator.py
 constava/constants.py
 constava/dihedrals.py
+constava/ensemblereader.py
+constava/ensembles.py
+constava/methods.py
+constava/pdfestimators.py
+constava/results.py
+constava/resultswriter.py
 constava.egg-info/PKG-INFO
 constava.egg-info/SOURCES.txt
 constava.egg-info/dependency_links.txt
 constava.egg-info/entry_points.txt
 constava.egg-info/requires.txt
 constava.egg-info/top_level.txt
-constava/calc/__init__.py
-constava/calc/calculator.py
-constava/calc/pdfestimators.py
-constava/calc/subsampling.py
 constava/data/constava_default_training_data.json
-constava/datautils/__init__.py
-constava/datautils/ensembles.py
-constava/datautils/results.py
-constava/io/__init__.py
-constava/io/ensemblereader.py
-constava/io/resultswriter.py
-constava/wrapper/__init__.py
-constava/wrapper/wrapper_utils.py
+constava/wrapper_source/__init__.py
+constava/wrapper_source/wrapper_utils.py
```

### Comparing `constava-0.1.0/setup.py` & `constava-0.1.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="constava",
-    version="0.1.0",
+    version="0.1.0b3",
     author="Wim Vranken",
     author_email="wim.vranken@vub.be",
     description="This software is used to calculate conformational states probability & conformational state "
                 "variability from a protein structure ensemble.",
     license="OSI Approved :: GNU General Public License v3 (GPLv3)",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -28,17 +28,17 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Scientific/Engineering :: Physics",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
-        "Development Status :: 5 - Production/Stable"
+        "Development Status :: 4 - Beta"
     ],
-    python_requires=">=3.6, <3.11",
+    python_requires=">=3.6",
     install_requires=[
         "MDAnalysis",
         "numpy",
         "pandas",
         "scikit-learn",
     ],
     entry_points={
```

