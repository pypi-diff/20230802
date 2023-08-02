# Comparing `tmp/types-aiobotocore-qldb-2.5.2.tar.gz` & `tmp/types-aiobotocore-qldb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qldb-2.5.2.tar", last modified: Sat Jul  8 01:44:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-qldb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
```

## Comparing `types-aiobotocore-qldb-2.5.2.tar` & `types-aiobotocore-qldb-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.062720 types-aiobotocore-qldb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-08 01:44:09.054720 types-aiobotocore-qldb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12445 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:09.062720 types-aiobotocore-qldb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.054720 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-07-08 01:36:54.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-07-08 01:36:54.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-07-08 01:36:54.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-07-08 01:36:54.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:53.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:09.054720 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:44:08.000000 types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.033491 types-aiobotocore-qldb-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-08-02 14:52:50.029491 types-aiobotocore-qldb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.033491 types-aiobotocore-qldb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.025491 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16612 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17819 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17792 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:13.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.029491 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:49.000000 types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qldb-2.5.2/LICENSE` & `types-aiobotocore-qldb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2/PKG-INFO` & `types-aiobotocore-qldb-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore qldb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore qldb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -34,29 +33,29 @@
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-qldb?color=blue)](https://pypistats.org/packages/types-aiobotocore-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.QLDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -286,52 +285,53 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_qldb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
@@ -345,15 +345,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-qldb-2.5.2/README.md` & `types-aiobotocore-qldb-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-qldb?color=blue)](https://pypistats.org/packages/types-aiobotocore-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.QLDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -253,52 +253,53 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_qldb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
@@ -312,15 +313,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-qldb-2.5.2/setup.py` & `types-aiobotocore-qldb-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qldb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        " 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="aiobotocore qldb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore qldb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_qldb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/__main__.py` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QLDB 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.QLDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2")
+    print("2.5.2.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/client.py` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_qldb.client import QLDBClient
 
     session = get_session()
     async with session.create_client("qldb") as client:
         client: QLDBClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OutputFormatType, PermissionsModeType
 from .type_defs import (
     CancelJournalKinesisStreamResponseTypeDef,
@@ -36,14 +35,15 @@
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
     ListLedgersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3ExportConfigurationTypeDef,
     StreamJournalToKinesisResponseTypeDef,
+    TimestampTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
@@ -164,16 +164,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#describe_ledger)
         """
 
     async def export_journal_to_s3(
         self,
         *,
         Name: str,
-        InclusiveStartTime: Union[datetime, str],
-        ExclusiveEndTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
+        ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
         OutputFormat: OutputFormatType = ...
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3) bucket.
@@ -286,19 +286,19 @@
         """
 
     async def stream_journal_to_kinesis(
         self,
         *,
         LedgerName: str,
         RoleArn: str,
-        InclusiveStartTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: Union[datetime, str] = ...
+        ExclusiveEndTime: TimestampTypeDef = ...
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/client.pyi` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_qldb.client import QLDBClient
 
     session = get_session()
     async with session.create_client("qldb") as client:
         client: QLDBClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import OutputFormatType, PermissionsModeType
 from .type_defs import (
     CancelJournalKinesisStreamResponseTypeDef,
@@ -36,14 +35,15 @@
     ListJournalKinesisStreamsForLedgerResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
     ListLedgersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     S3ExportConfigurationTypeDef,
     StreamJournalToKinesisResponseTypeDef,
+    TimestampTypeDef,
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
@@ -152,16 +152,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.describe_ledger)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#describe_ledger)
         """
     async def export_journal_to_s3(
         self,
         *,
         Name: str,
-        InclusiveStartTime: Union[datetime, str],
-        ExclusiveEndTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
+        ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
         OutputFormat: OutputFormatType = ...
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3) bucket.
@@ -264,19 +264,19 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#list_tags_for_resource)
         """
     async def stream_journal_to_kinesis(
         self,
         *,
         LedgerName: str,
         RoleArn: str,
-        InclusiveStartTime: Union[datetime, str],
+        InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: Union[datetime, str] = ...
+        ExclusiveEndTime: TimestampTypeDef = ...
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/literals.py` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/literals.pyi` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/type_defs.py` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
-    data: CancelJournalKinesisStreamRequestRequestTypeDef = {...}
+    data: CancelJournalKinesisStreamRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -30,42 +30,43 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
-    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
+    "TimestampTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3EncryptionConfigurationTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerPermissionsModeResponseTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
+    "CreateLedgerResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
+    "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
@@ -86,19 +87,22 @@
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -118,28 +122,14 @@
 
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
 
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -184,29 +174,15 @@
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
-    {
-        "ExportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
@@ -316,33 +292,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
@@ -356,22 +313,14 @@
 
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
 
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -388,24 +337,14 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -420,38 +359,101 @@
 
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
 
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -474,24 +476,24 @@
 
 
 GetBlockResponseTypeDef = TypedDict(
     "GetBlockResponseTypeDef",
     {
         "Block": ValueHolderTypeDef,
         "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDigestResponseTypeDef = TypedDict(
     "GetDigestResponseTypeDef",
     {
         "Digest": bytes,
         "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
@@ -515,15 +517,15 @@
 
 
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
         "Proof": ValueHolderTypeDef,
         "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
@@ -554,24 +556,24 @@
 
 
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
-        "InclusiveStartTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
         "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_OptionalStreamJournalToKinesisRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "ExclusiveEndTime": TimestampTypeDef,
     },
     total=False,
 )
 
 
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
@@ -581,15 +583,15 @@
 
 
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -598,33 +600,33 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
+        "ExclusiveEndTime": TimestampTypeDef,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
 _OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
@@ -668,28 +670,28 @@
     pass
 
 
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb/type_defs.pyi` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestRequestTypeDef
 
-    data: CancelJournalKinesisStreamRequestRequestTypeDef = {...}
+    data: CancelJournalKinesisStreamRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -29,42 +29,43 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
-    "CancelJournalKinesisStreamResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
-    "CreateLedgerResponseTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
     "DescribeLedgerRequestRequestTypeDef",
     "LedgerEncryptionDescriptionTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExportJournalToS3ResponseTypeDef",
+    "TimestampTypeDef",
     "ValueHolderTypeDef",
     "GetDigestRequestRequestTypeDef",
     "KinesisConfigurationTypeDef",
     "LedgerSummaryTypeDef",
     "ListJournalKinesisStreamsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsForLedgerRequestRequestTypeDef",
     "ListJournalS3ExportsRequestRequestTypeDef",
     "ListLedgersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "S3EncryptionConfigurationTypeDef",
-    "StreamJournalToKinesisResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
-    "UpdateLedgerPermissionsModeResponseTypeDef",
     "UpdateLedgerRequestRequestTypeDef",
+    "CancelJournalKinesisStreamResponseTypeDef",
+    "CreateLedgerResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportJournalToS3ResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StreamJournalToKinesisResponseTypeDef",
+    "UpdateLedgerPermissionsModeResponseTypeDef",
     "DescribeLedgerResponseTypeDef",
     "UpdateLedgerResponseTypeDef",
     "GetBlockRequestRequestTypeDef",
     "GetBlockResponseTypeDef",
     "GetDigestResponseTypeDef",
     "GetRevisionRequestRequestTypeDef",
     "GetRevisionResponseTypeDef",
@@ -85,19 +86,22 @@
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     {
         "LedgerName": str,
         "StreamId": str,
     },
 )
 
-CancelJournalKinesisStreamResponseTypeDef = TypedDict(
-    "CancelJournalKinesisStreamResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLedgerRequestRequestTypeDef",
     {
         "Name": str,
@@ -115,28 +119,14 @@
 )
 
 class CreateLedgerRequestRequestTypeDef(
     _RequiredCreateLedgerRequestRequestTypeDef, _OptionalCreateLedgerRequestRequestTypeDef
 ):
     pass
 
-CreateLedgerResponseTypeDef = TypedDict(
-    "CreateLedgerResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "State": LedgerStateType,
-        "CreationDateTime": datetime,
-        "PermissionsMode": PermissionsModeType,
-        "DeletionProtection": bool,
-        "KmsKeyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLedgerRequestRequestTypeDef = TypedDict(
     "DeleteLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -179,29 +169,15 @@
 )
 
 class LedgerEncryptionDescriptionTypeDef(
     _RequiredLedgerEncryptionDescriptionTypeDef, _OptionalLedgerEncryptionDescriptionTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExportJournalToS3ResponseTypeDef = TypedDict(
-    "ExportJournalToS3ResponseTypeDef",
-    {
-        "ExportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 ValueHolderTypeDef = TypedDict(
     "ValueHolderTypeDef",
     {
         "IonText": str,
     },
     total=False,
 )
@@ -305,33 +281,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredS3EncryptionConfigurationTypeDef = TypedDict(
     "_RequiredS3EncryptionConfigurationTypeDef",
     {
         "ObjectEncryptionType": S3ObjectEncryptionTypeType,
     },
 )
 _OptionalS3EncryptionConfigurationTypeDef = TypedDict(
@@ -343,22 +300,14 @@
 )
 
 class S3EncryptionConfigurationTypeDef(
     _RequiredS3EncryptionConfigurationTypeDef, _OptionalS3EncryptionConfigurationTypeDef
 ):
     pass
 
-StreamJournalToKinesisResponseTypeDef = TypedDict(
-    "StreamJournalToKinesisResponseTypeDef",
-    {
-        "StreamId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -375,24 +324,14 @@
     "UpdateLedgerPermissionsModeRequestRequestTypeDef",
     {
         "Name": str,
         "PermissionsMode": PermissionsModeType,
     },
 )
 
-UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
-    "UpdateLedgerPermissionsModeResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "PermissionsMode": PermissionsModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateLedgerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLedgerRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateLedgerRequestRequestTypeDef = TypedDict(
@@ -405,38 +344,101 @@
 )
 
 class UpdateLedgerRequestRequestTypeDef(
     _RequiredUpdateLedgerRequestRequestTypeDef, _OptionalUpdateLedgerRequestRequestTypeDef
 ):
     pass
 
+CancelJournalKinesisStreamResponseTypeDef = TypedDict(
+    "CancelJournalKinesisStreamResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLedgerResponseTypeDef = TypedDict(
+    "CreateLedgerResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "State": LedgerStateType,
+        "CreationDateTime": datetime,
+        "PermissionsMode": PermissionsModeType,
+        "DeletionProtection": bool,
+        "KmsKeyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportJournalToS3ResponseTypeDef = TypedDict(
+    "ExportJournalToS3ResponseTypeDef",
+    {
+        "ExportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StreamJournalToKinesisResponseTypeDef = TypedDict(
+    "StreamJournalToKinesisResponseTypeDef",
+    {
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateLedgerPermissionsModeResponseTypeDef = TypedDict(
+    "UpdateLedgerPermissionsModeResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "PermissionsMode": PermissionsModeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeLedgerResponseTypeDef = TypedDict(
     "DescribeLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "PermissionsMode": PermissionsModeType,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLedgerResponseTypeDef = TypedDict(
     "UpdateLedgerResponseTypeDef",
     {
         "Name": str,
         "Arn": str,
         "State": LedgerStateType,
         "CreationDateTime": datetime,
         "DeletionProtection": bool,
         "EncryptionDescription": LedgerEncryptionDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetBlockRequestRequestTypeDef = TypedDict(
     "_RequiredGetBlockRequestRequestTypeDef",
     {
         "Name": str,
@@ -457,24 +459,24 @@
     pass
 
 GetBlockResponseTypeDef = TypedDict(
     "GetBlockResponseTypeDef",
     {
         "Block": ValueHolderTypeDef,
         "Proof": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDigestResponseTypeDef = TypedDict(
     "GetDigestResponseTypeDef",
     {
         "Digest": bytes,
         "DigestTipAddress": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetRevisionRequestRequestTypeDef = TypedDict(
     "_RequiredGetRevisionRequestRequestTypeDef",
     {
         "Name": str,
@@ -496,15 +498,15 @@
     pass
 
 GetRevisionResponseTypeDef = TypedDict(
     "GetRevisionResponseTypeDef",
     {
         "Proof": ValueHolderTypeDef,
         "Revision": ValueHolderTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredJournalKinesisStreamDescriptionTypeDef = TypedDict(
     "_RequiredJournalKinesisStreamDescriptionTypeDef",
     {
         "LedgerName": str,
@@ -533,24 +535,24 @@
     pass
 
 _RequiredStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_RequiredStreamJournalToKinesisRequestRequestTypeDef",
     {
         "LedgerName": str,
         "RoleArn": str,
-        "InclusiveStartTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
         "KinesisConfiguration": KinesisConfigurationTypeDef,
         "StreamName": str,
     },
 )
 _OptionalStreamJournalToKinesisRequestRequestTypeDef = TypedDict(
     "_OptionalStreamJournalToKinesisRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "ExclusiveEndTime": TimestampTypeDef,
     },
     total=False,
 )
 
 class StreamJournalToKinesisRequestRequestTypeDef(
     _RequiredStreamJournalToKinesisRequestRequestTypeDef,
     _OptionalStreamJournalToKinesisRequestRequestTypeDef,
@@ -558,15 +560,15 @@
     pass
 
 ListLedgersResponseTypeDef = TypedDict(
     "ListLedgersResponseTypeDef",
     {
         "Ledgers": List[LedgerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3ExportConfigurationTypeDef = TypedDict(
     "S3ExportConfigurationTypeDef",
     {
         "Bucket": str,
@@ -575,33 +577,33 @@
     },
 )
 
 DescribeJournalKinesisStreamResponseTypeDef = TypedDict(
     "DescribeJournalKinesisStreamResponseTypeDef",
     {
         "Stream": JournalKinesisStreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalKinesisStreamsForLedgerResponseTypeDef = TypedDict(
     "ListJournalKinesisStreamsForLedgerResponseTypeDef",
     {
         "Streams": List[JournalKinesisStreamDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_RequiredExportJournalToS3RequestRequestTypeDef",
     {
         "Name": str,
-        "InclusiveStartTime": Union[datetime, str],
-        "ExclusiveEndTime": Union[datetime, str],
+        "InclusiveStartTime": TimestampTypeDef,
+        "ExclusiveEndTime": TimestampTypeDef,
         "S3ExportConfiguration": S3ExportConfigurationTypeDef,
         "RoleArn": str,
     },
 )
 _OptionalExportJournalToS3RequestRequestTypeDef = TypedDict(
     "_OptionalExportJournalToS3RequestRequestTypeDef",
     {
@@ -641,28 +643,28 @@
 ):
     pass
 
 DescribeJournalS3ExportResponseTypeDef = TypedDict(
     "DescribeJournalS3ExportResponseTypeDef",
     {
         "ExportDescription": JournalS3ExportDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsForLedgerResponseTypeDef = TypedDict(
     "ListJournalS3ExportsForLedgerResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJournalS3ExportsResponseTypeDef = TypedDict(
     "ListJournalS3ExportsResponseTypeDef",
     {
         "JournalS3Exports": List[JournalS3ExportDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/PKG-INFO` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.QLDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore qldb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore qldb type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -34,29 +33,29 @@
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-qldb?color=blue)](https://pypistats.org/packages/types-aiobotocore-qldb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.QLDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -286,52 +285,53 @@
 )
 
 
 def check_value(value: EncryptionStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_qldb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_qldb.type_defs import (
     CancelJournalKinesisStreamRequestRequestTypeDef,
-    CancelJournalKinesisStreamResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateLedgerRequestRequestTypeDef,
-    CreateLedgerResponseTypeDef,
     DeleteLedgerRequestRequestTypeDef,
     DescribeJournalKinesisStreamRequestRequestTypeDef,
     DescribeJournalS3ExportRequestRequestTypeDef,
     DescribeLedgerRequestRequestTypeDef,
     LedgerEncryptionDescriptionTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExportJournalToS3ResponseTypeDef,
+    TimestampTypeDef,
     ValueHolderTypeDef,
     GetDigestRequestRequestTypeDef,
     KinesisConfigurationTypeDef,
     LedgerSummaryTypeDef,
     ListJournalKinesisStreamsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsForLedgerRequestRequestTypeDef,
     ListJournalS3ExportsRequestRequestTypeDef,
     ListLedgersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     S3EncryptionConfigurationTypeDef,
-    StreamJournalToKinesisResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateLedgerPermissionsModeRequestRequestTypeDef,
-    UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerRequestRequestTypeDef,
+    CancelJournalKinesisStreamResponseTypeDef,
+    CreateLedgerResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportJournalToS3ResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StreamJournalToKinesisResponseTypeDef,
+    UpdateLedgerPermissionsModeResponseTypeDef,
     DescribeLedgerResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     GetBlockRequestRequestTypeDef,
     GetBlockResponseTypeDef,
     GetDigestResponseTypeDef,
     GetRevisionRequestRequestTypeDef,
     GetRevisionResponseTypeDef,
@@ -345,15 +345,15 @@
     JournalS3ExportDescriptionTypeDef,
     DescribeJournalS3ExportResponseTypeDef,
     ListJournalS3ExportsForLedgerResponseTypeDef,
     ListJournalS3ExportsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelJournalKinesisStreamRequestRequestTypeDef:
+def get_value() -> CancelJournalKinesisStreamRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-qldb-2.5.2/types_aiobotocore_qldb.egg-info/SOURCES.txt` & `types-aiobotocore-qldb-2.5.2.post1/types_aiobotocore_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

