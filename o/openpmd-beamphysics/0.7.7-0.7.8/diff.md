# Comparing `tmp/openpmd-beamphysics-0.7.7.tar.gz` & `tmp/openpmd-beamphysics-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-irn1_pkw/openpmd-beamphysics-0.7.7.tar", last modified: Tue Jul 18 18:30:32 2023, max compression
+gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-hv9qnal5/openpmd-beamphysics-0.7.8.tar", last modified: Wed Aug  2 16:41:41 2023, max compression
```

## Comparing `openpmd-beamphysics-0.7.7.tar` & `openpmd-beamphysics-0.7.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/fieldmesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/ansys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/astra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/bmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/elegant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/genesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/litrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/lucretia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/opal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/simion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/superfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    35085 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/species.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/tests/test_particlegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24315 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/fieldmesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/ansys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/astra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/bmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/elegant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/litrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/lucretia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/opal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/simion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/superfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/pmd_beamphysics/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:41:41.000000 openpmd-beamphysics-0.7.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/tests/test_particlegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-08-02 16:41:31.000000 openpmd-beamphysics-0.7.8/versioneer.py
```

### Comparing `openpmd-beamphysics-0.7.7/LICENSE` & `openpmd-beamphysics-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/PKG-INFO` & `openpmd-beamphysics-0.7.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.7
+Version: 0.7.8
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.7/README.md` & `openpmd-beamphysics-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/PKG-INFO` & `openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.7
+Version: 0.7.8
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/SOURCES.txt` & `openpmd-beamphysics-0.7.8/openpmd_beamphysics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/analysis.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/analysis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/conversion.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/conversion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/expansion.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/expansion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/fieldmesh.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/fields/fieldmesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pmd_beamphysics.writers import write_pmd_field, pmd_field_init
 
 from pmd_beamphysics import tools
 
 from pmd_beamphysics.plot import plot_fieldmesh_cylindrical_2d, plot_fieldmesh_cylindrical_1d
 
 from pmd_beamphysics.interfaces.ansys import read_ansys_ascii_3d_fields
-from pmd_beamphysics.interfaces.astra import read_astra_3d_fieldmaps, write_astra_3d_fieldmaps
+from pmd_beamphysics.interfaces.astra import write_astra_1d_fieldmap, read_astra_3d_fieldmaps, write_astra_3d_fieldmaps, astra_1d_fieldmap_data
 from pmd_beamphysics.interfaces.gpt import write_gpt_fieldmesh
 from pmd_beamphysics.interfaces.impact import create_impact_solrf_fieldmap_fourier, create_impact_solrf_ele
 from pmd_beamphysics.interfaces.superfish import write_superfish_t7, read_superfish_t7
 
 from pmd_beamphysics.fields.expansion import expand_fieldmesh_from_onaxis
 from pmd_beamphysics.fields.conversion import fieldmesh_rectangular_to_cylindrically_symmetric_data
 
@@ -98,16 +98,18 @@
     
     - `.plot`
     - `.plot_onaxis`
     
     Writers
     
     - `.write`
+    - `.write_astra_1d`
     - `.write_astra_3d`
     - `.to_cylindrical`
+    - `.to_astra_1d`
     - `.to_impact_solrf`
     - `.write_gpt`
     - `.write_superfish`
         
     Constructors (class methods):
     
     - `.from_ansys_ascii_3d`
@@ -341,15 +343,24 @@
             h5 = File(fname, 'w')
             pmd_field_init(h5, externalFieldPath='/ExternalFieldPath/%T/')
             g = h5.create_group('/ExternalFieldPath/1/')
         else:
             g = h5
     
         write_pmd_field(g, self.data, name=name)   
-        
+   
+    @functools.wraps(write_astra_1d_fieldmap)
+    def write_astra_1d(self, filePath):      
+        return  write_astra_1d_fieldmap(self, filePath)
+    
+    def to_astra_1d(self):
+        z, fz = astra_1d_fieldmap_data(self)   
+        dat = np.array([z, fz]).T 
+        return {'attrs': {'type': 'astra_1d'}, 'data': dat}
+
     def write_astra_3d(self, common_filePath, verbose=False):      
         return  write_astra_3d_fieldmaps(self, common_filePath)
           
         
     @functools.wraps(create_impact_solrf_ele)      
     def to_impact_solrf(self, *args, **kwargs):
         return create_impact_solrf_ele(self, *args, **kwargs)
```

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/ansys.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/ansys.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/astra.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/astra.py`

 * *Files 13% similar despite different names*

