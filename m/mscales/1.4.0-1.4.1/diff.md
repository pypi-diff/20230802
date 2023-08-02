# Comparing `tmp/mscales-1.4.0.tar.gz` & `tmp/mscales-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mscales-1.4.0.tar", last modified: Fri Jul 28 16:49:54 2023, max compression
+gzip compressed data, was "dist/mscales-1.4.1.tar", last modified: Wed Aug  2 13:08:27 2023, max compression
```

## Comparing `mscales-1.4.0.tar` & `mscales-1.4.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2023-05-31 17:16:11.000000 mscales-1.4.0/AUTHORS.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2023-05-31 17:16:11.000000 mscales-1.4.0/CONTRIBUTING.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2023-05-31 17:16:11.000000 mscales-1.4.0/LICENSE
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2023-05-31 17:16:11.000000 mscales-1.4.0/MANIFEST.in
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-07-28 16:49:54.902812 mscales-1.4.0/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      975 2023-07-28 16:41:27.000000 mscales-1.4.0/README.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.898811 mscales-1.4.0/docs/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      655 2023-07-12 14:02:42.000000 mscales-1.4.0/docs/Makefile
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      779 2023-07-12 14:02:42.000000 mscales-1.4.0/docs/make.bat
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.898811 mscales-1.4.0/docs/source/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3574 2023-07-28 16:23:15.000000 mscales-1.4.0/docs/source/basic.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7379 2023-07-13 12:17:47.000000 mscales-1.4.0/docs/source/conf.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      418 2023-07-12 14:46:17.000000 mscales-1.4.0/docs/source/index.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2023-07-28 16:23:15.000000 mscales-1.4.0/docs/source/quickstart.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1624 2023-07-28 16:47:57.000000 mscales-1.4.0/docs/source/release-history.rst
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2023-05-31 17:16:11.000000 mscales-1.4.0/docs/source/scales.rst
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      229 2023-07-12 14:46:22.000000 mscales-1.4.0/mscales/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/_version.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    15496 2023-07-28 16:23:20.000000 mscales-1.4.0/mscales/basic.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/concepts.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/plots.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2023-07-12 14:56:49.000000 mscales-1.4.0/mscales/scales.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/sound.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales/tests/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/__init__.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/conftest.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2023-05-31 17:16:11.000000 mscales-1.4.0/mscales/tests/test_examples.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3138 2023-07-28 16:23:20.000000 mscales-1.4.0/mscales/utils.py
-drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-07-28 16:49:54.902812 mscales-1.4.0/mscales.egg-info/
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/PKG-INFO
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      666 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/SOURCES.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/dependency_links.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       29 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/requires.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-07-28 16:49:54.000000 mscales-1.4.0/mscales.egg-info/top_level.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       81 2023-07-13 16:14:25.000000 mscales-1.4.0/requirements.txt
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-07-28 16:49:54.902812 mscales-1.4.0/setup.cfg
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2023-06-15 17:01:06.000000 mscales-1.4.0/setup.py
--rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2023-05-31 17:16:11.000000 mscales-1.4.0/versioneer.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      170 2022-03-29 15:41:07.000000 mscales-1.4.1/AUTHORS.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3032 2022-03-29 15:41:07.000000 mscales-1.4.1/CONTRIBUTING.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1522 2022-03-29 15:41:07.000000 mscales-1.4.1/LICENSE
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      360 2022-03-29 15:41:07.000000 mscales-1.4.1/MANIFEST.in
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-08-02 13:08:27.000000 mscales-1.4.1/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      975 2023-08-02 13:01:32.000000 mscales-1.4.1/README.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/docs/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      655 2023-08-02 13:01:32.000000 mscales-1.4.1/docs/Makefile
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      779 2023-08-02 13:01:32.000000 mscales-1.4.1/docs/make.bat
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/docs/source/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3574 2023-08-02 13:01:32.000000 mscales-1.4.1/docs/source/basic.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     7379 2023-08-02 13:01:32.000000 mscales-1.4.1/docs/source/conf.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      418 2023-08-02 13:01:32.000000 mscales-1.4.1/docs/source/index.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3534 2022-05-24 13:07:53.000000 mscales-1.4.1/docs/source/quickstart.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1706 2023-08-02 13:03:44.000000 mscales-1.4.1/docs/source/release-history.rst
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       71 2022-05-23 12:38:15.000000 mscales-1.4.1/docs/source/scales.rst
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      229 2023-08-02 13:01:32.000000 mscales-1.4.1/mscales/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      497 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales/_version.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    15809 2023-08-02 13:06:33.000000 mscales-1.4.1/mscales/basic.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      529 2022-05-17 19:38:58.000000 mscales-1.4.1/mscales/concepts.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1109 2022-05-23 12:38:15.000000 mscales-1.4.1/mscales/plots.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1553 2022-05-23 14:33:08.000000 mscales-1.4.1/mscales/scales.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1610 2023-02-01 12:04:32.000000 mscales-1.4.1/mscales/sound.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales/tests/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2022-04-10 10:31:08.000000 mscales-1.4.1/mscales/tests/__init__.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        0 2022-04-10 10:31:08.000000 mscales-1.4.1/mscales/tests/conftest.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      160 2022-11-04 09:23:36.000000 mscales-1.4.1/mscales/tests/test_examples.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     3138 2023-08-02 13:01:32.000000 mscales-1.4.1/mscales/utils.py
+drwxrwxr-x   0 fmoss     (1000) fmoss     (1000)        0 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     1430 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/PKG-INFO
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      666 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        1 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       29 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/requires.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)        8 2023-08-02 13:08:27.000000 mscales-1.4.1/mscales.egg-info/top_level.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)       81 2023-08-02 13:01:32.000000 mscales-1.4.1/requirements.txt
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)      178 2023-08-02 13:08:27.000000 mscales-1.4.1/setup.cfg
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)     2149 2022-05-23 12:53:33.000000 mscales-1.4.1/setup.py
+-rw-rw-r--   0 fmoss     (1000) fmoss     (1000)    68611 2022-03-29 15:41:07.000000 mscales-1.4.1/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `mscales-1.4.0/CONTRIBUTING.rst` & `mscales-1.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/LICENSE` & `mscales-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/PKG-INFO` & `mscales-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.4.0/README.rst` & `mscales-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/Makefile` & `mscales-1.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/make.bat` & `mscales-1.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/source/basic.rst` & `mscales-1.4.1/docs/source/basic.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/source/conf.py` & `mscales-1.4.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/source/quickstart.rst` & `mscales-1.4.1/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/docs/source/release-history.rst` & `mscales-1.4.1/docs/source/release-history.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Release History
 ===============
 
+v1.4.1 (2023-08-02)
+-------------------
+
+- hotfix: fix .utils import in basic.py
+
 v1.4.0 (2023-07-28)
 -------------------
 
 - add several scale properties to PitchClassSet type
 
 v1.3.7 (2023-07-21)
 -------------------
```

