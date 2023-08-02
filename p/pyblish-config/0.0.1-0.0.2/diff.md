# Comparing `tmp/pyblish-config-0.0.1.tar.gz` & `tmp/pyblish-config-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblish-config-0.0.1.tar", last modified: Tue Jul  4 15:35:45 2023, max compression
+gzip compressed data, was "pyblish-config-0.0.2.tar", last modified: Wed Aug  2 08:05:26 2023, max compression
```

## Comparing `pyblish-config-0.0.1.tar` & `pyblish-config-0.0.2.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.464664 pyblish-config-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 15:35:45.464664 pyblish-config-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/pyblish_config/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/pyblish_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-07-04 15:35:45.000000 pyblish-config-0.0.1/pyblish_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-04 15:35:45.000000 pyblish-config-0.0.1/pyblish_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 15:35:45.000000 pyblish-config-0.0.1/pyblish_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-04 15:35:45.000000 pyblish-config-0.0.1/pyblish_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-04 15:35:45.000000 pyblish-config-0.0.1/pyblish_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/pyblish_config_creator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config_creator/config_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    33489 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config_creator/config_creator_GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_config_creator/plugin_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/pyblish_extended/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_extended/Plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_extended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/pyblish_extended/convertor/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_extended/convertor/convertor_pymesh_meshname.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/pyblish_extended/convertor/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_extended/convertor/plugins/convertor_string_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyblish_extended/convertor/testing_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/config_sample.json
--rw-r--r--   0 runner    (1001) docker     (123)    63025 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/managager_screenshot.JPG
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/sample_apply_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/sample_create_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/sample_filter_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/conmpare.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/inhouse generic plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/inhouse generic plugins/submit screenshot to inhouse server.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/sample/test files/marketplace (same as projects)/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/marketplace (same as projects)/collect all meshes/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/marketplace (same as projects)/collect all meshes/collect_meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/sample/test files/projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/
--rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_char_bob.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_obj_car.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52174 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_obj_gun.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52195 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/obj_pistol.ma
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/
--rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_alice.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_john.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_obj_sword.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52195 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/F_obj_pistol.ma
--rw-r--r--   0 runner    (1001) docker     (123)    52174 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/obj_gun.ma
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.456663 pyblish-config-0.0.1/sample/test files/projects/pyblish starter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.460663 pyblish-config-0.0.1/sample/test files/projects/pyblish starter/validate mesh normals/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/pyblish starter/validate mesh normals/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/projects/pyblish starter/validate mesh normals/validate_normals.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/pyblish isnta setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/test files/rules.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.464664 pyblish-config-0.0.1/sample/validate_folder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:45.464664 pyblish-config-0.0.1/sample/validate_folder/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/plugins/CollectFilePaths.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/plugins/ValidateFilePaths.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/sample_config_folder.json
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/sample_validate_folder_BF_create_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/sample_validate_folder_BF_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 15:35:35.000000 pyblish-config-0.0.1/sample/validate_folder/sample_validate_folder_FF.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 15:35:45.464664 pyblish-config-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.357216 pyblish-config-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 08:05:26.357216 pyblish-config-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/pyblish_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/pyblish_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-08-02 08:05:26.000000 pyblish-config-0.0.2/pyblish_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-02 08:05:26.000000 pyblish-config-0.0.2/pyblish_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 08:05:26.000000 pyblish-config-0.0.2/pyblish_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-02 08:05:26.000000 pyblish-config-0.0.2/pyblish_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-02 08:05:26.000000 pyblish-config-0.0.2/pyblish_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/pyblish_config_creator/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config_creator/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config_creator/config_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33489 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config_creator/config_creator_GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_config_creator/plugin_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/pyblish_extended/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_extended/Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_extended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/pyblish_extended/convertor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_extended/convertor/convertor_pymesh_meshname.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/pyblish_extended/convertor/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_extended/convertor/plugins/convertor_string_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyblish_extended/convertor/testing_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/config_sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)    63025 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/managager_screenshot.JPG
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/sample_apply_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/sample_create_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/sample_filter_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/conmpare.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/inhouse generic plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/inhouse generic plugins/submit screenshot to inhouse server.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/sample/test files/marketplace (same as projects)/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/marketplace (same as projects)/collect all meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/marketplace (same as projects)/collect all meshes/collect_meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/sample/test files/projects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/
+-rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_char_bob.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_obj_car.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52174 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_obj_gun.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52195 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/obj_pistol.ma
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/
+-rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_alice.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52199 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_john.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52254 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_obj_sword.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52195 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/F_obj_pistol.ma
+-rw-r--r--   0 runner    (1001) docker     (123)    52174 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/obj_gun.ma
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.349216 pyblish-config-0.0.2/sample/test files/projects/pyblish starter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.353216 pyblish-config-0.0.2/sample/test files/projects/pyblish starter/validate mesh normals/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/pyblish starter/validate mesh normals/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/projects/pyblish starter/validate mesh normals/validate_normals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/pyblish isnta setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/test files/rules.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.357216 pyblish-config-0.0.2/sample/validate_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:26.357216 pyblish-config-0.0.2/sample/validate_folder/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/plugins/CollectFilePaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/plugins/ValidateFilePaths.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/sample_config_folder.json
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/sample_validate_folder_BF_create_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/sample_validate_folder_BF_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-02 08:05:13.000000 pyblish-config-0.0.2/sample/validate_folder/sample_validate_folder_FF.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 08:05:26.357216 pyblish-config-0.0.2/setup.cfg
```

### Comparing `pyblish-config-0.0.1/.github/workflows/python-publish.yml` & `pyblish-config-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/.gitignore` & `pyblish-config-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/LICENSE` & `pyblish-config-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/PKG-INFO` & `pyblish-config-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: pyblish-config
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control the flow and settings of your Pyblish plugins with config files
 Author: Hannes D
 Project-URL: Homepage, https://github.com/hannesdelbeke/pyblish-config
 Project-URL: Source, https://github.com/hannesdelbeke/pyblish-config
 Keywords: plugin,addon,add-on,extension,manager,studio,dcc,pipeline
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pyblish-plugin-manager
-
-![screenshot](sample/managager_screenshot.JPG)
-
-the plugin manager allows you to override pyblish plugin settings externally. The aim is to assist with pipeline configuration and promote sharing and reusing plugins.
+# pyblish-config [![PyPI](https://img.shields.io/pypi/v/pyblish-config)](https://pypi.org/project/pyblish-config/) 
 
 ## overwriting attributes
 to make sure your pipeline doesnt break when updating plugins.
 pyblish config only overwrites settings it finds in the settings file
 it leaves everything else at default value.
 
 example:
