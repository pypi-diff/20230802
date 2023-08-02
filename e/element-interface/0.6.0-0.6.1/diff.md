# Comparing `tmp/element-interface-0.6.0.tar.gz` & `tmp/element-interface-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "element-interface-0.6.0.tar", last modified: Thu Jul 27 15:38:44 2023, max compression
+gzip compressed data, was "element-interface-0.6.1.tar", last modified: Wed Aug  2 18:37:19 2023, max compression
```

## Comparing `element-interface-0.6.0.tar` & `element-interface-0.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 15:38:39.000000 element-interface-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-27 15:38:44.539561 element-interface-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-27 15:38:39.000000 element-interface-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/element_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/caiman_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/dandi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/extract_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/extract_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/prairie_view_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/run_caiman.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/scanimage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/suite2p_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/suite2p_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-27 15:38:39.000000 element-interface-0.6.0/element_interface/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 15:38:44.539561 element-interface-0.6.0/element_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 15:38:44.000000 element-interface-0.6.0/element_interface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 15:38:44.539561 element-interface-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-27 15:38:39.000000 element-interface-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:37:19.508216 element-interface-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 18:37:15.000000 element-interface-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 18:37:19.504216 element-interface-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-02 18:37:15.000000 element-interface-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:37:19.504216 element-interface-0.6.1/element_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12565 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/caiman_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/dandi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/extract_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/extract_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/prairie_view_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/run_caiman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/scanimage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/suite2p_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/suite2p_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-02 18:37:15.000000 element-interface-0.6.1/element_interface/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:37:19.504216 element-interface-0.6.1/element_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-02 18:37:19.000000 element-interface-0.6.1/element_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 18:37:19.000000 element-interface-0.6.1/element_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:37:19.000000 element-interface-0.6.1/element_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 18:37:19.000000 element-interface-0.6.1/element_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 18:37:19.000000 element-interface-0.6.1/element_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 18:37:19.508216 element-interface-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-02 18:37:15.000000 element-interface-0.6.1/setup.py
```

### Comparing `element-interface-0.6.0/LICENSE` & `element-interface-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/PKG-INFO` & `element-interface-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-interface
-Version: 0.6.0
+Version: 0.6.1
 Summary: Loaders of neurophysiological data into the DataJoint Elements
 Home-page: https://github.com/datajoint/element-interface
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-interface-0.6.0/README.md` & `element-interface-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/caiman_loader.py` & `element-interface-0.6.1/element_interface/caiman_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/dandi.py` & `element-interface-0.6.1/element_interface/dandi.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,58 +8,59 @@
 def upload_to_dandi(
     data_directory: str,
     dandiset_id: str,
     staging: bool = True,
     working_directory: str = None,
     api_key: str = None,
     sync: bool = False,
+    existing: str = "refresh",
 ):
     """Upload NWB files to DANDI Archive
 
     Args:
         data_directory (str): directory that contains source data
         dandiset_id (str): 6-digit zero-padded string
         staging (bool): If true, use staging server. If false, use production server.
         working_directory (str, optional): Dir in which to create symlinked dandiset.
             Must have write permissions to this directory. Default is current directory.
         api_key (str, optional): Provide the DANDI API key if not already in an
             environmental variable DANDI_API_KEY
         sync (str, optional): If True, delete all files in archive that are not present
             in the local directory.
+        existing (str, optional): see full description from `dandi upload --help`
     """
 
     working_directory = working_directory or os.path.curdir
 
     if api_key is not None:
         os.environ["DANDI_API_KEY"] = api_key
 
     dandiset_directory = os.path.join(
         working_directory, str(dandiset_id)
     )  # enforce str
 
-    download(
-        f"https://gui-staging.dandiarchive.org/#/dandiset/{dandiset_id}"
-        if staging
-        else f"https://dandiarchive.org/dandiset/{dandiset_id}",
-        output_dir=working_directory,
+    dandiset_url = f"https://gui-staging.dandiarchive.org/#/dandiset/{dandiset_id}" if staging else f"https://dandiarchive.org/dandiset/{dandiset_id}/draft"
+
+    subprocess.run(
+        ["dandi", "download", "--download", "dandiset.yaml", "-o", working_directory, dandiset_url],
+        shell=True, 
     )
 
     subprocess.run(
         ["dandi", "organize", "-d", dandiset_directory, data_directory, "-f", "dry"],
         shell=True,  # without this param, subprocess interprets first arg as file/dir
     )
 
     subprocess.run(
         ["dandi", "organize", "-d", dandiset_directory, data_directory], shell=True
     )
 
-    print(
-        f"work_dir: {working_directory}\ndata_dir: {data_directory}\n"
-        + f"dand_dir: {dandiset_directory}"
+    subprocess.run(
+        ["dandi", "validate", dandiset_directory], shell=True
     )
 
     upload(
-        [dandiset_directory],
-        # dandiset_path=dandiset_directory, # dandi.upload has no such arg
+        paths=[dandiset_directory],
         dandi_instance="dandi-staging" if staging else "dandi",
+        existing=existing,
         sync=sync,
     )
```

### Comparing `element-interface-0.6.0/element_interface/extract_loader.py` & `element-interface-0.6.1/element_interface/extract_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/extract_trigger.py` & `element-interface-0.6.1/element_interface/extract_trigger.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/prairie_view_loader.py` & `element-interface-0.6.1/element_interface/prairie_view_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/run_caiman.py` & `element-interface-0.6.1/element_interface/run_caiman.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/scanimage_utils.py` & `element-interface-0.6.1/element_interface/scanimage_utils.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/suite2p_loader.py` & `element-interface-0.6.1/element_interface/suite2p_loader.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/suite2p_trigger.py` & `element-interface-0.6.1/element_interface/suite2p_trigger.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface/utils.py` & `element-interface-0.6.1/element_interface/utils.py`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/element_interface.egg-info/PKG-INFO` & `element-interface-0.6.1/element_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: element-interface
-Version: 0.6.0
+Version: 0.6.1
 Summary: Loaders of neurophysiological data into the DataJoint Elements
 Home-page: https://github.com/datajoint/element-interface
 Author: DataJoint
 Author-email: info@datajoint.com
 License: MIT
 Keywords: neuroscience calcium-imaging science datajoint
 Platform: UNKNOWN
```

### Comparing `element-interface-0.6.0/element_interface.egg-info/SOURCES.txt` & `element-interface-0.6.1/element_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `element-interface-0.6.0/setup.py` & `element-interface-0.6.1/setup.py`

 * *Files identical despite different names*

