# Comparing `tmp/monolith_filemanager-1.1.1.tar.gz` & `tmp/monolith_filemanager-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/monolith_filemanager-1.1.1.tar", last modified: Mon Jul 31 10:13:55 2023, max compression
+gzip compressed data, was "monolith_filemanager-2.0.0.tar", last modified: Wed Aug  2 08:06:53 2023, max compression
```

## Comparing `monolith_filemanager-1.1.1.tar` & `monolith_filemanager-2.0.0.tar`

### file list

```diff
@@ -1,95 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    13756 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/local_file_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18004 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/s3_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/adapters/version_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/components/path_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/hello.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_boto.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/console_commands/install_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/gmsh_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/hdf5_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/joblib_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/json_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/keras_model_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/numpy_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/pandas_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/protobuf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/standard_pickle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/vtk_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/file/yml_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/bucket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/s3storage/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/monolith_filemanager/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 10:13:45.000000 monolith_filemanager-1.1.1/monolith_filemanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 10:13:54.000000 monolith_filemanager-1.1.1/monolith_filemanager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/requirements_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/operator_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/requirements_manager/requirements_manager_class.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22915 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_local_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_s3_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/adapters/test_version_identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/components/test_path_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_joblib_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_json_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_keras_model_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_numpyfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_protobuf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_standard_pickle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/file/test_yml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/requirements_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/requirements_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/requirements_manager/test_requirements_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:13:55.000000 monolith_filemanager-1.1.1/tests/s3storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_bucket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/s3storage/test_v1engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-31 10:12:16.000000 monolith_filemanager-1.1.1/tests/test_path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.746175 monolith_filemanager-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-08-02 08:06:53.742175 monolith_filemanager-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1621 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (122)     8432 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.710173 monolith_filemanager-2.0.0/monolith_filemanager/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.714173 monolith_filemanager-2.0.0/monolith_filemanager/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4162 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      745 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13756 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/local_file_processes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18068 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/s3_processes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/adapters/version_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.714173 monolith_filemanager-2.0.0/monolith_filemanager/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/components/path_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.718173 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/hello.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/install_boto.py
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/install_flask.py
+-rw-r--r--   0 runner    (1001) docker     (122)      238 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/console_commands/install_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.726174 monolith_filemanager-2.0.0/monolith_filemanager/file/
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1005 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1035 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/hdf5_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)      900 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/joblib_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/json_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1634 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/keras_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3639 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/matlab.py
+-rw-r--r--   0 runner    (1001) docker     (122)      922 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/numpy_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6548 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/pandas_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/protobuf_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1096 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/standard_pickle_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/stl_object_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/vtk_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/file/yml_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.726174 monolith_filemanager-2.0.0/monolith_filemanager/s3storage/
+-rw-r--r--   0 runner    (1001) docker     (122)     7258 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/s3storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/s3storage/bucket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/s3storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6532 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/s3storage/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-08-02 08:06:41.000000 monolith_filemanager-2.0.0/monolith_filemanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.710173 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8923 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      635 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-08-02 08:06:53.000000 monolith_filemanager-2.0.0/monolith_filemanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.730174 monolith_filemanager-2.0.0/requirements_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/requirements_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/requirements_manager/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/requirements_manager/operator_enums.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3803 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/requirements_manager/requirements_manager_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-02 08:06:53.746175 monolith_filemanager-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.730174 monolith_filemanager-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.734175 monolith_filemanager-2.0.0/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22915 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/adapters/test_local_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19599 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/adapters/test_s3_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/adapters/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/adapters/test_version_identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.734175 monolith_filemanager-2.0.0/tests/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      789 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/components/test_path_map.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.742175 monolith_filemanager-2.0.0/tests/file/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_joblib_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1559 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_json_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1568 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_keras_model_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_numpyfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1879 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_protobuf_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1792 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_standard_pickle_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1246 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/file/test_yml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.742175 monolith_filemanager-2.0.0/tests/requirements_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/requirements_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/requirements_manager/test_requirements_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 08:06:53.742175 monolith_filemanager-2.0.0/tests/s3storage/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/s3storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/s3storage/test_bucket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5462 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/s3storage/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/s3storage/test_v1engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-08-02 08:04:41.000000 monolith_filemanager-2.0.0/tests/test_path.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `monolith_filemanager-1.1.1/LICENSE` & `monolith_filemanager-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/PKG-INFO` & `monolith_filemanager-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: monolith_filemanager
-Version: 1.1.1
+Version: 2.0.0
 Summary: Python package for reading and writing files
 Home-page: https://github.com/MonolithAILtd/monolith-filemanager
-Author: Maxwell Flitton
-Author-email: maxwell@gmail.com
+Author: Monolith AI
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: 3d
 Provides-Extra: matlab
 License-File: LICENSE
 
 # General File Manager
@@ -193,15 +192,14 @@
 The module supports the following extensions:
 
 - csv
 - dat
 - data
 - hdf5
 - h5
-- hdf5
 - hdf
 - json
 - joblib
 - mat
 - npy
 - parquet
 - vtk
@@ -231,14 +229,11 @@
 to update the package version number:
 ```yaml
 # Must be one of either: patch, minor or major
 release_type: "minor"
 ```
 
 # Contributing 
-This repo is still fairly new so contributing will require some communication. 
-You can contact with ideas and outline for a feature at ```maxwell@monolithai.com```.
-
 Writing code is not the only way you can contribute. Merely using the module is a help, if you come across any issues 
 feel free to raise them in the issues section of the Github page as this enables us to make the module more stable.
 If there are any issues that you want to solve, your pull request has to have documentation, 100% unit test coverage 
 and functional testing.
```

