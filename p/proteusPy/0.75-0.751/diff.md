# Comparing `tmp/proteusPy-0.75.tar.gz` & `tmp/proteusPy-0.751.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteusPy-0.75.tar", last modified: Thu Jul 27 18:06:24 2023, max compression
+gzip compressed data, was "proteusPy-0.751.tar", last modified: Wed Aug  2 00:59:42 2023, max compression
```

## Comparing `proteusPy-0.75.tar` & `proteusPy-0.751.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.369599 proteusPy-0.75/
--rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.75/MANIFEST.in
--rw-r--r--   0 egs        (505) staff       (20)     5087 2023-07-27 18:06:24.369661 proteusPy-0.75/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)     4000 2023-07-26 00:26:52.000000 proteusPy-0.75/README.md
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.366454 proteusPy-0.75/proteusPy/
--rw-r--r--   0 egs        (505) staff       (20)    93581 2023-07-16 03:29:22.000000 proteusPy-0.75/proteusPy/Disulfide.py
--rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.75/proteusPy/DisulfideClass_Constructor.py
--rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.75/proteusPy/DisulfideClasses.py
--rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.75/proteusPy/DisulfideExceptions.py
--rw-r--r--   0 egs        (505) staff       (20)    38194 2023-07-13 01:45:02.000000 proteusPy-0.75/proteusPy/DisulfideList.py
--rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.75/proteusPy/DisulfideLoader.py
--rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.75/proteusPy/ProteusGlobals.py
--rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.75/proteusPy/ProteusPyWarning.py
--rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.75/proteusPy/Residue.py
--rw-r--r--   0 egs        (505) staff       (20)     1641 2023-07-13 01:45:45.000000 proteusPy-0.75/proteusPy/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.75/proteusPy/angle_annotation.py
--rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.75/proteusPy/atoms.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.369269 proteusPy-0.75/proteusPy/data/
--rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.75/proteusPy/data/__init__.py
--rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.75/proteusPy/data/ss_completed.txt
--rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.75/proteusPy/data/ss_ids.txt
--rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.75/proteusPy/data/ss_query.json
--rw-r--r--   0 egs        (505) staff       (20)    21225 2023-07-15 22:25:26.000000 proteusPy-0.75/proteusPy/turtle3D.py
--rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.75/proteusPy/utility.py
-drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-07-27 18:06:24.367402 proteusPy-0.75/proteusPy.egg-info/
--rw-r--r--   0 egs        (505) staff       (20)     5087 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/PKG-INFO
--rw-r--r--   0 egs        (505) staff       (20)      744 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/SOURCES.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/dependency_links.txt
--rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.75/proteusPy.egg-info/not-zip-safe
--rw-r--r--   0 egs        (505) staff       (20)       10 2023-07-27 18:06:24.000000 proteusPy-0.75/proteusPy.egg-info/top_level.txt
--rw-r--r--   0 egs        (505) staff       (20)      107 2023-07-27 18:06:24.370121 proteusPy-0.75/setup.cfg
--rw-r--r--   0 egs        (505) staff       (20)     3522 2023-07-13 00:54:34.000000 proteusPy-0.75/setup.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-08-02 00:59:42.094851 proteusPy-0.751/
+-rw-r--r--   0 egs        (505) staff       (20)       65 2023-07-09 01:16:52.000000 proteusPy-0.751/MANIFEST.in
+-rw-r--r--   0 egs        (505) staff       (20)     5110 2023-08-02 00:59:42.094956 proteusPy-0.751/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)     4022 2023-07-27 18:09:40.000000 proteusPy-0.751/README.md
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-08-02 00:59:42.076212 proteusPy-0.751/proteusPy/
+-rw-r--r--   0 egs        (505) staff       (20)    93580 2023-08-02 00:57:07.000000 proteusPy-0.751/proteusPy/Disulfide.py
+-rw-r--r--   0 egs        (505) staff       (20)    20687 2023-03-20 23:29:05.000000 proteusPy-0.751/proteusPy/DisulfideClass_Constructor.py
+-rw-r--r--   0 egs        (505) staff       (20)    17282 2023-03-23 00:51:13.000000 proteusPy-0.751/proteusPy/DisulfideClasses.py
+-rw-r--r--   0 egs        (505) staff       (20)     1027 2023-07-11 00:53:43.000000 proteusPy-0.751/proteusPy/DisulfideExceptions.py
+-rw-r--r--   0 egs        (505) staff       (20)    37855 2023-07-27 18:59:10.000000 proteusPy-0.751/proteusPy/DisulfideList.py
+-rw-r--r--   0 egs        (505) staff       (20)    23705 2023-07-06 15:13:40.000000 proteusPy-0.751/proteusPy/DisulfideLoader.py
+-rw-r--r--   0 egs        (505) staff       (20)      830 2023-07-03 22:51:19.000000 proteusPy-0.751/proteusPy/ProteusGlobals.py
+-rw-r--r--   0 egs        (505) staff       (20)      395 2022-12-04 05:59:19.000000 proteusPy-0.751/proteusPy/ProteusPyWarning.py
+-rw-r--r--   0 egs        (505) staff       (20)     4934 2023-02-21 01:14:53.000000 proteusPy-0.751/proteusPy/Residue.py
+-rw-r--r--   0 egs        (505) staff       (20)     1642 2023-08-02 00:58:40.000000 proteusPy-0.751/proteusPy/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)    13442 2023-03-09 14:54:17.000000 proteusPy-0.751/proteusPy/angle_annotation.py
+-rw-r--r--   0 egs        (505) staff       (20)     1297 2023-02-10 03:20:34.000000 proteusPy-0.751/proteusPy/atoms.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-08-02 00:59:42.094396 proteusPy-0.751/proteusPy/data/
+-rw-r--r--   0 egs        (505) staff       (20)     2687 2023-07-04 13:46:04.000000 proteusPy-0.751/proteusPy/data/__init__.py
+-rw-r--r--   0 egs        (505) staff       (20)     8670 2022-12-12 14:44:16.000000 proteusPy-0.751/proteusPy/data/ss_completed.txt
+-rw-r--r--   0 egs        (505) staff       (20)   191074 2022-11-27 00:05:31.000000 proteusPy-0.751/proteusPy/data/ss_ids.txt
+-rw-r--r--   0 egs        (505) staff       (20)      800 2023-02-05 06:37:57.000000 proteusPy-0.751/proteusPy/data/ss_query.json
+-rw-r--r--   0 egs        (505) staff       (20)    21225 2023-07-15 22:25:26.000000 proteusPy-0.751/proteusPy/turtle3D.py
+-rw-r--r--   0 egs        (505) staff       (20)    12468 2023-07-11 00:53:43.000000 proteusPy-0.751/proteusPy/utility.py
+drwxr-xr-x   0 egs        (505) staff       (20)        0 2023-08-02 00:59:42.088669 proteusPy-0.751/proteusPy.egg-info/
+-rw-r--r--   0 egs        (505) staff       (20)     5110 2023-08-02 00:59:41.000000 proteusPy-0.751/proteusPy.egg-info/PKG-INFO
+-rw-r--r--   0 egs        (505) staff       (20)      744 2023-08-02 00:59:42.000000 proteusPy-0.751/proteusPy.egg-info/SOURCES.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-08-02 00:59:41.000000 proteusPy-0.751/proteusPy.egg-info/dependency_links.txt
+-rw-r--r--   0 egs        (505) staff       (20)        1 2023-07-02 20:10:40.000000 proteusPy-0.751/proteusPy.egg-info/not-zip-safe
+-rw-r--r--   0 egs        (505) staff       (20)       10 2023-08-02 00:59:41.000000 proteusPy-0.751/proteusPy.egg-info/top_level.txt
+-rw-r--r--   0 egs        (505) staff       (20)      107 2023-08-02 00:59:42.095238 proteusPy-0.751/setup.cfg
+-rw-r--r--   0 egs        (505) staff       (20)     3522 2023-07-13 00:54:34.000000 proteusPy-0.751/setup.py
```

### Comparing `proteusPy-0.75/PKG-INFO` & `proteusPy-0.751/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.75
+Version: 0.751
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
@@ -20,48 +20,52 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-*proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+# Summary
+
+**proteusPy** is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+
+## Virtual Environment Creation
 
-# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
-2. *Build the environment.* 
+2. *Build the environment.*
    It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
-       - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: 
-         ```
+       - <https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage>
+       - From a shell prompt:
+
+         ```console
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
           $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-  ```
-I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining.
+
+## General Usage
 
-### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
-### The Future
+## The Future
+
 I am continuing to explore the initial disulfide structural classes gleaned from Hogg *et al.* further using the sextant class approach. This offers much higher class resolution and reveals subgroups within the broad class. I'd also like to explore the catalytic and allosteric classes in more detail to look for common structural elements.
 
-### Publications
-* https://doi.org/10.1021/bi00368a023
-* https://doi.org/10.1021/bi00368a024
-* https://doi.org/10.1016/0092-8674(92)90140-8
-* http://dx.doi.org/10.2174/092986708783330566
+## Publications
 
+- <https://doi.org/10.1021/bi00368a023>
+- <https://doi.org/10.1021/bi00368a024>
+- <https://doi.org/10.1016/0092-8674(92)90140-8>
+- <http://dx.doi.org/10.2174/092986708783330566>
 
 *NB:* This distribution is being developed slowly. proteusPy relies on my fork of the ``Bio`` Python package to download and build the database. As a result, one can't download and create the database locally unless the BioPython patch is applied. The changed python file is in the repo's data directory - ``parse_pdb_header.py``. Database analysis is unaffected without the patch. Also, if you're running on an M-series Mac then it's important to install Biopython first, since the generic release won't build on the M1. 7/4/23 -egs-
 
 Eric G. Suchanek, PhD., <mailto:suchanek@mac.com>
-
```

