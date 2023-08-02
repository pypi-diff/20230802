# Comparing `tmp/alvadescpy-0.1.2.tar.gz` & `tmp/alvadescpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alvadescpy-0.1.2.tar", last modified: Fri Apr  2 01:32:03 2021, max compression
+gzip compressed data, was "alvadescpy-0.1.3.tar", last modified: Wed Aug  2 03:55:03 2023, max compression
```

## Comparing `alvadescpy-0.1.2.tar` & `alvadescpy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-04-02 01:32:03.175993 alvadescpy-0.1.2/
--rw-r--r--   0 tjkessler   (501) staff       (20)      262 2021-04-02 01:32:03.175840 alvadescpy-0.1.2/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)     3782 2021-03-25 21:24:07.000000 alvadescpy-0.1.2/README.md
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-04-02 01:32:03.174854 alvadescpy-0.1.2/alvadescpy/
--rw-r--r--   0 tjkessler   (501) staff       (20)      155 2021-04-02 01:30:25.000000 alvadescpy-0.1.2/alvadescpy/__init__.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     1360 2021-04-02 01:30:28.000000 alvadescpy-0.1.2/alvadescpy/functions.py
--rw-r--r--   0 tjkessler   (501) staff       (20)     6818 2021-04-02 01:30:18.000000 alvadescpy-0.1.2/alvadescpy/wrapper.py
-drwxr-xr-x   0 tjkessler   (501) staff       (20)        0 2021-04-02 01:32:03.175664 alvadescpy-0.1.2/alvadescpy.egg-info/
--rw-r--r--   0 tjkessler   (501) staff       (20)      262 2021-04-02 01:32:03.000000 alvadescpy-0.1.2/alvadescpy.egg-info/PKG-INFO
--rw-r--r--   0 tjkessler   (501) staff       (20)      256 2021-04-02 01:32:03.000000 alvadescpy-0.1.2/alvadescpy.egg-info/SOURCES.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2021-04-02 01:32:03.000000 alvadescpy-0.1.2/alvadescpy.egg-info/dependency_links.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)        1 2021-03-25 21:25:29.000000 alvadescpy-0.1.2/alvadescpy.egg-info/not-zip-safe
--rw-r--r--   0 tjkessler   (501) staff       (20)       11 2021-04-02 01:32:03.000000 alvadescpy-0.1.2/alvadescpy.egg-info/top_level.txt
--rw-r--r--   0 tjkessler   (501) staff       (20)       38 2021-04-02 01:32:03.176055 alvadescpy-0.1.2/setup.cfg
--rw-r--r--   0 tjkessler   (501) staff       (20)      368 2021-04-02 01:30:22.000000 alvadescpy-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:55:03.702370 alvadescpy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 03:55:03.702370 alvadescpy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:55:03.702370 alvadescpy-0.1.3/alvadescpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/alvadescpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/alvadescpy/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/alvadescpy/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 03:55:03.702370 alvadescpy-0.1.3/alvadescpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-08-02 03:55:03.000000 alvadescpy-0.1.3/alvadescpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 03:55:03.000000 alvadescpy-0.1.3/alvadescpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 03:55:03.000000 alvadescpy-0.1.3/alvadescpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 03:55:03.000000 alvadescpy-0.1.3/alvadescpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 03:54:52.000000 alvadescpy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 03:55:03.702370 alvadescpy-0.1.3/setup.cfg
```

### Comparing `alvadescpy-0.1.2/README.md` & `alvadescpy-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![UML Energy & Combustion Research Laboratory](http://faculty.uml.edu/Hunter_Mack/uploads/9/7/1/3/97138798/1481826668_2.png)](http://faculty.uml.edu/Hunter_Mack/)
+[![UML Energy & Combustion Research Laboratory](https://sites.uml.edu/hunter-mack/files/2021/11/ECRL_final.png)](http://faculty.uml.edu/Hunter_Mack/)
 
 # alvaDescPy: A Python wrapper for alvaDesc software
 
 [![GitHub version](https://badge.fury.io/gh/ecrl%2Falvadescpy.svg)](https://badge.fury.io/gh/ecrl%2Falvadescpy)
 [![PyPI version](https://badge.fury.io/py/alvadescpy.svg)](https://badge.fury.io/py/alvadescpy)
 [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/ecrl/alvadescpy/master/LICENSE.txt)
 
@@ -17,15 +17,15 @@
 ```
 
 Installation via cloned repository:
 
 ```
 $ git clone https://github.com/ecrl/alvadescpy
 $ cd alvadescpy
-$ python setup.py install
+$ pip install .
 ```
 
 There are currently no additional dependencies for alvaDescPy, however it requires a valid, licensed installation of [alvaDesc](https://www.alvascience.com/alvadesc/).
 
 ## Basic Usage
 
 alvaDescPy assumes the location of alvaDesc's command-line interface is located at your OS's default location. If alvaDesc is located in a different location, you can change the path:
```

### Comparing `alvadescpy-0.1.2/alvadescpy/functions.py` & `alvadescpy-0.1.3/alvadescpy/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # stdlib. imports
 from typing import TypeVar
 
 # alvadescpy imports
 from alvadescpy import alvadesc
 
 # custom argument and return variables
-_DESC = TypeVar('_DESC', str, list)
-_RET_VAL = TypeVar('_RET_VAL', dict, list)
+str_or_list = TypeVar('str_or_list', str, list)
+list_or_dict = TypeVar('list_or_dict', dict, list)
 
 
-def smiles_to_descriptors(smiles: str, descriptors: _DESC='ALL',
-                          labels: bool=True) -> _RET_VAL:
+def smiles_to_descriptors(smiles: str_or_list,
+                          descriptors: str_or_list = 'ALL',
+                          labels: bool = True) -> list_or_dict:
     ''' smiles_to_descriptors: returns molecular descriptors for a given
     molecule (represented by its SMILES string)
 
     Args:
         smiles (str, list): SMILES string for a given molecule
         descriptors (str, list): `ALL` for all descriptors, or list containing
             individual descriptors (str's)
@@ -33,10 +34,12 @@
 
     Returns:
         list, dict: returns a list of descriptor values if `labels` is False,
             else a dict
     '''
 
     if type(smiles) == list:
-        return [alvadesc(ismiles=smi, descriptors=descriptors, labels=labels)[0]
-                for smi in smiles]
+        return [
+            alvadesc(ismiles=smi, descriptors=descriptors, labels=labels)[0]
+            for smi in smiles
+        ]
     return alvadesc(ismiles=smiles, descriptors=descriptors, labels=labels)[0]
```

### Comparing `alvadescpy-0.1.2/alvadescpy/wrapper.py` & `alvadescpy-0.1.3/alvadescpy/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 # v.0.1.2
 # Developed in 2019 by Travis Kessler <travis.j.kessler@gmail.com>
 #
 # contains `alvadesc` function, a wrapper for alvaDesc software
 #
 
 # stdlib. imports
-from subprocess import check_output, PIPE, Popen, call
-from csv import writer, QUOTE_ALL
+from subprocess import PIPE, Popen
 from typing import TypeVar
 import platform
-from os.path import realpath
 
 # path to alvaDesc command line interface executable
 CONFIG = {
     'alvadesc_path': None
 }
 plt = platform.system()
 if plt == 'Windows':
-    CONFIG['alvadesc_path'] = 'C:\\Program Files\\Alvascience\\alvaDesc\\alvaDescCLI.exe'
+    CONFIG['alvadesc_path'] = 'C:\\Program Files\\Alvascience\\alvaDesc\\\
+alvaDescCLI.exe'
 elif plt == 'Darwin':
-    CONFIG['alvadesc_path'] = '/Applications/alvaDesc.app/Contents/MacOS/alvaDescCLI'
+    CONFIG['alvadesc_path'] = '/Applications/alvaDesc.app/Contents/MacOS/\
+alvaDescCLI'
 elif plt == 'Linux':
     CONFIG['alvadesc_path'] = '/usr/bin/alvaDescCLI'
 else:
     raise RuntimeError('Unknown/unsupported operating system: {}'.format(plt))
 
 # custom argument variable (either str or list)
-_DESC = TypeVar('_DESC', str, list)
+str_or_list = TypeVar('str_or_list', str, list)
 
 
 def _sub_call(command: str) -> list:
     ''' _sub_call: calls alvaDesc via subprocess.Popen
 
     Args:
         command (str): command to execute
@@ -50,20 +50,23 @@
             exception, CONFIG['alvadesc_path']
         ))
     except Exception as exception:
         raise Exception('{}'.format(exception))
     return p.communicate()[0].decode('utf-8')
 
 
-def alvadesc(script: str=None, ismiles: str=None, input_file: str=None,
-             inputtype: str=None, descriptors: _DESC=None, labels: bool=False,
-             ecfp: bool=False, pfp: bool=False, fpsize: int=1024, fpmin: int=0,
-             fpmax: int=2, count: bool=True, bits: int=2, fpoptions: str=None,
-             maccsfp: bool=False, output: str=None, threads: int=None) -> list:
-    ''' alvadesc: calls alvaDesc's command line interface; supports all arguments
+def alvadesc(script: str = None, ismiles: str = None, input_file: str = None,
+             inputtype: str = None, descriptors: str_or_list = None,
+             labels: bool = False, ecfp: bool = False, pfp: bool = False,
+             fpsize: int = 1024, fpmin: int = 0, fpmax: int = 2,
+             count: bool = True, bits: int = 2, fpoptions: str = None,
+             maccsfp: bool = False, output: str = None,
+             threads: int = None) -> list:
+    ''' alvadesc: calls alvaDesc's command line interface; supports all
+    arguments
 
     Args:
         script (str): path to script file containing all available options; if
             supplied, nothing else should be supplied
         ismiles (str): use a single SMILES string as input
         input_file (str): uses a set of molecules in this file as inputs
         inputtype (str): if `input_file` is supplied, this is mandatory (e.g.
```