### Comparing `monolith_filemanager-1.1.1/Pipfile` & `monolith_filemanager-2.0.0/Pipfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 [[source]]
 url = "https://pypi.org/simple"
 verify_ssl = true
 name = "pypi"
 
 [packages]
-globre = "==0.1.5"
 h5py = "==2.10.0"
 joblib = "==0.15.0"
 flask = "==1.1.4"
 # Pin flask subdependencies to continue using older version:
 # https://github.com/pallets/flask/issues/4494
 # https://stackoverflow.com/questions/71189819/importerror-cannot-import-name-json-from-itsdangerous
 # https://bobbyhadz.com/blog/python-importerror-cannot-import-name-baseresponse-from-werkzeug-wrappers
 # https://github.com/aws/aws-sam-cli/issues/3661
 jinja2 = "==2.11.3"
 itsdangerous = "==1.1.0"
 werkzeug = "==1.0.1"
 MarkupSafe = "==2.0.1"
-gmsh = "==4.9.0"
 tensorflow = "==2.2.0"
 # protobuf is a subdependency of tensorflow. It must be pinned to address:
 # https://protobuf.dev/news/2022-05-06/#python-updates
 protobuf = "==3.19.6"
-numpy = "==1.16.4"
-pandas = "==0.25.1"
+# numpy is also a subdependency of cadquery (via nptyping)
+numpy = "==1.22.4"
+pandas = "==1.0.5"
 dask = {version = "==2020.12.0", extras = ["complete"]}
 distributed = "==2021.1.1"
 dill = "==0.2.9"
 # This version of pyvista is necessary to resolve an import issue. See these:
 # https://github.com/pyvista/pyvista/discussions/2858
 # https://github.com/pyvista/pyvista/pull/2912
 pyvista = "==0.34.2"
@@ -36,15 +35,20 @@
 botocore = "==1.13.5"
 requests = "==2.22.0"
 openpyxl = "==3.0.7"
 pyarrow = "==0.16.0"
 xlwt = "==1.3.0"
 xlrd = "==1.2.0"
 scipy = "==1.4.1"
+cqkit = "==0.5.1"
+# This is a dependency of cqkit but ckqit requirements.txt and setup.py files don't list it
+cadquery = "==2.2.0"
+s3fs = "==0.3.0"
 
 [dev-packages]
 parameterized = "==0.7.0"
 mock = "==4.0.3"
 pytest = "==4.3.1"
+globre = "==0.1.5"
 
 [requires]
-python_version = "3.7"
+python_version = "3.8"
```

### Comparing `monolith_filemanager-1.1.1/README.md` & `monolith_filemanager-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,14 @@
 The module supports the following extensions:
 
 - csv
 - dat
 - data
 - hdf5
 - h5
-- hdf5
 - hdf
 - json
 - joblib
 - mat
 - npy
 - parquet
 - vtk