### Comparing `proteusPy-0.75/README.md` & `proteusPy-0.751/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-*proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+# Summary
+
+**proteusPy** is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+
+## Virtual Environment Creation
 
-# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
-2. *Build the environment.* 
+2. *Build the environment.*
    It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
-       - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: 
-         ```
+       - <https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage>
+       - From a shell prompt:
+
+         ```console
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
           $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-  ```
-I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining.
+
+## General Usage
 
-### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
-### The Future
+## The Future
+
 I am continuing to explore the initial disulfide structural classes gleaned from Hogg *et al.* further using the sextant class approach. This offers much higher class resolution and reveals subgroups within the broad class. I'd also like to explore the catalytic and allosteric classes in more detail to look for common structural elements.
 
-### Publications
-* https://doi.org/10.1021/bi00368a023
-* https://doi.org/10.1021/bi00368a024
-* https://doi.org/10.1016/0092-8674(92)90140-8
-* http://dx.doi.org/10.2174/092986708783330566
+## Publications
 
+- <https://doi.org/10.1021/bi00368a023>
+- <https://doi.org/10.1021/bi00368a024>
+- <https://doi.org/10.1016/0092-8674(92)90140-8>
+- <http://dx.doi.org/10.2174/092986708783330566>
 
 *NB:* This distribution is being developed slowly. proteusPy relies on my fork of the ``Bio`` Python package to download and build the database. As a result, one can't download and create the database locally unless the BioPython patch is applied. The changed python file is in the repo's data directory - ``parse_pdb_header.py``. Database analysis is unaffected without the patch. Also, if you're running on an M-series Mac then it's important to install Biopython first, since the generic release won't build on the M1. 7/4/23 -egs-
 
 Eric G. Suchanek, PhD., <mailto:suchanek@mac.com>
-
```

### Comparing `proteusPy-0.75/proteusPy/Disulfide.py` & `proteusPy-0.751/proteusPy/Disulfide.py`

 * *Files 0% similar despite different names*

