# Comparing `tmp/types-aiobotocore-amplifyuibuilder-2.5.2.tar.gz` & `tmp/types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.tar` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.241650 types-aiobotocore-amplifyuibuilder-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-07-08 01:43:12.241650 types-aiobotocore-amplifyuibuilder-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17131 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.241650 types-aiobotocore-amplifyuibuilder-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.225650 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23816 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23775 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-07-08 01:25:29.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-08 01:25:29.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48035 2023-07-08 01:25:30.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47943 2023-07-08 01:25:30.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:28.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.241650 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18732 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:12.000000 types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.433660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.433660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58612 2023-08-02 14:32:56.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58502 2023-08-02 14:32:56.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/LICENSE` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/PKG-INFO` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifyuibuilder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplifyuibuilder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplifyuibuilder"></a>
 
 # types-aiobotocore-amplifyuibuilder
 
 [![PyPI - types-aiobotocore-amplifyuibuilder](https://img.shields.io/pypi/v/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifyuibuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [types-aiobotocore-amplifyuibuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/).
 
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
@@ -344,144 +343,166 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifyuibuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifyuibuilder.type_defs import (
-    ActionParametersTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
+    UpdateThemeDataTypeDef,
+    ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
+    ValueMappingsOutputTypeDef,
+    ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
     UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
     UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
-    UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingTypeDef,
-    ValueMappingsTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/README.md` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-amplifyuibuilder"></a>
 
 # types-aiobotocore-amplifyuibuilder
 
 [![PyPI - types-aiobotocore-amplifyuibuilder](https://img.shields.io/pypi/v/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifyuibuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [types-aiobotocore-amplifyuibuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/).
 
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
@@ -311,144 +311,166 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifyuibuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifyuibuilder.type_defs import (
-    ActionParametersTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
+    UpdateThemeDataTypeDef,
+    ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
+    ValueMappingsOutputTypeDef,
+    ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
     UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
     UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
-    UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingTypeDef,
-    ValueMappingsTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/setup.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifyuibuilder",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with"
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
-    keywords="aiobotocore amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore amplifyuibuilder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_amplifyuibuilder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/"
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__init__.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__init__.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/__main__.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/client.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,45 +126,45 @@
         """
 
     async def create_component(
         self,
         *,
         appId: str,
         environmentName: str,
-        componentToCreate: "CreateComponentDataTypeDef",
+        componentToCreate: CreateComponentDataTypeDef,
         clientToken: str = ...
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_component)
         """
 
     async def create_form(
         self,
         *,
         appId: str,
         environmentName: str,
-        formToCreate: "CreateFormDataTypeDef",
+        formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
         Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_form)
         """
 
     async def create_theme(
         self,
         *,
         appId: str,
         environmentName: str,
-        themeToCreate: "CreateThemeDataTypeDef",
+        themeToCreate: CreateThemeDataTypeDef,
         clientToken: str = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme to apply to the components in an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_theme)
@@ -197,15 +197,15 @@
         Deletes a theme from an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#delete_theme)
         """
 
     async def exchange_code_for_token(
-        self, *, provider: Literal["figma"], request: "ExchangeCodeForTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], request: ExchangeCodeForTokenRequestBodyTypeDef
     ) -> ExchangeCodeForTokenResponseTypeDef:
         """
         Exchanges an access code for a token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#exchange_code_for_token)
         """
@@ -349,39 +349,39 @@
 
     async def put_metadata_flag(
         self,
         *,
         appId: str,
         environmentName: str,
         featureName: str,
-        body: "PutMetadataFlagBodyTypeDef"
+        body: PutMetadataFlagBodyTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Stores the metadata information about a feature on a form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.put_metadata_flag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#put_metadata_flag)
         """
 
     async def refresh_token(
-        self, *, provider: Literal["figma"], refreshTokenBody: "RefreshTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], refreshTokenBody: RefreshTokenRequestBodyTypeDef
     ) -> RefreshTokenResponseTypeDef:
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#refresh_token)
         """
 
     async def start_codegen_job(
         self,
         *,
         appId: str,
         environmentName: str,
-        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
         Starts a code generation job for for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
@@ -390,15 +390,15 @@
 
     async def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedComponent: "UpdateComponentDataTypeDef",
+        updatedComponent: UpdateComponentDataTypeDef,
         clientToken: str = ...
     ) -> UpdateComponentResponseTypeDef:
         """
         Updates an existing component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_component)
@@ -406,15 +406,15 @@
 
     async def update_form(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedForm: "UpdateFormDataTypeDef",
+        updatedForm: UpdateFormDataTypeDef,
         clientToken: str = ...
     ) -> UpdateFormResponseTypeDef:
         """
         Updates an existing form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_form)
@@ -422,15 +422,15 @@
 
     async def update_theme(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedTheme: "UpdateThemeDataTypeDef",
+        updatedTheme: UpdateThemeDataTypeDef,
         clientToken: str = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates an existing theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_theme)
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/client.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -119,43 +119,43 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#close)
         """
     async def create_component(
         self,
         *,
         appId: str,
         environmentName: str,
-        componentToCreate: "CreateComponentDataTypeDef",
+        componentToCreate: CreateComponentDataTypeDef,
         clientToken: str = ...
     ) -> CreateComponentResponseTypeDef:
         """
         Creates a new component for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_component)
         """
     async def create_form(
         self,
         *,
         appId: str,
         environmentName: str,
-        formToCreate: "CreateFormDataTypeDef",
+        formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
         Creates a new form for an Amplify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_form)
         """
     async def create_theme(
         self,
         *,
         appId: str,
         environmentName: str,
-        themeToCreate: "CreateThemeDataTypeDef",
+        themeToCreate: CreateThemeDataTypeDef,
         clientToken: str = ...
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme to apply to the components in an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#create_theme)
@@ -184,15 +184,15 @@
         """
         Deletes a theme from an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.delete_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#delete_theme)
         """
     async def exchange_code_for_token(
-        self, *, provider: Literal["figma"], request: "ExchangeCodeForTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], request: ExchangeCodeForTokenRequestBodyTypeDef
     ) -> ExchangeCodeForTokenResponseTypeDef:
         """
         Exchanges an access code for a token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.exchange_code_for_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#exchange_code_for_token)
         """
@@ -322,37 +322,37 @@
         """
     async def put_metadata_flag(
         self,
         *,
         appId: str,
         environmentName: str,
         featureName: str,
-        body: "PutMetadataFlagBodyTypeDef"
+        body: PutMetadataFlagBodyTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Stores the metadata information about a feature on a form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.put_metadata_flag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#put_metadata_flag)
         """
     async def refresh_token(
-        self, *, provider: Literal["figma"], refreshTokenBody: "RefreshTokenRequestBodyTypeDef"
+        self, *, provider: Literal["figma"], refreshTokenBody: RefreshTokenRequestBodyTypeDef
     ) -> RefreshTokenResponseTypeDef:
         """
         Refreshes a previously issued access token that might have expired.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.refresh_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#refresh_token)
         """
     async def start_codegen_job(
         self,
         *,
         appId: str,
         environmentName: str,
-        codegenJobToCreate: "StartCodegenJobDataTypeDef",
+        codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
         Starts a code generation job for for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
@@ -360,45 +360,45 @@
         """
     async def update_component(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedComponent: "UpdateComponentDataTypeDef",
+        updatedComponent: UpdateComponentDataTypeDef,
         clientToken: str = ...
     ) -> UpdateComponentResponseTypeDef:
         """
         Updates an existing component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_component)
         """
     async def update_form(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedForm: "UpdateFormDataTypeDef",
+        updatedForm: UpdateFormDataTypeDef,
         clientToken: str = ...
     ) -> UpdateFormResponseTypeDef:
         """
         Updates an existing form.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_form)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_form)
         """
     async def update_theme(
         self,
         *,
         appId: str,
         environmentName: str,
         id: str,
-        updatedTheme: "UpdateThemeDataTypeDef",
+        updatedTheme: UpdateThemeDataTypeDef,
         clientToken: str = ...
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates an existing theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.update_theme)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/client/#update_theme)
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/literals.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/literals.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/paginator.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,103 +72,103 @@
 class ExportComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
 
 class ExportFormsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
 
 class ExportThemesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
 
 class ListCodegenJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcodegenjobspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCodegenJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcodegenjobspaginator)
         """
 
 
 class ListComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
 
 class ListFormsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listformspaginator)
         """
 
 
 class ListThemesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listthemespaginator)
         """
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/paginator.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -69,97 +69,97 @@
 class ExportComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportcomponentspaginator)
         """
 
 class ExportFormsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportForms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportformspaginator)
         """
 
 class ExportThemesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ExportThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#exportthemespaginator)
         """
 
 class ListCodegenJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcodegenjobspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCodegenJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListCodegenJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcodegenjobspaginator)
         """
 
 class ListComponentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcomponentspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listcomponentspaginator)
         """
 
 class ListFormsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listformspaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFormsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListForms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listformspaginator)
         """
 
 class ListThemesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listthemespaginator)
     """
 
     def paginate(
-        self, *, appId: str, environmentName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appId: str, environmentName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThemesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/paginators/#listthemespaginator)
         """
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/type_defs.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplifyuibuilder.type_defs import ActionParametersTypeDef
+    from types_aiobotocore_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: ActionParametersTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,235 +37,232 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ActionParametersTypeDef",
+    "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataFieldTypeDef",
-    "CodegenGenericDataModelTypeDef",
-    "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "CodegenJobGenericDataSchemaTypeDef",
-    "CodegenJobRenderConfigTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "CodegenJobTypeDef",
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
-    "ComponentBindingPropertiesValueTypeDef",
-    "ComponentChildTypeDef",
     "ComponentConditionPropertyTypeDef",
-    "ComponentDataConfigurationTypeDef",
-    "ComponentEventTypeDef",
+    "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
-    "ComponentPropertyTypeDef",
+    "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentTypeDef",
+    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
-    "CreateComponentDataTypeDef",
-    "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateFormDataTypeDef",
-    "CreateFormRequestRequestTypeDef",
-    "CreateFormResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
-    "CreateThemeRequestRequestTypeDef",
-    "CreateThemeResponseTypeDef",
+    "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
-    "ExchangeCodeForTokenRequestRequestTypeDef",
-    "ExchangeCodeForTokenResponseTypeDef",
-    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
-    "ExportComponentsResponseTypeDef",
-    "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
-    "ExportFormsResponseTypeDef",
-    "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
-    "ExportThemesResponseTypeDef",
-    "FieldConfigTypeDef",
-    "FieldInputConfigTypeDef",
     "FieldPositionTypeDef",
+    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
+    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
-    "FormBindingElementTypeDef",
-    "FormButtonTypeDef",
-    "FormCTATypeDef",
-    "FormDataTypeConfigTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
-    "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
-    "FormInputValuePropertyTypeDef",
     "FormStyleConfigTypeDef",
-    "FormStyleTypeDef",
-    "FormSummaryTypeDef",
-    "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
-    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
-    "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
-    "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
-    "GetThemeResponseTypeDef",
-    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
-    "ListCodegenJobsResponseTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListComponentsResponseTypeDef",
-    "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
-    "ListFormsResponseTypeDef",
-    "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
-    "ListThemesResponseTypeDef",
-    "MutationActionSetStateParameterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ThemeSummaryTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
-    "PutMetadataFlagRequestRequestTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "RefreshTokenRequestRequestTypeDef",
-    "RefreshTokenResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SectionalElementTypeDef",
-    "SortPropertyTypeDef",
-    "StartCodegenJobDataTypeDef",
-    "StartCodegenJobRequestRequestTypeDef",
-    "StartCodegenJobResponseTypeDef",
-    "ThemeSummaryTypeDef",
-    "ThemeTypeDef",
+    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
+    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
+    "UpdateThemeDataTypeDef",
+    "ValueMappingTypeDef",
+    "ActionParametersOutputTypeDef",
+    "ActionParametersTypeDef",
+    "CodegenGenericDataFieldOutputTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValueTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
+    "ComponentDataConfigurationTypeDef",
+    "ComponentPropertyOutputTypeDef",
+    "ComponentPropertyTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExchangeCodeForTokenResponseTypeDef",
+    "GetMetadataResponseTypeDef",
+    "ListCodegenJobsResponseTypeDef",
+    "ListComponentsResponseTypeDef",
+    "RefreshTokenResponseTypeDef",
+    "FormSummaryTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "CreateThemeResponseTypeDef",
+    "ExportThemesResponseTypeDef",
+    "GetThemeResponseTypeDef",
+    "UpdateThemeResponseTypeDef",
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "ExportFormsRequestExportFormsPaginateTypeDef",
+    "ExportThemesRequestExportThemesPaginateTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListFormsRequestListFormsPaginateTypeDef",
+    "ListThemesRequestListThemesPaginateTypeDef",
+    "FormButtonTypeDef",
+    "SectionalElementTypeDef",
+    "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyTypeDef",
+    "FormStyleTypeDef",
+    "ListThemesResponseTypeDef",
+    "PutMetadataFlagRequestRequestTypeDef",
+    "RefreshTokenRequestRequestTypeDef",
+    "UpdateThemeRequestRequestTypeDef",
+    "ComponentEventOutputTypeDef",
+    "ComponentEventTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "ListFormsResponseTypeDef",
+    "FormCTATypeDef",
+    "ValueMappingsOutputTypeDef",
+    "ValueMappingsTypeDef",
+    "ComponentChildOutputTypeDef",
+    "ComponentTypeDef",
+    "ComponentChildTypeDef",
+    "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
-    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "FieldInputConfigOutputTypeDef",
+    "FieldInputConfigTypeDef",
+    "CreateComponentResponseTypeDef",
+    "ExportComponentsResponseTypeDef",
+    "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
+    "CreateComponentRequestRequestTypeDef",
+    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "FieldConfigOutputTypeDef",
+    "FieldConfigTypeDef",
+    "GetCodegenJobResponseTypeDef",
+    "StartCodegenJobResponseTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "FormTypeDef",
+    "CreateFormDataTypeDef",
     "UpdateFormDataTypeDef",
-    "UpdateFormRequestRequestTypeDef",
+    "CreateFormResponseTypeDef",
+    "ExportFormsResponseTypeDef",
+    "GetFormResponseTypeDef",
     "UpdateFormResponseTypeDef",
-    "UpdateThemeDataTypeDef",
-    "UpdateThemeRequestRequestTypeDef",
-    "UpdateThemeResponseTypeDef",
-    "ValueMappingTypeDef",
-    "ValueMappingsTypeDef",
+    "CreateFormRequestRequestTypeDef",
+    "UpdateFormRequestRequestTypeDef",
 )
 
-ActionParametersTypeDef = TypedDict(
-    "ActionParametersTypeDef",
+MutationActionSetStateParameterTypeDef = TypedDict(
+    "MutationActionSetStateParameterTypeDef",
     {
-        "type": "ComponentPropertyTypeDef",
-        "url": "ComponentPropertyTypeDef",
-        "anchor": "ComponentPropertyTypeDef",
-        "target": "ComponentPropertyTypeDef",
-        "global": "ComponentPropertyTypeDef",
-        "model": str,
-        "id": "ComponentPropertyTypeDef",
-        "fields": Mapping[str, "ComponentPropertyTypeDef"],
-        "state": "MutationActionSetStateParameterTypeDef",
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyTypeDef",
     },
-    total=False,
 )
 
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
-CodegenGenericDataEnumTypeDef = TypedDict(
-    "CodegenGenericDataEnumTypeDef",
+CodegenGenericDataEnumOutputTypeDef = TypedDict(
+    "CodegenGenericDataEnumOutputTypeDef",
     {
         "values": List[str],
     },
 )
 
-_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldTypeDef",
+CodegenGenericDataEnumTypeDef = TypedDict(
+    "CodegenGenericDataEnumTypeDef",
     {
-        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
+        "values": Sequence[str],
     },
-    total=False,
 )
 
-
-class CodegenGenericDataFieldTypeDef(
-    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
-):
-    pass
-
-
-_RequiredCodegenGenericDataModelTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelTypeDef",
+_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": List[str],
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
     },
 )
-_OptionalCodegenGenericDataModelTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelTypeDef",
+_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
-        "isJoinTable": bool,
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
     },
     total=False,
 )
 
 
-class CodegenGenericDataModelTypeDef(
-    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+class CodegenGenericDataRelationshipTypeOutputTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
 ):
     pass
 
 
-CodegenGenericDataNonModelTypeDef = TypedDict(
-    "CodegenGenericDataNonModelTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-    },
-)
-
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": List[str],
+        "relatedModelFields": Sequence[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
+        "associatedFields": Sequence[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 
 class CodegenGenericDataRelationshipTypeTypeDef(
@@ -279,28 +276,22 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
-    },
-)
-
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
     {
-        "react": "ReactStartCodegenJobDataTypeDef",
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
     },
     total=False,
 )
 
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
@@ -321,44 +312,29 @@
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
 
-_RequiredCodegenJobTypeDef = TypedDict(
-    "_RequiredCodegenJobTypeDef",
+ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     {
-        "id": str,
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalCodegenJobTypeDef = TypedDict(
-    "_OptionalCodegenJobTypeDef",
-    {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "status": CodegenJobStatusType,
-        "statusMessage": str,
-        "asset": "CodegenJobAssetTypeDef",
-        "tags": Dict[str, str],
-        "createdAt": datetime,
-        "modifiedAt": datetime,
+        "model": str,
+        "field": str,
+        "predicates": List["PredicateOutputTypeDef"],
+        "userAttribute": str,
+        "bucket": str,
+        "key": str,
+        "defaultValue": str,
+        "slotName": str,
     },
     total=False,
 )
 
-
-class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
-    pass
-
-
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -366,92 +342,34 @@
         "key": str,
         "defaultValue": str,
         "slotName": str,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
-        "defaultValue": str,
-    },
-    total=False,
-)
-
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-    },
-)
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
-    {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
-    pass
-
-
 ComponentConditionPropertyTypeDef = TypedDict(
     "ComponentConditionPropertyTypeDef",
     {
         "property": str,
         "field": str,
         "operator": str,
         "operand": str,
         "then": Dict[str, Any],
         "else": Dict[str, Any],
         "operandType": str,
     },
     total=False,
 )
 
-_RequiredComponentDataConfigurationTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationTypeDef",
-    {
-        "sort": Sequence["SortPropertyTypeDef"],
-        "predicate": "PredicateTypeDef",
-        "identifiers": Sequence[str],
-    },
-    total=False,
-)
-
-
-class ComponentDataConfigurationTypeDef(
-    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
-):
-    pass
-
-
-ComponentEventTypeDef = TypedDict(
-    "ComponentEventTypeDef",
+SortPropertyTypeDef = TypedDict(
+    "SortPropertyTypeDef",
     {
-        "action": str,
-        "parameters": "ActionParametersTypeDef",
-        "bindingEvent": str,
+        "field": str,
+        "direction": SortDirectionType,
     },
-    total=False,
 )
 
 _RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
@@ -468,1328 +386,1688 @@
 class ComponentPropertyBindingPropertiesTypeDef(
     _RequiredComponentPropertyBindingPropertiesTypeDef,
     _OptionalComponentPropertyBindingPropertiesTypeDef,
 ):
     pass
 
 
-ComponentPropertyTypeDef = TypedDict(
-    "ComponentPropertyTypeDef",
+FormBindingElementTypeDef = TypedDict(
+    "FormBindingElementTypeDef",
     {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Mapping[str, "FormBindingElementTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": Sequence[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
+        "element": str,
         "property": str,
     },
-    total=False,
 )
 
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
+ComponentVariantOutputTypeDef = TypedDict(
+    "ComponentVariantOutputTypeDef",
+    {
+        "variantValues": Dict[str, str],
+        "overrides": Dict[str, Dict[str, str]],
+    },
+    total=False,
+)
+
+ComponentVariantTypeDef = TypedDict(
+    "ComponentVariantTypeDef",
+    {
+        "variantValues": Mapping[str, str],
+        "overrides": Mapping[str, Mapping[str, str]],
+    },
+    total=False,
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+FormDataTypeConfigTypeDef = TypedDict(
+    "FormDataTypeConfigTypeDef",
+    {
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
+    },
+)
+
+_RequiredCreateThemeDataTypeDef = TypedDict(
+    "_RequiredCreateThemeDataTypeDef",
+    {
+        "name": str,
+        "values": Sequence["ThemeValuesTypeDef"],
+    },
+)
+_OptionalCreateThemeDataTypeDef = TypedDict(
+    "_OptionalCreateThemeDataTypeDef",
+    {
+        "overrides": Sequence["ThemeValuesTypeDef"],
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
+    pass
+
+
+_RequiredThemeTypeDef = TypedDict(
+    "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
-        "componentType": str,
-        "properties": Dict[str, "ComponentPropertyTypeDef"],
-        "variants": List["ComponentVariantTypeDef"],
-        "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueTypeDef"],
         "createdAt": datetime,
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
+_OptionalThemeTypeDef = TypedDict(
+    "_OptionalThemeTypeDef",
     {
-        "sourceId": str,
-        "children": List["ComponentChildTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationTypeDef"],
         "modifiedAt": datetime,
+        "overrides": List["ThemeValuesOutputTypeDef"],
         "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
     },
     total=False,
 )
 
 
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
+class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
 
-ComponentVariantTypeDef = TypedDict(
-    "ComponentVariantTypeDef",
+DeleteComponentRequestRequestTypeDef = TypedDict(
+    "DeleteComponentRequestRequestTypeDef",
     {
-        "variantValues": Mapping[str, str],
-        "overrides": Mapping[str, Mapping[str, str]],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-_RequiredCreateComponentDataTypeDef = TypedDict(
-    "_RequiredCreateComponentDataTypeDef",
+DeleteFormRequestRequestTypeDef = TypedDict(
+    "DeleteFormRequestRequestTypeDef",
     {
-        "name": str,
-        "componentType": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
-        "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
-_OptionalCreateComponentDataTypeDef = TypedDict(
-    "_OptionalCreateComponentDataTypeDef",
+
+DeleteThemeRequestRequestTypeDef = TypedDict(
+    "DeleteThemeRequestRequestTypeDef",
     {
-        "sourceId": str,
-        "children": Sequence["ComponentChildTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "tags": Mapping[str, str],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+
+_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
+    {
+        "code": str,
+        "redirectUri": str,
+    },
+)
+_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
+    {
+        "clientId": str,
     },
     total=False,
 )
 
 
-class CreateComponentDataTypeDef(
-    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+class ExchangeCodeForTokenRequestBodyTypeDef(
+    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
 ):
     pass
 
 
-_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateComponentRequestRequestTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "componentToCreate": "CreateComponentDataTypeDef",
     },
 )
-_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateComponentRequestRequestTypeDef",
+_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateComponentRequestRequestTypeDef(
-    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+class ExportComponentsRequestRequestTypeDef(
+    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
 ):
     pass
 
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
-    {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
+_RequiredExportFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportFormsRequestRequestTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
+_OptionalExportFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportFormsRequestRequestTypeDef",
     {
-        "cta": "FormCTATypeDef",
-        "tags": Mapping[str, str],
-        "labelDecorator": LabelDecoratorType,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+class ExportFormsRequestRequestTypeDef(
+    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
+):
     pass
 
 
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
+_RequiredExportThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredExportThemesRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "formToCreate": "CreateFormDataTypeDef",
     },
 )
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
+_OptionalExportThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalExportThemesRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "nextToken": str,
     },
     total=False,
 )
 
 
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+class ExportThemesRequestRequestTypeDef(
+    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
 ):
     pass
 
 
-CreateFormResponseTypeDef = TypedDict(
-    "CreateFormResponseTypeDef",
+FieldPositionTypeDef = TypedDict(
+    "FieldPositionTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "fixed": Literal["first"],
+        "rightOf": str,
+        "below": str,
     },
+    total=False,
 )
 
-_RequiredCreateThemeDataTypeDef = TypedDict(
-    "_RequiredCreateThemeDataTypeDef",
+_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationOutputTypeDef",
     {
-        "name": str,
-        "values": Sequence["ThemeValuesTypeDef"],
+        "type": str,
     },
 )
-_OptionalCreateThemeDataTypeDef = TypedDict(
-    "_OptionalCreateThemeDataTypeDef",
+_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationOutputTypeDef",
     {
-        "overrides": Sequence["ThemeValuesTypeDef"],
-        "tags": Mapping[str, str],
+        "strValues": List[str],
+        "numValues": List[int],
+        "validationMessage": str,
     },
     total=False,
 )
 
 
-class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
+class FieldValidationConfigurationOutputTypeDef(
+    _RequiredFieldValidationConfigurationOutputTypeDef,
+    _OptionalFieldValidationConfigurationOutputTypeDef,
+):
     pass
 
 
-_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateThemeRequestRequestTypeDef",
+_RequiredFieldValidationConfigurationTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "themeToCreate": "CreateThemeDataTypeDef",
+        "type": str,
     },
 )
-_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateThemeRequestRequestTypeDef",
+_OptionalFieldValidationConfigurationTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationTypeDef",
     {
-        "clientToken": str,
+        "strValues": Sequence[str],
+        "numValues": Sequence[int],
+        "validationMessage": str,
     },
     total=False,
 )
 
 
-class CreateThemeRequestRequestTypeDef(
-    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
+class FieldValidationConfigurationTypeDef(
+    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
 
-CreateThemeResponseTypeDef = TypedDict(
-    "CreateThemeResponseTypeDef",
+_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigOutputTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": List[str],
     },
 )
-
-DeleteComponentRequestRequestTypeDef = TypedDict(
-    "DeleteComponentRequestRequestTypeDef",
+_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
+    total=False,
 )
 
-DeleteFormRequestRequestTypeDef = TypedDict(
-    "DeleteFormRequestRequestTypeDef",
+
+class FileUploaderFieldConfigOutputTypeDef(
+    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": Sequence[str],
     },
 )
-
-DeleteThemeRequestRequestTypeDef = TypedDict(
-    "DeleteThemeRequestRequestTypeDef",
+_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
+    total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+
+class FileUploaderFieldConfigTypeDef(
+    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
+):
+    pass
+
+
+FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "model": str,
     },
+    total=False,
 )
 
-_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
+_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "code": str,
-        "redirectUri": str,
+        "property": str,
     },
 )
-_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
+_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "clientId": str,
+        "field": str,
     },
     total=False,
 )
 
 
-class ExchangeCodeForTokenRequestBodyTypeDef(
-    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
+class FormInputValuePropertyBindingPropertiesTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
 ):
     pass
 
 
-ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
-    "ExchangeCodeForTokenRequestRequestTypeDef",
+FormStyleConfigTypeDef = TypedDict(
+    "FormStyleConfigTypeDef",
     {
-        "provider": Literal["figma"],
-        "request": "ExchangeCodeForTokenRequestBodyTypeDef",
+        "tokenReference": str,
+        "value": str,
     },
+    total=False,
 )
 
-ExchangeCodeForTokenResponseTypeDef = TypedDict(
-    "ExchangeCodeForTokenResponseTypeDef",
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
 
-_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
+GetComponentRequestRequestTypeDef = TypedDict(
+    "GetComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "id": str,
     },
 )
-_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
+
+GetFormRequestRequestTypeDef = TypedDict(
+    "GetFormRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
+GetMetadataRequestRequestTypeDef = TypedDict(
+    "GetMetadataRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
 
-class ExportComponentsRequestExportComponentsPaginateTypeDef(
-    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
-    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
-):
-    pass
-
+GetThemeRequestRequestTypeDef = TypedDict(
+    "GetThemeRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
 
-_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestRequestTypeDef",
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestRequestTypeDef",
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportComponentsRequestRequestTypeDef(
-    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
 ):
     pass
 
 
-ExportComponentsResponseTypeDef = TypedDict(
-    "ExportComponentsResponseTypeDef",
+_RequiredListComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListComponentsRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListComponentsRequestRequestTypeDef",
     {
-        "entities": List["ComponentTypeDef"],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "maxResults": int,
     },
+    total=False,
 )
 
-_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
+
+class ListComponentsRequestRequestTypeDef(
+    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
+_OptionalListFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFormsRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportFormsRequestExportFormsPaginateTypeDef(
-    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
-    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
+class ListFormsRequestRequestTypeDef(
+    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredExportFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportFormsRequestRequestTypeDef",
+_RequiredListThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredListThemesRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportFormsRequestRequestTypeDef",
+_OptionalListThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalListThemesRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class ExportFormsRequestRequestTypeDef(
-    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
+class ListThemesRequestRequestTypeDef(
+    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
 ):
     pass
 
 
-ExportFormsResponseTypeDef = TypedDict(
-    "ExportFormsResponseTypeDef",
+ThemeSummaryTypeDef = TypedDict(
+    "ThemeSummaryTypeDef",
     {
-        "entities": List["FormTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
     },
 )
 
-_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
+    total=False,
 )
-_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
+
+PredicateTypeDef = TypedDict(
+    "PredicateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "or": Sequence[Dict[str, Any]],
+        "and": Sequence[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
     total=False,
 )
 
+PutMetadataFlagBodyTypeDef = TypedDict(
+    "PutMetadataFlagBodyTypeDef",
+    {
+        "newValue": str,
+    },
+)
 
-class ExportThemesRequestExportThemesPaginateTypeDef(
-    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
-    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
-):
-    pass
-
-
-_RequiredExportThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredExportThemesRequestRequestTypeDef",
+_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredRefreshTokenRequestBodyTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "token": str,
     },
 )
-_OptionalExportThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalExportThemesRequestRequestTypeDef",
+_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalRefreshTokenRequestBodyTypeDef",
     {
-        "nextToken": str,
+        "clientId": str,
     },
     total=False,
 )
 
 
-class ExportThemesRequestRequestTypeDef(
-    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
+class RefreshTokenRequestBodyTypeDef(
+    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
 ):
     pass
 
 
-ExportThemesResponseTypeDef = TypedDict(
-    "ExportThemesResponseTypeDef",
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
     {
-        "entities": List["ThemeTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "value": str,
+        "children": List[Dict[str, Any]],
     },
+    total=False,
 )
 
-FieldConfigTypeDef = TypedDict(
-    "FieldConfigTypeDef",
+ThemeValueTypeDef = TypedDict(
+    "ThemeValueTypeDef",
     {
-        "label": str,
-        "position": "FieldPositionTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigTypeDef",
-        "validations": Sequence["FieldValidationConfigurationTypeDef"],
+        "value": str,
+        "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-_RequiredFieldInputConfigTypeDef = TypedDict(
-    "_RequiredFieldInputConfigTypeDef",
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
     {
-        "type": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
+    total=False,
 )
-_OptionalFieldInputConfigTypeDef = TypedDict(
-    "_OptionalFieldInputConfigTypeDef",
+
+ThemeValuesTypeDef = TypedDict(
+    "ThemeValuesTypeDef",
     {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsTypeDef",
+        "key": str,
+        "value": Dict[str, Any],
+    },
+    total=False,
+)
+
+_RequiredUpdateThemeDataTypeDef = TypedDict(
+    "_RequiredUpdateThemeDataTypeDef",
+    {
+        "values": Sequence["ThemeValuesTypeDef"],
+    },
+)
+_OptionalUpdateThemeDataTypeDef = TypedDict(
+    "_OptionalUpdateThemeDataTypeDef",
+    {
+        "id": str,
         "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigTypeDef",
+        "overrides": Sequence["ThemeValuesTypeDef"],
     },
     total=False,
 )
 
 
-class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
     pass
 
 
-FieldPositionTypeDef = TypedDict(
-    "FieldPositionTypeDef",
+_RequiredValueMappingTypeDef = TypedDict(
+    "_RequiredValueMappingTypeDef",
     {
-        "fixed": Literal["first"],
-        "rightOf": str,
-        "below": str,
+        "value": "FormInputValuePropertyTypeDef",
+    },
+)
+_OptionalValueMappingTypeDef = TypedDict(
+    "_OptionalValueMappingTypeDef",
+    {
+        "displayValue": "FormInputValuePropertyTypeDef",
     },
     total=False,
 )
 
-_RequiredFieldValidationConfigurationTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationTypeDef",
+
+class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
+    pass
+
+
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
     {
-        "type": str,
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
+    total=False,
 )
-_OptionalFieldValidationConfigurationTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationTypeDef",
+
+ActionParametersTypeDef = TypedDict(
+    "ActionParametersTypeDef",
     {
-        "strValues": Sequence[str],
-        "numValues": Sequence[int],
-        "validationMessage": str,
+        "type": "ComponentPropertyTypeDef",
+        "url": "ComponentPropertyTypeDef",
+        "anchor": "ComponentPropertyTypeDef",
+        "target": "ComponentPropertyTypeDef",
+        "global": "ComponentPropertyTypeDef",
+        "model": str,
+        "id": "ComponentPropertyTypeDef",
+        "fields": Mapping[str, "ComponentPropertyTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
+    },
+    total=False,
+)
+
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
+    {
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
+    },
+)
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
+    {
+        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
     },
     total=False,
 )
 
 
-class FieldValidationConfigurationTypeDef(
-    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
 ):
     pass
 
 
-_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigTypeDef",
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
     {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": Sequence[str],
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
 )
-_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigTypeDef",
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
     {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
+        "relationship": CodegenGenericDataRelationshipTypeTypeDef,
     },
     total=False,
 )
 
 
-class FileUploaderFieldConfigTypeDef(
-    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
 
-FormBindingElementTypeDef = TypedDict(
-    "FormBindingElementTypeDef",
-    {
-        "element": str,
-        "property": str,
-    },
-)
-
-FormButtonTypeDef = TypedDict(
-    "FormButtonTypeDef",
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
     {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionTypeDef",
+        "react": ReactStartCodegenJobDataTypeDef,
     },
     total=False,
 )
 
-FormCTATypeDef = TypedDict(
-    "FormCTATypeDef",
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonTypeDef",
-        "cancel": "FormButtonTypeDef",
-        "submit": "FormButtonTypeDef",
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
+        "defaultValue": str,
     },
     total=False,
 )
 
-FormDataTypeConfigTypeDef = TypedDict(
-    "FormDataTypeConfigTypeDef",
+ComponentBindingPropertiesValueTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueTypeDef",
     {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
+        "defaultValue": str,
     },
+    total=False,
 )
 
-FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesTypeDef",
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
     {
         "model": str,
     },
-    total=False,
 )
-
-FormInputBindingPropertiesValueTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueTypeDef",
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
     {
-        "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
+        "sort": List[SortPropertyTypeDef],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
     },
     total=False,
 )
 
-_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
+
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
+):
+    pass
+
+
+_RequiredComponentDataConfigurationTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationTypeDef",
     {
-        "property": str,
+        "model": str,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
+_OptionalComponentDataConfigurationTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationTypeDef",
     {
-        "field": str,
+        "sort": Sequence[SortPropertyTypeDef],
+        "predicate": "PredicateTypeDef",
+        "identifiers": Sequence[str],
     },
     total=False,
 )
 
 
-class FormInputValuePropertyBindingPropertiesTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
+class ComponentDataConfigurationTypeDef(
+    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
 
-FormInputValuePropertyTypeDef = TypedDict(
-    "FormInputValuePropertyTypeDef",
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
     {
         "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
-        "concat": Sequence[Dict[str, Any]],
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": List[Dict[str, Any]],
+        "condition": "ComponentConditionPropertyTypeDef",
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
     total=False,
 )
 
-FormStyleConfigTypeDef = TypedDict(
-    "FormStyleConfigTypeDef",
+ComponentPropertyTypeDef = TypedDict(
+    "ComponentPropertyTypeDef",
     {
-        "tokenReference": str,
         "value": str,
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Mapping[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": Sequence[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
     total=False,
 )
 
-FormStyleTypeDef = TypedDict(
-    "FormStyleTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "horizontalGap": "FormStyleConfigTypeDef",
-        "verticalGap": "FormStyleConfigTypeDef",
-        "outerPadding": "FormStyleConfigTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-FormSummaryTypeDef = TypedDict(
-    "FormSummaryTypeDef",
+ExchangeCodeForTokenResponseTypeDef = TypedDict(
+    "ExchangeCodeForTokenResponseTypeDef",
     {
-        "appId": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "environmentName": str,
-        "formActionType": FormActionTypeType,
-        "id": str,
-        "name": str,
+        "accessToken": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+GetMetadataResponseTypeDef = TypedDict(
+    "GetMetadataResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "formActionType": FormActionTypeType,
-        "style": "FormStyleTypeDef",
-        "dataType": "FormDataTypeConfigTypeDef",
-        "fields": Dict[str, "FieldConfigTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
+        "features": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
     {
-        "tags": Dict[str, str],
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "entities": List[CodegenJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
-    pass
-
-
-GetCodegenJobRequestRequestTypeDef = TypedDict(
-    "GetCodegenJobRequestRequestTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "entities": List[ComponentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetCodegenJobResponseTypeDef = TypedDict(
-    "GetCodegenJobResponseTypeDef",
+RefreshTokenResponseTypeDef = TypedDict(
+    "RefreshTokenResponseTypeDef",
     {
-        "job": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessToken": str,
+        "expiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetComponentRequestRequestTypeDef = TypedDict(
-    "GetComponentRequestRequestTypeDef",
+FormSummaryTypeDef = TypedDict(
+    "FormSummaryTypeDef",
     {
         "appId": str,
+        "dataType": FormDataTypeConfigTypeDef,
         "environmentName": str,
+        "formActionType": FormActionTypeType,
         "id": str,
+        "name": str,
     },
 )
 
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
+_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateThemeRequestRequestTypeDef",
     {
-        "component": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "themeToCreate": CreateThemeDataTypeDef,
     },
 )
-
-GetFormRequestRequestTypeDef = TypedDict(
-    "GetFormRequestRequestTypeDef",
+_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateThemeRequestRequestTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "clientToken": str,
     },
+    total=False,
 )
 
-GetFormResponseTypeDef = TypedDict(
-    "GetFormResponseTypeDef",
+
+class CreateThemeRequestRequestTypeDef(
+    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
+):
+    pass
+
+
+CreateThemeResponseTypeDef = TypedDict(
+    "CreateThemeResponseTypeDef",
     {
-        "form": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMetadataRequestRequestTypeDef = TypedDict(
-    "GetMetadataRequestRequestTypeDef",
+ExportThemesResponseTypeDef = TypedDict(
+    "ExportThemesResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "entities": List[ThemeTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMetadataResponseTypeDef = TypedDict(
-    "GetMetadataResponseTypeDef",
+GetThemeResponseTypeDef = TypedDict(
+    "GetThemeResponseTypeDef",
     {
-        "features": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "theme": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetThemeRequestRequestTypeDef = TypedDict(
-    "GetThemeRequestRequestTypeDef",
+UpdateThemeResponseTypeDef = TypedDict(
+    "UpdateThemeResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetThemeResponseTypeDef = TypedDict(
-    "GetThemeResponseTypeDef",
+ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
+    "ExchangeCodeForTokenRequestRequestTypeDef",
     {
-        "theme": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "provider": Literal["figma"],
+        "request": ExchangeCodeForTokenRequestBodyTypeDef,
     },
 )
 
-_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
-    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
-    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+class ExportComponentsRequestExportComponentsPaginateTypeDef(
+    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
+    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestRequestTypeDef",
+_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestRequestTypeDef",
+_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListCodegenJobsRequestRequestTypeDef(
-    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
+class ExportFormsRequestExportFormsPaginateTypeDef(
+    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
+    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
 ):
     pass
 
 
-ListCodegenJobsResponseTypeDef = TypedDict(
-    "ListCodegenJobsResponseTypeDef",
-    {
-        "entities": List["CodegenJobSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
+_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
+_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListComponentsRequestListComponentsPaginateTypeDef(
-    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
-    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
+class ExportThemesRequestExportThemesPaginateTypeDef(
+    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
+    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListComponentsRequestRequestTypeDef",
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListComponentsRequestRequestTypeDef",
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListComponentsRequestRequestTypeDef(
-    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
 ):
     pass
 
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
-    {
-        "entities": List["ComponentSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_RequiredListFormsRequestListFormsPaginateTypeDef",
+_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_OptionalListFormsRequestListFormsPaginateTypeDef",
+_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListFormsRequestListFormsPaginateTypeDef(
-    _RequiredListFormsRequestListFormsPaginateTypeDef,
-    _OptionalListFormsRequestListFormsPaginateTypeDef,
+class ListComponentsRequestListComponentsPaginateTypeDef(
+    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
+    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFormsRequestRequestTypeDef",
+_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_RequiredListFormsRequestListFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFormsRequestRequestTypeDef",
+_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_OptionalListFormsRequestListFormsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class ListFormsRequestRequestTypeDef(
-    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
+class ListFormsRequestListFormsPaginateTypeDef(
+    _RequiredListFormsRequestListFormsPaginateTypeDef,
+    _OptionalListFormsRequestListFormsPaginateTypeDef,
 ):
     pass
 
 
-ListFormsResponseTypeDef = TypedDict(
-    "ListFormsResponseTypeDef",
-    {
-        "entities": List["FormSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
     "_RequiredListThemesRequestListThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
     "_OptionalListThemesRequestListThemesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListThemesRequestListThemesPaginateTypeDef(
     _RequiredListThemesRequestListThemesPaginateTypeDef,
     _OptionalListThemesRequestListThemesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredListThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredListThemesRequestRequestTypeDef",
+FormButtonTypeDef = TypedDict(
+    "FormButtonTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "excluded": bool,
+        "children": str,
+        "position": FieldPositionTypeDef,
     },
+    total=False,
 )
-_OptionalListThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalListThemesRequestRequestTypeDef",
+
+_RequiredSectionalElementTypeDef = TypedDict(
+    "_RequiredSectionalElementTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "type": str,
+    },
+)
+_OptionalSectionalElementTypeDef = TypedDict(
+    "_OptionalSectionalElementTypeDef",
+    {
+        "position": FieldPositionTypeDef,
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
     },
     total=False,
 )
 
 
-class ListThemesRequestRequestTypeDef(
-    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
-):
+class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
     pass
 
 
-ListThemesResponseTypeDef = TypedDict(
-    "ListThemesResponseTypeDef",
-    {
-        "entities": List["ThemeSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-MutationActionSetStateParameterTypeDef = TypedDict(
-    "MutationActionSetStateParameterTypeDef",
+FormInputBindingPropertiesValueTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyTypeDef",
+        "type": str,
+        "bindingProperties": FormInputBindingPropertiesValuePropertiesTypeDef,
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FormInputValuePropertyTypeDef = TypedDict(
+    "FormInputValuePropertyTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "value": str,
+        "bindingProperties": FormInputValuePropertyBindingPropertiesTypeDef,
+        "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-PredicateTypeDef = TypedDict(
-    "PredicateTypeDef",
+FormStyleTypeDef = TypedDict(
+    "FormStyleTypeDef",
     {
-        "or": Sequence[Dict[str, Any]],
-        "and": Sequence[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "horizontalGap": FormStyleConfigTypeDef,
+        "verticalGap": FormStyleConfigTypeDef,
+        "outerPadding": FormStyleConfigTypeDef,
     },
     total=False,
 )
 
-PutMetadataFlagBodyTypeDef = TypedDict(
-    "PutMetadataFlagBodyTypeDef",
+ListThemesResponseTypeDef = TypedDict(
+    "ListThemesResponseTypeDef",
     {
-        "newValue": str,
+        "entities": List[ThemeSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetadataFlagRequestRequestTypeDef = TypedDict(
     "PutMetadataFlagRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "featureName": str,
-        "body": "PutMetadataFlagBodyTypeDef",
+        "body": PutMetadataFlagBodyTypeDef,
     },
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
+RefreshTokenRequestRequestTypeDef = TypedDict(
+    "RefreshTokenRequestRequestTypeDef",
     {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
+        "provider": Literal["figma"],
+        "refreshTokenBody": RefreshTokenRequestBodyTypeDef,
     },
-    total=False,
 )
 
-_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredRefreshTokenRequestBodyTypeDef",
+_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemeRequestRequestTypeDef",
     {
-        "token": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedTheme": UpdateThemeDataTypeDef,
     },
 )
-_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalRefreshTokenRequestBodyTypeDef",
+_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemeRequestRequestTypeDef",
     {
-        "clientId": str,
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class RefreshTokenRequestBodyTypeDef(
-    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
+class UpdateThemeRequestRequestTypeDef(
+    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
 
-RefreshTokenRequestRequestTypeDef = TypedDict(
-    "RefreshTokenRequestRequestTypeDef",
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
     {
-        "provider": Literal["figma"],
-        "refreshTokenBody": "RefreshTokenRequestBodyTypeDef",
+        "action": str,
+        "parameters": ActionParametersOutputTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-RefreshTokenResponseTypeDef = TypedDict(
-    "RefreshTokenResponseTypeDef",
+ComponentEventTypeDef = TypedDict(
+    "ComponentEventTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "action": str,
+        "parameters": ActionParametersTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
+        "primaryKeys": List[str],
+    },
+)
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
+    {
+        "isJoinTable": bool,
     },
+    total=False,
 )
 
-_RequiredSectionalElementTypeDef = TypedDict(
-    "_RequiredSectionalElementTypeDef",
+
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
+):
+    pass
+
+
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
     {
-        "type": str,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
     },
 )
-_OptionalSectionalElementTypeDef = TypedDict(
-    "_OptionalSectionalElementTypeDef",
+
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "position": "FieldPositionTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": Sequence[str],
+    },
+)
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
+    {
+        "isJoinTable": bool,
     },
     total=False,
 )
 
 
-class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+):
     pass
 
 
-SortPropertyTypeDef = TypedDict(
-    "SortPropertyTypeDef",
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
-_RequiredStartCodegenJobDataTypeDef = TypedDict(
-    "_RequiredStartCodegenJobDataTypeDef",
+ListFormsResponseTypeDef = TypedDict(
+    "ListFormsResponseTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "entities": List[FormSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartCodegenJobDataTypeDef = TypedDict(
-    "_OptionalStartCodegenJobDataTypeDef",
+
+FormCTATypeDef = TypedDict(
+    "FormCTATypeDef",
     {
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "tags": Mapping[str, str],
+        "position": FormButtonsPositionType,
+        "clear": FormButtonTypeDef,
+        "cancel": FormButtonTypeDef,
+        "submit": FormButtonTypeDef,
     },
     total=False,
 )
 
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
+    {
+        "values": List[ValueMappingTypeDef],
+    },
+)
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
+    {
+        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
+    },
+    total=False,
+)
 
-class StartCodegenJobDataTypeDef(
-    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
+
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
 ):
     pass
 
 
-_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCodegenJobRequestRequestTypeDef",
+_RequiredValueMappingsTypeDef = TypedDict(
+    "_RequiredValueMappingsTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+        "values": Sequence[ValueMappingTypeDef],
     },
 )
-_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCodegenJobRequestRequestTypeDef",
+_OptionalValueMappingsTypeDef = TypedDict(
+    "_OptionalValueMappingsTypeDef",
     {
-        "clientToken": str,
+        "bindingProperties": Mapping[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
 
-class StartCodegenJobRequestRequestTypeDef(
-    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
-):
+class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
     pass
 
 
-StartCodegenJobResponseTypeDef = TypedDict(
-    "StartCodegenJobResponseTypeDef",
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
     {
-        "entity": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "componentType": str,
+        "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
     },
 )
-
-ThemeSummaryTypeDef = TypedDict(
-    "ThemeSummaryTypeDef",
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "sourceId": str,
     },
+    total=False,
 )
 
-_RequiredThemeTypeDef = TypedDict(
-    "_RequiredThemeTypeDef",
+
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
+
+_RequiredComponentTypeDef = TypedDict(
+    "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
+        "componentType": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List[ComponentVariantOutputTypeDef],
+        "overrides": Dict[str, Dict[str, str]],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
         "createdAt": datetime,
-        "values": List["ThemeValuesTypeDef"],
     },
 )
-_OptionalThemeTypeDef = TypedDict(
-    "_OptionalThemeTypeDef",
+_OptionalComponentTypeDef = TypedDict(
+    "_OptionalComponentTypeDef",
     {
+        "sourceId": str,
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesTypeDef"],
         "tags": Dict[str, str],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
 
-class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
+class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
 
-ThemeValueTypeDef = TypedDict(
-    "ThemeValueTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
+    {
+        "componentType": str,
+        "name": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+    },
+)
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "value": str,
         "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "sourceId": str,
     },
     total=False,
 )
 
-ThemeValuesTypeDef = TypedDict(
-    "ThemeValuesTypeDef",
+
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
+    pass
+
+
+_RequiredCreateComponentDataTypeDef = TypedDict(
+    "_RequiredCreateComponentDataTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "name": str,
+        "componentType": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
+        "overrides": Mapping[str, Mapping[str, str]],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+    },
+)
+_OptionalCreateComponentDataTypeDef = TypedDict(
+    "_OptionalCreateComponentDataTypeDef",
+    {
+        "sourceId": str,
+        "children": Sequence["ComponentChildTypeDef"],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "tags": Mapping[str, str],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
+
+class CreateComponentDataTypeDef(
+    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+):
+    pass
+
+
 UpdateComponentDataTypeDef = TypedDict(
     "UpdateComponentDataTypeDef",
     {
         "id": str,
         "name": str,
         "sourceId": str,
         "componentType": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
         "children": Sequence["ComponentChildTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
         "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "events": Mapping[str, "ComponentEventTypeDef"],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
+    },
+)
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Mapping[str, CodegenGenericDataModelTypeDef],
+        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
+    },
+)
+
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsOutputTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
+    pass
+
+
+_RequiredFieldInputConfigTypeDef = TypedDict(
+    "_RequiredFieldInputConfigTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigTypeDef = TypedDict(
+    "_OptionalFieldInputConfigTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+    pass
+
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportComponentsResponseTypeDef = TypedDict(
+    "ExportComponentsResponseTypeDef",
+    {
+        "entities": List[ComponentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "component": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentResponseTypeDef = TypedDict(
+    "UpdateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateComponentRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "componentToCreate": CreateComponentDataTypeDef,
+    },
+)
+_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateComponentRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateComponentRequestRequestTypeDef(
+    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredUpdateComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedComponent": "UpdateComponentDataTypeDef",
+        "updatedComponent": UpdateComponentDataTypeDef,
     },
 )
 _OptionalUpdateComponentRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1799,152 +2077,275 @@
 
 class UpdateComponentRequestRequestTypeDef(
     _RequiredUpdateComponentRequestRequestTypeDef, _OptionalUpdateComponentRequestRequestTypeDef
 ):
     pass
 
 
-UpdateComponentResponseTypeDef = TypedDict(
-    "UpdateComponentResponseTypeDef",
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
     {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-
-UpdateFormDataTypeDef = TypedDict(
-    "UpdateFormDataTypeDef",
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": CodegenJobAssetTypeDef,
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFormRequestRequestTypeDef",
+
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
+
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "updatedForm": "UpdateFormDataTypeDef",
+        "renderConfig": CodegenJobRenderConfigTypeDef,
     },
 )
-_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFormRequestRequestTypeDef",
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
     {
-        "clientToken": str,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class UpdateFormRequestRequestTypeDef(
-    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
 
-UpdateFormResponseTypeDef = TypedDict(
-    "UpdateFormResponseTypeDef",
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigOutputTypeDef,
+        "validations": List[FieldValidationConfigurationOutputTypeDef],
     },
+    total=False,
 )
 
-_RequiredUpdateThemeDataTypeDef = TypedDict(
-    "_RequiredUpdateThemeDataTypeDef",
+FieldConfigTypeDef = TypedDict(
+    "FieldConfigTypeDef",
     {
-        "values": Sequence["ThemeValuesTypeDef"],
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigTypeDef,
+        "validations": Sequence[FieldValidationConfigurationTypeDef],
     },
+    total=False,
 )
-_OptionalUpdateThemeDataTypeDef = TypedDict(
-    "_OptionalUpdateThemeDataTypeDef",
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
     {
-        "id": str,
-        "name": str,
-        "overrides": Sequence["ThemeValuesTypeDef"],
+        "job": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "codegenJobToCreate": StartCodegenJobDataTypeDef,
+    },
+)
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
+):
     pass
 
 
-_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemeRequestRequestTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedTheme": "UpdateThemeDataTypeDef",
+        "name": str,
+        "formActionType": FormActionTypeType,
+        "style": FormStyleTypeDef,
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigOutputTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "schemaVersion": str,
     },
 )
-_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemeRequestRequestTypeDef",
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
     {
-        "clientToken": str,
+        "tags": Dict[str, str],
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 
-class UpdateThemeRequestRequestTypeDef(
-    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
-):
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
 
-UpdateThemeResponseTypeDef = TypedDict(
-    "UpdateThemeResponseTypeDef",
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+    },
+)
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
+    {
+        "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
 
-_RequiredValueMappingTypeDef = TypedDict(
-    "_RequiredValueMappingTypeDef",
+
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+    pass
+
+
+UpdateFormDataTypeDef = TypedDict(
+    "UpdateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
-_OptionalValueMappingTypeDef = TypedDict(
-    "_OptionalValueMappingTypeDef",
+
+CreateFormResponseTypeDef = TypedDict(
+    "CreateFormResponseTypeDef",
     {
-        "displayValue": "FormInputValuePropertyTypeDef",
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportFormsResponseTypeDef = TypedDict(
+    "ExportFormsResponseTypeDef",
+    {
+        "entities": List[FormTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFormResponseTypeDef = TypedDict(
+    "GetFormResponseTypeDef",
+    {
+        "form": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFormResponseTypeDef = TypedDict(
+    "UpdateFormResponseTypeDef",
+    {
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
+    },
+)
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+):
     pass
 
 
-_RequiredValueMappingsTypeDef = TypedDict(
-    "_RequiredValueMappingsTypeDef",
+_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFormRequestRequestTypeDef",
     {
-        "values": Sequence["ValueMappingTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedForm": UpdateFormDataTypeDef,
     },
 )
-_OptionalValueMappingsTypeDef = TypedDict(
-    "_OptionalValueMappingsTypeDef",
+_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Mapping[str, "FormInputBindingPropertiesValueTypeDef"],
+        "clientToken": str,
     },
     total=False,
 )
 
 
-class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
+class UpdateFormRequestRequestTypeDef(
+    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+):
     pass
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder/type_defs.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplifyuibuilder service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplifyuibuilder.type_defs import ActionParametersTypeDef
+    from types_aiobotocore_amplifyuibuilder.type_defs import MutationActionSetStateParameterTypeDef
 
-    data: ActionParametersTypeDef = {...}
+    data: MutationActionSetStateParameterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,231 +36,230 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ActionParametersTypeDef",
+    "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
+    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataFieldTypeDef",
-    "CodegenGenericDataModelTypeDef",
-    "CodegenGenericDataNonModelTypeDef",
+    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "CodegenJobGenericDataSchemaTypeDef",
-    "CodegenJobRenderConfigTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "CodegenJobTypeDef",
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
-    "ComponentBindingPropertiesValueTypeDef",
-    "ComponentChildTypeDef",
     "ComponentConditionPropertyTypeDef",
-    "ComponentDataConfigurationTypeDef",
-    "ComponentEventTypeDef",
+    "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
-    "ComponentPropertyTypeDef",
+    "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentTypeDef",
+    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
-    "CreateComponentDataTypeDef",
-    "CreateComponentRequestRequestTypeDef",
-    "CreateComponentResponseTypeDef",
-    "CreateFormDataTypeDef",
-    "CreateFormRequestRequestTypeDef",
-    "CreateFormResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
-    "CreateThemeRequestRequestTypeDef",
-    "CreateThemeResponseTypeDef",
+    "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
-    "ExchangeCodeForTokenRequestRequestTypeDef",
-    "ExchangeCodeForTokenResponseTypeDef",
-    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
-    "ExportComponentsResponseTypeDef",
-    "ExportFormsRequestExportFormsPaginateTypeDef",
     "ExportFormsRequestRequestTypeDef",
-    "ExportFormsResponseTypeDef",
-    "ExportThemesRequestExportThemesPaginateTypeDef",
     "ExportThemesRequestRequestTypeDef",
-    "ExportThemesResponseTypeDef",
-    "FieldConfigTypeDef",
-    "FieldInputConfigTypeDef",
     "FieldPositionTypeDef",
+    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
+    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
-    "FormBindingElementTypeDef",
-    "FormButtonTypeDef",
-    "FormCTATypeDef",
-    "FormDataTypeConfigTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
-    "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
-    "FormInputValuePropertyTypeDef",
     "FormStyleConfigTypeDef",
-    "FormStyleTypeDef",
-    "FormSummaryTypeDef",
-    "FormTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
-    "GetCodegenJobResponseTypeDef",
     "GetComponentRequestRequestTypeDef",
-    "GetComponentResponseTypeDef",
     "GetFormRequestRequestTypeDef",
-    "GetFormResponseTypeDef",
     "GetMetadataRequestRequestTypeDef",
-    "GetMetadataResponseTypeDef",
     "GetThemeRequestRequestTypeDef",
-    "GetThemeResponseTypeDef",
-    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
-    "ListCodegenJobsResponseTypeDef",
-    "ListComponentsRequestListComponentsPaginateTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListComponentsResponseTypeDef",
-    "ListFormsRequestListFormsPaginateTypeDef",
     "ListFormsRequestRequestTypeDef",
-    "ListFormsResponseTypeDef",
-    "ListThemesRequestListThemesPaginateTypeDef",
     "ListThemesRequestRequestTypeDef",
-    "ListThemesResponseTypeDef",
-    "MutationActionSetStateParameterTypeDef",
-    "PaginatorConfigTypeDef",
+    "ThemeSummaryTypeDef",
+    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
-    "PutMetadataFlagRequestRequestTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "RefreshTokenRequestRequestTypeDef",
-    "RefreshTokenResponseTypeDef",
-    "ResponseMetadataTypeDef",
-    "SectionalElementTypeDef",
-    "SortPropertyTypeDef",
-    "StartCodegenJobDataTypeDef",
-    "StartCodegenJobRequestRequestTypeDef",
-    "StartCodegenJobResponseTypeDef",
-    "ThemeSummaryTypeDef",
-    "ThemeTypeDef",
+    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
+    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
+    "UpdateThemeDataTypeDef",
+    "ValueMappingTypeDef",
+    "ActionParametersOutputTypeDef",
+    "ActionParametersTypeDef",
+    "CodegenGenericDataFieldOutputTypeDef",
+    "CodegenGenericDataFieldTypeDef",
+    "CodegenJobRenderConfigTypeDef",
+    "ComponentBindingPropertiesValueOutputTypeDef",
+    "ComponentBindingPropertiesValueTypeDef",
+    "ComponentDataConfigurationOutputTypeDef",
+    "ComponentDataConfigurationTypeDef",
+    "ComponentPropertyOutputTypeDef",
+    "ComponentPropertyTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExchangeCodeForTokenResponseTypeDef",
+    "GetMetadataResponseTypeDef",
+    "ListCodegenJobsResponseTypeDef",
+    "ListComponentsResponseTypeDef",
+    "RefreshTokenResponseTypeDef",
+    "FormSummaryTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "CreateThemeResponseTypeDef",
+    "ExportThemesResponseTypeDef",
+    "GetThemeResponseTypeDef",
+    "UpdateThemeResponseTypeDef",
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    "ExportComponentsRequestExportComponentsPaginateTypeDef",
+    "ExportFormsRequestExportFormsPaginateTypeDef",
+    "ExportThemesRequestExportThemesPaginateTypeDef",
+    "ListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+    "ListComponentsRequestListComponentsPaginateTypeDef",
+    "ListFormsRequestListFormsPaginateTypeDef",
+    "ListThemesRequestListThemesPaginateTypeDef",
+    "FormButtonTypeDef",
+    "SectionalElementTypeDef",
+    "FormInputBindingPropertiesValueTypeDef",
+    "FormInputValuePropertyTypeDef",
+    "FormStyleTypeDef",
+    "ListThemesResponseTypeDef",
+    "PutMetadataFlagRequestRequestTypeDef",
+    "RefreshTokenRequestRequestTypeDef",
+    "UpdateThemeRequestRequestTypeDef",
+    "ComponentEventOutputTypeDef",
+    "ComponentEventTypeDef",
+    "CodegenGenericDataModelOutputTypeDef",
+    "CodegenGenericDataNonModelOutputTypeDef",
+    "CodegenGenericDataModelTypeDef",
+    "CodegenGenericDataNonModelTypeDef",
+    "ListFormsResponseTypeDef",
+    "FormCTATypeDef",
+    "ValueMappingsOutputTypeDef",
+    "ValueMappingsTypeDef",
+    "ComponentChildOutputTypeDef",
+    "ComponentTypeDef",
+    "ComponentChildTypeDef",
+    "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
-    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    "CodegenJobGenericDataSchemaTypeDef",
+    "FieldInputConfigOutputTypeDef",
+    "FieldInputConfigTypeDef",
+    "CreateComponentResponseTypeDef",
+    "ExportComponentsResponseTypeDef",
+    "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
+    "CreateComponentRequestRequestTypeDef",
+    "UpdateComponentRequestRequestTypeDef",
+    "CodegenJobTypeDef",
+    "StartCodegenJobDataTypeDef",
+    "FieldConfigOutputTypeDef",
+    "FieldConfigTypeDef",
+    "GetCodegenJobResponseTypeDef",
+    "StartCodegenJobResponseTypeDef",
+    "StartCodegenJobRequestRequestTypeDef",
+    "FormTypeDef",
+    "CreateFormDataTypeDef",
     "UpdateFormDataTypeDef",
-    "UpdateFormRequestRequestTypeDef",
+    "CreateFormResponseTypeDef",
+    "ExportFormsResponseTypeDef",
+    "GetFormResponseTypeDef",
     "UpdateFormResponseTypeDef",
-    "UpdateThemeDataTypeDef",
-    "UpdateThemeRequestRequestTypeDef",
-    "UpdateThemeResponseTypeDef",
-    "ValueMappingTypeDef",
-    "ValueMappingsTypeDef",
+    "CreateFormRequestRequestTypeDef",
+    "UpdateFormRequestRequestTypeDef",
 )
 
-ActionParametersTypeDef = TypedDict(
-    "ActionParametersTypeDef",
+MutationActionSetStateParameterTypeDef = TypedDict(
+    "MutationActionSetStateParameterTypeDef",
     {
-        "type": "ComponentPropertyTypeDef",
-        "url": "ComponentPropertyTypeDef",
-        "anchor": "ComponentPropertyTypeDef",
-        "target": "ComponentPropertyTypeDef",
-        "global": "ComponentPropertyTypeDef",
-        "model": str,
-        "id": "ComponentPropertyTypeDef",
-        "fields": Mapping[str, "ComponentPropertyTypeDef"],
-        "state": "MutationActionSetStateParameterTypeDef",
+        "componentName": str,
+        "property": str,
+        "set": "ComponentPropertyTypeDef",
     },
-    total=False,
 )
 
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
-CodegenGenericDataEnumTypeDef = TypedDict(
-    "CodegenGenericDataEnumTypeDef",
+CodegenGenericDataEnumOutputTypeDef = TypedDict(
+    "CodegenGenericDataEnumOutputTypeDef",
     {
         "values": List[str],
     },
 )
 
-_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldTypeDef",
+CodegenGenericDataEnumTypeDef = TypedDict(
+    "CodegenGenericDataEnumTypeDef",
     {
-        "relationship": "CodegenGenericDataRelationshipTypeTypeDef",
+        "values": Sequence[str],
     },
-    total=False,
 )
 
-class CodegenGenericDataFieldTypeDef(
-    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
-):
-    pass
-
-_RequiredCodegenGenericDataModelTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelTypeDef",
+_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-        "primaryKeys": List[str],
+        "type": GenericDataRelationshipTypeType,
+        "relatedModelName": str,
     },
 )
-_OptionalCodegenGenericDataModelTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelTypeDef",
+_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
     {
-        "isJoinTable": bool,
+        "relatedModelFields": List[str],
+        "canUnlinkAssociatedModel": bool,
+        "relatedJoinFieldName": str,
+        "relatedJoinTableName": str,
+        "belongsToFieldOnRelatedModel": str,
+        "associatedFields": List[str],
+        "isHasManyIndex": bool,
     },
     total=False,
 )
 
-class CodegenGenericDataModelTypeDef(
-    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+class CodegenGenericDataRelationshipTypeOutputTypeDef(
+    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
+    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
 ):
     pass
 
-CodegenGenericDataNonModelTypeDef = TypedDict(
-    "CodegenGenericDataNonModelTypeDef",
-    {
-        "fields": Dict[str, "CodegenGenericDataFieldTypeDef"],
-    },
-)
-
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": List[str],
+        "relatedModelFields": Sequence[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
+        "associatedFields": Sequence[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 class CodegenGenericDataRelationshipTypeTypeDef(
     _RequiredCodegenGenericDataRelationshipTypeTypeDef,
@@ -272,28 +271,22 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, "CodegenGenericDataModelTypeDef"],
-        "enums": Dict[str, "CodegenGenericDataEnumTypeDef"],
-        "nonModels": Dict[str, "CodegenGenericDataNonModelTypeDef"],
-    },
-)
-
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
     {
-        "react": "ReactStartCodegenJobDataTypeDef",
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
     },
     total=False,
 )
 
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
@@ -312,42 +305,29 @@
 )
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
-_RequiredCodegenJobTypeDef = TypedDict(
-    "_RequiredCodegenJobTypeDef",
-    {
-        "id": str,
-        "appId": str,
-        "environmentName": str,
-    },
-)
-_OptionalCodegenJobTypeDef = TypedDict(
-    "_OptionalCodegenJobTypeDef",
+ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "status": CodegenJobStatusType,
-        "statusMessage": str,
-        "asset": "CodegenJobAssetTypeDef",
-        "tags": Dict[str, str],
-        "createdAt": datetime,
-        "modifiedAt": datetime,
+        "model": str,
+        "field": str,
+        "predicates": List["PredicateOutputTypeDef"],
+        "userAttribute": str,
+        "bucket": str,
+        "key": str,
+        "defaultValue": str,
+        "slotName": str,
     },
     total=False,
 )
 
-class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
-    pass
-
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -355,88 +335,34 @@
         "key": str,
         "defaultValue": str,
         "slotName": str,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueTypeDef",
-    {
-        "type": str,
-        "bindingProperties": "ComponentBindingPropertiesValuePropertiesTypeDef",
-        "defaultValue": str,
-    },
-    total=False,
-)
-
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-    },
-)
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
-    {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
-    pass
-
 ComponentConditionPropertyTypeDef = TypedDict(
     "ComponentConditionPropertyTypeDef",
     {
         "property": str,
         "field": str,
         "operator": str,
         "operand": str,
         "then": Dict[str, Any],
         "else": Dict[str, Any],
         "operandType": str,
     },
     total=False,
 )
 
-_RequiredComponentDataConfigurationTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationTypeDef",
-    {
-        "sort": Sequence["SortPropertyTypeDef"],
-        "predicate": "PredicateTypeDef",
-        "identifiers": Sequence[str],
-    },
-    total=False,
-)
-
-class ComponentDataConfigurationTypeDef(
-    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
-):
-    pass
-
-ComponentEventTypeDef = TypedDict(
-    "ComponentEventTypeDef",
+SortPropertyTypeDef = TypedDict(
+    "SortPropertyTypeDef",
     {
-        "action": str,
-        "parameters": "ActionParametersTypeDef",
-        "bindingEvent": str,
+        "field": str,
+        "direction": SortDirectionType,
     },
-    total=False,
 )
 
 _RequiredComponentPropertyBindingPropertiesTypeDef = TypedDict(
     "_RequiredComponentPropertyBindingPropertiesTypeDef",
     {
         "property": str,
     },
@@ -451,1264 +377,1602 @@
 
 class ComponentPropertyBindingPropertiesTypeDef(
     _RequiredComponentPropertyBindingPropertiesTypeDef,
     _OptionalComponentPropertyBindingPropertiesTypeDef,
 ):
     pass
 
-ComponentPropertyTypeDef = TypedDict(
-    "ComponentPropertyTypeDef",
+FormBindingElementTypeDef = TypedDict(
+    "FormBindingElementTypeDef",
     {
-        "value": str,
-        "bindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "collectionBindingProperties": "ComponentPropertyBindingPropertiesTypeDef",
-        "defaultValue": str,
-        "model": str,
-        "bindings": Mapping[str, "FormBindingElementTypeDef"],
-        "event": str,
-        "userAttribute": str,
-        "concat": Sequence[Dict[str, Any]],
-        "condition": Dict[str, Any],
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
+        "element": str,
         "property": str,
     },
-    total=False,
 )
 
 ComponentSummaryTypeDef = TypedDict(
     "ComponentSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
     },
 )
 
-_RequiredComponentTypeDef = TypedDict(
-    "_RequiredComponentTypeDef",
+ComponentVariantOutputTypeDef = TypedDict(
+    "ComponentVariantOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "componentType": str,
-        "properties": Dict[str, "ComponentPropertyTypeDef"],
-        "variants": List["ComponentVariantTypeDef"],
+        "variantValues": Dict[str, str],
         "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, "ComponentBindingPropertiesValueTypeDef"],
-        "createdAt": datetime,
-    },
-)
-_OptionalComponentTypeDef = TypedDict(
-    "_OptionalComponentTypeDef",
-    {
-        "sourceId": str,
-        "children": List["ComponentChildTypeDef"],
-        "collectionProperties": Dict[str, "ComponentDataConfigurationTypeDef"],
-        "modifiedAt": datetime,
-        "tags": Dict[str, str],
-        "events": Dict[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
     },
     total=False,
 )
 
-class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
-    pass
-
 ComponentVariantTypeDef = TypedDict(
     "ComponentVariantTypeDef",
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
 )
 
-_RequiredCreateComponentDataTypeDef = TypedDict(
-    "_RequiredCreateComponentDataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+FormDataTypeConfigTypeDef = TypedDict(
+    "FormDataTypeConfigTypeDef",
+    {
+        "dataSourceType": FormDataSourceTypeType,
+        "dataTypeName": str,
+    },
+)
+
+_RequiredCreateThemeDataTypeDef = TypedDict(
+    "_RequiredCreateThemeDataTypeDef",
     {
         "name": str,
-        "componentType": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
-        "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
+        "values": Sequence["ThemeValuesTypeDef"],
     },
 )
-_OptionalCreateComponentDataTypeDef = TypedDict(
-    "_OptionalCreateComponentDataTypeDef",
+_OptionalCreateThemeDataTypeDef = TypedDict(
+    "_OptionalCreateThemeDataTypeDef",
     {
-        "sourceId": str,
-        "children": Sequence["ComponentChildTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
+        "overrides": Sequence["ThemeValuesTypeDef"],
         "tags": Mapping[str, str],
-        "events": Mapping[str, "ComponentEventTypeDef"],
-        "schemaVersion": str,
     },
     total=False,
 )
 
-class CreateComponentDataTypeDef(
-    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
-):
+class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
     pass
 
-_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateComponentRequestRequestTypeDef",
+_RequiredThemeTypeDef = TypedDict(
+    "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "componentToCreate": "CreateComponentDataTypeDef",
+        "id": str,
+        "name": str,
+        "createdAt": datetime,
+        "values": List["ThemeValuesOutputTypeDef"],
     },
 )
-_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateComponentRequestRequestTypeDef",
+_OptionalThemeTypeDef = TypedDict(
+    "_OptionalThemeTypeDef",
     {
-        "clientToken": str,
+        "modifiedAt": datetime,
+        "overrides": List["ThemeValuesOutputTypeDef"],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateComponentRequestRequestTypeDef(
-    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
-):
+class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
 
-CreateComponentResponseTypeDef = TypedDict(
-    "CreateComponentResponseTypeDef",
+DeleteComponentRequestRequestTypeDef = TypedDict(
+    "DeleteComponentRequestRequestTypeDef",
     {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
 
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
+DeleteFormRequestRequestTypeDef = TypedDict(
+    "DeleteFormRequestRequestTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
 )
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
+
+DeleteThemeRequestRequestTypeDef = TypedDict(
+    "DeleteThemeRequestRequestTypeDef",
     {
-        "cta": "FormCTATypeDef",
-        "tags": Mapping[str, str],
-        "labelDecorator": LabelDecoratorType,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
-    pass
-
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
+_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "formToCreate": "CreateFormDataTypeDef",
+        "code": str,
+        "redirectUri": str,
     },
 )
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
+_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
     {
-        "clientToken": str,
+        "clientId": str,
     },
     total=False,
 )
 
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+class ExchangeCodeForTokenRequestBodyTypeDef(
+    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
 ):
     pass
 
-CreateFormResponseTypeDef = TypedDict(
-    "CreateFormResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-_RequiredCreateThemeDataTypeDef = TypedDict(
-    "_RequiredCreateThemeDataTypeDef",
+_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestRequestTypeDef",
     {
-        "name": str,
-        "values": Sequence["ThemeValuesTypeDef"],
+        "appId": str,
+        "environmentName": str,
     },
 )
-_OptionalCreateThemeDataTypeDef = TypedDict(
-    "_OptionalCreateThemeDataTypeDef",
+_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestRequestTypeDef",
     {
-        "overrides": Sequence["ThemeValuesTypeDef"],
-        "tags": Mapping[str, str],
+        "nextToken": str,
     },
     total=False,
 )
 
-class CreateThemeDataTypeDef(_RequiredCreateThemeDataTypeDef, _OptionalCreateThemeDataTypeDef):
+class ExportComponentsRequestRequestTypeDef(
+    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
+):
     pass
 
-_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateThemeRequestRequestTypeDef",
+_RequiredExportFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredExportFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
-        "themeToCreate": "CreateThemeDataTypeDef",
     },
 )
-_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateThemeRequestRequestTypeDef",
+_OptionalExportFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalExportFormsRequestRequestTypeDef",
     {
-        "clientToken": str,
+        "nextToken": str,
     },
     total=False,
 )
 
-class CreateThemeRequestRequestTypeDef(
-    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
+class ExportFormsRequestRequestTypeDef(
+    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
 ):
     pass
 
-CreateThemeResponseTypeDef = TypedDict(
-    "CreateThemeResponseTypeDef",
+_RequiredExportThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredExportThemesRequestRequestTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
     },
 )
-
-DeleteComponentRequestRequestTypeDef = TypedDict(
-    "DeleteComponentRequestRequestTypeDef",
+_OptionalExportThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalExportThemesRequestRequestTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "nextToken": str,
     },
+    total=False,
 )
 
-DeleteFormRequestRequestTypeDef = TypedDict(
-    "DeleteFormRequestRequestTypeDef",
+class ExportThemesRequestRequestTypeDef(
+    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
+):
+    pass
+
+FieldPositionTypeDef = TypedDict(
+    "FieldPositionTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "fixed": Literal["first"],
+        "rightOf": str,
+        "below": str,
     },
+    total=False,
 )
 
-DeleteThemeRequestRequestTypeDef = TypedDict(
-    "DeleteThemeRequestRequestTypeDef",
+_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "type": str,
     },
 )
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationOutputTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "strValues": List[str],
+        "numValues": List[int],
+        "validationMessage": str,
     },
+    total=False,
 )
 
-_RequiredExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredExchangeCodeForTokenRequestBodyTypeDef",
+class FieldValidationConfigurationOutputTypeDef(
+    _RequiredFieldValidationConfigurationOutputTypeDef,
+    _OptionalFieldValidationConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredFieldValidationConfigurationTypeDef = TypedDict(
+    "_RequiredFieldValidationConfigurationTypeDef",
     {
-        "code": str,
-        "redirectUri": str,
+        "type": str,
     },
 )
-_OptionalExchangeCodeForTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalExchangeCodeForTokenRequestBodyTypeDef",
+_OptionalFieldValidationConfigurationTypeDef = TypedDict(
+    "_OptionalFieldValidationConfigurationTypeDef",
     {
-        "clientId": str,
+        "strValues": Sequence[str],
+        "numValues": Sequence[int],
+        "validationMessage": str,
     },
     total=False,
 )
 
-class ExchangeCodeForTokenRequestBodyTypeDef(
-    _RequiredExchangeCodeForTokenRequestBodyTypeDef, _OptionalExchangeCodeForTokenRequestBodyTypeDef
+class FieldValidationConfigurationTypeDef(
+    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
-ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
-    "ExchangeCodeForTokenRequestRequestTypeDef",
+_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigOutputTypeDef",
     {
-        "provider": Literal["figma"],
-        "request": "ExchangeCodeForTokenRequestBodyTypeDef",
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": List[str],
     },
 )
-
-ExchangeCodeForTokenResponseTypeDef = TypedDict(
-    "ExchangeCodeForTokenResponseTypeDef",
+_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigOutputTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
+    total=False,
 )
 
-_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
+class FileUploaderFieldConfigOutputTypeDef(
+    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
+):
+    pass
+
+_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
+    "_RequiredFileUploaderFieldConfigTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "accessLevel": StorageAccessLevelType,
+        "acceptedFileTypes": Sequence[str],
     },
 )
-_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
+_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
+    "_OptionalFileUploaderFieldConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "showThumbnails": bool,
+        "isResumable": bool,
+        "maxFileCount": int,
+        "maxSize": int,
     },
     total=False,
 )
 
-class ExportComponentsRequestExportComponentsPaginateTypeDef(
-    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
-    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
+class FileUploaderFieldConfigTypeDef(
+    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
 ):
     pass
 
-_RequiredExportComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportComponentsRequestRequestTypeDef",
+FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
+    "FormInputBindingPropertiesValuePropertiesTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "model": str,
     },
+    total=False,
 )
-_OptionalExportComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportComponentsRequestRequestTypeDef",
+
+_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
     {
-        "nextToken": str,
+        "property": str,
+    },
+)
+_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
+    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
+    {
+        "field": str,
     },
     total=False,
 )
 
-class ExportComponentsRequestRequestTypeDef(
-    _RequiredExportComponentsRequestRequestTypeDef, _OptionalExportComponentsRequestRequestTypeDef
+class FormInputValuePropertyBindingPropertiesTypeDef(
+    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
+    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
 ):
     pass
 
-ExportComponentsResponseTypeDef = TypedDict(
-    "ExportComponentsResponseTypeDef",
+FormStyleConfigTypeDef = TypedDict(
+    "FormStyleConfigTypeDef",
     {
-        "entities": List["ComponentTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tokenReference": str,
+        "value": str,
     },
+    total=False,
 )
 
-_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
+GetCodegenJobRequestRequestTypeDef = TypedDict(
+    "GetCodegenJobRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "id": str,
     },
 )
-_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
-    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
+
+GetComponentRequestRequestTypeDef = TypedDict(
+    "GetComponentRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
     },
-    total=False,
 )
 
-class ExportFormsRequestExportFormsPaginateTypeDef(
-    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
-    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
-):
-    pass
+GetFormRequestRequestTypeDef = TypedDict(
+    "GetFormRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
 
-_RequiredExportFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredExportFormsRequestRequestTypeDef",
+GetMetadataRequestRequestTypeDef = TypedDict(
+    "GetMetadataRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalExportFormsRequestRequestTypeDef",
+
+GetThemeRequestRequestTypeDef = TypedDict(
+    "GetThemeRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+    },
+)
+
+_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class ExportFormsRequestRequestTypeDef(
-    _RequiredExportFormsRequestRequestTypeDef, _OptionalExportFormsRequestRequestTypeDef
+class ListCodegenJobsRequestRequestTypeDef(
+    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
 ):
     pass
 
-ExportFormsResponseTypeDef = TypedDict(
-    "ExportFormsResponseTypeDef",
+_RequiredListComponentsRequestRequestTypeDef = TypedDict(
+    "_RequiredListComponentsRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListComponentsRequestRequestTypeDef = TypedDict(
+    "_OptionalListComponentsRequestRequestTypeDef",
     {
-        "entities": List["FormTypeDef"],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "maxResults": int,
     },
+    total=False,
 )
 
-_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
+class ListComponentsRequestRequestTypeDef(
+    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListFormsRequestRequestTypeDef = TypedDict(
+    "_RequiredListFormsRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
-    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
+_OptionalListFormsRequestRequestTypeDef = TypedDict(
+    "_OptionalListFormsRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class ExportThemesRequestExportThemesPaginateTypeDef(
-    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
-    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
+class ListFormsRequestRequestTypeDef(
+    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
 ):
     pass
 
-_RequiredExportThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredExportThemesRequestRequestTypeDef",
+_RequiredListThemesRequestRequestTypeDef = TypedDict(
+    "_RequiredListThemesRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalExportThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalExportThemesRequestRequestTypeDef",
+_OptionalListThemesRequestRequestTypeDef = TypedDict(
+    "_OptionalListThemesRequestRequestTypeDef",
     {
         "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-class ExportThemesRequestRequestTypeDef(
-    _RequiredExportThemesRequestRequestTypeDef, _OptionalExportThemesRequestRequestTypeDef
+class ListThemesRequestRequestTypeDef(
+    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
 ):
     pass
 
-ExportThemesResponseTypeDef = TypedDict(
-    "ExportThemesResponseTypeDef",
+ThemeSummaryTypeDef = TypedDict(
+    "ThemeSummaryTypeDef",
     {
-        "entities": List["ThemeTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "name": str,
     },
 )
 
-FieldConfigTypeDef = TypedDict(
-    "FieldConfigTypeDef",
+PredicateOutputTypeDef = TypedDict(
+    "PredicateOutputTypeDef",
     {
-        "label": str,
-        "position": "FieldPositionTypeDef",
-        "excluded": bool,
-        "inputType": "FieldInputConfigTypeDef",
-        "validations": Sequence["FieldValidationConfigurationTypeDef"],
+        "or": List[Dict[str, Any]],
+        "and": List[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
     total=False,
 )
 
-_RequiredFieldInputConfigTypeDef = TypedDict(
-    "_RequiredFieldInputConfigTypeDef",
+PredicateTypeDef = TypedDict(
+    "PredicateTypeDef",
     {
-        "type": str,
+        "or": Sequence[Dict[str, Any]],
+        "and": Sequence[Dict[str, Any]],
+        "field": str,
+        "operator": str,
+        "operand": str,
+        "operandType": str,
     },
+    total=False,
 )
-_OptionalFieldInputConfigTypeDef = TypedDict(
-    "_OptionalFieldInputConfigTypeDef",
+
+PutMetadataFlagBodyTypeDef = TypedDict(
+    "PutMetadataFlagBodyTypeDef",
     {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": "ValueMappingsTypeDef",
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": "FileUploaderFieldConfigTypeDef",
+        "newValue": str,
+    },
+)
+
+_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_RequiredRefreshTokenRequestBodyTypeDef",
+    {
+        "token": str,
+    },
+)
+_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
+    "_OptionalRefreshTokenRequestBodyTypeDef",
+    {
+        "clientId": str,
     },
     total=False,
 )
 
-class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+class RefreshTokenRequestBodyTypeDef(
+    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
+):
     pass
 
-FieldPositionTypeDef = TypedDict(
-    "FieldPositionTypeDef",
+ThemeValueOutputTypeDef = TypedDict(
+    "ThemeValueOutputTypeDef",
     {
-        "fixed": Literal["first"],
-        "rightOf": str,
-        "below": str,
+        "value": str,
+        "children": List[Dict[str, Any]],
     },
     total=False,
 )
 
-_RequiredFieldValidationConfigurationTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationTypeDef",
+ThemeValueTypeDef = TypedDict(
+    "ThemeValueTypeDef",
     {
-        "type": str,
+        "value": str,
+        "children": Sequence[Dict[str, Any]],
     },
+    total=False,
 )
-_OptionalFieldValidationConfigurationTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationTypeDef",
+
+ThemeValuesOutputTypeDef = TypedDict(
+    "ThemeValuesOutputTypeDef",
     {
-        "strValues": Sequence[str],
-        "numValues": Sequence[int],
-        "validationMessage": str,
+        "key": str,
+        "value": Dict[str, Any],
     },
     total=False,
 )
 
-class FieldValidationConfigurationTypeDef(
-    _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
-):
-    pass
+ThemeValuesTypeDef = TypedDict(
+    "ThemeValuesTypeDef",
+    {
+        "key": str,
+        "value": Dict[str, Any],
+    },
+    total=False,
+)
 
-_RequiredFileUploaderFieldConfigTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigTypeDef",
+_RequiredUpdateThemeDataTypeDef = TypedDict(
+    "_RequiredUpdateThemeDataTypeDef",
     {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": Sequence[str],
+        "values": Sequence["ThemeValuesTypeDef"],
     },
 )
-_OptionalFileUploaderFieldConfigTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigTypeDef",
+_OptionalUpdateThemeDataTypeDef = TypedDict(
+    "_OptionalUpdateThemeDataTypeDef",
     {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
+        "id": str,
+        "name": str,
+        "overrides": Sequence["ThemeValuesTypeDef"],
     },
     total=False,
 )
 
-class FileUploaderFieldConfigTypeDef(
-    _RequiredFileUploaderFieldConfigTypeDef, _OptionalFileUploaderFieldConfigTypeDef
-):
+class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
     pass
 
-FormBindingElementTypeDef = TypedDict(
-    "FormBindingElementTypeDef",
+_RequiredValueMappingTypeDef = TypedDict(
+    "_RequiredValueMappingTypeDef",
     {
-        "element": str,
-        "property": str,
+        "value": "FormInputValuePropertyTypeDef",
     },
 )
-
-FormButtonTypeDef = TypedDict(
-    "FormButtonTypeDef",
+_OptionalValueMappingTypeDef = TypedDict(
+    "_OptionalValueMappingTypeDef",
     {
-        "excluded": bool,
-        "children": str,
-        "position": "FieldPositionTypeDef",
+        "displayValue": "FormInputValuePropertyTypeDef",
     },
     total=False,
 )
 
-FormCTATypeDef = TypedDict(
-    "FormCTATypeDef",
+class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
+    pass
+
+ActionParametersOutputTypeDef = TypedDict(
+    "ActionParametersOutputTypeDef",
     {
-        "position": FormButtonsPositionType,
-        "clear": "FormButtonTypeDef",
-        "cancel": "FormButtonTypeDef",
-        "submit": "FormButtonTypeDef",
+        "type": "ComponentPropertyOutputTypeDef",
+        "url": "ComponentPropertyOutputTypeDef",
+        "anchor": "ComponentPropertyOutputTypeDef",
+        "target": "ComponentPropertyOutputTypeDef",
+        "global": "ComponentPropertyOutputTypeDef",
+        "model": str,
+        "id": "ComponentPropertyOutputTypeDef",
+        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
-FormDataTypeConfigTypeDef = TypedDict(
-    "FormDataTypeConfigTypeDef",
+ActionParametersTypeDef = TypedDict(
+    "ActionParametersTypeDef",
     {
-        "dataSourceType": FormDataSourceTypeType,
-        "dataTypeName": str,
+        "type": "ComponentPropertyTypeDef",
+        "url": "ComponentPropertyTypeDef",
+        "anchor": "ComponentPropertyTypeDef",
+        "target": "ComponentPropertyTypeDef",
+        "global": "ComponentPropertyTypeDef",
+        "model": str,
+        "id": "ComponentPropertyTypeDef",
+        "fields": Mapping[str, "ComponentPropertyTypeDef"],
+        "state": MutationActionSetStateParameterTypeDef,
     },
+    total=False,
 )
 
-FormInputBindingPropertiesValuePropertiesTypeDef = TypedDict(
-    "FormInputBindingPropertiesValuePropertiesTypeDef",
+_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldOutputTypeDef",
     {
-        "model": str,
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
-    total=False,
 )
-
-FormInputBindingPropertiesValueTypeDef = TypedDict(
-    "FormInputBindingPropertiesValueTypeDef",
+_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldOutputTypeDef",
     {
-        "type": str,
-        "bindingProperties": "FormInputBindingPropertiesValuePropertiesTypeDef",
+        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_RequiredFormInputValuePropertyBindingPropertiesTypeDef",
+class CodegenGenericDataFieldOutputTypeDef(
+    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
+):
+    pass
+
+_RequiredCodegenGenericDataFieldTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataFieldTypeDef",
     {
-        "property": str,
+        "dataType": CodegenGenericDataFieldDataTypeType,
+        "dataTypeValue": str,
+        "required": bool,
+        "readOnly": bool,
+        "isArray": bool,
     },
 )
-_OptionalFormInputValuePropertyBindingPropertiesTypeDef = TypedDict(
-    "_OptionalFormInputValuePropertyBindingPropertiesTypeDef",
+_OptionalCodegenGenericDataFieldTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataFieldTypeDef",
     {
-        "field": str,
+        "relationship": CodegenGenericDataRelationshipTypeTypeDef,
     },
     total=False,
 )
 
-class FormInputValuePropertyBindingPropertiesTypeDef(
-    _RequiredFormInputValuePropertyBindingPropertiesTypeDef,
-    _OptionalFormInputValuePropertyBindingPropertiesTypeDef,
+class CodegenGenericDataFieldTypeDef(
+    _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
-FormInputValuePropertyTypeDef = TypedDict(
-    "FormInputValuePropertyTypeDef",
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
     {
-        "value": str,
-        "bindingProperties": "FormInputValuePropertyBindingPropertiesTypeDef",
-        "concat": Sequence[Dict[str, Any]],
+        "react": ReactStartCodegenJobDataTypeDef,
     },
     total=False,
 )
 
-FormStyleConfigTypeDef = TypedDict(
-    "FormStyleConfigTypeDef",
+ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueOutputTypeDef",
     {
-        "tokenReference": str,
-        "value": str,
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
+        "defaultValue": str,
     },
     total=False,
 )
 
-FormStyleTypeDef = TypedDict(
-    "FormStyleTypeDef",
+ComponentBindingPropertiesValueTypeDef = TypedDict(
+    "ComponentBindingPropertiesValueTypeDef",
     {
-        "horizontalGap": "FormStyleConfigTypeDef",
-        "verticalGap": "FormStyleConfigTypeDef",
-        "outerPadding": "FormStyleConfigTypeDef",
+        "type": str,
+        "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
+        "defaultValue": str,
     },
     total=False,
 )
 
-FormSummaryTypeDef = TypedDict(
-    "FormSummaryTypeDef",
+_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationOutputTypeDef",
     {
-        "appId": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "environmentName": str,
-        "formActionType": FormActionTypeType,
-        "id": str,
-        "name": str,
+        "model": str,
     },
 )
+_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationOutputTypeDef",
+    {
+        "sort": List[SortPropertyTypeDef],
+        "predicate": "PredicateOutputTypeDef",
+        "identifiers": List[str],
+    },
+    total=False,
+)
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+class ComponentDataConfigurationOutputTypeDef(
+    _RequiredComponentDataConfigurationOutputTypeDef,
+    _OptionalComponentDataConfigurationOutputTypeDef,
+):
+    pass
+
+_RequiredComponentDataConfigurationTypeDef = TypedDict(
+    "_RequiredComponentDataConfigurationTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "name": str,
-        "formActionType": FormActionTypeType,
-        "style": "FormStyleTypeDef",
-        "dataType": "FormDataTypeConfigTypeDef",
-        "fields": Dict[str, "FieldConfigTypeDef"],
-        "sectionalElements": Dict[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
+        "model": str,
     },
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+_OptionalComponentDataConfigurationTypeDef = TypedDict(
+    "_OptionalComponentDataConfigurationTypeDef",
     {
-        "tags": Dict[str, str],
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "sort": Sequence[SortPropertyTypeDef],
+        "predicate": "PredicateTypeDef",
+        "identifiers": Sequence[str],
     },
     total=False,
 )
 
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+class ComponentDataConfigurationTypeDef(
+    _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
+):
     pass
 
-GetCodegenJobRequestRequestTypeDef = TypedDict(
-    "GetCodegenJobRequestRequestTypeDef",
+ComponentPropertyOutputTypeDef = TypedDict(
+    "ComponentPropertyOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "value": str,
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Dict[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": List[Dict[str, Any]],
+        "condition": "ComponentConditionPropertyTypeDef",
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
+    total=False,
 )
 
-GetCodegenJobResponseTypeDef = TypedDict(
-    "GetCodegenJobResponseTypeDef",
+ComponentPropertyTypeDef = TypedDict(
+    "ComponentPropertyTypeDef",
     {
-        "job": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "value": str,
+        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
+        "defaultValue": str,
+        "model": str,
+        "bindings": Mapping[str, FormBindingElementTypeDef],
+        "event": str,
+        "userAttribute": str,
+        "concat": Sequence[Dict[str, Any]],
+        "condition": Dict[str, Any],
+        "configured": bool,
+        "type": str,
+        "importedValue": str,
+        "componentName": str,
+        "property": str,
     },
+    total=False,
 )
 
-GetComponentRequestRequestTypeDef = TypedDict(
-    "GetComponentRequestRequestTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetComponentResponseTypeDef = TypedDict(
-    "GetComponentResponseTypeDef",
+ExchangeCodeForTokenResponseTypeDef = TypedDict(
+    "ExchangeCodeForTokenResponseTypeDef",
     {
-        "component": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessToken": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFormRequestRequestTypeDef = TypedDict(
-    "GetFormRequestRequestTypeDef",
+GetMetadataResponseTypeDef = TypedDict(
+    "GetMetadataResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "features": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetFormResponseTypeDef = TypedDict(
-    "GetFormResponseTypeDef",
+ListCodegenJobsResponseTypeDef = TypedDict(
+    "ListCodegenJobsResponseTypeDef",
     {
-        "form": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entities": List[CodegenJobSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMetadataRequestRequestTypeDef = TypedDict(
-    "GetMetadataRequestRequestTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "entities": List[ComponentSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetMetadataResponseTypeDef = TypedDict(
-    "GetMetadataResponseTypeDef",
+RefreshTokenResponseTypeDef = TypedDict(
+    "RefreshTokenResponseTypeDef",
     {
-        "features": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "accessToken": str,
+        "expiresIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetThemeRequestRequestTypeDef = TypedDict(
-    "GetThemeRequestRequestTypeDef",
+FormSummaryTypeDef = TypedDict(
+    "FormSummaryTypeDef",
     {
         "appId": str,
+        "dataType": FormDataTypeConfigTypeDef,
         "environmentName": str,
+        "formActionType": FormActionTypeType,
         "id": str,
+        "name": str,
     },
 )
 
-GetThemeResponseTypeDef = TypedDict(
-    "GetThemeResponseTypeDef",
-    {
-        "theme": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_RequiredCreateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateThemeRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
+        "themeToCreate": CreateThemeDataTypeDef,
     },
 )
-_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
+_OptionalCreateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateThemeRequestRequestTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "clientToken": str,
     },
     total=False,
 )
 
-class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
-    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
-    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+class CreateThemeRequestRequestTypeDef(
+    _RequiredCreateThemeRequestRequestTypeDef, _OptionalCreateThemeRequestRequestTypeDef
 ):
     pass
 
-_RequiredListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_RequiredListCodegenJobsRequestRequestTypeDef",
+CreateThemeResponseTypeDef = TypedDict(
+    "CreateThemeResponseTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalListCodegenJobsRequestRequestTypeDef = TypedDict(
-    "_OptionalListCodegenJobsRequestRequestTypeDef",
+
+ExportThemesResponseTypeDef = TypedDict(
+    "ExportThemesResponseTypeDef",
     {
+        "entities": List[ThemeTypeDef],
         "nextToken": str,
-        "maxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ListCodegenJobsRequestRequestTypeDef(
-    _RequiredListCodegenJobsRequestRequestTypeDef, _OptionalListCodegenJobsRequestRequestTypeDef
-):
-    pass
+GetThemeResponseTypeDef = TypedDict(
+    "GetThemeResponseTypeDef",
+    {
+        "theme": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ListCodegenJobsResponseTypeDef = TypedDict(
-    "ListCodegenJobsResponseTypeDef",
+UpdateThemeResponseTypeDef = TypedDict(
+    "UpdateThemeResponseTypeDef",
     {
-        "entities": List["CodegenJobSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entity": ThemeTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
+ExchangeCodeForTokenRequestRequestTypeDef = TypedDict(
+    "ExchangeCodeForTokenRequestRequestTypeDef",
+    {
+        "provider": Literal["figma"],
+        "request": ExchangeCodeForTokenRequestBodyTypeDef,
+    },
+)
+
+_RequiredExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_RequiredExportComponentsRequestExportComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
-    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
+_OptionalExportComponentsRequestExportComponentsPaginateTypeDef = TypedDict(
+    "_OptionalExportComponentsRequestExportComponentsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListComponentsRequestListComponentsPaginateTypeDef(
-    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
-    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
+class ExportComponentsRequestExportComponentsPaginateTypeDef(
+    _RequiredExportComponentsRequestExportComponentsPaginateTypeDef,
+    _OptionalExportComponentsRequestExportComponentsPaginateTypeDef,
 ):
     pass
 
-_RequiredListComponentsRequestRequestTypeDef = TypedDict(
-    "_RequiredListComponentsRequestRequestTypeDef",
+_RequiredExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_RequiredExportFormsRequestExportFormsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListComponentsRequestRequestTypeDef = TypedDict(
-    "_OptionalListComponentsRequestRequestTypeDef",
+_OptionalExportFormsRequestExportFormsPaginateTypeDef = TypedDict(
+    "_OptionalExportFormsRequestExportFormsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListComponentsRequestRequestTypeDef(
-    _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
+class ExportFormsRequestExportFormsPaginateTypeDef(
+    _RequiredExportFormsRequestExportFormsPaginateTypeDef,
+    _OptionalExportFormsRequestExportFormsPaginateTypeDef,
 ):
     pass
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+_RequiredExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_RequiredExportThemesRequestExportThemesPaginateTypeDef",
     {
-        "entities": List["ComponentSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalExportThemesRequestExportThemesPaginateTypeDef = TypedDict(
+    "_OptionalExportThemesRequestExportThemesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_RequiredListFormsRequestListFormsPaginateTypeDef",
+class ExportThemesRequestExportThemesPaginateTypeDef(
+    _RequiredExportThemesRequestExportThemesPaginateTypeDef,
+    _OptionalExportThemesRequestExportThemesPaginateTypeDef,
+):
+    pass
+
+_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
-    "_OptionalListFormsRequestListFormsPaginateTypeDef",
+_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef = TypedDict(
+    "_OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListFormsRequestListFormsPaginateTypeDef(
-    _RequiredListFormsRequestListFormsPaginateTypeDef,
-    _OptionalListFormsRequestListFormsPaginateTypeDef,
+class ListCodegenJobsRequestListCodegenJobsPaginateTypeDef(
+    _RequiredListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    _OptionalListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
 ):
     pass
 
-_RequiredListFormsRequestRequestTypeDef = TypedDict(
-    "_RequiredListFormsRequestRequestTypeDef",
+_RequiredListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_RequiredListComponentsRequestListComponentsPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
-_OptionalListFormsRequestRequestTypeDef = TypedDict(
-    "_OptionalListFormsRequestRequestTypeDef",
+_OptionalListComponentsRequestListComponentsPaginateTypeDef = TypedDict(
+    "_OptionalListComponentsRequestListComponentsPaginateTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class ListFormsRequestRequestTypeDef(
-    _RequiredListFormsRequestRequestTypeDef, _OptionalListFormsRequestRequestTypeDef
+class ListComponentsRequestListComponentsPaginateTypeDef(
+    _RequiredListComponentsRequestListComponentsPaginateTypeDef,
+    _OptionalListComponentsRequestListComponentsPaginateTypeDef,
 ):
     pass
 
-ListFormsResponseTypeDef = TypedDict(
-    "ListFormsResponseTypeDef",
+_RequiredListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_RequiredListFormsRequestListFormsPaginateTypeDef",
     {
-        "entities": List["FormSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "appId": str,
+        "environmentName": str,
+    },
+)
+_OptionalListFormsRequestListFormsPaginateTypeDef = TypedDict(
+    "_OptionalListFormsRequestListFormsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListFormsRequestListFormsPaginateTypeDef(
+    _RequiredListFormsRequestListFormsPaginateTypeDef,
+    _OptionalListFormsRequestListFormsPaginateTypeDef,
+):
+    pass
+
 _RequiredListThemesRequestListThemesPaginateTypeDef = TypedDict(
     "_RequiredListThemesRequestListThemesPaginateTypeDef",
     {
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalListThemesRequestListThemesPaginateTypeDef = TypedDict(
     "_OptionalListThemesRequestListThemesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListThemesRequestListThemesPaginateTypeDef(
     _RequiredListThemesRequestListThemesPaginateTypeDef,
     _OptionalListThemesRequestListThemesPaginateTypeDef,
 ):
     pass
 
-_RequiredListThemesRequestRequestTypeDef = TypedDict(
-    "_RequiredListThemesRequestRequestTypeDef",
+FormButtonTypeDef = TypedDict(
+    "FormButtonTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
+        "excluded": bool,
+        "children": str,
+        "position": FieldPositionTypeDef,
     },
+    total=False,
 )
-_OptionalListThemesRequestRequestTypeDef = TypedDict(
-    "_OptionalListThemesRequestRequestTypeDef",
+
+_RequiredSectionalElementTypeDef = TypedDict(
+    "_RequiredSectionalElementTypeDef",
     {
-        "nextToken": str,
-        "maxResults": int,
+        "type": str,
     },
-    total=False,
 )
-
-class ListThemesRequestRequestTypeDef(
-    _RequiredListThemesRequestRequestTypeDef, _OptionalListThemesRequestRequestTypeDef
-):
-    pass
-
-ListThemesResponseTypeDef = TypedDict(
-    "ListThemesResponseTypeDef",
+_OptionalSectionalElementTypeDef = TypedDict(
+    "_OptionalSectionalElementTypeDef",
     {
-        "entities": List["ThemeSummaryTypeDef"],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "position": FieldPositionTypeDef,
+        "text": str,
+        "level": int,
+        "orientation": str,
+        "excluded": bool,
     },
+    total=False,
 )
 
-MutationActionSetStateParameterTypeDef = TypedDict(
-    "MutationActionSetStateParameterTypeDef",
+class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+    pass
+
+FormInputBindingPropertiesValueTypeDef = TypedDict(
+    "FormInputBindingPropertiesValueTypeDef",
     {
-        "componentName": str,
-        "property": str,
-        "set": "ComponentPropertyTypeDef",
+        "type": str,
+        "bindingProperties": FormInputBindingPropertiesValuePropertiesTypeDef,
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+FormInputValuePropertyTypeDef = TypedDict(
+    "FormInputValuePropertyTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "value": str,
+        "bindingProperties": FormInputValuePropertyBindingPropertiesTypeDef,
+        "concat": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-PredicateTypeDef = TypedDict(
-    "PredicateTypeDef",
+FormStyleTypeDef = TypedDict(
+    "FormStyleTypeDef",
     {
-        "or": Sequence[Dict[str, Any]],
-        "and": Sequence[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
+        "horizontalGap": FormStyleConfigTypeDef,
+        "verticalGap": FormStyleConfigTypeDef,
+        "outerPadding": FormStyleConfigTypeDef,
     },
     total=False,
 )
 
-PutMetadataFlagBodyTypeDef = TypedDict(
-    "PutMetadataFlagBodyTypeDef",
+ListThemesResponseTypeDef = TypedDict(
+    "ListThemesResponseTypeDef",
     {
-        "newValue": str,
+        "entities": List[ThemeSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetadataFlagRequestRequestTypeDef = TypedDict(
     "PutMetadataFlagRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "featureName": str,
-        "body": "PutMetadataFlagBodyTypeDef",
+        "body": PutMetadataFlagBodyTypeDef,
     },
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
+RefreshTokenRequestRequestTypeDef = TypedDict(
+    "RefreshTokenRequestRequestTypeDef",
     {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
+        "provider": Literal["figma"],
+        "refreshTokenBody": RefreshTokenRequestBodyTypeDef,
     },
-    total=False,
 )
 
-_RequiredRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_RequiredRefreshTokenRequestBodyTypeDef",
+_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateThemeRequestRequestTypeDef",
     {
-        "token": str,
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedTheme": UpdateThemeDataTypeDef,
     },
 )
-_OptionalRefreshTokenRequestBodyTypeDef = TypedDict(
-    "_OptionalRefreshTokenRequestBodyTypeDef",
+_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateThemeRequestRequestTypeDef",
     {
-        "clientId": str,
+        "clientToken": str,
     },
     total=False,
 )
 
-class RefreshTokenRequestBodyTypeDef(
-    _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
+class UpdateThemeRequestRequestTypeDef(
+    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
-RefreshTokenRequestRequestTypeDef = TypedDict(
-    "RefreshTokenRequestRequestTypeDef",
+ComponentEventOutputTypeDef = TypedDict(
+    "ComponentEventOutputTypeDef",
     {
-        "provider": Literal["figma"],
-        "refreshTokenBody": "RefreshTokenRequestBodyTypeDef",
+        "action": str,
+        "parameters": ActionParametersOutputTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-RefreshTokenResponseTypeDef = TypedDict(
-    "RefreshTokenResponseTypeDef",
+ComponentEventTypeDef = TypedDict(
+    "ComponentEventTypeDef",
     {
-        "accessToken": str,
-        "expiresIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "action": str,
+        "parameters": ActionParametersTypeDef,
+        "bindingEvent": str,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
+        "primaryKeys": List[str],
     },
 )
+_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelOutputTypeDef",
+    {
+        "isJoinTable": bool,
+    },
+    total=False,
+)
 
-_RequiredSectionalElementTypeDef = TypedDict(
-    "_RequiredSectionalElementTypeDef",
+class CodegenGenericDataModelOutputTypeDef(
+    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
+):
+    pass
+
+CodegenGenericDataNonModelOutputTypeDef = TypedDict(
+    "CodegenGenericDataNonModelOutputTypeDef",
     {
-        "type": str,
+        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
     },
 )
-_OptionalSectionalElementTypeDef = TypedDict(
-    "_OptionalSectionalElementTypeDef",
+
+_RequiredCodegenGenericDataModelTypeDef = TypedDict(
+    "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "position": "FieldPositionTypeDef",
-        "text": str,
-        "level": int,
-        "orientation": str,
-        "excluded": bool,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": Sequence[str],
+    },
+)
+_OptionalCodegenGenericDataModelTypeDef = TypedDict(
+    "_OptionalCodegenGenericDataModelTypeDef",
+    {
+        "isJoinTable": bool,
     },
     total=False,
 )
 
-class SectionalElementTypeDef(_RequiredSectionalElementTypeDef, _OptionalSectionalElementTypeDef):
+class CodegenGenericDataModelTypeDef(
+    _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
+):
     pass
 
-SortPropertyTypeDef = TypedDict(
-    "SortPropertyTypeDef",
+CodegenGenericDataNonModelTypeDef = TypedDict(
+    "CodegenGenericDataNonModelTypeDef",
     {
-        "field": str,
-        "direction": SortDirectionType,
+        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
-_RequiredStartCodegenJobDataTypeDef = TypedDict(
-    "_RequiredStartCodegenJobDataTypeDef",
+ListFormsResponseTypeDef = TypedDict(
+    "ListFormsResponseTypeDef",
     {
-        "renderConfig": "CodegenJobRenderConfigTypeDef",
+        "entities": List[FormSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartCodegenJobDataTypeDef = TypedDict(
-    "_OptionalStartCodegenJobDataTypeDef",
+
+FormCTATypeDef = TypedDict(
+    "FormCTATypeDef",
     {
-        "genericDataSchema": "CodegenJobGenericDataSchemaTypeDef",
-        "autoGenerateForms": bool,
-        "features": "CodegenFeatureFlagsTypeDef",
-        "tags": Mapping[str, str],
+        "position": FormButtonsPositionType,
+        "clear": FormButtonTypeDef,
+        "cancel": FormButtonTypeDef,
+        "submit": FormButtonTypeDef,
     },
     total=False,
 )
 
-class StartCodegenJobDataTypeDef(
-    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
-):
-    pass
-
-_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_RequiredStartCodegenJobRequestRequestTypeDef",
+_RequiredValueMappingsOutputTypeDef = TypedDict(
+    "_RequiredValueMappingsOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "codegenJobToCreate": "StartCodegenJobDataTypeDef",
+        "values": List[ValueMappingTypeDef],
     },
 )
-_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
-    "_OptionalStartCodegenJobRequestRequestTypeDef",
+_OptionalValueMappingsOutputTypeDef = TypedDict(
+    "_OptionalValueMappingsOutputTypeDef",
     {
-        "clientToken": str,
+        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
     },
     total=False,
 )
 
-class StartCodegenJobRequestRequestTypeDef(
-    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
+class ValueMappingsOutputTypeDef(
+    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
 ):
     pass
 
-StartCodegenJobResponseTypeDef = TypedDict(
-    "StartCodegenJobResponseTypeDef",
+_RequiredValueMappingsTypeDef = TypedDict(
+    "_RequiredValueMappingsTypeDef",
+    {
+        "values": Sequence[ValueMappingTypeDef],
+    },
+)
+_OptionalValueMappingsTypeDef = TypedDict(
+    "_OptionalValueMappingsTypeDef",
     {
-        "entity": "CodegenJobTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "bindingProperties": Mapping[str, FormInputBindingPropertiesValueTypeDef],
     },
+    total=False,
 )
 
-ThemeSummaryTypeDef = TypedDict(
-    "ThemeSummaryTypeDef",
+class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
+    pass
+
+_RequiredComponentChildOutputTypeDef = TypedDict(
+    "_RequiredComponentChildOutputTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
+        "componentType": str,
         "name": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+    },
+)
+_OptionalComponentChildOutputTypeDef = TypedDict(
+    "_OptionalComponentChildOutputTypeDef",
+    {
+        "children": List[Dict[str, Any]],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "sourceId": str,
     },
+    total=False,
 )
 
-_RequiredThemeTypeDef = TypedDict(
-    "_RequiredThemeTypeDef",
+class ComponentChildOutputTypeDef(
+    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
+):
+    pass
+
+_RequiredComponentTypeDef = TypedDict(
+    "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
+        "componentType": str,
+        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "variants": List[ComponentVariantOutputTypeDef],
+        "overrides": Dict[str, Dict[str, str]],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
         "createdAt": datetime,
-        "values": List["ThemeValuesTypeDef"],
     },
 )
-_OptionalThemeTypeDef = TypedDict(
-    "_OptionalThemeTypeDef",
+_OptionalComponentTypeDef = TypedDict(
+    "_OptionalComponentTypeDef",
     {
+        "sourceId": str,
+        "children": List["ComponentChildOutputTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesTypeDef"],
         "tags": Dict[str, str],
+        "events": Dict[str, ComponentEventOutputTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
-class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
+class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
-ThemeValueTypeDef = TypedDict(
-    "ThemeValueTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
+    {
+        "componentType": str,
+        "name": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+    },
+)
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "value": str,
         "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "sourceId": str,
     },
     total=False,
 )
 
-ThemeValuesTypeDef = TypedDict(
-    "ThemeValuesTypeDef",
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
+    pass
+
+_RequiredCreateComponentDataTypeDef = TypedDict(
+    "_RequiredCreateComponentDataTypeDef",
     {
-        "key": str,
-        "value": Dict[str, Any],
+        "name": str,
+        "componentType": str,
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
+        "overrides": Mapping[str, Mapping[str, str]],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+    },
+)
+_OptionalCreateComponentDataTypeDef = TypedDict(
+    "_OptionalCreateComponentDataTypeDef",
+    {
+        "sourceId": str,
+        "children": Sequence["ComponentChildTypeDef"],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "tags": Mapping[str, str],
+        "events": Mapping[str, ComponentEventTypeDef],
+        "schemaVersion": str,
     },
     total=False,
 )
 
+class CreateComponentDataTypeDef(
+    _RequiredCreateComponentDataTypeDef, _OptionalCreateComponentDataTypeDef
+):
+    pass
+
 UpdateComponentDataTypeDef = TypedDict(
     "UpdateComponentDataTypeDef",
     {
         "id": str,
         "name": str,
         "sourceId": str,
         "componentType": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
         "children": Sequence["ComponentChildTypeDef"],
-        "variants": Sequence["ComponentVariantTypeDef"],
+        "variants": Sequence[ComponentVariantTypeDef],
         "overrides": Mapping[str, Mapping[str, str]],
-        "bindingProperties": Mapping[str, "ComponentBindingPropertiesValueTypeDef"],
-        "collectionProperties": Mapping[str, "ComponentDataConfigurationTypeDef"],
-        "events": Mapping[str, "ComponentEventTypeDef"],
+        "bindingProperties": Mapping[str, ComponentBindingPropertiesValueTypeDef],
+        "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
+        "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaOutputTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
+    },
+)
+
+CodegenJobGenericDataSchemaTypeDef = TypedDict(
+    "CodegenJobGenericDataSchemaTypeDef",
+    {
+        "dataSourceType": Literal["DataStore"],
+        "models": Mapping[str, CodegenGenericDataModelTypeDef],
+        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
+    },
+)
+
+_RequiredFieldInputConfigOutputTypeDef = TypedDict(
+    "_RequiredFieldInputConfigOutputTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigOutputTypeDef = TypedDict(
+    "_OptionalFieldInputConfigOutputTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsOutputTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class FieldInputConfigOutputTypeDef(
+    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
+):
+    pass
+
+_RequiredFieldInputConfigTypeDef = TypedDict(
+    "_RequiredFieldInputConfigTypeDef",
+    {
+        "type": str,
+    },
+)
+_OptionalFieldInputConfigTypeDef = TypedDict(
+    "_OptionalFieldInputConfigTypeDef",
+    {
+        "required": bool,
+        "readOnly": bool,
+        "placeholder": str,
+        "defaultValue": str,
+        "descriptiveText": str,
+        "defaultChecked": bool,
+        "defaultCountryCode": str,
+        "valueMappings": ValueMappingsTypeDef,
+        "name": str,
+        "minValue": float,
+        "maxValue": float,
+        "step": float,
+        "value": str,
+        "isArray": bool,
+        "fileUploaderConfig": FileUploaderFieldConfigTypeDef,
+    },
+    total=False,
+)
+
+class FieldInputConfigTypeDef(_RequiredFieldInputConfigTypeDef, _OptionalFieldInputConfigTypeDef):
+    pass
+
+CreateComponentResponseTypeDef = TypedDict(
+    "CreateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportComponentsResponseTypeDef = TypedDict(
+    "ExportComponentsResponseTypeDef",
+    {
+        "entities": List[ComponentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComponentResponseTypeDef = TypedDict(
+    "GetComponentResponseTypeDef",
+    {
+        "component": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentResponseTypeDef = TypedDict(
+    "UpdateComponentResponseTypeDef",
+    {
+        "entity": ComponentTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateComponentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateComponentRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "componentToCreate": CreateComponentDataTypeDef,
+    },
+)
+_OptionalCreateComponentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateComponentRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateComponentRequestRequestTypeDef(
+    _RequiredCreateComponentRequestRequestTypeDef, _OptionalCreateComponentRequestRequestTypeDef
+):
+    pass
+
 _RequiredUpdateComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateComponentRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedComponent": "UpdateComponentDataTypeDef",
+        "updatedComponent": UpdateComponentDataTypeDef,
     },
 )
 _OptionalUpdateComponentRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
@@ -1716,143 +1980,262 @@
 )
 
 class UpdateComponentRequestRequestTypeDef(
     _RequiredUpdateComponentRequestRequestTypeDef, _OptionalUpdateComponentRequestRequestTypeDef
 ):
     pass
 
-UpdateComponentResponseTypeDef = TypedDict(
-    "UpdateComponentResponseTypeDef",
+_RequiredCodegenJobTypeDef = TypedDict(
+    "_RequiredCodegenJobTypeDef",
     {
-        "entity": "ComponentTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "id": str,
+        "appId": str,
+        "environmentName": str,
     },
 )
-
-UpdateFormDataTypeDef = TypedDict(
-    "UpdateFormDataTypeDef",
+_OptionalCodegenJobTypeDef = TypedDict(
+    "_OptionalCodegenJobTypeDef",
     {
-        "name": str,
-        "dataType": "FormDataTypeConfigTypeDef",
-        "formActionType": FormActionTypeType,
-        "fields": Mapping[str, "FieldConfigTypeDef"],
-        "style": "FormStyleTypeDef",
-        "sectionalElements": Mapping[str, "SectionalElementTypeDef"],
-        "schemaVersion": str,
-        "cta": "FormCTATypeDef",
-        "labelDecorator": LabelDecoratorType,
+        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "status": CodegenJobStatusType,
+        "statusMessage": str,
+        "asset": CodegenJobAssetTypeDef,
+        "tags": Dict[str, str],
+        "createdAt": datetime,
+        "modifiedAt": datetime,
     },
     total=False,
 )
 
-_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateFormRequestRequestTypeDef",
+class CodegenJobTypeDef(_RequiredCodegenJobTypeDef, _OptionalCodegenJobTypeDef):
+    pass
+
+_RequiredStartCodegenJobDataTypeDef = TypedDict(
+    "_RequiredStartCodegenJobDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
-        "updatedForm": "UpdateFormDataTypeDef",
+        "renderConfig": CodegenJobRenderConfigTypeDef,
     },
 )
-_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateFormRequestRequestTypeDef",
+_OptionalStartCodegenJobDataTypeDef = TypedDict(
+    "_OptionalStartCodegenJobDataTypeDef",
     {
-        "clientToken": str,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
+        "autoGenerateForms": bool,
+        "features": CodegenFeatureFlagsTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateFormRequestRequestTypeDef(
-    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+class StartCodegenJobDataTypeDef(
+    _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
-UpdateFormResponseTypeDef = TypedDict(
-    "UpdateFormResponseTypeDef",
+FieldConfigOutputTypeDef = TypedDict(
+    "FieldConfigOutputTypeDef",
     {
-        "entity": "FormTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigOutputTypeDef,
+        "validations": List[FieldValidationConfigurationOutputTypeDef],
     },
+    total=False,
 )
 
-_RequiredUpdateThemeDataTypeDef = TypedDict(
-    "_RequiredUpdateThemeDataTypeDef",
+FieldConfigTypeDef = TypedDict(
+    "FieldConfigTypeDef",
     {
-        "values": Sequence["ThemeValuesTypeDef"],
+        "label": str,
+        "position": FieldPositionTypeDef,
+        "excluded": bool,
+        "inputType": FieldInputConfigTypeDef,
+        "validations": Sequence[FieldValidationConfigurationTypeDef],
     },
+    total=False,
 )
-_OptionalUpdateThemeDataTypeDef = TypedDict(
-    "_OptionalUpdateThemeDataTypeDef",
+
+GetCodegenJobResponseTypeDef = TypedDict(
+    "GetCodegenJobResponseTypeDef",
     {
-        "id": str,
-        "name": str,
-        "overrides": Sequence["ThemeValuesTypeDef"],
+        "job": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCodegenJobResponseTypeDef = TypedDict(
+    "StartCodegenJobResponseTypeDef",
+    {
+        "entity": CodegenJobTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_RequiredStartCodegenJobRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "codegenJobToCreate": StartCodegenJobDataTypeDef,
+    },
+)
+_OptionalStartCodegenJobRequestRequestTypeDef = TypedDict(
+    "_OptionalStartCodegenJobRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
-class UpdateThemeDataTypeDef(_RequiredUpdateThemeDataTypeDef, _OptionalUpdateThemeDataTypeDef):
+class StartCodegenJobRequestRequestTypeDef(
+    _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
+):
     pass
 
-_RequiredUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateThemeRequestRequestTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
-        "updatedTheme": "UpdateThemeDataTypeDef",
+        "name": str,
+        "formActionType": FormActionTypeType,
+        "style": FormStyleTypeDef,
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigOutputTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "schemaVersion": str,
     },
 )
-_OptionalUpdateThemeRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateThemeRequestRequestTypeDef",
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
     {
-        "clientToken": str,
+        "tags": Dict[str, str],
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
-class UpdateThemeRequestRequestTypeDef(
-    _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
-):
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
-UpdateThemeResponseTypeDef = TypedDict(
-    "UpdateThemeResponseTypeDef",
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "entity": "ThemeTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+    },
+)
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
+    {
+        "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
 
-_RequiredValueMappingTypeDef = TypedDict(
-    "_RequiredValueMappingTypeDef",
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+    pass
+
+UpdateFormDataTypeDef = TypedDict(
+    "UpdateFormDataTypeDef",
     {
-        "value": "FormInputValuePropertyTypeDef",
+        "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
+        "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
+        "style": FormStyleTypeDef,
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "schemaVersion": str,
+        "cta": FormCTATypeDef,
+        "labelDecorator": LabelDecoratorType,
     },
+    total=False,
 )
-_OptionalValueMappingTypeDef = TypedDict(
-    "_OptionalValueMappingTypeDef",
+
+CreateFormResponseTypeDef = TypedDict(
+    "CreateFormResponseTypeDef",
     {
-        "displayValue": "FormInputValuePropertyTypeDef",
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportFormsResponseTypeDef = TypedDict(
+    "ExportFormsResponseTypeDef",
+    {
+        "entities": List[FormTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFormResponseTypeDef = TypedDict(
+    "GetFormResponseTypeDef",
+    {
+        "form": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFormResponseTypeDef = TypedDict(
+    "UpdateFormResponseTypeDef",
+    {
+        "entity": FormTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
+    },
+)
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
+    {
+        "clientToken": str,
     },
     total=False,
 )
 
-class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+):
     pass
 
-_RequiredValueMappingsTypeDef = TypedDict(
-    "_RequiredValueMappingsTypeDef",
+_RequiredUpdateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateFormRequestRequestTypeDef",
     {
-        "values": Sequence["ValueMappingTypeDef"],
+        "appId": str,
+        "environmentName": str,
+        "id": str,
+        "updatedForm": UpdateFormDataTypeDef,
     },
 )
-_OptionalValueMappingsTypeDef = TypedDict(
-    "_OptionalValueMappingsTypeDef",
+_OptionalUpdateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateFormRequestRequestTypeDef",
     {
-        "bindingProperties": Mapping[str, "FormInputBindingPropertiesValueTypeDef"],
+        "clientToken": str,
     },
     total=False,
 )
 
-class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
+class UpdateFormRequestRequestTypeDef(
+    _RequiredUpdateFormRequestRequestTypeDef, _OptionalUpdateFormRequestRequestTypeDef
+):
     pass
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-amplifyuibuilder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore amplifyuibuilder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore amplifyuibuilder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-amplifyuibuilder"></a>
 
 # types-aiobotocore-amplifyuibuilder
 
 [![PyPI - types-aiobotocore-amplifyuibuilder](https://img.shields.io/pypi/v/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-amplifyuibuilder?color=blue)](https://pypistats.org/packages/types-aiobotocore-amplifyuibuilder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-amplifyuibuilder)](https://pepy.tech/project/types-aiobotocore-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AmplifyUIBuilder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
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
 [types-aiobotocore-amplifyuibuilder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder/).
 
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
@@ -344,144 +343,166 @@
 )
 
 
 def check_value(value: CodegenGenericDataFieldDataTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_amplifyuibuilder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_amplifyuibuilder.type_defs import (
-    ActionParametersTypeDef,
+    MutationActionSetStateParameterTypeDef,
     CodegenFeatureFlagsTypeDef,
+    CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
-    CodegenGenericDataFieldTypeDef,
-    CodegenGenericDataModelTypeDef,
-    CodegenGenericDataNonModelTypeDef,
+    CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    CodegenJobGenericDataSchemaTypeDef,
-    CodegenJobRenderConfigTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
-    CodegenJobTypeDef,
+    ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
-    ComponentBindingPropertiesValueTypeDef,
-    ComponentChildTypeDef,
     ComponentConditionPropertyTypeDef,
-    ComponentDataConfigurationTypeDef,
-    ComponentEventTypeDef,
+    SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
-    ComponentPropertyTypeDef,
+    FormBindingElementTypeDef,
     ComponentSummaryTypeDef,
-    ComponentTypeDef,
+    ComponentVariantOutputTypeDef,
     ComponentVariantTypeDef,
-    CreateComponentDataTypeDef,
-    CreateComponentRequestRequestTypeDef,
-    CreateComponentResponseTypeDef,
-    CreateFormDataTypeDef,
-    CreateFormRequestRequestTypeDef,
-    CreateFormResponseTypeDef,
+    ResponseMetadataTypeDef,
+    FormDataTypeConfigTypeDef,
     CreateThemeDataTypeDef,
-    CreateThemeRequestRequestTypeDef,
-    CreateThemeResponseTypeDef,
+    ThemeTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteFormRequestRequestTypeDef,
     DeleteThemeRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExchangeCodeForTokenRequestBodyTypeDef,
-    ExchangeCodeForTokenRequestRequestTypeDef,
-    ExchangeCodeForTokenResponseTypeDef,
-    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ExportComponentsRequestRequestTypeDef,
-    ExportComponentsResponseTypeDef,
-    ExportFormsRequestExportFormsPaginateTypeDef,
     ExportFormsRequestRequestTypeDef,
-    ExportFormsResponseTypeDef,
-    ExportThemesRequestExportThemesPaginateTypeDef,
     ExportThemesRequestRequestTypeDef,
-    ExportThemesResponseTypeDef,
-    FieldConfigTypeDef,
-    FieldInputConfigTypeDef,
     FieldPositionTypeDef,
+    FieldValidationConfigurationOutputTypeDef,
     FieldValidationConfigurationTypeDef,
+    FileUploaderFieldConfigOutputTypeDef,
     FileUploaderFieldConfigTypeDef,
-    FormBindingElementTypeDef,
-    FormButtonTypeDef,
-    FormCTATypeDef,
-    FormDataTypeConfigTypeDef,
     FormInputBindingPropertiesValuePropertiesTypeDef,
-    FormInputBindingPropertiesValueTypeDef,
     FormInputValuePropertyBindingPropertiesTypeDef,
-    FormInputValuePropertyTypeDef,
     FormStyleConfigTypeDef,
-    FormStyleTypeDef,
-    FormSummaryTypeDef,
-    FormTypeDef,
     GetCodegenJobRequestRequestTypeDef,
-    GetCodegenJobResponseTypeDef,
     GetComponentRequestRequestTypeDef,
-    GetComponentResponseTypeDef,
     GetFormRequestRequestTypeDef,
-    GetFormResponseTypeDef,
     GetMetadataRequestRequestTypeDef,
-    GetMetadataResponseTypeDef,
     GetThemeRequestRequestTypeDef,
-    GetThemeResponseTypeDef,
-    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
     ListCodegenJobsRequestRequestTypeDef,
-    ListCodegenJobsResponseTypeDef,
-    ListComponentsRequestListComponentsPaginateTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListComponentsResponseTypeDef,
-    ListFormsRequestListFormsPaginateTypeDef,
     ListFormsRequestRequestTypeDef,
-    ListFormsResponseTypeDef,
-    ListThemesRequestListThemesPaginateTypeDef,
     ListThemesRequestRequestTypeDef,
-    ListThemesResponseTypeDef,
-    MutationActionSetStateParameterTypeDef,
-    PaginatorConfigTypeDef,
+    ThemeSummaryTypeDef,
+    PredicateOutputTypeDef,
     PredicateTypeDef,
     PutMetadataFlagBodyTypeDef,
-    PutMetadataFlagRequestRequestTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     RefreshTokenRequestBodyTypeDef,
-    RefreshTokenRequestRequestTypeDef,
-    RefreshTokenResponseTypeDef,
-    ResponseMetadataTypeDef,
-    SectionalElementTypeDef,
-    SortPropertyTypeDef,
-    StartCodegenJobDataTypeDef,
-    StartCodegenJobRequestRequestTypeDef,
-    StartCodegenJobResponseTypeDef,
-    ThemeSummaryTypeDef,
-    ThemeTypeDef,
+    ThemeValueOutputTypeDef,
     ThemeValueTypeDef,
+    ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
+    UpdateThemeDataTypeDef,
+    ValueMappingTypeDef,
+    ActionParametersOutputTypeDef,
+    ActionParametersTypeDef,
+    CodegenGenericDataFieldOutputTypeDef,
+    CodegenGenericDataFieldTypeDef,
+    CodegenJobRenderConfigTypeDef,
+    ComponentBindingPropertiesValueOutputTypeDef,
+    ComponentBindingPropertiesValueTypeDef,
+    ComponentDataConfigurationOutputTypeDef,
+    ComponentDataConfigurationTypeDef,
+    ComponentPropertyOutputTypeDef,
+    ComponentPropertyTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExchangeCodeForTokenResponseTypeDef,
+    GetMetadataResponseTypeDef,
+    ListCodegenJobsResponseTypeDef,
+    ListComponentsResponseTypeDef,
+    RefreshTokenResponseTypeDef,
+    FormSummaryTypeDef,
+    CreateThemeRequestRequestTypeDef,
+    CreateThemeResponseTypeDef,
+    ExportThemesResponseTypeDef,
+    GetThemeResponseTypeDef,
+    UpdateThemeResponseTypeDef,
+    ExchangeCodeForTokenRequestRequestTypeDef,
+    ExportComponentsRequestExportComponentsPaginateTypeDef,
+    ExportFormsRequestExportFormsPaginateTypeDef,
+    ExportThemesRequestExportThemesPaginateTypeDef,
+    ListCodegenJobsRequestListCodegenJobsPaginateTypeDef,
+    ListComponentsRequestListComponentsPaginateTypeDef,
+    ListFormsRequestListFormsPaginateTypeDef,
+    ListThemesRequestListThemesPaginateTypeDef,
+    FormButtonTypeDef,
+    SectionalElementTypeDef,
+    FormInputBindingPropertiesValueTypeDef,
+    FormInputValuePropertyTypeDef,
+    FormStyleTypeDef,
+    ListThemesResponseTypeDef,
+    PutMetadataFlagRequestRequestTypeDef,
+    RefreshTokenRequestRequestTypeDef,
+    UpdateThemeRequestRequestTypeDef,
+    ComponentEventOutputTypeDef,
+    ComponentEventTypeDef,
+    CodegenGenericDataModelOutputTypeDef,
+    CodegenGenericDataNonModelOutputTypeDef,
+    CodegenGenericDataModelTypeDef,
+    CodegenGenericDataNonModelTypeDef,
+    ListFormsResponseTypeDef,
+    FormCTATypeDef,
+    ValueMappingsOutputTypeDef,
+    ValueMappingsTypeDef,
+    ComponentChildOutputTypeDef,
+    ComponentTypeDef,
+    ComponentChildTypeDef,
+    CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
-    UpdateComponentRequestRequestTypeDef,
+    CodegenJobGenericDataSchemaOutputTypeDef,
+    CodegenJobGenericDataSchemaTypeDef,
+    FieldInputConfigOutputTypeDef,
+    FieldInputConfigTypeDef,
+    CreateComponentResponseTypeDef,
+    ExportComponentsResponseTypeDef,
+    GetComponentResponseTypeDef,
     UpdateComponentResponseTypeDef,
+    CreateComponentRequestRequestTypeDef,
+    UpdateComponentRequestRequestTypeDef,
+    CodegenJobTypeDef,
+    StartCodegenJobDataTypeDef,
+    FieldConfigOutputTypeDef,
+    FieldConfigTypeDef,
+    GetCodegenJobResponseTypeDef,
+    StartCodegenJobResponseTypeDef,
+    StartCodegenJobRequestRequestTypeDef,
+    FormTypeDef,
+    CreateFormDataTypeDef,
     UpdateFormDataTypeDef,
-    UpdateFormRequestRequestTypeDef,
+    CreateFormResponseTypeDef,
+    ExportFormsResponseTypeDef,
+    GetFormResponseTypeDef,
     UpdateFormResponseTypeDef,
-    UpdateThemeDataTypeDef,
-    UpdateThemeRequestRequestTypeDef,
-    UpdateThemeResponseTypeDef,
-    ValueMappingTypeDef,
-    ValueMappingsTypeDef,
+    CreateFormRequestRequestTypeDef,
+    UpdateFormRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActionParametersTypeDef:
+def get_value() -> MutationActionSetStateParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt` & `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