@@ -214,14 +213,11 @@
 to update the package version number:
 ```yaml
 # Must be one of either: patch, minor or major
 release_type: "minor"
 ```
 
 # Contributing 
-This repo is still fairly new so contributing will require some communication. 
-You can contact with ideas and outline for a feature at ```maxwell@monolithai.com```.
-
 Writing code is not the only way you can contribute. Merely using the module is a help, if you come across any issues 
 feel free to raise them in the issues section of the Github page as this enables us to make the module more stable.
 If there are any issues that you want to solve, your pull request has to have documentation, 100% unit test coverage 
 and functional testing.
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/__init__.py` & `monolith_filemanager-2.0.0/monolith_filemanager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .path import FilePath
 from .adapters.base import Base
 from .adapters.s3_processes import S3ProcessesAdapter
 from .adapters.local_file_processes import LocalFileProcessesAdapter
 from .components.path_map import PathMap
 
-
 def file_manager(file_path: Union[str, FilePath], caching: Optional[Any] = None) -> Base:
     """
     Gets the correct adapter based on the path.
 
     :param file_path: (str) file path
     :param caching: (Optional[Any]) the CacheManager object to be used
     :return: initialized adapter object
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/adapters/base.py` & `monolith_filemanager-2.0.0/monolith_filemanager/adapters/base.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/adapters/errors.py` & `monolith_filemanager-2.0.0/monolith_filemanager/adapters/errors.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/adapters/local_file_processes.py` & `monolith_filemanager-2.0.0/monolith_filemanager/adapters/local_file_processes.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/adapters/s3_processes.py` & `monolith_filemanager-2.0.0/monolith_filemanager/adapters/s3_processes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import posixpath
 from typing import Any, Union, Tuple, List, Optional
 from urllib.parse import unquote
 
-import globre
-
 from monolith_filemanager.adapters.base import Base
 from monolith_filemanager.adapters.errors import S3ProcessesAdapterError
+from monolith_filemanager.adapters.utils import monolith_globre_match
 from monolith_filemanager.file.base import File, FilePath
 from monolith_filemanager.s3storage import V1Engine
 
 
 class S3ProcessesAdapter(Base):
     """
     This is a class for managing the interface of s3 file commands.
@@ -315,15 +314,15 @@
         :return: (str) cleaned string
         """
         res = unquote(text)
         return res
 
     @staticmethod
     def _glob_match(pattern: str, file: str):
-        return bool(globre.match(pattern, file))
+        return bool(monolith_globre_match(pattern, file))
 
     def rename_file(self, new_name: str) -> None:
         """
         Checks file to rename exists, checks new name not already taken.
         Copies file object to new location/name within bucket and then deletes old object.
 
         :param new_name: (str) new file name without extension
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/adapters/version_identifier.py` & `monolith_filemanager-2.0.0/monolith_filemanager/adapters/version_identifier.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/components/path_map.py` & `monolith_filemanager-2.0.0/monolith_filemanager/components/path_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/console_commands/hello.py` & `monolith_filemanager-2.0.0/monolith_filemanager/console_commands/hello.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/errors.py` & `monolith_filemanager-2.0.0/monolith_filemanager/errors.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/__init__.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     def init_bindings(self) -> None:
         """
         Imports and loads the file objects.
 
         :return: None
         """
         if self.bindings_imported is False:
-            from monolith_filemanager.file.gmsh_file import GmshFile
-            self.add_binding(file_object=GmshFile)
+            from monolith_filemanager.file.stl_object_file import StlObjectFile
+            self.add_binding(file_object=StlObjectFile)
             from monolith_filemanager.file.hdf5_file import Hdf5File
             self.add_binding(file_object=Hdf5File)
             from monolith_filemanager.file.json_file import JSONFile
             self.add_binding(file_object=JSONFile)
             from monolith_filemanager.file.keras_model_file import KerasModelFile
             self.add_binding(file_object=KerasModelFile)
             from monolith_filemanager.file.numpy_file import NumpyFile
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/base.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/base.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/errors.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,20 +38,14 @@
 
 class YamlFileError(Exception):
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
 
-class StlFileError(Exception):
-
-    def __init__(self, message: str) -> None:
-        super().__init__(message)
-
-
 class VtkFileError(Exception):
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
 
 class PickleFileError(Exception):
