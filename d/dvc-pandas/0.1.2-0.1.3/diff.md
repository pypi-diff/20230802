# Comparing `tmp/dvc-pandas-0.1.2.tar.gz` & `tmp/dvc-pandas-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-pandas-0.1.2.tar", last modified: Thu Jul 27 17:22:37 2023, max compression
+gzip compressed data, was "dvc-pandas-0.1.3.tar", last modified: Wed Aug  2 09:30:16 2023, max compression
```

## Comparing `dvc-pandas-0.1.2.tar` & `dvc-pandas-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/
--rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/LICENSE
--rw-rw-r--   0 jey       (1000) jey       (1000)      593 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/README.md
--rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.2/pyproject.toml
--rw-rw-r--   0 jey       (1000) jey       (1000)     1025 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/setup.cfg
--rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.2/setup.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/dvc_pandas/
--rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.2/src/dvc_pandas/__init__.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-07-26 16:41:53.000000 dvc-pandas-0.1.2/src/dvc_pandas/dataset.py
--rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.2/src/dvc_pandas/dvc.py
--rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.2/src/dvc_pandas/git.py
--rw-rw-r--   0 jey       (1000) jey       (1000)    14041 2023-07-27 16:44:40.000000 dvc-pandas-0.1.2/src/dvc_pandas/repository.py
-drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-07-27 17:22:37.593719 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/
--rw-rw-r--   0 jey       (1000) jey       (1000)      593 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 jey       (1000) jey       (1000)      366 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       91 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/requires.txt
--rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-07-27 17:22:37.000000 dvc-pandas-0.1.2/src/dvc_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-08-02 09:30:16.434660 dvc-pandas-0.1.3/
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1068 2021-04-06 11:20:04.000000 dvc-pandas-0.1.3/LICENSE
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-08-02 09:30:16.434660 dvc-pandas-0.1.3/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)       13 2021-04-06 11:20:04.000000 dvc-pandas-0.1.3/README.md
+-rw-rw-r--   0 jey       (1000) jey       (1000)      304 2022-02-09 06:54:41.000000 dvc-pandas-0.1.3/pyproject.toml
+-rw-rw-r--   0 jey       (1000) jey       (1000)     1025 2023-08-02 09:30:16.434660 dvc-pandas-0.1.3/setup.cfg
+-rw-rw-r--   0 jey       (1000) jey       (1000)      120 2021-04-06 11:20:04.000000 dvc-pandas-0.1.3/setup.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-08-02 09:30:16.430660 dvc-pandas-0.1.3/src/
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-08-02 09:30:16.434660 dvc-pandas-0.1.3/src/dvc_pandas/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      154 2021-06-12 14:42:57.000000 dvc-pandas-0.1.3/src/dvc_pandas/__init__.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     3606 2023-07-26 16:41:53.000000 dvc-pandas-0.1.3/src/dvc_pandas/dataset.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)      352 2021-06-12 14:42:57.000000 dvc-pandas-0.1.3/src/dvc_pandas/dvc.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)     2705 2023-04-11 14:35:40.000000 dvc-pandas-0.1.3/src/dvc_pandas/git.py
+-rw-rw-r--   0 jey       (1000) jey       (1000)    14077 2023-08-02 05:45:49.000000 dvc-pandas-0.1.3/src/dvc_pandas/repository.py
+drwxrwxr-x   0 jey       (1000) jey       (1000)        0 2023-08-02 09:30:16.434660 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/
+-rw-rw-r--   0 jey       (1000) jey       (1000)      556 2023-08-02 09:30:16.000000 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 jey       (1000) jey       (1000)      366 2023-08-02 09:30:16.000000 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)        1 2023-08-02 09:30:16.000000 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       91 2023-08-02 09:30:16.000000 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/requires.txt
+-rw-rw-r--   0 jey       (1000) jey       (1000)       11 2023-08-02 09:30:16.000000 dvc-pandas-0.1.3/src/dvc_pandas.egg-info/top_level.txt
```

### Comparing `dvc-pandas-0.1.2/LICENSE` & `dvc-pandas-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.2/PKG-INFO` & `dvc-pandas-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
-
-
```

### Comparing `dvc-pandas-0.1.2/setup.cfg` & `dvc-pandas-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dvc-pandas
-version = 0.1.2
+version = 0.1.3
 author = Bernhard Bliem
 author_email = bernhard.bliem@kausal.tech
 description = Wrapper for DVC and git to easily fetch Pandas dataframes
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kausaltech/dvc-pandas
 project_urls =
