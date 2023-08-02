# Comparing `tmp/pynest-api-0.0.3.tar.gz` & `tmp/pynest-api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynest-api-0.0.3.tar", last modified: Mon Jul 17 15:44:44 2023, max compression
+gzip compressed data, was "pynest-api-0.1.0.tar", last modified: Wed Aug  2 05:26:49 2023, max compression
```

## Comparing `pynest-api-0.0.3.tar` & `pynest-api-0.1.0.tar`

### file list

```diff
@@ -1,56 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-17 15:44:19.000000 pynest-api-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-17 15:44:44.670378 pynest-api-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-17 15:44:19.000000 pynest-api-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/cli/click_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/common/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/orm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/requierments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/common/templates/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/core/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.666378 pynest-api-0.0.3/nest/core/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/base_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/database/orm_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/core/decorators/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/modules/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/modules/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/nest/marketplace/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:19.000000 pynest-api-0.0.3/nest/marketplace/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:44:44.670378 pynest-api-0.0.3/pynest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14472 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 15:44:44.000000 pynest-api-0.0.3/pynest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 15:44:19.000000 pynest-api-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:44:44.670378 pynest-api-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.534696 pynest-api-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 05:26:23.000000 pynest-api-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-08-02 05:26:49.534696 pynest-api-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-08-02 05:26:23.000000 pynest-api-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.514696 pynest-api-0.1.0/nest/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.518696 pynest-api-0.1.0/nest/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16322 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/cli/click_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.518696 pynest-api-0.1.0/nest/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.522696 pynest-api-0.1.0/nest/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/orm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/requierments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/common/templates/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.522696 pynest-api-0.1.0/nest/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.526696 pynest-api-0.1.0/nest/core/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/base_odm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/base_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/odm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/database/orm_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.526696 pynest-api-0.1.0/nest/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/decorators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/decorators/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/core/decorators/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.530696 pynest-api-0.1.0/nest/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.530696 pynest-api-0.1.0/nest/marketplace/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/marketplace/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.530696 pynest-api-0.1.0/nest/marketplace/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/marketplace/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.530696 pynest-api-0.1.0/nest/marketplace/modules/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/marketplace/modules/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.530696 pynest-api-0.1.0/nest/marketplace/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:23.000000 pynest-api-0.1.0/nest/marketplace/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 05:26:49.534696 pynest-api-0.1.0/pynest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14845 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 05:26:49.000000 pynest-api-0.1.0/pynest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 05:26:23.000000 pynest-api-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 05:26:49.534696 pynest-api-0.1.0/setup.cfg
```

### Comparing `pynest-api-0.0.3/LICENSE` & `pynest-api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.3/PKG-INFO` & `pynest-api-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6e65  : 2.1.Name: pyne
 00000020: 7374 2d61 7069 0a56 6572 7369 6f6e 3a20  st-api.Version: 
-00000030: 302e 302e 330a 5375 6d6d 6172 793a 2050  0.0.3.Summary: P
+00000030: 302e 312e 300a 5375 6d6d 6172 793a 2050  0.1.0.Summary: P
 00000040: 794e 6573 7420 6973 2061 2046 6173 7441  yNest is a FastA
 00000050: 5049 2041 6273 7472 6163 7469 6f6e 2066  PI Abstraction f
 00000060: 6f72 2062 7569 6c64 696e 6720 6d69 6372  or building micr
 00000070: 6f73 6572 7669 6365 732c 2069 6e66 6c75  oservices, influ
 00000080: 656e 6365 6420 6279 204e 6573 744a 532e  enced by NestJS.
 00000090: 0a41 7574 686f 722d 656d 6169 6c3a 2049  .Author-email: I
 000000a0: 7461 7920 4461 7220 3c69 7461 7932 3830  tay Dar <itay280
@@ -102,804 +102,827 @@
 00000650: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
 00000660: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
 00000670: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
 00000680: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
 00000690: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
 000006a0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 000006b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000006c0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+000006c0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
 000006d0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 000006e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000006f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000006f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
 00000700: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 00000710: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000720: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000730: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000740: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000750: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000760: 2033 2e31 300a 5265 7175 6972 6573 2d50   3.10.Requires-P
-00000770: 7974 686f 6e3a 203e 3d33 2e38 2e31 0a44  ython: >=3.8.1.D
-00000780: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-00000790: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000007a0: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-000007b0: 4578 7472 613a 2074 6573 740a 4c69 6365  Extra: test.Lice
-000007c0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000007d0: 450a 0a3c 7020 616c 6967 6e3d 2263 656e  E..<p align="cen
-000007e0: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-000007f0: 3d22 646f 6373 2f69 6d67 732f 7079 6e65  ="docs/imgs/pyne
-00000800: 7374 5f6c 6f67 6f2d 6d6f 6469 6669 6564  st_logo-modified
-00000810: 2e70 6e67 2220 7469 746c 653d 2270 796e  .png" title="pyn
-00000820: 6573 7420 6c6f 676f 2220 7769 6474 683d  est logo" width=
-00000830: 2232 3030 223e 0a3c 2f70 3e0a 3c70 2061  "200">.</p>.<p a
-00000840: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00000850: 2020 203c 656d 3e50 794e 6573 7420 6973     <em>PyNest is
-00000860: 2061 2050 7974 686f 6e20 6672 616d 6577   a Python framew
-00000870: 6f72 6b20 6275 696c 7420 6f6e 2074 6f70  ork built on top
-00000880: 206f 6620 4661 7374 4150 4920 7468 6174   of FastAPI that
-00000890: 2066 6f6c 6c6f 7773 2074 6865 206d 6f64   follows the mod
-000008a0: 756c 6172 2061 7263 6869 7465 6374 7572  ular architectur
-000008b0: 6520 6f66 204e 6573 744a 533c 2f65 6d3e  e of NestJS</em>
-000008c0: 0a3c 2f70 3e0a 3c70 2061 6c69 676e 3d22  .</p>.<p align="
-000008d0: 6365 6e74 6572 223e 0a3c 6120 6872 6566  center">.<a href
-000008e0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-000008f0: 7267 2f70 726f 6a65 6374 2f70 796e 6573  rg/project/pynes
-00000900: 742d 6170 6922 2074 6172 6765 743d 225f  t-api" target="_
-00000910: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-00000920: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000930: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000940: 692f 762f 7079 6e65 7374 2d61 7069 3f63  i/v/pynest-api?c
-00000950: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
-00000960: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
-00000970: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
-00000980: 6520 7665 7273 696f 6e22 3e0a 3c2f 613e  e version">.</a>
-00000990: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-000009a0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000009b0: 6374 2f70 796e 6573 742d 6170 6922 2074  ct/pynest-api" t
-000009c0: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
-000009d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000009e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000009f0: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000a00: 696f 6e73 2f70 796e 6573 742d 6170 692e  ions/pynest-api.
-00000a10: 7376 673f 636f 6c6f 723d 2532 3333 3444  svg?color=%2334D
-00000a20: 3035 3822 2061 6c74 3d22 5375 7070 6f72  058" alt="Suppor
-00000a30: 7465 6420 5079 7468 6f6e 2076 6572 7369  ted Python versi
-00000a40: 6f6e 7322 3e0a 3c2f 613e 0a3c 2f70 3e0a  ons">.</a>.</p>.
-00000a50: 0a23 2050 794e 6573 7420 2d20 4465 7363  .# PyNest - Desc
-00000a60: 7269 7074 696f 6e0a 0a50 794e 6573 7420  ription..PyNest 
-00000a70: 6973 2064 6573 6967 6e65 6420 746f 2068  is designed to h
-00000a80: 656c 7020 7374 7275 6374 7572 6520 796f  elp structure yo
-00000a90: 7572 2041 5049 7320 696e 2061 6e20 696e  ur APIs in an in
-00000aa0: 7475 6974 6976 652c 2065 6173 7920 746f  tuitive, easy to
-00000ab0: 2075 6e64 6572 7374 616e 642c 2061 6e64   understand, and
-00000ac0: 2065 6e6a 6f79 6162 6c65 2077 6179 2e0a   enjoyable way..
-00000ad0: 0a57 6974 6820 5079 4e65 7374 2c20 796f  .With PyNest, yo
-00000ae0: 7520 6361 6e20 6275 696c 6420 7363 616c  u can build scal
-00000af0: 6162 6c65 2061 6e64 206d 6169 6e74 6169  able and maintai
-00000b00: 6e61 626c 6520 4150 4973 2077 6974 6820  nable APIs with 
-00000b10: 6561 7365 2e20 5468 6520 6672 616d 6577  ease. The framew
-00000b20: 6f72 6b20 7375 7070 6f72 7473 2064 6570  ork supports dep
-00000b30: 656e 6465 6e63 7920 696e 6a65 6374 696f  endency injectio
-00000b40: 6e2c 2074 7970 6520 616e 6e6f 7461 7469  n, type annotati
-00000b50: 6f6e 732c 2064 6563 6f72 6174 6f72 732c  ons, decorators,
-00000b60: 2061 6e64 2063 6f64 6520 6765 6e65 7261   and code genera
-00000b70: 7469 6f6e 2c20 6d61 6b69 6e67 2069 7420  tion, making it 
-00000b80: 6561 7379 2074 6f20 7772 6974 6520 636c  easy to write cl
-00000b90: 6561 6e20 616e 6420 7465 7374 6162 6c65  ean and testable
-00000ba0: 2063 6f64 652e 0a0a 5468 6973 2066 7261   code...This fra
-00000bb0: 6d65 776f 726b 2069 7320 6e6f 7420 6120  mework is not a 
-00000bc0: 6469 7265 6374 2070 6f72 7420 6f66 204e  direct port of N
-00000bd0: 6573 744a 5320 746f 2050 7974 686f 6e20  estJS to Python 
-00000be0: 6275 7420 7261 7468 6572 2061 2072 652d  but rather a re-
-00000bf0: 696d 6167 696e 696e 6720 6f66 2074 6865  imagining of the
-00000c00: 2066 7261 6d65 776f 726b 2073 7065 6369   framework speci
-00000c10: 6669 6361 6c6c 7920 666f 7220 5079 7468  fically for Pyth
-00000c20: 6f6e 2064 6576 656c 6f70 6572 732c 2069  on developers, i
-00000c30: 6e63 6c75 6469 6e67 2064 6174 6120 7363  ncluding data sc
-00000c40: 6965 6e74 6973 7473 2c20 6461 7461 2061  ientists, data a
-00000c50: 6e61 6c79 7374 732c 2061 6e64 2064 6174  nalysts, and dat
-00000c60: 6120 656e 6769 6e65 6572 732e 2049 7420  a engineers. It 
-00000c70: 6169 6d73 2074 6f20 6173 7369 7374 2074  aims to assist t
-00000c80: 6865 6d20 696e 2062 7569 6c64 696e 6720  hem in building 
-00000c90: 6265 7474 6572 2061 6e64 2066 6173 7465  better and faste
-00000ca0: 7220 4150 4973 2066 6f72 2074 6865 6972  r APIs for their
-00000cb0: 2064 6174 6120 6170 706c 6963 6174 696f   data applicatio
-00000cc0: 6e73 2e0a 0a23 2320 4765 7474 696e 6720  ns...## Getting 
-00000cd0: 5374 6172 7465 640a 546f 2067 6574 2073  Started.To get s
-00000ce0: 7461 7274 6564 2077 6974 6820 5079 4e65  tarted with PyNe
-00000cf0: 7374 2c20 796f 7527 6c6c 206e 6565 6420  st, you'll need 
-00000d00: 746f 2069 6e73 7461 6c6c 2069 7420 7573  to install it us
-00000d10: 696e 6720 7069 703a 0a0a 6060 6062 6173  ing pip:..```bas
-00000d20: 680a 7069 7020 696e 7374 616c 6c20 7079  h.pip install py
-00000d30: 6e65 7374 2d61 7069 0a60 6060 0a0a 2323  nest-api.```..##
-00000d40: 2320 5374 6172 7420 7769 7468 2063 6c69  # Start with cli
-00000d50: 0a60 6060 6261 7368 0a70 796e 6573 7420  .```bash.pynest 
-00000d60: 6372 6561 7465 2d6e 6573 742d 6170 7020  create-nest-app 
-00000d70: 2d6e 206d 795f 6170 705f 6e61 6d65 0a60  -n my_app_name.`
-00000d80: 6060 0a0a 7468 6973 2063 6f6d 6d61 6e64  ``..this command
-00000d90: 2077 696c 6c20 6372 6561 7465 2061 206e   will create a n
-00000da0: 6577 2070 726f 6a65 6374 2077 6974 6820  ew project with 
-00000db0: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
-00000dc0: 7275 6374 7572 653a 0a0a 6060 6074 6578  ructure:..```tex
-00000dd0: 740a e294 9ce2 9480 e294 8020 6170 702e  t.......... app.
-00000de0: 7079 0ae2 949c e294 80e2 9480 206f 726d  py.......... orm
-00000df0: 5f63 6f6e 6669 672e 7079 0ae2 949c e294  _config.py......
-00000e00: 80e2 9480 206d 6169 6e2e 7079 0ae2 949c  .... main.py....
-00000e10: e294 80e2 9480 2073 7263 0ae2 9482 2020  ...... src....  
-00000e20: 2020 e294 9ce2 9480 e294 8020 5f5f 696e    ......... __in
-00000e30: 6974 5f5f 2e70 790a e294 8220 2020 20e2  it__.py....    .
-00000e40: 949c e294 80e2 9480 2065 7861 6d70 6c65  ........ example
-00000e50: 730a e294 8220 2020 20e2 9482 2020 2020  s....    ...    
-00000e60: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
-00000e70: 5f5f 2e70 790a e294 8220 2020 20e2 9482  __.py....    ...
-00000e80: 2020 2020 e294 9ce2 9480 e294 8020 6578      ......... ex
-00000e90: 616d 706c 6573 5f63 6f6e 7472 6f6c 6c65  amples_controlle
-00000ea0: 722e 7079 0ae2 9482 2020 2020 e294 8220  r.py....    ... 
-00000eb0: 2020 20e2 949c e294 80e2 9480 2065 7861     ......... exa
-00000ec0: 6d70 6c65 735f 7365 7276 6963 652e 7079  mples_service.py
-00000ed0: 0ae2 9482 2020 2020 e294 8220 2020 20e2  ....    ...    .
-00000ee0: 949c e294 80e2 9480 2065 7861 6d70 6c65  ........ example
-00000ef0: 735f 6d6f 6465 6c2e 7079 0ae2 9482 2020  s_model.py....  
-00000f00: 2020 e294 9ce2 9480 e294 8020 20e2 949c    .........  ...
-00000f10: e294 80e2 9480 2065 7861 6d70 6c65 735f  ...... examples_
-00000f20: 656e 7469 7479 2e70 790a e294 8220 2020  entity.py....   
-00000f30: 20e2 949c e294 80e2 9480 2020 e294 9ce2   .........  ....
-00000f40: 9480 e294 8020 6578 616d 706c 6573 5f6d  ..... examples_m
-00000f50: 6f64 756c 652e 7079 0a60 6060 0a0a 6f6e  odule.py.```..on
-00000f60: 6365 2079 6f75 2068 6176 6520 6372 6561  ce you have crea
-00000f70: 7465 6420 796f 7572 2061 7070 2c20 6765  ted your app, ge
-00000f80: 7420 696e 746f 2074 6865 2066 6f6c 6465  t into the folde
-00000f90: 7220 616e 6420 7275 6e20 7468 6520 666f  r and run the fo
-00000fa0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-00000fb0: 0a0a 6060 6062 6173 680a 6364 206d 795f  ..```bash.cd my_
-00000fc0: 6170 705f 6e61 6d65 0a60 6060 0a0a 7275  app_name.```..ru
-00000fd0: 6e20 7468 6520 7365 7276 6572 2077 6974  n the server wit
-00000fe0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
-00000ff0: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
-00001000: 680a 7576 6963 6f72 6e20 2261 7070 3a61  h.uvicorn "app:a
-00001010: 7070 2220 2d2d 686f 7374 2022 302e 302e  pp" --host "0.0.
-00001020: 302e 3022 202d 2d70 6f72 7420 2238 3022  0.0" --port "80"
-00001030: 202d 2d72 656c 6f61 640a 6060 600a 0a4e   --reload.```..N
-00001040: 6f77 2079 6f75 2063 616e 2076 6973 6974  ow you can visit
-00001050: 205b 4f70 656e 4150 495d 2868 7474 703a   [OpenAPI](http:
-00001060: 2f2f 6c6f 6361 6c68 6f73 743a 3830 2f64  //localhost:80/d
-00001070: 6f63 7329 2069 6e20 796f 7572 2062 726f  ocs) in your bro
-00001080: 7773 6572 2074 6f20 7365 6520 7468 6520  wser to see the 
-00001090: 6465 6661 756c 7420 4150 4920 646f 6375  default API docu
-000010a0: 6d65 6e74 6174 696f 6e2e 0a0a 2323 2320  mentation...### 
-000010b0: 4164 6469 6e67 206d 6f64 756c 6573 0a0a  Adding modules..
-000010c0: 546f 2061 6464 2061 206e 6577 206d 6f64  To add a new mod
-000010d0: 756c 6520 746f 2079 6f75 7220 6170 706c  ule to your appl
-000010e0: 6963 6174 696f 6e2c 2079 6f75 2063 616e  ication, you can
-000010f0: 2075 7365 2074 6865 2070 796e 6573 7420   use the pynest 
-00001100: 6765 6e65 7261 7465 206d 6f64 756c 6520  generate module 
-00001110: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
-00001120: 680a 7079 6e65 7374 2067 656e 6572 6174  h.pynest generat
-00001130: 652d 6d6f 6475 6c65 202d 6e20 7573 6572  e-module -n user
-00001140: 730a 6060 600a 0a54 6869 7320 7769 6c6c  s.```..This will
-00001150: 2063 7265 6174 6520 6120 6e65 7720 6d6f   create a new mo
-00001160: 6475 6c65 2063 616c 6c65 6420 6060 6075  dule called ```u
-00001170: 7365 7273 6060 6020 696e 2079 6f75 7220  sers``` in your 
-00001180: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-00001190: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
-000011a0: 7472 7563 7475 7265 3a0a 0a60 6060 7465  tructure:..```te
-000011b0: 7874 0ae2 949c e294 80e2 9480 2075 7365  xt.......... use
-000011c0: 7273 0ae2 9482 2020 2020 e294 9ce2 9480  rs....    ......
-000011d0: e294 8020 5f5f 696e 6974 5f5f 2e70 790a  ... __init__.py.
-000011e0: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
-000011f0: 2075 7365 7273 5f63 6f6e 7472 6f6c 6c65   users_controlle
-00001200: 722e 7079 0ae2 9482 2020 2020 e294 9ce2  r.py....    ....
-00001210: 9480 e294 8020 7573 6572 735f 7365 7276  ..... users_serv
-00001220: 6963 652e 7079 0ae2 9482 2020 2020 e294  ice.py....    ..
-00001230: 9ce2 9480 e294 8020 7573 6572 735f 6d6f  ....... users_mo
-00001240: 6465 6c2e 7079 0ae2 9482 2020 2020 e294  del.py....    ..
-00001250: 9ce2 9480 e294 8020 7573 6572 735f 656e  ....... users_en
-00001260: 7469 7479 2e70 790a e294 8220 2020 20e2  tity.py....    .
-00001270: 949c e294 80e2 9480 2075 7365 7273 5f6d  ........ users_m
-00001280: 6f64 756c 652e 7079 0a60 6060 0a0a 5468  odule.py.```..Th
-00001290: 6520 7573 6572 7320 6d6f 6475 6c65 2077  e users module w
-000012a0: 696c 6c20 696d 6d65 6469 6174 656c 7920  ill immediately 
-000012b0: 7265 6769 7374 6572 2069 7473 656c 6620  register itself 
-000012c0: 7769 7468 2074 6865 2061 7070 6c69 6361  with the applica
-000012d0: 7469 6f6e 2061 6e64 2077 696c 6c20 6265  tion and will be
-000012e0: 2061 7661 696c 6162 6c65 2066 6f72 2075   available for u
-000012f0: 7365 2e0a 0a59 6f75 2063 616e 2074 6865  se...You can the
-00001300: 6e20 7374 6172 7420 6465 6669 6e69 6e67  n start defining
-00001310: 2072 6f75 7465 7320 616e 6420 6f74 6865   routes and othe
-00001320: 7220 6170 706c 6963 6174 696f 6e20 636f  r application co
-00001330: 6d70 6f6e 656e 7473 2075 7369 6e67 2064  mponents using d
-00001340: 6563 6f72 6174 6f72 7320 616e 6420 6f74  ecorators and ot
-00001350: 6865 7220 5079 4e65 7374 2063 6f6e 7374  her PyNest const
-00001360: 7275 6374 732e 0a0a 466f 7220 6d6f 7265  ructs...For more
-00001370: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00001380: 686f 7720 746f 2075 7365 2050 794e 6573  how to use PyNes
-00001390: 742c 2063 6865 636b 206f 7574 2074 6865  t, check out the
-000013a0: 206f 6666 6963 6961 6c20 646f 6375 6d65   official docume
-000013b0: 6e74 6174 696f 6e20 6174 2068 7474 7073  ntation at https
-000013c0: 3a2f 2f70 7974 686f 6e6e 6573 742e 6769  ://pythonnest.gi
-000013d0: 7468 7562 2e69 6f2f 5079 4e65 7374 2f2e  thub.io/PyNest/.
-000013e0: 0a0a 2323 2053 7461 7274 696e 6720 6120  ..## Starting a 
-000013f0: 6e65 7720 7072 6f6a 6563 7420 6d61 6e75  new project manu
-00001400: 616c 6c79 0a0a 6060 6074 6578 740a 4e4f  ally..```text.NO
-00001410: 5449 4345 3a20 666f 7220 7468 6520 666f  TICE: for the fo
-00001420: 6c6c 6f77 696e 6720 6578 616d 706c 652c  llowing example,
-00001430: 2077 6520 7769 6c6c 2075 7365 2074 6865   we will use the
-00001440: 2070 726f 6475 6374 7320 6d6f 6475 6c65   products module
-00001450: 2e20 0a60 6060 0a0a 546f 2073 7461 7274  . .```..To start
-00001460: 2061 206e 6577 2070 726f 6a65 6374 206d   a new project m
-00001470: 616e 7561 6c6c 792c 2079 6f75 276c 6c20  anually, you'll 
-00001480: 6e65 6564 2074 6f20 6372 6561 7465 2061  need to create a
-00001490: 2070 726f 6a65 6374 2074 6861 7420 666f   project that fo
-000014a0: 6c6c 6f77 7320 7468 6973 2073 7472 7563  llows this struc
-000014b0: 7475 7265 3a0a 0a60 6060 7465 7874 0ae2  ture:..```text..
-000014c0: 949c e294 80e2 9480 2061 7070 2e70 790a  ........ app.py.
-000014d0: e294 9ce2 9480 e294 8020 6f72 6d5f 636f  ......... orm_co
-000014e0: 6e66 6967 2e70 790a e294 9ce2 9480 e294  nfig.py.........
-000014f0: 8020 6d61 696e 2e70 790a e294 9ce2 9480  . main.py.......
-00001500: e294 8020 7372 630a e294 8220 2020 20e2  ... src....    .
-00001510: 949c e294 80e2 9480 205f 5f69 6e69 745f  ........ __init_
-00001520: 5f2e 7079 0ae2 9482 2020 2020 e294 9ce2  _.py....    ....
-00001530: 9480 e294 8020 7072 6f64 7563 7473 0ae2  ..... products..
-00001540: 9482 2020 2020 e294 8220 2020 20e2 949c  ..    ...    ...
-00001550: e294 80e2 9480 205f 5f69 6e69 745f 5f2e  ...... __init__.
-00001560: 7079 0ae2 9482 2020 2020 e294 8220 2020  py....    ...   
-00001570: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
-00001580: 6374 735f 636f 6e74 726f 6c6c 6572 2e70  cts_controller.p
-00001590: 790a e294 8220 2020 20e2 9482 2020 2020  y....    ...    
-000015a0: e294 9ce2 9480 e294 8020 7072 6f64 7563  ......... produc
-000015b0: 7473 5f73 6572 7669 6365 2e70 790a e294  ts_service.py...
-000015c0: 8220 2020 20e2 9482 2020 2020 e294 9ce2  .    ...    ....
-000015d0: 9480 e294 8020 7072 6f64 7563 7473 5f6d  ..... products_m
-000015e0: 6f64 656c 2e70 790a e294 8220 2020 20e2  odel.py....    .
-000015f0: 949c e294 80e2 9480 2020 e294 9ce2 9480  ........  ......
-00001600: e294 8020 7072 6f64 7563 7473 5f65 6e74  ... products_ent
-00001610: 6974 792e 7079 0ae2 9482 2020 2020 e294  ity.py....    ..
-00001620: 9ce2 9480 e294 8020 20e2 949c e294 80e2  .......  .......
-00001630: 9480 2070 726f 6475 6374 735f 6d6f 6475  .. products_modu
-00001640: 6c65 2e70 790a 6060 600a 0a45 7870 6c61  le.py.```..Expla
-00001650: 6e61 7469 6f6e 3a20 5468 6973 2069 7320  nation: This is 
-00001660: 7468 6520 6469 7265 6374 6f72 7920 7374  the directory st
-00001670: 7275 6374 7572 6520 666f 7220 796f 7572  ructure for your
-00001680: 2070 726f 6a65 6374 2e20 4974 2069 6e63   project. It inc
-00001690: 6c75 6465 7320 7468 6520 6d61 696e 2066  ludes the main f
-000016a0: 696c 6573 2061 6e64 2061 2073 7263 2064  iles and a src d
-000016b0: 6972 6563 746f 7279 2074 6861 7420 636f  irectory that co
-000016c0: 6e74 6169 6e73 2079 6f75 7220 7072 6f6a  ntains your proj
-000016d0: 6563 7427 7320 736f 7572 6365 2063 6f64  ect's source cod
-000016e0: 652e 0a0a 2323 2320 4372 6561 7469 6e67  e...### Creating
-000016f0: 2074 6865 2066 696c 6573 0a0a 2323 2323   the files..####
-00001700: 206d 6169 6e2e 7079 0a60 6060 7079 7468   main.py.```pyth
-00001710: 6f6e 0a69 6d70 6f72 7420 7576 6963 6f72  on.import uvicor
-00001720: 6e0a 0a0a 6966 205f 5f6e 616d 655f 5f20  n...if __name__ 
-00001730: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00001740: 2020 2075 7669 636f 726e 2e72 756e 280a     uvicorn.run(.
-00001750: 2020 2020 2020 2020 2761 7070 3a61 7070          'app:app
-00001760: 272c 0a20 2020 2020 2020 2068 6f73 743d  ',.        host=
-00001770: 2230 2e30 2e30 2e30 222c 0a20 2020 2020  "0.0.0.0",.     
-00001780: 2020 2070 6f72 743d 3830 2c0a 2020 2020     port=80,.    
-00001790: 290a 6060 600a 0a54 6869 7320 6973 2074  ).```..This is t
-000017a0: 6865 206d 6169 6e2e 7079 2066 696c 652c  he main.py file,
-000017b0: 2077 6869 6368 2069 7320 7265 7370 6f6e   which is respon
-000017c0: 7369 626c 6520 666f 7220 7275 6e6e 696e  sible for runnin
-000017d0: 6720 796f 7572 2061 7070 6c69 6361 7469  g your applicati
-000017e0: 6f6e 2075 7369 6e67 2074 6865 2055 7669  on using the Uvi
-000017f0: 636f 726e 2073 6572 7665 722e 0a3c 6272  corn server..<br
-00001800: 3e0a 4974 2069 6d70 6f72 7473 2074 6865  >.It imports the
-00001810: 2075 7669 636f 726e 206c 6962 7261 7279   uvicorn library
-00001820: 2061 6e64 2073 7461 7274 7320 7468 6520   and starts the 
-00001830: 7365 7276 6572 2077 6974 6820 7468 6520  server with the 
-00001840: 7370 6563 6966 6965 6420 686f 7374 2061  specified host a
-00001850: 6e64 2070 6f72 742e 0a0a 0a23 2323 2320  nd port....#### 
-00001860: 6170 702e 7079 0a0a 6060 6070 7974 686f  app.py..```pytho
-00001870: 6e0a 6672 6f6d 206f 726d 5f63 6f6e 6669  n.from orm_confi
-00001880: 6720 696d 706f 7274 2063 6f6e 6669 670a  g import config.
-00001890: 6672 6f6d 206e 6573 742e 636f 7265 2069  from nest.core i
-000018a0: 6d70 6f72 7420 4170 700a 6672 6f6d 2073  mport App.from s
-000018b0: 7263 2e70 726f 6475 6374 732e 7072 6f64  rc.products.prod
-000018c0: 7563 7473 5f6d 6f64 756c 6520 696d 706f  ucts_module impo
-000018d0: 7274 2050 726f 6475 6374 734d 6f64 756c  rt ProductsModul
-000018e0: 650a 0a61 7070 203d 2041 7070 280a 2020  e..app = App(.  
-000018f0: 2020 6465 7363 7269 7074 696f 6e3d 2259    description="Y
-00001900: 6f75 7220 6170 7020 6465 7363 7269 7074  our app descript
-00001910: 696f 6e22 2c0a 2020 2020 6d6f 6475 6c65  ion",.    module
-00001920: 733d 5b0a 2020 2020 2020 2020 5072 6f64  s=[.        Prod
-00001930: 7563 7473 4d6f 6475 6c65 0a20 2020 205d  uctsModule.    ]
-00001940: 2c0a 2020 2020 696e 6974 5f64 623d 636f  ,.    init_db=co
-00001950: 6e66 6967 2e63 7265 6174 655f 616c 6c0a  nfig.create_all.
-00001960: 290a 6060 600a 0a54 6869 7320 6973 2074  ).```..This is t
-00001970: 6865 2061 7070 2e70 7920 6669 6c65 2c20  he app.py file, 
-00001980: 7768 6963 6820 6973 2074 6865 2065 6e74  which is the ent
-00001990: 7279 2070 6f69 6e74 2066 6f72 2079 6f75  ry point for you
-000019a0: 7220 6170 706c 6963 6174 696f 6e2e 2049  r application. I
-000019b0: 7420 696d 706f 7274 7320 6e65 6365 7373  t imports necess
-000019c0: 6172 7920 6d6f 6475 6c65 7320 616e 6420  ary modules and 
-000019d0: 7365 7473 2075 7020 7468 6520 4170 7020  sets up the App 
-000019e0: 6f62 6a65 6374 2077 6974 6820 6120 6465  object with a de
-000019f0: 7363 7269 7074 696f 6e20 616e 6420 7468  scription and th
-00001a00: 6520 5072 6f64 7563 7473 4d6f 6475 6c65  e ProductsModule
-00001a10: 2e0a 3c62 723e 0a49 7420 616c 736f 2069  ..<br>.It also i
-00001a20: 6e69 7469 616c 697a 6573 2074 6865 2064  nitializes the d
-00001a30: 6174 6162 6173 6520 7573 696e 6720 7468  atabase using th
-00001a40: 6520 636f 6e66 6967 2e63 7265 6174 655f  e config.create_
-00001a50: 616c 6c20 6675 6e63 7469 6f6e 2e0a 0a23  all function...#
-00001a60: 2323 2320 6f72 6d5f 636f 6e66 6967 2e70  ### orm_config.p
-00001a70: 790a 6060 6070 7974 686f 6e0a 6672 6f6d  y.```python.from
-00001a80: 206e 6573 742e 636f 7265 2069 6d70 6f72   nest.core impor
-00001a90: 7420 4f72 6d53 6572 7669 6365 0a69 6d70  t OrmService.imp
-00001aa0: 6f72 7420 6f73 0a66 726f 6d20 646f 7465  ort os.from dote
-00001ab0: 6e76 2069 6d70 6f72 7420 6c6f 6164 5f64  nv import load_d
-00001ac0: 6f74 656e 760a 0a6c 6f61 645f 646f 7465  otenv..load_dote
-00001ad0: 6e76 2829 0a0a 636f 6e66 6967 203d 204f  nv()..config = O
-00001ae0: 726d 5365 7276 6963 6528 0a20 2020 2064  rmService(.    d
-00001af0: 625f 7479 7065 3d22 796f 7572 5f64 625f  b_type="your_db_
-00001b00: 7479 7065 222c 0a20 2020 2063 6f6e 6669  type",.    confi
-00001b10: 675f 7061 7261 6d73 3d64 6963 7428 0a20  g_params=dict(. 
-00001b20: 2020 2020 2020 2075 7365 723d 6f73 2e67         user=os.g
-00001b30: 6574 656e 7628 2244 425f 5553 4552 2229  etenv("DB_USER")
-00001b40: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
-00001b50: 7264 3d6f 732e 6765 7465 6e76 2822 4442  rd=os.getenv("DB
-00001b60: 5f50 4153 5357 4f52 4422 292c 0a20 2020  _PASSWORD"),.   
-00001b70: 2020 2020 2068 6f73 743d 6f73 2e67 6574       host=os.get
-00001b80: 656e 7628 2244 425f 484f 5354 2229 2c0a  env("DB_HOST"),.
-00001b90: 2020 2020 2020 2020 706f 7274 3d6f 732e          port=os.
-00001ba0: 6765 7465 6e76 2822 4442 5f50 4f52 5422  getenv("DB_PORT"
-00001bb0: 292c 0a20 2020 2020 2020 2064 6174 6162  ),.        datab
-00001bc0: 6173 653d 6f73 2e67 6574 656e 7628 2244  ase=os.getenv("D
-00001bd0: 425f 4e41 4d45 2229 2c0a 2020 2020 292c  B_NAME"),.    ),
-00001be0: 0a29 0a60 6060 0a0a 5468 6973 2069 7320  .).```..This is 
-00001bf0: 7468 6520 6f72 6d5f 636f 6e66 6967 2e70  the orm_config.p
-00001c00: 7920 6669 6c65 2c20 7768 6963 6820 636f  y file, which co
-00001c10: 6e74 6169 6e73 2074 6865 2063 6f6e 6669  ntains the confi
-00001c20: 6775 7261 7469 6f6e 2066 6f72 2079 6f75  guration for you
-00001c30: 7220 4f52 4d20 284f 626a 6563 742d 5265  r ORM (Object-Re
-00001c40: 6c61 7469 6f6e 616c 204d 6170 7069 6e67  lational Mapping
-00001c50: 2920 7365 7276 6963 652e 0a0a 4974 2069  ) service...It i
-00001c60: 6d70 6f72 7473 206e 6563 6573 7361 7279  mports necessary
-00001c70: 206c 6962 7261 7269 6573 2c20 6c6f 6164   libraries, load
-00001c80: 7320 656e 7669 726f 6e6d 656e 7420 7661  s environment va
-00001c90: 7269 6162 6c65 7320 7573 696e 6720 646f  riables using do
-00001ca0: 7465 6e76 2c20 616e 6420 6372 6561 7465  tenv, and create
-00001cb0: 7320 616e 204f 726d 5365 7276 6963 6520  s an OrmService 
-00001cc0: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00001cd0: 7370 6563 6966 6965 6420 6461 7461 6261  specified databa
-00001ce0: 7365 2074 7970 6520 616e 6420 636f 6e66  se type and conf
-00001cf0: 6967 7572 6174 696f 6e20 7061 7261 6d65  iguration parame
-00001d00: 7465 7273 2e0a 0a2d 2d2d 0a0a 4f6e 6365  ters...---..Once
-00001d10: 2077 6520 7365 7420 7570 2074 6869 7320   we set up this 
-00001d20: 3320 6669 6c65 732c 2077 6520 6361 6e20  3 files, we can 
-00001d30: 7374 6172 7420 6372 6561 7469 6e67 206f  start creating o
-00001d40: 7572 206d 6f64 756c 6573 2e20 6561 6368  ur modules. each
-00001d50: 206d 6f64 756c 6520 6973 2061 2066 6f6c   module is a fol
-00001d60: 6465 7220 7769 7468 2074 6865 2066 6f6c  der with the fol
-00001d70: 6c6f 7769 6e67 2073 7472 7563 7475 7265  lowing structure
-00001d80: 3a0a 0a60 6060 7465 7874 200a e294 9ce2  :..```text .....
-00001d90: 9480 e294 8020 7072 6f64 7563 7473 0ae2  ..... products..
-00001da0: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
-00001db0: 5f5f 696e 6974 5f5f 2e70 790a e294 8220  __init__.py.... 
-00001dc0: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
-00001dd0: 6475 6374 735f 636f 6e74 726f 6c6c 6572  ducts_controller
-00001de0: 2e70 790a e294 8220 2020 20e2 949c e294  .py....    .....
-00001df0: 80e2 9480 2070 726f 6475 6374 735f 7365  .... products_se
-00001e00: 7276 6963 652e 7079 0ae2 9482 2020 2020  rvice.py....    
-00001e10: e294 9ce2 9480 e294 8020 7072 6f64 7563  ......... produc
-00001e20: 7473 5f6d 6f64 656c 2e70 790a 7c20 2020  ts_model.py.|   
-00001e30: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
-00001e40: 6374 735f 656e 7469 7479 2e70 790a e294  cts_entity.py...
-00001e50: 8220 2020 20e2 949c e294 80e2 9480 2070  .    ......... p
-00001e60: 726f 6475 6374 735f 6d6f 6475 6c65 2e70  roducts_module.p
-00001e70: 790a 6060 600a 0a54 6869 7320 6973 2074  y.```..This is t
-00001e80: 6865 2073 7472 7563 7475 7265 206f 6620  he structure of 
-00001e90: 6120 6d6f 6475 6c65 2066 6f6c 6465 722e  a module folder.
-00001ea0: 2049 7420 696e 636c 7564 6573 2061 6e20   It includes an 
-00001eb0: 5f5f 696e 6974 5f5f 2e70 7920 6669 6c65  __init__.py file
-00001ec0: 2074 6f20 6d61 6b65 2074 6865 2066 6f6c   to make the fol
-00001ed0: 6465 7220 6120 5079 7468 6f6e 2070 6163  der a Python pac
-00001ee0: 6b61 6765 2c0a 3c62 723e 0a41 7320 7765  kage,.<br>.As we
-00001ef0: 6c6c 2061 7320 7370 6563 6966 6963 2066  ll as specific f
-00001f00: 696c 6573 2066 6f72 2074 6865 206d 6f64  iles for the mod
-00001f10: 756c 6527 7320 636f 6e74 726f 6c6c 6572  ule's controller
-00001f20: 2c20 7365 7276 6963 652c 206d 6f64 656c  , service, model
-00001f30: 2c20 656e 7469 7479 2c20 616e 6420 6d6f  , entity, and mo
-00001f40: 6475 6c65 2063 6f6e 6669 6775 7261 7469  dule configurati
-00001f50: 6f6e 732e 0a0a 2323 2323 2070 726f 6475  ons...#### produ
-00001f60: 6374 735f 6d6f 6465 6c2e 7079 0a60 6060  cts_model.py.```
-00001f70: 7079 7468 6f6e 0a66 726f 6d20 7079 6461  python.from pyda
-00001f80: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
-00001f90: 4d6f 6465 6c0a 0a0a 636c 6173 7320 5072  Model...class Pr
-00001fa0: 6f64 7563 7428 4261 7365 4d6f 6465 6c29  oduct(BaseModel)
-00001fb0: 3a0a 2020 2020 6e61 6d65 3a20 7374 720a  :.    name: str.
-00001fc0: 2020 2020 7072 6963 653a 2066 6c6f 6174      price: float
-00001fd0: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00001fe0: 3a20 7374 720a 6060 600a 0a54 6869 7320  : str.```..This 
-00001ff0: 6973 2074 6865 2070 726f 6475 6374 735f  is the products_
-00002000: 6d6f 6465 6c2e 7079 2066 696c 652c 2077  model.py file, w
-00002010: 6869 6368 2064 6566 696e 6573 2074 6865  hich defines the
-00002020: 2050 726f 6475 6374 206d 6f64 656c 2075   Product model u
-00002030: 7369 6e67 2074 6865 2042 6173 654d 6f64  sing the BaseMod
-00002040: 656c 2063 6c61 7373 2066 726f 6d20 7468  el class from th
-00002050: 6520 7079 6461 6e74 6963 206c 6962 7261  e pydantic libra
-00002060: 7279 2e0a 3c62 723e 0a54 6865 206d 6f64  ry..<br>.The mod
-00002070: 656c 2072 6570 7265 7365 6e74 7320 7468  el represents th
-00002080: 6520 7374 7275 6374 7572 6520 616e 6420  e structure and 
-00002090: 6174 7472 6962 7574 6573 206f 6620 6120  attributes of a 
-000020a0: 7072 6f64 7563 742e 0a0a 2323 2323 2070  product...#### p
-000020b0: 726f 6475 6374 735f 656e 7469 7479 2e70  roducts_entity.p
-000020c0: 790a 0a60 6060 7079 7468 6f6e 0a66 726f  y..```python.fro
-000020d0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
-000020e0: 6f72 7420 436f 6c75 6d6e 2c20 496e 7465  ort Column, Inte
-000020f0: 6765 722c 2053 7472 696e 672c 2046 6c6f  ger, String, Flo
-00002100: 6174 0a66 726f 6d20 6f72 6d5f 636f 6e66  at.from orm_conf
-00002110: 6967 2069 6d70 6f72 7420 636f 6e66 6967  ig import config
-00002120: 0a0a 0a63 6c61 7373 2050 726f 6475 6374  ...class Product
-00002130: 2863 6f6e 6669 672e 4261 7365 293a 0a20  (config.Base):. 
-00002140: 2020 205f 5f74 6162 6c65 6e61 6d65 5f5f     __tablename__
-00002150: 203d 2022 7072 6f64 7563 7473 220a 0a20   = "products".. 
-00002160: 2020 2069 6420 3d20 436f 6c75 6d6e 2849     id = Column(I
-00002170: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-00002180: 6b65 793d 5472 7565 2c20 696e 6465 783d  key=True, index=
-00002190: 5472 7565 2c20 6175 746f 696e 6372 656d  True, autoincrem
-000021a0: 656e 743d 5472 7565 290a 2020 2020 6e61  ent=True).    na
-000021b0: 6d65 203d 2043 6f6c 756d 6e28 5374 7269  me = Column(Stri
-000021c0: 6e67 290a 2020 2020 7072 6963 6520 3d20  ng).    price = 
-000021d0: 436f 6c75 6d6e 2846 6c6f 6174 290a 2020  Column(Float).  
-000021e0: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
-000021f0: 436f 6c75 6d6e 2853 7472 696e 6729 0a60  Column(String).`
-00002200: 6060 0a0a 5468 6973 2069 7320 7468 6520  ``..This is the 
-00002210: 7072 6f64 7563 7473 5f65 6e74 6974 792e  products_entity.
-00002220: 7079 2066 696c 652c 2077 6869 6368 2064  py file, which d
-00002230: 6566 696e 6573 2074 6865 2050 726f 6475  efines the Produ
-00002240: 6374 2065 6e74 6974 7920 7573 696e 6720  ct entity using 
-00002250: 5351 4c41 6c63 6865 6d79 2e20 0a3c 6272  SQLAlchemy. .<br
-00002260: 3e0a 4974 2069 6d70 6f72 7473 206e 6563  >.It imports nec
-00002270: 6573 7361 7279 206d 6f64 756c 6573 2061  essary modules a
-00002280: 6e64 2069 6e68 6572 6974 7320 6672 6f6d  nd inherits from
-00002290: 2074 6865 2063 6f6e 6669 672e 4261 7365   the config.Base
-000022a0: 2063 6c61 7373 2e20 5468 6520 656e 7469   class. The enti
-000022b0: 7479 2072 6570 7265 7365 6e74 7320 7468  ty represents th
-000022c0: 6520 6461 7461 6261 7365 2074 6162 6c65  e database table
-000022d0: 2066 6f72 2073 746f 7269 6e67 2070 726f   for storing pro
-000022e0: 6475 6374 732c 2077 6974 6820 636f 6c75  ducts, with colu
-000022f0: 6d6e 7320 666f 7220 6964 2c20 6e61 6d65  mns for id, name
-00002300: 2c20 7072 6963 652c 2061 6e64 2064 6573  , price, and des
-00002310: 6372 6970 7469 6f6e 2e0a 0a23 2323 2320  cription...#### 
-00002320: 7072 6f64 7563 7473 5f73 6572 7669 6365  products_service
-00002330: 2e70 790a 0a60 6060 7079 7468 6f6e 0a66  .py..```python.f
-00002340: 726f 6d20 7372 632e 7072 6f64 7563 7473  rom src.products
-00002350: 2e70 726f 6475 6374 735f 6d6f 6465 6c20  .products_model 
-00002360: 696d 706f 7274 2050 726f 6475 6374 0a66  import Product.f
-00002370: 726f 6d20 7372 632e 7072 6f64 7563 7473  rom src.products
-00002380: 2e70 726f 6475 6374 735f 656e 7469 7479  .products_entity
-00002390: 2069 6d70 6f72 7420 5072 6f64 7563 7420   import Product 
-000023a0: 6173 2050 726f 6475 6374 456e 7469 7479  as ProductEntity
-000023b0: 0a66 726f 6d20 6f72 6d5f 636f 6e66 6967  .from orm_config
-000023c0: 2069 6d70 6f72 7420 636f 6e66 6967 0a66   import config.f
-000023d0: 726f 6d20 6e65 7374 2e63 6f72 652e 6465  rom nest.core.de
-000023e0: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
-000023f0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
-00002400: 6572 0a0a 0a63 6c61 7373 2050 726f 6475  er...class Produ
-00002410: 6374 7353 6572 7669 6365 3a0a 2020 2020  ctsService:.    
-00002420: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00002430: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00002440: 2e63 6f6e 6669 6720 3d20 636f 6e66 6967  .config = config
-00002450: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00002460: 7373 696f 6e20 3d20 7365 6c66 2e63 6f6e  ssion = self.con
-00002470: 6669 672e 6765 745f 6462 2829 0a0a 2020  fig.get_db()..  
-00002480: 2020 4064 625f 7265 7175 6573 745f 6861    @db_request_ha
-00002490: 6e64 6c65 720a 2020 2020 6465 6620 6164  ndler.    def ad
-000024a0: 645f 7072 6f64 7563 7428 7365 6c66 2c20  d_product(self, 
-000024b0: 7072 6f64 7563 743a 2050 726f 6475 6374  product: Product
-000024c0: 293a 0a20 2020 2020 2020 2070 726f 6475  ):.        produ
-000024d0: 6374 5f65 6e74 6974 7920 3d20 5072 6f64  ct_entity = Prod
-000024e0: 7563 7445 6e74 6974 7928 0a20 2020 2020  uctEntity(.     
-000024f0: 2020 2020 2020 206e 616d 653d 7072 6f64         name=prod
-00002500: 7563 742e 6e61 6d65 2c0a 2020 2020 2020  uct.name,.      
-00002510: 2020 2020 2020 7072 6963 653d 7072 6f64        price=prod
-00002520: 7563 742e 7072 6963 652c 0a20 2020 2020  uct.price,.     
-00002530: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00002540: 6f6e 3d70 726f 6475 6374 2e64 6573 6372  on=product.descr
-00002550: 6970 7469 6f6e 0a20 2020 2020 2020 2029  iption.        )
-00002560: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00002570: 7373 696f 6e2e 6164 6428 7072 6f64 7563  ssion.add(produc
-00002580: 745f 656e 7469 7479 290a 2020 2020 2020  t_entity).      
-00002590: 2020 7365 6c66 2e73 6573 7369 6f6e 2e63    self.session.c
-000025a0: 6f6d 6d69 7428 290a 2020 2020 2020 2020  ommit().        
-000025b0: 7265 7475 726e 2070 726f 6475 6374 5f65  return product_e
-000025c0: 6e74 6974 792e 6964 0a0a 2020 2020 4064  ntity.id..    @d
-000025d0: 625f 7265 7175 6573 745f 6861 6e64 6c65  b_request_handle
-000025e0: 720a 2020 2020 6465 6620 6765 745f 7072  r.    def get_pr
-000025f0: 6f64 7563 7473 2873 656c 6629 3a0a 2020  oducts(self):.  
-00002600: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002610: 662e 7365 7373 696f 6e2e 7175 6572 7928  f.session.query(
-00002620: 5072 6f64 7563 7445 6e74 6974 7929 2e61  ProductEntity).a
-00002630: 6c6c 2829 0a0a 2020 2020 4064 625f 7265  ll()..    @db_re
-00002640: 7175 6573 745f 6861 6e64 6c65 720a 2020  quest_handler.  
-00002650: 2020 6465 6620 6765 745f 7072 6f64 7563    def get_produc
-00002660: 7428 7365 6c66 2c20 7072 6f64 7563 745f  t(self, product_
-00002670: 6964 3a20 696e 7429 3a0a 2020 2020 2020  id: int):.      
-00002680: 2020 7265 7475 726e 2073 656c 662e 7365    return self.se
-00002690: 7373 696f 6e2e 7175 6572 7928 5072 6f64  ssion.query(Prod
-000026a0: 7563 7445 6e74 6974 7929 2e66 696c 7465  uctEntity).filte
-000026b0: 7228 5072 6f64 7563 7445 6e74 6974 792e  r(ProductEntity.
-000026c0: 6964 203d 3d20 7072 6f64 7563 745f 6964  id == product_id
-000026d0: 292e 6669 7273 7428 290a 0a20 2020 2040  ).first()..    @
-000026e0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
-000026f0: 6572 0a20 2020 2064 6566 206c 6173 745f  er.    def last_
-00002700: 7072 6f64 7563 7428 7365 6c66 293a 0a20  product(self):. 
-00002710: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00002720: 6c66 2e73 6573 7369 6f6e 2e71 7565 7279  lf.session.query
-00002730: 2850 726f 6475 6374 456e 7469 7479 292e  (ProductEntity).
-00002740: 6f72 6465 725f 6279 2850 726f 6475 6374  order_by(Product
-00002750: 456e 7469 7479 2e69 642e 6465 7363 2829  Entity.id.desc()
-00002760: 292e 6669 7273 7428 290a 6060 600a 0a54  ).first().```..T
-00002770: 6869 7320 6973 2074 6865 2073 6572 7669  his is the servi
-00002780: 6365 2066 696c 652c 2077 6869 6368 2063  ce file, which c
-00002790: 6f6e 7461 696e 7320 7468 6520 5072 6f64  ontains the Prod
-000027a0: 7563 7473 5365 7276 6963 6520 636c 6173  uctsService clas
-000027b0: 732e 2049 7420 696d 706f 7274 7320 6e65  s. It imports ne
-000027c0: 6365 7373 6172 7920 6d6f 6475 6c65 7320  cessary modules 
-000027d0: 616e 6420 6465 6669 6e65 7320 6d65 7468  and defines meth
-000027e0: 6f64 7320 666f 7220 696e 7465 7261 6374  ods for interact
-000027f0: 696e 6720 7769 7468 2074 6865 2064 6174  ing with the dat
-00002800: 6162 6173 652e 200a 3c62 723e 0a54 6865  abase. .<br>.The
-00002810: 206d 6574 686f 6473 2069 6e63 6c75 6465   methods include
-00002820: 2061 6464 696e 6720 6120 7072 6f64 7563   adding a produc
-00002830: 742c 2067 6574 7469 6e67 2061 6c6c 2070  t, getting all p
-00002840: 726f 6475 6374 732c 2067 6574 7469 6e67  roducts, getting
-00002850: 2061 2073 7065 6369 6669 6320 7072 6f64   a specific prod
-00002860: 7563 7420 6279 2049 442c 2061 6e64 2072  uct by ID, and r
-00002870: 6574 7269 6576 696e 6720 7468 6520 6c61  etrieving the la
-00002880: 7374 2061 6464 6564 2070 726f 6475 6374  st added product
-00002890: 2e0a 3c62 723e 0a54 6865 2060 4064 625f  ..<br>.The `@db_
-000028a0: 7265 7175 6573 745f 6861 6e64 6c65 7260  request_handler`
-000028b0: 2064 6563 6f72 6174 6f72 2069 7320 7265   decorator is re
-000028c0: 7370 6f6e 7369 626c 6520 666f 7220 6d61  sponsible for ma
-000028d0: 6e61 6769 6e67 2074 6865 2064 6174 6162  naging the datab
-000028e0: 6173 6520 7365 7373 696f 6e20 616e 6420  ase session and 
-000028f0: 6861 6e64 6c69 6e67 2061 6e79 2065 7863  handling any exc
-00002900: 6570 7469 6f6e 7320 7468 6174 206d 6179  eptions that may
-00002910: 206f 6363 7572 2064 7572 696e 6720 6461   occur during da
-00002920: 7461 6261 7365 206f 7065 7261 7469 6f6e  tabase operation
-00002930: 732e 0a0a 0a23 2323 2320 7072 6f64 7563  s....#### produc
-00002940: 7473 5f63 6f6e 7472 6f6c 6c65 722e 7079  ts_controller.py
-00002950: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00002960: 206e 6573 742e 636f 7265 2069 6d70 6f72   nest.core impor
-00002970: 7420 4465 7065 6e64 732c 2043 6f6e 7472  t Depends, Contr
-00002980: 6f6c 6c65 722c 2047 6574 2c20 506f 7374  oller, Get, Post
-00002990: 0a66 726f 6d20 7372 632e 7072 6f64 7563  .from src.produc
-000029a0: 7473 2e70 726f 6475 6374 735f 7365 7276  ts.products_serv
-000029b0: 6963 6520 696d 706f 7274 2050 726f 6475  ice import Produ
-000029c0: 6374 7353 6572 7669 6365 0a66 726f 6d20  ctsService.from 
-000029d0: 7372 632e 7072 6f64 7563 7473 2e70 726f  src.products.pro
-000029e0: 6475 6374 735f 6d6f 6465 6c20 696d 706f  ducts_model impo
-000029f0: 7274 2050 726f 6475 6374 0a0a 0a40 436f  rt Product...@Co
-00002a00: 6e74 726f 6c6c 6572 2822 7072 6f64 7563  ntroller("produc
-00002a10: 7473 2229 0a63 6c61 7373 2050 726f 6475  ts").class Produ
-00002a20: 6374 7343 6f6e 7472 6f6c 6c65 723a 0a20  ctsController:. 
-00002a30: 2020 2073 6572 7669 6365 3a20 5072 6f64     service: Prod
-00002a40: 7563 7473 5365 7276 6963 6520 3d20 4465  uctsService = De
-00002a50: 7065 6e64 7328 5072 6f64 7563 7473 5365  pends(ProductsSe
-00002a60: 7276 6963 6529 0a0a 2020 2020 4047 6574  rvice)..    @Get
-00002a70: 2822 2f67 6574 5f70 726f 6475 6374 7322  ("/get_products"
-00002a80: 290a 2020 2020 6465 6620 6765 745f 7072  ).    def get_pr
-00002a90: 6f64 7563 7473 2873 656c 6629 3a0a 2020  oducts(self):.  
-00002aa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002ab0: 662e 7365 7276 6963 652e 6765 745f 7072  f.service.get_pr
-00002ac0: 6f64 7563 7473 2829 0a0a 2020 2020 4047  oducts()..    @G
-00002ad0: 6574 2822 2f67 6574 5f70 726f 6475 6374  et("/get_product
-00002ae0: 2f7b 7072 6f64 7563 745f 6964 7d22 290a  /{product_id}").
-00002af0: 2020 2020 6465 6620 6765 745f 7072 6f64      def get_prod
-00002b00: 7563 7428 7365 6c66 2c20 7072 6f64 7563  uct(self, produc
-00002b10: 745f 6964 3a20 696e 7429 3a0a 2020 2020  t_id: int):.    
-00002b20: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002b30: 7365 7276 6963 652e 6765 745f 7072 6f64  service.get_prod
-00002b40: 7563 7428 7072 6f64 7563 745f 6964 290a  uct(product_id).
-00002b50: 0a20 2020 2040 506f 7374 2822 2f61 6464  .    @Post("/add
-00002b60: 5f70 726f 6475 6374 2229 0a20 2020 2064  _product").    d
-00002b70: 6566 2061 6464 5f70 726f 6475 6374 2873  ef add_product(s
-00002b80: 656c 662c 2070 726f 6475 6374 3a20 5072  elf, product: Pr
-00002b90: 6f64 7563 7429 3a0a 2020 2020 2020 2020  oduct):.        
-00002ba0: 7265 7475 726e 2073 656c 662e 7365 7276  return self.serv
-00002bb0: 6963 652e 6164 645f 7072 6f64 7563 7428  ice.add_product(
-00002bc0: 7072 6f64 7563 7429 0a0a 2020 2020 4047  product)..    @G
-00002bd0: 6574 2822 2f6c 6173 745f 7072 6f64 7563  et("/last_produc
-00002be0: 7422 290a 2020 2020 6465 6620 6c61 7374  t").    def last
-00002bf0: 5f70 726f 6475 6374 2873 656c 6629 3a0a  _product(self):.
-00002c00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002c10: 656c 662e 7365 7276 6963 652e 6c61 7374  elf.service.last
-00002c20: 5f70 726f 6475 6374 2829 0a60 6060 0a49  _product().```.I
-00002c30: 6e20 7375 6d6d 6172 792c 2074 6865 2060  n summary, the `
-00002c40: 6465 636f 7261 746f 7273 6020 616e 6420  decorators` and 
-00002c50: 7468 6520 6044 6570 656e 6473 6020 636c  the `Depends` cl
-00002c60: 6173 7320 6172 6520 7573 6564 2074 6f20  ass are used to 
-00002c70: 6465 6669 6e65 2072 6f75 7465 7320 616e  define routes an
-00002c80: 6420 4854 5450 206d 6574 686f 6473 2066  d HTTP methods f
-00002c90: 6f72 2074 6865 0a3c 6272 3e0a 6050 726f  or the.<br>.`Pro
-00002ca0: 6475 6374 7343 6f6e 7472 6f6c 6c65 7260  ductsController`
-00002cb0: 2063 6c61 7373 2c20 616e 6420 746f 2069   class, and to i
-00002cc0: 6e6a 6563 7420 7468 6520 6050 726f 6475  nject the `Produ
-00002cd0: 6374 7353 6572 7669 6365 6020 6465 7065  ctsService` depe
-00002ce0: 6e64 656e 6379 2069 6e74 6f20 7468 6520  ndency into the 
-00002cf0: 7365 7276 6963 6520 6174 7472 6962 7574  service attribut
-00002d00: 6520 6f66 2074 6865 2063 6f6e 7472 6f6c  e of the control
-00002d10: 6c65 722e 0a3c 6272 3e0a 5468 6973 2061  ler..<br>.This a
-00002d20: 6c6c 6f77 7320 7468 6520 636f 6e74 726f  llows the contro
-00002d30: 6c6c 6572 2074 6f20 6861 6e64 6c65 2069  ller to handle i
-00002d40: 6e63 6f6d 696e 6720 7265 7175 6573 7473  ncoming requests
-00002d50: 2061 6e64 2069 6e74 6572 6163 7420 7769   and interact wi
-00002d60: 7468 0a3c 6272 3e0a 5468 6520 7365 7276  th.<br>.The serv
-00002d70: 6963 6520 746f 2070 6572 666f 726d 2073  ice to perform s
-00002d80: 7065 6369 6669 6320 6163 7469 6f6e 7320  pecific actions 
-00002d90: 6261 7365 6420 6f6e 2074 6865 2072 6f75  based on the rou
-00002da0: 7465 7320 616e 6420 6d65 7468 6f64 7320  tes and methods 
-00002db0: 6465 6669 6e65 642e 0a0a 0a23 2323 2320  defined....#### 
-00002dc0: 7072 6f64 7563 7473 5f6d 6f64 756c 652e  products_module.
-00002dd0: 7079 0a0a 6060 6070 7974 686f 6e0a 6672  py..```python.fr
-00002de0: 6f6d 2073 7263 2e70 726f 6475 6374 732e  om src.products.
-00002df0: 7072 6f64 7563 7473 5f63 6f6e 7472 6f6c  products_control
-00002e00: 6c65 7220 696d 706f 7274 2050 726f 6475  ler import Produ
-00002e10: 6374 7343 6f6e 7472 6f6c 6c65 720a 6672  ctsController.fr
-00002e20: 6f6d 2073 7263 2e70 726f 6475 6374 732e  om src.products.
-00002e30: 7072 6f64 7563 7473 5f73 6572 7669 6365  products_service
-00002e40: 2069 6d70 6f72 7420 5072 6f64 7563 7473   import Products
-00002e50: 5365 7276 6963 650a 0a0a 636c 6173 7320  Service...class 
-00002e60: 5072 6f64 7563 7473 4d6f 6475 6c65 3a0a  ProductsModule:.
-00002e70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00002e80: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00002e90: 2073 656c 662e 7072 6f76 6964 6572 7320   self.providers 
-00002ea0: 3d20 5b50 726f 6475 6374 7353 6572 7669  = [ProductsServi
-00002eb0: 6365 5d0a 2020 2020 2020 2020 7365 6c66  ce].        self
-00002ec0: 2e63 6f6e 7472 6f6c 6c65 7273 203d 205b  .controllers = [
-00002ed0: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
-00002ee0: 6572 5d0a 6060 600a 0a54 6869 7320 6d6f  er].```..This mo
-00002ef0: 6475 6c65 2063 616e 2062 6520 7265 6769  dule can be regi
-00002f00: 7374 6572 6564 2061 6e64 2075 7365 6420  stered and used 
-00002f10: 696e 2079 6f75 7220 6170 706c 6963 6174  in your applicat
-00002f20: 696f 6e2e 204f 6e63 6520 7468 6520 6d6f  ion. Once the mo
-00002f30: 6475 6c65 2069 7320 7265 6769 7374 6572  dule is register
-00002f40: 6564 2c20 7468 6520 636f 6e74 726f 6c6c  ed, the controll
-00002f50: 6572 2072 6f75 7465 7320 7769 6c6c 2062  er routes will b
-00002f60: 6520 6176 6169 6c61 626c 6520 6174 2074  e available at t
-00002f70: 6865 2073 7065 6369 6669 6564 2070 6174  he specified pat
-00002f80: 682e 0a0a 5468 6973 2035 2063 6f6d 706f  h...This 5 compo
-00002f90: 6e65 6e74 7320 6172 6520 7468 6520 6d69  nents are the mi
-00002fa0: 6e69 6d75 6d20 7265 7175 6972 6564 2074  nimum required t
-00002fb0: 6f20 6372 6561 7465 2061 206d 6f64 756c  o create a modul
-00002fc0: 6520 7468 6174 2077 6f72 6b73 2077 6974  e that works wit
-00002fd0: 6820 7468 6520 4f52 4d2e 0a54 6865 7265  h the ORM..There
-00002fe0: 2061 7265 206d 616e 7920 6d6f 7265 206f   are many more o
-00002ff0: 7074 696f 6e73 206f 6620 686f 7720 796f  ptions of how yo
-00003000: 7520 6361 6e20 6465 7369 676e 2079 6f75  u can design you
-00003010: 7220 6d6f 6475 6c65 7320 616e 6420 7768  r modules and wh
-00003020: 6963 6820 6461 7461 6261 7365 7320 796f  ich databases yo
-00003030: 7520 6361 6e20 7573 652c 2062 7574 2074  u can use, but t
-00003040: 6869 7320 6973 2074 6865 2064 6566 6175  his is the defau
-00003050: 6c74 2062 6173 6963 2073 7472 7563 7475  lt basic structu
-00003060: 7265 2e0a 0a23 2320 4b65 7920 4665 6174  re...## Key Feat
-00003070: 7572 6573 0a23 2323 204d 6f64 756c 6172  ures.### Modular
-00003080: 2041 7263 6869 7465 6374 7572 650a 0a50   Architecture..P
-00003090: 794e 6573 7420 666f 6c6c 6f77 7320 7468  yNest follows th
-000030a0: 6520 6d6f 6475 6c61 7220 6172 6368 6974  e modular archit
-000030b0: 6563 7475 7265 206f 6620 4e65 7374 4a53  ecture of NestJS
-000030c0: 2c20 7768 6963 6820 616c 6c6f 7773 2066  , which allows f
-000030d0: 6f72 2065 6173 7920 7365 7061 7261 7469  or easy separati
-000030e0: 6f6e 206f 6620 636f 6e63 6572 6e73 2061  on of concerns a
-000030f0: 6e64 2063 6f64 6520 6f72 6761 6e69 7a61  nd code organiza
-00003100: 7469 6f6e 2e20 4561 6368 206d 6f64 756c  tion. Each modul
-00003110: 6520 636f 6e74 6169 6e73 2061 2063 6f6c  e contains a col
-00003120: 6c65 6374 696f 6e20 6f66 2072 656c 6174  lection of relat
-00003130: 6564 2063 6f6e 7472 6f6c 6c65 7273 2c20  ed controllers, 
-00003140: 7365 7276 6963 6573 2c20 616e 6420 7072  services, and pr
-00003150: 6f76 6964 6572 732e 0a0a 2323 2320 4465  oviders...### De
-00003160: 7065 6e64 656e 6379 2049 6e6a 6563 7469  pendency Injecti
-00003170: 6f6e 0a50 794e 6573 7420 7375 7070 6f72  on.PyNest suppor
-00003180: 7473 2064 6570 656e 6465 6e63 7920 696e  ts dependency in
-00003190: 6a65 6374 696f 6e2c 2077 6869 6368 206d  jection, which m
-000031a0: 616b 6573 2069 7420 6561 7379 2074 6f20  akes it easy to 
-000031b0: 6d61 6e61 6765 2064 6570 656e 6465 6e63  manage dependenc
-000031c0: 6965 7320 616e 6420 7772 6974 6520 7465  ies and write te
-000031d0: 7374 6162 6c65 2063 6f64 652e 2059 6f75  stable code. You
-000031e0: 2063 616e 2065 6173 696c 7920 696e 6a65   can easily inje
-000031f0: 6374 2073 6572 7669 6365 7320 616e 6420  ct services and 
-00003200: 7072 6f76 6964 6572 7320 696e 746f 2079  providers into y
-00003210: 6f75 7220 636f 6e74 726f 6c6c 6572 7320  our controllers 
-00003220: 7573 696e 6720 6465 636f 7261 746f 7273  using decorators
-00003230: 2e0a 0a0a 2323 2320 4465 636f 7261 746f  ....### Decorato
-00003240: 7273 0a0a 5079 4e65 7374 206d 616b 6573  rs..PyNest makes
-00003250: 2065 7874 656e 7369 7665 2075 7365 206f   extensive use o
-00003260: 6620 6465 636f 7261 746f 7273 2074 6f20  f decorators to 
-00003270: 6465 6669 6e65 2072 6f75 7465 732c 206d  define routes, m
-00003280: 6964 646c 6577 6172 652c 2061 6e64 206f  iddleware, and o
-00003290: 7468 6572 2061 7070 6c69 6361 7469 6f6e  ther application
-000032a0: 2063 6f6d 706f 6e65 6e74 732e 2054 6869   components. Thi
-000032b0: 7320 6865 6c70 7320 6b65 6570 2074 6865  s helps keep the
-000032c0: 2063 6f64 6520 636f 6e63 6973 6520 616e   code concise an
-000032d0: 6420 6561 7379 2074 6f20 7265 6164 2e0a  d easy to read..
-000032e0: 0a23 2323 2054 7970 6520 416e 6e6f 7461  .### Type Annota
-000032f0: 7469 6f6e 730a 0a50 794e 6573 7420 6c65  tions..PyNest le
-00003300: 7665 7261 6765 7320 5079 7468 6f6e 2773  verages Python's
-00003310: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
-00003320: 7320 746f 2070 726f 7669 6465 2062 6574  s to provide bet
-00003330: 7465 7220 746f 6f6c 696e 6720 616e 6420  ter tooling and 
-00003340: 6865 6c70 2070 7265 7665 6e74 2065 7272  help prevent err
-00003350: 6f72 732e 2059 6f75 2063 616e 2061 6e6e  ors. You can ann
-00003360: 6f74 6174 6520 796f 7572 2063 6f6e 7472  otate your contr
-00003370: 6f6c 6c65 7273 2c20 7365 7276 6963 6573  ollers, services
-00003380: 2c20 616e 6420 7072 6f76 6964 6572 7320  , and providers 
-00003390: 7769 7468 2074 7970 6573 2074 6f20 6d61  with types to ma
-000033a0: 6b65 2079 6f75 7220 636f 6465 206d 6f72  ke your code mor
-000033b0: 6520 726f 6275 7374 2e0a 0a23 2323 2043  e robust...### C
-000033c0: 6f64 6520 4765 6e65 7261 7469 6f6e 0a0a  ode Generation..
-000033d0: 5079 4e65 7374 2069 6e63 6c75 6465 7320  PyNest includes 
-000033e0: 6120 636f 6465 2067 656e 6572 6174 696f  a code generatio
-000033f0: 6e20 746f 6f6c 2074 6861 7420 6361 6e20  n tool that can 
-00003400: 6372 6561 7465 2062 6f69 6c65 7270 6c61  create boilerpla
-00003410: 7465 2063 6f64 6520 666f 7220 6d6f 6475  te code for modu
-00003420: 6c65 732c 2063 6f6e 7472 6f6c 6c65 7273  les, controllers
-00003430: 2c20 616e 6420 6f74 6865 7220 636f 6d70  , and other comp
-00003440: 6f6e 656e 7473 2e20 5468 6973 2073 6176  onents. This sav
-00003450: 6573 2079 6f75 2074 696d 6520 616e 6420  es you time and 
-00003460: 6865 6c70 7320 796f 7520 666f 6375 7320  helps you focus 
-00003470: 6f6e 2077 7269 7469 6e67 2074 6865 2063  on writing the c
-00003480: 6f64 6520 7468 6174 206d 6174 7465 7273  ode that matters
-00003490: 2e0a 0a23 2320 4675 7475 7265 2050 6c61  ...## Future Pla
-000034a0: 6e73 0a0a 2d20 5b20 5d20 4372 6561 7465  ns..- [ ] Create
-000034b0: 204d 6172 6b65 7470 6c61 6365 2066 6f72   Marketplace for
-000034c0: 206d 6f64 756c 6573 2077 6865 7265 2064   modules where d
-000034d0: 6576 656c 6f70 6572 7320 6361 6e20 7368  evelopers can sh
-000034e0: 6172 6520 7468 6569 7220 6d6f 6475 6c65  are their module
-000034f0: 7320 616e 6420 646f 776e 6c6f 6164 206d  s and download m
-00003500: 6f64 756c 6573 2063 7265 6174 6564 2062  odules created b
-00003510: 7920 6f74 6865 7273 2e0a 2d20 5b20 5d20  y others..- [ ] 
-00003520: 4372 6574 6520 4162 7374 7261 6374 696f  Crete Abstractio
-00003530: 6e20 636c 6173 7320 746f 204d 6f64 756c  n class to Modul
-00003540: 6573 2061 6e64 2053 6572 7669 6365 7320  es and Services 
-00003550: 746f 2061 6c6c 6f77 2066 6f72 2065 6173  to allow for eas
-00003560: 7920 6372 6561 7469 6f6e 206f 6620 6d6f  y creation of mo
-00003570: 6475 6c65 7320 616e 6420 7365 7276 6963  dules and servic
-00003580: 6573 2e0a 2d20 5b20 5d20 4164 6420 696e  es..- [ ] Add in
-00003590: 6865 7269 7461 6e63 6520 6265 7477 6565  heritance betwee
-000035a0: 6e20 636f 6e74 726f 6c6c 6572 7320 666f  n controllers fo
-000035b0: 7220 6372 6561 7469 6e67 206d 6f72 6520  r creating more 
-000035c0: 636f 6d70 6c65 7820 636f 6e74 726f 6c6c  complex controll
-000035d0: 6572 732e 0a2d 205b 205d 2041 6464 2073  ers..- [ ] Add s
-000035e0: 7570 706f 7274 2066 6f72 206f 7468 6572  upport for other
-000035f0: 2064 6174 6162 6173 6573 2028 6d6f 6e67   databases (mong
-00003600: 6f44 422c 2072 6564 6973 2c20 6574 632e  oDB, redis, etc.
-00003610: 290a 2d20 5b20 5d20 4372 6561 7465 206f  ).- [ ] Create o
-00003620: 7574 2d6f 662d 7468 652d 626f 7820 6175  ut-of-the-box au
-00003630: 7468 656e 7469 6361 7469 6f6e 206d 6f64  thentication mod
-00003640: 756c 6520 7468 6174 2063 616e 2062 6520  ule that can be 
-00003650: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00003660: 6420 696e 746f 2061 6e79 2061 7070 6c69  d into any appli
-00003670: 6361 7469 6f6e 2e0a 2d20 5b20 5d20 4164  cation..- [ ] Ad
-00003680: 6420 7375 7070 6f72 7420 666f 7220 6f74  d support for ot
-00003690: 6865 7220 7465 7374 696e 6720 6672 616d  her testing fram
-000036a0: 6577 6f72 6b73 2061 6e64 2063 7265 6174  eworks and creat
-000036b0: 6520 7465 7374 696e 6720 7465 6d70 6c61  e testing templa
-000036c0: 7465 732e 0a2d 205b 205d 2041 6464 2073  tes..- [ ] Add s
-000036d0: 7570 706f 7274 2066 6f72 206f 7468 6572  upport for other
-000036e0: 2077 6562 2066 7261 6d65 776f 726b 7320   web frameworks 
-000036f0: 2846 6c61 736b 2c20 446a 616e 676f 2c20  (Flask, Django, 
-00003700: 6574 632e 2920 2d20 5361 6d65 2041 7263  etc.) - Same Arc
-00003710: 6869 7465 6374 7572 652c 2064 6966 6665  hitecture, diffe
-00003720: 7265 6e74 2065 6e67 696e 652e 0a0a 0a23  rent engine....#
-00003730: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-00003740: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
-00003750: 6520 7765 6c63 6f6d 6521 2050 6c65 6173  e welcome! Pleas
-00003760: 6520 6665 656c 2066 7265 6520 746f 2067  e feel free to g
-00003770: 7261 6220 6f6e 6520 6f66 2074 6865 206f  rab one of the o
-00003780: 7065 6e20 6973 7375 6573 2c0a 6f72 206f  pen issues,.or o
-00003790: 7065 6e20 6120 6e65 7720 6f6e 6520 6966  pen a new one if
-000037a0: 2079 6f75 2068 6176 6520 616e 2069 6465   you have an ide
-000037b0: 6120 666f 7220 6120 6e65 7720 6665 6174  a for a new feat
-000037c0: 7572 6520 6f72 2069 6d70 726f 7665 6d65  ure or improveme
-000037d0: 6e74 2e0a 0a54 6869 7320 776f 756c 6420  nt...This would 
-000037e0: 6272 696e 6720 6120 6875 6765 2069 6d70  bring a huge imp
-000037f0: 6163 7420 746f 2074 6865 2070 726f 6a65  act to the proje
-00003800: 6374 2061 6e64 2074 6865 2063 6f6d 6d75  ct and the commu
-00003810: 6e69 7479 2e0a 0a23 2320 4c69 6365 6e73  nity...## Licens
-00003820: 650a 0a50 794e 6573 7420 6973 205b 4d49  e..PyNest is [MI
-00003830: 5420 6c69 6365 6e73 6564 5d28 4c49 4345  T licensed](LICE
-00003840: 4e53 4529 2e0a 0a23 2320 4372 6564 6974  NSE)...## Credit
-00003850: 730a 0a50 794e 6573 7420 6973 2069 6e73  s..PyNest is ins
-00003860: 7069 7265 6420 6279 205b 4e65 7374 4a53  pired by [NestJS
-00003870: 5d28 6874 7470 733a 2f2f 6e65 7374 6a73  ](https://nestjs
-00003880: 2e63 6f6d 2f29 2e0a                      .com/)..
+00000730: 2e31 300a 5265 7175 6972 6573 2d50 7974  .10.Requires-Pyt
+00000740: 686f 6e3a 203e 3d33 2e38 2e31 0a44 6573  hon: >=3.8.1.Des
+00000750: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000760: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000770: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+00000780: 7472 613a 2074 6573 740a 4c69 6365 6e73  tra: test.Licens
+00000790: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+000007a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000007b0: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
+000007c0: 646f 6373 2f69 6d67 732f 7079 6e65 7374  docs/imgs/pynest
+000007d0: 5f6c 6f67 6f2d 6d6f 6469 6669 6564 2e70  _logo-modified.p
+000007e0: 6e67 2220 7469 746c 653d 2270 796e 6573  ng" title="pynes
+000007f0: 7420 6c6f 676f 2220 7769 6474 683d 2232  t logo" width="2
+00000800: 3030 223e 0a3c 2f70 3e0a 3c70 2061 6c69  00">.</p>.<p ali
+00000810: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000820: 203c 656d 3e50 794e 6573 7420 6973 2061   <em>PyNest is a
+00000830: 2050 7974 686f 6e20 6672 616d 6577 6f72   Python framewor
+00000840: 6b20 6275 696c 7420 6f6e 2074 6f70 206f  k built on top o
+00000850: 6620 4661 7374 4150 4920 7468 6174 2066  f FastAPI that f
+00000860: 6f6c 6c6f 7773 2074 6865 206d 6f64 756c  ollows the modul
+00000870: 6172 2061 7263 6869 7465 6374 7572 6520  ar architecture 
+00000880: 6f66 204e 6573 744a 533c 2f65 6d3e 0a3c  of NestJS</em>.<
+00000890: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
+000008a0: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+000008b0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000008c0: 2e6f 7267 2f70 726f 6a65 6374 2f70 796e  .org/project/pyn
+000008d0: 6573 742d 6170 6922 3e0a 2020 2020 2020  est-api">.      
+000008e0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000008f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000900: 696f 2f70 7970 692f 762f 7079 6e65 7374  io/pypi/v/pynest
+00000910: 2d61 7069 3f63 6f6c 6f72 3d25 3233 3334  -api?color=%2334
+00000920: 4430 3538 266c 6162 656c 3d70 7970 6925  D058&label=pypi%
+00000930: 3230 7061 636b 6167 6522 2061 6c74 3d22  20package" alt="
+00000940: 5665 7273 696f 6e22 3e0a 2020 2020 3c2f  Version">.    </
+00000950: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000960: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000970: 2f70 726f 6a65 6374 2f70 796e 6573 742d  /project/pynest-
+00000980: 6170 6922 3e0a 2020 2020 2020 2020 3c69  api">.        <i
+00000990: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000009a0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000009b0: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
+000009c0: 796e 6573 742d 6170 692e 7376 673f 636f  ynest-api.svg?co
+000009d0: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
+000009e0: 6c74 3d22 5079 7468 6f6e 223e 0a20 2020  lt="Python">.   
+000009f0: 203c 2f61 3e0a 2020 2020 3c61 2068 7265   </a>.    <a hre
+00000a00: 663d 2268 7474 7073 3a2f 2f70 6570 792e  f="https://pepy.
+00000a10: 7465 6368 2f70 726f 6a65 6374 2f70 796e  tech/project/pyn
+00000a20: 6573 742d 6170 6922 3e0a 2020 2020 2020  est-api">.      
+00000a30: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000a40: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+00000a50: 7465 6368 2f70 6572 736f 6e61 6c69 7a65  tech/personalize
+00000a60: 642d 6261 6467 652f 7079 6e65 7374 2d61  d-badge/pynest-a
+00000a70: 7069 3f70 6572 696f 643d 6d6f 6e74 6826  pi?period=month&
+00000a80: 756e 6974 733d 696e 7465 726e 6174 696f  units=internatio
+00000a90: 6e61 6c5f 7379 7374 656d 266c 6566 745f  nal_system&left_
+00000aa0: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
+00000ab0: 5f63 6f6c 6f72 3d62 7269 6768 7467 7265  _color=brightgre
+00000ac0: 656e 266c 6566 745f 7465 7874 3d44 6f77  en&left_text=Dow
+00000ad0: 6e6c 6f61 6473 2220 616c 743d 2244 6f77  nloads" alt="Dow
+00000ae0: 6e6c 6f61 6473 223e 0a20 2020 203c 2f61  nloads">.    </a
+00000af0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00000b00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000b10: 6d2f 5079 7468 6f6e 4e65 7374 2f50 794e  m/PythonNest/PyN
+00000b20: 6573 742f 626c 6f62 2f6d 6169 6e2f 4c49  est/blob/main/LI
+00000b30: 4345 4e53 4522 3e0a 2020 2020 2020 2020  CENSE">.        
+00000b40: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000b50: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000b60: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+00000b70: 5079 7468 6f6e 4e65 7374 2f50 796e 6573  PythonNest/Pynes
+00000b80: 7422 2061 6c74 3d22 4c69 6365 6e73 6522  t" alt="License"
+00000b90: 3e0a 2020 2020 3c2f 613e 0a3c 2f70 3e0a  >.    </a>.</p>.
+00000ba0: 0a0a 2320 4465 7363 7269 7074 696f 6e0a  ..# Description.
+00000bb0: 0a50 794e 6573 7420 6973 2064 6573 6967  .PyNest is desig
+00000bc0: 6e65 6420 746f 2068 656c 7020 7374 7275  ned to help stru
+00000bd0: 6374 7572 6520 796f 7572 2041 5049 7320  cture your APIs 
+00000be0: 696e 2061 6e20 696e 7475 6974 6976 652c  in an intuitive,
+00000bf0: 2065 6173 7920 746f 2075 6e64 6572 7374   easy to underst
+00000c00: 616e 642c 2061 6e64 2065 6e6a 6f79 6162  and, and enjoyab
+00000c10: 6c65 2077 6179 2e0a 0a57 6974 6820 5079  le way...With Py
+00000c20: 4e65 7374 2c20 796f 7520 6361 6e20 6275  Nest, you can bu
+00000c30: 696c 6420 7363 616c 6162 6c65 2061 6e64  ild scalable and
+00000c40: 206d 6169 6e74 6169 6e61 626c 6520 4150   maintainable AP
+00000c50: 4973 2077 6974 6820 6561 7365 2e20 5468  Is with ease. Th
+00000c60: 6520 6672 616d 6577 6f72 6b20 7375 7070  e framework supp
+00000c70: 6f72 7473 2064 6570 656e 6465 6e63 7920  orts dependency 
+00000c80: 696e 6a65 6374 696f 6e2c 2074 7970 6520  injection, type 
+00000c90: 616e 6e6f 7461 7469 6f6e 732c 2064 6563  annotations, dec
+00000ca0: 6f72 6174 6f72 732c 2061 6e64 2063 6f64  orators, and cod
+00000cb0: 6520 6765 6e65 7261 7469 6f6e 2c20 6d61  e generation, ma
+00000cc0: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
+00000cd0: 7772 6974 6520 636c 6561 6e20 616e 6420  write clean and 
+00000ce0: 7465 7374 6162 6c65 2063 6f64 652e 0a0a  testable code...
+00000cf0: 5468 6973 2066 7261 6d65 776f 726b 2069  This framework i
+00000d00: 7320 6e6f 7420 6120 6469 7265 6374 2070  s not a direct p
+00000d10: 6f72 7420 6f66 204e 6573 744a 5320 746f  ort of NestJS to
+00000d20: 2050 7974 686f 6e20 6275 7420 7261 7468   Python but rath
+00000d30: 6572 2061 2072 652d 696d 6167 696e 696e  er a re-imaginin
+00000d40: 6720 6f66 2074 6865 2066 7261 6d65 776f  g of the framewo
+00000d50: 726b 2073 7065 6369 6669 6361 6c6c 7920  rk specifically 
+00000d60: 666f 7220 5079 7468 6f6e 2064 6576 656c  for Python devel
+00000d70: 6f70 6572 732c 2069 6e63 6c75 6469 6e67  opers, including
+00000d80: 2064 6174 6120 7363 6965 6e74 6973 7473   data scientists
+00000d90: 2c20 6461 7461 2061 6e61 6c79 7374 732c  , data analysts,
+00000da0: 2061 6e64 2064 6174 6120 656e 6769 6e65   and data engine
+00000db0: 6572 732e 2049 7420 6169 6d73 2074 6f20  ers. It aims to 
+00000dc0: 6173 7369 7374 2074 6865 6d20 696e 2062  assist them in b
+00000dd0: 7569 6c64 696e 6720 6265 7474 6572 2061  uilding better a
+00000de0: 6e64 2066 6173 7465 7220 4150 4973 2066  nd faster APIs f
+00000df0: 6f72 2074 6865 6972 2064 6174 6120 6170  or their data ap
+00000e00: 706c 6963 6174 696f 6e73 2e0a 0a23 2320  plications...## 
+00000e10: 4765 7474 696e 6720 5374 6172 7465 640a  Getting Started.
+00000e20: 546f 2067 6574 2073 7461 7274 6564 2077  To get started w
+00000e30: 6974 6820 5079 4e65 7374 2c20 796f 7527  ith PyNest, you'
+00000e40: 6c6c 206e 6565 6420 746f 2069 6e73 7461  ll need to insta
+00000e50: 6c6c 2069 7420 7573 696e 6720 7069 703a  ll it using pip:
+00000e60: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00000e70: 7374 616c 6c20 7079 6e65 7374 2d61 7069  stall pynest-api
+00000e80: 0a60 6060 0a0a 2323 2320 5374 6172 7420  .```..### Start 
+00000e90: 7769 7468 2063 6c69 0a60 6060 6261 7368  with cli.```bash
+00000ea0: 0a70 796e 6573 7420 6372 6561 7465 2d6e  .pynest create-n
+00000eb0: 6573 742d 6170 7020 2d6e 206d 795f 6170  est-app -n my_ap
+00000ec0: 705f 6e61 6d65 0a60 6060 0a0a 7468 6973  p_name.```..this
+00000ed0: 2063 6f6d 6d61 6e64 2077 696c 6c20 6372   command will cr
+00000ee0: 6561 7465 2061 206e 6577 2070 726f 6a65  eate a new proje
+00000ef0: 6374 2077 6974 6820 7468 6520 666f 6c6c  ct with the foll
+00000f00: 6f77 696e 6720 7374 7275 6374 7572 653a  owing structure:
+00000f10: 0a0a 6060 6074 6578 740a e294 9ce2 9480  ..```text.......
+00000f20: e294 8020 6170 702e 7079 0ae2 949c e294  ... app.py......
+00000f30: 80e2 9480 206f 726d 5f63 6f6e 6669 672e  .... orm_config.
+00000f40: 7079 0ae2 949c e294 80e2 9480 206d 6169  py.......... mai
+00000f50: 6e2e 7079 0ae2 949c e294 80e2 9480 2073  n.py.......... s
+00000f60: 7263 0ae2 9482 2020 2020 e294 9ce2 9480  rc....    ......
+00000f70: e294 8020 5f5f 696e 6974 5f5f 2e70 790a  ... __init__.py.
+00000f80: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00000f90: 2065 7861 6d70 6c65 730a e294 8220 2020   examples....   
+00000fa0: 20e2 9482 2020 2020 e294 9ce2 9480 e294   ...    ........
+00000fb0: 8020 5f5f 696e 6974 5f5f 2e70 790a e294  . __init__.py...
+00000fc0: 8220 2020 20e2 9482 2020 2020 e294 9ce2  .    ...    ....
+00000fd0: 9480 e294 8020 6578 616d 706c 6573 5f63  ..... examples_c
+00000fe0: 6f6e 7472 6f6c 6c65 722e 7079 0ae2 9482  ontroller.py....
+00000ff0: 2020 2020 e294 8220 2020 20e2 949c e294      ...    .....
+00001000: 80e2 9480 2065 7861 6d70 6c65 735f 7365  .... examples_se
+00001010: 7276 6963 652e 7079 0ae2 9482 2020 2020  rvice.py....    
+00001020: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001030: 2065 7861 6d70 6c65 735f 6d6f 6465 6c2e   examples_model.
+00001040: 7079 0ae2 9482 2020 2020 e294 9ce2 9480  py....    ......
+00001050: e294 8020 20e2 949c e294 80e2 9480 2065  ...  ......... e
+00001060: 7861 6d70 6c65 735f 656e 7469 7479 2e70  xamples_entity.p
+00001070: 790a e294 8220 2020 20e2 949c e294 80e2  y....    .......
+00001080: 9480 2020 e294 9ce2 9480 e294 8020 6578  ..  ......... ex
+00001090: 616d 706c 6573 5f6d 6f64 756c 652e 7079  amples_module.py
+000010a0: 0a60 6060 0a0a 6f6e 6365 2079 6f75 2068  .```..once you h
+000010b0: 6176 6520 6372 6561 7465 6420 796f 7572  ave created your
+000010c0: 2061 7070 2c20 6765 7420 696e 746f 2074   app, get into t
+000010d0: 6865 2066 6f6c 6465 7220 616e 6420 7275  he folder and ru
+000010e0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000010f0: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
+00001100: 680a 6364 206d 795f 6170 705f 6e61 6d65  h.cd my_app_name
+00001110: 0a60 6060 0a0a 7275 6e20 7468 6520 7365  .```..run the se
+00001120: 7276 6572 2077 6974 6820 7468 6520 666f  rver with the fo
+00001130: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+00001140: 0a0a 6060 6062 6173 680a 7576 6963 6f72  ..```bash.uvicor
+00001150: 6e20 2261 7070 3a61 7070 2220 2d2d 686f  n "app:app" --ho
+00001160: 7374 2022 302e 302e 302e 3022 202d 2d70  st "0.0.0.0" --p
+00001170: 6f72 7420 2238 3022 202d 2d72 656c 6f61  ort "80" --reloa
+00001180: 640a 6060 600a 0a4e 6f77 2079 6f75 2063  d.```..Now you c
+00001190: 616e 2076 6973 6974 205b 4f70 656e 4150  an visit [OpenAP
+000011a0: 495d 2868 7474 703a 2f2f 6c6f 6361 6c68  I](http://localh
+000011b0: 6f73 743a 3830 2f64 6f63 7329 2069 6e20  ost:80/docs) in 
+000011c0: 796f 7572 2062 726f 7773 6572 2074 6f20  your browser to 
+000011d0: 7365 6520 7468 6520 6465 6661 756c 7420  see the default 
+000011e0: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
+000011f0: 6e2e 0a0a 2323 2320 4164 6469 6e67 206d  n...### Adding m
+00001200: 6f64 756c 6573 0a0a 546f 2061 6464 2061  odules..To add a
+00001210: 206e 6577 206d 6f64 756c 6520 746f 2079   new module to y
+00001220: 6f75 7220 6170 706c 6963 6174 696f 6e2c  our application,
+00001230: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
+00001240: 2070 796e 6573 7420 6765 6e65 7261 7465   pynest generate
+00001250: 206d 6f64 756c 6520 636f 6d6d 616e 643a   module command:
+00001260: 0a0a 6060 6062 6173 680a 7079 6e65 7374  ..```bash.pynest
+00001270: 2067 656e 6572 6174 652d 6d6f 6475 6c65   generate-module
+00001280: 202d 6e20 7573 6572 730a 6060 600a 0a54   -n users.```..T
+00001290: 6869 7320 7769 6c6c 2063 7265 6174 6520  his will create 
+000012a0: 6120 6e65 7720 6d6f 6475 6c65 2063 616c  a new module cal
+000012b0: 6c65 6420 6060 6075 7365 7273 6060 6020  led ```users``` 
+000012c0: 696e 2079 6f75 7220 6170 706c 6963 6174  in your applicat
+000012d0: 696f 6e20 7769 7468 2074 6865 2066 6f6c  ion with the fol
+000012e0: 6c6f 7769 6e67 2073 7472 7563 7475 7265  lowing structure
+000012f0: 3a0a 0a60 6060 7465 7874 0ae2 949c e294  :..```text......
+00001300: 80e2 9480 2075 7365 7273 0ae2 9482 2020  .... users....  
+00001310: 2020 e294 9ce2 9480 e294 8020 5f5f 696e    ......... __in
+00001320: 6974 5f5f 2e70 790a e294 8220 2020 20e2  it__.py....    .
+00001330: 949c e294 80e2 9480 2075 7365 7273 5f63  ........ users_c
+00001340: 6f6e 7472 6f6c 6c65 722e 7079 0ae2 9482  ontroller.py....
+00001350: 2020 2020 e294 9ce2 9480 e294 8020 7573      ......... us
+00001360: 6572 735f 7365 7276 6963 652e 7079 0ae2  ers_service.py..
+00001370: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+00001380: 7573 6572 735f 6d6f 6465 6c2e 7079 0ae2  users_model.py..
+00001390: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+000013a0: 7573 6572 735f 656e 7469 7479 2e70 790a  users_entity.py.
+000013b0: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+000013c0: 2075 7365 7273 5f6d 6f64 756c 652e 7079   users_module.py
+000013d0: 0a60 6060 0a0a 5468 6520 7573 6572 7320  .```..The users 
+000013e0: 6d6f 6475 6c65 2077 696c 6c20 696d 6d65  module will imme
+000013f0: 6469 6174 656c 7920 7265 6769 7374 6572  diately register
+00001400: 2069 7473 656c 6620 7769 7468 2074 6865   itself with the
+00001410: 2061 7070 6c69 6361 7469 6f6e 2061 6e64   application and
+00001420: 2077 696c 6c20 6265 2061 7661 696c 6162   will be availab
+00001430: 6c65 2066 6f72 2075 7365 2e0a 0a59 6f75  le for use...You
+00001440: 2063 616e 2074 6865 6e20 7374 6172 7420   can then start 
+00001450: 6465 6669 6e69 6e67 2072 6f75 7465 7320  defining routes 
+00001460: 616e 6420 6f74 6865 7220 6170 706c 6963  and other applic
+00001470: 6174 696f 6e20 636f 6d70 6f6e 656e 7473  ation components
+00001480: 2075 7369 6e67 2064 6563 6f72 6174 6f72   using decorator
+00001490: 7320 616e 6420 6f74 6865 7220 5079 4e65  s and other PyNe
+000014a0: 7374 2063 6f6e 7374 7275 6374 732e 0a0a  st constructs...
+000014b0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+000014c0: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
+000014d0: 7365 2050 794e 6573 742c 2063 6865 636b  se PyNest, check
+000014e0: 206f 7574 2074 6865 206f 6666 6963 6961   out the officia
+000014f0: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
+00001500: 6174 2068 7474 7073 3a2f 2f70 7974 686f  at https://pytho
+00001510: 6e6e 6573 742e 6769 7468 7562 2e69 6f2f  nnest.github.io/
+00001520: 5079 4e65 7374 2f2e 0a0a 2323 2053 7461  PyNest/...## Sta
+00001530: 7274 696e 6720 6120 6e65 7720 7072 6f6a  rting a new proj
+00001540: 6563 7420 6d61 6e75 616c 6c79 0a0a 6060  ect manually..``
+00001550: 6074 6578 740a 4e4f 5449 4345 3a20 666f  `text.NOTICE: fo
+00001560: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+00001570: 6578 616d 706c 652c 2077 6520 7769 6c6c  example, we will
+00001580: 2075 7365 2074 6865 2070 726f 6475 6374   use the product
+00001590: 7320 6d6f 6475 6c65 2e20 0a60 6060 0a0a  s module. .```..
+000015a0: 546f 2073 7461 7274 2061 206e 6577 2070  To start a new p
+000015b0: 726f 6a65 6374 206d 616e 7561 6c6c 792c  roject manually,
+000015c0: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
+000015d0: 6372 6561 7465 2061 2070 726f 6a65 6374  create a project
+000015e0: 2074 6861 7420 666f 6c6c 6f77 7320 7468   that follows th
+000015f0: 6973 2073 7472 7563 7475 7265 3a0a 0a60  is structure:..`
+00001600: 6060 7465 7874 0ae2 949c e294 80e2 9480  ``text..........
+00001610: 2061 7070 2e70 790a e294 9ce2 9480 e294   app.py.........
+00001620: 8020 6f72 6d5f 636f 6e66 6967 2e70 790a  . orm_config.py.
+00001630: e294 9ce2 9480 e294 8020 6d61 696e 2e70  ......... main.p
+00001640: 790a e294 9ce2 9480 e294 8020 7372 630a  y.......... src.
+00001650: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001660: 205f 5f69 6e69 745f 5f2e 7079 0ae2 9482   __init__.py....
+00001670: 2020 2020 e294 9ce2 9480 e294 8020 7072      ......... pr
+00001680: 6f64 7563 7473 0ae2 9482 2020 2020 e294  oducts....    ..
+00001690: 8220 2020 20e2 949c e294 80e2 9480 205f  .    ......... _
+000016a0: 5f69 6e69 745f 5f2e 7079 0ae2 9482 2020  _init__.py....  
+000016b0: 2020 e294 8220 2020 20e2 949c e294 80e2    ...    .......
+000016c0: 9480 2070 726f 6475 6374 735f 636f 6e74  .. products_cont
+000016d0: 726f 6c6c 6572 2e70 790a e294 8220 2020  roller.py....   
+000016e0: 20e2 9482 2020 2020 e294 9ce2 9480 e294   ...    ........
+000016f0: 8020 7072 6f64 7563 7473 5f73 6572 7669  . products_servi
+00001700: 6365 2e70 790a e294 8220 2020 20e2 9482  ce.py....    ...
+00001710: 2020 2020 e294 9ce2 9480 e294 8020 7072      ......... pr
+00001720: 6f64 7563 7473 5f6d 6f64 656c 2e70 790a  oducts_model.py.
+00001730: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001740: 2020 e294 9ce2 9480 e294 8020 7072 6f64    ......... prod
+00001750: 7563 7473 5f65 6e74 6974 792e 7079 0ae2  ucts_entity.py..
+00001760: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+00001770: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
+00001780: 6374 735f 6d6f 6475 6c65 2e70 790a 6060  cts_module.py.``
+00001790: 600a 0a45 7870 6c61 6e61 7469 6f6e 3a20  `..Explanation: 
+000017a0: 5468 6973 2069 7320 7468 6520 6469 7265  This is the dire
+000017b0: 6374 6f72 7920 7374 7275 6374 7572 6520  ctory structure 
+000017c0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+000017d0: 2e20 4974 2069 6e63 6c75 6465 7320 7468  . It includes th
+000017e0: 6520 6d61 696e 2066 696c 6573 2061 6e64  e main files and
+000017f0: 2061 2073 7263 2064 6972 6563 746f 7279   a src directory
+00001800: 2074 6861 7420 636f 6e74 6169 6e73 2079   that contains y
+00001810: 6f75 7220 7072 6f6a 6563 7427 7320 736f  our project's so
+00001820: 7572 6365 2063 6f64 652e 0a0a 2323 2320  urce code...### 
+00001830: 4372 6561 7469 6e67 2074 6865 2066 696c  Creating the fil
+00001840: 6573 0a0a 2323 2323 206d 6169 6e2e 7079  es..#### main.py
+00001850: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00001860: 7420 7576 6963 6f72 6e0a 0a0a 6966 205f  t uvicorn...if _
+00001870: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00001880: 696e 5f5f 273a 0a20 2020 2075 7669 636f  in__':.    uvico
+00001890: 726e 2e72 756e 280a 2020 2020 2020 2020  rn.run(.        
+000018a0: 2761 7070 3a61 7070 272c 0a20 2020 2020  'app:app',.     
+000018b0: 2020 2068 6f73 743d 2230 2e30 2e30 2e30     host="0.0.0.0
+000018c0: 222c 0a20 2020 2020 2020 2070 6f72 743d  ",.        port=
+000018d0: 3830 2c0a 2020 2020 290a 6060 600a 0a54  80,.    ).```..T
+000018e0: 6869 7320 6973 2074 6865 206d 6169 6e2e  his is the main.
+000018f0: 7079 2066 696c 652c 2077 6869 6368 2069  py file, which i
+00001900: 7320 7265 7370 6f6e 7369 626c 6520 666f  s responsible fo
+00001910: 7220 7275 6e6e 696e 6720 796f 7572 2061  r running your a
+00001920: 7070 6c69 6361 7469 6f6e 2075 7369 6e67  pplication using
+00001930: 2074 6865 2055 7669 636f 726e 2073 6572   the Uvicorn ser
+00001940: 7665 722e 0a3c 6272 3e0a 4974 2069 6d70  ver..<br>.It imp
+00001950: 6f72 7473 2074 6865 2075 7669 636f 726e  orts the uvicorn
+00001960: 206c 6962 7261 7279 2061 6e64 2073 7461   library and sta
+00001970: 7274 7320 7468 6520 7365 7276 6572 2077  rts the server w
+00001980: 6974 6820 7468 6520 7370 6563 6966 6965  ith the specifie
+00001990: 6420 686f 7374 2061 6e64 2070 6f72 742e  d host and port.
+000019a0: 0a0a 0a23 2323 2320 6170 702e 7079 0a0a  ...#### app.py..
+000019b0: 6060 6070 7974 686f 6e0a 6672 6f6d 206f  ```python.from o
+000019c0: 726d 5f63 6f6e 6669 6720 696d 706f 7274  rm_config import
+000019d0: 2063 6f6e 6669 670a 6672 6f6d 206e 6573   config.from nes
+000019e0: 742e 636f 7265 2069 6d70 6f72 7420 4170  t.core import Ap
+000019f0: 700a 6672 6f6d 2073 7263 2e70 726f 6475  p.from src.produ
+00001a00: 6374 732e 7072 6f64 7563 7473 5f6d 6f64  cts.products_mod
+00001a10: 756c 6520 696d 706f 7274 2050 726f 6475  ule import Produ
+00001a20: 6374 734d 6f64 756c 650a 0a61 7070 203d  ctsModule..app =
+00001a30: 2041 7070 280a 2020 2020 6465 7363 7269   App(.    descri
+00001a40: 7074 696f 6e3d 2259 6f75 7220 6170 7020  ption="Your app 
+00001a50: 6465 7363 7269 7074 696f 6e22 2c0a 2020  description",.  
+00001a60: 2020 6d6f 6475 6c65 733d 5b0a 2020 2020    modules=[.    
+00001a70: 2020 2020 5072 6f64 7563 7473 4d6f 6475      ProductsModu
+00001a80: 6c65 0a20 2020 205d 2c0a 2020 2020 696e  le.    ],.    in
+00001a90: 6974 5f64 623d 636f 6e66 6967 2e63 7265  it_db=config.cre
+00001aa0: 6174 655f 616c 6c0a 290a 6060 600a 0a54  ate_all.).```..T
+00001ab0: 6869 7320 6973 2074 6865 2061 7070 2e70  his is the app.p
+00001ac0: 7920 6669 6c65 2c20 7768 6963 6820 6973  y file, which is
+00001ad0: 2074 6865 2065 6e74 7279 2070 6f69 6e74   the entry point
+00001ae0: 2066 6f72 2079 6f75 7220 6170 706c 6963   for your applic
+00001af0: 6174 696f 6e2e 2049 7420 696d 706f 7274  ation. It import
+00001b00: 7320 6e65 6365 7373 6172 7920 6d6f 6475  s necessary modu
+00001b10: 6c65 7320 616e 6420 7365 7473 2075 7020  les and sets up 
+00001b20: 7468 6520 4170 7020 6f62 6a65 6374 2077  the App object w
+00001b30: 6974 6820 6120 6465 7363 7269 7074 696f  ith a descriptio
+00001b40: 6e20 616e 6420 7468 6520 5072 6f64 7563  n and the Produc
+00001b50: 7473 4d6f 6475 6c65 2e0a 3c62 723e 0a49  tsModule..<br>.I
+00001b60: 7420 616c 736f 2069 6e69 7469 616c 697a  t also initializ
+00001b70: 6573 2074 6865 2064 6174 6162 6173 6520  es the database 
+00001b80: 7573 696e 6720 7468 6520 636f 6e66 6967  using the config
+00001b90: 2e63 7265 6174 655f 616c 6c20 6675 6e63  .create_all func
+00001ba0: 7469 6f6e 2e0a 0a23 2323 2320 6f72 6d5f  tion...#### orm_
+00001bb0: 636f 6e66 6967 2e70 790a 6060 6070 7974  config.py.```pyt
+00001bc0: 686f 6e0a 6672 6f6d 206e 6573 742e 636f  hon.from nest.co
+00001bd0: 7265 2069 6d70 6f72 7420 4f72 6d53 6572  re import OrmSer
+00001be0: 7669 6365 0a69 6d70 6f72 7420 6f73 0a66  vice.import os.f
+00001bf0: 726f 6d20 646f 7465 6e76 2069 6d70 6f72  rom dotenv impor
+00001c00: 7420 6c6f 6164 5f64 6f74 656e 760a 0a6c  t load_dotenv..l
+00001c10: 6f61 645f 646f 7465 6e76 2829 0a0a 636f  oad_dotenv()..co
+00001c20: 6e66 6967 203d 204f 726d 5365 7276 6963  nfig = OrmServic
+00001c30: 6528 0a20 2020 2064 625f 7479 7065 3d22  e(.    db_type="
+00001c40: 796f 7572 5f64 625f 7479 7065 222c 0a20  your_db_type",. 
+00001c50: 2020 2063 6f6e 6669 675f 7061 7261 6d73     config_params
+00001c60: 3d64 6963 7428 0a20 2020 2020 2020 2075  =dict(.        u
+00001c70: 7365 723d 6f73 2e67 6574 656e 7628 2244  ser=os.getenv("D
+00001c80: 425f 5553 4552 2229 2c0a 2020 2020 2020  B_USER"),.      
+00001c90: 2020 7061 7373 776f 7264 3d6f 732e 6765    password=os.ge
+00001ca0: 7465 6e76 2822 4442 5f50 4153 5357 4f52  tenv("DB_PASSWOR
+00001cb0: 4422 292c 0a20 2020 2020 2020 2068 6f73  D"),.        hos
+00001cc0: 743d 6f73 2e67 6574 656e 7628 2244 425f  t=os.getenv("DB_
+00001cd0: 484f 5354 2229 2c0a 2020 2020 2020 2020  HOST"),.        
+00001ce0: 706f 7274 3d6f 732e 6765 7465 6e76 2822  port=os.getenv("
+00001cf0: 4442 5f50 4f52 5422 292c 0a20 2020 2020  DB_PORT"),.     
+00001d00: 2020 2064 6174 6162 6173 653d 6f73 2e67     database=os.g
+00001d10: 6574 656e 7628 2244 425f 4e41 4d45 2229  etenv("DB_NAME")
+00001d20: 2c0a 2020 2020 292c 0a29 0a60 6060 0a0a  ,.    ),.).```..
+00001d30: 5468 6973 2069 7320 7468 6520 6f72 6d5f  This is the orm_
+00001d40: 636f 6e66 6967 2e70 7920 6669 6c65 2c20  config.py file, 
+00001d50: 7768 6963 6820 636f 6e74 6169 6e73 2074  which contains t
+00001d60: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+00001d70: 2066 6f72 2079 6f75 7220 4f52 4d20 284f   for your ORM (O
+00001d80: 626a 6563 742d 5265 6c61 7469 6f6e 616c  bject-Relational
+00001d90: 204d 6170 7069 6e67 2920 7365 7276 6963   Mapping) servic
+00001da0: 652e 0a0a 4974 2069 6d70 6f72 7473 206e  e...It imports n
+00001db0: 6563 6573 7361 7279 206c 6962 7261 7269  ecessary librari
+00001dc0: 6573 2c20 6c6f 6164 7320 656e 7669 726f  es, loads enviro
+00001dd0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00001de0: 7573 696e 6720 646f 7465 6e76 2c20 616e  using dotenv, an
+00001df0: 6420 6372 6561 7465 7320 616e 204f 726d  d creates an Orm
+00001e00: 5365 7276 6963 6520 6f62 6a65 6374 2077  Service object w
+00001e10: 6974 6820 7468 6520 7370 6563 6966 6965  ith the specifie
+00001e20: 6420 6461 7461 6261 7365 2074 7970 6520  d database type 
+00001e30: 616e 6420 636f 6e66 6967 7572 6174 696f  and configuratio
+00001e40: 6e20 7061 7261 6d65 7465 7273 2e0a 0a2d  n parameters...-
+00001e50: 2d2d 0a0a 4f6e 6365 2077 6520 7365 7420  --..Once we set 
+00001e60: 7570 2074 6869 7320 3320 6669 6c65 732c  up this 3 files,
+00001e70: 2077 6520 6361 6e20 7374 6172 7420 6372   we can start cr
+00001e80: 6561 7469 6e67 206f 7572 206d 6f64 756c  eating our modul
+00001e90: 6573 2e20 6561 6368 206d 6f64 756c 6520  es. each module 
+00001ea0: 6973 2061 2066 6f6c 6465 7220 7769 7468  is a folder with
+00001eb0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00001ec0: 7472 7563 7475 7265 3a0a 0a60 6060 7465  tructure:..```te
+00001ed0: 7874 200a e294 9ce2 9480 e294 8020 7072  xt .......... pr
+00001ee0: 6f64 7563 7473 0ae2 9482 2020 2020 e294  oducts....    ..
+00001ef0: 9ce2 9480 e294 8020 5f5f 696e 6974 5f5f  ....... __init__
+00001f00: 2e70 790a e294 8220 2020 20e2 949c e294  .py....    .....
+00001f10: 80e2 9480 2070 726f 6475 6374 735f 636f  .... products_co
+00001f20: 6e74 726f 6c6c 6572 2e70 790a e294 8220  ntroller.py.... 
+00001f30: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
+00001f40: 6475 6374 735f 7365 7276 6963 652e 7079  ducts_service.py
+00001f50: 0ae2 9482 2020 2020 e294 9ce2 9480 e294  ....    ........
+00001f60: 8020 7072 6f64 7563 7473 5f6d 6f64 656c  . products_model
+00001f70: 2e70 790a 7c20 2020 20e2 949c e294 80e2  .py.|    .......
+00001f80: 9480 2070 726f 6475 6374 735f 656e 7469  .. products_enti
+00001f90: 7479 2e70 790a e294 8220 2020 20e2 949c  ty.py....    ...
+00001fa0: e294 80e2 9480 2070 726f 6475 6374 735f  ...... products_
+00001fb0: 6d6f 6475 6c65 2e70 790a 6060 600a 0a54  module.py.```..T
+00001fc0: 6869 7320 6973 2074 6865 2073 7472 7563  his is the struc
+00001fd0: 7475 7265 206f 6620 6120 6d6f 6475 6c65  ture of a module
+00001fe0: 2066 6f6c 6465 722e 2049 7420 696e 636c   folder. It incl
+00001ff0: 7564 6573 2061 6e20 5f5f 696e 6974 5f5f  udes an __init__
+00002000: 2e70 7920 6669 6c65 2074 6f20 6d61 6b65  .py file to make
+00002010: 2074 6865 2066 6f6c 6465 7220 6120 5079   the folder a Py
+00002020: 7468 6f6e 2070 6163 6b61 6765 2c0a 3c62  thon package,.<b
+00002030: 723e 0a41 7320 7765 6c6c 2061 7320 7370  r>.As well as sp
+00002040: 6563 6966 6963 2066 696c 6573 2066 6f72  ecific files for
+00002050: 2074 6865 206d 6f64 756c 6527 7320 636f   the module's co
+00002060: 6e74 726f 6c6c 6572 2c20 7365 7276 6963  ntroller, servic
+00002070: 652c 206d 6f64 656c 2c20 656e 7469 7479  e, model, entity
+00002080: 2c20 616e 6420 6d6f 6475 6c65 2063 6f6e  , and module con
+00002090: 6669 6775 7261 7469 6f6e 732e 0a0a 2323  figurations...##
+000020a0: 2323 2070 726f 6475 6374 735f 6d6f 6465  ## products_mode
+000020b0: 6c2e 7079 0a60 6060 7079 7468 6f6e 0a66  l.py.```python.f
+000020c0: 726f 6d20 7079 6461 6e74 6963 2069 6d70  rom pydantic imp
+000020d0: 6f72 7420 4261 7365 4d6f 6465 6c0a 0a0a  ort BaseModel...
+000020e0: 636c 6173 7320 5072 6f64 7563 7428 4261  class Product(Ba
+000020f0: 7365 4d6f 6465 6c29 3a0a 2020 2020 6e61  seModel):.    na
+00002100: 6d65 3a20 7374 720a 2020 2020 7072 6963  me: str.    pric
+00002110: 653a 2066 6c6f 6174 0a20 2020 2064 6573  e: float.    des
+00002120: 6372 6970 7469 6f6e 3a20 7374 720a 6060  cription: str.``
+00002130: 600a 0a54 6869 7320 6973 2074 6865 2070  `..This is the p
+00002140: 726f 6475 6374 735f 6d6f 6465 6c2e 7079  roducts_model.py
+00002150: 2066 696c 652c 2077 6869 6368 2064 6566   file, which def
+00002160: 696e 6573 2074 6865 2050 726f 6475 6374  ines the Product
+00002170: 206d 6f64 656c 2075 7369 6e67 2074 6865   model using the
+00002180: 2042 6173 654d 6f64 656c 2063 6c61 7373   BaseModel class
+00002190: 2066 726f 6d20 7468 6520 7079 6461 6e74   from the pydant
+000021a0: 6963 206c 6962 7261 7279 2e0a 3c62 723e  ic library..<br>
+000021b0: 0a54 6865 206d 6f64 656c 2072 6570 7265  .The model repre
+000021c0: 7365 6e74 7320 7468 6520 7374 7275 6374  sents the struct
+000021d0: 7572 6520 616e 6420 6174 7472 6962 7574  ure and attribut
+000021e0: 6573 206f 6620 6120 7072 6f64 7563 742e  es of a product.
+000021f0: 0a0a 2323 2323 2070 726f 6475 6374 735f  ..#### products_
+00002200: 656e 7469 7479 2e70 790a 0a60 6060 7079  entity.py..```py
+00002210: 7468 6f6e 0a66 726f 6d20 7371 6c61 6c63  thon.from sqlalc
+00002220: 6865 6d79 2069 6d70 6f72 7420 436f 6c75  hemy import Colu
+00002230: 6d6e 2c20 496e 7465 6765 722c 2053 7472  mn, Integer, Str
+00002240: 696e 672c 2046 6c6f 6174 0a66 726f 6d20  ing, Float.from 
+00002250: 6f72 6d5f 636f 6e66 6967 2069 6d70 6f72  orm_config impor
+00002260: 7420 636f 6e66 6967 0a0a 0a63 6c61 7373  t config...class
+00002270: 2050 726f 6475 6374 2863 6f6e 6669 672e   Product(config.
+00002280: 4261 7365 293a 0a20 2020 205f 5f74 6162  Base):.    __tab
+00002290: 6c65 6e61 6d65 5f5f 203d 2022 7072 6f64  lename__ = "prod
+000022a0: 7563 7473 220a 0a20 2020 2069 6420 3d20  ucts"..    id = 
+000022b0: 436f 6c75 6d6e 2849 6e74 6567 6572 2c20  Column(Integer, 
+000022c0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+000022d0: 2c20 696e 6465 783d 5472 7565 2c20 6175  , index=True, au
+000022e0: 746f 696e 6372 656d 656e 743d 5472 7565  toincrement=True
+000022f0: 290a 2020 2020 6e61 6d65 203d 2043 6f6c  ).    name = Col
+00002300: 756d 6e28 5374 7269 6e67 290a 2020 2020  umn(String).    
+00002310: 7072 6963 6520 3d20 436f 6c75 6d6e 2846  price = Column(F
+00002320: 6c6f 6174 290a 2020 2020 6465 7363 7269  loat).    descri
+00002330: 7074 696f 6e20 3d20 436f 6c75 6d6e 2853  ption = Column(S
+00002340: 7472 696e 6729 0a60 6060 0a0a 5468 6973  tring).```..This
+00002350: 2069 7320 7468 6520 7072 6f64 7563 7473   is the products
+00002360: 5f65 6e74 6974 792e 7079 2066 696c 652c  _entity.py file,
+00002370: 2077 6869 6368 2064 6566 696e 6573 2074   which defines t
+00002380: 6865 2050 726f 6475 6374 2065 6e74 6974  he Product entit
+00002390: 7920 7573 696e 6720 5351 4c41 6c63 6865  y using SQLAlche
+000023a0: 6d79 2e20 0a3c 6272 3e0a 4974 2069 6d70  my. .<br>.It imp
+000023b0: 6f72 7473 206e 6563 6573 7361 7279 206d  orts necessary m
+000023c0: 6f64 756c 6573 2061 6e64 2069 6e68 6572  odules and inher
+000023d0: 6974 7320 6672 6f6d 2074 6865 2063 6f6e  its from the con
+000023e0: 6669 672e 4261 7365 2063 6c61 7373 2e20  fig.Base class. 
+000023f0: 5468 6520 656e 7469 7479 2072 6570 7265  The entity repre
+00002400: 7365 6e74 7320 7468 6520 6461 7461 6261  sents the databa
+00002410: 7365 2074 6162 6c65 2066 6f72 2073 746f  se table for sto
+00002420: 7269 6e67 2070 726f 6475 6374 732c 2077  ring products, w
+00002430: 6974 6820 636f 6c75 6d6e 7320 666f 7220  ith columns for 
+00002440: 6964 2c20 6e61 6d65 2c20 7072 6963 652c  id, name, price,
+00002450: 2061 6e64 2064 6573 6372 6970 7469 6f6e   and description
+00002460: 2e0a 0a23 2323 2320 7072 6f64 7563 7473  ...#### products
+00002470: 5f73 6572 7669 6365 2e70 790a 0a60 6060  _service.py..```
+00002480: 7079 7468 6f6e 0a66 726f 6d20 7372 632e  python.from src.
+00002490: 7072 6f64 7563 7473 2e70 726f 6475 6374  products.product
+000024a0: 735f 6d6f 6465 6c20 696d 706f 7274 2050  s_model import P
+000024b0: 726f 6475 6374 0a66 726f 6d20 7372 632e  roduct.from src.
+000024c0: 7072 6f64 7563 7473 2e70 726f 6475 6374  products.product
+000024d0: 735f 656e 7469 7479 2069 6d70 6f72 7420  s_entity import 
+000024e0: 5072 6f64 7563 7420 6173 2050 726f 6475  Product as Produ
+000024f0: 6374 456e 7469 7479 0a66 726f 6d20 6f72  ctEntity.from or
+00002500: 6d5f 636f 6e66 6967 2069 6d70 6f72 7420  m_config import 
+00002510: 636f 6e66 6967 0a66 726f 6d20 6e65 7374  config.from nest
+00002520: 2e63 6f72 652e 6465 636f 7261 746f 7273  .core.decorators
+00002530: 2069 6d70 6f72 7420 6462 5f72 6571 7565   import db_reque
+00002540: 7374 5f68 616e 646c 6572 0a66 726f 6d20  st_handler.from 
+00002550: 6675 6e63 746f 6f6c 7320 696d 706f 7274  functools import
+00002560: 206c 7275 5f63 6163 6865 0a0a 0a40 6c72   lru_cache...@lr
+00002570: 755f 6361 6368 6528 290a 636c 6173 7320  u_cache().class 
+00002580: 5072 6f64 7563 7473 5365 7276 6963 653a  ProductsService:
+00002590: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000025a0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+000025b0: 2073 656c 662e 636f 6e66 6967 203d 2063   self.config = c
+000025c0: 6f6e 6669 670a 2020 2020 2020 2020 7365  onfig.        se
+000025d0: 6c66 2e73 6573 7369 6f6e 203d 2073 656c  lf.session = sel
+000025e0: 662e 636f 6e66 6967 2e67 6574 5f64 6228  f.config.get_db(
+000025f0: 290a 0a20 2020 2040 6462 5f72 6571 7565  )..    @db_reque
+00002600: 7374 5f68 616e 646c 6572 0a20 2020 2064  st_handler.    d
+00002610: 6566 2061 6464 5f70 726f 6475 6374 2873  ef add_product(s
+00002620: 656c 662c 2070 726f 6475 6374 3a20 5072  elf, product: Pr
+00002630: 6f64 7563 7429 3a0a 2020 2020 2020 2020  oduct):.        
+00002640: 7072 6f64 7563 745f 656e 7469 7479 203d  product_entity =
+00002650: 2050 726f 6475 6374 456e 7469 7479 280a   ProductEntity(.
+00002660: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00002670: 3d70 726f 6475 6374 2e6e 616d 652c 0a20  =product.name,. 
+00002680: 2020 2020 2020 2020 2020 2070 7269 6365             price
+00002690: 3d70 726f 6475 6374 2e70 7269 6365 2c0a  =product.price,.
+000026a0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000026b0: 7269 7074 696f 6e3d 7072 6f64 7563 742e  ription=product.
+000026c0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
+000026d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000026e0: 6c66 2e73 6573 7369 6f6e 2e61 6464 2870  lf.session.add(p
+000026f0: 726f 6475 6374 5f65 6e74 6974 7929 0a20  roduct_entity). 
+00002700: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+00002710: 696f 6e2e 636f 6d6d 6974 2829 0a20 2020  ion.commit().   
+00002720: 2020 2020 2072 6574 7572 6e20 7072 6f64       return prod
+00002730: 7563 745f 656e 7469 7479 2e69 640a 0a20  uct_entity.id.. 
+00002740: 2020 2040 6462 5f72 6571 7565 7374 5f68     @db_request_h
+00002750: 616e 646c 6572 0a20 2020 2064 6566 2067  andler.    def g
+00002760: 6574 5f70 726f 6475 6374 7328 7365 6c66  et_products(self
+00002770: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002780: 6e20 7365 6c66 2e73 6573 7369 6f6e 2e71  n self.session.q
+00002790: 7565 7279 2850 726f 6475 6374 456e 7469  uery(ProductEnti
+000027a0: 7479 292e 616c 6c28 290a 0a20 2020 2040  ty).all()..    @
+000027b0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
+000027c0: 6572 0a20 2020 2064 6566 2067 6574 5f70  er.    def get_p
+000027d0: 726f 6475 6374 2873 656c 662c 2070 726f  roduct(self, pro
+000027e0: 6475 6374 5f69 643a 2069 6e74 293a 0a20  duct_id: int):. 
+000027f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00002800: 6c66 2e73 6573 7369 6f6e 2e71 7565 7279  lf.session.query
+00002810: 2850 726f 6475 6374 456e 7469 7479 292e  (ProductEntity).
+00002820: 6669 6c74 6572 2850 726f 6475 6374 456e  filter(ProductEn
+00002830: 7469 7479 2e69 6420 3d3d 2070 726f 6475  tity.id == produ
+00002840: 6374 5f69 6429 2e66 6972 7374 2829 0a0a  ct_id).first()..
+00002850: 2020 2020 4064 625f 7265 7175 6573 745f      @db_request_
+00002860: 6861 6e64 6c65 720a 2020 2020 6465 6620  handler.    def 
+00002870: 6c61 7374 5f70 726f 6475 6374 2873 656c  last_product(sel
+00002880: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00002890: 726e 2073 656c 662e 7365 7373 696f 6e2e  rn self.session.
+000028a0: 7175 6572 7928 5072 6f64 7563 7445 6e74  query(ProductEnt
+000028b0: 6974 7929 2e6f 7264 6572 5f62 7928 5072  ity).order_by(Pr
+000028c0: 6f64 7563 7445 6e74 6974 792e 6964 2e64  oductEntity.id.d
+000028d0: 6573 6328 2929 2e66 6972 7374 2829 0a60  esc()).first().`
+000028e0: 6060 0a0a 5468 6973 2069 7320 7468 6520  ``..This is the 
+000028f0: 7365 7276 6963 6520 6669 6c65 2c20 7768  service file, wh
+00002900: 6963 6820 636f 6e74 6169 6e73 2074 6865  ich contains the
+00002910: 2050 726f 6475 6374 7353 6572 7669 6365   ProductsService
+00002920: 2063 6c61 7373 2e20 4974 2069 6d70 6f72   class. It impor
+00002930: 7473 206e 6563 6573 7361 7279 206d 6f64  ts necessary mod
+00002940: 756c 6573 2061 6e64 2064 6566 696e 6573  ules and defines
+00002950: 206d 6574 686f 6473 2066 6f72 2069 6e74   methods for int
+00002960: 6572 6163 7469 6e67 2077 6974 6820 7468  eracting with th
+00002970: 6520 6461 7461 6261 7365 2e20 0a3c 6272  e database. .<br
+00002980: 3e0a 5468 6520 6d65 7468 6f64 7320 696e  >.The methods in
+00002990: 636c 7564 6520 6164 6469 6e67 2061 2070  clude adding a p
+000029a0: 726f 6475 6374 2c20 6765 7474 696e 6720  roduct, getting 
+000029b0: 616c 6c20 7072 6f64 7563 7473 2c20 6765  all products, ge
+000029c0: 7474 696e 6720 6120 7370 6563 6966 6963  tting a specific
+000029d0: 2070 726f 6475 6374 2062 7920 4944 2c20   product by ID, 
+000029e0: 616e 6420 7265 7472 6965 7669 6e67 2074  and retrieving t
+000029f0: 6865 206c 6173 7420 6164 6465 6420 7072  he last added pr
+00002a00: 6f64 7563 742e 0a3c 6272 3e0a 5468 6520  oduct..<br>.The 
+00002a10: 6040 6462 5f72 6571 7565 7374 5f68 616e  `@db_request_han
+00002a20: 646c 6572 6020 6465 636f 7261 746f 7220  dler` decorator 
+00002a30: 6973 2072 6573 706f 6e73 6962 6c65 2066  is responsible f
+00002a40: 6f72 206d 616e 6167 696e 6720 7468 6520  or managing the 
+00002a50: 6461 7461 6261 7365 2073 6573 7369 6f6e  database session
+00002a60: 2061 6e64 2068 616e 646c 696e 6720 616e   and handling an
+00002a70: 7920 6578 6365 7074 696f 6e73 2074 6861  y exceptions tha
+00002a80: 7420 6d61 7920 6f63 6375 7220 6475 7269  t may occur duri
+00002a90: 6e67 2064 6174 6162 6173 6520 6f70 6572  ng database oper
+00002aa0: 6174 696f 6e73 2e0a 0a0a 2323 2323 2070  ations....#### p
+00002ab0: 726f 6475 6374 735f 636f 6e74 726f 6c6c  roducts_controll
+00002ac0: 6572 2e70 790a 0a60 6060 7079 7468 6f6e  er.py..```python
+00002ad0: 0a66 726f 6d20 6e65 7374 2e63 6f72 6520  .from nest.core 
+00002ae0: 696d 706f 7274 2044 6570 656e 6473 2c20  import Depends, 
+00002af0: 436f 6e74 726f 6c6c 6572 2c20 4765 742c  Controller, Get,
+00002b00: 2050 6f73 740a 6672 6f6d 2073 7263 2e70   Post.from src.p
+00002b10: 726f 6475 6374 732e 7072 6f64 7563 7473  roducts.products
+00002b20: 5f73 6572 7669 6365 2069 6d70 6f72 7420  _service import 
+00002b30: 5072 6f64 7563 7473 5365 7276 6963 650a  ProductsService.
+00002b40: 6672 6f6d 2073 7263 2e70 726f 6475 6374  from src.product
+00002b50: 732e 7072 6f64 7563 7473 5f6d 6f64 656c  s.products_model
+00002b60: 2069 6d70 6f72 7420 5072 6f64 7563 740a   import Product.
+00002b70: 0a0a 4043 6f6e 7472 6f6c 6c65 7228 2270  ..@Controller("p
+00002b80: 726f 6475 6374 7322 290a 636c 6173 7320  roducts").class 
+00002b90: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
+00002ba0: 6572 3a0a 2020 2020 7365 7276 6963 653a  er:.    service:
+00002bb0: 2050 726f 6475 6374 7353 6572 7669 6365   ProductsService
+00002bc0: 203d 2044 6570 656e 6473 2850 726f 6475   = Depends(Produ
+00002bd0: 6374 7353 6572 7669 6365 290a 0a20 2020  ctsService)..   
+00002be0: 2040 4765 7428 222f 6765 745f 7072 6f64   @Get("/get_prod
+00002bf0: 7563 7473 2229 0a20 2020 2064 6566 2067  ucts").    def g
+00002c00: 6574 5f70 726f 6475 6374 7328 7365 6c66  et_products(self
+00002c10: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002c20: 6e20 7365 6c66 2e73 6572 7669 6365 2e67  n self.service.g
+00002c30: 6574 5f70 726f 6475 6374 7328 290a 0a20  et_products().. 
+00002c40: 2020 2040 4765 7428 222f 6765 745f 7072     @Get("/get_pr
+00002c50: 6f64 7563 742f 7b70 726f 6475 6374 5f69  oduct/{product_i
+00002c60: 647d 2229 0a20 2020 2064 6566 2067 6574  d}").    def get
+00002c70: 5f70 726f 6475 6374 2873 656c 662c 2070  _product(self, p
+00002c80: 726f 6475 6374 5f69 643a 2069 6e74 293a  roduct_id: int):
+00002c90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002ca0: 7365 6c66 2e73 6572 7669 6365 2e67 6574  self.service.get
+00002cb0: 5f70 726f 6475 6374 2870 726f 6475 6374  _product(product
+00002cc0: 5f69 6429 0a0a 2020 2020 4050 6f73 7428  _id)..    @Post(
+00002cd0: 222f 6164 645f 7072 6f64 7563 7422 290a  "/add_product").
+00002ce0: 2020 2020 6465 6620 6164 645f 7072 6f64      def add_prod
+00002cf0: 7563 7428 7365 6c66 2c20 7072 6f64 7563  uct(self, produc
+00002d00: 743a 2050 726f 6475 6374 293a 0a20 2020  t: Product):.   
+00002d10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002d20: 2e73 6572 7669 6365 2e61 6464 5f70 726f  .service.add_pro
+00002d30: 6475 6374 2870 726f 6475 6374 290a 0a20  duct(product).. 
+00002d40: 2020 2040 4765 7428 222f 6c61 7374 5f70     @Get("/last_p
+00002d50: 726f 6475 6374 2229 0a20 2020 2064 6566  roduct").    def
+00002d60: 206c 6173 745f 7072 6f64 7563 7428 7365   last_product(se
+00002d70: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00002d80: 7572 6e20 7365 6c66 2e73 6572 7669 6365  urn self.service
+00002d90: 2e6c 6173 745f 7072 6f64 7563 7428 290a  .last_product().
+00002da0: 6060 600a 496e 2073 756d 6d61 7279 2c20  ```.In summary, 
+00002db0: 7468 6520 6064 6563 6f72 6174 6f72 7360  the `decorators`
+00002dc0: 2061 6e64 2074 6865 2060 4465 7065 6e64   and the `Depend
+00002dd0: 7360 2063 6c61 7373 2061 7265 2075 7365  s` class are use
+00002de0: 6420 746f 2064 6566 696e 6520 726f 7574  d to define rout
+00002df0: 6573 2061 6e64 2048 5454 5020 6d65 7468  es and HTTP meth
+00002e00: 6f64 7320 666f 7220 7468 650a 3c62 723e  ods for the.<br>
+00002e10: 0a60 5072 6f64 7563 7473 436f 6e74 726f  .`ProductsContro
+00002e20: 6c6c 6572 6020 636c 6173 732c 2061 6e64  ller` class, and
+00002e30: 2074 6f20 696e 6a65 6374 2074 6865 2060   to inject the `
+00002e40: 5072 6f64 7563 7473 5365 7276 6963 6560  ProductsService`
+00002e50: 2064 6570 656e 6465 6e63 7920 696e 746f   dependency into
+00002e60: 2074 6865 2073 6572 7669 6365 2061 7474   the service att
+00002e70: 7269 6275 7465 206f 6620 7468 6520 636f  ribute of the co
+00002e80: 6e74 726f 6c6c 6572 2e0a 3c62 723e 0a54  ntroller..<br>.T
+00002e90: 6869 7320 616c 6c6f 7773 2074 6865 2063  his allows the c
+00002ea0: 6f6e 7472 6f6c 6c65 7220 746f 2068 616e  ontroller to han
+00002eb0: 646c 6520 696e 636f 6d69 6e67 2072 6571  dle incoming req
+00002ec0: 7565 7374 7320 616e 6420 696e 7465 7261  uests and intera
+00002ed0: 6374 2077 6974 680a 3c62 723e 0a54 6865  ct with.<br>.The
+00002ee0: 2073 6572 7669 6365 2074 6f20 7065 7266   service to perf
+00002ef0: 6f72 6d20 7370 6563 6966 6963 2061 6374  orm specific act
+00002f00: 696f 6e73 2062 6173 6564 206f 6e20 7468  ions based on th
+00002f10: 6520 726f 7574 6573 2061 6e64 206d 6574  e routes and met
+00002f20: 686f 6473 2064 6566 696e 6564 2e0a 0a0a  hods defined....
+00002f30: 2323 2323 2070 726f 6475 6374 735f 6d6f  #### products_mo
+00002f40: 6475 6c65 2e70 790a 0a60 6060 7079 7468  dule.py..```pyth
+00002f50: 6f6e 0a66 726f 6d20 7372 632e 7072 6f64  on.from src.prod
+00002f60: 7563 7473 2e70 726f 6475 6374 735f 636f  ucts.products_co
+00002f70: 6e74 726f 6c6c 6572 2069 6d70 6f72 7420  ntroller import 
+00002f80: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
+00002f90: 6572 0a66 726f 6d20 7372 632e 7072 6f64  er.from src.prod
+00002fa0: 7563 7473 2e70 726f 6475 6374 735f 7365  ucts.products_se
+00002fb0: 7276 6963 6520 696d 706f 7274 2050 726f  rvice import Pro
+00002fc0: 6475 6374 7353 6572 7669 6365 0a0a 0a63  ductsService...c
+00002fd0: 6c61 7373 2050 726f 6475 6374 734d 6f64  lass ProductsMod
+00002fe0: 756c 653a 0a0a 2020 2020 6465 6620 5f5f  ule:..    def __
+00002ff0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00003000: 2020 2020 2020 7365 6c66 2e70 726f 7669        self.provi
+00003010: 6465 7273 203d 205b 5072 6f64 7563 7473  ders = [Products
+00003020: 5365 7276 6963 655d 0a20 2020 2020 2020  Service].       
+00003030: 2073 656c 662e 636f 6e74 726f 6c6c 6572   self.controller
+00003040: 7320 3d20 5b50 726f 6475 6374 7343 6f6e  s = [ProductsCon
+00003050: 7472 6f6c 6c65 725d 0a60 6060 0a0a 5468  troller].```..Th
+00003060: 6973 206d 6f64 756c 6520 6361 6e20 6265  is module can be
+00003070: 2072 6567 6973 7465 7265 6420 616e 6420   registered and 
+00003080: 7573 6564 2069 6e20 796f 7572 2061 7070  used in your app
+00003090: 6c69 6361 7469 6f6e 2e20 4f6e 6365 2074  lication. Once t
+000030a0: 6865 206d 6f64 756c 6520 6973 2072 6567  he module is reg
+000030b0: 6973 7465 7265 642c 2074 6865 2063 6f6e  istered, the con
+000030c0: 7472 6f6c 6c65 7220 726f 7574 6573 2077  troller routes w
+000030d0: 696c 6c20 6265 2061 7661 696c 6162 6c65  ill be available
+000030e0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
+000030f0: 6420 7061 7468 2e0a 0a54 6869 7320 3520  d path...This 5 
+00003100: 636f 6d70 6f6e 656e 7473 2061 7265 2074  components are t
+00003110: 6865 206d 696e 696d 756d 2072 6571 7569  he minimum requi
+00003120: 7265 6420 746f 2063 7265 6174 6520 6120  red to create a 
+00003130: 6d6f 6475 6c65 2074 6861 7420 776f 726b  module that work
+00003140: 7320 7769 7468 2074 6865 204f 524d 2e0a  s with the ORM..
+00003150: 5468 6572 6520 6172 6520 6d61 6e79 206d  There are many m
+00003160: 6f72 6520 6f70 7469 6f6e 7320 6f66 2068  ore options of h
+00003170: 6f77 2079 6f75 2063 616e 2064 6573 6967  ow you can desig
+00003180: 6e20 796f 7572 206d 6f64 756c 6573 2061  n your modules a
+00003190: 6e64 2077 6869 6368 2064 6174 6162 6173  nd which databas
+000031a0: 6573 2079 6f75 2063 616e 2075 7365 2c20  es you can use, 
+000031b0: 6275 7420 7468 6973 2069 7320 7468 6520  but this is the 
+000031c0: 6465 6661 756c 7420 6261 7369 6320 7374  default basic st
+000031d0: 7275 6374 7572 652e 0a0a 2323 204b 6579  ructure...## Key
+000031e0: 2046 6561 7475 7265 730a 2323 2320 4d6f   Features.### Mo
+000031f0: 6475 6c61 7220 4172 6368 6974 6563 7475  dular Architectu
+00003200: 7265 0a0a 5079 4e65 7374 2066 6f6c 6c6f  re..PyNest follo
+00003210: 7773 2074 6865 206d 6f64 756c 6172 2061  ws the modular a
+00003220: 7263 6869 7465 6374 7572 6520 6f66 204e  rchitecture of N
+00003230: 6573 744a 532c 2077 6869 6368 2061 6c6c  estJS, which all
+00003240: 6f77 7320 666f 7220 6561 7379 2073 6570  ows for easy sep
+00003250: 6172 6174 696f 6e20 6f66 2063 6f6e 6365  aration of conce
+00003260: 726e 7320 616e 6420 636f 6465 206f 7267  rns and code org
+00003270: 616e 697a 6174 696f 6e2e 2045 6163 6820  anization. Each 
+00003280: 6d6f 6475 6c65 2063 6f6e 7461 696e 7320  module contains 
+00003290: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
+000032a0: 7265 6c61 7465 6420 636f 6e74 726f 6c6c  related controll
+000032b0: 6572 732c 2073 6572 7669 6365 732c 2061  ers, services, a
+000032c0: 6e64 2070 726f 7669 6465 7273 2e0a 0a23  nd providers...#
+000032d0: 2323 2044 6570 656e 6465 6e63 7920 496e  ## Dependency In
+000032e0: 6a65 6374 696f 6e0a 5079 4e65 7374 2073  jection.PyNest s
+000032f0: 7570 706f 7274 7320 6465 7065 6e64 656e  upports dependen
+00003300: 6379 2069 6e6a 6563 7469 6f6e 2c20 7768  cy injection, wh
+00003310: 6963 6820 6d61 6b65 7320 6974 2065 6173  ich makes it eas
+00003320: 7920 746f 206d 616e 6167 6520 6465 7065  y to manage depe
+00003330: 6e64 656e 6369 6573 2061 6e64 2077 7269  ndencies and wri
+00003340: 7465 2074 6573 7461 626c 6520 636f 6465  te testable code
+00003350: 2e20 596f 7520 6361 6e20 6561 7369 6c79  . You can easily
+00003360: 2069 6e6a 6563 7420 7365 7276 6963 6573   inject services
+00003370: 2061 6e64 2070 726f 7669 6465 7273 2069   and providers i
+00003380: 6e74 6f20 796f 7572 2063 6f6e 7472 6f6c  nto your control
+00003390: 6c65 7273 2075 7369 6e67 2064 6563 6f72  lers using decor
+000033a0: 6174 6f72 732e 0a0a 0a23 2323 2044 6563  ators....### Dec
+000033b0: 6f72 6174 6f72 730a 0a50 794e 6573 7420  orators..PyNest 
+000033c0: 6d61 6b65 7320 6578 7465 6e73 6976 6520  makes extensive 
+000033d0: 7573 6520 6f66 2064 6563 6f72 6174 6f72  use of decorator
+000033e0: 7320 746f 2064 6566 696e 6520 726f 7574  s to define rout
+000033f0: 6573 2c20 6d69 6464 6c65 7761 7265 2c20  es, middleware, 
+00003400: 616e 6420 6f74 6865 7220 6170 706c 6963  and other applic
+00003410: 6174 696f 6e20 636f 6d70 6f6e 656e 7473  ation components
+00003420: 2e20 5468 6973 2068 656c 7073 206b 6565  . This helps kee
+00003430: 7020 7468 6520 636f 6465 2063 6f6e 6369  p the code conci
+00003440: 7365 2061 6e64 2065 6173 7920 746f 2072  se and easy to r
+00003450: 6561 642e 0a0a 2323 2320 5479 7065 2041  ead...### Type A
+00003460: 6e6e 6f74 6174 696f 6e73 0a0a 5079 4e65  nnotations..PyNe
+00003470: 7374 206c 6576 6572 6167 6573 2050 7974  st leverages Pyt
+00003480: 686f 6e27 7320 7479 7065 2061 6e6e 6f74  hon's type annot
+00003490: 6174 696f 6e73 2074 6f20 7072 6f76 6964  ations to provid
+000034a0: 6520 6265 7474 6572 2074 6f6f 6c69 6e67  e better tooling
+000034b0: 2061 6e64 2068 656c 7020 7072 6576 656e   and help preven
+000034c0: 7420 6572 726f 7273 2e20 596f 7520 6361  t errors. You ca
+000034d0: 6e20 616e 6e6f 7461 7465 2079 6f75 7220  n annotate your 
+000034e0: 636f 6e74 726f 6c6c 6572 732c 2073 6572  controllers, ser
+000034f0: 7669 6365 732c 2061 6e64 2070 726f 7669  vices, and provi
+00003500: 6465 7273 2077 6974 6820 7479 7065 7320  ders with types 
+00003510: 746f 206d 616b 6520 796f 7572 2063 6f64  to make your cod
+00003520: 6520 6d6f 7265 2072 6f62 7573 742e 0a0a  e more robust...
+00003530: 2323 2320 436f 6465 2047 656e 6572 6174  ### Code Generat
+00003540: 696f 6e0a 0a50 794e 6573 7420 696e 636c  ion..PyNest incl
+00003550: 7564 6573 2061 2063 6f64 6520 6765 6e65  udes a code gene
+00003560: 7261 7469 6f6e 2074 6f6f 6c20 7468 6174  ration tool that
+00003570: 2063 616e 2063 7265 6174 6520 626f 696c   can create boil
+00003580: 6572 706c 6174 6520 636f 6465 2066 6f72  erplate code for
+00003590: 206d 6f64 756c 6573 2c20 636f 6e74 726f   modules, contro
+000035a0: 6c6c 6572 732c 2061 6e64 206f 7468 6572  llers, and other
+000035b0: 2063 6f6d 706f 6e65 6e74 732e 2054 6869   components. Thi
+000035c0: 7320 7361 7665 7320 796f 7520 7469 6d65  s saves you time
+000035d0: 2061 6e64 2068 656c 7073 2079 6f75 2066   and helps you f
+000035e0: 6f63 7573 206f 6e20 7772 6974 696e 6720  ocus on writing 
+000035f0: 7468 6520 636f 6465 2074 6861 7420 6d61  the code that ma
+00003600: 7474 6572 732e 0a0a 2323 2046 7574 7572  tters...## Futur
+00003610: 6520 506c 616e 730a 0a2d 205b 205d 2043  e Plans..- [ ] C
+00003620: 7265 6174 6520 4d61 726b 6574 706c 6163  reate Marketplac
+00003630: 6520 666f 7220 6d6f 6475 6c65 7320 7768  e for modules wh
+00003640: 6572 6520 6465 7665 6c6f 7065 7273 2063  ere developers c
+00003650: 616e 2073 6861 7265 2074 6865 6972 206d  an share their m
+00003660: 6f64 756c 6573 2061 6e64 2064 6f77 6e6c  odules and downl
+00003670: 6f61 6420 6d6f 6475 6c65 7320 6372 6561  oad modules crea
+00003680: 7465 6420 6279 206f 7468 6572 732e 0a2d  ted by others..-
+00003690: 205b 205d 2043 7265 7465 2041 6273 7472   [ ] Crete Abstr
+000036a0: 6163 7469 6f6e 2063 6c61 7373 2074 6f20  action class to 
+000036b0: 4d6f 6475 6c65 7320 616e 6420 5365 7276  Modules and Serv
+000036c0: 6963 6573 2074 6f20 616c 6c6f 7720 666f  ices to allow fo
+000036d0: 7220 6561 7379 2063 7265 6174 696f 6e20  r easy creation 
+000036e0: 6f66 206d 6f64 756c 6573 2061 6e64 2073  of modules and s
+000036f0: 6572 7669 6365 732e 0a2d 205b 205d 2041  ervices..- [ ] A
+00003700: 6464 2069 6e68 6572 6974 616e 6365 2062  dd inheritance b
+00003710: 6574 7765 656e 2063 6f6e 7472 6f6c 6c65  etween controlle
+00003720: 7273 2066 6f72 2063 7265 6174 696e 6720  rs for creating 
+00003730: 6d6f 7265 2063 6f6d 706c 6578 2063 6f6e  more complex con
+00003740: 7472 6f6c 6c65 7273 2e0a 2d20 5b20 5d20  trollers..- [ ] 
+00003750: 4164 6420 7375 7070 6f72 7420 666f 7220  Add support for 
+00003760: 6f74 6865 7220 6461 7461 6261 7365 7320  other databases 
+00003770: 286d 6f6e 676f 4442 2c20 7265 6469 732c  (mongoDB, redis,
+00003780: 2065 7463 2e29 0a2d 205b 205d 2043 7265   etc.).- [ ] Cre
+00003790: 6174 6520 6f75 742d 6f66 2d74 6865 2d62  ate out-of-the-b
+000037a0: 6f78 2061 7574 6865 6e74 6963 6174 696f  ox authenticatio
+000037b0: 6e20 6d6f 6475 6c65 2074 6861 7420 6361  n module that ca
+000037c0: 6e20 6265 2065 6173 696c 7920 696e 7465  n be easily inte
+000037d0: 6772 6174 6564 2069 6e74 6f20 616e 7920  grated into any 
+000037e0: 6170 706c 6963 6174 696f 6e2e 0a2d 205b  application..- [
+000037f0: 205d 2041 6464 2073 7570 706f 7274 2066   ] Add support f
+00003800: 6f72 206f 7468 6572 2074 6573 7469 6e67  or other testing
+00003810: 2066 7261 6d65 776f 726b 7320 616e 6420   frameworks and 
+00003820: 6372 6561 7465 2074 6573 7469 6e67 2074  create testing t
+00003830: 656d 706c 6174 6573 2e0a 2d20 5b20 5d20  emplates..- [ ] 
+00003840: 4164 6420 7375 7070 6f72 7420 666f 7220  Add support for 
+00003850: 6f74 6865 7220 7765 6220 6672 616d 6577  other web framew
+00003860: 6f72 6b73 2028 466c 6173 6b2c 2044 6a61  orks (Flask, Dja
+00003870: 6e67 6f2c 2065 7463 2e29 202d 2053 616d  ngo, etc.) - Sam
+00003880: 6520 4172 6368 6974 6563 7475 7265 2c20  e Architecture, 
+00003890: 6469 6666 6572 656e 7420 656e 6769 6e65  different engine
+000038a0: 2e0a 0a0a 2323 2043 6f6e 7472 6962 7574  ....## Contribut
+000038b0: 696e 670a 0a43 6f6e 7472 6962 7574 696f  ing..Contributio
+000038c0: 6e73 2061 7265 2077 656c 636f 6d65 2120  ns are welcome! 
+000038d0: 506c 6561 7365 2066 6565 6c20 6672 6565  Please feel free
+000038e0: 2074 6f20 6772 6162 206f 6e65 206f 6620   to grab one of 
+000038f0: 7468 6520 6f70 656e 2069 7373 7565 732c  the open issues,
+00003900: 0a6f 7220 6f70 656e 2061 206e 6577 206f  .or open a new o
+00003910: 6e65 2069 6620 796f 7520 6861 7665 2061  ne if you have a
+00003920: 6e20 6964 6561 2066 6f72 2061 206e 6577  n idea for a new
+00003930: 2066 6561 7475 7265 206f 7220 696d 7072   feature or impr
+00003940: 6f76 656d 656e 742e 0a0a 5468 6973 2077  ovement...This w
+00003950: 6f75 6c64 2062 7269 6e67 2061 2068 7567  ould bring a hug
+00003960: 6520 696d 7061 6374 2074 6f20 7468 6520  e impact to the 
+00003970: 7072 6f6a 6563 7420 616e 6420 7468 6520  project and the 
+00003980: 636f 6d6d 756e 6974 792e 0a0a 2323 204c  community...## L
+00003990: 6963 656e 7365 0a0a 5079 4e65 7374 2069  icense..PyNest i
+000039a0: 7320 5b4d 4954 206c 6963 656e 7365 645d  s [MIT licensed]
+000039b0: 284c 4943 454e 5345 292e 0a0a 2323 2043  (LICENSE)...## C
+000039c0: 7265 6469 7473 0a0a 5079 4e65 7374 2069  redits..PyNest i
+000039d0: 7320 696e 7370 6972 6564 2062 7920 5b4e  s inspired by [N
+000039e0: 6573 744a 535d 2868 7474 7073 3a2f 2f6e  estJS](https://n
+000039f0: 6573 746a 732e 636f 6d2f 292e 0a         estjs.com/)..
```

### Comparing `pynest-api-0.0.3/README.md` & `pynest-api-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 <p align="center">
   <img src="docs/imgs/pynest_logo-modified.png" title="pynest logo" width="200">
 </p>
 <p align="center">
     <em>PyNest is a Python framework built on top of FastAPI that follows the modular architecture of NestJS</em>
 </p>
 <p align="center">
-<a href="https://pypi.org/project/pynest-api" target="_blank">
-    <img src="https://img.shields.io/pypi/v/pynest-api?color=%2334D058&label=pypi%20package" alt="Package version">
-</a>
-<a href="https://pypi.org/project/pynest-api" target="_blank">
-    <img src="https://img.shields.io/pypi/pyversions/pynest-api.svg?color=%2334D058" alt="Supported Python versions">
-</a>
+    <a href="https://pypi.org/project/pynest-api">
+        <img src="https://img.shields.io/pypi/v/pynest-api?color=%2334D058&label=pypi%20package" alt="Version">
+    </a>
+    <a href="https://pypi.org/project/pynest-api">
+        <img src="https://img.shields.io/pypi/pyversions/pynest-api.svg?color=%2334D058" alt="Python">
+    </a>
+    <a href="https://pepy.tech/project/pynest-api">
+        <img src="https://static.pepy.tech/personalized-badge/pynest-api?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads" alt="Downloads">
+    </a>
+    <a href="https://github.com/PythonNest/PyNest/blob/main/LICENSE">
+        <img src="https://img.shields.io/github/license/PythonNest/Pynest" alt="License">
+    </a>
 </p>
 
-# PyNest - Description
+
+# Description
 
 PyNest is designed to help structure your APIs in an intuitive, easy to understand, and enjoyable way.
 
 With PyNest, you can build scalable and maintainable APIs with ease. The framework supports dependency injection, type annotations, decorators, and code generation, making it easy to write clean and testable code.
 
 This framework is not a direct port of NestJS to Python but rather a re-imagining of the framework specifically for Python developers, including data scientists, data analysts, and data engineers. It aims to assist them in building better and faster APIs for their data applications.
 
@@ -235,16 +242,18 @@
 #### products_service.py
 
 ```python
 from src.products.products_model import Product
 from src.products.products_entity import Product as ProductEntity
 from orm_config import config
 from nest.core.decorators import db_request_handler
+from functools import lru_cache
 
 
+@lru_cache()
 class ProductsService:
     def __init__(self):
         self.config = config
         self.session = self.config.get_db()
 
     @db_request_handler
     def add_product(self, product: Product):
```

### Comparing `pynest-api-0.0.3/nest/cli/cli.py` & `pynest-api-0.1.0/nest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.3/nest/cli/click_handlers.py` & `pynest-api-0.1.0/nest/cli/click_handlers.py`

 * *Files 19% similar despite different names*

```diff
@@ -98,25 +98,25 @@
     Returns:
         None
     """
     requirements_template = generate_requirements()
     create_file(path, requirements_template)
 
 
-def create_app(path: Path) -> None:
+def create_app(path: Path, db_type) -> None:
     """
     Create an app.py file at the specified path using a template.
 
     Args:
         path (Path): The path to the app.py file.
 
     Returns:
         None
     """
-    app_template = generate_app()
+    app_template = generate_app(db_type)
     create_file(path, app_template)
 
 
 def create_orm_config(path: Path, db_type: str) -> None:
     """
     Create an orm_config.py file at the specified path using a template.
 
@@ -127,41 +127,42 @@
     Returns:
         None
     """
     orm_config_template = generate_orm_config(db_type)
     create_file(path, orm_config_template)
 
 
-def create_controller(path: Path, name: str) -> None:
+def create_controller(path: Path, name: str, db_type: str) -> None:
     """
     Create a controller file at the specified path using a template.
 
     Args:
         path (Path): The path to the controller file.
         name (str): The name of the controller.
 
     Returns:
         None
     """
-    controller_template = generate_controller(name)
+    controller_template = generate_controller(name, db_type)
     create_file(path, controller_template)
 
 
-def create_service(path: Path, name: str) -> None:
+def create_service(path: Path, name: str, db_type: str) -> None:
     """
     Create a service file at the specified path using a template.
 
     Args:
         path (Path): The path to the service file.
         name (str): The name of the service.
+        db_type (str): The type of the database.
 
     Returns:
         None
     """
-    service_template = generate_service(name)
+    service_template = generate_service(name, db_type)
     create_file(path, service_template)
 
 
 def create_module(path: Path, name: str) -> None:
     """
     Create a module file at the specified path using a template.
 
@@ -172,26 +173,26 @@
     Returns:
         None
     """
     module_template = generate_module(name)
     create_file(path, module_template)
 
 
-def create_entity(path: Path, name: str) -> None:
+def create_entity(path: Path, name: str, db_type: str) -> None:
     """
     Create an entity file at the specified path using a template.
 
     Args:
         path (Path): The path to the entity file.
         name (str): The name of the entity.
 
     Returns:
         None
     """
-    entity_template = generate_entity(name)
+    entity_template = generate_entity(name, db_type)
     create_file(path, entity_template)
 
 
 def create_dockerfile(path: Path) -> None:
     """
     Create a Dockerfile file at the specified path using a template.
 
@@ -203,24 +204,26 @@
     """
     dockerfile_template = generate_dockerfile()
     create_file(path, dockerfile_template)
 
 
 def install_requirements(path: Path, db_type: str) -> None:
     os.chdir(path)
-    subprocess.run("python -m venv venv && source venv/bin/activate", shell=True)
-    subprocess.run(["python", "-m", "pip", "install", "--upgrade", "pip"])
-    subprocess.run(["pip", "install", "-r", "requirements.txt"])
+    # subprocess.run("python -m venv venv && source venv/bin/activate", shell=True)
+    # subprocess.run(["python", "-m", "pip", "install", "--upgrade", "pip"])
+    # subprocess.run(["pip", "install", "-r", "requirements.txt"])
     if db_type == "mysql":
         subprocess.run(["pip", "install", "mysql-connector-python==8.0.33"])
     elif db_type == "postgresql":
         subprocess.run(["pip", "install", "psycopg2-binary==2.9.6"])
         print(
             "You need to install postgresql in your system\nfor production use only psycopg2"
         )
+    elif db_type == "mongodb":
+        subprocess.run(["pip", "install", "motor", "beanie"])
 
 
 def create_nest_app(name: str, db_type: str = "sqlite"):
     """
     Create a new nest app
 
     :param name: The name of the app
@@ -244,19 +247,20 @@
     │    ├──  ├── examples_entity.py
     │    ├──  ├── examples_module.py
 
         .....................
 
     │    ├── another module
     """
+
     path = Path(os.getcwd())
     root_path = path / name
     create_folder(path / name)
     print("Start creating nest app ...")
-    create_app(root_path / "app.py")
+    create_app(root_path / "app.py", db_type)
     print("app.py created successfully")
     create_orm_config(root_path / "orm_config.py", db_type)
     print("orm_config.py created successfully")
     create_main(root_path / "main.py")
     print("main.py created successfully")
     create_requirements(root_path / "requirements.txt")
     print("requirements.txt created successfully")
@@ -270,27 +274,28 @@
     create_folder(src_path)
     create_file(src_path / "__init__.py", "")
 
     print("creating examples module folder ... ")
     examples_path = src_path / "examples"
     create_folder(examples_path)
     create_file(examples_path / "__init__.py", "")
-    create_controller(examples_path / "examples_controller.py", "examples")
+    create_controller(examples_path / "examples_controller.py", "examples", db_type)
     print("controller created successfully")
-    create_service(examples_path / "examples_service.py", "examples")
+    create_service(examples_path / "examples_service.py", "examples", db_type)
     print("service created successfully")
     create_models(examples_path / "examples_model.py", "examples")
     print("model created successfully")
-    create_entity(examples_path / "examples_entity.py", "examples")
+    create_entity(examples_path / "examples_entity.py", "examples", db_type)
     print("entity created successfully")
     create_module(examples_path / "examples_module.py", "examples")
     print("module created successfully")
     if db_type == "sqlite":
         create_dockerfile(root_path / "Dockerfile")
         print("Dockerfile created successfully")
+    install_requirements(root_path, db_type)
 
     time.sleep(1)
     print("Project created successfully")
 
 
 def find_target_folder(path, target="src"):
     """
@@ -323,76 +328,163 @@
             if dir == target:
                 return os.path.join(root, dir)
 
     # If target folder is not found, return None
     return None
 
 
-def append_module_to_app(path_to_app_py: Path, new_module: str):
-    """
-    Append a module import statement to the app.py file.
+def get_import_string(path_to_file: Path, new_module: str, db_type: str):
+    split_new_module = new_module.split("_")
+    capitalized_new_module = "".join([word.capitalize() for word in split_new_module])
 
-    Args:
-        path_to_app_py (Path): The path to the app.py file.
-        new_module (str): The name of the new module to import.
+    if path_to_file.name == "app.py":
+        new_import = f"from src.{new_module}.{new_module}_module import {capitalized_new_module}Module\n"
+    elif path_to_file.name == "orm_config.py":
+        new_import = f"from src.{new_module}.{new_module}_entity import {capitalized_new_module}\n"
+    else:
+        raise ValueError(f"File {path_to_file} is not supported")
 
-    Raises:
-        FileNotFoundError: If the app.py file does not exist.
+    return new_import, capitalized_new_module
 
-    Returns:
-        None
-    """
+
+def append_import(path_to_app_py: Path, new_module: str, db_type: str):
     if not os.path.exists(path_to_app_py):
         raise FileNotFoundError(f"File {path_to_app_py} not found")
     with open(path_to_app_py, "r") as file:
         lines = file.readlines()
 
-    imports_end_index = [i for i, line in enumerate(lines) if "import" in line][-1]
+    new_module_import, capitalized_new_module = get_import_string(path_to_app_py, new_module, db_type)
 
-    split_new_module = new_module.split("_")
-    capitalized_new_module = "".join([word.capitalize() for word in split_new_module])
-
-    new_module_import = f"from src.{new_module}.{new_module}_module import {capitalized_new_module}Module\n"
+    imports_end_index = [i for i, line in enumerate(lines) if " import " in line][-1]
 
     lines = (
             lines[: imports_end_index + 1]
             + [new_module_import]
             + lines[imports_end_index + 1:]
     )
 
-    # Find the line index where the modules list starts
-    modules_start_index = next(
-        (i for i, line in enumerate(lines) if "modules=[" in line),
-        len(lines) - 1,  # If modules list not found, append the new module at the end
-    )
+    return lines, capitalized_new_module
 
-    # Find the line index where the modules list ends
+
+def get_module_end_index(lines, modules_start_index):
     modules_end_index = next(
         (
             i
             for i, line in enumerate(
             lines[modules_start_index:], start=modules_start_index
         )
             if "]" in line
         ),
         len(lines)
         - 1,  # If closing bracket not found, append the new module at the end
     )
+    return modules_end_index
+
+
+def append_module_to_app(path_to_app_py: Path, new_module: str, db_type: str):
+    """
+    Append a module import statement to the app.py file.
+
+    Args:
+        path_to_app_py (Path): The path to the app.py file.
+        new_module (str): The name of the new module to import.
+        db_type (str): The type of database to use.
+
+    return new_import, capitalized_new_module
+
+    Returns:
+        None
+    """
+    split_new_module = new_module.split("_")
+    capitalized_new_module = "".join([word.capitalize() for word in split_new_module])
+
+    lines, _ = append_import(path_to_app_py, new_module, db_type)
+    # Find the line index where the modules list starts
+    modules_start_index = next(
+        (i for i, line in enumerate(lines) if "modules=[" in line),
+        len(lines) - 1,  # If modules list not found, append the new module at the end
+    )
+    return modules_end_index
+
+
+def append_module_to_app(path_to_app_py: Path, new_module: str, db_type: str):
+    """
+    Append a module import statement to the app.py file.
+
+    Args:
+        path_to_app_py (Path): The path to the app.py file.
+        new_module (str): The name of the new module to import.
+        db_type (str): The type of database to use.
+
+    Raises:
+        FileNotFoundError: If the app.py file does not exist.
+
+    Returns:
+        None
+    """
+    split_new_module = new_module.split("_")
+    capitalized_new_module = "".join([word.capitalize() for word in split_new_module])
+
+    lines, _ = append_import(path_to_app_py, new_module, db_type)
+    # Find the line index where the modules list starts
+    modules_start_index = next(
+        (i for i, line in enumerate(lines) if "modules=[" in line),
+        len(lines) - 1,  # If modules list not found, append the new module at the end
+    )
+
+    # Find the line index where the modules list ends
+    modules_end_index = get_module_end_index(lines, modules_start_index)
+
+    # Find the line index where the modules list ends
+    modules_end_index = get_module_end_index(lines, modules_start_index)
 
     # Insert the new module before the closing bracket or at the end of the file
     new_lines = (
             lines[:modules_end_index]
             + [f"        {capitalized_new_module}Module,\n"]
             + lines[modules_end_index:]
     )
 
     with open(path_to_app_py, "w") as file:
         file.writelines(new_lines)
 
 
+def get_db_type(config_file: Path):
+    with open(config_file, "r") as file:
+        lines = file.readlines()
+    for line in lines:
+        if "db_type" in line:
+            return line.split("=")[1].strip().replace('"', "").replace(",", "")
+    raise Exception("db_type not found in orm_config.py")
+
+
+def add_document_to_odm_config(config_file: Path, new_module: str, db_type: str):
+    split_new_module = new_module.split("_")
+    capitalized_new_module = "".join([word.capitalize() for word in split_new_module])
+
+    lines, _ = append_import(config_file, new_module, db_type)
+    modules_start_index = next(
+        (i for i, line in enumerate(lines) if "document_models=[" in line),
+        len(lines) - 1,  # If modules list not found, append the new module at the end
+    )
+
+    modules_end_index = get_module_end_index(lines, modules_start_index)
+    if modules_end_index - modules_start_index == 0:
+        lines[modules_start_index] = lines[modules_start_index].split("[")[0] + f"[{capitalized_new_module}, " + lines[modules_end_index].split("[")[1]
+    else:
+        lines = (
+                lines[:modules_end_index]
+                + [f"        {capitalized_new_module}Module,\n"]
+                + lines[modules_end_index:]
+        )
+
+    with open(config_file, "w") as file:
+        file.writelines(lines)
+
+
 def create_nest_module(name: str):
     """
     Create a new nest module
 
     :param name: The name of the module
 
     The files structure are:
@@ -401,21 +493,30 @@
     ├── module_name_controller.py
     ├── module_name_service.py
     ├── module_name_model.py
     ├── module_name_entity.py
     ├── module_name_module.py
     """
     src_path = Path(find_target_folder(os.getcwd(), "src"))
+
+    if name in [x.name for x in src_path.iterdir()]:
+        raise Exception(f"module {name} already exists")
     if not src_path:
         raise Exception("src folder not found")
 
+    config_file = src_path.parent / "orm_config.py"
+    if not config_file.exists():
+        raise Exception("orm_config.py file not found")
+    db_type = get_db_type(config_file)
+    if db_type == "mongodb":
+        add_document_to_odm_config(config_file, name, db_type)
     module_path = src_path / name
     create_folder(module_path)
     create_file(module_path / "__init__.py", "")
-    create_controller(module_path / f"{name}_controller.py", name)
-    create_service(module_path / f"{name}_service.py", name)
+    create_controller(module_path / f"{name}_controller.py", name, db_type)
+    create_service(module_path / f"{name}_service.py", name, db_type)
     create_models(module_path / f"{name}_model.py", name)
-    create_entity(module_path / f"{name}_entity.py", name)
+    create_entity(module_path / f"{name}_entity.py", name, db_type)
     create_module(module_path / f"{name}_module.py", name)
-    append_module_to_app(src_path.parent / "app.py", name)
+    append_module_to_app(src_path.parent / "app.py", name, db_type)
 
     print(f"Module {name} created successfully!")
```

### Comparing `pynest-api-0.0.3/nest/common/templates/module.py` & `pynest-api-0.1.0/nest/common/templates/module.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.3/nest/common/templates/orm_config.py` & `pynest-api-0.1.0/nest/common/templates/orm_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 def generate_orm_config(db_type: str):
-    base_template = """from nest.core.database.base_orm import OrmService
+    if db_type == "mongodb":
+        service_import = "from nest.core.database.base_odm import OdmService\n" \
+                         "from src.examples.examples_entity import Examples"
+    else:
+        service_import = "from nest.core.database.base_orm import OrmService"
+
+    base_template = f"""{service_import}
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
     """
 
     if db_type == "sqlite":
@@ -37,9 +43,24 @@
         db_name=os.getenv("MYSQL_DB_NAME"),
         user=os.getenv("MYSQL_USER"),
         password=os.getenv("MYSQL_PASSWORD"),
         port=int(os.getenv("MYSQL_PORT")),
     )
 )
         """
+    elif db_type == "mongodb":
+        return f"""{base_template}
+
+config = OdmService(
+    db_type="{db_type}",
+    config_params={{
+        "db_name": os.getenv("DB_NAME"),
+        "host": os.getenv("DB_HOST"),
+        "user": os.getenv("DB_USER"),
+        "password": os.getenv("DB_PASSWORD"),
+        "port": os.getenv("DB_PORT"),
+    }},
+    document_models=[Examples]
+)       
+        """
     else:
         raise ValueError(f"Unsupported db type: {db_type}")
```

### Comparing `pynest-api-0.0.3/nest/common/templates/readme.py` & `pynest-api-0.1.0/nest/common/templates/readme.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.3/nest/common/templates/service.py` & `pynest-api-0.1.0/nest/common/templates/service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,38 @@
-def generate_service(controller_name: str) -> str:
+def generate_service(controller_name: str, db_type: str) -> str:
     split_controller_name = controller_name.split("_")
     capitalized_controller_name = "".join(
         [word.capitalize() for word in split_controller_name]
     )
-    template = f"""from src.{controller_name}.{controller_name}_model import {capitalized_controller_name}
+    if db_type == "mongodb":
+        template = f"""from src.{controller_name}.{controller_name}_model import {capitalized_controller_name}
+from src.{controller_name}.{controller_name}_entity import {capitalized_controller_name} as {capitalized_controller_name}Entity
+from nest.core.decorators import db_request_handler
+from functools import lru_cache
+
+
+@lru_cache()
+class {capitalized_controller_name}Service:
+
+    @db_request_handler
+    async def add_{controller_name}(self, {controller_name}: {capitalized_controller_name}):
+        new_{controller_name} = {capitalized_controller_name}Entity(
+            **{controller_name}.dict()
+        )
+        await new_{controller_name}.save()
+        return new_{controller_name}.id
+
+    @db_request_handler
+    async def get_{controller_name}(self):
+        return await {capitalized_controller_name}Entity.find_all().to_list()
+
+"""
+    else:
+
+        template = f"""from src.{controller_name}.{controller_name}_model import {capitalized_controller_name}
 from src.{controller_name}.{controller_name}_entity import {capitalized_controller_name} as {capitalized_controller_name}Entity
 from orm_config import config
 from nest.core.decorators import db_request_handler
 from functools import lru_cache
 
 
 @lru_cache()
@@ -26,8 +51,8 @@
         self.session.commit()
         return new_{controller_name}.id
 
     @db_request_handler
     def get_{controller_name}(self):
         return self.session.query({capitalized_controller_name}Entity).all()
  """
-    return template
+    return template
```

### Comparing `pynest-api-0.0.3/nest/core/app.py` & `pynest-api-0.1.0/nest/core/app.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from typing import List, Callable
 from fastapi import FastAPI, APIRouter
 
 
 class App(FastAPI):
-    def __init__(self, description: str, modules: List, init_db: Callable = None):
+    def __init__(self, description: str, modules: List):
         """
         Initializes the App instance.
 
         Args:
             description (str): The description of the application.
             modules (List): A list of modules to register.
-            init_db (Callable, optional): A callable function to initialize the database. Defaults to None.
 
         """
         super().__init__(description=description)
         self.modules = modules
         self._register_controllers()
-        if init_db:
-            init_db()
 
     def _register_controllers(self):
         """
         Registers the controllers from the provided modules.
 
         """
         for module in self.modules:
```

### Comparing `pynest-api-0.0.3/nest/core/database/base_orm.py` & `pynest-api-0.1.0/nest/core/database/base_orm.py`

 * *Files identical despite different names*

### Comparing `pynest-api-0.0.3/nest/core/database/orm_config.py` & `pynest-api-0.1.0/nest/core/database/orm_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,13 @@
-from abc import abstractmethod
+from pydantic import BaseConfig
+from nest.core.database.config import ConfigFactoryBase
+from nest.core.database.config import BaseProvider
 
 
-class BaseOrmConfig:
-    """
-    Base abstract class for ORM (Object-Relational Mapping) configurations.
-
-    """
-
-    @abstractmethod
-    def get_engine_url(self) -> str:
-        """
-        Returns the engine URL for the ORM.
-
-        Returns:
-            str: The engine URL.
-
-        """
-        pass
-
-
-class BaseOrmProvider(BaseOrmConfig):
-    """
-    Base class for ORM providers that implement the BaseOrmConfig interface.
-
-    Args:
-        host (str): The database host.
-        db_name (str): The name of the database.
-        user (str): The username for database authentication.
-        password (str): The password for database authentication.
-        port (int): The database port number.
-
-    """
-
-    def __init__(self, host: str, db_name: str, user: str, password: str, port: int):
-        """
-        Initializes the BaseOrmProvider instance.
-
-        Args:
-            host (str): The database host.
-            db_name (str): The name of the database.
-            user (str): The username for database authentication.
-            password (str): The password for database authentication.
-            port (int): The database port number.
-
-        """
-        self.host = host
-        self.db_name = db_name
-        self.user = user
-        self.password = password
-        self.port = port
-
-    def get_engine_url(self) -> str:
-        """
-        Returns the engine URL for the ORM.
-
-        Returns:
-            str: The engine URL.
-
-        """
-        pass
-
-
-class PostgresConfig(BaseOrmProvider):
+class PostgresConfig(BaseProvider):
     """
     ORM configuration for PostgreSQL.
 
     Args:
         host (str): The database host.
         db_name (str): The name of the database.
         user (str): The username for database authentication.
@@ -95,15 +37,15 @@
         Returns:
             str: The engine URL.
 
         """
         return f"postgresql+psycopg2://{self.user}:{self.password}@{self.host}:{self.port}/{self.db_name}"
 
 
-class MySQLConfig(BaseOrmProvider):
+class MySQLConfig(BaseProvider):
     """
     ORM configuration for MySQL.
 
     Args:
         host (str): The database host.
         db_name (str): The name of the database.
         user (str): The username for database authentication.
@@ -130,18 +72,18 @@
         """
         Returns the engine URL for the ORM.
 
         Returns:
             str: The engine URL.
 
         """
-        return f"mysql+mysqlconnector://{self.user}:{self.password}@{self.host}"
+        return f"mysql+mysqlconnector://{self.user}:{self.password}@{self.host}:{self.port}/{self.db_name}"
 
 
-class SQLiteConfig(BaseOrmConfig):
+class SQLiteConfig(BaseConfig):
     """
     ORM configuration for SQLite.
 
     Args:
         db_name (str): The name of the SQLite database file.
 
     """
@@ -163,15 +105,15 @@
         Returns:
             str: The engine URL.
 
         """
         return f"sqlite:///{self.db_name}.db"
 
 
-class ConfigFactory:
+class ConfigFactory(ConfigFactoryBase):
     """
     Factory class for retrieving the appropriate ORM configuration based on the database type.
 
     Args:
         db_type (str): The type of database.
 
     """
@@ -180,15 +122,15 @@
         """
         Initializes the ConfigFactory instance.
 
         Args:
             db_type (str): The type of database.
 
         """
-        self.db_type = db_type
+        super().__init__(db_type)
 
     def get_config(self):
         """
         Returns the appropriate ORM configuration class based on the database type.
 
         Returns:
             class: The ORM configuration class.
```

### Comparing `pynest-api-0.0.3/nest/core/decorators/controller.py` & `pynest-api-0.1.0/nest/core/decorators/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from fastapi_utils.cbv import _cbv as ClassBasedView
-from fastapi_utils.inferring_router import InferringRouter
+from fastapi.routing import APIRouter
+from nest.core.decorators.helpers import class_based_view as ClassBasedView
 
 
 def Controller(tag: str = None, prefix: str = None):
     """
     Decorator that turns a class into a controller, allowing you to define routes using FastAPI decorators.
 
     Args:
@@ -16,16 +16,16 @@
     """
     if prefix:
         if not prefix.startswith("/"):
             prefix = "/" + prefix
         if prefix.endswith("/"):
             prefix = prefix[:-1]
 
-    def wrapper(cls):
-        router = InferringRouter(tags=[tag] if tag else None)
+    def wrapper(cls) -> ClassBasedView:
+        router = APIRouter(tags=[tag] if tag else None)
 
         for name, method in cls.__dict__.items():
             if callable(method) and hasattr(method, "method"):
                 if not method.__path__:
                     raise Exception("Missing path")
                 else:
                     if prefix:
@@ -66,18 +66,18 @@
                             method,
                             methods=["PATCH"],
                             **method.__kwargs__
                         )
                     else:
                         raise Exception("Invalid method")
 
-        def get_router():
+        def get_router() -> APIRouter:
             """
             Returns:
-                InferringRouter: The router associated with the controller.
+                APIRouter: The router associated with the controller.
             """
             return router
 
         cls.get_router = get_router
 
         return ClassBasedView(router=router, cls=cls)
```

### Comparing `pynest-api-0.0.3/nest/core/decorators/database.py` & `pynest-api-0.1.0/nest/core/decorators/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 
     def wrapper(self, *args, **kwargs):
         try:
             s = time.time()
             result = func(self, *args, **kwargs)
             p_time = time.time() - s
             logging.info(f"request finished after {p_time}")
-            self.session.close()
+            if hasattr(self, 'session'):
+                # Check if self is an instance of OrmService
+                self.session.close()
             return result
         except Exception as e:
             logging.error(e)
-            self.session.rollback()
-            self.session.close()
+            if hasattr(self, 'session'):
+                # Check if self is an instance of OrmService
+                self.session.rollback()
+                self.session.close()
             return HTTPException(status_code=500, detail=str(e))
 
     return wrapper
```

### Comparing `pynest-api-0.0.3/pynest_api.egg-info/PKG-INFO` & `pynest-api-0.1.0/pynest_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7079 6e65  : 2.1.Name: pyne
 00000020: 7374 2d61 7069 0a56 6572 7369 6f6e 3a20  st-api.Version: 
-00000030: 302e 302e 330a 5375 6d6d 6172 793a 2050  0.0.3.Summary: P
+00000030: 302e 312e 300a 5375 6d6d 6172 793a 2050  0.1.0.Summary: P
 00000040: 794e 6573 7420 6973 2061 2046 6173 7441  yNest is a FastA
 00000050: 5049 2041 6273 7472 6163 7469 6f6e 2066  PI Abstraction f
 00000060: 6f72 2062 7569 6c64 696e 6720 6d69 6372  or building micr
 00000070: 6f73 6572 7669 6365 732c 2069 6e66 6c75  oservices, influ
 00000080: 656e 6365 6420 6279 204e 6573 744a 532e  enced by NestJS.
 00000090: 0a41 7574 686f 722d 656d 6169 6c3a 2049  .Author-email: I
 000000a0: 7461 7920 4461 7220 3c69 7461 7932 3830  tay Dar <itay280
@@ -102,804 +102,827 @@
 00000650: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
 00000660: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
 00000670: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
 00000680: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
 00000690: 2049 6e64 6570 656e 6465 6e74 0a43 6c61   Independent.Cla
 000006a0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 000006b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000006c0: 2050 7974 686f 6e20 3a3a 2033 2e37 0a43   Python :: 3.7.C
+000006c0: 2050 7974 686f 6e20 3a3a 2033 2e38 0a43   Python :: 3.8.C
 000006d0: 6c61 7373 6966 6965 723a 2050 726f 6772  lassifier: Progr
 000006e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000006f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e38  :: Python :: 3.8
+000006f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
 00000700: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
 00000710: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 00000720: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000730: 2e39 0a43 6c61 7373 6966 6965 723a 2050  .9.Classifier: P
-00000740: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000750: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000760: 2033 2e31 300a 5265 7175 6972 6573 2d50   3.10.Requires-P
-00000770: 7974 686f 6e3a 203e 3d33 2e38 2e31 0a44  ython: >=3.8.1.D
-00000780: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-00000790: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-000007a0: 726b 646f 776e 0a50 726f 7669 6465 732d  rkdown.Provides-
-000007b0: 4578 7472 613a 2074 6573 740a 4c69 6365  Extra: test.Lice
-000007c0: 6e73 652d 4669 6c65 3a20 4c49 4345 4e53  nse-File: LICENS
-000007d0: 450a 0a3c 7020 616c 6967 6e3d 2263 656e  E..<p align="cen
-000007e0: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-000007f0: 3d22 646f 6373 2f69 6d67 732f 7079 6e65  ="docs/imgs/pyne
-00000800: 7374 5f6c 6f67 6f2d 6d6f 6469 6669 6564  st_logo-modified
-00000810: 2e70 6e67 2220 7469 746c 653d 2270 796e  .png" title="pyn
-00000820: 6573 7420 6c6f 676f 2220 7769 6474 683d  est logo" width=
-00000830: 2232 3030 223e 0a3c 2f70 3e0a 3c70 2061  "200">.</p>.<p a
-00000840: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
-00000850: 2020 203c 656d 3e50 794e 6573 7420 6973     <em>PyNest is
-00000860: 2061 2050 7974 686f 6e20 6672 616d 6577   a Python framew
-00000870: 6f72 6b20 6275 696c 7420 6f6e 2074 6f70  ork built on top
-00000880: 206f 6620 4661 7374 4150 4920 7468 6174   of FastAPI that
-00000890: 2066 6f6c 6c6f 7773 2074 6865 206d 6f64   follows the mod
-000008a0: 756c 6172 2061 7263 6869 7465 6374 7572  ular architectur
-000008b0: 6520 6f66 204e 6573 744a 533c 2f65 6d3e  e of NestJS</em>
-000008c0: 0a3c 2f70 3e0a 3c70 2061 6c69 676e 3d22  .</p>.<p align="
-000008d0: 6365 6e74 6572 223e 0a3c 6120 6872 6566  center">.<a href
-000008e0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-000008f0: 7267 2f70 726f 6a65 6374 2f70 796e 6573  rg/project/pynes
-00000900: 742d 6170 6922 2074 6172 6765 743d 225f  t-api" target="_
-00000910: 626c 616e 6b22 3e0a 2020 2020 3c69 6d67  blank">.    <img
-00000920: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00000930: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00000940: 692f 762f 7079 6e65 7374 2d61 7069 3f63  i/v/pynest-api?c
-00000950: 6f6c 6f72 3d25 3233 3334 4430 3538 266c  olor=%2334D058&l
-00000960: 6162 656c 3d70 7970 6925 3230 7061 636b  abel=pypi%20pack
-00000970: 6167 6522 2061 6c74 3d22 5061 636b 6167  age" alt="Packag
-00000980: 6520 7665 7273 696f 6e22 3e0a 3c2f 613e  e version">.</a>
-00000990: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-000009a0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
-000009b0: 6374 2f70 796e 6573 742d 6170 6922 2074  ct/pynest-api" t
-000009c0: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
-000009d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000009e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000009f0: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
-00000a00: 696f 6e73 2f70 796e 6573 742d 6170 692e  ions/pynest-api.
-00000a10: 7376 673f 636f 6c6f 723d 2532 3333 3444  svg?color=%2334D
-00000a20: 3035 3822 2061 6c74 3d22 5375 7070 6f72  058" alt="Suppor
-00000a30: 7465 6420 5079 7468 6f6e 2076 6572 7369  ted Python versi
-00000a40: 6f6e 7322 3e0a 3c2f 613e 0a3c 2f70 3e0a  ons">.</a>.</p>.
-00000a50: 0a23 2050 794e 6573 7420 2d20 4465 7363  .# PyNest - Desc
-00000a60: 7269 7074 696f 6e0a 0a50 794e 6573 7420  ription..PyNest 
-00000a70: 6973 2064 6573 6967 6e65 6420 746f 2068  is designed to h
-00000a80: 656c 7020 7374 7275 6374 7572 6520 796f  elp structure yo
-00000a90: 7572 2041 5049 7320 696e 2061 6e20 696e  ur APIs in an in
-00000aa0: 7475 6974 6976 652c 2065 6173 7920 746f  tuitive, easy to
-00000ab0: 2075 6e64 6572 7374 616e 642c 2061 6e64   understand, and
-00000ac0: 2065 6e6a 6f79 6162 6c65 2077 6179 2e0a   enjoyable way..
-00000ad0: 0a57 6974 6820 5079 4e65 7374 2c20 796f  .With PyNest, yo
-00000ae0: 7520 6361 6e20 6275 696c 6420 7363 616c  u can build scal
-00000af0: 6162 6c65 2061 6e64 206d 6169 6e74 6169  able and maintai
-00000b00: 6e61 626c 6520 4150 4973 2077 6974 6820  nable APIs with 
-00000b10: 6561 7365 2e20 5468 6520 6672 616d 6577  ease. The framew
-00000b20: 6f72 6b20 7375 7070 6f72 7473 2064 6570  ork supports dep
-00000b30: 656e 6465 6e63 7920 696e 6a65 6374 696f  endency injectio
-00000b40: 6e2c 2074 7970 6520 616e 6e6f 7461 7469  n, type annotati
-00000b50: 6f6e 732c 2064 6563 6f72 6174 6f72 732c  ons, decorators,
-00000b60: 2061 6e64 2063 6f64 6520 6765 6e65 7261   and code genera
-00000b70: 7469 6f6e 2c20 6d61 6b69 6e67 2069 7420  tion, making it 
-00000b80: 6561 7379 2074 6f20 7772 6974 6520 636c  easy to write cl
-00000b90: 6561 6e20 616e 6420 7465 7374 6162 6c65  ean and testable
-00000ba0: 2063 6f64 652e 0a0a 5468 6973 2066 7261   code...This fra
-00000bb0: 6d65 776f 726b 2069 7320 6e6f 7420 6120  mework is not a 
-00000bc0: 6469 7265 6374 2070 6f72 7420 6f66 204e  direct port of N
-00000bd0: 6573 744a 5320 746f 2050 7974 686f 6e20  estJS to Python 
-00000be0: 6275 7420 7261 7468 6572 2061 2072 652d  but rather a re-
-00000bf0: 696d 6167 696e 696e 6720 6f66 2074 6865  imagining of the
-00000c00: 2066 7261 6d65 776f 726b 2073 7065 6369   framework speci
-00000c10: 6669 6361 6c6c 7920 666f 7220 5079 7468  fically for Pyth
-00000c20: 6f6e 2064 6576 656c 6f70 6572 732c 2069  on developers, i
-00000c30: 6e63 6c75 6469 6e67 2064 6174 6120 7363  ncluding data sc
-00000c40: 6965 6e74 6973 7473 2c20 6461 7461 2061  ientists, data a
-00000c50: 6e61 6c79 7374 732c 2061 6e64 2064 6174  nalysts, and dat
-00000c60: 6120 656e 6769 6e65 6572 732e 2049 7420  a engineers. It 
-00000c70: 6169 6d73 2074 6f20 6173 7369 7374 2074  aims to assist t
-00000c80: 6865 6d20 696e 2062 7569 6c64 696e 6720  hem in building 
-00000c90: 6265 7474 6572 2061 6e64 2066 6173 7465  better and faste
-00000ca0: 7220 4150 4973 2066 6f72 2074 6865 6972  r APIs for their
-00000cb0: 2064 6174 6120 6170 706c 6963 6174 696f   data applicatio
-00000cc0: 6e73 2e0a 0a23 2320 4765 7474 696e 6720  ns...## Getting 
-00000cd0: 5374 6172 7465 640a 546f 2067 6574 2073  Started.To get s
-00000ce0: 7461 7274 6564 2077 6974 6820 5079 4e65  tarted with PyNe
-00000cf0: 7374 2c20 796f 7527 6c6c 206e 6565 6420  st, you'll need 
-00000d00: 746f 2069 6e73 7461 6c6c 2069 7420 7573  to install it us
-00000d10: 696e 6720 7069 703a 0a0a 6060 6062 6173  ing pip:..```bas
-00000d20: 680a 7069 7020 696e 7374 616c 6c20 7079  h.pip install py
-00000d30: 6e65 7374 2d61 7069 0a60 6060 0a0a 2323  nest-api.```..##
-00000d40: 2320 5374 6172 7420 7769 7468 2063 6c69  # Start with cli
-00000d50: 0a60 6060 6261 7368 0a70 796e 6573 7420  .```bash.pynest 
-00000d60: 6372 6561 7465 2d6e 6573 742d 6170 7020  create-nest-app 
-00000d70: 2d6e 206d 795f 6170 705f 6e61 6d65 0a60  -n my_app_name.`
-00000d80: 6060 0a0a 7468 6973 2063 6f6d 6d61 6e64  ``..this command
-00000d90: 2077 696c 6c20 6372 6561 7465 2061 206e   will create a n
-00000da0: 6577 2070 726f 6a65 6374 2077 6974 6820  ew project with 
-00000db0: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
-00000dc0: 7275 6374 7572 653a 0a0a 6060 6074 6578  ructure:..```tex
-00000dd0: 740a e294 9ce2 9480 e294 8020 6170 702e  t.......... app.
-00000de0: 7079 0ae2 949c e294 80e2 9480 206f 726d  py.......... orm
-00000df0: 5f63 6f6e 6669 672e 7079 0ae2 949c e294  _config.py......
-00000e00: 80e2 9480 206d 6169 6e2e 7079 0ae2 949c  .... main.py....
-00000e10: e294 80e2 9480 2073 7263 0ae2 9482 2020  ...... src....  
-00000e20: 2020 e294 9ce2 9480 e294 8020 5f5f 696e    ......... __in
-00000e30: 6974 5f5f 2e70 790a e294 8220 2020 20e2  it__.py....    .
-00000e40: 949c e294 80e2 9480 2065 7861 6d70 6c65  ........ example
-00000e50: 730a e294 8220 2020 20e2 9482 2020 2020  s....    ...    
-00000e60: e294 9ce2 9480 e294 8020 5f5f 696e 6974  ......... __init
-00000e70: 5f5f 2e70 790a e294 8220 2020 20e2 9482  __.py....    ...
-00000e80: 2020 2020 e294 9ce2 9480 e294 8020 6578      ......... ex
-00000e90: 616d 706c 6573 5f63 6f6e 7472 6f6c 6c65  amples_controlle
-00000ea0: 722e 7079 0ae2 9482 2020 2020 e294 8220  r.py....    ... 
-00000eb0: 2020 20e2 949c e294 80e2 9480 2065 7861     ......... exa
-00000ec0: 6d70 6c65 735f 7365 7276 6963 652e 7079  mples_service.py
-00000ed0: 0ae2 9482 2020 2020 e294 8220 2020 20e2  ....    ...    .
-00000ee0: 949c e294 80e2 9480 2065 7861 6d70 6c65  ........ example
-00000ef0: 735f 6d6f 6465 6c2e 7079 0ae2 9482 2020  s_model.py....  
-00000f00: 2020 e294 9ce2 9480 e294 8020 20e2 949c    .........  ...
-00000f10: e294 80e2 9480 2065 7861 6d70 6c65 735f  ...... examples_
-00000f20: 656e 7469 7479 2e70 790a e294 8220 2020  entity.py....   
-00000f30: 20e2 949c e294 80e2 9480 2020 e294 9ce2   .........  ....
-00000f40: 9480 e294 8020 6578 616d 706c 6573 5f6d  ..... examples_m
-00000f50: 6f64 756c 652e 7079 0a60 6060 0a0a 6f6e  odule.py.```..on
-00000f60: 6365 2079 6f75 2068 6176 6520 6372 6561  ce you have crea
-00000f70: 7465 6420 796f 7572 2061 7070 2c20 6765  ted your app, ge
-00000f80: 7420 696e 746f 2074 6865 2066 6f6c 6465  t into the folde
-00000f90: 7220 616e 6420 7275 6e20 7468 6520 666f  r and run the fo
-00000fa0: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
-00000fb0: 0a0a 6060 6062 6173 680a 6364 206d 795f  ..```bash.cd my_
-00000fc0: 6170 705f 6e61 6d65 0a60 6060 0a0a 7275  app_name.```..ru
-00000fd0: 6e20 7468 6520 7365 7276 6572 2077 6974  n the server wit
-00000fe0: 6820 7468 6520 666f 6c6c 6f77 696e 6720  h the following 
-00000ff0: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
-00001000: 680a 7576 6963 6f72 6e20 2261 7070 3a61  h.uvicorn "app:a
-00001010: 7070 2220 2d2d 686f 7374 2022 302e 302e  pp" --host "0.0.
-00001020: 302e 3022 202d 2d70 6f72 7420 2238 3022  0.0" --port "80"
-00001030: 202d 2d72 656c 6f61 640a 6060 600a 0a4e   --reload.```..N
-00001040: 6f77 2079 6f75 2063 616e 2076 6973 6974  ow you can visit
-00001050: 205b 4f70 656e 4150 495d 2868 7474 703a   [OpenAPI](http:
-00001060: 2f2f 6c6f 6361 6c68 6f73 743a 3830 2f64  //localhost:80/d
-00001070: 6f63 7329 2069 6e20 796f 7572 2062 726f  ocs) in your bro
-00001080: 7773 6572 2074 6f20 7365 6520 7468 6520  wser to see the 
-00001090: 6465 6661 756c 7420 4150 4920 646f 6375  default API docu
-000010a0: 6d65 6e74 6174 696f 6e2e 0a0a 2323 2320  mentation...### 
-000010b0: 4164 6469 6e67 206d 6f64 756c 6573 0a0a  Adding modules..
-000010c0: 546f 2061 6464 2061 206e 6577 206d 6f64  To add a new mod
-000010d0: 756c 6520 746f 2079 6f75 7220 6170 706c  ule to your appl
-000010e0: 6963 6174 696f 6e2c 2079 6f75 2063 616e  ication, you can
-000010f0: 2075 7365 2074 6865 2070 796e 6573 7420   use the pynest 
-00001100: 6765 6e65 7261 7465 206d 6f64 756c 6520  generate module 
-00001110: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
-00001120: 680a 7079 6e65 7374 2067 656e 6572 6174  h.pynest generat
-00001130: 652d 6d6f 6475 6c65 202d 6e20 7573 6572  e-module -n user
-00001140: 730a 6060 600a 0a54 6869 7320 7769 6c6c  s.```..This will
-00001150: 2063 7265 6174 6520 6120 6e65 7720 6d6f   create a new mo
-00001160: 6475 6c65 2063 616c 6c65 6420 6060 6075  dule called ```u
-00001170: 7365 7273 6060 6020 696e 2079 6f75 7220  sers``` in your 
-00001180: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-00001190: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
-000011a0: 7472 7563 7475 7265 3a0a 0a60 6060 7465  tructure:..```te
-000011b0: 7874 0ae2 949c e294 80e2 9480 2075 7365  xt.......... use
-000011c0: 7273 0ae2 9482 2020 2020 e294 9ce2 9480  rs....    ......
-000011d0: e294 8020 5f5f 696e 6974 5f5f 2e70 790a  ... __init__.py.
-000011e0: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
-000011f0: 2075 7365 7273 5f63 6f6e 7472 6f6c 6c65   users_controlle
-00001200: 722e 7079 0ae2 9482 2020 2020 e294 9ce2  r.py....    ....
-00001210: 9480 e294 8020 7573 6572 735f 7365 7276  ..... users_serv
-00001220: 6963 652e 7079 0ae2 9482 2020 2020 e294  ice.py....    ..
-00001230: 9ce2 9480 e294 8020 7573 6572 735f 6d6f  ....... users_mo
-00001240: 6465 6c2e 7079 0ae2 9482 2020 2020 e294  del.py....    ..
-00001250: 9ce2 9480 e294 8020 7573 6572 735f 656e  ....... users_en
-00001260: 7469 7479 2e70 790a e294 8220 2020 20e2  tity.py....    .
-00001270: 949c e294 80e2 9480 2075 7365 7273 5f6d  ........ users_m
-00001280: 6f64 756c 652e 7079 0a60 6060 0a0a 5468  odule.py.```..Th
-00001290: 6520 7573 6572 7320 6d6f 6475 6c65 2077  e users module w
-000012a0: 696c 6c20 696d 6d65 6469 6174 656c 7920  ill immediately 
-000012b0: 7265 6769 7374 6572 2069 7473 656c 6620  register itself 
-000012c0: 7769 7468 2074 6865 2061 7070 6c69 6361  with the applica
-000012d0: 7469 6f6e 2061 6e64 2077 696c 6c20 6265  tion and will be
-000012e0: 2061 7661 696c 6162 6c65 2066 6f72 2075   available for u
-000012f0: 7365 2e0a 0a59 6f75 2063 616e 2074 6865  se...You can the
-00001300: 6e20 7374 6172 7420 6465 6669 6e69 6e67  n start defining
-00001310: 2072 6f75 7465 7320 616e 6420 6f74 6865   routes and othe
-00001320: 7220 6170 706c 6963 6174 696f 6e20 636f  r application co
-00001330: 6d70 6f6e 656e 7473 2075 7369 6e67 2064  mponents using d
-00001340: 6563 6f72 6174 6f72 7320 616e 6420 6f74  ecorators and ot
-00001350: 6865 7220 5079 4e65 7374 2063 6f6e 7374  her PyNest const
-00001360: 7275 6374 732e 0a0a 466f 7220 6d6f 7265  ructs...For more
-00001370: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00001380: 686f 7720 746f 2075 7365 2050 794e 6573  how to use PyNes
-00001390: 742c 2063 6865 636b 206f 7574 2074 6865  t, check out the
-000013a0: 206f 6666 6963 6961 6c20 646f 6375 6d65   official docume
-000013b0: 6e74 6174 696f 6e20 6174 2068 7474 7073  ntation at https
-000013c0: 3a2f 2f70 7974 686f 6e6e 6573 742e 6769  ://pythonnest.gi
-000013d0: 7468 7562 2e69 6f2f 5079 4e65 7374 2f2e  thub.io/PyNest/.
-000013e0: 0a0a 2323 2053 7461 7274 696e 6720 6120  ..## Starting a 
-000013f0: 6e65 7720 7072 6f6a 6563 7420 6d61 6e75  new project manu
-00001400: 616c 6c79 0a0a 6060 6074 6578 740a 4e4f  ally..```text.NO
-00001410: 5449 4345 3a20 666f 7220 7468 6520 666f  TICE: for the fo
-00001420: 6c6c 6f77 696e 6720 6578 616d 706c 652c  llowing example,
-00001430: 2077 6520 7769 6c6c 2075 7365 2074 6865   we will use the
-00001440: 2070 726f 6475 6374 7320 6d6f 6475 6c65   products module
-00001450: 2e20 0a60 6060 0a0a 546f 2073 7461 7274  . .```..To start
-00001460: 2061 206e 6577 2070 726f 6a65 6374 206d   a new project m
-00001470: 616e 7561 6c6c 792c 2079 6f75 276c 6c20  anually, you'll 
-00001480: 6e65 6564 2074 6f20 6372 6561 7465 2061  need to create a
-00001490: 2070 726f 6a65 6374 2074 6861 7420 666f   project that fo
-000014a0: 6c6c 6f77 7320 7468 6973 2073 7472 7563  llows this struc
-000014b0: 7475 7265 3a0a 0a60 6060 7465 7874 0ae2  ture:..```text..
-000014c0: 949c e294 80e2 9480 2061 7070 2e70 790a  ........ app.py.
-000014d0: e294 9ce2 9480 e294 8020 6f72 6d5f 636f  ......... orm_co
-000014e0: 6e66 6967 2e70 790a e294 9ce2 9480 e294  nfig.py.........
-000014f0: 8020 6d61 696e 2e70 790a e294 9ce2 9480  . main.py.......
-00001500: e294 8020 7372 630a e294 8220 2020 20e2  ... src....    .
-00001510: 949c e294 80e2 9480 205f 5f69 6e69 745f  ........ __init_
-00001520: 5f2e 7079 0ae2 9482 2020 2020 e294 9ce2  _.py....    ....
-00001530: 9480 e294 8020 7072 6f64 7563 7473 0ae2  ..... products..
-00001540: 9482 2020 2020 e294 8220 2020 20e2 949c  ..    ...    ...
-00001550: e294 80e2 9480 205f 5f69 6e69 745f 5f2e  ...... __init__.
-00001560: 7079 0ae2 9482 2020 2020 e294 8220 2020  py....    ...   
-00001570: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
-00001580: 6374 735f 636f 6e74 726f 6c6c 6572 2e70  cts_controller.p
-00001590: 790a e294 8220 2020 20e2 9482 2020 2020  y....    ...    
-000015a0: e294 9ce2 9480 e294 8020 7072 6f64 7563  ......... produc
-000015b0: 7473 5f73 6572 7669 6365 2e70 790a e294  ts_service.py...
-000015c0: 8220 2020 20e2 9482 2020 2020 e294 9ce2  .    ...    ....
-000015d0: 9480 e294 8020 7072 6f64 7563 7473 5f6d  ..... products_m
-000015e0: 6f64 656c 2e70 790a e294 8220 2020 20e2  odel.py....    .
-000015f0: 949c e294 80e2 9480 2020 e294 9ce2 9480  ........  ......
-00001600: e294 8020 7072 6f64 7563 7473 5f65 6e74  ... products_ent
-00001610: 6974 792e 7079 0ae2 9482 2020 2020 e294  ity.py....    ..
-00001620: 9ce2 9480 e294 8020 20e2 949c e294 80e2  .......  .......
-00001630: 9480 2070 726f 6475 6374 735f 6d6f 6475  .. products_modu
-00001640: 6c65 2e70 790a 6060 600a 0a45 7870 6c61  le.py.```..Expla
-00001650: 6e61 7469 6f6e 3a20 5468 6973 2069 7320  nation: This is 
-00001660: 7468 6520 6469 7265 6374 6f72 7920 7374  the directory st
-00001670: 7275 6374 7572 6520 666f 7220 796f 7572  ructure for your
-00001680: 2070 726f 6a65 6374 2e20 4974 2069 6e63   project. It inc
-00001690: 6c75 6465 7320 7468 6520 6d61 696e 2066  ludes the main f
-000016a0: 696c 6573 2061 6e64 2061 2073 7263 2064  iles and a src d
-000016b0: 6972 6563 746f 7279 2074 6861 7420 636f  irectory that co
-000016c0: 6e74 6169 6e73 2079 6f75 7220 7072 6f6a  ntains your proj
-000016d0: 6563 7427 7320 736f 7572 6365 2063 6f64  ect's source cod
-000016e0: 652e 0a0a 2323 2320 4372 6561 7469 6e67  e...### Creating
-000016f0: 2074 6865 2066 696c 6573 0a0a 2323 2323   the files..####
-00001700: 206d 6169 6e2e 7079 0a60 6060 7079 7468   main.py.```pyth
-00001710: 6f6e 0a69 6d70 6f72 7420 7576 6963 6f72  on.import uvicor
-00001720: 6e0a 0a0a 6966 205f 5f6e 616d 655f 5f20  n...if __name__ 
-00001730: 3d3d 2027 5f5f 6d61 696e 5f5f 273a 0a20  == '__main__':. 
-00001740: 2020 2075 7669 636f 726e 2e72 756e 280a     uvicorn.run(.
-00001750: 2020 2020 2020 2020 2761 7070 3a61 7070          'app:app
-00001760: 272c 0a20 2020 2020 2020 2068 6f73 743d  ',.        host=
-00001770: 2230 2e30 2e30 2e30 222c 0a20 2020 2020  "0.0.0.0",.     
-00001780: 2020 2070 6f72 743d 3830 2c0a 2020 2020     port=80,.    
-00001790: 290a 6060 600a 0a54 6869 7320 6973 2074  ).```..This is t
-000017a0: 6865 206d 6169 6e2e 7079 2066 696c 652c  he main.py file,
-000017b0: 2077 6869 6368 2069 7320 7265 7370 6f6e   which is respon
-000017c0: 7369 626c 6520 666f 7220 7275 6e6e 696e  sible for runnin
-000017d0: 6720 796f 7572 2061 7070 6c69 6361 7469  g your applicati
-000017e0: 6f6e 2075 7369 6e67 2074 6865 2055 7669  on using the Uvi
-000017f0: 636f 726e 2073 6572 7665 722e 0a3c 6272  corn server..<br
-00001800: 3e0a 4974 2069 6d70 6f72 7473 2074 6865  >.It imports the
-00001810: 2075 7669 636f 726e 206c 6962 7261 7279   uvicorn library
-00001820: 2061 6e64 2073 7461 7274 7320 7468 6520   and starts the 
-00001830: 7365 7276 6572 2077 6974 6820 7468 6520  server with the 
-00001840: 7370 6563 6966 6965 6420 686f 7374 2061  specified host a
-00001850: 6e64 2070 6f72 742e 0a0a 0a23 2323 2320  nd port....#### 
-00001860: 6170 702e 7079 0a0a 6060 6070 7974 686f  app.py..```pytho
-00001870: 6e0a 6672 6f6d 206f 726d 5f63 6f6e 6669  n.from orm_confi
-00001880: 6720 696d 706f 7274 2063 6f6e 6669 670a  g import config.
-00001890: 6672 6f6d 206e 6573 742e 636f 7265 2069  from nest.core i
-000018a0: 6d70 6f72 7420 4170 700a 6672 6f6d 2073  mport App.from s
-000018b0: 7263 2e70 726f 6475 6374 732e 7072 6f64  rc.products.prod
-000018c0: 7563 7473 5f6d 6f64 756c 6520 696d 706f  ucts_module impo
-000018d0: 7274 2050 726f 6475 6374 734d 6f64 756c  rt ProductsModul
-000018e0: 650a 0a61 7070 203d 2041 7070 280a 2020  e..app = App(.  
-000018f0: 2020 6465 7363 7269 7074 696f 6e3d 2259    description="Y
-00001900: 6f75 7220 6170 7020 6465 7363 7269 7074  our app descript
-00001910: 696f 6e22 2c0a 2020 2020 6d6f 6475 6c65  ion",.    module
-00001920: 733d 5b0a 2020 2020 2020 2020 5072 6f64  s=[.        Prod
-00001930: 7563 7473 4d6f 6475 6c65 0a20 2020 205d  uctsModule.    ]
-00001940: 2c0a 2020 2020 696e 6974 5f64 623d 636f  ,.    init_db=co
-00001950: 6e66 6967 2e63 7265 6174 655f 616c 6c0a  nfig.create_all.
-00001960: 290a 6060 600a 0a54 6869 7320 6973 2074  ).```..This is t
-00001970: 6865 2061 7070 2e70 7920 6669 6c65 2c20  he app.py file, 
-00001980: 7768 6963 6820 6973 2074 6865 2065 6e74  which is the ent
-00001990: 7279 2070 6f69 6e74 2066 6f72 2079 6f75  ry point for you
-000019a0: 7220 6170 706c 6963 6174 696f 6e2e 2049  r application. I
-000019b0: 7420 696d 706f 7274 7320 6e65 6365 7373  t imports necess
-000019c0: 6172 7920 6d6f 6475 6c65 7320 616e 6420  ary modules and 
-000019d0: 7365 7473 2075 7020 7468 6520 4170 7020  sets up the App 
-000019e0: 6f62 6a65 6374 2077 6974 6820 6120 6465  object with a de
-000019f0: 7363 7269 7074 696f 6e20 616e 6420 7468  scription and th
-00001a00: 6520 5072 6f64 7563 7473 4d6f 6475 6c65  e ProductsModule
-00001a10: 2e0a 3c62 723e 0a49 7420 616c 736f 2069  ..<br>.It also i
-00001a20: 6e69 7469 616c 697a 6573 2074 6865 2064  nitializes the d
-00001a30: 6174 6162 6173 6520 7573 696e 6720 7468  atabase using th
-00001a40: 6520 636f 6e66 6967 2e63 7265 6174 655f  e config.create_
-00001a50: 616c 6c20 6675 6e63 7469 6f6e 2e0a 0a23  all function...#
-00001a60: 2323 2320 6f72 6d5f 636f 6e66 6967 2e70  ### orm_config.p
-00001a70: 790a 6060 6070 7974 686f 6e0a 6672 6f6d  y.```python.from
-00001a80: 206e 6573 742e 636f 7265 2069 6d70 6f72   nest.core impor
-00001a90: 7420 4f72 6d53 6572 7669 6365 0a69 6d70  t OrmService.imp
-00001aa0: 6f72 7420 6f73 0a66 726f 6d20 646f 7465  ort os.from dote
-00001ab0: 6e76 2069 6d70 6f72 7420 6c6f 6164 5f64  nv import load_d
-00001ac0: 6f74 656e 760a 0a6c 6f61 645f 646f 7465  otenv..load_dote
-00001ad0: 6e76 2829 0a0a 636f 6e66 6967 203d 204f  nv()..config = O
-00001ae0: 726d 5365 7276 6963 6528 0a20 2020 2064  rmService(.    d
-00001af0: 625f 7479 7065 3d22 796f 7572 5f64 625f  b_type="your_db_
-00001b00: 7479 7065 222c 0a20 2020 2063 6f6e 6669  type",.    confi
-00001b10: 675f 7061 7261 6d73 3d64 6963 7428 0a20  g_params=dict(. 
-00001b20: 2020 2020 2020 2075 7365 723d 6f73 2e67         user=os.g
-00001b30: 6574 656e 7628 2244 425f 5553 4552 2229  etenv("DB_USER")
-00001b40: 2c0a 2020 2020 2020 2020 7061 7373 776f  ,.        passwo
-00001b50: 7264 3d6f 732e 6765 7465 6e76 2822 4442  rd=os.getenv("DB
-00001b60: 5f50 4153 5357 4f52 4422 292c 0a20 2020  _PASSWORD"),.   
-00001b70: 2020 2020 2068 6f73 743d 6f73 2e67 6574       host=os.get
-00001b80: 656e 7628 2244 425f 484f 5354 2229 2c0a  env("DB_HOST"),.
-00001b90: 2020 2020 2020 2020 706f 7274 3d6f 732e          port=os.
-00001ba0: 6765 7465 6e76 2822 4442 5f50 4f52 5422  getenv("DB_PORT"
-00001bb0: 292c 0a20 2020 2020 2020 2064 6174 6162  ),.        datab
-00001bc0: 6173 653d 6f73 2e67 6574 656e 7628 2244  ase=os.getenv("D
-00001bd0: 425f 4e41 4d45 2229 2c0a 2020 2020 292c  B_NAME"),.    ),
-00001be0: 0a29 0a60 6060 0a0a 5468 6973 2069 7320  .).```..This is 
-00001bf0: 7468 6520 6f72 6d5f 636f 6e66 6967 2e70  the orm_config.p
-00001c00: 7920 6669 6c65 2c20 7768 6963 6820 636f  y file, which co
-00001c10: 6e74 6169 6e73 2074 6865 2063 6f6e 6669  ntains the confi
-00001c20: 6775 7261 7469 6f6e 2066 6f72 2079 6f75  guration for you
-00001c30: 7220 4f52 4d20 284f 626a 6563 742d 5265  r ORM (Object-Re
-00001c40: 6c61 7469 6f6e 616c 204d 6170 7069 6e67  lational Mapping
-00001c50: 2920 7365 7276 6963 652e 0a0a 4974 2069  ) service...It i
-00001c60: 6d70 6f72 7473 206e 6563 6573 7361 7279  mports necessary
-00001c70: 206c 6962 7261 7269 6573 2c20 6c6f 6164   libraries, load
-00001c80: 7320 656e 7669 726f 6e6d 656e 7420 7661  s environment va
-00001c90: 7269 6162 6c65 7320 7573 696e 6720 646f  riables using do
-00001ca0: 7465 6e76 2c20 616e 6420 6372 6561 7465  tenv, and create
-00001cb0: 7320 616e 204f 726d 5365 7276 6963 6520  s an OrmService 
-00001cc0: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00001cd0: 7370 6563 6966 6965 6420 6461 7461 6261  specified databa
-00001ce0: 7365 2074 7970 6520 616e 6420 636f 6e66  se type and conf
-00001cf0: 6967 7572 6174 696f 6e20 7061 7261 6d65  iguration parame
-00001d00: 7465 7273 2e0a 0a2d 2d2d 0a0a 4f6e 6365  ters...---..Once
-00001d10: 2077 6520 7365 7420 7570 2074 6869 7320   we set up this 
-00001d20: 3320 6669 6c65 732c 2077 6520 6361 6e20  3 files, we can 
-00001d30: 7374 6172 7420 6372 6561 7469 6e67 206f  start creating o
-00001d40: 7572 206d 6f64 756c 6573 2e20 6561 6368  ur modules. each
-00001d50: 206d 6f64 756c 6520 6973 2061 2066 6f6c   module is a fol
-00001d60: 6465 7220 7769 7468 2074 6865 2066 6f6c  der with the fol
-00001d70: 6c6f 7769 6e67 2073 7472 7563 7475 7265  lowing structure
-00001d80: 3a0a 0a60 6060 7465 7874 200a e294 9ce2  :..```text .....
-00001d90: 9480 e294 8020 7072 6f64 7563 7473 0ae2  ..... products..
-00001da0: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
-00001db0: 5f5f 696e 6974 5f5f 2e70 790a e294 8220  __init__.py.... 
-00001dc0: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
-00001dd0: 6475 6374 735f 636f 6e74 726f 6c6c 6572  ducts_controller
-00001de0: 2e70 790a e294 8220 2020 20e2 949c e294  .py....    .....
-00001df0: 80e2 9480 2070 726f 6475 6374 735f 7365  .... products_se
-00001e00: 7276 6963 652e 7079 0ae2 9482 2020 2020  rvice.py....    
-00001e10: e294 9ce2 9480 e294 8020 7072 6f64 7563  ......... produc
-00001e20: 7473 5f6d 6f64 656c 2e70 790a 7c20 2020  ts_model.py.|   
-00001e30: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
-00001e40: 6374 735f 656e 7469 7479 2e70 790a e294  cts_entity.py...
-00001e50: 8220 2020 20e2 949c e294 80e2 9480 2070  .    ......... p
-00001e60: 726f 6475 6374 735f 6d6f 6475 6c65 2e70  roducts_module.p
-00001e70: 790a 6060 600a 0a54 6869 7320 6973 2074  y.```..This is t
-00001e80: 6865 2073 7472 7563 7475 7265 206f 6620  he structure of 
-00001e90: 6120 6d6f 6475 6c65 2066 6f6c 6465 722e  a module folder.
-00001ea0: 2049 7420 696e 636c 7564 6573 2061 6e20   It includes an 
-00001eb0: 5f5f 696e 6974 5f5f 2e70 7920 6669 6c65  __init__.py file
-00001ec0: 2074 6f20 6d61 6b65 2074 6865 2066 6f6c   to make the fol
-00001ed0: 6465 7220 6120 5079 7468 6f6e 2070 6163  der a Python pac
-00001ee0: 6b61 6765 2c0a 3c62 723e 0a41 7320 7765  kage,.<br>.As we
-00001ef0: 6c6c 2061 7320 7370 6563 6966 6963 2066  ll as specific f
-00001f00: 696c 6573 2066 6f72 2074 6865 206d 6f64  iles for the mod
-00001f10: 756c 6527 7320 636f 6e74 726f 6c6c 6572  ule's controller
-00001f20: 2c20 7365 7276 6963 652c 206d 6f64 656c  , service, model
-00001f30: 2c20 656e 7469 7479 2c20 616e 6420 6d6f  , entity, and mo
-00001f40: 6475 6c65 2063 6f6e 6669 6775 7261 7469  dule configurati
-00001f50: 6f6e 732e 0a0a 2323 2323 2070 726f 6475  ons...#### produ
-00001f60: 6374 735f 6d6f 6465 6c2e 7079 0a60 6060  cts_model.py.```
-00001f70: 7079 7468 6f6e 0a66 726f 6d20 7079 6461  python.from pyda
-00001f80: 6e74 6963 2069 6d70 6f72 7420 4261 7365  ntic import Base
-00001f90: 4d6f 6465 6c0a 0a0a 636c 6173 7320 5072  Model...class Pr
-00001fa0: 6f64 7563 7428 4261 7365 4d6f 6465 6c29  oduct(BaseModel)
-00001fb0: 3a0a 2020 2020 6e61 6d65 3a20 7374 720a  :.    name: str.
-00001fc0: 2020 2020 7072 6963 653a 2066 6c6f 6174      price: float
-00001fd0: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00001fe0: 3a20 7374 720a 6060 600a 0a54 6869 7320  : str.```..This 
-00001ff0: 6973 2074 6865 2070 726f 6475 6374 735f  is the products_
-00002000: 6d6f 6465 6c2e 7079 2066 696c 652c 2077  model.py file, w
-00002010: 6869 6368 2064 6566 696e 6573 2074 6865  hich defines the
-00002020: 2050 726f 6475 6374 206d 6f64 656c 2075   Product model u
-00002030: 7369 6e67 2074 6865 2042 6173 654d 6f64  sing the BaseMod
-00002040: 656c 2063 6c61 7373 2066 726f 6d20 7468  el class from th
-00002050: 6520 7079 6461 6e74 6963 206c 6962 7261  e pydantic libra
-00002060: 7279 2e0a 3c62 723e 0a54 6865 206d 6f64  ry..<br>.The mod
-00002070: 656c 2072 6570 7265 7365 6e74 7320 7468  el represents th
-00002080: 6520 7374 7275 6374 7572 6520 616e 6420  e structure and 
-00002090: 6174 7472 6962 7574 6573 206f 6620 6120  attributes of a 
-000020a0: 7072 6f64 7563 742e 0a0a 2323 2323 2070  product...#### p
-000020b0: 726f 6475 6374 735f 656e 7469 7479 2e70  roducts_entity.p
-000020c0: 790a 0a60 6060 7079 7468 6f6e 0a66 726f  y..```python.fro
-000020d0: 6d20 7371 6c61 6c63 6865 6d79 2069 6d70  m sqlalchemy imp
-000020e0: 6f72 7420 436f 6c75 6d6e 2c20 496e 7465  ort Column, Inte
-000020f0: 6765 722c 2053 7472 696e 672c 2046 6c6f  ger, String, Flo
-00002100: 6174 0a66 726f 6d20 6f72 6d5f 636f 6e66  at.from orm_conf
-00002110: 6967 2069 6d70 6f72 7420 636f 6e66 6967  ig import config
-00002120: 0a0a 0a63 6c61 7373 2050 726f 6475 6374  ...class Product
-00002130: 2863 6f6e 6669 672e 4261 7365 293a 0a20  (config.Base):. 
-00002140: 2020 205f 5f74 6162 6c65 6e61 6d65 5f5f     __tablename__
-00002150: 203d 2022 7072 6f64 7563 7473 220a 0a20   = "products".. 
-00002160: 2020 2069 6420 3d20 436f 6c75 6d6e 2849     id = Column(I
-00002170: 6e74 6567 6572 2c20 7072 696d 6172 795f  nteger, primary_
-00002180: 6b65 793d 5472 7565 2c20 696e 6465 783d  key=True, index=
-00002190: 5472 7565 2c20 6175 746f 696e 6372 656d  True, autoincrem
-000021a0: 656e 743d 5472 7565 290a 2020 2020 6e61  ent=True).    na
-000021b0: 6d65 203d 2043 6f6c 756d 6e28 5374 7269  me = Column(Stri
-000021c0: 6e67 290a 2020 2020 7072 6963 6520 3d20  ng).    price = 
-000021d0: 436f 6c75 6d6e 2846 6c6f 6174 290a 2020  Column(Float).  
-000021e0: 2020 6465 7363 7269 7074 696f 6e20 3d20    description = 
-000021f0: 436f 6c75 6d6e 2853 7472 696e 6729 0a60  Column(String).`
-00002200: 6060 0a0a 5468 6973 2069 7320 7468 6520  ``..This is the 
-00002210: 7072 6f64 7563 7473 5f65 6e74 6974 792e  products_entity.
-00002220: 7079 2066 696c 652c 2077 6869 6368 2064  py file, which d
-00002230: 6566 696e 6573 2074 6865 2050 726f 6475  efines the Produ
-00002240: 6374 2065 6e74 6974 7920 7573 696e 6720  ct entity using 
-00002250: 5351 4c41 6c63 6865 6d79 2e20 0a3c 6272  SQLAlchemy. .<br
-00002260: 3e0a 4974 2069 6d70 6f72 7473 206e 6563  >.It imports nec
-00002270: 6573 7361 7279 206d 6f64 756c 6573 2061  essary modules a
-00002280: 6e64 2069 6e68 6572 6974 7320 6672 6f6d  nd inherits from
-00002290: 2074 6865 2063 6f6e 6669 672e 4261 7365   the config.Base
-000022a0: 2063 6c61 7373 2e20 5468 6520 656e 7469   class. The enti
-000022b0: 7479 2072 6570 7265 7365 6e74 7320 7468  ty represents th
-000022c0: 6520 6461 7461 6261 7365 2074 6162 6c65  e database table
-000022d0: 2066 6f72 2073 746f 7269 6e67 2070 726f   for storing pro
-000022e0: 6475 6374 732c 2077 6974 6820 636f 6c75  ducts, with colu
-000022f0: 6d6e 7320 666f 7220 6964 2c20 6e61 6d65  mns for id, name
-00002300: 2c20 7072 6963 652c 2061 6e64 2064 6573  , price, and des
-00002310: 6372 6970 7469 6f6e 2e0a 0a23 2323 2320  cription...#### 
-00002320: 7072 6f64 7563 7473 5f73 6572 7669 6365  products_service
-00002330: 2e70 790a 0a60 6060 7079 7468 6f6e 0a66  .py..```python.f
-00002340: 726f 6d20 7372 632e 7072 6f64 7563 7473  rom src.products
-00002350: 2e70 726f 6475 6374 735f 6d6f 6465 6c20  .products_model 
-00002360: 696d 706f 7274 2050 726f 6475 6374 0a66  import Product.f
-00002370: 726f 6d20 7372 632e 7072 6f64 7563 7473  rom src.products
-00002380: 2e70 726f 6475 6374 735f 656e 7469 7479  .products_entity
-00002390: 2069 6d70 6f72 7420 5072 6f64 7563 7420   import Product 
-000023a0: 6173 2050 726f 6475 6374 456e 7469 7479  as ProductEntity
-000023b0: 0a66 726f 6d20 6f72 6d5f 636f 6e66 6967  .from orm_config
-000023c0: 2069 6d70 6f72 7420 636f 6e66 6967 0a66   import config.f
-000023d0: 726f 6d20 6e65 7374 2e63 6f72 652e 6465  rom nest.core.de
-000023e0: 636f 7261 746f 7273 2069 6d70 6f72 7420  corators import 
-000023f0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
-00002400: 6572 0a0a 0a63 6c61 7373 2050 726f 6475  er...class Produ
-00002410: 6374 7353 6572 7669 6365 3a0a 2020 2020  ctsService:.    
-00002420: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-00002430: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-00002440: 2e63 6f6e 6669 6720 3d20 636f 6e66 6967  .config = config
-00002450: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00002460: 7373 696f 6e20 3d20 7365 6c66 2e63 6f6e  ssion = self.con
-00002470: 6669 672e 6765 745f 6462 2829 0a0a 2020  fig.get_db()..  
-00002480: 2020 4064 625f 7265 7175 6573 745f 6861    @db_request_ha
-00002490: 6e64 6c65 720a 2020 2020 6465 6620 6164  ndler.    def ad
-000024a0: 645f 7072 6f64 7563 7428 7365 6c66 2c20  d_product(self, 
-000024b0: 7072 6f64 7563 743a 2050 726f 6475 6374  product: Product
-000024c0: 293a 0a20 2020 2020 2020 2070 726f 6475  ):.        produ
-000024d0: 6374 5f65 6e74 6974 7920 3d20 5072 6f64  ct_entity = Prod
-000024e0: 7563 7445 6e74 6974 7928 0a20 2020 2020  uctEntity(.     
-000024f0: 2020 2020 2020 206e 616d 653d 7072 6f64         name=prod
-00002500: 7563 742e 6e61 6d65 2c0a 2020 2020 2020  uct.name,.      
-00002510: 2020 2020 2020 7072 6963 653d 7072 6f64        price=prod
-00002520: 7563 742e 7072 6963 652c 0a20 2020 2020  uct.price,.     
-00002530: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00002540: 6f6e 3d70 726f 6475 6374 2e64 6573 6372  on=product.descr
-00002550: 6970 7469 6f6e 0a20 2020 2020 2020 2029  iption.        )
-00002560: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
-00002570: 7373 696f 6e2e 6164 6428 7072 6f64 7563  ssion.add(produc
-00002580: 745f 656e 7469 7479 290a 2020 2020 2020  t_entity).      
-00002590: 2020 7365 6c66 2e73 6573 7369 6f6e 2e63    self.session.c
-000025a0: 6f6d 6d69 7428 290a 2020 2020 2020 2020  ommit().        
-000025b0: 7265 7475 726e 2070 726f 6475 6374 5f65  return product_e
-000025c0: 6e74 6974 792e 6964 0a0a 2020 2020 4064  ntity.id..    @d
-000025d0: 625f 7265 7175 6573 745f 6861 6e64 6c65  b_request_handle
-000025e0: 720a 2020 2020 6465 6620 6765 745f 7072  r.    def get_pr
-000025f0: 6f64 7563 7473 2873 656c 6629 3a0a 2020  oducts(self):.  
-00002600: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002610: 662e 7365 7373 696f 6e2e 7175 6572 7928  f.session.query(
-00002620: 5072 6f64 7563 7445 6e74 6974 7929 2e61  ProductEntity).a
-00002630: 6c6c 2829 0a0a 2020 2020 4064 625f 7265  ll()..    @db_re
-00002640: 7175 6573 745f 6861 6e64 6c65 720a 2020  quest_handler.  
-00002650: 2020 6465 6620 6765 745f 7072 6f64 7563    def get_produc
-00002660: 7428 7365 6c66 2c20 7072 6f64 7563 745f  t(self, product_
-00002670: 6964 3a20 696e 7429 3a0a 2020 2020 2020  id: int):.      
-00002680: 2020 7265 7475 726e 2073 656c 662e 7365    return self.se
-00002690: 7373 696f 6e2e 7175 6572 7928 5072 6f64  ssion.query(Prod
-000026a0: 7563 7445 6e74 6974 7929 2e66 696c 7465  uctEntity).filte
-000026b0: 7228 5072 6f64 7563 7445 6e74 6974 792e  r(ProductEntity.
-000026c0: 6964 203d 3d20 7072 6f64 7563 745f 6964  id == product_id
-000026d0: 292e 6669 7273 7428 290a 0a20 2020 2040  ).first()..    @
-000026e0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
-000026f0: 6572 0a20 2020 2064 6566 206c 6173 745f  er.    def last_
-00002700: 7072 6f64 7563 7428 7365 6c66 293a 0a20  product(self):. 
-00002710: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00002720: 6c66 2e73 6573 7369 6f6e 2e71 7565 7279  lf.session.query
-00002730: 2850 726f 6475 6374 456e 7469 7479 292e  (ProductEntity).
-00002740: 6f72 6465 725f 6279 2850 726f 6475 6374  order_by(Product
-00002750: 456e 7469 7479 2e69 642e 6465 7363 2829  Entity.id.desc()
-00002760: 292e 6669 7273 7428 290a 6060 600a 0a54  ).first().```..T
-00002770: 6869 7320 6973 2074 6865 2073 6572 7669  his is the servi
-00002780: 6365 2066 696c 652c 2077 6869 6368 2063  ce file, which c
-00002790: 6f6e 7461 696e 7320 7468 6520 5072 6f64  ontains the Prod
-000027a0: 7563 7473 5365 7276 6963 6520 636c 6173  uctsService clas
-000027b0: 732e 2049 7420 696d 706f 7274 7320 6e65  s. It imports ne
-000027c0: 6365 7373 6172 7920 6d6f 6475 6c65 7320  cessary modules 
-000027d0: 616e 6420 6465 6669 6e65 7320 6d65 7468  and defines meth
-000027e0: 6f64 7320 666f 7220 696e 7465 7261 6374  ods for interact
-000027f0: 696e 6720 7769 7468 2074 6865 2064 6174  ing with the dat
-00002800: 6162 6173 652e 200a 3c62 723e 0a54 6865  abase. .<br>.The
-00002810: 206d 6574 686f 6473 2069 6e63 6c75 6465   methods include
-00002820: 2061 6464 696e 6720 6120 7072 6f64 7563   adding a produc
-00002830: 742c 2067 6574 7469 6e67 2061 6c6c 2070  t, getting all p
-00002840: 726f 6475 6374 732c 2067 6574 7469 6e67  roducts, getting
-00002850: 2061 2073 7065 6369 6669 6320 7072 6f64   a specific prod
-00002860: 7563 7420 6279 2049 442c 2061 6e64 2072  uct by ID, and r
-00002870: 6574 7269 6576 696e 6720 7468 6520 6c61  etrieving the la
-00002880: 7374 2061 6464 6564 2070 726f 6475 6374  st added product
-00002890: 2e0a 3c62 723e 0a54 6865 2060 4064 625f  ..<br>.The `@db_
-000028a0: 7265 7175 6573 745f 6861 6e64 6c65 7260  request_handler`
-000028b0: 2064 6563 6f72 6174 6f72 2069 7320 7265   decorator is re
-000028c0: 7370 6f6e 7369 626c 6520 666f 7220 6d61  sponsible for ma
-000028d0: 6e61 6769 6e67 2074 6865 2064 6174 6162  naging the datab
-000028e0: 6173 6520 7365 7373 696f 6e20 616e 6420  ase session and 
-000028f0: 6861 6e64 6c69 6e67 2061 6e79 2065 7863  handling any exc
-00002900: 6570 7469 6f6e 7320 7468 6174 206d 6179  eptions that may
-00002910: 206f 6363 7572 2064 7572 696e 6720 6461   occur during da
-00002920: 7461 6261 7365 206f 7065 7261 7469 6f6e  tabase operation
-00002930: 732e 0a0a 0a23 2323 2320 7072 6f64 7563  s....#### produc
-00002940: 7473 5f63 6f6e 7472 6f6c 6c65 722e 7079  ts_controller.py
-00002950: 0a0a 6060 6070 7974 686f 6e0a 6672 6f6d  ..```python.from
-00002960: 206e 6573 742e 636f 7265 2069 6d70 6f72   nest.core impor
-00002970: 7420 4465 7065 6e64 732c 2043 6f6e 7472  t Depends, Contr
-00002980: 6f6c 6c65 722c 2047 6574 2c20 506f 7374  oller, Get, Post
-00002990: 0a66 726f 6d20 7372 632e 7072 6f64 7563  .from src.produc
-000029a0: 7473 2e70 726f 6475 6374 735f 7365 7276  ts.products_serv
-000029b0: 6963 6520 696d 706f 7274 2050 726f 6475  ice import Produ
-000029c0: 6374 7353 6572 7669 6365 0a66 726f 6d20  ctsService.from 
-000029d0: 7372 632e 7072 6f64 7563 7473 2e70 726f  src.products.pro
-000029e0: 6475 6374 735f 6d6f 6465 6c20 696d 706f  ducts_model impo
-000029f0: 7274 2050 726f 6475 6374 0a0a 0a40 436f  rt Product...@Co
-00002a00: 6e74 726f 6c6c 6572 2822 7072 6f64 7563  ntroller("produc
-00002a10: 7473 2229 0a63 6c61 7373 2050 726f 6475  ts").class Produ
-00002a20: 6374 7343 6f6e 7472 6f6c 6c65 723a 0a20  ctsController:. 
-00002a30: 2020 2073 6572 7669 6365 3a20 5072 6f64     service: Prod
-00002a40: 7563 7473 5365 7276 6963 6520 3d20 4465  uctsService = De
-00002a50: 7065 6e64 7328 5072 6f64 7563 7473 5365  pends(ProductsSe
-00002a60: 7276 6963 6529 0a0a 2020 2020 4047 6574  rvice)..    @Get
-00002a70: 2822 2f67 6574 5f70 726f 6475 6374 7322  ("/get_products"
-00002a80: 290a 2020 2020 6465 6620 6765 745f 7072  ).    def get_pr
-00002a90: 6f64 7563 7473 2873 656c 6629 3a0a 2020  oducts(self):.  
-00002aa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00002ab0: 662e 7365 7276 6963 652e 6765 745f 7072  f.service.get_pr
-00002ac0: 6f64 7563 7473 2829 0a0a 2020 2020 4047  oducts()..    @G
-00002ad0: 6574 2822 2f67 6574 5f70 726f 6475 6374  et("/get_product
-00002ae0: 2f7b 7072 6f64 7563 745f 6964 7d22 290a  /{product_id}").
-00002af0: 2020 2020 6465 6620 6765 745f 7072 6f64      def get_prod
-00002b00: 7563 7428 7365 6c66 2c20 7072 6f64 7563  uct(self, produc
-00002b10: 745f 6964 3a20 696e 7429 3a0a 2020 2020  t_id: int):.    
-00002b20: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00002b30: 7365 7276 6963 652e 6765 745f 7072 6f64  service.get_prod
-00002b40: 7563 7428 7072 6f64 7563 745f 6964 290a  uct(product_id).
-00002b50: 0a20 2020 2040 506f 7374 2822 2f61 6464  .    @Post("/add
-00002b60: 5f70 726f 6475 6374 2229 0a20 2020 2064  _product").    d
-00002b70: 6566 2061 6464 5f70 726f 6475 6374 2873  ef add_product(s
-00002b80: 656c 662c 2070 726f 6475 6374 3a20 5072  elf, product: Pr
-00002b90: 6f64 7563 7429 3a0a 2020 2020 2020 2020  oduct):.        
-00002ba0: 7265 7475 726e 2073 656c 662e 7365 7276  return self.serv
-00002bb0: 6963 652e 6164 645f 7072 6f64 7563 7428  ice.add_product(
-00002bc0: 7072 6f64 7563 7429 0a0a 2020 2020 4047  product)..    @G
-00002bd0: 6574 2822 2f6c 6173 745f 7072 6f64 7563  et("/last_produc
-00002be0: 7422 290a 2020 2020 6465 6620 6c61 7374  t").    def last
-00002bf0: 5f70 726f 6475 6374 2873 656c 6629 3a0a  _product(self):.
-00002c00: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002c10: 656c 662e 7365 7276 6963 652e 6c61 7374  elf.service.last
-00002c20: 5f70 726f 6475 6374 2829 0a60 6060 0a49  _product().```.I
-00002c30: 6e20 7375 6d6d 6172 792c 2074 6865 2060  n summary, the `
-00002c40: 6465 636f 7261 746f 7273 6020 616e 6420  decorators` and 
-00002c50: 7468 6520 6044 6570 656e 6473 6020 636c  the `Depends` cl
-00002c60: 6173 7320 6172 6520 7573 6564 2074 6f20  ass are used to 
-00002c70: 6465 6669 6e65 2072 6f75 7465 7320 616e  define routes an
-00002c80: 6420 4854 5450 206d 6574 686f 6473 2066  d HTTP methods f
-00002c90: 6f72 2074 6865 0a3c 6272 3e0a 6050 726f  or the.<br>.`Pro
-00002ca0: 6475 6374 7343 6f6e 7472 6f6c 6c65 7260  ductsController`
-00002cb0: 2063 6c61 7373 2c20 616e 6420 746f 2069   class, and to i
-00002cc0: 6e6a 6563 7420 7468 6520 6050 726f 6475  nject the `Produ
-00002cd0: 6374 7353 6572 7669 6365 6020 6465 7065  ctsService` depe
-00002ce0: 6e64 656e 6379 2069 6e74 6f20 7468 6520  ndency into the 
-00002cf0: 7365 7276 6963 6520 6174 7472 6962 7574  service attribut
-00002d00: 6520 6f66 2074 6865 2063 6f6e 7472 6f6c  e of the control
-00002d10: 6c65 722e 0a3c 6272 3e0a 5468 6973 2061  ler..<br>.This a
-00002d20: 6c6c 6f77 7320 7468 6520 636f 6e74 726f  llows the contro
-00002d30: 6c6c 6572 2074 6f20 6861 6e64 6c65 2069  ller to handle i
-00002d40: 6e63 6f6d 696e 6720 7265 7175 6573 7473  ncoming requests
-00002d50: 2061 6e64 2069 6e74 6572 6163 7420 7769   and interact wi
-00002d60: 7468 0a3c 6272 3e0a 5468 6520 7365 7276  th.<br>.The serv
-00002d70: 6963 6520 746f 2070 6572 666f 726d 2073  ice to perform s
-00002d80: 7065 6369 6669 6320 6163 7469 6f6e 7320  pecific actions 
-00002d90: 6261 7365 6420 6f6e 2074 6865 2072 6f75  based on the rou
-00002da0: 7465 7320 616e 6420 6d65 7468 6f64 7320  tes and methods 
-00002db0: 6465 6669 6e65 642e 0a0a 0a23 2323 2320  defined....#### 
-00002dc0: 7072 6f64 7563 7473 5f6d 6f64 756c 652e  products_module.
-00002dd0: 7079 0a0a 6060 6070 7974 686f 6e0a 6672  py..```python.fr
-00002de0: 6f6d 2073 7263 2e70 726f 6475 6374 732e  om src.products.
-00002df0: 7072 6f64 7563 7473 5f63 6f6e 7472 6f6c  products_control
-00002e00: 6c65 7220 696d 706f 7274 2050 726f 6475  ler import Produ
-00002e10: 6374 7343 6f6e 7472 6f6c 6c65 720a 6672  ctsController.fr
-00002e20: 6f6d 2073 7263 2e70 726f 6475 6374 732e  om src.products.
-00002e30: 7072 6f64 7563 7473 5f73 6572 7669 6365  products_service
-00002e40: 2069 6d70 6f72 7420 5072 6f64 7563 7473   import Products
-00002e50: 5365 7276 6963 650a 0a0a 636c 6173 7320  Service...class 
-00002e60: 5072 6f64 7563 7473 4d6f 6475 6c65 3a0a  ProductsModule:.
-00002e70: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00002e80: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00002e90: 2073 656c 662e 7072 6f76 6964 6572 7320   self.providers 
-00002ea0: 3d20 5b50 726f 6475 6374 7353 6572 7669  = [ProductsServi
-00002eb0: 6365 5d0a 2020 2020 2020 2020 7365 6c66  ce].        self
-00002ec0: 2e63 6f6e 7472 6f6c 6c65 7273 203d 205b  .controllers = [
-00002ed0: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
-00002ee0: 6572 5d0a 6060 600a 0a54 6869 7320 6d6f  er].```..This mo
-00002ef0: 6475 6c65 2063 616e 2062 6520 7265 6769  dule can be regi
-00002f00: 7374 6572 6564 2061 6e64 2075 7365 6420  stered and used 
-00002f10: 696e 2079 6f75 7220 6170 706c 6963 6174  in your applicat
-00002f20: 696f 6e2e 204f 6e63 6520 7468 6520 6d6f  ion. Once the mo
-00002f30: 6475 6c65 2069 7320 7265 6769 7374 6572  dule is register
-00002f40: 6564 2c20 7468 6520 636f 6e74 726f 6c6c  ed, the controll
-00002f50: 6572 2072 6f75 7465 7320 7769 6c6c 2062  er routes will b
-00002f60: 6520 6176 6169 6c61 626c 6520 6174 2074  e available at t
-00002f70: 6865 2073 7065 6369 6669 6564 2070 6174  he specified pat
-00002f80: 682e 0a0a 5468 6973 2035 2063 6f6d 706f  h...This 5 compo
-00002f90: 6e65 6e74 7320 6172 6520 7468 6520 6d69  nents are the mi
-00002fa0: 6e69 6d75 6d20 7265 7175 6972 6564 2074  nimum required t
-00002fb0: 6f20 6372 6561 7465 2061 206d 6f64 756c  o create a modul
-00002fc0: 6520 7468 6174 2077 6f72 6b73 2077 6974  e that works wit
-00002fd0: 6820 7468 6520 4f52 4d2e 0a54 6865 7265  h the ORM..There
-00002fe0: 2061 7265 206d 616e 7920 6d6f 7265 206f   are many more o
-00002ff0: 7074 696f 6e73 206f 6620 686f 7720 796f  ptions of how yo
-00003000: 7520 6361 6e20 6465 7369 676e 2079 6f75  u can design you
-00003010: 7220 6d6f 6475 6c65 7320 616e 6420 7768  r modules and wh
-00003020: 6963 6820 6461 7461 6261 7365 7320 796f  ich databases yo
-00003030: 7520 6361 6e20 7573 652c 2062 7574 2074  u can use, but t
-00003040: 6869 7320 6973 2074 6865 2064 6566 6175  his is the defau
-00003050: 6c74 2062 6173 6963 2073 7472 7563 7475  lt basic structu
-00003060: 7265 2e0a 0a23 2320 4b65 7920 4665 6174  re...## Key Feat
-00003070: 7572 6573 0a23 2323 204d 6f64 756c 6172  ures.### Modular
-00003080: 2041 7263 6869 7465 6374 7572 650a 0a50   Architecture..P
-00003090: 794e 6573 7420 666f 6c6c 6f77 7320 7468  yNest follows th
-000030a0: 6520 6d6f 6475 6c61 7220 6172 6368 6974  e modular archit
-000030b0: 6563 7475 7265 206f 6620 4e65 7374 4a53  ecture of NestJS
-000030c0: 2c20 7768 6963 6820 616c 6c6f 7773 2066  , which allows f
-000030d0: 6f72 2065 6173 7920 7365 7061 7261 7469  or easy separati
-000030e0: 6f6e 206f 6620 636f 6e63 6572 6e73 2061  on of concerns a
-000030f0: 6e64 2063 6f64 6520 6f72 6761 6e69 7a61  nd code organiza
-00003100: 7469 6f6e 2e20 4561 6368 206d 6f64 756c  tion. Each modul
-00003110: 6520 636f 6e74 6169 6e73 2061 2063 6f6c  e contains a col
-00003120: 6c65 6374 696f 6e20 6f66 2072 656c 6174  lection of relat
-00003130: 6564 2063 6f6e 7472 6f6c 6c65 7273 2c20  ed controllers, 
-00003140: 7365 7276 6963 6573 2c20 616e 6420 7072  services, and pr
-00003150: 6f76 6964 6572 732e 0a0a 2323 2320 4465  oviders...### De
-00003160: 7065 6e64 656e 6379 2049 6e6a 6563 7469  pendency Injecti
-00003170: 6f6e 0a50 794e 6573 7420 7375 7070 6f72  on.PyNest suppor
-00003180: 7473 2064 6570 656e 6465 6e63 7920 696e  ts dependency in
-00003190: 6a65 6374 696f 6e2c 2077 6869 6368 206d  jection, which m
-000031a0: 616b 6573 2069 7420 6561 7379 2074 6f20  akes it easy to 
-000031b0: 6d61 6e61 6765 2064 6570 656e 6465 6e63  manage dependenc
-000031c0: 6965 7320 616e 6420 7772 6974 6520 7465  ies and write te
-000031d0: 7374 6162 6c65 2063 6f64 652e 2059 6f75  stable code. You
-000031e0: 2063 616e 2065 6173 696c 7920 696e 6a65   can easily inje
-000031f0: 6374 2073 6572 7669 6365 7320 616e 6420  ct services and 
-00003200: 7072 6f76 6964 6572 7320 696e 746f 2079  providers into y
-00003210: 6f75 7220 636f 6e74 726f 6c6c 6572 7320  our controllers 
-00003220: 7573 696e 6720 6465 636f 7261 746f 7273  using decorators
-00003230: 2e0a 0a0a 2323 2320 4465 636f 7261 746f  ....### Decorato
-00003240: 7273 0a0a 5079 4e65 7374 206d 616b 6573  rs..PyNest makes
-00003250: 2065 7874 656e 7369 7665 2075 7365 206f   extensive use o
-00003260: 6620 6465 636f 7261 746f 7273 2074 6f20  f decorators to 
-00003270: 6465 6669 6e65 2072 6f75 7465 732c 206d  define routes, m
-00003280: 6964 646c 6577 6172 652c 2061 6e64 206f  iddleware, and o
-00003290: 7468 6572 2061 7070 6c69 6361 7469 6f6e  ther application
-000032a0: 2063 6f6d 706f 6e65 6e74 732e 2054 6869   components. Thi
-000032b0: 7320 6865 6c70 7320 6b65 6570 2074 6865  s helps keep the
-000032c0: 2063 6f64 6520 636f 6e63 6973 6520 616e   code concise an
-000032d0: 6420 6561 7379 2074 6f20 7265 6164 2e0a  d easy to read..
-000032e0: 0a23 2323 2054 7970 6520 416e 6e6f 7461  .### Type Annota
-000032f0: 7469 6f6e 730a 0a50 794e 6573 7420 6c65  tions..PyNest le
-00003300: 7665 7261 6765 7320 5079 7468 6f6e 2773  verages Python's
-00003310: 2074 7970 6520 616e 6e6f 7461 7469 6f6e   type annotation
-00003320: 7320 746f 2070 726f 7669 6465 2062 6574  s to provide bet
-00003330: 7465 7220 746f 6f6c 696e 6720 616e 6420  ter tooling and 
-00003340: 6865 6c70 2070 7265 7665 6e74 2065 7272  help prevent err
-00003350: 6f72 732e 2059 6f75 2063 616e 2061 6e6e  ors. You can ann
-00003360: 6f74 6174 6520 796f 7572 2063 6f6e 7472  otate your contr
-00003370: 6f6c 6c65 7273 2c20 7365 7276 6963 6573  ollers, services
-00003380: 2c20 616e 6420 7072 6f76 6964 6572 7320  , and providers 
-00003390: 7769 7468 2074 7970 6573 2074 6f20 6d61  with types to ma
-000033a0: 6b65 2079 6f75 7220 636f 6465 206d 6f72  ke your code mor
-000033b0: 6520 726f 6275 7374 2e0a 0a23 2323 2043  e robust...### C
-000033c0: 6f64 6520 4765 6e65 7261 7469 6f6e 0a0a  ode Generation..
-000033d0: 5079 4e65 7374 2069 6e63 6c75 6465 7320  PyNest includes 
-000033e0: 6120 636f 6465 2067 656e 6572 6174 696f  a code generatio
-000033f0: 6e20 746f 6f6c 2074 6861 7420 6361 6e20  n tool that can 
-00003400: 6372 6561 7465 2062 6f69 6c65 7270 6c61  create boilerpla
-00003410: 7465 2063 6f64 6520 666f 7220 6d6f 6475  te code for modu
-00003420: 6c65 732c 2063 6f6e 7472 6f6c 6c65 7273  les, controllers
-00003430: 2c20 616e 6420 6f74 6865 7220 636f 6d70  , and other comp
-00003440: 6f6e 656e 7473 2e20 5468 6973 2073 6176  onents. This sav
-00003450: 6573 2079 6f75 2074 696d 6520 616e 6420  es you time and 
-00003460: 6865 6c70 7320 796f 7520 666f 6375 7320  helps you focus 
-00003470: 6f6e 2077 7269 7469 6e67 2074 6865 2063  on writing the c
-00003480: 6f64 6520 7468 6174 206d 6174 7465 7273  ode that matters
-00003490: 2e0a 0a23 2320 4675 7475 7265 2050 6c61  ...## Future Pla
-000034a0: 6e73 0a0a 2d20 5b20 5d20 4372 6561 7465  ns..- [ ] Create
-000034b0: 204d 6172 6b65 7470 6c61 6365 2066 6f72   Marketplace for
-000034c0: 206d 6f64 756c 6573 2077 6865 7265 2064   modules where d
-000034d0: 6576 656c 6f70 6572 7320 6361 6e20 7368  evelopers can sh
-000034e0: 6172 6520 7468 6569 7220 6d6f 6475 6c65  are their module
-000034f0: 7320 616e 6420 646f 776e 6c6f 6164 206d  s and download m
-00003500: 6f64 756c 6573 2063 7265 6174 6564 2062  odules created b
-00003510: 7920 6f74 6865 7273 2e0a 2d20 5b20 5d20  y others..- [ ] 
-00003520: 4372 6574 6520 4162 7374 7261 6374 696f  Crete Abstractio
-00003530: 6e20 636c 6173 7320 746f 204d 6f64 756c  n class to Modul
-00003540: 6573 2061 6e64 2053 6572 7669 6365 7320  es and Services 
-00003550: 746f 2061 6c6c 6f77 2066 6f72 2065 6173  to allow for eas
-00003560: 7920 6372 6561 7469 6f6e 206f 6620 6d6f  y creation of mo
-00003570: 6475 6c65 7320 616e 6420 7365 7276 6963  dules and servic
-00003580: 6573 2e0a 2d20 5b20 5d20 4164 6420 696e  es..- [ ] Add in
-00003590: 6865 7269 7461 6e63 6520 6265 7477 6565  heritance betwee
-000035a0: 6e20 636f 6e74 726f 6c6c 6572 7320 666f  n controllers fo
-000035b0: 7220 6372 6561 7469 6e67 206d 6f72 6520  r creating more 
-000035c0: 636f 6d70 6c65 7820 636f 6e74 726f 6c6c  complex controll
-000035d0: 6572 732e 0a2d 205b 205d 2041 6464 2073  ers..- [ ] Add s
-000035e0: 7570 706f 7274 2066 6f72 206f 7468 6572  upport for other
-000035f0: 2064 6174 6162 6173 6573 2028 6d6f 6e67   databases (mong
-00003600: 6f44 422c 2072 6564 6973 2c20 6574 632e  oDB, redis, etc.
-00003610: 290a 2d20 5b20 5d20 4372 6561 7465 206f  ).- [ ] Create o
-00003620: 7574 2d6f 662d 7468 652d 626f 7820 6175  ut-of-the-box au
-00003630: 7468 656e 7469 6361 7469 6f6e 206d 6f64  thentication mod
-00003640: 756c 6520 7468 6174 2063 616e 2062 6520  ule that can be 
-00003650: 6561 7369 6c79 2069 6e74 6567 7261 7465  easily integrate
-00003660: 6420 696e 746f 2061 6e79 2061 7070 6c69  d into any appli
-00003670: 6361 7469 6f6e 2e0a 2d20 5b20 5d20 4164  cation..- [ ] Ad
-00003680: 6420 7375 7070 6f72 7420 666f 7220 6f74  d support for ot
-00003690: 6865 7220 7465 7374 696e 6720 6672 616d  her testing fram
-000036a0: 6577 6f72 6b73 2061 6e64 2063 7265 6174  eworks and creat
-000036b0: 6520 7465 7374 696e 6720 7465 6d70 6c61  e testing templa
-000036c0: 7465 732e 0a2d 205b 205d 2041 6464 2073  tes..- [ ] Add s
-000036d0: 7570 706f 7274 2066 6f72 206f 7468 6572  upport for other
-000036e0: 2077 6562 2066 7261 6d65 776f 726b 7320   web frameworks 
-000036f0: 2846 6c61 736b 2c20 446a 616e 676f 2c20  (Flask, Django, 
-00003700: 6574 632e 2920 2d20 5361 6d65 2041 7263  etc.) - Same Arc
-00003710: 6869 7465 6374 7572 652c 2064 6966 6665  hitecture, diffe
-00003720: 7265 6e74 2065 6e67 696e 652e 0a0a 0a23  rent engine....#
-00003730: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-00003740: 436f 6e74 7269 6275 7469 6f6e 7320 6172  Contributions ar
-00003750: 6520 7765 6c63 6f6d 6521 2050 6c65 6173  e welcome! Pleas
-00003760: 6520 6665 656c 2066 7265 6520 746f 2067  e feel free to g
-00003770: 7261 6220 6f6e 6520 6f66 2074 6865 206f  rab one of the o
-00003780: 7065 6e20 6973 7375 6573 2c0a 6f72 206f  pen issues,.or o
-00003790: 7065 6e20 6120 6e65 7720 6f6e 6520 6966  pen a new one if
-000037a0: 2079 6f75 2068 6176 6520 616e 2069 6465   you have an ide
-000037b0: 6120 666f 7220 6120 6e65 7720 6665 6174  a for a new feat
-000037c0: 7572 6520 6f72 2069 6d70 726f 7665 6d65  ure or improveme
-000037d0: 6e74 2e0a 0a54 6869 7320 776f 756c 6420  nt...This would 
-000037e0: 6272 696e 6720 6120 6875 6765 2069 6d70  bring a huge imp
-000037f0: 6163 7420 746f 2074 6865 2070 726f 6a65  act to the proje
-00003800: 6374 2061 6e64 2074 6865 2063 6f6d 6d75  ct and the commu
-00003810: 6e69 7479 2e0a 0a23 2320 4c69 6365 6e73  nity...## Licens
-00003820: 650a 0a50 794e 6573 7420 6973 205b 4d49  e..PyNest is [MI
-00003830: 5420 6c69 6365 6e73 6564 5d28 4c49 4345  T licensed](LICE
-00003840: 4e53 4529 2e0a 0a23 2320 4372 6564 6974  NSE)...## Credit
-00003850: 730a 0a50 794e 6573 7420 6973 2069 6e73  s..PyNest is ins
-00003860: 7069 7265 6420 6279 205b 4e65 7374 4a53  pired by [NestJS
-00003870: 5d28 6874 7470 733a 2f2f 6e65 7374 6a73  ](https://nestjs
-00003880: 2e63 6f6d 2f29 2e0a                      .com/)..
+00000730: 2e31 300a 5265 7175 6972 6573 2d50 7974  .10.Requires-Pyt
+00000740: 686f 6e3a 203e 3d33 2e38 2e31 0a44 6573  hon: >=3.8.1.Des
+00000750: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
+00000760: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
+00000770: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
+00000780: 7472 613a 2074 6573 740a 4c69 6365 6e73  tra: test.Licens
+00000790: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+000007a0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
+000007b0: 7222 3e0a 2020 3c69 6d67 2073 7263 3d22  r">.  <img src="
+000007c0: 646f 6373 2f69 6d67 732f 7079 6e65 7374  docs/imgs/pynest
+000007d0: 5f6c 6f67 6f2d 6d6f 6469 6669 6564 2e70  _logo-modified.p
+000007e0: 6e67 2220 7469 746c 653d 2270 796e 6573  ng" title="pynes
+000007f0: 7420 6c6f 676f 2220 7769 6474 683d 2232  t logo" width="2
+00000800: 3030 223e 0a3c 2f70 3e0a 3c70 2061 6c69  00">.</p>.<p ali
+00000810: 676e 3d22 6365 6e74 6572 223e 0a20 2020  gn="center">.   
+00000820: 203c 656d 3e50 794e 6573 7420 6973 2061   <em>PyNest is a
+00000830: 2050 7974 686f 6e20 6672 616d 6577 6f72   Python framewor
+00000840: 6b20 6275 696c 7420 6f6e 2074 6f70 206f  k built on top o
+00000850: 6620 4661 7374 4150 4920 7468 6174 2066  f FastAPI that f
+00000860: 6f6c 6c6f 7773 2074 6865 206d 6f64 756c  ollows the modul
+00000870: 6172 2061 7263 6869 7465 6374 7572 6520  ar architecture 
+00000880: 6f66 204e 6573 744a 533c 2f65 6d3e 0a3c  of NestJS</em>.<
+00000890: 2f70 3e0a 3c70 2061 6c69 676e 3d22 6365  /p>.<p align="ce
+000008a0: 6e74 6572 223e 0a20 2020 203c 6120 6872  nter">.    <a hr
+000008b0: 6566 3d22 6874 7470 733a 2f2f 7079 7069  ef="https://pypi
+000008c0: 2e6f 7267 2f70 726f 6a65 6374 2f70 796e  .org/project/pyn
+000008d0: 6573 742d 6170 6922 3e0a 2020 2020 2020  est-api">.      
+000008e0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000008f0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000900: 696f 2f70 7970 692f 762f 7079 6e65 7374  io/pypi/v/pynest
+00000910: 2d61 7069 3f63 6f6c 6f72 3d25 3233 3334  -api?color=%2334
+00000920: 4430 3538 266c 6162 656c 3d70 7970 6925  D058&label=pypi%
+00000930: 3230 7061 636b 6167 6522 2061 6c74 3d22  20package" alt="
+00000940: 5665 7273 696f 6e22 3e0a 2020 2020 3c2f  Version">.    </
+00000950: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+00000960: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000970: 2f70 726f 6a65 6374 2f70 796e 6573 742d  /project/pynest-
+00000980: 6170 6922 3e0a 2020 2020 2020 2020 3c69  api">.        <i
+00000990: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+000009a0: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+000009b0: 7970 692f 7079 7665 7273 696f 6e73 2f70  ypi/pyversions/p
+000009c0: 796e 6573 742d 6170 692e 7376 673f 636f  ynest-api.svg?co
+000009d0: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
+000009e0: 6c74 3d22 5079 7468 6f6e 223e 0a20 2020  lt="Python">.   
+000009f0: 203c 2f61 3e0a 2020 2020 3c61 2068 7265   </a>.    <a hre
+00000a00: 663d 2268 7474 7073 3a2f 2f70 6570 792e  f="https://pepy.
+00000a10: 7465 6368 2f70 726f 6a65 6374 2f70 796e  tech/project/pyn
+00000a20: 6573 742d 6170 6922 3e0a 2020 2020 2020  est-api">.      
+00000a30: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000a40: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
+00000a50: 7465 6368 2f70 6572 736f 6e61 6c69 7a65  tech/personalize
+00000a60: 642d 6261 6467 652f 7079 6e65 7374 2d61  d-badge/pynest-a
+00000a70: 7069 3f70 6572 696f 643d 6d6f 6e74 6826  pi?period=month&
+00000a80: 756e 6974 733d 696e 7465 726e 6174 696f  units=internatio
+00000a90: 6e61 6c5f 7379 7374 656d 266c 6566 745f  nal_system&left_
+00000aa0: 636f 6c6f 723d 6772 6579 2672 6967 6874  color=grey&right
+00000ab0: 5f63 6f6c 6f72 3d62 7269 6768 7467 7265  _color=brightgre
+00000ac0: 656e 266c 6566 745f 7465 7874 3d44 6f77  en&left_text=Dow
+00000ad0: 6e6c 6f61 6473 2220 616c 743d 2244 6f77  nloads" alt="Dow
+00000ae0: 6e6c 6f61 6473 223e 0a20 2020 203c 2f61  nloads">.    </a
+00000af0: 3e0a 2020 2020 3c61 2068 7265 663d 2268  >.    <a href="h
+00000b00: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000b10: 6d2f 5079 7468 6f6e 4e65 7374 2f50 794e  m/PythonNest/PyN
+00000b20: 6573 742f 626c 6f62 2f6d 6169 6e2f 4c49  est/blob/main/LI
+00000b30: 4345 4e53 4522 3e0a 2020 2020 2020 2020  CENSE">.        
+00000b40: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00000b50: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000b60: 2f67 6974 6875 622f 6c69 6365 6e73 652f  /github/license/
+00000b70: 5079 7468 6f6e 4e65 7374 2f50 796e 6573  PythonNest/Pynes
+00000b80: 7422 2061 6c74 3d22 4c69 6365 6e73 6522  t" alt="License"
+00000b90: 3e0a 2020 2020 3c2f 613e 0a3c 2f70 3e0a  >.    </a>.</p>.
+00000ba0: 0a0a 2320 4465 7363 7269 7074 696f 6e0a  ..# Description.
+00000bb0: 0a50 794e 6573 7420 6973 2064 6573 6967  .PyNest is desig
+00000bc0: 6e65 6420 746f 2068 656c 7020 7374 7275  ned to help stru
+00000bd0: 6374 7572 6520 796f 7572 2041 5049 7320  cture your APIs 
+00000be0: 696e 2061 6e20 696e 7475 6974 6976 652c  in an intuitive,
+00000bf0: 2065 6173 7920 746f 2075 6e64 6572 7374   easy to underst
+00000c00: 616e 642c 2061 6e64 2065 6e6a 6f79 6162  and, and enjoyab
+00000c10: 6c65 2077 6179 2e0a 0a57 6974 6820 5079  le way...With Py
+00000c20: 4e65 7374 2c20 796f 7520 6361 6e20 6275  Nest, you can bu
+00000c30: 696c 6420 7363 616c 6162 6c65 2061 6e64  ild scalable and
+00000c40: 206d 6169 6e74 6169 6e61 626c 6520 4150   maintainable AP
+00000c50: 4973 2077 6974 6820 6561 7365 2e20 5468  Is with ease. Th
+00000c60: 6520 6672 616d 6577 6f72 6b20 7375 7070  e framework supp
+00000c70: 6f72 7473 2064 6570 656e 6465 6e63 7920  orts dependency 
+00000c80: 696e 6a65 6374 696f 6e2c 2074 7970 6520  injection, type 
+00000c90: 616e 6e6f 7461 7469 6f6e 732c 2064 6563  annotations, dec
+00000ca0: 6f72 6174 6f72 732c 2061 6e64 2063 6f64  orators, and cod
+00000cb0: 6520 6765 6e65 7261 7469 6f6e 2c20 6d61  e generation, ma
+00000cc0: 6b69 6e67 2069 7420 6561 7379 2074 6f20  king it easy to 
+00000cd0: 7772 6974 6520 636c 6561 6e20 616e 6420  write clean and 
+00000ce0: 7465 7374 6162 6c65 2063 6f64 652e 0a0a  testable code...
+00000cf0: 5468 6973 2066 7261 6d65 776f 726b 2069  This framework i
+00000d00: 7320 6e6f 7420 6120 6469 7265 6374 2070  s not a direct p
+00000d10: 6f72 7420 6f66 204e 6573 744a 5320 746f  ort of NestJS to
+00000d20: 2050 7974 686f 6e20 6275 7420 7261 7468   Python but rath
+00000d30: 6572 2061 2072 652d 696d 6167 696e 696e  er a re-imaginin
+00000d40: 6720 6f66 2074 6865 2066 7261 6d65 776f  g of the framewo
+00000d50: 726b 2073 7065 6369 6669 6361 6c6c 7920  rk specifically 
+00000d60: 666f 7220 5079 7468 6f6e 2064 6576 656c  for Python devel
+00000d70: 6f70 6572 732c 2069 6e63 6c75 6469 6e67  opers, including
+00000d80: 2064 6174 6120 7363 6965 6e74 6973 7473   data scientists
+00000d90: 2c20 6461 7461 2061 6e61 6c79 7374 732c  , data analysts,
+00000da0: 2061 6e64 2064 6174 6120 656e 6769 6e65   and data engine
+00000db0: 6572 732e 2049 7420 6169 6d73 2074 6f20  ers. It aims to 
+00000dc0: 6173 7369 7374 2074 6865 6d20 696e 2062  assist them in b
+00000dd0: 7569 6c64 696e 6720 6265 7474 6572 2061  uilding better a
+00000de0: 6e64 2066 6173 7465 7220 4150 4973 2066  nd faster APIs f
+00000df0: 6f72 2074 6865 6972 2064 6174 6120 6170  or their data ap
+00000e00: 706c 6963 6174 696f 6e73 2e0a 0a23 2320  plications...## 
+00000e10: 4765 7474 696e 6720 5374 6172 7465 640a  Getting Started.
+00000e20: 546f 2067 6574 2073 7461 7274 6564 2077  To get started w
+00000e30: 6974 6820 5079 4e65 7374 2c20 796f 7527  ith PyNest, you'
+00000e40: 6c6c 206e 6565 6420 746f 2069 6e73 7461  ll need to insta
+00000e50: 6c6c 2069 7420 7573 696e 6720 7069 703a  ll it using pip:
+00000e60: 0a0a 6060 6062 6173 680a 7069 7020 696e  ..```bash.pip in
+00000e70: 7374 616c 6c20 7079 6e65 7374 2d61 7069  stall pynest-api
+00000e80: 0a60 6060 0a0a 2323 2320 5374 6172 7420  .```..### Start 
+00000e90: 7769 7468 2063 6c69 0a60 6060 6261 7368  with cli.```bash
+00000ea0: 0a70 796e 6573 7420 6372 6561 7465 2d6e  .pynest create-n
+00000eb0: 6573 742d 6170 7020 2d6e 206d 795f 6170  est-app -n my_ap
+00000ec0: 705f 6e61 6d65 0a60 6060 0a0a 7468 6973  p_name.```..this
+00000ed0: 2063 6f6d 6d61 6e64 2077 696c 6c20 6372   command will cr
+00000ee0: 6561 7465 2061 206e 6577 2070 726f 6a65  eate a new proje
+00000ef0: 6374 2077 6974 6820 7468 6520 666f 6c6c  ct with the foll
+00000f00: 6f77 696e 6720 7374 7275 6374 7572 653a  owing structure:
+00000f10: 0a0a 6060 6074 6578 740a e294 9ce2 9480  ..```text.......
+00000f20: e294 8020 6170 702e 7079 0ae2 949c e294  ... app.py......
+00000f30: 80e2 9480 206f 726d 5f63 6f6e 6669 672e  .... orm_config.
+00000f40: 7079 0ae2 949c e294 80e2 9480 206d 6169  py.......... mai
+00000f50: 6e2e 7079 0ae2 949c e294 80e2 9480 2073  n.py.......... s
+00000f60: 7263 0ae2 9482 2020 2020 e294 9ce2 9480  rc....    ......
+00000f70: e294 8020 5f5f 696e 6974 5f5f 2e70 790a  ... __init__.py.
+00000f80: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00000f90: 2065 7861 6d70 6c65 730a e294 8220 2020   examples....   
+00000fa0: 20e2 9482 2020 2020 e294 9ce2 9480 e294   ...    ........
+00000fb0: 8020 5f5f 696e 6974 5f5f 2e70 790a e294  . __init__.py...
+00000fc0: 8220 2020 20e2 9482 2020 2020 e294 9ce2  .    ...    ....
+00000fd0: 9480 e294 8020 6578 616d 706c 6573 5f63  ..... examples_c
+00000fe0: 6f6e 7472 6f6c 6c65 722e 7079 0ae2 9482  ontroller.py....
+00000ff0: 2020 2020 e294 8220 2020 20e2 949c e294      ...    .....
+00001000: 80e2 9480 2065 7861 6d70 6c65 735f 7365  .... examples_se
+00001010: 7276 6963 652e 7079 0ae2 9482 2020 2020  rvice.py....    
+00001020: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001030: 2065 7861 6d70 6c65 735f 6d6f 6465 6c2e   examples_model.
+00001040: 7079 0ae2 9482 2020 2020 e294 9ce2 9480  py....    ......
+00001050: e294 8020 20e2 949c e294 80e2 9480 2065  ...  ......... e
+00001060: 7861 6d70 6c65 735f 656e 7469 7479 2e70  xamples_entity.p
+00001070: 790a e294 8220 2020 20e2 949c e294 80e2  y....    .......
+00001080: 9480 2020 e294 9ce2 9480 e294 8020 6578  ..  ......... ex
+00001090: 616d 706c 6573 5f6d 6f64 756c 652e 7079  amples_module.py
+000010a0: 0a60 6060 0a0a 6f6e 6365 2079 6f75 2068  .```..once you h
+000010b0: 6176 6520 6372 6561 7465 6420 796f 7572  ave created your
+000010c0: 2061 7070 2c20 6765 7420 696e 746f 2074   app, get into t
+000010d0: 6865 2066 6f6c 6465 7220 616e 6420 7275  he folder and ru
+000010e0: 6e20 7468 6520 666f 6c6c 6f77 696e 6720  n the following 
+000010f0: 636f 6d6d 616e 643a 0a0a 6060 6062 6173  command:..```bas
+00001100: 680a 6364 206d 795f 6170 705f 6e61 6d65  h.cd my_app_name
+00001110: 0a60 6060 0a0a 7275 6e20 7468 6520 7365  .```..run the se
+00001120: 7276 6572 2077 6974 6820 7468 6520 666f  rver with the fo
+00001130: 6c6c 6f77 696e 6720 636f 6d6d 616e 643a  llowing command:
+00001140: 0a0a 6060 6062 6173 680a 7576 6963 6f72  ..```bash.uvicor
+00001150: 6e20 2261 7070 3a61 7070 2220 2d2d 686f  n "app:app" --ho
+00001160: 7374 2022 302e 302e 302e 3022 202d 2d70  st "0.0.0.0" --p
+00001170: 6f72 7420 2238 3022 202d 2d72 656c 6f61  ort "80" --reloa
+00001180: 640a 6060 600a 0a4e 6f77 2079 6f75 2063  d.```..Now you c
+00001190: 616e 2076 6973 6974 205b 4f70 656e 4150  an visit [OpenAP
+000011a0: 495d 2868 7474 703a 2f2f 6c6f 6361 6c68  I](http://localh
+000011b0: 6f73 743a 3830 2f64 6f63 7329 2069 6e20  ost:80/docs) in 
+000011c0: 796f 7572 2062 726f 7773 6572 2074 6f20  your browser to 
+000011d0: 7365 6520 7468 6520 6465 6661 756c 7420  see the default 
+000011e0: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
+000011f0: 6e2e 0a0a 2323 2320 4164 6469 6e67 206d  n...### Adding m
+00001200: 6f64 756c 6573 0a0a 546f 2061 6464 2061  odules..To add a
+00001210: 206e 6577 206d 6f64 756c 6520 746f 2079   new module to y
+00001220: 6f75 7220 6170 706c 6963 6174 696f 6e2c  our application,
+00001230: 2079 6f75 2063 616e 2075 7365 2074 6865   you can use the
+00001240: 2070 796e 6573 7420 6765 6e65 7261 7465   pynest generate
+00001250: 206d 6f64 756c 6520 636f 6d6d 616e 643a   module command:
+00001260: 0a0a 6060 6062 6173 680a 7079 6e65 7374  ..```bash.pynest
+00001270: 2067 656e 6572 6174 652d 6d6f 6475 6c65   generate-module
+00001280: 202d 6e20 7573 6572 730a 6060 600a 0a54   -n users.```..T
+00001290: 6869 7320 7769 6c6c 2063 7265 6174 6520  his will create 
+000012a0: 6120 6e65 7720 6d6f 6475 6c65 2063 616c  a new module cal
+000012b0: 6c65 6420 6060 6075 7365 7273 6060 6020  led ```users``` 
+000012c0: 696e 2079 6f75 7220 6170 706c 6963 6174  in your applicat
+000012d0: 696f 6e20 7769 7468 2074 6865 2066 6f6c  ion with the fol
+000012e0: 6c6f 7769 6e67 2073 7472 7563 7475 7265  lowing structure
+000012f0: 3a0a 0a60 6060 7465 7874 0ae2 949c e294  :..```text......
+00001300: 80e2 9480 2075 7365 7273 0ae2 9482 2020  .... users....  
+00001310: 2020 e294 9ce2 9480 e294 8020 5f5f 696e    ......... __in
+00001320: 6974 5f5f 2e70 790a e294 8220 2020 20e2  it__.py....    .
+00001330: 949c e294 80e2 9480 2075 7365 7273 5f63  ........ users_c
+00001340: 6f6e 7472 6f6c 6c65 722e 7079 0ae2 9482  ontroller.py....
+00001350: 2020 2020 e294 9ce2 9480 e294 8020 7573      ......... us
+00001360: 6572 735f 7365 7276 6963 652e 7079 0ae2  ers_service.py..
+00001370: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+00001380: 7573 6572 735f 6d6f 6465 6c2e 7079 0ae2  users_model.py..
+00001390: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+000013a0: 7573 6572 735f 656e 7469 7479 2e70 790a  users_entity.py.
+000013b0: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+000013c0: 2075 7365 7273 5f6d 6f64 756c 652e 7079   users_module.py
+000013d0: 0a60 6060 0a0a 5468 6520 7573 6572 7320  .```..The users 
+000013e0: 6d6f 6475 6c65 2077 696c 6c20 696d 6d65  module will imme
+000013f0: 6469 6174 656c 7920 7265 6769 7374 6572  diately register
+00001400: 2069 7473 656c 6620 7769 7468 2074 6865   itself with the
+00001410: 2061 7070 6c69 6361 7469 6f6e 2061 6e64   application and
+00001420: 2077 696c 6c20 6265 2061 7661 696c 6162   will be availab
+00001430: 6c65 2066 6f72 2075 7365 2e0a 0a59 6f75  le for use...You
+00001440: 2063 616e 2074 6865 6e20 7374 6172 7420   can then start 
+00001450: 6465 6669 6e69 6e67 2072 6f75 7465 7320  defining routes 
+00001460: 616e 6420 6f74 6865 7220 6170 706c 6963  and other applic
+00001470: 6174 696f 6e20 636f 6d70 6f6e 656e 7473  ation components
+00001480: 2075 7369 6e67 2064 6563 6f72 6174 6f72   using decorator
+00001490: 7320 616e 6420 6f74 6865 7220 5079 4e65  s and other PyNe
+000014a0: 7374 2063 6f6e 7374 7275 6374 732e 0a0a  st constructs...
+000014b0: 466f 7220 6d6f 7265 2069 6e66 6f72 6d61  For more informa
+000014c0: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
+000014d0: 7365 2050 794e 6573 742c 2063 6865 636b  se PyNest, check
+000014e0: 206f 7574 2074 6865 206f 6666 6963 6961   out the officia
+000014f0: 6c20 646f 6375 6d65 6e74 6174 696f 6e20  l documentation 
+00001500: 6174 2068 7474 7073 3a2f 2f70 7974 686f  at https://pytho
+00001510: 6e6e 6573 742e 6769 7468 7562 2e69 6f2f  nnest.github.io/
+00001520: 5079 4e65 7374 2f2e 0a0a 2323 2053 7461  PyNest/...## Sta
+00001530: 7274 696e 6720 6120 6e65 7720 7072 6f6a  rting a new proj
+00001540: 6563 7420 6d61 6e75 616c 6c79 0a0a 6060  ect manually..``
+00001550: 6074 6578 740a 4e4f 5449 4345 3a20 666f  `text.NOTICE: fo
+00001560: 7220 7468 6520 666f 6c6c 6f77 696e 6720  r the following 
+00001570: 6578 616d 706c 652c 2077 6520 7769 6c6c  example, we will
+00001580: 2075 7365 2074 6865 2070 726f 6475 6374   use the product
+00001590: 7320 6d6f 6475 6c65 2e20 0a60 6060 0a0a  s module. .```..
+000015a0: 546f 2073 7461 7274 2061 206e 6577 2070  To start a new p
+000015b0: 726f 6a65 6374 206d 616e 7561 6c6c 792c  roject manually,
+000015c0: 2079 6f75 276c 6c20 6e65 6564 2074 6f20   you'll need to 
+000015d0: 6372 6561 7465 2061 2070 726f 6a65 6374  create a project
+000015e0: 2074 6861 7420 666f 6c6c 6f77 7320 7468   that follows th
+000015f0: 6973 2073 7472 7563 7475 7265 3a0a 0a60  is structure:..`
+00001600: 6060 7465 7874 0ae2 949c e294 80e2 9480  ``text..........
+00001610: 2061 7070 2e70 790a e294 9ce2 9480 e294   app.py.........
+00001620: 8020 6f72 6d5f 636f 6e66 6967 2e70 790a  . orm_config.py.
+00001630: e294 9ce2 9480 e294 8020 6d61 696e 2e70  ......... main.p
+00001640: 790a e294 9ce2 9480 e294 8020 7372 630a  y.......... src.
+00001650: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001660: 205f 5f69 6e69 745f 5f2e 7079 0ae2 9482   __init__.py....
+00001670: 2020 2020 e294 9ce2 9480 e294 8020 7072      ......... pr
+00001680: 6f64 7563 7473 0ae2 9482 2020 2020 e294  oducts....    ..
+00001690: 8220 2020 20e2 949c e294 80e2 9480 205f  .    ......... _
+000016a0: 5f69 6e69 745f 5f2e 7079 0ae2 9482 2020  _init__.py....  
+000016b0: 2020 e294 8220 2020 20e2 949c e294 80e2    ...    .......
+000016c0: 9480 2070 726f 6475 6374 735f 636f 6e74  .. products_cont
+000016d0: 726f 6c6c 6572 2e70 790a e294 8220 2020  roller.py....   
+000016e0: 20e2 9482 2020 2020 e294 9ce2 9480 e294   ...    ........
+000016f0: 8020 7072 6f64 7563 7473 5f73 6572 7669  . products_servi
+00001700: 6365 2e70 790a e294 8220 2020 20e2 9482  ce.py....    ...
+00001710: 2020 2020 e294 9ce2 9480 e294 8020 7072      ......... pr
+00001720: 6f64 7563 7473 5f6d 6f64 656c 2e70 790a  oducts_model.py.
+00001730: e294 8220 2020 20e2 949c e294 80e2 9480  ...    .........
+00001740: 2020 e294 9ce2 9480 e294 8020 7072 6f64    ......... prod
+00001750: 7563 7473 5f65 6e74 6974 792e 7079 0ae2  ucts_entity.py..
+00001760: 9482 2020 2020 e294 9ce2 9480 e294 8020  ..    ......... 
+00001770: 20e2 949c e294 80e2 9480 2070 726f 6475   ......... produ
+00001780: 6374 735f 6d6f 6475 6c65 2e70 790a 6060  cts_module.py.``
+00001790: 600a 0a45 7870 6c61 6e61 7469 6f6e 3a20  `..Explanation: 
+000017a0: 5468 6973 2069 7320 7468 6520 6469 7265  This is the dire
+000017b0: 6374 6f72 7920 7374 7275 6374 7572 6520  ctory structure 
+000017c0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
+000017d0: 2e20 4974 2069 6e63 6c75 6465 7320 7468  . It includes th
+000017e0: 6520 6d61 696e 2066 696c 6573 2061 6e64  e main files and
+000017f0: 2061 2073 7263 2064 6972 6563 746f 7279   a src directory
+00001800: 2074 6861 7420 636f 6e74 6169 6e73 2079   that contains y
+00001810: 6f75 7220 7072 6f6a 6563 7427 7320 736f  our project's so
+00001820: 7572 6365 2063 6f64 652e 0a0a 2323 2320  urce code...### 
+00001830: 4372 6561 7469 6e67 2074 6865 2066 696c  Creating the fil
+00001840: 6573 0a0a 2323 2323 206d 6169 6e2e 7079  es..#### main.py
+00001850: 0a60 6060 7079 7468 6f6e 0a69 6d70 6f72  .```python.impor
+00001860: 7420 7576 6963 6f72 6e0a 0a0a 6966 205f  t uvicorn...if _
+00001870: 5f6e 616d 655f 5f20 3d3d 2027 5f5f 6d61  _name__ == '__ma
+00001880: 696e 5f5f 273a 0a20 2020 2075 7669 636f  in__':.    uvico
+00001890: 726e 2e72 756e 280a 2020 2020 2020 2020  rn.run(.        
+000018a0: 2761 7070 3a61 7070 272c 0a20 2020 2020  'app:app',.     
+000018b0: 2020 2068 6f73 743d 2230 2e30 2e30 2e30     host="0.0.0.0
+000018c0: 222c 0a20 2020 2020 2020 2070 6f72 743d  ",.        port=
+000018d0: 3830 2c0a 2020 2020 290a 6060 600a 0a54  80,.    ).```..T
+000018e0: 6869 7320 6973 2074 6865 206d 6169 6e2e  his is the main.
+000018f0: 7079 2066 696c 652c 2077 6869 6368 2069  py file, which i
+00001900: 7320 7265 7370 6f6e 7369 626c 6520 666f  s responsible fo
+00001910: 7220 7275 6e6e 696e 6720 796f 7572 2061  r running your a
+00001920: 7070 6c69 6361 7469 6f6e 2075 7369 6e67  pplication using
+00001930: 2074 6865 2055 7669 636f 726e 2073 6572   the Uvicorn ser
+00001940: 7665 722e 0a3c 6272 3e0a 4974 2069 6d70  ver..<br>.It imp
+00001950: 6f72 7473 2074 6865 2075 7669 636f 726e  orts the uvicorn
+00001960: 206c 6962 7261 7279 2061 6e64 2073 7461   library and sta
+00001970: 7274 7320 7468 6520 7365 7276 6572 2077  rts the server w
+00001980: 6974 6820 7468 6520 7370 6563 6966 6965  ith the specifie
+00001990: 6420 686f 7374 2061 6e64 2070 6f72 742e  d host and port.
+000019a0: 0a0a 0a23 2323 2320 6170 702e 7079 0a0a  ...#### app.py..
+000019b0: 6060 6070 7974 686f 6e0a 6672 6f6d 206f  ```python.from o
+000019c0: 726d 5f63 6f6e 6669 6720 696d 706f 7274  rm_config import
+000019d0: 2063 6f6e 6669 670a 6672 6f6d 206e 6573   config.from nes
+000019e0: 742e 636f 7265 2069 6d70 6f72 7420 4170  t.core import Ap
+000019f0: 700a 6672 6f6d 2073 7263 2e70 726f 6475  p.from src.produ
+00001a00: 6374 732e 7072 6f64 7563 7473 5f6d 6f64  cts.products_mod
+00001a10: 756c 6520 696d 706f 7274 2050 726f 6475  ule import Produ
+00001a20: 6374 734d 6f64 756c 650a 0a61 7070 203d  ctsModule..app =
+00001a30: 2041 7070 280a 2020 2020 6465 7363 7269   App(.    descri
+00001a40: 7074 696f 6e3d 2259 6f75 7220 6170 7020  ption="Your app 
+00001a50: 6465 7363 7269 7074 696f 6e22 2c0a 2020  description",.  
+00001a60: 2020 6d6f 6475 6c65 733d 5b0a 2020 2020    modules=[.    
+00001a70: 2020 2020 5072 6f64 7563 7473 4d6f 6475      ProductsModu
+00001a80: 6c65 0a20 2020 205d 2c0a 2020 2020 696e  le.    ],.    in
+00001a90: 6974 5f64 623d 636f 6e66 6967 2e63 7265  it_db=config.cre
+00001aa0: 6174 655f 616c 6c0a 290a 6060 600a 0a54  ate_all.).```..T
+00001ab0: 6869 7320 6973 2074 6865 2061 7070 2e70  his is the app.p
+00001ac0: 7920 6669 6c65 2c20 7768 6963 6820 6973  y file, which is
+00001ad0: 2074 6865 2065 6e74 7279 2070 6f69 6e74   the entry point
+00001ae0: 2066 6f72 2079 6f75 7220 6170 706c 6963   for your applic
+00001af0: 6174 696f 6e2e 2049 7420 696d 706f 7274  ation. It import
+00001b00: 7320 6e65 6365 7373 6172 7920 6d6f 6475  s necessary modu
+00001b10: 6c65 7320 616e 6420 7365 7473 2075 7020  les and sets up 
+00001b20: 7468 6520 4170 7020 6f62 6a65 6374 2077  the App object w
+00001b30: 6974 6820 6120 6465 7363 7269 7074 696f  ith a descriptio
+00001b40: 6e20 616e 6420 7468 6520 5072 6f64 7563  n and the Produc
+00001b50: 7473 4d6f 6475 6c65 2e0a 3c62 723e 0a49  tsModule..<br>.I
+00001b60: 7420 616c 736f 2069 6e69 7469 616c 697a  t also initializ
+00001b70: 6573 2074 6865 2064 6174 6162 6173 6520  es the database 
+00001b80: 7573 696e 6720 7468 6520 636f 6e66 6967  using the config
+00001b90: 2e63 7265 6174 655f 616c 6c20 6675 6e63  .create_all func
+00001ba0: 7469 6f6e 2e0a 0a23 2323 2320 6f72 6d5f  tion...#### orm_
+00001bb0: 636f 6e66 6967 2e70 790a 6060 6070 7974  config.py.```pyt
+00001bc0: 686f 6e0a 6672 6f6d 206e 6573 742e 636f  hon.from nest.co
+00001bd0: 7265 2069 6d70 6f72 7420 4f72 6d53 6572  re import OrmSer
+00001be0: 7669 6365 0a69 6d70 6f72 7420 6f73 0a66  vice.import os.f
+00001bf0: 726f 6d20 646f 7465 6e76 2069 6d70 6f72  rom dotenv impor
+00001c00: 7420 6c6f 6164 5f64 6f74 656e 760a 0a6c  t load_dotenv..l
+00001c10: 6f61 645f 646f 7465 6e76 2829 0a0a 636f  oad_dotenv()..co
+00001c20: 6e66 6967 203d 204f 726d 5365 7276 6963  nfig = OrmServic
+00001c30: 6528 0a20 2020 2064 625f 7479 7065 3d22  e(.    db_type="
+00001c40: 796f 7572 5f64 625f 7479 7065 222c 0a20  your_db_type",. 
+00001c50: 2020 2063 6f6e 6669 675f 7061 7261 6d73     config_params
+00001c60: 3d64 6963 7428 0a20 2020 2020 2020 2075  =dict(.        u
+00001c70: 7365 723d 6f73 2e67 6574 656e 7628 2244  ser=os.getenv("D
+00001c80: 425f 5553 4552 2229 2c0a 2020 2020 2020  B_USER"),.      
+00001c90: 2020 7061 7373 776f 7264 3d6f 732e 6765    password=os.ge
+00001ca0: 7465 6e76 2822 4442 5f50 4153 5357 4f52  tenv("DB_PASSWOR
+00001cb0: 4422 292c 0a20 2020 2020 2020 2068 6f73  D"),.        hos
+00001cc0: 743d 6f73 2e67 6574 656e 7628 2244 425f  t=os.getenv("DB_
+00001cd0: 484f 5354 2229 2c0a 2020 2020 2020 2020  HOST"),.        
+00001ce0: 706f 7274 3d6f 732e 6765 7465 6e76 2822  port=os.getenv("
+00001cf0: 4442 5f50 4f52 5422 292c 0a20 2020 2020  DB_PORT"),.     
+00001d00: 2020 2064 6174 6162 6173 653d 6f73 2e67     database=os.g
+00001d10: 6574 656e 7628 2244 425f 4e41 4d45 2229  etenv("DB_NAME")
+00001d20: 2c0a 2020 2020 292c 0a29 0a60 6060 0a0a  ,.    ),.).```..
+00001d30: 5468 6973 2069 7320 7468 6520 6f72 6d5f  This is the orm_
+00001d40: 636f 6e66 6967 2e70 7920 6669 6c65 2c20  config.py file, 
+00001d50: 7768 6963 6820 636f 6e74 6169 6e73 2074  which contains t
+00001d60: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+00001d70: 2066 6f72 2079 6f75 7220 4f52 4d20 284f   for your ORM (O
+00001d80: 626a 6563 742d 5265 6c61 7469 6f6e 616c  bject-Relational
+00001d90: 204d 6170 7069 6e67 2920 7365 7276 6963   Mapping) servic
+00001da0: 652e 0a0a 4974 2069 6d70 6f72 7473 206e  e...It imports n
+00001db0: 6563 6573 7361 7279 206c 6962 7261 7269  ecessary librari
+00001dc0: 6573 2c20 6c6f 6164 7320 656e 7669 726f  es, loads enviro
+00001dd0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
+00001de0: 7573 696e 6720 646f 7465 6e76 2c20 616e  using dotenv, an
+00001df0: 6420 6372 6561 7465 7320 616e 204f 726d  d creates an Orm
+00001e00: 5365 7276 6963 6520 6f62 6a65 6374 2077  Service object w
+00001e10: 6974 6820 7468 6520 7370 6563 6966 6965  ith the specifie
+00001e20: 6420 6461 7461 6261 7365 2074 7970 6520  d database type 
+00001e30: 616e 6420 636f 6e66 6967 7572 6174 696f  and configuratio
+00001e40: 6e20 7061 7261 6d65 7465 7273 2e0a 0a2d  n parameters...-
+00001e50: 2d2d 0a0a 4f6e 6365 2077 6520 7365 7420  --..Once we set 
+00001e60: 7570 2074 6869 7320 3320 6669 6c65 732c  up this 3 files,
+00001e70: 2077 6520 6361 6e20 7374 6172 7420 6372   we can start cr
+00001e80: 6561 7469 6e67 206f 7572 206d 6f64 756c  eating our modul
+00001e90: 6573 2e20 6561 6368 206d 6f64 756c 6520  es. each module 
+00001ea0: 6973 2061 2066 6f6c 6465 7220 7769 7468  is a folder with
+00001eb0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2073   the following s
+00001ec0: 7472 7563 7475 7265 3a0a 0a60 6060 7465  tructure:..```te
+00001ed0: 7874 200a e294 9ce2 9480 e294 8020 7072  xt .......... pr
+00001ee0: 6f64 7563 7473 0ae2 9482 2020 2020 e294  oducts....    ..
+00001ef0: 9ce2 9480 e294 8020 5f5f 696e 6974 5f5f  ....... __init__
+00001f00: 2e70 790a e294 8220 2020 20e2 949c e294  .py....    .....
+00001f10: 80e2 9480 2070 726f 6475 6374 735f 636f  .... products_co
+00001f20: 6e74 726f 6c6c 6572 2e70 790a e294 8220  ntroller.py.... 
+00001f30: 2020 20e2 949c e294 80e2 9480 2070 726f     ......... pro
+00001f40: 6475 6374 735f 7365 7276 6963 652e 7079  ducts_service.py
+00001f50: 0ae2 9482 2020 2020 e294 9ce2 9480 e294  ....    ........
+00001f60: 8020 7072 6f64 7563 7473 5f6d 6f64 656c  . products_model
+00001f70: 2e70 790a 7c20 2020 20e2 949c e294 80e2  .py.|    .......
+00001f80: 9480 2070 726f 6475 6374 735f 656e 7469  .. products_enti
+00001f90: 7479 2e70 790a e294 8220 2020 20e2 949c  ty.py....    ...
+00001fa0: e294 80e2 9480 2070 726f 6475 6374 735f  ...... products_
+00001fb0: 6d6f 6475 6c65 2e70 790a 6060 600a 0a54  module.py.```..T
+00001fc0: 6869 7320 6973 2074 6865 2073 7472 7563  his is the struc
+00001fd0: 7475 7265 206f 6620 6120 6d6f 6475 6c65  ture of a module
+00001fe0: 2066 6f6c 6465 722e 2049 7420 696e 636c   folder. It incl
+00001ff0: 7564 6573 2061 6e20 5f5f 696e 6974 5f5f  udes an __init__
+00002000: 2e70 7920 6669 6c65 2074 6f20 6d61 6b65  .py file to make
+00002010: 2074 6865 2066 6f6c 6465 7220 6120 5079   the folder a Py
+00002020: 7468 6f6e 2070 6163 6b61 6765 2c0a 3c62  thon package,.<b
+00002030: 723e 0a41 7320 7765 6c6c 2061 7320 7370  r>.As well as sp
+00002040: 6563 6966 6963 2066 696c 6573 2066 6f72  ecific files for
+00002050: 2074 6865 206d 6f64 756c 6527 7320 636f   the module's co
+00002060: 6e74 726f 6c6c 6572 2c20 7365 7276 6963  ntroller, servic
+00002070: 652c 206d 6f64 656c 2c20 656e 7469 7479  e, model, entity
+00002080: 2c20 616e 6420 6d6f 6475 6c65 2063 6f6e  , and module con
+00002090: 6669 6775 7261 7469 6f6e 732e 0a0a 2323  figurations...##
+000020a0: 2323 2070 726f 6475 6374 735f 6d6f 6465  ## products_mode
+000020b0: 6c2e 7079 0a60 6060 7079 7468 6f6e 0a66  l.py.```python.f
+000020c0: 726f 6d20 7079 6461 6e74 6963 2069 6d70  rom pydantic imp
+000020d0: 6f72 7420 4261 7365 4d6f 6465 6c0a 0a0a  ort BaseModel...
+000020e0: 636c 6173 7320 5072 6f64 7563 7428 4261  class Product(Ba
+000020f0: 7365 4d6f 6465 6c29 3a0a 2020 2020 6e61  seModel):.    na
+00002100: 6d65 3a20 7374 720a 2020 2020 7072 6963  me: str.    pric
+00002110: 653a 2066 6c6f 6174 0a20 2020 2064 6573  e: float.    des
+00002120: 6372 6970 7469 6f6e 3a20 7374 720a 6060  cription: str.``
+00002130: 600a 0a54 6869 7320 6973 2074 6865 2070  `..This is the p
+00002140: 726f 6475 6374 735f 6d6f 6465 6c2e 7079  roducts_model.py
+00002150: 2066 696c 652c 2077 6869 6368 2064 6566   file, which def
+00002160: 696e 6573 2074 6865 2050 726f 6475 6374  ines the Product
+00002170: 206d 6f64 656c 2075 7369 6e67 2074 6865   model using the
+00002180: 2042 6173 654d 6f64 656c 2063 6c61 7373   BaseModel class
+00002190: 2066 726f 6d20 7468 6520 7079 6461 6e74   from the pydant
+000021a0: 6963 206c 6962 7261 7279 2e0a 3c62 723e  ic library..<br>
+000021b0: 0a54 6865 206d 6f64 656c 2072 6570 7265  .The model repre
+000021c0: 7365 6e74 7320 7468 6520 7374 7275 6374  sents the struct
+000021d0: 7572 6520 616e 6420 6174 7472 6962 7574  ure and attribut
+000021e0: 6573 206f 6620 6120 7072 6f64 7563 742e  es of a product.
+000021f0: 0a0a 2323 2323 2070 726f 6475 6374 735f  ..#### products_
+00002200: 656e 7469 7479 2e70 790a 0a60 6060 7079  entity.py..```py
+00002210: 7468 6f6e 0a66 726f 6d20 7371 6c61 6c63  thon.from sqlalc
+00002220: 6865 6d79 2069 6d70 6f72 7420 436f 6c75  hemy import Colu
+00002230: 6d6e 2c20 496e 7465 6765 722c 2053 7472  mn, Integer, Str
+00002240: 696e 672c 2046 6c6f 6174 0a66 726f 6d20  ing, Float.from 
+00002250: 6f72 6d5f 636f 6e66 6967 2069 6d70 6f72  orm_config impor
+00002260: 7420 636f 6e66 6967 0a0a 0a63 6c61 7373  t config...class
+00002270: 2050 726f 6475 6374 2863 6f6e 6669 672e   Product(config.
+00002280: 4261 7365 293a 0a20 2020 205f 5f74 6162  Base):.    __tab
+00002290: 6c65 6e61 6d65 5f5f 203d 2022 7072 6f64  lename__ = "prod
+000022a0: 7563 7473 220a 0a20 2020 2069 6420 3d20  ucts"..    id = 
+000022b0: 436f 6c75 6d6e 2849 6e74 6567 6572 2c20  Column(Integer, 
+000022c0: 7072 696d 6172 795f 6b65 793d 5472 7565  primary_key=True
+000022d0: 2c20 696e 6465 783d 5472 7565 2c20 6175  , index=True, au
+000022e0: 746f 696e 6372 656d 656e 743d 5472 7565  toincrement=True
+000022f0: 290a 2020 2020 6e61 6d65 203d 2043 6f6c  ).    name = Col
+00002300: 756d 6e28 5374 7269 6e67 290a 2020 2020  umn(String).    
+00002310: 7072 6963 6520 3d20 436f 6c75 6d6e 2846  price = Column(F
+00002320: 6c6f 6174 290a 2020 2020 6465 7363 7269  loat).    descri
+00002330: 7074 696f 6e20 3d20 436f 6c75 6d6e 2853  ption = Column(S
+00002340: 7472 696e 6729 0a60 6060 0a0a 5468 6973  tring).```..This
+00002350: 2069 7320 7468 6520 7072 6f64 7563 7473   is the products
+00002360: 5f65 6e74 6974 792e 7079 2066 696c 652c  _entity.py file,
+00002370: 2077 6869 6368 2064 6566 696e 6573 2074   which defines t
+00002380: 6865 2050 726f 6475 6374 2065 6e74 6974  he Product entit
+00002390: 7920 7573 696e 6720 5351 4c41 6c63 6865  y using SQLAlche
+000023a0: 6d79 2e20 0a3c 6272 3e0a 4974 2069 6d70  my. .<br>.It imp
+000023b0: 6f72 7473 206e 6563 6573 7361 7279 206d  orts necessary m
+000023c0: 6f64 756c 6573 2061 6e64 2069 6e68 6572  odules and inher
+000023d0: 6974 7320 6672 6f6d 2074 6865 2063 6f6e  its from the con
+000023e0: 6669 672e 4261 7365 2063 6c61 7373 2e20  fig.Base class. 
+000023f0: 5468 6520 656e 7469 7479 2072 6570 7265  The entity repre
+00002400: 7365 6e74 7320 7468 6520 6461 7461 6261  sents the databa
+00002410: 7365 2074 6162 6c65 2066 6f72 2073 746f  se table for sto
+00002420: 7269 6e67 2070 726f 6475 6374 732c 2077  ring products, w
+00002430: 6974 6820 636f 6c75 6d6e 7320 666f 7220  ith columns for 
+00002440: 6964 2c20 6e61 6d65 2c20 7072 6963 652c  id, name, price,
+00002450: 2061 6e64 2064 6573 6372 6970 7469 6f6e   and description
+00002460: 2e0a 0a23 2323 2320 7072 6f64 7563 7473  ...#### products
+00002470: 5f73 6572 7669 6365 2e70 790a 0a60 6060  _service.py..```
+00002480: 7079 7468 6f6e 0a66 726f 6d20 7372 632e  python.from src.
+00002490: 7072 6f64 7563 7473 2e70 726f 6475 6374  products.product
+000024a0: 735f 6d6f 6465 6c20 696d 706f 7274 2050  s_model import P
+000024b0: 726f 6475 6374 0a66 726f 6d20 7372 632e  roduct.from src.
+000024c0: 7072 6f64 7563 7473 2e70 726f 6475 6374  products.product
+000024d0: 735f 656e 7469 7479 2069 6d70 6f72 7420  s_entity import 
+000024e0: 5072 6f64 7563 7420 6173 2050 726f 6475  Product as Produ
+000024f0: 6374 456e 7469 7479 0a66 726f 6d20 6f72  ctEntity.from or
+00002500: 6d5f 636f 6e66 6967 2069 6d70 6f72 7420  m_config import 
+00002510: 636f 6e66 6967 0a66 726f 6d20 6e65 7374  config.from nest
+00002520: 2e63 6f72 652e 6465 636f 7261 746f 7273  .core.decorators
+00002530: 2069 6d70 6f72 7420 6462 5f72 6571 7565   import db_reque
+00002540: 7374 5f68 616e 646c 6572 0a66 726f 6d20  st_handler.from 
+00002550: 6675 6e63 746f 6f6c 7320 696d 706f 7274  functools import
+00002560: 206c 7275 5f63 6163 6865 0a0a 0a40 6c72   lru_cache...@lr
+00002570: 755f 6361 6368 6528 290a 636c 6173 7320  u_cache().class 
+00002580: 5072 6f64 7563 7473 5365 7276 6963 653a  ProductsService:
+00002590: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000025a0: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+000025b0: 2073 656c 662e 636f 6e66 6967 203d 2063   self.config = c
+000025c0: 6f6e 6669 670a 2020 2020 2020 2020 7365  onfig.        se
+000025d0: 6c66 2e73 6573 7369 6f6e 203d 2073 656c  lf.session = sel
+000025e0: 662e 636f 6e66 6967 2e67 6574 5f64 6228  f.config.get_db(
+000025f0: 290a 0a20 2020 2040 6462 5f72 6571 7565  )..    @db_reque
+00002600: 7374 5f68 616e 646c 6572 0a20 2020 2064  st_handler.    d
+00002610: 6566 2061 6464 5f70 726f 6475 6374 2873  ef add_product(s
+00002620: 656c 662c 2070 726f 6475 6374 3a20 5072  elf, product: Pr
+00002630: 6f64 7563 7429 3a0a 2020 2020 2020 2020  oduct):.        
+00002640: 7072 6f64 7563 745f 656e 7469 7479 203d  product_entity =
+00002650: 2050 726f 6475 6374 456e 7469 7479 280a   ProductEntity(.
+00002660: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00002670: 3d70 726f 6475 6374 2e6e 616d 652c 0a20  =product.name,. 
+00002680: 2020 2020 2020 2020 2020 2070 7269 6365             price
+00002690: 3d70 726f 6475 6374 2e70 7269 6365 2c0a  =product.price,.
+000026a0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000026b0: 7269 7074 696f 6e3d 7072 6f64 7563 742e  ription=product.
+000026c0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
+000026d0: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000026e0: 6c66 2e73 6573 7369 6f6e 2e61 6464 2870  lf.session.add(p
+000026f0: 726f 6475 6374 5f65 6e74 6974 7929 0a20  roduct_entity). 
+00002700: 2020 2020 2020 2073 656c 662e 7365 7373         self.sess
+00002710: 696f 6e2e 636f 6d6d 6974 2829 0a20 2020  ion.commit().   
+00002720: 2020 2020 2072 6574 7572 6e20 7072 6f64       return prod
+00002730: 7563 745f 656e 7469 7479 2e69 640a 0a20  uct_entity.id.. 
+00002740: 2020 2040 6462 5f72 6571 7565 7374 5f68     @db_request_h
+00002750: 616e 646c 6572 0a20 2020 2064 6566 2067  andler.    def g
+00002760: 6574 5f70 726f 6475 6374 7328 7365 6c66  et_products(self
+00002770: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002780: 6e20 7365 6c66 2e73 6573 7369 6f6e 2e71  n self.session.q
+00002790: 7565 7279 2850 726f 6475 6374 456e 7469  uery(ProductEnti
+000027a0: 7479 292e 616c 6c28 290a 0a20 2020 2040  ty).all()..    @
+000027b0: 6462 5f72 6571 7565 7374 5f68 616e 646c  db_request_handl
+000027c0: 6572 0a20 2020 2064 6566 2067 6574 5f70  er.    def get_p
+000027d0: 726f 6475 6374 2873 656c 662c 2070 726f  roduct(self, pro
+000027e0: 6475 6374 5f69 643a 2069 6e74 293a 0a20  duct_id: int):. 
+000027f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00002800: 6c66 2e73 6573 7369 6f6e 2e71 7565 7279  lf.session.query
+00002810: 2850 726f 6475 6374 456e 7469 7479 292e  (ProductEntity).
+00002820: 6669 6c74 6572 2850 726f 6475 6374 456e  filter(ProductEn
+00002830: 7469 7479 2e69 6420 3d3d 2070 726f 6475  tity.id == produ
+00002840: 6374 5f69 6429 2e66 6972 7374 2829 0a0a  ct_id).first()..
+00002850: 2020 2020 4064 625f 7265 7175 6573 745f      @db_request_
+00002860: 6861 6e64 6c65 720a 2020 2020 6465 6620  handler.    def 
+00002870: 6c61 7374 5f70 726f 6475 6374 2873 656c  last_product(sel
+00002880: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
+00002890: 726e 2073 656c 662e 7365 7373 696f 6e2e  rn self.session.
+000028a0: 7175 6572 7928 5072 6f64 7563 7445 6e74  query(ProductEnt
+000028b0: 6974 7929 2e6f 7264 6572 5f62 7928 5072  ity).order_by(Pr
+000028c0: 6f64 7563 7445 6e74 6974 792e 6964 2e64  oductEntity.id.d
+000028d0: 6573 6328 2929 2e66 6972 7374 2829 0a60  esc()).first().`
+000028e0: 6060 0a0a 5468 6973 2069 7320 7468 6520  ``..This is the 
+000028f0: 7365 7276 6963 6520 6669 6c65 2c20 7768  service file, wh
+00002900: 6963 6820 636f 6e74 6169 6e73 2074 6865  ich contains the
+00002910: 2050 726f 6475 6374 7353 6572 7669 6365   ProductsService
+00002920: 2063 6c61 7373 2e20 4974 2069 6d70 6f72   class. It impor
+00002930: 7473 206e 6563 6573 7361 7279 206d 6f64  ts necessary mod
+00002940: 756c 6573 2061 6e64 2064 6566 696e 6573  ules and defines
+00002950: 206d 6574 686f 6473 2066 6f72 2069 6e74   methods for int
+00002960: 6572 6163 7469 6e67 2077 6974 6820 7468  eracting with th
+00002970: 6520 6461 7461 6261 7365 2e20 0a3c 6272  e database. .<br
+00002980: 3e0a 5468 6520 6d65 7468 6f64 7320 696e  >.The methods in
+00002990: 636c 7564 6520 6164 6469 6e67 2061 2070  clude adding a p
+000029a0: 726f 6475 6374 2c20 6765 7474 696e 6720  roduct, getting 
+000029b0: 616c 6c20 7072 6f64 7563 7473 2c20 6765  all products, ge
+000029c0: 7474 696e 6720 6120 7370 6563 6966 6963  tting a specific
+000029d0: 2070 726f 6475 6374 2062 7920 4944 2c20   product by ID, 
+000029e0: 616e 6420 7265 7472 6965 7669 6e67 2074  and retrieving t
+000029f0: 6865 206c 6173 7420 6164 6465 6420 7072  he last added pr
+00002a00: 6f64 7563 742e 0a3c 6272 3e0a 5468 6520  oduct..<br>.The 
+00002a10: 6040 6462 5f72 6571 7565 7374 5f68 616e  `@db_request_han
+00002a20: 646c 6572 6020 6465 636f 7261 746f 7220  dler` decorator 
+00002a30: 6973 2072 6573 706f 6e73 6962 6c65 2066  is responsible f
+00002a40: 6f72 206d 616e 6167 696e 6720 7468 6520  or managing the 
+00002a50: 6461 7461 6261 7365 2073 6573 7369 6f6e  database session
+00002a60: 2061 6e64 2068 616e 646c 696e 6720 616e   and handling an
+00002a70: 7920 6578 6365 7074 696f 6e73 2074 6861  y exceptions tha
+00002a80: 7420 6d61 7920 6f63 6375 7220 6475 7269  t may occur duri
+00002a90: 6e67 2064 6174 6162 6173 6520 6f70 6572  ng database oper
+00002aa0: 6174 696f 6e73 2e0a 0a0a 2323 2323 2070  ations....#### p
+00002ab0: 726f 6475 6374 735f 636f 6e74 726f 6c6c  roducts_controll
+00002ac0: 6572 2e70 790a 0a60 6060 7079 7468 6f6e  er.py..```python
+00002ad0: 0a66 726f 6d20 6e65 7374 2e63 6f72 6520  .from nest.core 
+00002ae0: 696d 706f 7274 2044 6570 656e 6473 2c20  import Depends, 
+00002af0: 436f 6e74 726f 6c6c 6572 2c20 4765 742c  Controller, Get,
+00002b00: 2050 6f73 740a 6672 6f6d 2073 7263 2e70   Post.from src.p
+00002b10: 726f 6475 6374 732e 7072 6f64 7563 7473  roducts.products
+00002b20: 5f73 6572 7669 6365 2069 6d70 6f72 7420  _service import 
+00002b30: 5072 6f64 7563 7473 5365 7276 6963 650a  ProductsService.
+00002b40: 6672 6f6d 2073 7263 2e70 726f 6475 6374  from src.product
+00002b50: 732e 7072 6f64 7563 7473 5f6d 6f64 656c  s.products_model
+00002b60: 2069 6d70 6f72 7420 5072 6f64 7563 740a   import Product.
+00002b70: 0a0a 4043 6f6e 7472 6f6c 6c65 7228 2270  ..@Controller("p
+00002b80: 726f 6475 6374 7322 290a 636c 6173 7320  roducts").class 
+00002b90: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
+00002ba0: 6572 3a0a 2020 2020 7365 7276 6963 653a  er:.    service:
+00002bb0: 2050 726f 6475 6374 7353 6572 7669 6365   ProductsService
+00002bc0: 203d 2044 6570 656e 6473 2850 726f 6475   = Depends(Produ
+00002bd0: 6374 7353 6572 7669 6365 290a 0a20 2020  ctsService)..   
+00002be0: 2040 4765 7428 222f 6765 745f 7072 6f64   @Get("/get_prod
+00002bf0: 7563 7473 2229 0a20 2020 2064 6566 2067  ucts").    def g
+00002c00: 6574 5f70 726f 6475 6374 7328 7365 6c66  et_products(self
+00002c10: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00002c20: 6e20 7365 6c66 2e73 6572 7669 6365 2e67  n self.service.g
+00002c30: 6574 5f70 726f 6475 6374 7328 290a 0a20  et_products().. 
+00002c40: 2020 2040 4765 7428 222f 6765 745f 7072     @Get("/get_pr
+00002c50: 6f64 7563 742f 7b70 726f 6475 6374 5f69  oduct/{product_i
+00002c60: 647d 2229 0a20 2020 2064 6566 2067 6574  d}").    def get
+00002c70: 5f70 726f 6475 6374 2873 656c 662c 2070  _product(self, p
+00002c80: 726f 6475 6374 5f69 643a 2069 6e74 293a  roduct_id: int):
+00002c90: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002ca0: 7365 6c66 2e73 6572 7669 6365 2e67 6574  self.service.get
+00002cb0: 5f70 726f 6475 6374 2870 726f 6475 6374  _product(product
+00002cc0: 5f69 6429 0a0a 2020 2020 4050 6f73 7428  _id)..    @Post(
+00002cd0: 222f 6164 645f 7072 6f64 7563 7422 290a  "/add_product").
+00002ce0: 2020 2020 6465 6620 6164 645f 7072 6f64      def add_prod
+00002cf0: 7563 7428 7365 6c66 2c20 7072 6f64 7563  uct(self, produc
+00002d00: 743a 2050 726f 6475 6374 293a 0a20 2020  t: Product):.   
+00002d10: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00002d20: 2e73 6572 7669 6365 2e61 6464 5f70 726f  .service.add_pro
+00002d30: 6475 6374 2870 726f 6475 6374 290a 0a20  duct(product).. 
+00002d40: 2020 2040 4765 7428 222f 6c61 7374 5f70     @Get("/last_p
+00002d50: 726f 6475 6374 2229 0a20 2020 2064 6566  roduct").    def
+00002d60: 206c 6173 745f 7072 6f64 7563 7428 7365   last_product(se
+00002d70: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
+00002d80: 7572 6e20 7365 6c66 2e73 6572 7669 6365  urn self.service
+00002d90: 2e6c 6173 745f 7072 6f64 7563 7428 290a  .last_product().
+00002da0: 6060 600a 496e 2073 756d 6d61 7279 2c20  ```.In summary, 
+00002db0: 7468 6520 6064 6563 6f72 6174 6f72 7360  the `decorators`
+00002dc0: 2061 6e64 2074 6865 2060 4465 7065 6e64   and the `Depend
+00002dd0: 7360 2063 6c61 7373 2061 7265 2075 7365  s` class are use
+00002de0: 6420 746f 2064 6566 696e 6520 726f 7574  d to define rout
+00002df0: 6573 2061 6e64 2048 5454 5020 6d65 7468  es and HTTP meth
+00002e00: 6f64 7320 666f 7220 7468 650a 3c62 723e  ods for the.<br>
+00002e10: 0a60 5072 6f64 7563 7473 436f 6e74 726f  .`ProductsContro
+00002e20: 6c6c 6572 6020 636c 6173 732c 2061 6e64  ller` class, and
+00002e30: 2074 6f20 696e 6a65 6374 2074 6865 2060   to inject the `
+00002e40: 5072 6f64 7563 7473 5365 7276 6963 6560  ProductsService`
+00002e50: 2064 6570 656e 6465 6e63 7920 696e 746f   dependency into
+00002e60: 2074 6865 2073 6572 7669 6365 2061 7474   the service att
+00002e70: 7269 6275 7465 206f 6620 7468 6520 636f  ribute of the co
+00002e80: 6e74 726f 6c6c 6572 2e0a 3c62 723e 0a54  ntroller..<br>.T
+00002e90: 6869 7320 616c 6c6f 7773 2074 6865 2063  his allows the c
+00002ea0: 6f6e 7472 6f6c 6c65 7220 746f 2068 616e  ontroller to han
+00002eb0: 646c 6520 696e 636f 6d69 6e67 2072 6571  dle incoming req
+00002ec0: 7565 7374 7320 616e 6420 696e 7465 7261  uests and intera
+00002ed0: 6374 2077 6974 680a 3c62 723e 0a54 6865  ct with.<br>.The
+00002ee0: 2073 6572 7669 6365 2074 6f20 7065 7266   service to perf
+00002ef0: 6f72 6d20 7370 6563 6966 6963 2061 6374  orm specific act
+00002f00: 696f 6e73 2062 6173 6564 206f 6e20 7468  ions based on th
+00002f10: 6520 726f 7574 6573 2061 6e64 206d 6574  e routes and met
+00002f20: 686f 6473 2064 6566 696e 6564 2e0a 0a0a  hods defined....
+00002f30: 2323 2323 2070 726f 6475 6374 735f 6d6f  #### products_mo
+00002f40: 6475 6c65 2e70 790a 0a60 6060 7079 7468  dule.py..```pyth
+00002f50: 6f6e 0a66 726f 6d20 7372 632e 7072 6f64  on.from src.prod
+00002f60: 7563 7473 2e70 726f 6475 6374 735f 636f  ucts.products_co
+00002f70: 6e74 726f 6c6c 6572 2069 6d70 6f72 7420  ntroller import 
+00002f80: 5072 6f64 7563 7473 436f 6e74 726f 6c6c  ProductsControll
+00002f90: 6572 0a66 726f 6d20 7372 632e 7072 6f64  er.from src.prod
+00002fa0: 7563 7473 2e70 726f 6475 6374 735f 7365  ucts.products_se
+00002fb0: 7276 6963 6520 696d 706f 7274 2050 726f  rvice import Pro
+00002fc0: 6475 6374 7353 6572 7669 6365 0a0a 0a63  ductsService...c
+00002fd0: 6c61 7373 2050 726f 6475 6374 734d 6f64  lass ProductsMod
+00002fe0: 756c 653a 0a0a 2020 2020 6465 6620 5f5f  ule:..    def __
+00002ff0: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00003000: 2020 2020 2020 7365 6c66 2e70 726f 7669        self.provi
+00003010: 6465 7273 203d 205b 5072 6f64 7563 7473  ders = [Products
+00003020: 5365 7276 6963 655d 0a20 2020 2020 2020  Service].       
+00003030: 2073 656c 662e 636f 6e74 726f 6c6c 6572   self.controller
+00003040: 7320 3d20 5b50 726f 6475 6374 7343 6f6e  s = [ProductsCon
+00003050: 7472 6f6c 6c65 725d 0a60 6060 0a0a 5468  troller].```..Th
+00003060: 6973 206d 6f64 756c 6520 6361 6e20 6265  is module can be
+00003070: 2072 6567 6973 7465 7265 6420 616e 6420   registered and 
+00003080: 7573 6564 2069 6e20 796f 7572 2061 7070  used in your app
+00003090: 6c69 6361 7469 6f6e 2e20 4f6e 6365 2074  lication. Once t
+000030a0: 6865 206d 6f64 756c 6520 6973 2072 6567  he module is reg
+000030b0: 6973 7465 7265 642c 2074 6865 2063 6f6e  istered, the con
+000030c0: 7472 6f6c 6c65 7220 726f 7574 6573 2077  troller routes w
+000030d0: 696c 6c20 6265 2061 7661 696c 6162 6c65  ill be available
+000030e0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
+000030f0: 6420 7061 7468 2e0a 0a54 6869 7320 3520  d path...This 5 
+00003100: 636f 6d70 6f6e 656e 7473 2061 7265 2074  components are t
+00003110: 6865 206d 696e 696d 756d 2072 6571 7569  he minimum requi
+00003120: 7265 6420 746f 2063 7265 6174 6520 6120  red to create a 
+00003130: 6d6f 6475 6c65 2074 6861 7420 776f 726b  module that work
+00003140: 7320 7769 7468 2074 6865 204f 524d 2e0a  s with the ORM..
+00003150: 5468 6572 6520 6172 6520 6d61 6e79 206d  There are many m
+00003160: 6f72 6520 6f70 7469 6f6e 7320 6f66 2068  ore options of h
+00003170: 6f77 2079 6f75 2063 616e 2064 6573 6967  ow you can desig
+00003180: 6e20 796f 7572 206d 6f64 756c 6573 2061  n your modules a
+00003190: 6e64 2077 6869 6368 2064 6174 6162 6173  nd which databas
+000031a0: 6573 2079 6f75 2063 616e 2075 7365 2c20  es you can use, 
+000031b0: 6275 7420 7468 6973 2069 7320 7468 6520  but this is the 
+000031c0: 6465 6661 756c 7420 6261 7369 6320 7374  default basic st
+000031d0: 7275 6374 7572 652e 0a0a 2323 204b 6579  ructure...## Key
+000031e0: 2046 6561 7475 7265 730a 2323 2320 4d6f   Features.### Mo
+000031f0: 6475 6c61 7220 4172 6368 6974 6563 7475  dular Architectu
+00003200: 7265 0a0a 5079 4e65 7374 2066 6f6c 6c6f  re..PyNest follo
+00003210: 7773 2074 6865 206d 6f64 756c 6172 2061  ws the modular a
+00003220: 7263 6869 7465 6374 7572 6520 6f66 204e  rchitecture of N
+00003230: 6573 744a 532c 2077 6869 6368 2061 6c6c  estJS, which all
+00003240: 6f77 7320 666f 7220 6561 7379 2073 6570  ows for easy sep
+00003250: 6172 6174 696f 6e20 6f66 2063 6f6e 6365  aration of conce
+00003260: 726e 7320 616e 6420 636f 6465 206f 7267  rns and code org
+00003270: 616e 697a 6174 696f 6e2e 2045 6163 6820  anization. Each 
+00003280: 6d6f 6475 6c65 2063 6f6e 7461 696e 7320  module contains 
+00003290: 6120 636f 6c6c 6563 7469 6f6e 206f 6620  a collection of 
+000032a0: 7265 6c61 7465 6420 636f 6e74 726f 6c6c  related controll
+000032b0: 6572 732c 2073 6572 7669 6365 732c 2061  ers, services, a
+000032c0: 6e64 2070 726f 7669 6465 7273 2e0a 0a23  nd providers...#
+000032d0: 2323 2044 6570 656e 6465 6e63 7920 496e  ## Dependency In
+000032e0: 6a65 6374 696f 6e0a 5079 4e65 7374 2073  jection.PyNest s
+000032f0: 7570 706f 7274 7320 6465 7065 6e64 656e  upports dependen
+00003300: 6379 2069 6e6a 6563 7469 6f6e 2c20 7768  cy injection, wh
+00003310: 6963 6820 6d61 6b65 7320 6974 2065 6173  ich makes it eas
+00003320: 7920 746f 206d 616e 6167 6520 6465 7065  y to manage depe
+00003330: 6e64 656e 6369 6573 2061 6e64 2077 7269  ndencies and wri
+00003340: 7465 2074 6573 7461 626c 6520 636f 6465  te testable code
+00003350: 2e20 596f 7520 6361 6e20 6561 7369 6c79  . You can easily
+00003360: 2069 6e6a 6563 7420 7365 7276 6963 6573   inject services
+00003370: 2061 6e64 2070 726f 7669 6465 7273 2069   and providers i
+00003380: 6e74 6f20 796f 7572 2063 6f6e 7472 6f6c  nto your control
+00003390: 6c65 7273 2075 7369 6e67 2064 6563 6f72  lers using decor
+000033a0: 6174 6f72 732e 0a0a 0a23 2323 2044 6563  ators....### Dec
+000033b0: 6f72 6174 6f72 730a 0a50 794e 6573 7420  orators..PyNest 
+000033c0: 6d61 6b65 7320 6578 7465 6e73 6976 6520  makes extensive 
+000033d0: 7573 6520 6f66 2064 6563 6f72 6174 6f72  use of decorator
+000033e0: 7320 746f 2064 6566 696e 6520 726f 7574  s to define rout
+000033f0: 6573 2c20 6d69 6464 6c65 7761 7265 2c20  es, middleware, 
+00003400: 616e 6420 6f74 6865 7220 6170 706c 6963  and other applic
+00003410: 6174 696f 6e20 636f 6d70 6f6e 656e 7473  ation components
+00003420: 2e20 5468 6973 2068 656c 7073 206b 6565  . This helps kee
+00003430: 7020 7468 6520 636f 6465 2063 6f6e 6369  p the code conci
+00003440: 7365 2061 6e64 2065 6173 7920 746f 2072  se and easy to r
+00003450: 6561 642e 0a0a 2323 2320 5479 7065 2041  ead...### Type A
+00003460: 6e6e 6f74 6174 696f 6e73 0a0a 5079 4e65  nnotations..PyNe
+00003470: 7374 206c 6576 6572 6167 6573 2050 7974  st leverages Pyt
+00003480: 686f 6e27 7320 7479 7065 2061 6e6e 6f74  hon's type annot
+00003490: 6174 696f 6e73 2074 6f20 7072 6f76 6964  ations to provid
+000034a0: 6520 6265 7474 6572 2074 6f6f 6c69 6e67  e better tooling
+000034b0: 2061 6e64 2068 656c 7020 7072 6576 656e   and help preven
+000034c0: 7420 6572 726f 7273 2e20 596f 7520 6361  t errors. You ca
+000034d0: 6e20 616e 6e6f 7461 7465 2079 6f75 7220  n annotate your 
+000034e0: 636f 6e74 726f 6c6c 6572 732c 2073 6572  controllers, ser
+000034f0: 7669 6365 732c 2061 6e64 2070 726f 7669  vices, and provi
+00003500: 6465 7273 2077 6974 6820 7479 7065 7320  ders with types 
+00003510: 746f 206d 616b 6520 796f 7572 2063 6f64  to make your cod
+00003520: 6520 6d6f 7265 2072 6f62 7573 742e 0a0a  e more robust...
+00003530: 2323 2320 436f 6465 2047 656e 6572 6174  ### Code Generat
+00003540: 696f 6e0a 0a50 794e 6573 7420 696e 636c  ion..PyNest incl
+00003550: 7564 6573 2061 2063 6f64 6520 6765 6e65  udes a code gene
+00003560: 7261 7469 6f6e 2074 6f6f 6c20 7468 6174  ration tool that
+00003570: 2063 616e 2063 7265 6174 6520 626f 696c   can create boil
+00003580: 6572 706c 6174 6520 636f 6465 2066 6f72  erplate code for
+00003590: 206d 6f64 756c 6573 2c20 636f 6e74 726f   modules, contro
+000035a0: 6c6c 6572 732c 2061 6e64 206f 7468 6572  llers, and other
+000035b0: 2063 6f6d 706f 6e65 6e74 732e 2054 6869   components. Thi
+000035c0: 7320 7361 7665 7320 796f 7520 7469 6d65  s saves you time
+000035d0: 2061 6e64 2068 656c 7073 2079 6f75 2066   and helps you f
+000035e0: 6f63 7573 206f 6e20 7772 6974 696e 6720  ocus on writing 
+000035f0: 7468 6520 636f 6465 2074 6861 7420 6d61  the code that ma
+00003600: 7474 6572 732e 0a0a 2323 2046 7574 7572  tters...## Futur
+00003610: 6520 506c 616e 730a 0a2d 205b 205d 2043  e Plans..- [ ] C
+00003620: 7265 6174 6520 4d61 726b 6574 706c 6163  reate Marketplac
+00003630: 6520 666f 7220 6d6f 6475 6c65 7320 7768  e for modules wh
+00003640: 6572 6520 6465 7665 6c6f 7065 7273 2063  ere developers c
+00003650: 616e 2073 6861 7265 2074 6865 6972 206d  an share their m
+00003660: 6f64 756c 6573 2061 6e64 2064 6f77 6e6c  odules and downl
+00003670: 6f61 6420 6d6f 6475 6c65 7320 6372 6561  oad modules crea
+00003680: 7465 6420 6279 206f 7468 6572 732e 0a2d  ted by others..-
+00003690: 205b 205d 2043 7265 7465 2041 6273 7472   [ ] Crete Abstr
+000036a0: 6163 7469 6f6e 2063 6c61 7373 2074 6f20  action class to 
+000036b0: 4d6f 6475 6c65 7320 616e 6420 5365 7276  Modules and Serv
+000036c0: 6963 6573 2074 6f20 616c 6c6f 7720 666f  ices to allow fo
+000036d0: 7220 6561 7379 2063 7265 6174 696f 6e20  r easy creation 
+000036e0: 6f66 206d 6f64 756c 6573 2061 6e64 2073  of modules and s
+000036f0: 6572 7669 6365 732e 0a2d 205b 205d 2041  ervices..- [ ] A
+00003700: 6464 2069 6e68 6572 6974 616e 6365 2062  dd inheritance b
+00003710: 6574 7765 656e 2063 6f6e 7472 6f6c 6c65  etween controlle
+00003720: 7273 2066 6f72 2063 7265 6174 696e 6720  rs for creating 
+00003730: 6d6f 7265 2063 6f6d 706c 6578 2063 6f6e  more complex con
+00003740: 7472 6f6c 6c65 7273 2e0a 2d20 5b20 5d20  trollers..- [ ] 
+00003750: 4164 6420 7375 7070 6f72 7420 666f 7220  Add support for 
+00003760: 6f74 6865 7220 6461 7461 6261 7365 7320  other databases 
+00003770: 286d 6f6e 676f 4442 2c20 7265 6469 732c  (mongoDB, redis,
+00003780: 2065 7463 2e29 0a2d 205b 205d 2043 7265   etc.).- [ ] Cre
+00003790: 6174 6520 6f75 742d 6f66 2d74 6865 2d62  ate out-of-the-b
+000037a0: 6f78 2061 7574 6865 6e74 6963 6174 696f  ox authenticatio
+000037b0: 6e20 6d6f 6475 6c65 2074 6861 7420 6361  n module that ca
+000037c0: 6e20 6265 2065 6173 696c 7920 696e 7465  n be easily inte
+000037d0: 6772 6174 6564 2069 6e74 6f20 616e 7920  grated into any 
+000037e0: 6170 706c 6963 6174 696f 6e2e 0a2d 205b  application..- [
+000037f0: 205d 2041 6464 2073 7570 706f 7274 2066   ] Add support f
+00003800: 6f72 206f 7468 6572 2074 6573 7469 6e67  or other testing
+00003810: 2066 7261 6d65 776f 726b 7320 616e 6420   frameworks and 
+00003820: 6372 6561 7465 2074 6573 7469 6e67 2074  create testing t
+00003830: 656d 706c 6174 6573 2e0a 2d20 5b20 5d20  emplates..- [ ] 
+00003840: 4164 6420 7375 7070 6f72 7420 666f 7220  Add support for 
+00003850: 6f74 6865 7220 7765 6220 6672 616d 6577  other web framew
+00003860: 6f72 6b73 2028 466c 6173 6b2c 2044 6a61  orks (Flask, Dja
+00003870: 6e67 6f2c 2065 7463 2e29 202d 2053 616d  ngo, etc.) - Sam
+00003880: 6520 4172 6368 6974 6563 7475 7265 2c20  e Architecture, 
+00003890: 6469 6666 6572 656e 7420 656e 6769 6e65  different engine
+000038a0: 2e0a 0a0a 2323 2043 6f6e 7472 6962 7574  ....## Contribut
+000038b0: 696e 670a 0a43 6f6e 7472 6962 7574 696f  ing..Contributio
+000038c0: 6e73 2061 7265 2077 656c 636f 6d65 2120  ns are welcome! 
+000038d0: 506c 6561 7365 2066 6565 6c20 6672 6565  Please feel free
+000038e0: 2074 6f20 6772 6162 206f 6e65 206f 6620   to grab one of 
+000038f0: 7468 6520 6f70 656e 2069 7373 7565 732c  the open issues,
+00003900: 0a6f 7220 6f70 656e 2061 206e 6577 206f  .or open a new o
+00003910: 6e65 2069 6620 796f 7520 6861 7665 2061  ne if you have a
+00003920: 6e20 6964 6561 2066 6f72 2061 206e 6577  n idea for a new
+00003930: 2066 6561 7475 7265 206f 7220 696d 7072   feature or impr
+00003940: 6f76 656d 656e 742e 0a0a 5468 6973 2077  ovement...This w
+00003950: 6f75 6c64 2062 7269 6e67 2061 2068 7567  ould bring a hug
+00003960: 6520 696d 7061 6374 2074 6f20 7468 6520  e impact to the 
+00003970: 7072 6f6a 6563 7420 616e 6420 7468 6520  project and the 
+00003980: 636f 6d6d 756e 6974 792e 0a0a 2323 204c  community...## L
+00003990: 6963 656e 7365 0a0a 5079 4e65 7374 2069  icense..PyNest i
+000039a0: 7320 5b4d 4954 206c 6963 656e 7365 645d  s [MIT licensed]
+000039b0: 284c 4943 454e 5345 292e 0a0a 2323 2043  (LICENSE)...## C
+000039c0: 7265 6469 7473 0a0a 5079 4e65 7374 2069  redits..PyNest i
+000039d0: 7320 696e 7370 6972 6564 2062 7920 5b4e  s inspired by [N
+000039e0: 6573 744a 535d 2868 7474 7073 3a2f 2f6e  estJS](https://n
+000039f0: 6573 746a 732e 636f 6d2f 292e 0a         estjs.com/)..
```

### Comparing `pynest-api-0.0.3/pynest_api.egg-info/SOURCES.txt` & `pynest-api-0.1.0/pynest_api.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 nest/__init__.py
 nest/cli/__init__.py
 nest/cli/cli.py
 nest/cli/click_handlers.py
 nest/common/__init__.py
-nest/common/common.py
 nest/common/templates/__init__.py
 nest/common/templates/app.py
 nest/common/templates/controller.py
 nest/common/templates/dockerfile.py
 nest/common/templates/entity.py
 nest/common/templates/main.py
 nest/common/templates/model.py
@@ -18,19 +17,23 @@
 nest/common/templates/orm_config.py
 nest/common/templates/readme.py
 nest/common/templates/requierments.py
 nest/common/templates/service.py
 nest/core/__init__.py
 nest/core/app.py
 nest/core/database/__init__.py
+nest/core/database/base_odm.py
 nest/core/database/base_orm.py
+nest/core/database/config.py
+nest/core/database/odm_config.py
 nest/core/database/orm_config.py
 nest/core/decorators/__init__.py
 nest/core/decorators/controller.py
 nest/core/decorators/database.py
+nest/core/decorators/helpers.py
 nest/marketplace/__init__.py
 nest/marketplace/controllers/__init__.py
 nest/marketplace/modules/__init__.py
 nest/marketplace/modules/auth/__init__.py
 nest/marketplace/services/__init__.py
 pynest_api.egg-info/PKG-INFO
 pynest_api.egg-info/SOURCES.txt
```

### Comparing `pynest-api-0.0.3/pyproject.toml` & `pynest-api-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,34 +13,24 @@
     { name = "Itay Dar", email = "itay2803@gmail.com" },
 ]
 dynamic = ["version"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
-    "anyio==3.6.2",
-    "click==8.1.3",
+    "click==8.1.6",
     "fastapi==0.95.1",
-    "fastapi-utils==0.2.1",
-    "greenlet==2.0.2",
-    "h11==0.14.0",
-    "idna==3.4",
-    "pydantic==1.10.7",
     "python-dotenv==1.0.0",
-    "sniffio==1.3.0",
-    "SQLAlchemy==1.4.48",
-    "starlette==0.26.1",
-    "typing_extensions==4.5.0",
-    "uvicorn==0.22.0",
+    "SQLAlchemy==2.0.19",
+    "uvicorn==0.23.1",
 ]
 
 [tool.setuptools.dynamic]
 version = { attr = "nest.__init__.__version__" }
 
 [tool.pip]
 index-url = "https://pypi.org/simple"
```