@@ -74,17 +68,17 @@
 
 class VTKFileError(Exception):
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
 
-class GmshFileError(Exception):
+class ProtobufFileError(Exception):
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
 
 
-class ProtobufFileError(Exception):
+class StlObjectFileError(Exception):
 
-    def __init__(self, message: str) -> None:
+    def __init(self, message: str) -> None:
         super().__init__(message)
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/hdf5_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/hdf5_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/joblib_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/joblib_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/json_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/json_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/keras_model_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/keras_model_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/matlab.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/matlab.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/numpy_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/numpy_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/pandas_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/pandas_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/protobuf_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/protobuf_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/standard_pickle_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/standard_pickle_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/vtk_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/vtk_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/file/yml_file.py` & `monolith_filemanager-2.0.0/monolith_filemanager/file/yml_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/path.py` & `monolith_filemanager-2.0.0/monolith_filemanager/path.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/__init__.py` & `monolith_filemanager-2.0.0/monolith_filemanager/s3storage/__init__.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/bucket_manager.py` & `monolith_filemanager-2.0.0/monolith_filemanager/s3storage/bucket_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager/s3storage/file_manager.py` & `monolith_filemanager-2.0.0/monolith_filemanager/s3storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager.egg-info/PKG-INFO` & `monolith_filemanager-2.0.0/monolith_filemanager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: monolith-filemanager
-Version: 1.1.1
+Version: 2.0.0
 Summary: Python package for reading and writing files
 Home-page: https://github.com/MonolithAILtd/monolith-filemanager
-Author: Maxwell Flitton
-Author-email: maxwell@gmail.com
+Author: Monolith AI
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: flask
 Provides-Extra: 3d
 Provides-Extra: matlab
 License-File: LICENSE
 
 # General File Manager
@@ -193,15 +192,14 @@
 The module supports the following extensions:
 
 - csv
 - dat
 - data
 - hdf5
 - h5
-- hdf5
 - hdf
 - json
 - joblib
 - mat
 - npy
 - parquet
 - vtk
@@ -231,14 +229,11 @@
 to update the package version number:
 ```yaml
 # Must be one of either: patch, minor or major
 release_type: "minor"
 ```
 
 # Contributing 
-This repo is still fairly new so contributing will require some communication. 
-You can contact with ideas and outline for a feature at ```maxwell@monolithai.com```.
-
 Writing code is not the only way you can contribute. Merely using the module is a help, if you come across any issues 
 feel free to raise them in the issues section of the Github page as this enables us to make the module more stable.
 If there are any issues that you want to solve, your pull request has to have documentation, 100% unit test coverage 
 and functional testing.
```

### Comparing `monolith_filemanager-1.1.1/monolith_filemanager.egg-info/SOURCES.txt` & `monolith_filemanager-2.0.0/monolith_filemanager.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,49 +15,51 @@
 monolith_filemanager.egg-info/requires.txt
 monolith_filemanager.egg-info/top_level.txt
 monolith_filemanager/adapters/__init__.py
 monolith_filemanager/adapters/base.py
 monolith_filemanager/adapters/errors.py
 monolith_filemanager/adapters/local_file_processes.py
 monolith_filemanager/adapters/s3_processes.py
+monolith_filemanager/adapters/utils.py
 monolith_filemanager/adapters/version_identifier.py
 monolith_filemanager/components/__init__.py
 monolith_filemanager/components/path_map.py
 monolith_filemanager/console_commands/__init__.py
 monolith_filemanager/console_commands/hello.py
 monolith_filemanager/console_commands/install_boto.py
 monolith_filemanager/console_commands/install_flask.py
 monolith_filemanager/console_commands/install_tensorflow.py
 monolith_filemanager/file/__init__.py
 monolith_filemanager/file/base.py
 monolith_filemanager/file/errors.py
-monolith_filemanager/file/gmsh_file.py
 monolith_filemanager/file/hdf5_file.py
 monolith_filemanager/file/joblib_file.py
 monolith_filemanager/file/json_file.py
 monolith_filemanager/file/keras_model_file.py
 monolith_filemanager/file/matlab.py
 monolith_filemanager/file/numpy_file.py
 monolith_filemanager/file/pandas_file.py
 monolith_filemanager/file/protobuf_file.py
 monolith_filemanager/file/standard_pickle_file.py