```

### Comparing `dvc-pandas-0.1.2/src/dvc_pandas/dataset.py` & `dvc-pandas-0.1.3/src/dvc_pandas/dataset.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.2/src/dvc_pandas/git.py` & `dvc-pandas-0.1.3/src/dvc_pandas/git.py`

 * *Files identical despite different names*

### Comparing `dvc-pandas-0.1.2/src/dvc_pandas/repository.py` & `dvc-pandas-0.1.3/src/dvc_pandas/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             dvc_file_path = parquet_path.parent / (parquet_path.name + '.dvc')
             yaml = YAML()
             with open(dvc_file_path, 'rt') as file:
                 dvc_data = yaml.load(file)
 
             if should_pull(parquet_path, dvc_data):
                 self.log_info(f"Pull dataset {parquet_path} from DVC using remote {self.dvc_remote}")
-                self.dvc_repo.pull(str(parquet_path), remote=self.dvc_remote)
+                self.dvc_repo.pull(str(parquet_path), remote=self.dvc_remote, force=True)
 
             df = pd.read_parquet(parquet_path)
 
             metadata = dvc_data.get('meta')
             if metadata is None:
                 units = None
             else:
@@ -260,15 +260,15 @@
             # self.dvc_repo.gc(all_commits=True, cloud=True, remote=self.dvc_remote)
             # TODO: Before reinstating the previous line, make sure gc doesn't delete blobs for which we don't have
             # a git commit because our git repository is outdated.
             raise
         finally:
             # Remove old version (or new if we rolled back) from cache
             logger.debug("Collect garbage in local DVC repository")
-            self.dvc_repo.gc(workspace=True)
+            self.dvc_repo.gc(workspace=True, force=True)
 
     @ensure_repo_lock
     def add(self, dataset: Dataset):
         """Create or update parquet file from dataset, but do not create .dvc file, commit or push."""
         if self.read_only:
             raise ValueError("add was called while repository is read-only.")
 
@@ -288,15 +288,15 @@
             # Remove old .dvc file (if it exists) and replace it with a new one
             dvc_file_path = path.parent / (path.name + '.dvc')
             if dvc_file_path.exists():
                 logger.debug(f"Remove file {dvc_file_path} from DVC")
                 self.dvc_repo.remove(str(dvc_file_path))
 
             logger.debug(f"Add file {path} to DVC")
-            self.dvc_repo.add(str(path))
+            self.dvc_repo.add(str(path), force=True)
 
             logger.debug(f"Set metadata to {stage_item.metadata}")
             set_dvc_file_metadata(dvc_file_path, stage_item.metadata)
 
             # Add .dvc file and .gitignore to index
             gitignore_path = dvc_file_path.parent / '.gitignore'
             self.git_repo.index.add([str(dvc_file_path), str(gitignore_path)])
```

### Comparing `dvc-pandas-0.1.2/src/dvc_pandas.egg-info/PKG-INFO` & `dvc-pandas-0.1.3/src/dvc_pandas.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: dvc-pandas
-Version: 0.1.2
+Version: 0.1.3
 Summary: Wrapper for DVC and git to easily fetch Pandas dataframes
 Home-page: https://github.com/kausaltech/dvc-pandas
 Author: Bernhard Bliem
 Author-email: bernhard.bliem@kausal.tech
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/kausaltech/dvc-pandas/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dvc-pandas
-
-
```

