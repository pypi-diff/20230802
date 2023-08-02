# Comparing `tmp/jupyternb-setup-1.3.5.tar.gz` & `tmp/jupyternb-setup-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyternb-setup-1.3.5.tar", last modified: Wed Jun  7 01:47:51 2023, max compression
+gzip compressed data, was "jupyternb-setup-1.3.6.tar", last modified: Wed Aug  2 14:25:56 2023, max compression
```

## Comparing `jupyternb-setup-1.3.5.tar` & `jupyternb-setup-1.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1806 2023-06-01 18:13:01.086115 jupyternb-setup-1.3.5/.gitignore
--rw-r--r--   0        0        0     1071 2023-06-01 17:22:55.849765 jupyternb-setup-1.3.5/LICENSE
--rw-r--r--   0        0        0     4667 2023-06-01 17:22:55.850054 jupyternb-setup-1.3.5/README.md
--rw-r--r--   0        0        0       48 2023-06-07 01:39:34.185379 jupyternb-setup-1.3.5/jupyternb/__init__.py
--rw-r--r--   0        0        0    15458 2023-06-07 01:39:26.326953 jupyternb-setup-1.3.5/jupyternb/jupyter_startup.py
--rw-r--r--   0        0        0      977 2023-06-01 18:23:33.328333 jupyternb-setup-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1806 2023-08-02 14:23:27.952914 jupyternb-setup-1.3.6/.gitignore
+-rw-r--r--   0        0        0     1071 2023-08-02 14:23:27.953109 jupyternb-setup-1.3.6/LICENSE
+-rw-r--r--   0        0        0     4667 2023-08-02 14:23:27.953290 jupyternb-setup-1.3.6/README.md
+-rw-r--r--   0        0        0       48 2023-08-02 14:25:42.939141 jupyternb-setup-1.3.6/jupyternb/__init__.py
+-rw-r--r--   0        0        0    15545 2023-08-02 14:25:42.933050 jupyternb-setup-1.3.6/jupyternb/jupyter_startup.py
+-rw-r--r--   0        0        0      977 2023-08-02 14:23:27.953869 jupyternb-setup-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 jupyternb-setup-1.3.6/PKG-INFO
```

### Comparing `jupyternb-setup-1.3.5/.gitignore` & `jupyternb-setup-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.5/LICENSE` & `jupyternb-setup-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.5/README.md` & `jupyternb-setup-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.5/jupyternb/jupyter_startup.py` & `jupyternb-setup-1.3.6/jupyternb/jupyter_startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,16 @@
             traceback.print_exc()
 
     def update_permissions(self):
         """
         Find the location of the key files and change their permission
         :return:
         """
+        if not os.path.exists(f"{self.config_location}/fabric_rc"):
+            return
         # Open the file in read mode
         with open(f"{self.config_location}/fabric_rc", 'r') as file:
             # Read the content of the file
             content = file.read()
 
         # Split the content into lines
         lines = content.splitlines()
```

### Comparing `jupyternb-setup-1.3.5/pyproject.toml` & `jupyternb-setup-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyternb-setup-1.3.5/PKG-INFO` & `jupyternb-setup-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyternb-setup
-Version: 1.3.5
+Version: 1.3.6
 Summary: Fabric Jupyter Notebook Container Setup
 Keywords: Fabric Jupyter Notebook Container Setup,Jupyter Hub,Jupyter Notebook
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

