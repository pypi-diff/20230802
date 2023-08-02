# Comparing `tmp/types-aiobotocore-application-insights-2.5.2.tar.gz` & `tmp/types-aiobotocore-application-insights-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-insights-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-insights-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-application-insights-2.5.2.tar` & `types-aiobotocore-application-insights-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.497692 types-aiobotocore-application-insights-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-08 01:43:14.497692 types-aiobotocore-application-insights-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.497692 types-aiobotocore-application-insights-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.497692 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22650 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19816 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19801 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:48.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.497692 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15191 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 01:43:14.000000 types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22619 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-insights-2.5.2/LICENSE` & `types-aiobotocore-application-insights-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2/PKG-INFO` & `types-aiobotocore-application-insights-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore application-insights type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore application-insights type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-insights"></a>
 
 # types-aiobotocore-application-insights
 
 [![PyPI - types-aiobotocore-application-insights](https://img.shields.io/pypi/v/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-insights?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
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
@@ -292,82 +291,84 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_insights.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    DescribeComponentResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_value() -> ApplicationComponentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2/README.md` & `types-aiobotocore-application-insights-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-application-insights"></a>
 
 # types-aiobotocore-application-insights
 
 [![PyPI - types-aiobotocore-application-insights](https://img.shields.io/pypi/v/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-insights?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
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
@@ -259,82 +259,84 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_insights.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    DescribeComponentResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_value() -> ApplicationComponentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2/setup.py` & `types-aiobotocore-application-insights-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-insights",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore application-insights type-annotations boto3-stubs mypy typeshed autocomplete"
+        "aiobotocore application-insights type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_application_insights": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/",
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__init__.py` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__init__.pyi` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/__main__.py` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationInsights 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/client.py` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("application-insights") as client:
         client: ApplicationInsightsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ConfigurationEventStatusType, TierType
 from .type_defs import (
     CreateApplicationResponseTypeDef,
@@ -37,14 +36,15 @@
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -293,16 +293,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
 
     async def list_configuration_history(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
@@ -336,16 +336,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
 
     async def list_problems(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/client.pyi` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("application-insights") as client:
         client: ApplicationInsightsClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ConfigurationEventStatusType, TierType
 from .type_defs import (
     CreateApplicationResponseTypeDef,
@@ -37,14 +36,15 @@
     ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
     ListLogPatternSetsResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     ListProblemsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
     UpdateApplicationResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -269,16 +269,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_components)
         """
     async def list_configuration_history(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         EventStatus: ConfigurationEventStatusType = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListConfigurationHistoryResponseTypeDef:
         """
         Lists the INFO, WARN, and ERROR events for periodic configuration updates
         performed by Application Insights.
@@ -309,16 +309,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights.Client.list_log_patterns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/client/#list_log_patterns)
         """
     async def list_problems(
         self,
         *,
         ResourceGroupName: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         ComponentName: str = ...
     ) -> ListProblemsResponseTypeDef:
         """
         Lists the problems with your application.
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/literals.py` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/literals.pyi` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/type_defs.py` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
 
-    data: ApplicationComponentTypeDef = {...}
+    data: ApplicationComponentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -39,64 +39,65 @@
 
 
 __all__ = (
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListConfigurationHistoryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
-    "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "DescribeComponentResponseTypeDef",
-    "ListComponentsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeComponentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "ListComponentsResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    "ListProblemsRequestRequestTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
@@ -142,14 +143,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
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
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -213,40 +225,22 @@
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
 
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
 
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
-    {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
@@ -379,27 +373,15 @@
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
     pass
 
 
-ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
-    "ListConfigurationHistoryRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": ConfigurationEventStatusType,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
@@ -415,24 +397,14 @@
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
-    {
-        "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
@@ -448,45 +420,21 @@
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
 
-ListProblemsRequestRequestTypeDef = TypedDict(
-    "ListProblemsRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ComponentName": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -585,147 +533,175 @@
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
 
-DescribeComponentResponseTypeDef = TypedDict(
-    "DescribeComponentResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
-        "ApplicationComponent": ApplicationComponentTypeDef,
-        "ResourceList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceGroupName": str,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentResponseTypeDef = TypedDict(
+    "DescribeComponentResponseTypeDef",
+    {
+        "ApplicationComponent": ApplicationComponentTypeDef,
+        "ResourceList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
     {
         "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -733,28 +709,54 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": ConfigurationEventStatusType,
+        "MaxResults": int,
+        "NextToken": str,
     },
+    total=False,
+)
+
+ListProblemsRequestRequestTypeDef = TypedDict(
+    "ListProblemsRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ComponentName": str,
+    },
+    total=False,
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights/type_defs.pyi` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_application_insights.type_defs import ApplicationComponentTypeDef
 
-    data: ApplicationComponentTypeDef = {...}
+    data: ApplicationComponentTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -38,64 +38,65 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationComponentTypeDef",
     "ApplicationInfoTypeDef",
     "ConfigurationEventTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "CreateLogPatternRequestRequestTypeDef",
     "LogPatternTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteLogPatternRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DescribeComponentConfigurationRecommendationRequestRequestTypeDef",
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
     "DescribeComponentConfigurationRequestRequestTypeDef",
-    "DescribeComponentConfigurationResponseTypeDef",
     "DescribeComponentRequestRequestTypeDef",
     "DescribeLogPatternRequestRequestTypeDef",
     "DescribeObservationRequestRequestTypeDef",
     "ObservationTypeDef",
     "DescribeProblemObservationsRequestRequestTypeDef",
     "DescribeProblemRequestRequestTypeDef",
     "ProblemTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
-    "ListConfigurationHistoryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ListLogPatternSetsRequestRequestTypeDef",
-    "ListLogPatternSetsResponseTypeDef",
     "ListLogPatternsRequestRequestTypeDef",
-    "ListProblemsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
     "UpdateComponentConfigurationRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "UpdateLogPatternRequestRequestTypeDef",
-    "DescribeComponentResponseTypeDef",
-    "ListComponentsResponseTypeDef",
+    "CreateApplicationRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "DescribeApplicationResponseTypeDef",
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    "DescribeComponentConfigurationResponseTypeDef",
+    "DescribeComponentResponseTypeDef",
     "ListApplicationsResponseTypeDef",
-    "UpdateApplicationResponseTypeDef",
+    "ListComponentsResponseTypeDef",
     "ListConfigurationHistoryResponseTypeDef",
-    "CreateApplicationRequestRequestTypeDef",
+    "ListLogPatternSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "UpdateApplicationResponseTypeDef",
     "CreateLogPatternResponseTypeDef",
     "DescribeLogPatternResponseTypeDef",
     "ListLogPatternsResponseTypeDef",
     "UpdateLogPatternResponseTypeDef",
     "DescribeObservationResponseTypeDef",
     "RelatedObservationsTypeDef",
     "DescribeProblemResponseTypeDef",
     "ListProblemsResponseTypeDef",
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    "ListProblemsRequestRequestTypeDef",
     "DescribeProblemObservationsResponseTypeDef",
 )
 
 ApplicationComponentTypeDef = TypedDict(
     "ApplicationComponentTypeDef",
     {
         "ComponentName": str,
@@ -141,14 +142,25 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
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
 CreateComponentRequestRequestTypeDef = TypedDict(
     "CreateComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "ResourceList": Sequence[str],
     },
@@ -212,40 +224,22 @@
     {
         "ResourceGroupName": str,
         "ComponentName": str,
         "Tier": TierType,
     },
 )
 
-DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationRecommendationResponseTypeDef",
-    {
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeComponentConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeComponentConfigurationRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
 
-DescribeComponentConfigurationResponseTypeDef = TypedDict(
-    "DescribeComponentConfigurationResponseTypeDef",
-    {
-        "Monitor": bool,
-        "Tier": TierType,
-        "ComponentConfiguration": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeComponentRequestRequestTypeDef = TypedDict(
     "DescribeComponentRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
         "ComponentName": str,
     },
 )
@@ -376,27 +370,15 @@
 )
 
 class ListComponentsRequestRequestTypeDef(
     _RequiredListComponentsRequestRequestTypeDef, _OptionalListComponentsRequestRequestTypeDef
 ):
     pass
 
-ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
-    "ListConfigurationHistoryRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "EventStatus": ConfigurationEventStatusType,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredListLogPatternSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternSetsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternSetsRequestRequestTypeDef = TypedDict(
@@ -410,24 +392,14 @@
 
 class ListLogPatternSetsRequestRequestTypeDef(
     _RequiredListLogPatternSetsRequestRequestTypeDef,
     _OptionalListLogPatternSetsRequestRequestTypeDef,
 ):
     pass
 
-ListLogPatternSetsResponseTypeDef = TypedDict(
-    "ListLogPatternSetsResponseTypeDef",
-    {
-        "ResourceGroupName": str,
-        "LogPatternSets": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListLogPatternsRequestRequestTypeDef = TypedDict(
     "_RequiredListLogPatternsRequestRequestTypeDef",
     {
         "ResourceGroupName": str,
     },
 )
 _OptionalListLogPatternsRequestRequestTypeDef = TypedDict(
@@ -441,45 +413,21 @@
 )
 
 class ListLogPatternsRequestRequestTypeDef(
     _RequiredListLogPatternsRequestRequestTypeDef, _OptionalListLogPatternsRequestRequestTypeDef
 ):
     pass
 
-ListProblemsRequestRequestTypeDef = TypedDict(
-    "ListProblemsRequestRequestTypeDef",
-    {
-        "ResourceGroupName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "MaxResults": int,
-        "NextToken": str,
-        "ComponentName": str,
-    },
-    total=False,
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -570,147 +518,175 @@
 )
 
 class UpdateLogPatternRequestRequestTypeDef(
     _RequiredUpdateLogPatternRequestRequestTypeDef, _OptionalUpdateLogPatternRequestRequestTypeDef
 ):
     pass
 
-DescribeComponentResponseTypeDef = TypedDict(
-    "DescribeComponentResponseTypeDef",
+CreateApplicationRequestRequestTypeDef = TypedDict(
+    "CreateApplicationRequestRequestTypeDef",
     {
-        "ApplicationComponent": ApplicationComponentTypeDef,
-        "ResourceList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceGroupName": str,
+        "OpsCenterEnabled": bool,
+        "CWEMonitorEnabled": bool,
+        "OpsItemSNSTopicArn": str,
+        "Tags": Sequence[TagTypeDef],
+        "AutoConfigEnabled": bool,
+        "AutoCreate": bool,
+        "GroupingType": Literal["ACCOUNT_BASED"],
     },
+    total=False,
 )
 
-ListComponentsResponseTypeDef = TypedDict(
-    "ListComponentsResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "ApplicationComponentList": List[ApplicationComponentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
     },
 )
 
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationRecommendationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationRecommendationResponseTypeDef",
+    {
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentConfigurationResponseTypeDef = TypedDict(
+    "DescribeComponentConfigurationResponseTypeDef",
+    {
+        "Monitor": bool,
+        "Tier": TierType,
+        "ComponentConfiguration": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeComponentResponseTypeDef = TypedDict(
+    "DescribeComponentResponseTypeDef",
+    {
+        "ApplicationComponent": ApplicationComponentTypeDef,
+        "ResourceList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationInfoList": List[ApplicationInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApplicationResponseTypeDef = TypedDict(
-    "UpdateApplicationResponseTypeDef",
+ListComponentsResponseTypeDef = TypedDict(
+    "ListComponentsResponseTypeDef",
     {
-        "ApplicationInfo": ApplicationInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ApplicationComponentList": List[ApplicationComponentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConfigurationHistoryResponseTypeDef = TypedDict(
     "ListConfigurationHistoryResponseTypeDef",
     {
         "EventList": List[ConfigurationEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApplicationRequestRequestTypeDef = TypedDict(
-    "CreateApplicationRequestRequestTypeDef",
+ListLogPatternSetsResponseTypeDef = TypedDict(
+    "ListLogPatternSetsResponseTypeDef",
     {
         "ResourceGroupName": str,
-        "OpsCenterEnabled": bool,
-        "CWEMonitorEnabled": bool,
-        "OpsItemSNSTopicArn": str,
-        "Tags": Sequence[TagTypeDef],
-        "AutoConfigEnabled": bool,
-        "AutoCreate": bool,
-        "GroupingType": Literal["ACCOUNT_BASED"],
+        "LogPatternSets": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+UpdateApplicationResponseTypeDef = TypedDict(
+    "UpdateApplicationResponseTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationInfo": ApplicationInfoTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLogPatternResponseTypeDef = TypedDict(
     "CreateLogPatternResponseTypeDef",
     {
         "LogPattern": LogPatternTypeDef,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeLogPatternResponseTypeDef = TypedDict(
     "DescribeLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLogPatternsResponseTypeDef = TypedDict(
     "ListLogPatternsResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPatterns": List[LogPatternTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLogPatternResponseTypeDef = TypedDict(
     "UpdateLogPatternResponseTypeDef",
     {
         "ResourceGroupName": str,
         "LogPattern": LogPatternTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObservationResponseTypeDef = TypedDict(
     "DescribeObservationResponseTypeDef",
     {
         "Observation": ObservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedObservationsTypeDef = TypedDict(
     "RelatedObservationsTypeDef",
     {
         "ObservationList": List[ObservationTypeDef],
@@ -718,28 +694,54 @@
     total=False,
 )
 
 DescribeProblemResponseTypeDef = TypedDict(
     "DescribeProblemResponseTypeDef",
     {
         "Problem": ProblemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProblemsResponseTypeDef = TypedDict(
     "ListProblemsResponseTypeDef",
     {
         "ProblemList": List[ProblemTypeDef],
         "NextToken": str,
         "ResourceGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationHistoryRequestRequestTypeDef = TypedDict(
+    "ListConfigurationHistoryRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "EventStatus": ConfigurationEventStatusType,
+        "MaxResults": int,
+        "NextToken": str,
     },
+    total=False,
+)
+
+ListProblemsRequestRequestTypeDef = TypedDict(
+    "ListProblemsRequestRequestTypeDef",
+    {
+        "ResourceGroupName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "MaxResults": int,
+        "NextToken": str,
+        "ComponentName": str,
+    },
+    total=False,
 )
 
 DescribeProblemObservationsResponseTypeDef = TypedDict(
     "DescribeProblemObservationsResponseTypeDef",
     {
         "RelatedObservations": RelatedObservationsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/PKG-INFO` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-insights
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore application-insights type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore application-insights type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-insights"></a>
 
 # types-aiobotocore-application-insights
 
 [![PyPI - types-aiobotocore-application-insights](https://img.shields.io/pypi/v/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-insights.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-insights)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-application-insights?color=blue)](https://pypistats.org/packages/types-aiobotocore-application-insights)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-application-insights)](https://pepy.tech/project/types-aiobotocore-application-insights)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationInsights 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights)
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
 [types-aiobotocore-application-insights docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights/).
 
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
@@ -292,82 +291,84 @@
 )
 
 
 def check_value(value: CloudWatchEventSourceType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_application_insights.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_application_insights.type_defs import (
     ApplicationComponentTypeDef,
     ApplicationInfoTypeDef,
     ConfigurationEventTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateComponentRequestRequestTypeDef,
     CreateLogPatternRequestRequestTypeDef,
     LogPatternTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DeleteComponentRequestRequestTypeDef,
     DeleteLogPatternRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DescribeComponentConfigurationRecommendationRequestRequestTypeDef,
-    DescribeComponentConfigurationRecommendationResponseTypeDef,
     DescribeComponentConfigurationRequestRequestTypeDef,
-    DescribeComponentConfigurationResponseTypeDef,
     DescribeComponentRequestRequestTypeDef,
     DescribeLogPatternRequestRequestTypeDef,
     DescribeObservationRequestRequestTypeDef,
     ObservationTypeDef,
     DescribeProblemObservationsRequestRequestTypeDef,
     DescribeProblemRequestRequestTypeDef,
     ProblemTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListComponentsRequestRequestTypeDef,
-    ListConfigurationHistoryRequestRequestTypeDef,
+    TimestampTypeDef,
     ListLogPatternSetsRequestRequestTypeDef,
-    ListLogPatternSetsResponseTypeDef,
     ListLogPatternsRequestRequestTypeDef,
-    ListProblemsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
     UpdateComponentConfigurationRequestRequestTypeDef,
     UpdateComponentRequestRequestTypeDef,
     UpdateLogPatternRequestRequestTypeDef,
-    DescribeComponentResponseTypeDef,
-    ListComponentsResponseTypeDef,
+    CreateApplicationRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     DescribeApplicationResponseTypeDef,
+    DescribeComponentConfigurationRecommendationResponseTypeDef,
+    DescribeComponentConfigurationResponseTypeDef,
+    DescribeComponentResponseTypeDef,
     ListApplicationsResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
+    ListComponentsResponseTypeDef,
     ListConfigurationHistoryResponseTypeDef,
-    CreateApplicationRequestRequestTypeDef,
+    ListLogPatternSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    UpdateApplicationResponseTypeDef,
     CreateLogPatternResponseTypeDef,
     DescribeLogPatternResponseTypeDef,
     ListLogPatternsResponseTypeDef,
     UpdateLogPatternResponseTypeDef,
     DescribeObservationResponseTypeDef,
     RelatedObservationsTypeDef,
     DescribeProblemResponseTypeDef,
     ListProblemsResponseTypeDef,
+    ListConfigurationHistoryRequestRequestTypeDef,
+    ListProblemsRequestRequestTypeDef,
     DescribeProblemObservationsResponseTypeDef,
 )
 
 
-def get_structure() -> ApplicationComponentTypeDef:
+def get_value() -> ApplicationComponentTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-application-insights-2.5.2/types_aiobotocore_application_insights.egg-info/SOURCES.txt` & `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