+monolith_filemanager/file/stl_object_file.py
 monolith_filemanager/file/vtk_file.py
 monolith_filemanager/file/yml_file.py
 monolith_filemanager/s3storage/__init__.py
 monolith_filemanager/s3storage/bucket_manager.py
 monolith_filemanager/s3storage/errors.py
 monolith_filemanager/s3storage/file_manager.py
 requirements_manager/__init__.py
 requirements_manager/errors.py
 requirements_manager/operator_enums.py
 requirements_manager/requirements_manager_class.py
 tests/test_path.py
 tests/adapters/__init__.py
 tests/adapters/test_local_adapter.py
 tests/adapters/test_s3_adapter.py
+tests/adapters/test_utils.py
 tests/adapters/test_version_identifier.py
 tests/components/__init__.py
 tests/components/test_path_map.py
 tests/file/__init__.py
 tests/file/test_base.py
 tests/file/test_hdf5.py
 tests/file/test_joblib_file.py
```

### Comparing `monolith_filemanager-1.1.1/requirements_manager/requirements_manager_class.py` & `monolith_filemanager-2.0.0/requirements_manager/requirements_manager_class.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/setup.py` & `monolith_filemanager-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,46 @@
-import pathlib
-
 import setuptools
 from setuptools import find_packages
 from setuptools.command.build_py import build_py as build_py_orig
 
 from requirements_manager import RequirementsManager, OperatorEnum
 
-# from setuptools import dist
-# dist.Distribution().fetch_build_eggs(['Cython==0.29'])
-# from Cython.Build import cythonize
-
 extras_packages = {
-    "flask": ["flask", "tensorflow", "boto3"],
-    "3d": ["pyvista", "gmsh"],
+    "flask": ["flask", "tensorflow", "boto3", "protobuf", "jinja2", "itsdangerous", "werkzeug",
+              "markupsafe"],
+    "3d": ["pyvista", "cqkit", "cadquery"],
     "matlab": ["scipy"]
 }
 
+__version__ = '2.0.0'
 
 class CustomBuildPy(build_py_orig):
     """
     subclass build_py so that we collect no .py files inside the built pip package
     this is done by overriding build_packages method with a noop
     """
     def build_packages(self):
         pass
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open(str(pathlib.Path(__file__).parent.absolute()) + "/monolith_filemanager/version.py", "r") as fh:
-    version = fh.read().split("=")[1].replace("'", "")
-
 directives = {
     'language_level': 3,
     'always_allow_keywords': True
 }
 
 requirements = RequirementsManager()
 
 
 setuptools.setup(
     name="monolith_filemanager",
-    version=version,
-    author="Maxwell Flitton",
-    author_email="maxwell@gmail.com",
+    version=__version__,
+    author="Monolith AI",
     description="Python package for reading and writing files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MonolithAILtd/monolith-filemanager",
     install_requires=requirements.get_packages(operator=OperatorEnum.GREATER_THAN_EQUAL),
     extras_require={
         'flask': requirements.get_packages(operator=OperatorEnum.GREATER_THAN_EQUAL, extras_require=extras_packages["flask"]),
@@ -57,22 +49,18 @@
     },
     packages=find_packages(exclude=("tests",)),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3',
+    python_requires='>=3.8',
     tests_require=['pytest'],
     entry_points={
         'console_scripts': [
             'file-hello = monolith_filemanager.console_commands.hello:print_logo',
             'file-install-flask = monolith_filemanager.console_commands.install_flask:install_flask',
             'file-install-tensorflow = monolith_filemanager.console_commands.install_tensorflow:install_tensorflow',
             'file-install-aws = monolith_filemanager.console_commands.install_boto:install_boto'
         ],
     }
-    # ext_modules=cythonize("caching/**/*.py", exclude="tests/**/*.py", compiler_directives=directives, nthreads=4),
-    # cmdclass={'build_py': CustomBuildPy},
-    # include_package_data=False,
-    # options={"bdist_wheel": {"universal": "1"}}
 )
