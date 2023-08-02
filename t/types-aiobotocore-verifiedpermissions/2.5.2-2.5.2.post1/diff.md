# Comparing `tmp/types-aiobotocore-verifiedpermissions-2.5.2.tar.gz` & `tmp/types-aiobotocore-verifiedpermissions-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.2.tar", last modified: Sat Jul  8 01:44:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
```

## Comparing `types-aiobotocore-verifiedpermissions-2.5.2.tar` & `types-aiobotocore-verifiedpermissions-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.747022 types-aiobotocore-verifiedpermissions-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17218 2023-07-08 01:44:26.747022 types-aiobotocore-verifiedpermissions-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:26.747022 types-aiobotocore-verifiedpermissions-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.743022 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31266 2023-07-08 01:42:12.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31215 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:11.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:26.747022 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17218 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:26.000000 types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.881432 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31216 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/LICENSE` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore verifiedpermissions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore verifiedpermissions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-verifiedpermissions"></a>
 
 # types-aiobotocore-verifiedpermissions
 
 [![PyPI - types-aiobotocore-verifiedpermissions](https://img.shields.io/pypi/v/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-verifiedpermissions?color=blue)](https://pypistats.org/packages/types-aiobotocore-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -326,85 +325,86 @@
 )
 
 
 def check_value(value: DecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_verifiedpermissions.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    UpdatePolicyOutputTypeDef,
     ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
@@ -422,15 +422,15 @@
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
     CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
-def get_structure() -> ActionIdentifierTypeDef:
+def get_value() -> ActionIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/README.md` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-verifiedpermissions"></a>
 
 # types-aiobotocore-verifiedpermissions
 
 [![PyPI - types-aiobotocore-verifiedpermissions](https://img.shields.io/pypi/v/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-verifiedpermissions?color=blue)](https://pypistats.org/packages/types-aiobotocore-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -293,85 +293,86 @@
 )
 
 
 def check_value(value: DecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_verifiedpermissions.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    UpdatePolicyOutputTypeDef,
     ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
@@ -389,15 +390,15 @@
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
     CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
-def get_structure() -> ActionIdentifierTypeDef:
+def get_value() -> ActionIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/setup.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-verifiedpermissions",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        " mypy-boto3-builder 7.17.1"
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
-    keywords=(
-        "aiobotocore verifiedpermissions type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore verifiedpermissions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_verifiedpermissions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__init__.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__init__.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/__main__.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.VerifiedPermissions 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/client.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/client.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/literals.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/literals.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/paginator.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
 
@@ -85,43 +85,43 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
 
 class ListPolicyStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
 
 class ListPolicyTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/paginator.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filters: Sequence[IdentitySourceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIdentitySourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListIdentitySources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listidentitysourcespaginator)
         """
 
 class ListPoliciesPaginator(AioPaginator):
@@ -81,41 +81,41 @@
     """
 
     def paginate(
         self,
         *,
         policyStoreId: str,
         filter: PolicyFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyStoresPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyStoresOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyStores.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicystorespaginator)
         """
 
 class ListPolicyTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
     """
 
     def paginate(
-        self, *, policyStoreId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyStoreId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPolicyTemplatesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions.Paginator.ListPolicyTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/paginators/#listpolicytemplatespaginator)
         """
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/type_defs.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_verifiedpermissions.type_defs import ActionIdentifierTypeDef
 
-    data: ActionIdentifierTypeDef = {...}
+    data: ActionIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import DecisionType, PolicyTypeType, ValidationModeType
@@ -28,72 +28,72 @@
 
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ValidationSettingsTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
-    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "PutSchemaOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
-    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
-    "UpdatePolicyOutputTypeDef",
     "ConfigurationTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
+    "GetSchemaOutputTypeDef",
+    "PutSchemaOutputTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyOutputTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
@@ -155,43 +155,32 @@
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "statement": str,
     },
 )
@@ -208,25 +197,14 @@
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
 
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
 )
@@ -306,45 +284,21 @@
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
 
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -356,18 +310,20 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -382,36 +338,14 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -450,24 +384,14 @@
 
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalStaticPolicyDefinitionDetailTypeDef = TypedDict(
@@ -518,36 +442,14 @@
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
@@ -562,25 +464,14 @@
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
 
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalUpdateStaticPolicyDefinitionTypeDef = TypedDict(
@@ -594,25 +485,14 @@
 
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
     },
@@ -629,52 +509,27 @@
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -764,34 +619,149 @@
 
 class TemplateLinkedPolicyDefinitionTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
 ):
     pass
 
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+    },
+    total=False,
+)
+
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
     {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
@@ -815,15 +785,15 @@
     "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "validationSettings": ValidationSettingsTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -833,114 +803,144 @@
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputRequestTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputRequestTypeDef",
+    {
+        "nextToken": str,
+        "maxResults": int,
+        "filters": Sequence[IdentitySourceFilterTypeDef],
+    },
+    total=False,
+)
+
+
+class ListIdentitySourcesInputRequestTypeDef(
+    _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
+):
+    pass
+
+
+IdentitySourceItemTypeDef = TypedDict(
+    "IdentitySourceItemTypeDef",
+    {
+        "createdDate": datetime,
+        "details": IdentitySourceItemDetailsTypeDef,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "principalEntityType": str,
     },
 )
 
 _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
     "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     {
         "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
     _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputRequestTypeDef",
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     {
         "policyStoreId": str,
     },
 )
-_OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputRequestTypeDef",
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
-        "filters": Sequence[IdentitySourceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListIdentitySourcesInputRequestTypeDef(
-    _RequiredListIdentitySourcesInputRequestTypeDef, _OptionalListIdentitySourcesInputRequestTypeDef
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
 ):
     pass
 
 
-IdentitySourceItemTypeDef = TypedDict(
-    "IdentitySourceItemTypeDef",
-    {
-        "createdDate": datetime,
-        "details": IdentitySourceItemDetailsTypeDef,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "principalEntityType": str,
-    },
-)
-
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1035,15 +1035,15 @@
 
 
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1134,15 +1134,15 @@
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
@@ -1181,15 +1181,15 @@
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1237,10 +1237,10 @@
 
 
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions/type_defs.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_verifiedpermissions.type_defs import ActionIdentifierTypeDef
 
-    data: ActionIdentifierTypeDef = {...}
+    data: ActionIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import DecisionType, PolicyTypeType, ValidationModeType
@@ -27,72 +27,72 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionIdentifierTypeDef",
     "EntityIdentifierTypeDef",
     "CognitoUserPoolConfigurationTypeDef",
     "ContextDefinitionTypeDef",
-    "CreateIdentitySourceOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "ValidationSettingsTypeDef",
-    "CreatePolicyStoreOutputTypeDef",
     "CreatePolicyTemplateInputRequestTypeDef",
-    "CreatePolicyTemplateOutputTypeDef",
     "DeleteIdentitySourceInputRequestTypeDef",
     "DeletePolicyInputRequestTypeDef",
     "DeletePolicyStoreInputRequestTypeDef",
     "DeletePolicyTemplateInputRequestTypeDef",
     "DeterminingPolicyItemTypeDef",
     "EvaluationErrorItemTypeDef",
     "GetIdentitySourceInputRequestTypeDef",
     "IdentitySourceDetailsTypeDef",
     "GetPolicyInputRequestTypeDef",
     "GetPolicyStoreInputRequestTypeDef",
     "GetPolicyTemplateInputRequestTypeDef",
-    "GetPolicyTemplateOutputTypeDef",
     "GetSchemaInputRequestTypeDef",
-    "GetSchemaOutputTypeDef",
     "IdentitySourceFilterTypeDef",
     "IdentitySourceItemDetailsTypeDef",
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListPolicyStoresInputRequestTypeDef",
     "PolicyStoreItemTypeDef",
-    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyTemplatesInputRequestTypeDef",
     "PolicyTemplateItemTypeDef",
-    "PaginatorConfigTypeDef",
     "StaticPolicyDefinitionDetailTypeDef",
     "StaticPolicyDefinitionItemTypeDef",
     "StaticPolicyDefinitionTypeDef",
     "SchemaDefinitionTypeDef",
-    "PutSchemaOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateCognitoUserPoolConfigurationTypeDef",
-    "UpdateIdentitySourceOutputTypeDef",
     "UpdateStaticPolicyDefinitionTypeDef",
-    "UpdatePolicyStoreOutputTypeDef",
     "UpdatePolicyTemplateInputRequestTypeDef",
-    "UpdatePolicyTemplateOutputTypeDef",
     "AttributeValueTypeDef",
-    "CreatePolicyOutputTypeDef",
     "EntityItemTypeDef",
     "EntityReferenceTypeDef",
     "TemplateLinkedPolicyDefinitionDetailTypeDef",
     "TemplateLinkedPolicyDefinitionItemTypeDef",
     "TemplateLinkedPolicyDefinitionTypeDef",
-    "UpdatePolicyOutputTypeDef",
     "ConfigurationTypeDef",
+    "CreateIdentitySourceOutputTypeDef",
+    "CreatePolicyOutputTypeDef",
+    "CreatePolicyStoreOutputTypeDef",
+    "CreatePolicyTemplateOutputTypeDef",
+    "GetPolicyTemplateOutputTypeDef",
+    "GetSchemaOutputTypeDef",
+    "PutSchemaOutputTypeDef",
+    "UpdateIdentitySourceOutputTypeDef",
+    "UpdatePolicyOutputTypeDef",
+    "UpdatePolicyStoreOutputTypeDef",
+    "UpdatePolicyTemplateOutputTypeDef",
     "CreatePolicyStoreInputRequestTypeDef",
     "GetPolicyStoreOutputTypeDef",
     "UpdatePolicyStoreInputRequestTypeDef",
     "IsAuthorizedOutputTypeDef",
     "IsAuthorizedWithTokenOutputTypeDef",
     "GetIdentitySourceOutputTypeDef",
-    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
     "ListIdentitySourcesInputRequestTypeDef",
     "IdentitySourceItemTypeDef",
+    "ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    "ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
     "ListPolicyStoresOutputTypeDef",
     "ListPolicyTemplatesOutputTypeDef",
     "PutSchemaInputRequestTypeDef",
     "UpdateConfigurationTypeDef",
     "UpdatePolicyDefinitionTypeDef",
     "EntitiesDefinitionTypeDef",
     "PolicyFilterTypeDef",
@@ -152,43 +152,32 @@
     "ContextDefinitionTypeDef",
     {
         "contextMap": Mapping[str, "AttributeValueTypeDef"],
     },
     total=False,
 )
 
-CreateIdentitySourceOutputTypeDef = TypedDict(
-    "CreateIdentitySourceOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ValidationSettingsTypeDef = TypedDict(
     "ValidationSettingsTypeDef",
     {
         "mode": ValidationModeType,
     },
 )
 
-CreatePolicyStoreOutputTypeDef = TypedDict(
-    "CreatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "statement": str,
     },
 )
@@ -203,25 +192,14 @@
 
 class CreatePolicyTemplateInputRequestTypeDef(
     _RequiredCreatePolicyTemplateInputRequestTypeDef,
     _OptionalCreatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-CreatePolicyTemplateOutputTypeDef = TypedDict(
-    "CreatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteIdentitySourceInputRequestTypeDef = TypedDict(
     "DeleteIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
         "identitySourceId": str,
     },
 )
@@ -301,45 +279,21 @@
     "GetPolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
     },
 )
 
-GetPolicyTemplateOutputTypeDef = TypedDict(
-    "GetPolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "description": str,
-        "statement": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSchemaInputRequestTypeDef = TypedDict(
     "GetSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 
-GetSchemaOutputTypeDef = TypedDict(
-    "GetSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "schema": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentitySourceFilterTypeDef = TypedDict(
     "IdentitySourceFilterTypeDef",
     {
         "principalEntityType": str,
     },
     total=False,
 )
@@ -351,18 +305,20 @@
         "userPoolArn": str,
         "discoveryUrl": str,
         "openIdIssuer": Literal["COGNITO"],
     },
     total=False,
 )
 
-ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
-    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListPolicyStoresInputRequestTypeDef = TypedDict(
     "ListPolicyStoresInputRequestTypeDef",
     {
@@ -377,34 +333,14 @@
     {
         "policyStoreId": str,
         "arn": str,
         "createdDate": datetime,
     },
 )
 
-_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
-    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyTemplatesInputRequestTypeDef = TypedDict(
     "_RequiredListPolicyTemplatesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListPolicyTemplatesInputRequestTypeDef = TypedDict(
@@ -439,24 +375,14 @@
 )
 
 class PolicyTemplateItemTypeDef(
     _RequiredPolicyTemplateItemTypeDef, _OptionalPolicyTemplateItemTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 _RequiredStaticPolicyDefinitionDetailTypeDef = TypedDict(
     "_RequiredStaticPolicyDefinitionDetailTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalStaticPolicyDefinitionDetailTypeDef = TypedDict(
@@ -503,36 +429,14 @@
     "SchemaDefinitionTypeDef",
     {
         "cedarJson": str,
     },
     total=False,
 )
 
-PutSchemaOutputTypeDef = TypedDict(
-    "PutSchemaOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "namespaces": List[str],
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
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
 _RequiredUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
     "_RequiredUpdateCognitoUserPoolConfigurationTypeDef",
     {
         "userPoolArn": str,
     },
 )
 _OptionalUpdateCognitoUserPoolConfigurationTypeDef = TypedDict(
@@ -545,25 +449,14 @@
 
 class UpdateCognitoUserPoolConfigurationTypeDef(
     _RequiredUpdateCognitoUserPoolConfigurationTypeDef,
     _OptionalUpdateCognitoUserPoolConfigurationTypeDef,
 ):
     pass
 
-UpdateIdentitySourceOutputTypeDef = TypedDict(
-    "UpdateIdentitySourceOutputTypeDef",
-    {
-        "createdDate": datetime,
-        "identitySourceId": str,
-        "lastUpdatedDate": datetime,
-        "policyStoreId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateStaticPolicyDefinitionTypeDef = TypedDict(
     "_RequiredUpdateStaticPolicyDefinitionTypeDef",
     {
         "statement": str,
     },
 )
 _OptionalUpdateStaticPolicyDefinitionTypeDef = TypedDict(
@@ -575,25 +468,14 @@
 )
 
 class UpdateStaticPolicyDefinitionTypeDef(
     _RequiredUpdateStaticPolicyDefinitionTypeDef, _OptionalUpdateStaticPolicyDefinitionTypeDef
 ):
     pass
 
-UpdatePolicyStoreOutputTypeDef = TypedDict(
-    "UpdatePolicyStoreOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "arn": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePolicyTemplateInputRequestTypeDef = TypedDict(
     "_RequiredUpdatePolicyTemplateInputRequestTypeDef",
     {
         "policyStoreId": str,
         "policyTemplateId": str,
         "statement": str,
     },
@@ -608,52 +490,27 @@
 
 class UpdatePolicyTemplateInputRequestTypeDef(
     _RequiredUpdatePolicyTemplateInputRequestTypeDef,
     _OptionalUpdatePolicyTemplateInputRequestTypeDef,
 ):
     pass
 
-UpdatePolicyTemplateOutputTypeDef = TypedDict(
-    "UpdatePolicyTemplateOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyTemplateId": str,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AttributeValueTypeDef = TypedDict(
     "AttributeValueTypeDef",
     {
         "boolean": bool,
         "entityIdentifier": EntityIdentifierTypeDef,
         "long": int,
         "string": str,
         "set": Sequence[Dict[str, Any]],
         "record": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-CreatePolicyOutputTypeDef = TypedDict(
-    "CreatePolicyOutputTypeDef",
-    {
-        "policyStoreId": str,
-        "policyId": str,
-        "policyType": PolicyTypeType,
-        "principal": EntityIdentifierTypeDef,
-        "resource": EntityIdentifierTypeDef,
-        "createdDate": datetime,
-        "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEntityItemTypeDef = TypedDict(
     "_RequiredEntityItemTypeDef",
     {
         "identifier": EntityIdentifierTypeDef,
     },
 )
 _OptionalEntityItemTypeDef = TypedDict(
@@ -735,34 +592,149 @@
 )
 
 class TemplateLinkedPolicyDefinitionTypeDef(
     _RequiredTemplateLinkedPolicyDefinitionTypeDef, _OptionalTemplateLinkedPolicyDefinitionTypeDef
 ):
     pass
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+    },
+    total=False,
+)
+
+CreateIdentitySourceOutputTypeDef = TypedDict(
+    "CreateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyOutputTypeDef = TypedDict(
+    "CreatePolicyOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyId": str,
+        "policyType": PolicyTypeType,
+        "principal": EntityIdentifierTypeDef,
+        "resource": EntityIdentifierTypeDef,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyStoreOutputTypeDef = TypedDict(
+    "CreatePolicyStoreOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyTemplateOutputTypeDef = TypedDict(
+    "CreatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyTemplateOutputTypeDef = TypedDict(
+    "GetPolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "description": str,
+        "statement": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSchemaOutputTypeDef = TypedDict(
+    "GetSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "schema": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSchemaOutputTypeDef = TypedDict(
+    "PutSchemaOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "namespaces": List[str],
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIdentitySourceOutputTypeDef = TypedDict(
+    "UpdateIdentitySourceOutputTypeDef",
+    {
+        "createdDate": datetime,
+        "identitySourceId": str,
+        "lastUpdatedDate": datetime,
+        "policyStoreId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePolicyOutputTypeDef = TypedDict(
     "UpdatePolicyOutputTypeDef",
     {
         "policyStoreId": str,
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
+UpdatePolicyStoreOutputTypeDef = TypedDict(
+    "UpdatePolicyStoreOutputTypeDef",
     {
-        "cognitoUserPoolConfiguration": CognitoUserPoolConfigurationTypeDef,
+        "policyStoreId": str,
+        "arn": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePolicyTemplateOutputTypeDef = TypedDict(
+    "UpdatePolicyTemplateOutputTypeDef",
+    {
+        "policyStoreId": str,
+        "policyTemplateId": str,
+        "createdDate": datetime,
+        "lastUpdatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreatePolicyStoreInputRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyStoreInputRequestTypeDef",
     {
         "validationSettings": ValidationSettingsTypeDef,
     },
@@ -784,15 +756,15 @@
     "GetPolicyStoreOutputTypeDef",
     {
         "policyStoreId": str,
         "arn": str,
         "validationSettings": ValidationSettingsTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePolicyStoreInputRequestTypeDef = TypedDict(
     "UpdatePolicyStoreInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -802,62 +774,41 @@
 
 IsAuthorizedOutputTypeDef = TypedDict(
     "IsAuthorizedOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IsAuthorizedWithTokenOutputTypeDef = TypedDict(
     "IsAuthorizedWithTokenOutputTypeDef",
     {
         "decision": DecisionType,
         "determiningPolicies": List[DeterminingPolicyItemTypeDef],
         "errors": List[EvaluationErrorItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentitySourceOutputTypeDef = TypedDict(
     "GetIdentitySourceOutputTypeDef",
     {
         "createdDate": datetime,
         "details": IdentitySourceDetailsTypeDef,
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "policyStoreId": str,
-    },
-)
-_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
-    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
-    {
-        "filters": Sequence[IdentitySourceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
-    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListIdentitySourcesInputRequestTypeDef = TypedDict(
     "_RequiredListIdentitySourcesInputRequestTypeDef",
     {
         "policyStoreId": str,
     },
 )
 _OptionalListIdentitySourcesInputRequestTypeDef = TypedDict(
@@ -883,29 +834,78 @@
         "identitySourceId": str,
         "lastUpdatedDate": datetime,
         "policyStoreId": str,
         "principalEntityType": str,
     },
 )
 
+_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef = TypedDict(
+    "_OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef",
+    {
+        "filters": Sequence[IdentitySourceFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef(
+    _RequiredListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    _OptionalListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+):
+    pass
+
+ListPolicyStoresInputListPolicyStoresPaginateTypeDef = TypedDict(
+    "ListPolicyStoresInputListPolicyStoresPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "policyStoreId": str,
+    },
+)
+_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef(
+    _RequiredListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+    _OptionalListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
+):
+    pass
+
 ListPolicyStoresOutputTypeDef = TypedDict(
     "ListPolicyStoresOutputTypeDef",
     {
         "nextToken": str,
         "policyStores": List[PolicyStoreItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyTemplatesOutputTypeDef = TypedDict(
     "ListPolicyTemplatesOutputTypeDef",
     {
         "nextToken": str,
         "policyTemplates": List[PolicyTemplateItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutSchemaInputRequestTypeDef = TypedDict(
     "PutSchemaInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -998,15 +998,15 @@
     pass
 
 ListIdentitySourcesOutputTypeDef = TypedDict(
     "ListIdentitySourcesOutputTypeDef",
     {
         "nextToken": str,
         "identitySources": List[IdentitySourceItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateIdentitySourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateIdentitySourceInputRequestTypeDef",
     {
         "policyStoreId": str,
@@ -1091,15 +1091,15 @@
         "policyStoreId": str,
     },
 )
 _OptionalListPoliciesInputListPoliciesPaginateTypeDef = TypedDict(
     "_OptionalListPoliciesInputListPoliciesPaginateTypeDef",
     {
         "filter": PolicyFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListPoliciesInputListPoliciesPaginateTypeDef(
     _RequiredListPoliciesInputListPoliciesPaginateTypeDef,
     _OptionalListPoliciesInputListPoliciesPaginateTypeDef,
@@ -1134,15 +1134,15 @@
         "policyId": str,
         "policyType": PolicyTypeType,
         "principal": EntityIdentifierTypeDef,
         "resource": EntityIdentifierTypeDef,
         "definition": PolicyDefinitionDetailTypeDef,
         "createdDate": datetime,
         "lastUpdatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPolicyItemTypeDef = TypedDict(
     "_RequiredPolicyItemTypeDef",
     {
         "policyStoreId": str,
@@ -1186,10 +1186,10 @@
     pass
 
 ListPoliciesOutputTypeDef = TypedDict(
     "ListPoliciesOutputTypeDef",
     {
         "nextToken": str,
         "policies": List[PolicyItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-verifiedpermissions
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore verifiedpermissions type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore verifiedpermissions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-verifiedpermissions"></a>
 
 # types-aiobotocore-verifiedpermissions
 
 [![PyPI - types-aiobotocore-verifiedpermissions](https://img.shields.io/pypi/v/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-verifiedpermissions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-verifiedpermissions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-verifiedpermissions?color=blue)](https://pypistats.org/packages/types-aiobotocore-verifiedpermissions)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-verifiedpermissions)](https://pepy.tech/project/types-aiobotocore-verifiedpermissions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VerifiedPermissions 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions)
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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -326,85 +325,86 @@
 )
 
 
 def check_value(value: DecisionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_verifiedpermissions.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_verifiedpermissions.type_defs import (
     ActionIdentifierTypeDef,
     EntityIdentifierTypeDef,
     CognitoUserPoolConfigurationTypeDef,
     ContextDefinitionTypeDef,
-    CreateIdentitySourceOutputTypeDef,
+    ResponseMetadataTypeDef,
     ValidationSettingsTypeDef,
-    CreatePolicyStoreOutputTypeDef,
     CreatePolicyTemplateInputRequestTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
     DeleteIdentitySourceInputRequestTypeDef,
     DeletePolicyInputRequestTypeDef,
     DeletePolicyStoreInputRequestTypeDef,
     DeletePolicyTemplateInputRequestTypeDef,
     DeterminingPolicyItemTypeDef,
     EvaluationErrorItemTypeDef,
     GetIdentitySourceInputRequestTypeDef,
     IdentitySourceDetailsTypeDef,
     GetPolicyInputRequestTypeDef,
     GetPolicyStoreInputRequestTypeDef,
     GetPolicyTemplateInputRequestTypeDef,
-    GetPolicyTemplateOutputTypeDef,
     GetSchemaInputRequestTypeDef,
-    GetSchemaOutputTypeDef,
     IdentitySourceFilterTypeDef,
     IdentitySourceItemDetailsTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListPolicyStoresInputRequestTypeDef,
     PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyTemplatesInputRequestTypeDef,
     PolicyTemplateItemTypeDef,
-    PaginatorConfigTypeDef,
     StaticPolicyDefinitionDetailTypeDef,
     StaticPolicyDefinitionItemTypeDef,
     StaticPolicyDefinitionTypeDef,
     SchemaDefinitionTypeDef,
-    PutSchemaOutputTypeDef,
-    ResponseMetadataTypeDef,
     UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
     UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
     UpdatePolicyTemplateInputRequestTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
     AttributeValueTypeDef,
-    CreatePolicyOutputTypeDef,
     EntityItemTypeDef,
     EntityReferenceTypeDef,
     TemplateLinkedPolicyDefinitionDetailTypeDef,
     TemplateLinkedPolicyDefinitionItemTypeDef,
     TemplateLinkedPolicyDefinitionTypeDef,
-    UpdatePolicyOutputTypeDef,
     ConfigurationTypeDef,
+    CreateIdentitySourceOutputTypeDef,
+    CreatePolicyOutputTypeDef,
+    CreatePolicyStoreOutputTypeDef,
+    CreatePolicyTemplateOutputTypeDef,
+    GetPolicyTemplateOutputTypeDef,
+    GetSchemaOutputTypeDef,
+    PutSchemaOutputTypeDef,
+    UpdateIdentitySourceOutputTypeDef,
+    UpdatePolicyOutputTypeDef,
+    UpdatePolicyStoreOutputTypeDef,
+    UpdatePolicyTemplateOutputTypeDef,
     CreatePolicyStoreInputRequestTypeDef,
     GetPolicyStoreOutputTypeDef,
     UpdatePolicyStoreInputRequestTypeDef,
     IsAuthorizedOutputTypeDef,
     IsAuthorizedWithTokenOutputTypeDef,
     GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
     ListIdentitySourcesInputRequestTypeDef,
     IdentitySourceItemTypeDef,
+    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
+    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
+    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
     ListPolicyStoresOutputTypeDef,
     ListPolicyTemplatesOutputTypeDef,
     PutSchemaInputRequestTypeDef,
     UpdateConfigurationTypeDef,
     UpdatePolicyDefinitionTypeDef,
     EntitiesDefinitionTypeDef,
     PolicyFilterTypeDef,
@@ -422,15 +422,15 @@
     GetPolicyOutputTypeDef,
     PolicyItemTypeDef,
     CreatePolicyInputRequestTypeDef,
     ListPoliciesOutputTypeDef,
 )
 
 
-def get_structure() -> ActionIdentifierTypeDef:
+def get_value() -> ActionIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt` & `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