@@ -35,7 +31,10 @@
 ## explicitly registering plugins
 the exception to this is the plugins registered.
 it will only use plugins matching the plugin names in the settings file
 
 example:
 you have 5 plugins registered. the settings file has 3 plugins listed.
 only those 3 plugins will be used.
+
+## config creator tool
+See the [config creator](https://github.com/hannesdelbeke/pyblish-config/tree/main/pyblish_config_creator), a little qt helper tool to help you  create configs. (still in alpha, will have bugs)
```

### Comparing `pyblish-config-0.0.1/README.md` & `pyblish-config-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# pyblish-plugin-manager
-
-![screenshot](sample/managager_screenshot.JPG)
-
-the plugin manager allows you to override pyblish plugin settings externally. The aim is to assist with pipeline configuration and promote sharing and reusing plugins.
+# pyblish-config [![PyPI](https://img.shields.io/pypi/v/pyblish-config)](https://pypi.org/project/pyblish-config/) 
 
 ## overwriting attributes
 to make sure your pipeline doesnt break when updating plugins.
 pyblish config only overwrites settings it finds in the settings file
 it leaves everything else at default value.
 
 example:
@@ -22,7 +18,10 @@
 ## explicitly registering plugins
 the exception to this is the plugins registered.
 it will only use plugins matching the plugin names in the settings file
 
 example:
 you have 5 plugins registered. the settings file has 3 plugins listed.
 only those 3 plugins will be used.
+
+## config creator tool
+See the [config creator](https://github.com/hannesdelbeke/pyblish-config/tree/main/pyblish_config_creator), a little qt helper tool to help you  create configs. (still in alpha, will have bugs)
```

### Comparing `pyblish-config-0.0.1/pyblish_config/config.py` & `pyblish-config-0.0.2/pyblish_config/config.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyblish_config.egg-info/PKG-INFO` & `pyblish-config-0.0.2/pyblish_config.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 Metadata-Version: 2.1
 Name: pyblish-config
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control the flow and settings of your Pyblish plugins with config files
 Author: Hannes D
 Project-URL: Homepage, https://github.com/hannesdelbeke/pyblish-config
 Project-URL: Source, https://github.com/hannesdelbeke/pyblish-config
 Keywords: plugin,addon,add-on,extension,manager,studio,dcc,pipeline
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# pyblish-plugin-manager
-
-![screenshot](sample/managager_screenshot.JPG)
-
-the plugin manager allows you to override pyblish plugin settings externally. The aim is to assist with pipeline configuration and promote sharing and reusing plugins.
+# pyblish-config [![PyPI](https://img.shields.io/pypi/v/pyblish-config)](https://pypi.org/project/pyblish-config/) 
 
 ## overwriting attributes
 to make sure your pipeline doesnt break when updating plugins.
 pyblish config only overwrites settings it finds in the settings file
 it leaves everything else at default value.
 
 example:
@@ -35,7 +31,10 @@
 ## explicitly registering plugins
 the exception to this is the plugins registered.
 it will only use plugins matching the plugin names in the settings file
 
 example:
 you have 5 plugins registered. the settings file has 3 plugins listed.
 only those 3 plugins will be used.
+
+## config creator tool
+See the [config creator](https://github.com/hannesdelbeke/pyblish-config/tree/main/pyblish_config_creator), a little qt helper tool to help you  create configs. (still in alpha, will have bugs)
```

### Comparing `pyblish-config-0.0.1/pyblish_config.egg-info/SOURCES.txt` & `pyblish-config-0.0.2/pyblish_config.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pyblish_config/__init__.py
 pyblish_config/config.py
 pyblish_config.egg-info/PKG-INFO
 pyblish_config.egg-info/SOURCES.txt
 pyblish_config.egg-info/dependency_links.txt
 pyblish_config.egg-info/requires.txt
 pyblish_config.egg-info/top_level.txt
+pyblish_config_creator/README.md
 pyblish_config_creator/__init__.py
 pyblish_config_creator/config_commands.py
 pyblish_config_creator/config_creator_GUI.py
 pyblish_config_creator/plugin_browser.py
 pyblish_extended/Plugin.py
 pyblish_extended/__init__.py
 pyblish_extended/convertor/convertor_pymesh_meshname.py
```

### Comparing `pyblish-config-0.0.1/pyblish_config_creator/config_creator_GUI.py` & `pyblish-config-0.0.2/pyblish_config_creator/config_creator_GUI.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyblish_extended/Plugin.py` & `pyblish-config-0.0.2/pyblish_extended/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyblish_extended/convertor/convertor_pymesh_meshname.py` & `pyblish-config-0.0.2/pyblish_extended/convertor/convertor_pymesh_meshname.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyblish_extended/convertor/plugins/convertor_string_int.py` & `pyblish-config-0.0.2/pyblish_extended/convertor/plugins/convertor_string_int.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyblish_extended/convertor/testing_convertor.py` & `pyblish-config-0.0.2/pyblish_extended/convertor/testing_convertor.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/pyproject.toml` & `pyblish-config-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 requires-python = ">=3.4"
 keywords = ["plugin", "addon", "add-on", "extension", "manager", "studio", "dcc", "pipeline"]
 #license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.7",
 ]
 #dynamic = ["dependencies"]
-dependencies = ['importlib-metadata; python_version<"3.7"', "pyblish"]
+dependencies = ['importlib-metadata; python_version<"3.7"', "pyblish-base"]
 #dynamic = ["version"]
-version = "0.0.1"
+version = "0.0.2"
 
 #[project.optional-dependencies]
 #yaml = ["pyyaml"]
 
 #[project.scripts]
 #my-script = "my_package.module:function"
```

### Comparing `pyblish-config-0.0.1/sample/managager_screenshot.JPG` & `pyblish-config-0.0.2/sample/managager_screenshot.JPG`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/sample_apply_config.py` & `pyblish-config-0.0.2/sample/sample_apply_config.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/sample_create_config.py` & `pyblish-config-0.0.2/sample/sample_create_config.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_char_bob.ma` & `pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_char_bob.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_obj_car.ma` & `pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_obj_car.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/BF_obj_gun.ma` & `pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/BF_obj_gun.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/battling field SHOOTER/obj_pistol.ma` & `pyblish-config-0.0.2/sample/test files/projects/battling field SHOOTER/obj_pistol.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_alice.ma` & `pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_alice.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_john.ma` & `pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_char_john.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_obj_sword.ma` & `pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/FF_obj_sword.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/F_obj_pistol.ma` & `pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/F_obj_pistol.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/final fantasia FANTASY RPG/meshes/obj_gun.ma` & `pyblish-config-0.0.2/sample/test files/projects/final fantasia FANTASY RPG/meshes/obj_gun.ma`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/projects/pyblish starter/validate mesh normals/validate_normals.py` & `pyblish-config-0.0.2/sample/test files/projects/pyblish starter/validate mesh normals/validate_normals.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/pyblish isnta setup.txt` & `pyblish-config-0.0.2/sample/test files/pyblish isnta setup.txt`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/test files/rules.txt` & `pyblish-config-0.0.2/sample/test files/rules.txt`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/validate_folder/plugins/CollectFilePaths.py` & `pyblish-config-0.0.2/sample/validate_folder/plugins/CollectFilePaths.py`

 * *Files identical despite different names*

### Comparing `pyblish-config-0.0.1/sample/validate_folder/sample_validate_folder_FF.py` & `pyblish-config-0.0.2/sample/validate_folder/sample_validate_folder_FF.py`

 * *Files identical despite different names*

