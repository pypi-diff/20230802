# Comparing `tmp/fgo_api_types-2023.8.1.1.53.3.tar.gz` & `tmp/fgo_api_types-2023.8.2.1.45.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.8.1.1.53.3.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.8.2.1.45.2.tar", max compression
```

## Comparing `fgo_api_types-2023.8.1.1.53.3.tar` & `fgo_api_types-2023.8.2.1.45.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-08-01 01:52:40.166273 fgo_api_types-2023.8.1.1.53.3/LICENSE
--rw-r--r--   0        0        0      449 2023-08-01 01:52:40.166273 fgo_api_types-2023.8.1.1.53.3/README.md
--rw-r--r--   0        0        0        0 2023-08-01 01:53:03.914244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3738 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/common.py
--rw-r--r--   0        0        0    38163 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/enums.py
--rw-r--r--   0        0        0   160790 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    79146 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/nice.py
--rw-r--r--   0        0        0    53437 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4207 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19183 2023-08-01 01:53:03.918244 fgo_api_types-2023.8.1.1.53.3/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-08-01 01:53:04.250244 fgo_api_types-2023.8.1.1.53.3/pyproject.toml
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.8.1.1.53.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-08-02 01:44:41.989705 fgo_api_types-2023.8.2.1.45.2/LICENSE
+-rw-r--r--   0        0        0      449 2023-08-02 01:44:41.989705 fgo_api_types-2023.8.2.1.45.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3738 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/common.py
+-rw-r--r--   0        0        0    38212 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   160790 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    79146 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    53437 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4207 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19183 2023-08-02 01:45:02.933723 fgo_api_types-2023.8.2.1.45.2/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-08-02 01:45:03.265724 fgo_api_types-2023.8.2.1.45.2/pyproject.toml
+-rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 fgo_api_types-2023.8.2.1.45.2/PKG-INFO
```

### Comparing `fgo_api_types-2023.8.1.1.53.3/LICENSE` & `fgo_api_types-2023.8.2.1.45.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/basic.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/common.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/enums.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -961,14 +961,15 @@
     holdingHolyGrail = "holdingHolyGrail"
     standardClassServant = "standardClassServant"
     classBeast = "classBeast"
     classBeastVI = "classBeastVI"
     classBeastVIBoss = "classBeastVIBoss"
     buffBound = "buffBound"
     buffDamageCut = "buffDamageCut"
+    marking = "marking"
 
 
 TRAIT_NAME: dict[int, Trait] = {
     1: Trait.genderMale,
     2: Trait.genderFemale,
     3: Trait.genderUnknown,
     100: Trait.classSaber,
@@ -1206,14 +1207,15 @@
     3066: Trait.buffSleep,
     3068: Trait.chenGongNp,
     3070: Trait.buffNullifyBuff,
     3076: Trait.cantBeSacrificed,
     3085: Trait.buffDamageCut,
     3086: Trait.gutsBlock,
     3087: Trait.buffBound,
+    3088: Trait.marking,
     # 6016: No detail
     # 6021: No detail
     # 6022: No detail
     # 10xxx: CCC Kiara buff
     4001: Trait.cardArts,
     4002: Trait.cardBuster,
     4003: Trait.cardQuick,
```

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/gameenums.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/nice.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/nice.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/raw.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/rayshift.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/fgo_api_types/search.py` & `fgo_api_types-2023.8.2.1.45.2/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.8.1.1.53.3/pyproject.toml` & `fgo_api_types-2023.8.2.1.45.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.08.01.01.53.03"
+version = "2023.08.02.01.45.02"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.8.1.1.53.3/PKG-INFO` & `fgo_api_types-2023.8.2.1.45.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.8.1.1.53.3
+Version: 2023.8.2.1.45.2
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