```

### Comparing `monolith_filemanager-1.1.1/tests/adapters/test_local_adapter.py` & `monolith_filemanager-2.0.0/tests/adapters/test_local_adapter.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/adapters/test_s3_adapter.py` & `monolith_filemanager-2.0.0/tests/adapters/test_s3_adapter.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/adapters/test_version_identifier.py` & `monolith_filemanager-2.0.0/tests/adapters/test_version_identifier.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/components/test_path_map.py` & `monolith_filemanager-2.0.0/tests/components/test_path_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_base.py` & `monolith_filemanager-2.0.0/tests/file/test_base.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_hdf5.py` & `monolith_filemanager-2.0.0/tests/file/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_joblib_file.py` & `monolith_filemanager-2.0.0/tests/file/test_joblib_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_json_file.py` & `monolith_filemanager-2.0.0/tests/file/test_json_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_keras_model_file.py` & `monolith_filemanager-2.0.0/tests/file/test_keras_model_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_map.py` & `monolith_filemanager-2.0.0/tests/file/test_map.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_numpyfile.py` & `monolith_filemanager-2.0.0/tests/file/test_numpyfile.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_pandas.py` & `monolith_filemanager-2.0.0/tests/file/test_pandas.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_protobuf_file.py` & `monolith_filemanager-2.0.0/tests/file/test_protobuf_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_standard_pickle_file.py` & `monolith_filemanager-2.0.0/tests/file/test_standard_pickle_file.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_vtk.py` & `monolith_filemanager-2.0.0/tests/file/test_vtk.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/file/test_yml.py` & `monolith_filemanager-2.0.0/tests/file/test_yml.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/requirements_manager/test_requirements_manager.py` & `monolith_filemanager-2.0.0/tests/requirements_manager/test_requirements_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 from requirements_manager import RequirementsManager, OperatorEnum
 from requirements_manager.errors import NoPackagesInPipfileError, PipfilePathDoesNotExistError
 
 
 extras_packages = {
     "flask": ["flask", "tensorflow", "boto3", "protobuf", "jinja2", "itsdangerous", "werkzeug",
               "markupsafe"],
-    "3d": ["pyvista", "gmsh"],
+    "3d": ["pyvista", "cqkit", "cadquery"],
     "matlab": ["scipy"]
 }
 
 flask_packages = ["flask>=1.1.4", "tensorflow>=2.2.0", "boto3>=1.10.5", "protobuf>=3.19.6",
                   "jinja2>=2.11.3", "itsdangerous>=1.1.0", "werkzeug>=1.0.1", "markupsafe>=2.0.1"]
-three_d_packages = ["gmsh>=4.9.0", "pyvista>=0.34.2"]
+three_d_packages = ["pyvista>=0.34.2", "cqkit>=0.5.1", "cadquery>=2.2.0"]
 matlab_packages = ["scipy>=1.4.1"]
 
-all_packages = ['globre>=0.1.5', 'h5py>=2.10.0', 'joblib>=0.15.0', 'numpy>=1.16.4', 'pandas>=0.25.1',
+all_packages = ['h5py>=2.10.0', 'joblib>=0.15.0', 'numpy>=1.22.4', 'pandas>=1.0.5',
                 'distributed>=2021.1.1', 'dill>=0.2.9', 'pyyaml>=5.1.2', 'boto3>=1.10.5', 'botocore>=1.13.5',
                 'requests>=2.22.0', 'openpyxl>=3.0.7', 'pyarrow>=0.16.0', 'xlwt>=1.3.0', 'xlrd>=1.2.0',
-                'dask[complete]>=2020.12.0'] + flask_packages + three_d_packages + matlab_packages
+                'dask[complete]>=2020.12.0', 's3fs>=0.3.0'] \
+                    + flask_packages + three_d_packages + matlab_packages
 
 
 class TestRequirementsManager(TestCase):
     """
     Simple functional Tests for RequirementsManager
     """
```

### Comparing `monolith_filemanager-1.1.1/tests/s3storage/test_bucket_manager.py` & `monolith_filemanager-2.0.0/tests/s3storage/test_bucket_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/s3storage/test_file_manager.py` & `monolith_filemanager-2.0.0/tests/s3storage/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/s3storage/test_v1engine.py` & `monolith_filemanager-2.0.0/tests/s3storage/test_v1engine.py`

 * *Files identical despite different names*

### Comparing `monolith_filemanager-1.1.1/tests/test_path.py` & `monolith_filemanager-2.0.0/tests/test_path.py`

 * *Files identical despite different names*