### Comparing `mscales-1.4.0/mscales/basic.py` & `mscales-1.4.1/mscales/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from itertools import combinations
 from collections.abc import Iterable
 import matplotlib.pyplot as plt
 import pretty_midi as pm
-from utils import find_ngrams
+from .utils import find_ngrams
 from collections import Counter
 
 rng = np.random.default_rng()
 
 
 class PitchClass:
     """
@@ -33,15 +33,17 @@
         else:
             raise TypeError(f"Can't add type {type(other)} to pitch class {self.p}.")
 
     def __sub__(self, other):
         if isinstance(other, PitchClassInterval):
             return PitchClass((self.p - other.i) % self.c)
         else:
-            raise TypeError(f"Can't subtract type {type(other)} from pitch class {self.p}.")
+            raise TypeError(
+                f"Can't subtract type {type(other)} from pitch class {self.p}."
+            )
 
     def __eq__(self, other):
         return self.p == other.p
 
 
 class PitchClassInterval:
     """
@@ -66,15 +68,17 @@
         else:
             raise TypeError(f"Can't add type {type(other)} to interval {self.i}.")
 
     def __sub__(self, other):
         if isinstance(other, PitchClassInterval):
             return self.i - other.i % self.c
         else:
-            raise TypeError(f"Can't subtract type {type(other)} from interval {self.i}.")
+            raise TypeError(
+                f"Can't subtract type {type(other)} from interval {self.i}."
+            )
 
     def __eq__(self, other):
         return self.i == other.i
 
 
 class PitchClassSet:
     """
@@ -85,19 +89,21 @@
         self.c = c
         self.d = len(pcset)
 
         if isinstance(pcset, str):
             assert all(
                 x in [str(i) for i in range(10)] + ["T"] + ["E"] for x in list(pcset)
             ), "Some pitch classes are not valid."
-            self.pcs = np.array([10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)])
+            self.pcs = np.array(
+                [10 if p == "T" else 11 if p == "E" else int(p) for p in list(pcset)]
+            )
         elif isinstance(pcset, (Iterable, PitchClassSet)):
             self.pcs = np.array([int(p) for p in pcset])
         else:
-            raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")        
+            raise TypeError(f"I don't recognize the pitch-class input {type(pcset)}.")
 
     def __repr__(self):
         return f"PitchClassSet({self.pcs})"
 
     def __str__(self):
         return str(set(self.pcs))
 
@@ -134,15 +140,17 @@
         self = self.sort()
 
         if len(self.pcs) == 0:
             raise "PitchClassSet is empty!"
         elif len(self.pcs) == 1:
             return self
         else:
-            rotations = np.array([np.roll(self.pcs, i) for i in range(self.pcs.shape[0])])
+            rotations = np.array(
+                [np.roll(self.pcs, i) for i in range(self.pcs.shape[0])]
+            )
             for length in range(self.d - 1, 0, -1):
                 spans = [(r[-1] - r[0]) % self.c for r in rotations[:, : length + 1]]
                 mask = spans == min(spans)
                 min_span_rotations = rotations[mask]
 
                 # if there is a tie in the first step and we want to obtain all candidates
                 # if there is only one candidate left
@@ -210,56 +218,66 @@
         for i in interval_classes:
             iv[i - 1] += 1
 
         return iv
 
     def maximally_even(self):
         """