```diff
@@ -149,15 +149,18 @@
 
     
     # Reference particle
     ref_particle = {'q':0}
     sigma = {}
     for k in ['x', 'y', 'z', 'px', 'py', 'pz', 't']:
         ref_particle[k] = particle_group.avg(k)
-        sigma[k] =  particle_group.std(k)
+        std = particle_group.std(k)
+        if std == 0:
+            std = 1e-12 # Give some size
+        sigma[k] = std
     ref_particle['t'] *= 1e9 # s -> nS
         
     # Make structured array
     dtype = np.dtype(list(zip(names, types)))
     data = np.zeros(size, dtype=dtype)
     for k in ['x', 'y', 'z', 'px', 'py', 'pz', 't']:
         data[k][i_start:] = getattr(particle_group, k)
@@ -199,21 +202,101 @@
         data[1]['x'] = 0.5*sigma['x'];data[1]['t'] =  0.5*sigma['t']
         data[2]['y'] = 0.5*sigma['y'];data[2]['t'] = -0.5*sigma['t']
         data[3]['x'] = 1.0*sigma['x'];data[3]['t'] =  sigma['t']
         data[4]['y'] = 1.0*sigma['y'];data[4]['t'] = -sigma['t']
         data[5]['x'] = 1.5*sigma['x'];data[5]['t'] =  1.5*sigma['t']
         data[6]['y'] = 1.5*sigma['y'];data[6]['t'] = -1.5*sigma['t']        
         data[1:7]['status'] = -3
+        data[1:7]['q'] = 0.5e-5 # ? Seems to be required 
         data[1:7]['pz'] = 0 #? This is what the Astra Generator does
     
     # Save in the 'high_res = T' format
     np.savetxt(outfile, data, fmt = ' '.join(8*['%20.12e']+2*['%4i']))
 
     
     
+    
+def write_astra_1d_fieldmap(fm, filePath): 
+    """
+    Writes an Astra fieldmap file from a FieldMesh object.
+    
+    Requires cylindrical geometry for now.
+    
+    Parameters
+    ----------
+    filePath: str
+        Filename to write to
+
+    """
+    
+    z, fz = astra_1d_fieldmap_data(fm)
+    
+    # Flatten dat   
+    dat = np.array([z, fz]).T    
+    
+    np.savetxt(filePath, dat, comments='') 
+    
+    
+    
+def astra_1d_fieldmap_data(fm): 
+    """
+    Astra fieldmap data.
+    
+    Requires cylindrical geometry for now.
+    
+    Returns
+    -------
+    z: array-like
+        z coordinate in meters
+    
+    fz: array-like
+        field amplitude corresponding to z
+    
+    """    
+    
+    
+    assert fm.geometry == 'cylindrical', f'Geometry: {fm.geometry} not implemented'
+    
+    assert fm.shape[1] == 1, 'Cylindrical symmetry required'
+    
+    dat = {}
+    z = fm.coord_vec('z')
+    
+    if fm.is_static:
+        if fm.is_pure_magnetic:
+            fz = np.real(fm['Bz'][0,0,:])
+        elif fm.is_pure_electric:
+            fz = np.real(fm['Ez'][0,0,:])           
+        else:
+            raise ValueError('Mixed static field TODO')
+            
+    else:
+        # Assume RF cavity, rotate onto the real axis
+        # Get complex fields
+        fz = fm.Ez[0,0,:]
+        
+        # Get imaginary argument (angle)
+        iangle = np.unique(np.mod(np.angle(fz), np.pi))
+    
+        # Make sure there is only one
+        assert len(iangle) == 1, print(iangle)
+        iangle = iangle[0]
+        
+        if iangle != 0:
+            rot = np.exp(-1j*iangle)
+            # print(f'Rotating complex field by {-iangle}')
+        else:
+            rot = 1   
+        fz = np.real(fz*rot)
+            
+    return z, fz  
+    
+    
+    
+    
 def vec_spacing(vec):
     """
     Returns the spacing and minimum of a coordinate.
     Asserts that the spacing is uniform
     """
     vmin = vec.min()
     vmax = vec.max()
```

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/bmad.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/bmad.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/elegant.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/elegant.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/genesis.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/genesis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/gpt.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/gpt.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/impact.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/impact.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/litrack.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/litrack.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/lucretia.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/lucretia.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/opal.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/opal.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/simion.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/simion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/superfish.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/interfaces/superfish.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/labels.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/labels.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/particles.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/particles.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,16 +755,17 @@
             t = self.avg('t')
         dt = t - self.t
         self.drift(dt)
         # Fix t to be exactly this value
         self.t = np.full(self.n_particle, t)
     
     # Writers
-    def write_astra(self, filePath, verbose=False):
-        write_astra(self, filePath, verbose=verbose)
+    @functools.wraps(write_astra)    
+    def write_astra(self, filePath, verbose=False, probe=False):
+        write_astra(self, filePath, verbose=verbose, probe=probe)
         
     def write_bmad(self, filePath, p0c=None, t_ref=0, verbose=False):
         write_bmad(self, filePath, p0c=p0c, t_ref=t_ref, verbose=verbose)        
 
     def write_elegant(self, filePath, verbose=False):
         write_elegant(self, filePath, verbose=verbose)
```

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/plot.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/plot.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/readers.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/readers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/species.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/species.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/statistics.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/statistics.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/tools.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/tools.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/units.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/units.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/pmd_beamphysics/writers.py` & `openpmd-beamphysics-0.7.8/pmd_beamphysics/writers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/setup.py` & `openpmd-beamphysics-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/tests/test_particlegroup.py` & `openpmd-beamphysics-0.7.8/tests/test_particlegroup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.7/versioneer.py` & `openpmd-beamphysics-0.7.8/versioneer.py`

 * *Files identical despite different names*