```diff
@@ -1134,15 +1134,15 @@
         the cutoff (Å) in the others list.
 
         :param others: DisulfideList to search
         :param cutoff: Distance cutoff (Å)
         :return: DisulfideList within the cutoff
         '''
 
-        res = [ss.copy() for ss in others if self.Distance_RMS(ss) <= cutoff]
+        res = [ss.copy() for ss in others if self.Distance_RMS(ss) < cutoff]
         return DisulfideList(res, 'neighbors')
 
     
     def Distance_RMS(self, other) -> float:
         '''
         Calculate the RMS distance between the internal coordinates of self and another Disulfide.
         :param other: Comparison Disulfide
```

### Comparing `proteusPy-0.75/proteusPy/DisulfideClass_Constructor.py` & `proteusPy-0.751/proteusPy/DisulfideClass_Constructor.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/DisulfideClasses.py` & `proteusPy-0.751/proteusPy/DisulfideClasses.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/DisulfideExceptions.py` & `proteusPy-0.751/proteusPy/DisulfideExceptions.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/DisulfideList.py` & `proteusPy-0.751/proteusPy/DisulfideList.py`

 * *Files 2% similar despite different names*

```diff
@@ -698,28 +698,14 @@
         Returns the Disulfide with the given name from the list.
         '''
         for ss in self.data:
             if ss.name == name:
                 return ss.copy()  # or ss.copy() !!!
         return None
 
-    def Oget_by_name(self, name) -> Disulfide:
-        '''
-        Returns the Disulfide with the given name from the list.
-        '''
-        sslist = self.data
-        res = None
-
-        for ss in sslist:
-            id = ss.name
-            if id == name:
-                res = ss.copy()
-                break
-        return res
-    
     def get_chains(self):
         '''
         Return the chain IDs for chains within the given Disulfide.
         :return: Chain IDs for given Disulfide
         '''
 
         res_dict = {'xxx'}
```

### Comparing `proteusPy-0.75/proteusPy/DisulfideLoader.py` & `proteusPy-0.751/proteusPy/DisulfideLoader.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/ProteusGlobals.py` & `proteusPy-0.751/proteusPy/ProteusGlobals.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/Residue.py` & `proteusPy-0.751/proteusPy/Residue.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/__init__.py` & `proteusPy-0.751/proteusPy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Eric G. Suchanek, PhD., all rights reserved
 # Subject to the MIT public license.
 
 """
 .. include:: ../README.md
 """
 
-__version__ = "0.75"
+__version__ = "0.751"
 
 import sys
 import os
 import glob
 import warnings
 import copy
```

### Comparing `proteusPy-0.75/proteusPy/angle_annotation.py` & `proteusPy-0.751/proteusPy/angle_annotation.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/atoms.py` & `proteusPy-0.751/proteusPy/atoms.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/data/__init__.py` & `proteusPy-0.751/proteusPy/data/__init__.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/data/ss_completed.txt` & `proteusPy-0.751/proteusPy/data/ss_completed.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/data/ss_ids.txt` & `proteusPy-0.751/proteusPy/data/ss_ids.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/data/ss_query.json` & `proteusPy-0.751/proteusPy/data/ss_query.json`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/turtle3D.py` & `proteusPy-0.751/proteusPy/turtle3D.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy/utility.py` & `proteusPy-0.751/proteusPy/utility.py`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/proteusPy.egg-info/PKG-INFO` & `proteusPy-0.751/proteusPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteusPy
-Version: 0.75
+Version: 0.751
 Summary: proteusPy - Protein Structure Analysis and Modeling Tools
 Home-page: https://github.com/suchanek/proteusPy/
 Author: Eric G. Suchanek, PhD
 Author-email: suchanek@mac.com
 License: MIT
 Project-URL: Documentation, https://suchanek.github.io/proteusPy/
 Project-URL: Source, https://github.com/suchanek/proteusPy/