-        Calculates all maximally even sets for chromatic cardinality c 
+        Calculates all maximally even sets for chromatic cardinality c
         and diatonic cardinality d.
         """
 
-        D = [ [ np.floor((self.c * k + m) / self.d).astype(int) for k in range(self.d) ] for m in range(self.c) ]
-        D = [ np.array(s) for s in set(tuple(i) for i in D) ]
+        D = [
+            [np.floor((self.c * k + m) / self.d).astype(int) for k in range(self.d)]
+            for m in range(self.c)
+        ]
+        D = [np.array(s) for s in set(tuple(i) for i in D)]
 
         for s in D:
             if set(s) == set(self.pcs):
                 return True
             else:
                 return False
 
     def spectrum(self, i):
         """
         Returns the spectrum of generic interval i,
         given chromatic cardinality c and diatonic cardinality d.
         """
 
-        assert i in range(self.d), f"Generic interval i={i} has to be between 0 and {self.d-1}."
+        assert i in range(
+            self.d
+        ), f"Generic interval i={i} has to be between 0 and {self.d-1}."
 
-        return { (k - j) % self.c for j, k in zip(self.pcs, np.roll(self.pcs, -i)) }
+        return {(k - j) % self.c for j, k in zip(self.pcs, np.roll(self.pcs, -i))}
 
     def myhill(self):
         """
         Returns whether pitch-class set has Myhill's property.
         """
 
-        specs = set([ len(self.spectrum(i=i)) for i in range(1,self.d) ])
-        
+        specs = set([len(self.spectrum(i=i)) for i in range(1, self.d)])
+
         return True if specs == {2} else False
 
     def cardinality_equals_variety(self):
         """
         Tests if cardinality equals variety holds for PCSet.
         See: https://en.wikipedia.org/wiki/Cardinality_equals_variety
         """
-        cev = True
-        for n in range(2,self.d + 1):
-            s = np.append(self.pcs, self.pcs[:n-1])
+
+        for n in range(2, self.d + 1):
+            s = np.append(self.pcs, self.pcs[: n - 1])
             ngrams = find_ngrams(s, n=n)
-            intervals = [ "".join([str((gram[i] - gram[i-1]) % 12) for i in range(1, len(gram))]) for gram in ngrams ]
+            intervals = [
+                "".join(
+                    [str((gram[i] - gram[i - 1]) % 12) for i in range(1, len(gram))]
+                )
+                for gram in ngrams
+            ]
             if n != len(Counter(intervals)):
                 return False
         return True
 
     def sum(self) -> int:
         return sum(self.pcs)
 
@@ -310,15 +328,17 @@
             return ax
         elif kind == "area":
             thetas += thetas[:1]
             radii += radii[:1]
             ax.plot(thetas, radii, c="k", zorder=5)
             ax.fill(thetas, radii, alpha=0.75, zorder=4)
         else:
-            print("I don't recognize the plot kind." "Valid values are 'polar' and 'bar'.")
+            print(
+                "I don't recognize the plot kind." "Valid values are 'polar' and 'bar'."
+            )
         if save:
             plt.savefig(save)
 
     def play(
         self,
         mode: str = "cloud",
         n_notes: int = 100,
@@ -328,15 +348,17 @@
         save_as: str = None,
     ):
 
         if mode == "cloud":
             starts = np.arange(n_notes) * note_duration  # onsets
             ends = starts + note_duration  # offsets
 
-            pitches = [x for x in rng.choice(np.nonzero(self.to_vector())[0], size=n_notes)]
+            pitches = [
+                x for x in rng.choice(np.nonzero(self.to_vector())[0], size=n_notes)
+            ]
             octaves = rng.choice(np.arange(3, 7), size=n_notes)
             midi_pitches = [(p + 12 * o) for p, o in list(zip(pitches, octaves))]
         elif mode == "chord":
             pitches = self.pcs
             octaves = [4] * pitches.shape[0]
             midi_pitches = [(p + 12 * o) for p, o in list(zip(pitches, octaves))]
 
@@ -385,19 +407,22 @@
         s += f"inverted\t: {self.invert()}" + "\n"
         s += f"T2I\t\t: {self.invert(2)}" + "\n"
         s += f"normal form\t: {self.normal_form()}" + "\n"
         s += f"prime form\t: {self.prime_form()}" + "\n"
         s += f"interval vector\t: {self.interval_vector()}" + "\n\n"
 
         s += "Diatonic Scale Theory" + "\n"
-        s += "====================="  + "\n"
-        s += f"Maximally even: {str(self.maximally_even())}" + "\n" 
+        s += "=====================" + "\n"
+        s += f"Maximally even: {str(self.maximally_even())}" + "\n"
         s += f"Spectrum (step): {str(self.spectrum(i=1))}" + "\n"
         s += f"Myhill's property: {str(self.myhill())}" + "\n"
-        s += f"Cardinality equals variety: {str(self.cardinality_equals_variety())}" + "\n\n" 
+        s += (
+            f"Cardinality equals variety: {str(self.cardinality_equals_variety())}"
+            + "\n\n"
+        )
 
         s += "Serialism" + "\n"
         s += "=========" + "\n"
         s += f"original\t: {self}" + "\n"
         s += f"retrograde\t: {self.retrograde()}" + "\n"
         s += f"inversion\t: {self.inversion()}" + "\n"
         s += f"retro.-inv.\t: {self.inversion().retrograde()}" + "\n"
@@ -431,15 +456,15 @@
     print(pcset.pcs)
     print(pcset.info())
     # ax = pcset.plot(kind="area")
     # plt.show()
 
     # pcset.play(save_as="test.mid", mode="cloud")
 
-    ## maximally even test
+    # maximally even test
     # t = PitchClassSet("1234")
     # dia = PitchClassSet("024579E")
     p = PitchClassSet("1368T")
     # oct = PitchClassSet("0134679T")
     print(p.info())
     # hex = PitchClassSet("E03478")
     # ten = PitchClassSet("02468", c=10)
```

### Comparing `mscales-1.4.0/mscales/concepts.py` & `mscales-1.4.1/mscales/concepts.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/mscales/plots.py` & `mscales-1.4.1/mscales/plots.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/mscales/scales.py` & `mscales-1.4.1/mscales/scales.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/mscales/sound.py` & `mscales-1.4.1/mscales/sound.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/mscales/utils.py` & `mscales-1.4.1/mscales/utils.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/mscales.egg-info/PKG-INFO` & `mscales-1.4.1/mscales.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mscales
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python package to generate and analyze musical scales.
 Home-page: https://github.com/fabianmoss/mscales
 Author: Fabian C. Moss
 Author-email: fabianmoss@gmail.com
 License: BSD (3-clause)
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
```

### Comparing `mscales-1.4.0/mscales.egg-info/SOURCES.txt` & `mscales-1.4.1/mscales.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/setup.py` & `mscales-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `mscales-1.4.0/versioneer.py` & `mscales-1.4.1/versioneer.py`

 * *Files identical despite different names*