@@ -20,48 +20,52 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
-*proteusPy* is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+# Summary
+
+**proteusPy** is a Python package specializing in the modeling and analysis of proteins of known structure with an emphasis on Disulfide Bonds. This package reprises my molecular modeling program [Proteus](https://doi.org/10.1021/bi00368a023), and relies on the [Turtle3D](https://suchanek.github.io/proteusPy/proteusPy/turtle3D.html) class. The turtle implements the functions ``Move``, ``Roll``, ``Yaw``, ``Pitch`` and ``Turn`` for movement in a three-dimensional space. The [Disulfide](https://suchanek.github.io/proteusPy/proteusPy/Disulfide.html) class implements methods to analyze the protein structure stabilizing element known as a *Disulfide Bond*. This class and its underlying methods are being used to perform a structural analysis of over 35,800 disulfide-bond containing proteins in the RCSB protein data bank.
+
+## Virtual Environment Creation
 
-# Virtual Environment Creation
 1. *Install Anaconda (<http://anaconda.org>)*
-2. *Build the environment.* 
+2. *Build the environment.*
    It's simplest to clone the repo via github since it contains all of the notebooks, test programs and raw Disulfide databases. The source code distribution can be also be used from pyPi as a normal package, within your own environment.
    - From the gitHub repository:
      - Install git-lfs
-       - https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage
-       - From a shell prompt: 
-         ```
+       - <https://help.github.com/en/github/managing-large-files/installing-git-large-file-storage>
+       - From a shell prompt:
+
+         ```console
           $ git-lfs track "*.csv" "*.pkl" "*.mp4"
           $ git clone https://github.com/suchanek/proteusPy
           $ cd proteusPy
           $ conda env create --name proteusPy --file=proteusPy.yml
           $ conda activate proteusPy
           $ pip install .
           $ jupyter nbextension enable --py --sys-prefix widgetsnbextension
 
-  ```
-I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining. 
+I hope you enjoy using proteusPy and would love to hear any success/insights gleaned from it. The Disulfide database is unique as far as I know, and is ripe for mining.
+
+## General Usage
 
-### General Usage
 Once the package is installed one can use the existing notebooks for analysis of the RCSB Disulfide database. The ``notebooks`` directory contains all of my Jupyter notebooks and is a good place to start. The ``DisulfideAnalysis.ipynb`` notebook contains the first analysis paper. The ``programs`` subdirectory contains the primary programs for downloading the RCSB disulfide-containing structure files, (``DisulfideDownloader.py``), extracting the disulfides and creating the database loaders (``DisulfideExtractor.py``) and cluster analysis, (``DisulfideClass_Analysis.py``).
 
 The first time one loads the database via ``Load_PDB_SS()`` the system will attempt to download the full and subset database from my Google Drive. If this fails the system will attempt to rebuild the database from the repo's ``data`` subdirectory (not the package's). If you've downloaded from github this will work correctly. If you've installed from pyPi via ``pip`` it will fail.
 
-### The Future
+## The Future
+
 I am continuing to explore the initial disulfide structural classes gleaned from Hogg *et al.* further using the sextant class approach. This offers much higher class resolution and reveals subgroups within the broad class. I'd also like to explore the catalytic and allosteric classes in more detail to look for common structural elements.
 
-### Publications
-* https://doi.org/10.1021/bi00368a023
-* https://doi.org/10.1021/bi00368a024
-* https://doi.org/10.1016/0092-8674(92)90140-8
-* http://dx.doi.org/10.2174/092986708783330566
+## Publications
 
+- <https://doi.org/10.1021/bi00368a023>
+- <https://doi.org/10.1021/bi00368a024>
+- <https://doi.org/10.1016/0092-8674(92)90140-8>
+- <http://dx.doi.org/10.2174/092986708783330566>
 
 *NB:* This distribution is being developed slowly. proteusPy relies on my fork of the ``Bio`` Python package to download and build the database. As a result, one can't download and create the database locally unless the BioPython patch is applied. The changed python file is in the repo's data directory - ``parse_pdb_header.py``. Database analysis is unaffected without the patch. Also, if you're running on an M-series Mac then it's important to install Biopython first, since the generic release won't build on the M1. 7/4/23 -egs-
 
 Eric G. Suchanek, PhD., <mailto:suchanek@mac.com>
-
```

### Comparing `proteusPy-0.75/proteusPy.egg-info/SOURCES.txt` & `proteusPy-0.751/proteusPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteusPy-0.75/setup.py` & `proteusPy-0.751/setup.py`

 * *Files identical despite different names*

