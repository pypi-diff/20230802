# Comparing `tmp/aws_prototyping_sdk.cdk_graph-0.12.26.tar.gz` & `tmp/aws_prototyping_sdk.cdk_graph-0.19.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_prototyping_sdk.cdk_graph-0.12.26.tar", last modified: Fri Dec  9 05:16:39 2022, max compression
+gzip compressed data, was "aws_prototyping_sdk.cdk_graph-0.19.56.tar", last modified: Wed Aug  2 01:34:03 2023, max compression
```

## Comparing `aws_prototyping_sdk.cdk_graph-0.12.26.tar` & `aws_prototyping_sdk.cdk_graph-0.19.56.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.515100 aws_prototyping_sdk.cdk_graph-0.12.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.515100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/
--rw-r--r--   0 runner    (1001) docker     (123)    81066 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   170614 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.12.26.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/graph/
--rw-r--r--   0 runner    (1001) docker     (123)   164347 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/serialized_graph/
--rw-r--r--   0 runner    (1001) docker     (123)    34049 2022-12-09 05:16:15.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 05:16:39.531100 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2022-12-09 05:16:37.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-09 05:16:39.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 05:16:38.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-09 05:16:39.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-09 05:16:39.000000 aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.932910 aws_prototyping_sdk.cdk_graph-0.19.56/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.932910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    83028 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   626370 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.56.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)   193146 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.936910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/serialized_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    35320 2023-08-02 01:33:55.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:34:03.932910 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 2023-08-02 01:34:03.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 01:34:03.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:34:03.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 01:34:03.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 01:34:03.000000 aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/LICENSE` & `aws_prototyping_sdk.cdk_graph-0.19.56/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/PKG-INFO` & `aws_prototyping_sdk.cdk_graph-0.19.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aws_prototyping_sdk.cdk_graph
-Version: 0.12.26
+Version: 0.19.56
 Summary: @aws-prototyping-sdk/cdk-graph
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -280,9 +280,7 @@
 * [ ] Find alternative synthesis solution that doesn't utilize CDK internals
 * [ ] Support custom Nodes and Edges
 * [ ] Improve logging, bookkeeping, and debugging
 * [ ] Implement store upgrade solution
 * [ ] Battle test the implementation against several plugins
 * [ ] Battle test the implementation in all target languages (currently tested in Typescript, but vended in all PDK supported languages)
 * [ ] Receive community feedback to validate approach
-
-
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/README.md` & `aws_prototyping_sdk.cdk_graph-0.19.56/README.md`

 * *Files identical despite different names*

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/setup.py` & `aws_prototyping_sdk.cdk_graph-0.19.56/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws_prototyping_sdk.cdk_graph",
-    "version": "0.12.26",
+    "version": "0.19.56",
     "description": "@aws-prototyping-sdk/cdk-graph",
     "license": "Apache-2.0",
     "url": "https://github.com/aws/aws-prototyping-sdk",
     "long_description_content_type": "text/markdown",
     "author": "AWS APJ COPE<apj-cope@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -24,38 +24,39 @@
         "aws_prototyping_sdk.cdk_graph",
         "aws_prototyping_sdk.cdk_graph._jsii",
         "aws_prototyping_sdk.cdk_graph.graph",
         "aws_prototyping_sdk.cdk_graph.serialized_graph"
     ],
     "package_data": {
         "aws_prototyping_sdk.cdk_graph._jsii": [
-            "cdk-graph@0.12.26.jsii.tgz"
+            "cdk-graph@0.19.56.jsii.tgz"
         ],
         "aws_prototyping_sdk.cdk_graph": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib>=2.53.0, <3.0.0",
-        "constructs>=10.1.162, <11.0.0",
-        "jsii>=1.71.0, <2.0.0",
-        "projen>=0.65.26, <0.66.0",
+        "aws-cdk-lib>=2.81.0, <3.0.0",
+        "constructs>=10.2.39, <11.0.0",
+        "jsii>=1.82.0, <2.0.0",
+        "projen>=0.71.92, <0.72.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 4 - Beta",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -272,26 +272,23 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import constructs
+import constructs as _constructs_77d1e7e8
 from .graph import (
     IEdgePredicate as _IEdgePredicate_786afb09,
     INodePredicate as _INodePredicate_1dc8755a,
     Node as _Node_ddadac9d,
     Store as _Store_6b467276,
 )
 from .serialized_graph import (
-    Attributes as _Attributes_b47661e3,
-    Entity as _Entity_794b3e11,
-    PlainObject as _PlainObject_c976ebcc,
-    Tags as _Tags_cf30c388,
+    Entity as _Entity_794b3e11, PlainObject as _PlainObject_c976ebcc
 )
 
 
 @jsii.enum(jsii_type="@aws-prototyping-sdk/cdk-graph.CdkConstructIds")
 class CdkConstructIds(enum.Enum):
     '''(experimental) Common cdk construct ids.
 
@@ -309,41 +306,36 @@
     EXPORTS = "EXPORTS"
     '''
     :stability: experimental
     '''
 
 
 class CdkGraph(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/cdk-graph.CdkGraph",
 ):
     '''(experimental) CdkGraph construct is the cdk-graph framework controller that is responsible for computing the graph, storing serialized graph, and instrumenting plugins per the plugin contract.
 
     :stability: experimental
     '''
 
     def __init__(
         self,
-        root: constructs.Construct,
+        root: _constructs_77d1e7e8.Construct,
         props: typing.Optional["ICdkGraphProps"] = None,
     ) -> None:
         '''
         :param root: -
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                root: constructs.Construct,
-                props: typing.Optional[ICdkGraphProps] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__28286f53bba3c64713566007568503857222212a302b0e060ba6e0b0d67633d0)
             check_type(argname="argument root", value=root, expected_type=type_hints["root"])
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [root, props])
 
     @jsii.member(jsii_name="report")
     def report(self) -> None:
         '''(experimental) Asynchronous report generation. This operation enables running expensive and non-synchronous report generation by plugins post synthesis.
@@ -371,37 +363,37 @@
 
         :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.sget(cls, "VERSION"))
 
     @builtins.property
     @jsii.member(jsii_name="config")
-    def config(self) -> "CdkGraphConfig":
+    def config(self) -> typing.Mapping[builtins.str, typing.Any]:
         '''(experimental) Config.
 
         :stability: experimental
         '''
-        return typing.cast("CdkGraphConfig", jsii.get(self, "config"))
+        return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.get(self, "config"))
 
     @builtins.property
     @jsii.member(jsii_name="plugins")
     def plugins(self) -> typing.List["ICdkGraphPlugin"]:
         '''(experimental) List of plugins registered with this instance.
 
         :stability: experimental
         '''
         return typing.cast(typing.List["ICdkGraphPlugin"], jsii.get(self, "plugins"))
 
     @builtins.property
     @jsii.member(jsii_name="root")
-    def root(self) -> constructs.Construct:
+    def root(self) -> _constructs_77d1e7e8.Construct:
         '''
         :stability: experimental
         '''
-        return typing.cast(constructs.Construct, jsii.get(self, "root"))
+        return typing.cast(_constructs_77d1e7e8.Construct, jsii.get(self, "root"))
 
     @builtins.property
     @jsii.member(jsii_name="graphContext")
     def graph_context(self) -> typing.Optional["CdkGraphContext"]:
         '''(experimental) Get the context for the graph instance.
 
         This will be ``undefined`` before construct synthesis has initiated.
@@ -439,30 +431,21 @@
         :param id: (experimental) The unique type of the artifact.
         :param source: (experimental) The source of the artifact (such as plugin, or core system, etc).
         :param description: (experimental) Description of artifact.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                *,
-                filename: builtins.str,
-                filepath: builtins.str,
-                id: builtins.str,
-                source: builtins.str,
-                description: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__23a3bf1400984efa0d22219618f9f7c2b1b3cf1e07948dc134f293b4b7c2799d)
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
             check_type(argname="argument filepath", value=filepath, expected_type=type_hints["filepath"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "filename": filename,
             "filepath": filepath,
             "id": id,
             "source": source,
         }
         if description is not None:
             self._values["description"] = description
@@ -541,63 +524,14 @@
     '''
     GRAPH = "GRAPH"
     '''
     :stability: experimental
     '''
 
 
-@jsii.data_type(
-    jsii_type="@aws-prototyping-sdk/cdk-graph.CdkGraphConfig",
-    jsii_struct_bases=[],
-    name_mapping={"outdir": "outdir"},
-)
-class CdkGraphConfig:
-    def __init__(self, *, outdir: typing.Optional[builtins.str] = None) -> None:
-        '''(experimental) CdkGraph configuration definition.
-
-        :param outdir: (experimental) Directory where artifacts are written. The key ``<cdk.out>`` will be replaced with the synthesizer cdk ``outdir``. Relative paths not prefixed with ``<cdk.out>`` will be relative to ``process.cwd`` Default: "<cdk.out>/cdkgraph"
-
-        :stability: experimental
-        '''
-        if __debug__:
-            def stub(*, outdir: typing.Optional[builtins.str] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
-            check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
-        self._values: typing.Dict[str, typing.Any] = {}
-        if outdir is not None:
-            self._values["outdir"] = outdir
-
-    @builtins.property
-    def outdir(self) -> typing.Optional[builtins.str]:
-        '''(experimental) Directory where artifacts are written.
-
-        The key ``<cdk.out>`` will be replaced with the synthesizer cdk ``outdir``.
-
-        Relative paths not prefixed with ``<cdk.out>`` will be relative to ``process.cwd``
-
-        :default: "<cdk.out>/cdkgraph"
-
-        :stability: experimental
-        '''
-        result = self._values.get("outdir")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "CdkGraphConfig(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 class CdkGraphContext(
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/cdk-graph.CdkGraphContext",
 ):
     '''(experimental) CdkGraph context.
 
     :stability: experimental
@@ -607,49 +541,43 @@
         '''
         :param store: -
         :param outdir: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(store: _Store_6b467276, outdir: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__989da9e5b172457303b3aef4ed9ac17f179950db8e46d91724cfbd2bef74748c)
             check_type(argname="argument store", value=store, expected_type=type_hints["store"])
             check_type(argname="argument outdir", value=outdir, expected_type=type_hints["outdir"])
         jsii.create(self.__class__, self, [store, outdir])
 
     @jsii.member(jsii_name="getArtifact")
     def get_artifact(self, id: builtins.str) -> CdkGraphArtifact:
         '''(experimental) Get CdkGraph artifact by id.
 
         :param id: -
 
         :stability: experimental
         :throws: Error is artifact does not exist
         '''
         if __debug__:
-            def stub(id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__816d6f7e514bec099b526e77f33ac86bf42b1f7c17752bd722a51497ead76673)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         return typing.cast(CdkGraphArtifact, jsii.invoke(self, "getArtifact", [id]))
 
     @jsii.member(jsii_name="hasArtifactFile")
     def has_artifact_file(self, filename: builtins.str) -> builtins.bool:
         '''(experimental) Indicates if context has an artifact with *filename* defined.
 
         :param filename: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(filename: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a1a00986a437e5e797c994f6208b3c343e30d18bbaace95f147963e9d81cadaa)
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
         return typing.cast(builtins.bool, jsii.invoke(self, "hasArtifactFile", [filename]))
 
     @jsii.member(jsii_name="logArtifact")
     def log_artifact(
         self,
         source: typing.Union[CdkGraph, "ICdkGraphPlugin"],
@@ -668,22 +596,15 @@
         :param filepath: Full path where the artifact is stored.
         :param description: Description of the artifact.
 
         :stability: experimental
         :throws: Error is artifact id or filename already exists
         '''
         if __debug__:
-            def stub(
-                source: typing.Union[CdkGraph, ICdkGraphPlugin],
-                id: builtins.str,
-                filepath: builtins.str,
-                description: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a7076e52c64c67503ac32339aed9bc664c32f9a2ddb2e991c39310e6ef95f54e)
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument filepath", value=filepath, expected_type=type_hints["filepath"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         return typing.cast(CdkGraphArtifact, jsii.invoke(self, "logArtifact", [source, id, filepath, description]))
 
     @jsii.member(jsii_name="writeArtifact")
@@ -702,23 +623,15 @@
         :param filename: Relative name of the file.
         :param data: -
         :param description: Description of the artifact.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                source: typing.Union[CdkGraph, ICdkGraphPlugin],
-                id: builtins.str,
-                filename: builtins.str,
-                data: builtins.str,
-                description: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__46503812b23f70feadc9d32271563a9cd498878137bf496eb61bc3691922e6e9)
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
             check_type(argname="argument data", value=data, expected_type=type_hints["data"])
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
         return typing.cast(CdkGraphArtifact, jsii.invoke(self, "writeArtifact", [source, id, filename, data, description]))
 
@@ -786,20 +699,18 @@
         :param fqn: 
         :param version: 
 
         :see: https://github.com/aws/aws-cdk/blob/cea1039e3664fdfa89c6f00cdaeb1a0185a12678/packages/%40aws-cdk/core/lib/private/runtime-info.ts#L22
         :stability: experimental
         '''
         if __debug__:
-            def stub(*, fqn: builtins.str, version: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0075161e9afebef046d274d60dcc85233e4fdd2bc46a8916a19dd21ded5d2e1a)
             check_type(argname="argument fqn", value=fqn, expected_type=type_hints["fqn"])
             check_type(argname="argument version", value=version, expected_type=type_hints["version"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "fqn": fqn,
             "version": version,
         }
 
     @builtins.property
     def fqn(self) -> builtins.str:
         '''
@@ -837,14 +748,22 @@
     :stability: experimental
     '''
 
     APP = "APP"
     '''
     :stability: experimental
     '''
+    PDKAPP_MONO = "PDKAPP_MONO"
+    '''
+    :stability: experimental
+    '''
+    PDKAPP = "PDKAPP"
+    '''
+    :stability: experimental
+    '''
     STAGE = "STAGE"
     '''
     :stability: experimental
     '''
     STACK = "STACK"
     '''
     :stability: experimental
@@ -905,14 +824,26 @@
     '''
     :stability: experimental
     '''
     LAMBDA_BASE = "LAMBDA_BASE"
     '''
     :stability: experimental
     '''
+    LAMBDA_SINGLETON = "LAMBDA_SINGLETON"
+    '''
+    :stability: experimental
+    '''
+    LAMBDA_LAYER_AWSCLI = "LAMBDA_LAYER_AWSCLI"
+    '''
+    :stability: experimental
+    '''
+    CFN_LAMBDA_PERMISSIONS = "CFN_LAMBDA_PERMISSIONS"
+    '''
+    :stability: experimental
+    '''
     ASSET_STAGING = "ASSET_STAGING"
     '''
     :stability: experimental
     '''
     S3_ASSET = "S3_ASSET"
     '''
     :stability: experimental
@@ -957,14 +888,18 @@
     '''
     :stability: experimental
     '''
     CFN_PUBLIC_SUBNET = "CFN_PUBLIC_SUBNET"
     '''
     :stability: experimental
     '''
+    IAM_ROLE = "IAM_ROLE"
+    '''
+    :stability: experimental
+    '''
 
 
 @jsii.enum(jsii_type="@aws-prototyping-sdk/cdk-graph.EdgeDirectionEnum")
 class EdgeDirectionEnum(enum.Enum):
     '''(experimental) EdgeDirection specifies in which direction the edge is directed or if it is undirected.
 
     :stability: experimental
@@ -1034,14 +969,19 @@
     :stability: experimental
     '''
     NON_EXTRANEOUS = "NON_EXTRANEOUS"
     '''(experimental) Collapses extraneous nodes to parent and prunes extraneous edges.
 
     :stability: experimental
     '''
+    NONE = "NONE"
+    '''(experimental) No filtering is performed which will output **verbose** graph.
+
+    :stability: experimental
+    '''
 
 
 @jsii.enum(jsii_type="@aws-prototyping-sdk/cdk-graph.FilterStrategy")
 class FilterStrategy(enum.Enum):
     '''(experimental) Filter strategy to apply to filter matches.
 
     :stability: experimental
@@ -1086,28 +1026,27 @@
     :stability: experimental
     '''
     EXTRANEOUS = "EXTRANEOUS"
     '''(experimental) Indicates that the entity is extraneous and considered collapsible to parent without impact of intent.
 
     :stability: experimental
     '''
-    RESOURCE_WRAPPER = "RESOURCE_WRAPPER"
-    '''(experimental) Indicates node is a simple CfnResource wrapper and can be collapsed without change of intent;
-
-    Determined by only containing a single child of "Default" or "Resource"
-
-    :stability: experimental
-    '''
     ASSET = "ASSET"
     '''(experimental) Indicates node is considered a CDK Asset (Lambda Code, Docker Image, etc).
 
     :stability: experimental
     '''
     CDK_OWNED = "CDK_OWNED"
-    '''(experimental) Indicates that node was created by CDK (``construct.node.defaultChild === CfnResource``).
+    '''(experimental) Indicates that node was created by CDK.
+
+    :see: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Resource.html#static-iswbrownedwbrresourceconstruct
+    :stability: experimental
+    '''
+    CFN_FQN = "CFN_FQN"
+    '''(experimental) Indicates node ConstructInfoFqn denotes a ``aws-cdk-lib.*.Cfn*`` construct.
 
     :stability: experimental
     '''
     CLOSED_EDGE = "CLOSED_EDGE"
     '''(experimental) Indicates that edge is closed;
 
     meaning ``source === target``. This flag only gets applied on creation of edge, not during mutations to maintain initial intent.
@@ -1117,19 +1056,35 @@
     MUTATED = "MUTATED"
     '''(experimental) Indicates that entity was mutated;
 
     meaning a mutation was performed to change originally computed graph value.
 
     :stability: experimental
     '''
-    WRAPPED_CFN_RESOURCE = "WRAPPED_CFN_RESOURCE"
-    '''(experimental) Indicates that cfn resource has equivalent cdk resource wrapper.
+    IMPORT = "IMPORT"
+    '''(experimental) Indicates that resource is imported into CDK (eg: ``lambda.Function.fromFunctionName()``, ``s3.Bucket.fromBucketArn()``).
 
-    (eg: Lambda => CfnLambda)
+    :stability: experimental
+    '''
+    CUSTOM_RESOURCE = "CUSTOM_RESOURCE"
+    '''(experimental) Indicates if node is a CustomResource.
+
+    :see: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.custom_resources-readme.html
+    :stability: experimental
+    '''
+    AWS_CUSTOM_RESOURCE = "AWS_CUSTOM_RESOURCE"
+    '''(experimental) Indicates if node is an AwsCustomResource, which is a custom resource that simply calls the AWS SDK API via singleton provider.
+
+    :see: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.custom_resources.AwsCustomResource.html
+    :stability: experimental
+    '''
+    AWS_API_CALL_LAMBDA = "AWS_API_CALL_LAMBDA"
+    '''(experimental) Indicates if lambda function resource is a singleton AWS API call lambda for AwsCustomResources.
 
+    :see: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.custom_resources.AwsCustomResource.html
     :stability: experimental
     '''
 
 
 @jsii.interface(jsii_type="@aws-prototyping-sdk/cdk-graph.ICdkGraphPlugin")
 class ICdkGraphPlugin(typing_extensions.Protocol):
     '''(experimental) CdkGraph **Plugin** interface.
@@ -1274,17 +1229,15 @@
         :stability: experimental
         '''
         return typing.cast("IGraphPluginBindCallback", jsii.get(self, "bind"))
 
     @bind.setter
     def bind(self, value: "IGraphPluginBindCallback") -> None:
         if __debug__:
-            def stub(value: IGraphPluginBindCallback) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__54a2cc255662b5e0876e8d0db605a73b801eab0609f7115a372a87534496cb3e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "bind", value)
 
     @builtins.property
     @jsii.member(jsii_name="inspect")
     def inspect(self) -> typing.Optional["IGraphVisitorCallback"]:
         '''(experimental) Node visitor callback for construct tree traversal.
@@ -1295,17 +1248,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional["IGraphVisitorCallback"], jsii.get(self, "inspect"))
 
     @inspect.setter
     def inspect(self, value: typing.Optional["IGraphVisitorCallback"]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[IGraphVisitorCallback]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__22f4e280b8570ce4b34179d204a45f016fc59269a033e588b8034098b2fd8a72)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "inspect", value)
 
     @builtins.property
     @jsii.member(jsii_name="report")
     def report(self) -> typing.Optional["IGraphReportCallback"]:
         '''(experimental) Generate asynchronous reports based on the graph.
@@ -1318,17 +1269,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional["IGraphReportCallback"], jsii.get(self, "report"))
 
     @report.setter
     def report(self, value: typing.Optional["IGraphReportCallback"]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[IGraphReportCallback]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__dc2ff5d90cebb53054076da0d81c370dce67943e3aa06c8a1acd6778dc66ded6)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "report", value)
 
     @builtins.property
     @jsii.member(jsii_name="synthesize")
     def synthesize(self) -> typing.Optional["IGraphSynthesizeCallback"]:
         '''(experimental) Called during CDK synthesize to generate synchronous artifacts based on the in-memory graph passed to the plugin.
@@ -1338,17 +1287,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional["IGraphSynthesizeCallback"], jsii.get(self, "synthesize"))
 
     @synthesize.setter
     def synthesize(self, value: typing.Optional["IGraphSynthesizeCallback"]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[IGraphSynthesizeCallback]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__6f284eaa765a86f8c6ceacf14f7621e610187a734600a8597ddf791545b56252)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "synthesize", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ICdkGraphPlugin).__jsii_proxy_class__ = lambda : _ICdkGraphPluginProxy
 
 
@@ -1393,51 +1340,22 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional[typing.List[ICdkGraphPlugin]], jsii.get(self, "plugins"))
 
     @plugins.setter
     def plugins(self, value: typing.Optional[typing.List[ICdkGraphPlugin]]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[typing.List[ICdkGraphPlugin]]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__f1d86fc532537a4c1bac00c94df2e3ff0525196089cba42fa07b1dd256e10727)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "plugins", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ICdkGraphProps).__jsii_proxy_class__ = lambda : _ICdkGraphPropsProxy
 
 
-@jsii.interface(jsii_type="@aws-prototyping-sdk/cdk-graph.ICounterRecord")
-class ICounterRecord(typing_extensions.Protocol):
-    '''(experimental) ICounterRecord is record of keyed counts from {@link Counters}.
-
-    The record is a mapping of ``key => count`` values.
-
-    :stability: experimental
-    '''
-
-    pass
-
-
-class _ICounterRecordProxy:
-    '''(experimental) ICounterRecord is record of keyed counts from {@link Counters}.
-
-    The record is a mapping of ``key => count`` values.
-
-    :stability: experimental
-    '''
-
-    __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.ICounterRecord"
-    pass
-
-# Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
-typing.cast(typing.Any, ICounterRecord).__jsii_proxy_class__ = lambda : _ICounterRecordProxy
-
-
 @jsii.interface(jsii_type="@aws-prototyping-sdk/cdk-graph.IFilterFocusCallback")
 class IFilterFocusCallback(typing_extensions.Protocol):
     '''(experimental) Determines focus node of filter plan.
 
     :stability: experimental
     '''
 
@@ -1647,15 +1565,15 @@
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order to visit nodes and edges during filtering.
 
         :default: {ConstructOrder.PREORDER}
 
         :stability: experimental
         '''
         ...
@@ -1717,22 +1635,22 @@
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[typing.Union[_Node_ddadac9d, IFilterFocusCallback, "IGraphFilterPlanFocusConfig"]], jsii.get(self, "focus"))
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order to visit nodes and edges during filtering.
 
         :default: {ConstructOrder.PREORDER}
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[constructs.ConstructOrder], jsii.get(self, "order"))
+        return typing.cast(typing.Optional[_constructs_77d1e7e8.ConstructOrder], jsii.get(self, "order"))
 
     @builtins.property
     @jsii.member(jsii_name="preset")
     def preset(self) -> typing.Optional[FilterPreset]:
         '''(experimental) Optional preset filter to apply before other filters.
 
         :stability: experimental
@@ -1939,22 +1857,22 @@
     },
 )
 class InferredNodeProps(_Entity_794b3e11):
     def __init__(
         self,
         *,
         uuid: builtins.str,
-        attributes: typing.Optional[typing.Union[_Attributes_b47661e3, typing.Dict[str, typing.Any]]] = None,
+        attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]]]]]]] = None,
         flags: typing.Optional[typing.Sequence[FlagEnum]] = None,
-        metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-        tags: typing.Optional[typing.Union[_Tags_cf30c388, typing.Dict[str, typing.Any]]] = None,
+        metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         dependencies: typing.Sequence[builtins.str],
-        unresolved_references: typing.Sequence[typing.Union["UnresolvedReference", typing.Dict[str, typing.Any]]],
+        unresolved_references: typing.Sequence[typing.Union["UnresolvedReference", typing.Dict[builtins.str, typing.Any]]],
         cfn_type: typing.Optional[builtins.str] = None,
-        construct_info: typing.Optional[typing.Union[ConstructInfo, typing.Dict[str, typing.Any]]] = None,
+        construct_info: typing.Optional[typing.Union[ConstructInfo, typing.Dict[builtins.str, typing.Any]]] = None,
         logical_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Inferred node props.
 
         :param uuid: (experimental) Universally unique identity.
         :param attributes: (experimental) Serializable entity attributes.
         :param flags: (experimental) Serializable entity flags.
@@ -1964,47 +1882,29 @@
         :param unresolved_references: 
         :param cfn_type: 
         :param construct_info: 
         :param logical_id: 
 
         :stability: experimental
         '''
-        if isinstance(attributes, dict):
-            attributes = _Attributes_b47661e3(**attributes)
-        if isinstance(tags, dict):
-            tags = _Tags_cf30c388(**tags)
         if isinstance(construct_info, dict):
             construct_info = ConstructInfo(**construct_info)
         if __debug__:
-            def stub(
-                *,
-                uuid: builtins.str,
-                attributes: typing.Optional[typing.Union[_Attributes_b47661e3, typing.Dict[str, typing.Any]]] = None,
-                flags: typing.Optional[typing.Sequence[FlagEnum]] = None,
-                metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-                tags: typing.Optional[typing.Union[_Tags_cf30c388, typing.Dict[str, typing.Any]]] = None,
-                dependencies: typing.Sequence[builtins.str],
-                unresolved_references: typing.Sequence[typing.Union[UnresolvedReference, typing.Dict[str, typing.Any]]],
-                cfn_type: typing.Optional[builtins.str] = None,
-                construct_info: typing.Optional[typing.Union[ConstructInfo, typing.Dict[str, typing.Any]]] = None,
-                logical_id: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__bc702434f9098ad5400a36b4d5fa85826622b6657d1dd0f3392de0bcab361f2c)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
             check_type(argname="argument attributes", value=attributes, expected_type=type_hints["attributes"])
             check_type(argname="argument flags", value=flags, expected_type=type_hints["flags"])
             check_type(argname="argument metadata", value=metadata, expected_type=type_hints["metadata"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument dependencies", value=dependencies, expected_type=type_hints["dependencies"])
             check_type(argname="argument unresolved_references", value=unresolved_references, expected_type=type_hints["unresolved_references"])
             check_type(argname="argument cfn_type", value=cfn_type, expected_type=type_hints["cfn_type"])
             check_type(argname="argument construct_info", value=construct_info, expected_type=type_hints["construct_info"])
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "uuid": uuid,
             "dependencies": dependencies,
             "unresolved_references": unresolved_references,
         }
         if attributes is not None:
             self._values["attributes"] = attributes
         if flags is not None:
@@ -2027,52 +1927,56 @@
         :stability: experimental
         '''
         result = self._values.get("uuid")
         assert result is not None, "Required property 'uuid' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def attributes(self) -> typing.Optional[_Attributes_b47661e3]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]]:
         '''(experimental) Serializable entity attributes.
 
-        :see: {@link Attributes}
+        :see: {@link Attributes }
         :stability: experimental
         '''
         result = self._values.get("attributes")
-        return typing.cast(typing.Optional[_Attributes_b47661e3], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]], result)
 
     @builtins.property
     def flags(self) -> typing.Optional[typing.List[FlagEnum]]:
         '''(experimental) Serializable entity flags.
 
-        :see: {@link FlagEnum}
+        :see: {@link FlagEnum }
         :stability: experimental
         '''
         result = self._values.get("flags")
         return typing.cast(typing.Optional[typing.List[FlagEnum]], result)
 
     @builtins.property
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Serializable entity metadata.
 
-        :see: {@link Metadata}
+        :see: {@link Metadata }
         :stability: experimental
         '''
         result = self._values.get("metadata")
-        return typing.cast(typing.Optional[typing.List[constructs.MetadataEntry]], result)
+        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]], result)
 
     @builtins.property
-    def tags(self) -> typing.Optional[_Tags_cf30c388]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Serializable entity tags.
 
-        :see: {@link Tags}
+        :see: {@link Tags }
         :stability: experimental
         '''
         result = self._values.get("tags")
-        return typing.cast(typing.Optional[_Tags_cf30c388], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def dependencies(self) -> typing.List[builtins.str]:
         '''
         :stability: experimental
         '''
         result = self._values.get("dependencies")
@@ -2224,14 +2128,19 @@
     :stability: experimental
     '''
     IMPORT = "IMPORT"
     '''(experimental) CloudFormation **Fn::ImportValue** reference.
 
     :stability: experimental
     '''
+    IMPORT_ARN = "IMPORT_ARN"
+    '''(experimental) CloudFormation **Fn::Join** reference of imported resourced (eg: ``s3.Bucket.fromBucketArn()``).
+
+    :stability: experimental
+    '''
 
 
 @jsii.data_type(
     jsii_type="@aws-prototyping-sdk/cdk-graph.UnresolvedReference",
     jsii_struct_bases=[],
     name_mapping={
         "reference_type": "referenceType",
@@ -2243,42 +2152,34 @@
 class UnresolvedReference:
     def __init__(
         self,
         *,
         reference_type: ReferenceTypeEnum,
         source: builtins.str,
         target: builtins.str,
-        value: typing.Optional[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[str, typing.Any]]]]]] = None,
+        value: typing.Optional[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]]]]]] = None,
     ) -> None:
         '''(experimental) Unresolved reference struct.
 
         During graph computation references are unresolved and stored in this struct.
 
         :param reference_type: 
         :param source: 
         :param target: 
         :param value: 
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                *,
-                reference_type: ReferenceTypeEnum,
-                source: builtins.str,
-                target: builtins.str,
-                value: typing.Optional[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[str, typing.Any]]]]]] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__22a96afbb679347fbf4941ecc53f62384c0e5f8327f8d5820451a63d0890f0ea)
             check_type(argname="argument reference_type", value=reference_type, expected_type=type_hints["reference_type"])
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "reference_type": reference_type,
             "source": source,
             "target": target,
         }
         if value is not None:
             self._values["value"] = value
 
@@ -2332,27 +2233,25 @@
 
 
 __all__ = [
     "CdkConstructIds",
     "CdkGraph",
     "CdkGraphArtifact",
     "CdkGraphArtifacts",
-    "CdkGraphConfig",
     "CdkGraphContext",
     "CfnAttributesEnum",
     "ConstructInfo",
     "ConstructInfoFqnEnum",
     "EdgeDirectionEnum",
     "EdgeTypeEnum",
     "FilterPreset",
     "FilterStrategy",
     "FlagEnum",
     "ICdkGraphPlugin",
     "ICdkGraphProps",
-    "ICounterRecord",
     "IFilterFocusCallback",
     "IGraphFilter",
     "IGraphFilterPlan",
     "IGraphFilterPlanFocusConfig",
     "IGraphPluginBindCallback",
     "IGraphReportCallback",
     "IGraphStoreFilter",
@@ -2368,7 +2267,127 @@
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
 from . import graph
 from . import serialized_graph
+
+def _typecheckingstub__28286f53bba3c64713566007568503857222212a302b0e060ba6e0b0d67633d0(
+    root: _constructs_77d1e7e8.Construct,
+    props: typing.Optional[ICdkGraphProps] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__23a3bf1400984efa0d22219618f9f7c2b1b3cf1e07948dc134f293b4b7c2799d(
+    *,
+    filename: builtins.str,
+    filepath: builtins.str,
+    id: builtins.str,
+    source: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__989da9e5b172457303b3aef4ed9ac17f179950db8e46d91724cfbd2bef74748c(
+    store: _Store_6b467276,
+    outdir: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__816d6f7e514bec099b526e77f33ac86bf42b1f7c17752bd722a51497ead76673(
+    id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a1a00986a437e5e797c994f6208b3c343e30d18bbaace95f147963e9d81cadaa(
+    filename: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a7076e52c64c67503ac32339aed9bc664c32f9a2ddb2e991c39310e6ef95f54e(
+    source: typing.Union[CdkGraph, ICdkGraphPlugin],
+    id: builtins.str,
+    filepath: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__46503812b23f70feadc9d32271563a9cd498878137bf496eb61bc3691922e6e9(
+    source: typing.Union[CdkGraph, ICdkGraphPlugin],
+    id: builtins.str,
+    filename: builtins.str,
+    data: builtins.str,
+    description: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0075161e9afebef046d274d60dcc85233e4fdd2bc46a8916a19dd21ded5d2e1a(
+    *,
+    fqn: builtins.str,
+    version: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__54a2cc255662b5e0876e8d0db605a73b801eab0609f7115a372a87534496cb3e(
+    value: IGraphPluginBindCallback,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__22f4e280b8570ce4b34179d204a45f016fc59269a033e588b8034098b2fd8a72(
+    value: typing.Optional[IGraphVisitorCallback],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dc2ff5d90cebb53054076da0d81c370dce67943e3aa06c8a1acd6778dc66ded6(
+    value: typing.Optional[IGraphReportCallback],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6f284eaa765a86f8c6ceacf14f7621e610187a734600a8597ddf791545b56252(
+    value: typing.Optional[IGraphSynthesizeCallback],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f1d86fc532537a4c1bac00c94df2e3ff0525196089cba42fa07b1dd256e10727(
+    value: typing.Optional[typing.List[ICdkGraphPlugin]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bc702434f9098ad5400a36b4d5fa85826622b6657d1dd0f3392de0bcab361f2c(
+    *,
+    uuid: builtins.str,
+    attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]]]]]]] = None,
+    flags: typing.Optional[typing.Sequence[FlagEnum]] = None,
+    metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    dependencies: typing.Sequence[builtins.str],
+    unresolved_references: typing.Sequence[typing.Union[UnresolvedReference, typing.Dict[builtins.str, typing.Any]]],
+    cfn_type: typing.Optional[builtins.str] = None,
+    construct_info: typing.Optional[typing.Union[ConstructInfo, typing.Dict[builtins.str, typing.Any]]] = None,
+    logical_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__22a96afbb679347fbf4941ecc53f62384c0e5f8327f8d5820451a63d0890f0ea(
+    *,
+    reference_type: ReferenceTypeEnum,
+    source: builtins.str,
+    target: builtins.str,
+    value: typing.Optional[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[_PlainObject_c976ebcc, typing.Dict[builtins.str, typing.Any]]]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/graph/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,35 +8,32 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from .._jsii import *
 
-import constructs
+import constructs as _constructs_77d1e7e8
 from .. import (
     ConstructInfo as _ConstructInfo_e912d4bb,
     EdgeDirectionEnum as _EdgeDirectionEnum_26ef4ba3,
     EdgeTypeEnum as _EdgeTypeEnum_1b13d7ee,
     FlagEnum as _FlagEnum_af90e158,
-    ICounterRecord as _ICounterRecord_97e6658c,
     NodeTypeEnum as _NodeTypeEnum_d56eed04,
     ReferenceTypeEnum as _ReferenceTypeEnum_f84a272a,
 )
 from ..serialized_graph import (
-    Attributes as _Attributes_b47661e3,
     Edge as _Edge_211392d6,
     GraphStore as _GraphStore_ffbd5720,
     ISerializableEdge as _ISerializableEdge_afcbbd54,
     ISerializableEntity as _ISerializableEntity_0dbfd411,
     ISerializableGraphStore as _ISerializableGraphStore_4640156f,
     ISerializableNode as _ISerializableNode_9eb400fa,
     Node as _Node_bc073df3,
     PlainObject as _PlainObject_c976ebcc,
-    Tags as _Tags_cf30c388,
 )
 
 
 class AppNode(
     Node,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/cdk-graph.Graph.AppNode",
@@ -49,33 +46,29 @@
     def __init__(self, props: "IAppNodeProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IAppNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0ea8733837e9bb40c0c1ec64c6feb23f2ed1eb8273206106202412f46230febc)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isAppNode")
     @builtins.classmethod
     def is_app_node(cls, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if node is a {@link AppNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__bc02148277079718cf5c2f39c016f5b52c973f922c600de573dfe478f1099ea8)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isAppNode", [node]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="PATH")
     def PATH(cls) -> builtins.str:
         '''(experimental) Fixed path of the App.
@@ -107,33 +100,29 @@
     def __init__(self, props: "IAttributeReferenceProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IAttributeReferenceProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4c00aba2e4c442b0b145e9d63dacde89d6cad17d0bca8108c310f8b64e92b4be)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isAtt")
     @builtins.classmethod
     def is_att(cls, edge: "Edge") -> builtins.bool:
         '''(experimental) Indicates if edge in an **Fn::GetAtt** {@link Reference}.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4bafcead49197db174341aefc0d5b06356f41cc6ec4cabc8fac26198d34a7c77)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isAtt", [edge]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ATT_VALUE")
     def ATT_VALUE(cls) -> builtins.str:
         '''(experimental) Attribute key for resolved value of attribute reference.
@@ -174,66 +163,58 @@
     def __init__(self, props: "IBaseEntityProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IBaseEntityProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__cd84a9b7a0cf09d1574c06e6f4d90abcb54ce21eb50a1ddbdfff201bfbc29b91)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="addAttribute")
     def add_attribute(self, key: builtins.str, value: typing.Any) -> None:
         '''(experimental) Add attribute.
 
         :param key: -
         :param value: -
 
         :stability: experimental
         :throws: Error if attribute for key already exists
         '''
         if __debug__:
-            def stub(key: builtins.str, value: typing.Any) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__913d0433bc5941f0e59ee1edd8c046080f32987b0ab6c5e19bc266fe027bf146)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "addAttribute", [key, value]))
 
     @jsii.member(jsii_name="addFlag")
     def add_flag(self, flag: _FlagEnum_af90e158) -> None:
         '''(experimental) Add flag.
 
         :param flag: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(flag: _FlagEnum_af90e158) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__033b704f8a3c2f15a71de50e0db70b6f64c4b7e621236182d7afa37d2d368613)
             check_type(argname="argument flag", value=flag, expected_type=type_hints["flag"])
         return typing.cast(None, jsii.invoke(self, "addFlag", [flag]))
 
     @jsii.member(jsii_name="addMetadata")
     def add_metadata(self, metadata_type: builtins.str, data: typing.Any) -> None:
         '''(experimental) Add metadata entry.
 
         :param metadata_type: -
         :param data: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(metadata_type: builtins.str, data: typing.Any) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__cd7e4b19c50d04193a5603d24e18130fd0ce75cc5f857918800659670b7b1f2a)
             check_type(argname="argument metadata_type", value=metadata_type, expected_type=type_hints["metadata_type"])
             check_type(argname="argument data", value=data, expected_type=type_hints["data"])
         return typing.cast(None, jsii.invoke(self, "addMetadata", [metadata_type, data]))
 
     @jsii.member(jsii_name="addTag")
     def add_tag(self, key: builtins.str, value: builtins.str) -> None:
         '''(experimental) Add tag.
@@ -241,17 +222,15 @@
         :param key: -
         :param value: -
 
         :stability: experimental
         :throws: Throws Error is tag for key already exists
         '''
         if __debug__:
-            def stub(key: builtins.str, value: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__144a4bdde601cb81c22f5fbfce2338b613a871b555081164aa45293a33462c97)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "addTag", [key, value]))
 
     @jsii.member(jsii_name="applyData")
     def apply_data(
         self,
@@ -266,72 +245,60 @@
         :param data: - The data to apply.
         :param overwrite: -
         :param apply_flags: - Indicates if data is overwritten - Indicates if flags should be applied.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                data: IBaseEntityDataProps,
-                overwrite: typing.Optional[builtins.bool] = None,
-                apply_flags: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__04a459899bd329d2e4da70421ba17a31f77418a63fdc6bd5f9f961a28646d657)
             check_type(argname="argument data", value=data, expected_type=type_hints["data"])
             check_type(argname="argument overwrite", value=overwrite, expected_type=type_hints["overwrite"])
             check_type(argname="argument apply_flags", value=apply_flags, expected_type=type_hints["apply_flags"])
         return typing.cast(None, jsii.invoke(self, "applyData", [data, overwrite, apply_flags]))
 
     @jsii.member(jsii_name="findMetadata")
     def find_metadata(
         self,
         metadata_type: builtins.str,
-    ) -> typing.List[constructs.MetadataEntry]:
+    ) -> typing.List[_constructs_77d1e7e8.MetadataEntry]:
         '''(experimental) Retrieves all metadata entries of a given type.
 
         :param metadata_type: -
 
         :stability: experimental
         :type: Readonly<SerializedGraph.Metadata>
         '''
         if __debug__:
-            def stub(metadata_type: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c0d83a5d6b8bda51859f759127513a969f1857e948919d6ddb6d356a8f0f4f83)
             check_type(argname="argument metadata_type", value=metadata_type, expected_type=type_hints["metadata_type"])
-        return typing.cast(typing.List[constructs.MetadataEntry], jsii.invoke(self, "findMetadata", [metadata_type]))
+        return typing.cast(typing.List[_constructs_77d1e7e8.MetadataEntry], jsii.invoke(self, "findMetadata", [metadata_type]))
 
     @jsii.member(jsii_name="getAttribute")
     def get_attribute(self, key: builtins.str) -> typing.Any:
         '''(experimental) Get attribute by key.
 
         :param key: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3834b50954aaca507835cac1f164e2d1138952543da9236359ef21d6ab4d98ef)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast(typing.Any, jsii.invoke(self, "getAttribute", [key]))
 
     @jsii.member(jsii_name="getTag")
     def get_tag(self, key: builtins.str) -> typing.Optional[builtins.str]:
         '''(experimental) Get tag by key.
 
         :param key: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__1363a79f63c40b917b308f8b4729b20d5f6487075463e75700b9635b24564164)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast(typing.Optional[builtins.str], jsii.invoke(self, "getTag", [key]))
 
     @jsii.member(jsii_name="hasAttribute")
     def has_attribute(
         self,
         key: builtins.str,
@@ -341,33 +308,29 @@
 
         :param key: -
         :param value: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str, value: typing.Any = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__64b3d7ba1056459f4e688ea0a44d03ec6261908f53a39f49b0f2efdf5bdad6d5)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(builtins.bool, jsii.invoke(self, "hasAttribute", [key, value]))
 
     @jsii.member(jsii_name="hasFlag")
     def has_flag(self, flag: _FlagEnum_af90e158) -> builtins.bool:
         '''(experimental) Indicates if entity has a given flag.
 
         :param flag: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(flag: _FlagEnum_af90e158) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__39e58d1c8b02a0e3dff78d26530288d9f6ccc04c3ec96cef394e1975b1572b1a)
             check_type(argname="argument flag", value=flag, expected_type=type_hints["flag"])
         return typing.cast(builtins.bool, jsii.invoke(self, "hasFlag", [flag]))
 
     @jsii.member(jsii_name="hasMetadata")
     def has_metadata(
         self,
         metadata_type: builtins.str,
@@ -377,17 +340,15 @@
 
         :param metadata_type: -
         :param data: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(metadata_type: builtins.str, data: typing.Any) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4928bedd38550599d6ca3f869e7168cd1f62e843c4be593ef78a6937899eda16)
             check_type(argname="argument metadata_type", value=metadata_type, expected_type=type_hints["metadata_type"])
             check_type(argname="argument data", value=data, expected_type=type_hints["data"])
         return typing.cast(builtins.bool, jsii.invoke(self, "hasMetadata", [metadata_type, data]))
 
     @jsii.member(jsii_name="hasTag")
     def has_tag(
         self,
@@ -398,20 +359,15 @@
 
         :param key: -
         :param value: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                key: builtins.str,
-                value: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ddcfff79d83e7452bec9439ed35aca725ab7baaac4652a3f897fc3b7f0300ee2)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(builtins.bool, jsii.invoke(self, "hasTag", [key, value]))
 
     @jsii.member(jsii_name="mutateDestroy")
     @abc.abstractmethod
     def mutate_destroy(self, strict: typing.Optional[builtins.bool] = None) -> None:
@@ -432,17 +388,15 @@
 
         :param key: -
         :param value: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str, value: typing.Any) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__df8536147c5294b85dcf0b4564016e283be874d48b901226622ed863f48d99fc)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "setAttribute", [key, value]))
 
     @jsii.member(jsii_name="setTag")
     def set_tag(self, key: builtins.str, value: builtins.str) -> None:
         '''(experimental) Set tag.
@@ -451,30 +405,30 @@
 
         :param key: -
         :param value: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str, value: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a8e3c2cf27179bb2c32917aa8a4cdc4f81bb829323dfae17b926d2d78030ec15)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "setTag", [key, value]))
 
     @builtins.property
     @jsii.member(jsii_name="attributes")
-    def attributes(self) -> _Attributes_b47661e3:
+    def attributes(
+        self,
+    ) -> typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]:
         '''(experimental) Get *readonly* record of all attributes.
 
         :stability: experimental
         :type: Readonly<SerializedGraph.Attributes>
         '''
-        return typing.cast(_Attributes_b47661e3, jsii.get(self, "attributes"))
+        return typing.cast(typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]], jsii.get(self, "attributes"))
 
     @builtins.property
     @jsii.member(jsii_name="flags")
     def flags(self) -> typing.List[_FlagEnum_af90e158]:
         '''(experimental) Get *readonly* list of all flags.
 
         :stability: experimental
@@ -498,40 +452,40 @@
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isMutated"))
 
     @builtins.property
     @jsii.member(jsii_name="metadata")
-    def metadata(self) -> typing.List[constructs.MetadataEntry]:
+    def metadata(self) -> typing.List[_constructs_77d1e7e8.MetadataEntry]:
         '''(experimental) Get *readonly* list of all metadata entries.
 
         :stability: experimental
         :type: Readonly<SerializedGraph.Metadata>
         '''
-        return typing.cast(typing.List[constructs.MetadataEntry], jsii.get(self, "metadata"))
+        return typing.cast(typing.List[_constructs_77d1e7e8.MetadataEntry], jsii.get(self, "metadata"))
 
     @builtins.property
     @jsii.member(jsii_name="store")
     def store(self) -> "Store":
         '''(experimental) Reference to the store.
 
         :stability: experimental
         '''
         return typing.cast("Store", jsii.get(self, "store"))
 
     @builtins.property
     @jsii.member(jsii_name="tags")
-    def tags(self) -> _Tags_cf30c388:
+    def tags(self) -> typing.Mapping[builtins.str, builtins.str]:
         '''(experimental) Get *readonly* record of all tags.
 
         :stability: experimental
         :type: Readonly<SerializedGraph.Tags>
         '''
-        return typing.cast(_Tags_cf30c388, jsii.get(self, "tags"))
+        return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.get(self, "tags"))
 
     @builtins.property
     @jsii.member(jsii_name="uuid")
     def uuid(self) -> builtins.str:
         '''(experimental) Universally unique identifier.
 
         :stability: experimental
@@ -546,17 +500,15 @@
 
         :param strict: - If ``strict``, then entity must not have any references remaining when attempting to destroy.
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ba4fd8a0a02bae9f886b47c9eb0f948c4d98d60935d19cd5ca6a568b276ce4fb)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the abstract class
 typing.cast(typing.Any, BaseEntity).__jsii_proxy_class__ = lambda : _BaseEntityProxy
 
 
@@ -573,44 +525,32 @@
     def __init__(self, props: "ICfnResourceNodeProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: ICfnResourceNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e911cbd53a062053f329bf8f21a964493c96016d01a786631899820c452ab446)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isCfnResourceNode")
     @builtins.classmethod
     def is_cfn_resource_node(cls, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if a node is a {@link CfnResourceNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4d16082b017b42d002eb6b446987841f2b7bac243a65193dedb18a6561c2a89f)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isCfnResourceNode", [node]))
 
-    @jsii.member(jsii_name="findNearestResource")
-    def find_nearest_resource(self) -> typing.Optional["ResourceNode"]:
-        '''(experimental) Finds the near *ancestor* that is a {@link ResourceNode}.
-
-        :stability: experimental
-        '''
-        return typing.cast(typing.Optional["ResourceNode"], jsii.invoke(self, "findNearestResource", []))
-
     @jsii.member(jsii_name="isEquivalentFqn")
     def is_equivalent_fqn(self, resource: "ResourceNode") -> builtins.bool:
         '''(experimental) Evaluates if CfnResourceNode fqn is equivalent to ResourceNode fqn.
 
         :param resource: - {@link Graph.ResourceNode} to compare.
 
         :return: Returns ``true`` if equivalent, otherwise ``false``
@@ -618,36 +558,69 @@
         :stability: experimental
 
         Example::
 
             `aws-cdk-lib.aws_lambda.Function` => `aws-cdk-lib.aws_lambda.CfnFunction`
         '''
         if __debug__:
-            def stub(resource: ResourceNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a3bd9dbf3af183f7178d5e6bfbc05cb2eb158af66809077e88ac2843e729c088)
             check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
         return typing.cast(builtins.bool, jsii.invoke(self, "isEquivalentFqn", [resource]))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, strict: typing.Optional[builtins.bool] = None) -> None:
         '''(experimental) Destroys this node by removing all references and removing this node from the store.
 
         :param strict: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c8126e1c5d05510fb78c69f5b3a92603095a2ba3936b17a1623aded85e07bce8)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
+    @jsii.python.classproperty
+    @jsii.member(jsii_name="ATT_IMPORT_ARN_TOKEN")
+    def ATT_IMPORT_ARN_TOKEN(cls) -> builtins.str:
+        '''(experimental) Normalized CfnReference attribute.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.str, jsii.sget(cls, "ATT_IMPORT_ARN_TOKEN"))
+
+    @builtins.property
+    @jsii.member(jsii_name="isExtraneous")
+    def is_extraneous(self) -> builtins.bool:
+        '''(experimental) Indicates if this node is considered a {@link FlagEnum.EXTRANEOUS} node or determined to be extraneous: - Clusters that contain no children.
+
+        :stability: experimental
+        :inheritdoc: true
+        '''
+        return typing.cast(builtins.bool, jsii.get(self, "isExtraneous"))
+
+    @builtins.property
+    @jsii.member(jsii_name="isImport")
+    def is_import(self) -> builtins.bool:
+        '''(experimental) Indicates if this CfnResource is imported (eg: ``s3.Bucket.fromBucketArn``).
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.bool, jsii.get(self, "isImport"))
+
+    @builtins.property
+    @jsii.member(jsii_name="resource")
+    def resource(self) -> typing.Optional["ResourceNode"]:
+        '''(experimental) Reference to the L2 Resource that wraps this L1 CfnResource if it is wrapped.
+
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional["ResourceNode"], jsii.get(self, "resource"))
+
 
 class Dependency(
     Edge,
     metaclass=jsii.JSIIMeta,
     jsii_type="@aws-prototyping-sdk/cdk-graph.Graph.Dependency",
 ):
     '''(experimental) Dependency edge class defines CloudFormation dependency between resources.
@@ -658,33 +631,29 @@
     def __init__(self, props: "ITypedEdgeProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: ITypedEdgeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e3a832ab6009d6f06c0cc05ec3e9e8daf8cb0d99eff297417f90fd6fe8abdae3)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isDependency")
     @builtins.classmethod
     def is_dependency(cls, edge: "Edge") -> builtins.bool:
         '''(experimental) Indicates if given edge is a {@link Dependency} edge.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a55827c31e3f0c190debbad285924c8e16583aec1492518472f16ea8b115e0b2)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isDependency", [edge]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="PREFIX")
     def PREFIX(cls) -> builtins.str:
         '''(experimental) Edge prefix to denote dependency edge.
@@ -708,66 +677,54 @@
     def __init__(self, props: "IEdgeProps") -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IEdgeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__565a79591863a77e6f20b2cee05753f8fc6dc34f127886a605b534322b17129d)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="findAllInChain")
     @builtins.classmethod
     def find_all_in_chain(
         cls,
-        chain: typing.Mapping[typing.Any, typing.Any],
+        chain: typing.Sequence[typing.Any],
         predicate: "IEdgePredicate",
     ) -> typing.List["Edge"]:
         '''(experimental) Find all matching edges based on predicate within an EdgeChain.
 
         :param chain: -
         :param predicate: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                chain: typing.Mapping[typing.Any, typing.Any],
-                predicate: IEdgePredicate,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__387eb08fb3ad1478680d570ef24f6a2880477cbd5ba3b4dcded22d2af555ac3e)
             check_type(argname="argument chain", value=chain, expected_type=type_hints["chain"])
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
         return typing.cast(typing.List["Edge"], jsii.sinvoke(cls, "findAllInChain", [chain, predicate]))
 
     @jsii.member(jsii_name="findInChain")
     @builtins.classmethod
     def find_in_chain(
         cls,
-        chain: typing.Mapping[typing.Any, typing.Any],
+        chain: typing.Sequence[typing.Any],
         predicate: "IEdgePredicate",
     ) -> typing.Optional["Edge"]:
         '''(experimental) Find first edge matching predicate within an EdgeChain.
 
         :param chain: -
         :param predicate: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                chain: typing.Mapping[typing.Any, typing.Any],
-                predicate: IEdgePredicate,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3c528f43aad9061a4a97f99a7f632c278fa4c84f06b8d3409fdbdfdaa3087015)
             check_type(argname="argument chain", value=chain, expected_type=type_hints["chain"])
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
         return typing.cast(typing.Optional["Edge"], jsii.sinvoke(cls, "findInChain", [chain, predicate]))
 
     @jsii.member(jsii_name="isEquivalent")
     def is_equivalent(self, edge: "Edge") -> builtins.bool:
         '''(experimental) Indicates if this edge is equivalent to another edge.
@@ -775,17 +732,15 @@
         Edges are considered equivalent if they share same type, source, and target.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b071eb51a19132929d9d74150028aa4a0a1878c6c0a676ed59b43918ffdab592)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.invoke(self, "isEquivalent", [edge]))
 
     @jsii.member(jsii_name="mutateConsume")
     def mutate_consume(self, edge: "Edge") -> None:
         '''(experimental) Merge an equivalent edge's data into this edge and destroy the other edge.
 
@@ -794,17 +749,15 @@
         :param edge: - The edge to consume.
 
         :stability: experimental
         :destructive: true
         :throws: Error is edge is not *equivalent*
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b485c5bcae6dc3fe89a85d85dd95031030180a125e969944f3cdc29bc26c988b)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(None, jsii.invoke(self, "mutateConsume", [edge]))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, _strict: typing.Optional[builtins.bool] = None) -> None:
         '''(experimental) Destroy the edge.
 
@@ -812,65 +765,57 @@
 
         :param _strict: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(_strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__9aea030ae019edff51a5a1ac1e8043cc7338c3da1903beb257e15a787ddfc08b)
             check_type(argname="argument _strict", value=_strict, expected_type=type_hints["_strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [_strict]))
 
     @jsii.member(jsii_name="mutateDirection")
     def mutate_direction(self, direction: _EdgeDirectionEnum_26ef4ba3) -> None:
         '''(experimental) Change the edge **direction**.
 
         :param direction: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(direction: _EdgeDirectionEnum_26ef4ba3) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__2cb143b5341533709729ec323073f11266b6753ebc21ef3738fe819546f3936f)
             check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
         return typing.cast(None, jsii.invoke(self, "mutateDirection", [direction]))
 
     @jsii.member(jsii_name="mutateSource")
     def mutate_source(self, node: "Node") -> None:
         '''(experimental) Change the edge **source**.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c8a24c3128555e01a36b640f5816c7c4c8535e403966bdba1f21a26d9c4f8dc3)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "mutateSource", [node]))
 
     @jsii.member(jsii_name="mutateTarget")
     def mutate_target(self, node: "Node") -> None:
         '''(experimental) Change the edge **target**.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0c3acaa20c79aa2c0c3260a60a9d720b03bfd685f7ee524732d24eec7844705e)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "mutateTarget", [node]))
 
     @jsii.member(jsii_name="toString")
     def to_string(self) -> builtins.str:
         '''(experimental) Get string representation of this edge.
 
@@ -1116,19 +1061,15 @@
 
     @value.setter
     def value(
         self,
         value: typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]],
     ) -> None:
         if __debug__:
-            def stub(
-                value: typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]],
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__878edd6fd09a1e14434186a5bcddbf91e475feec0e2163aad3930537d644a5f9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "value", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IAttributeReferenceProps).__jsii_proxy_class__ = lambda : _IAttributeReferencePropsProxy
 
 
@@ -1137,15 +1078,17 @@
     '''(experimental) Base interface for all store entities **data** props.
 
     :stability: experimental
     '''
 
     @builtins.property
     @jsii.member(jsii_name="attributes")
-    def attributes(self) -> typing.Optional[_Attributes_b47661e3]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]]:
         '''(experimental) Attributes.
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
@@ -1155,24 +1098,26 @@
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="metadata")
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Metadata entries.
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="tags")
-    def tags(self) -> typing.Optional[_Tags_cf30c388]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Tags.
 
         :stability: experimental
         '''
         ...
 
 
@@ -1182,47 +1127,51 @@
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.Graph.IBaseEntityDataProps"
 
     @builtins.property
     @jsii.member(jsii_name="attributes")
-    def attributes(self) -> typing.Optional[_Attributes_b47661e3]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]]:
         '''(experimental) Attributes.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_Attributes_b47661e3], jsii.get(self, "attributes"))
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]]], jsii.get(self, "attributes"))
 
     @builtins.property
     @jsii.member(jsii_name="flags")
     def flags(self) -> typing.Optional[typing.List[_FlagEnum_af90e158]]:
         '''(experimental) Flags.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[typing.List[_FlagEnum_af90e158]], jsii.get(self, "flags"))
 
     @builtins.property
     @jsii.member(jsii_name="metadata")
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Metadata entries.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[typing.List[constructs.MetadataEntry]], jsii.get(self, "metadata"))
+        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]], jsii.get(self, "metadata"))
 
     @builtins.property
     @jsii.member(jsii_name="tags")
-    def tags(self) -> typing.Optional[_Tags_cf30c388]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Tags.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[_Tags_cf30c388], jsii.get(self, "tags"))
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], jsii.get(self, "tags"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IBaseEntityDataProps).__jsii_proxy_class__ = lambda : _IBaseEntityDataPropsProxy
 
 
 @jsii.interface(jsii_type="@aws-prototyping-sdk/cdk-graph.Graph.IBaseEntityProps")
 class IBaseEntityProps(IBaseEntityDataProps, typing_extensions.Protocol):
@@ -1286,14 +1235,26 @@
 class ICfnResourceNodeProps(ITypedNodeProps, typing_extensions.Protocol):
     '''(experimental) CfnResourceNode props.
 
     :stability: experimental
     '''
 
     @builtins.property
+    @jsii.member(jsii_name="importArnToken")
+    def import_arn_token(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        ...
+
+    @import_arn_token.setter
+    def import_arn_token(self, value: typing.Optional[builtins.str]) -> None:
+        ...
+
+    @builtins.property
     @jsii.member(jsii_name="nodeType")
     def node_type(self) -> typing.Optional[_NodeTypeEnum_d56eed04]:
         '''
         :stability: experimental
         '''
         ...
 
@@ -1309,27 +1270,40 @@
 
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.Graph.ICfnResourceNodeProps"
 
     @builtins.property
+    @jsii.member(jsii_name="importArnToken")
+    def import_arn_token(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "importArnToken"))
+
+    @import_arn_token.setter
+    def import_arn_token(self, value: typing.Optional[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__85ea2e1dd1bb8c898b74a5b3df6a209a1b7f5c45c6021ce1f7799f142115dfb0)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "importArnToken", value)
+
+    @builtins.property
     @jsii.member(jsii_name="nodeType")
     def node_type(self) -> typing.Optional[_NodeTypeEnum_d56eed04]:
         '''
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_NodeTypeEnum_d56eed04], jsii.get(self, "nodeType"))
 
     @node_type.setter
     def node_type(self, value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__72f92b9a5013d310afd14008b47a2b1b0f49dd8d6196d7b881ff314a4f327606)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeType", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ICfnResourceNodeProps).__jsii_proxy_class__ = lambda : _ICfnResourceNodePropsProxy
 
 
@@ -1419,23 +1393,26 @@
     '''(experimental) Options for edge based search operations.
 
     :stability: experimental
     '''
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order of traversal during search path.
 
         :stability: experimental
         '''
         ...
 
     @order.setter
-    def order(self, value: typing.Optional[constructs.ConstructOrder]) -> None:
+    def order(
+        self,
+        value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+    ) -> None:
         ...
 
     @builtins.property
     @jsii.member(jsii_name="predicate")
     def predicate(self) -> typing.Optional[IEdgePredicate]:
         '''(experimental) The predicate to match edges(s).
 
@@ -1467,27 +1444,28 @@
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.Graph.IFindEdgeOptions"
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order of traversal during search path.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[constructs.ConstructOrder], jsii.get(self, "order"))
+        return typing.cast(typing.Optional[_constructs_77d1e7e8.ConstructOrder], jsii.get(self, "order"))
 
     @order.setter
-    def order(self, value: typing.Optional[constructs.ConstructOrder]) -> None:
+    def order(
+        self,
+        value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+    ) -> None:
         if __debug__:
-            def stub(value: typing.Optional[constructs.ConstructOrder]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e128cc9136dc85835714e718c2e64263b54381b317d8e2fb25eac37a0dbe09a3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "order", value)
 
     @builtins.property
     @jsii.member(jsii_name="predicate")
     def predicate(self) -> typing.Optional[IEdgePredicate]:
         '''(experimental) The predicate to match edges(s).
@@ -1495,17 +1473,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional[IEdgePredicate], jsii.get(self, "predicate"))
 
     @predicate.setter
     def predicate(self, value: typing.Optional[IEdgePredicate]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[IEdgePredicate]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b3e2686c736d7bbb5d02fc501bba4a79340cf0aaeb7e5166705d58d75a7ce901)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predicate", value)
 
     @builtins.property
     @jsii.member(jsii_name="reverse")
     def reverse(self) -> typing.Optional[builtins.bool]:
         '''(experimental) Indicates reverse order.
@@ -1513,17 +1489,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "reverse"))
 
     @reverse.setter
     def reverse(self, value: typing.Optional[builtins.bool]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[builtins.bool]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__7d06982107e5638704f17753180695706a67f521fe486ba6864ad966be2b926d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "reverse", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IFindEdgeOptions).__jsii_proxy_class__ = lambda : _IFindEdgeOptionsProxy
 
 
@@ -1532,23 +1506,26 @@
     '''(experimental) Options for node based search operations.
 
     :stability: experimental
     '''
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order of traversal during search path.
 
         :stability: experimental
         '''
         ...
 
     @order.setter
-    def order(self, value: typing.Optional[constructs.ConstructOrder]) -> None:
+    def order(
+        self,
+        value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+    ) -> None:
         ...
 
     @builtins.property
     @jsii.member(jsii_name="predicate")
     def predicate(self) -> typing.Optional["INodePredicate"]:
         '''(experimental) The predicate to match node(s).
 
@@ -1567,27 +1544,28 @@
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.Graph.IFindNodeOptions"
 
     @builtins.property
     @jsii.member(jsii_name="order")
-    def order(self) -> typing.Optional[constructs.ConstructOrder]:
+    def order(self) -> typing.Optional[_constructs_77d1e7e8.ConstructOrder]:
         '''(experimental) The order of traversal during search path.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Optional[constructs.ConstructOrder], jsii.get(self, "order"))
+        return typing.cast(typing.Optional[_constructs_77d1e7e8.ConstructOrder], jsii.get(self, "order"))
 
     @order.setter
-    def order(self, value: typing.Optional[constructs.ConstructOrder]) -> None:
+    def order(
+        self,
+        value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+    ) -> None:
         if __debug__:
-            def stub(value: typing.Optional[constructs.ConstructOrder]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__5c6c3ca546a80bddaa40e8e8125d2f18d4e694c6278b34d505f1a6886e57f0eb)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "order", value)
 
     @builtins.property
     @jsii.member(jsii_name="predicate")
     def predicate(self) -> typing.Optional["INodePredicate"]:
         '''(experimental) The predicate to match node(s).
@@ -1595,17 +1573,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional["INodePredicate"], jsii.get(self, "predicate"))
 
     @predicate.setter
     def predicate(self, value: typing.Optional["INodePredicate"]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[INodePredicate]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__f987a29e8c2569b783057aaaae9c7dc03ff37161dedd81262b64d5d75befe441)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "predicate", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IFindNodeOptions).__jsii_proxy_class__ = lambda : _IFindNodeOptionsProxy
 
 
@@ -1909,17 +1885,15 @@
 
     @reference_type.setter
     def reference_type(
         self,
         value: typing.Optional[_ReferenceTypeEnum_f84a272a],
     ) -> None:
         if __debug__:
-            def stub(value: typing.Optional[_ReferenceTypeEnum_f84a272a]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3bca673777e2ac574585bbe0366364c386fb5557588e28399e965e8ae60cecf6)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "referenceType", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IReferenceProps).__jsii_proxy_class__ = lambda : _IReferencePropsProxy
 
 
@@ -1975,17 +1949,15 @@
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "cdkOwned"))
 
     @cdk_owned.setter
     def cdk_owned(self, value: builtins.bool) -> None:
         if __debug__:
-            def stub(value: builtins.bool) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__178bc7d96fdc0715984a68df870e2d280353e17e9a9aea73dd6310fbc7b28287)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "cdkOwned", value)
 
     @builtins.property
     @jsii.member(jsii_name="nodeType")
     def node_type(self) -> typing.Optional[_NodeTypeEnum_d56eed04]:
         '''(experimental) Type of node.
@@ -1993,17 +1965,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_NodeTypeEnum_d56eed04], jsii.get(self, "nodeType"))
 
     @node_type.setter
     def node_type(self, value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__2d0a05e2350bf80bc0a81226a87e97cbbea288c0621085ca0e5bb28cb252e50c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeType", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IResourceNodeProps).__jsii_proxy_class__ = lambda : _IResourceNodePropsProxy
 
 
@@ -2046,17 +2016,15 @@
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_NodeTypeEnum_d56eed04], jsii.get(self, "nodeType"))
 
     @node_type.setter
     def node_type(self, value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
         if __debug__:
-            def stub(value: typing.Optional[_NodeTypeEnum_d56eed04]) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ca857bdc964fa7f62d5fd74d38056d8272dca6ede1e00732f7035612d2245f87)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "nodeType", value)
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IStackNodeProps).__jsii_proxy_class__ = lambda : _IStackNodePropsProxy
 
 
@@ -2065,15 +2033,15 @@
     '''(experimental) Interface for store counts.
 
     :stability: experimental
     '''
 
     @builtins.property
     @jsii.member(jsii_name="cfnResources")
-    def cfn_resources(self) -> _ICounterRecord_97e6658c:
+    def cfn_resources(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *cfnResourceType*.
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
@@ -2083,15 +2051,15 @@
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="edgeTypes")
-    def edge_types(self) -> _ICounterRecord_97e6658c:
+    def edge_types(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *edge type* ({@link EdgeTypeEnum}).
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
@@ -2101,15 +2069,15 @@
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
     @jsii.member(jsii_name="nodeTypes")
-    def node_types(self) -> _ICounterRecord_97e6658c:
+    def node_types(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *node type* ({@link NodeTypeEnum}).
 
         :stability: experimental
         '''
         ...
 
     @builtins.property
@@ -2137,56 +2105,56 @@
     :stability: experimental
     '''
 
     __jsii_type__: typing.ClassVar[str] = "@aws-prototyping-sdk/cdk-graph.Graph.IStoreCounts"
 
     @builtins.property
     @jsii.member(jsii_name="cfnResources")
-    def cfn_resources(self) -> _ICounterRecord_97e6658c:
+    def cfn_resources(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *cfnResourceType*.
 
         :stability: experimental
         '''
-        return typing.cast(_ICounterRecord_97e6658c, jsii.get(self, "cfnResources"))
+        return typing.cast(typing.Mapping[builtins.str, jsii.Number], jsii.get(self, "cfnResources"))
 
     @builtins.property
     @jsii.member(jsii_name="edges")
     def edges(self) -> jsii.Number:
         '''(experimental) Counts total number of edges in the store.
 
         :stability: experimental
         '''
         return typing.cast(jsii.Number, jsii.get(self, "edges"))
 
     @builtins.property
     @jsii.member(jsii_name="edgeTypes")
-    def edge_types(self) -> _ICounterRecord_97e6658c:
+    def edge_types(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *edge type* ({@link EdgeTypeEnum}).
 
         :stability: experimental
         '''
-        return typing.cast(_ICounterRecord_97e6658c, jsii.get(self, "edgeTypes"))
+        return typing.cast(typing.Mapping[builtins.str, jsii.Number], jsii.get(self, "edgeTypes"))
 
     @builtins.property
     @jsii.member(jsii_name="nodes")
     def nodes(self) -> jsii.Number:
         '''(experimental) Counts total number of nodes in the store.
 
         :stability: experimental
         '''
         return typing.cast(jsii.Number, jsii.get(self, "nodes"))
 
     @builtins.property
     @jsii.member(jsii_name="nodeTypes")
-    def node_types(self) -> _ICounterRecord_97e6658c:
+    def node_types(self) -> typing.Mapping[builtins.str, jsii.Number]:
         '''(experimental) Returns {@link ICounterRecord} containing total number of each *node type* ({@link NodeTypeEnum}).
 
         :stability: experimental
         '''
-        return typing.cast(_ICounterRecord_97e6658c, jsii.get(self, "nodeTypes"))
+        return typing.cast(typing.Mapping[builtins.str, jsii.Number], jsii.get(self, "nodeTypes"))
 
     @builtins.property
     @jsii.member(jsii_name="stacks")
     def stacks(self) -> jsii.Number:
         '''(experimental) Counts total number of stacks in the store.
 
         :stability: experimental
@@ -2433,33 +2401,29 @@
     def __init__(self, props: ITypedEdgeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: ITypedEdgeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__7db191189b140e450105ccbbdb4a26978d3b48093677c5add42077123d463e37)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isImport")
     @builtins.classmethod
     def is_import(cls, edge: Edge) -> builtins.bool:
         '''(experimental) Indicates if edge is **Fn::ImportValue** based {@link Reference}.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__d29bb2e1c3c371d810d65ed1a6bd689b3ef6de75564f8ef5a79833d151e8e250)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isImport", [edge]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="PREFIX")
     def PREFIX(cls) -> builtins.str:
         '''(experimental) Edge prefix to denote **Fn::ImportValue** type reference edge.
@@ -2482,49 +2446,43 @@
     def __init__(self, props: INestedStackNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: INestedStackNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e7ac6ad89768d3478915aafced62faf74e307c3ca7aa61e6db1a16c6a73963ec)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isNestedStackNode")
     @builtins.classmethod
     def is_nested_stack_node(cls, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if node is a {@link NestedStackNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3dc08a1f205bc85166f446d3fe57ff0c8ea632094a9c0ed3f512fbec7c0c181c)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isNestedStackNode", [node]))
 
     @jsii.member(jsii_name="mutateHoist")
     def mutate_hoist(self, new_parent: "Node") -> None:
         '''(experimental) Hoist *this node* to an *ancestor* by removing it from its current parent node and in turn moving it to the ancestor.
 
         :param new_parent: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(new_parent: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__6ae5c4fc3b8838fbd562ba92bb108ecf140f5d59d8196f11647b1c24c744d1fa)
             check_type(argname="argument new_parent", value=new_parent, expected_type=type_hints["new_parent"])
         return typing.cast(None, jsii.invoke(self, "mutateHoist", [new_parent]))
 
     @builtins.property
     @jsii.member(jsii_name="parentStack")
     def parent_stack(self) -> typing.Optional["StackNode"]:
         '''(experimental) Get parent stack of this nested stack.
@@ -2548,107 +2506,93 @@
     def __init__(self, props: INodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: INodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3828ead8bf86124c90920b21db316c8d96f4bde4c2509d9306b65e1e483cb803)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="addChild")
     def add_child(self, node: "Node") -> None:
         '''(experimental) Add *child* node.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__660e5266dcbccc6d68a1d665d5643f01fb811bca791da508b8406b1efea26218)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "addChild", [node]))
 
     @jsii.member(jsii_name="addLink")
     def add_link(self, edge: Edge) -> None:
         '''(experimental) Add *link* to another node.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__950a47b2f30805881fb396a1678934ae556f3922893543466c1492d83b151e4c)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(None, jsii.invoke(self, "addLink", [edge]))
 
     @jsii.member(jsii_name="addReverseLink")
     def add_reverse_link(self, edge: Edge) -> None:
         '''(experimental) Add *link* from another node.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__7920f9005a933cb465d01ab88083ace4be3c276a4522d4a25d07b888425572d3)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(None, jsii.invoke(self, "addReverseLink", [edge]))
 
     @jsii.member(jsii_name="doesDependOn")
     def does_depend_on(self, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if *this node* depends on *another node*.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__9919e8d8cb3b44c75cf59828f105875f4171e2024238efd84c1a118fb5514c99)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "doesDependOn", [node]))
 
     @jsii.member(jsii_name="doesReference")
     def does_reference(self, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if *this node* references *another node*.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__92ca223a5acf7697dc45ed9734aa2cacb08f6cd3b4db410734ad231276cbfcd9)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "doesReference", [node]))
 
     @jsii.member(jsii_name="find")
     def find(self, predicate: INodePredicate) -> typing.Optional["Node"]:
         '''(experimental) Recursively find the nearest sub-node matching predicate.
 
         :param predicate: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(predicate: INodePredicate) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4d7a1df56f19469cb4d9cb54f0940240ce497ecab57f4496d6960193aa3edfa9)
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
         return typing.cast(typing.Optional["Node"], jsii.invoke(self, "find", [predicate]))
 
     @jsii.member(jsii_name="findAll")
     def find_all(
         self,
         options: typing.Optional[IFindNodeOptions] = None,
@@ -2658,17 +2602,15 @@
         Optionally filter nodes based on predicate.
 
         :param options: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(options: typing.Optional[IFindNodeOptions] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3de1fad418cfe5f4719dc84ed7bba9d9adc9beac216010e2526dee0cfbdb209f)
             check_type(argname="argument options", value=options, expected_type=type_hints["options"])
         return typing.cast(typing.List["Node"], jsii.invoke(self, "findAll", [options]))
 
     @jsii.member(jsii_name="findAllLinks")
     def find_all_links(
         self,
         options: typing.Optional[IFindEdgeOptions] = None,
@@ -2678,17 +2620,15 @@
         Optionally filter links based on predicate.
 
         :param options: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(options: typing.Optional[IFindEdgeOptions] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__6d03cf83f5642506a7afbefaed492487101ef6ebc1d3cb2c986b164dcbdddd79)
             check_type(argname="argument options", value=options, expected_type=type_hints["options"])
         return typing.cast(typing.List[Edge], jsii.invoke(self, "findAllLinks", [options]))
 
     @jsii.member(jsii_name="findAncestor")
     def find_ancestor(
         self,
         predicate: INodePredicate,
@@ -2699,20 +2639,15 @@
         :param predicate: - Predicate to match ancestor.
         :param max: -
 
         :stability: experimental
         :max: {number} [max] - Optional maximum levels to ascend
         '''
         if __debug__:
-            def stub(
-                predicate: INodePredicate,
-                max: typing.Optional[jsii.Number] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__88395df03122aa635fb6f4597f050e985a0b4e55a16c5349adaa2448d38269fd)
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
             check_type(argname="argument max", value=max, expected_type=type_hints["max"])
         return typing.cast(typing.Optional["Node"], jsii.invoke(self, "findAncestor", [predicate, max]))
 
     @jsii.member(jsii_name="findChild")
     def find_child(self, id: builtins.str) -> typing.Optional["Node"]:
         '''(experimental) Find child with given *id*.
@@ -2720,17 +2655,15 @@
         Similar to ``find`` but does not throw error if no child found.
 
         :param id: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0371b61ddfb489c7f038cbadceaa548fb06394017828b31e7d9206aea6260a4f)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         return typing.cast(typing.Optional["Node"], jsii.invoke(self, "findChild", [id]))
 
     @jsii.member(jsii_name="findLink")
     def find_link(
         self,
         predicate: IEdgePredicate,
@@ -2748,22 +2681,15 @@
         :param reverse: Indicates if links are search in reverse order.
         :param follow: Indicates if link chain is followed.
         :param direct: Indicates that only *direct* links should be searched.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                predicate: IEdgePredicate,
-                reverse: typing.Optional[builtins.bool] = None,
-                follow: typing.Optional[builtins.bool] = None,
-                direct: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__1a7491d537c9ab799bce5d2ab30cffcb5310005cc132ed3f7ec71f6dbdd42415)
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
             check_type(argname="argument reverse", value=reverse, expected_type=type_hints["reverse"])
             check_type(argname="argument follow", value=follow, expected_type=type_hints["follow"])
             check_type(argname="argument direct", value=direct, expected_type=type_hints["direct"])
         return typing.cast(typing.Optional[Edge], jsii.invoke(self, "findLink", [predicate, reverse, follow, direct]))
 
     @jsii.member(jsii_name="findLinks")
@@ -2784,22 +2710,15 @@
         :param reverse: Indicates if links are search in reverse order.
         :param follow: Indicates if link chain is followed.
         :param direct: Indicates that only *direct* links should be searched.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                predicate: IEdgePredicate,
-                reverse: typing.Optional[builtins.bool] = None,
-                follow: typing.Optional[builtins.bool] = None,
-                direct: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8b0d0271faf5cdefcbaac49f7d8d077ad73e5e0575e996c71aeafbfa9f4fb213)
             check_type(argname="argument predicate", value=predicate, expected_type=type_hints["predicate"])
             check_type(argname="argument reverse", value=reverse, expected_type=type_hints["reverse"])
             check_type(argname="argument follow", value=follow, expected_type=type_hints["follow"])
             check_type(argname="argument direct", value=direct, expected_type=type_hints["direct"])
         return typing.cast(typing.List[Edge], jsii.invoke(self, "findLinks", [predicate, reverse, follow, direct]))
 
     @jsii.member(jsii_name="getCfnProp")
@@ -2810,98 +2729,86 @@
         '''(experimental) Get specific CloudFormation property.
 
         :param key: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(key: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__52a9cf6162894ad371b2be534f47cd170b0286b91525fc353614c491769c1ac4)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast(typing.Optional[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]]], jsii.invoke(self, "getCfnProp", [key]))
 
     @jsii.member(jsii_name="getChild")
     def get_child(self, id: builtins.str) -> "Node":
         '''(experimental) Get *child* node with given *id*.
 
         :param id: -
 
         :stability: experimental
         :throws: Error if no child with given id
         '''
         if __debug__:
-            def stub(id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__fbf0509ec81421028b36f5fc628975eaf4b3174ae9db597feb70ef1211d6d23d)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         return typing.cast("Node", jsii.invoke(self, "getChild", [id]))
 
     @jsii.member(jsii_name="getLinkChains")
     def get_link_chains(
         self,
         reverse: typing.Optional[builtins.bool] = None,
-    ) -> typing.List[typing.Mapping[typing.Any, typing.Any]]:
+    ) -> typing.List[typing.List[typing.Any]]:
         '''(experimental) Resolve all link chains.
 
         :param reverse: -
 
-        :see: {@link EdgeChain}
+        :see: {@link EdgeChain }
         :stability: experimental
         '''
         if __debug__:
-            def stub(reverse: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__328f00d8bbc774b58559a9bc2e3705be60b5fed106c181bdc43ad7ff230fbe93)
             check_type(argname="argument reverse", value=reverse, expected_type=type_hints["reverse"])
-        return typing.cast(typing.List[typing.Mapping[typing.Any, typing.Any]], jsii.invoke(self, "getLinkChains", [reverse]))
+        return typing.cast(typing.List[typing.List[typing.Any]], jsii.invoke(self, "getLinkChains", [reverse]))
 
     @jsii.member(jsii_name="getNearestAncestor")
     def get_nearest_ancestor(self, node: "Node") -> "Node":
         '''(experimental) Gets the nearest **common** *ancestor* shared between *this node* and another *node*.
 
         :param node: -
 
         :stability: experimental
         :throws: Error if *node* does not share a **common** *ancestor*
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a2010858ae6af994e0c04bcd399cca1662e3caa6dc5fccc2f74bd8e3975e5a41)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast("Node", jsii.invoke(self, "getNearestAncestor", [node]))
 
     @jsii.member(jsii_name="isAncestor")
     def is_ancestor(self, ancestor: "Node") -> builtins.bool:
         '''(experimental) Indicates if a specific *node* is an *ancestor* of *this node*.
 
         :param ancestor: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(ancestor: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__9fea04ff2f6aca6c7074518194316a202ea683acfb7d4edceb7d2f026ef771ce)
             check_type(argname="argument ancestor", value=ancestor, expected_type=type_hints["ancestor"])
         return typing.cast(builtins.bool, jsii.invoke(self, "isAncestor", [ancestor]))
 
     @jsii.member(jsii_name="isChild")
     def is_child(self, node: "Node") -> builtins.bool:
         '''(experimental) Indicates if specific *node* is a *child* of *this node*.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b3043d164cfb82d3cf4029f11e63febb27c3b10077624c5ef03d086a1b62b562)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "isChild", [node]))
 
     @jsii.member(jsii_name="mutateCollapse")
     def mutate_collapse(self) -> None:
         '''(experimental) Collapses all sub-nodes of *this node* into *this node*.
 
@@ -2916,17 +2823,15 @@
 
         :param ancestor: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(ancestor: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__607e9fc2abbc1b5eccb854daaa8a1ca6750284575a23065ca7c145185a0c2173)
             check_type(argname="argument ancestor", value=ancestor, expected_type=type_hints["ancestor"])
         return typing.cast("Node", jsii.invoke(self, "mutateCollapseTo", [ancestor]))
 
     @jsii.member(jsii_name="mutateCollapseToParent")
     def mutate_collapse_to_parent(self) -> "Node":
         '''(experimental) Collapses *this node* into *it's parent node*.
 
@@ -2941,81 +2846,85 @@
 
         :param strict: - Indicates that this node must not have references.
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__507e828ffc35a034c5da26332531323a871b4818e34d5a95a49ee3e9468578c1)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
     @jsii.member(jsii_name="mutateHoist")
     def mutate_hoist(self, new_parent: "Node") -> None:
         '''(experimental) Hoist *this node* to an *ancestor* by removing it from its current parent node and in turn moving it to the ancestor.
 
         :param new_parent: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(new_parent: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c90bf585a9bfeb5a8e8430ec071e0807b1431d2c6e3b71fb3f4c1eae62ec1f71)
             check_type(argname="argument new_parent", value=new_parent, expected_type=type_hints["new_parent"])
         return typing.cast(None, jsii.invoke(self, "mutateHoist", [new_parent]))
 
+    @jsii.member(jsii_name="mutateMove")
+    def mutate_move(self, new_parent: "Node") -> None:
+        '''(experimental) Move this node into a new parent node.
+
+        :param new_parent: - The parent to move this node to.
+
+        :stability: experimental
+        :destructive: true
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__98fcaba69666753f2c565722884fc3a0f6bccabf1301835f0408de885aad908d)
+            check_type(argname="argument new_parent", value=new_parent, expected_type=type_hints["new_parent"])
+        return typing.cast(None, jsii.invoke(self, "mutateMove", [new_parent]))
+
     @jsii.member(jsii_name="mutateRemoveChild")
     def mutate_remove_child(self, node: "Node") -> builtins.bool:
         '''(experimental) Remove a *child* node from *this node*.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__78fbc6d51eee317e9641c7eeb83f0201859c2425cc2bcbd5ed47fa7210226e53)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveChild", [node]))
 
     @jsii.member(jsii_name="mutateRemoveLink")
     def mutate_remove_link(self, link: Edge) -> builtins.bool:
         '''(experimental) Remove a *link* from *this node*.
 
         :param link: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(link: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e3763bcb6869549f2191966731ecc8ddb6470740f6a0af951d2660ce138c1f02)
             check_type(argname="argument link", value=link, expected_type=type_hints["link"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveLink", [link]))
 
     @jsii.member(jsii_name="mutateRemoveReverseLink")
     def mutate_remove_reverse_link(self, link: Edge) -> builtins.bool:
         '''(experimental) Remove a *link* to *this node*.
 
         :param link: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(link: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c0b8e3af21a48815eeb6cb406e9d94490aa14ed0d60a16d9a05bbb0a1e84f573)
             check_type(argname="argument link", value=link, expected_type=type_hints["link"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveReverseLink", [link]))
 
     @jsii.member(jsii_name="mutateUncluster")
     def mutate_uncluster(self) -> None:
         '''(experimental) Hoist all children to parent and collapse node to parent.
 
@@ -3033,15 +2942,15 @@
         return typing.cast(builtins.str, jsii.invoke(self, "toString", []))
 
     @builtins.property
     @jsii.member(jsii_name="allowDestructiveMutations")
     def allow_destructive_mutations(self) -> builtins.bool:
         '''(experimental) Indicates if this node allows destructive mutations.
 
-        :see: {@link Store.allowDestructiveMutations}
+        :see: {@link Store.allowDestructiveMutations }
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "allowDestructiveMutations"))
 
     @builtins.property
     @jsii.member(jsii_name="children")
     def children(self) -> typing.List["Node"]:
@@ -3052,25 +2961,25 @@
         return typing.cast(typing.List["Node"], jsii.get(self, "children"))
 
     @builtins.property
     @jsii.member(jsii_name="dependedOnBy")
     def depended_on_by(self) -> typing.List["Node"]:
         '''(experimental) Get list of **Nodes** that *depend on this node*.
 
-        :see: {@link Node.reverseDependencyLinks}
+        :see: {@link Node.reverseDependencyLinks }
         :stability: experimental
         '''
         return typing.cast(typing.List["Node"], jsii.get(self, "dependedOnBy"))
 
     @builtins.property
     @jsii.member(jsii_name="dependencies")
     def dependencies(self) -> typing.List["Node"]:
         '''(experimental) Get list of **Nodes** that *this node depends on*.
 
-        :see: {@link Node.dependencyLinks}
+        :see: {@link Node.dependencyLinks }
         :stability: experimental
         '''
         return typing.cast(typing.List["Node"], jsii.get(self, "dependencies"))
 
     @builtins.property
     @jsii.member(jsii_name="dependencyLinks")
     def dependency_links(self) -> typing.List[Dependency]:
@@ -3104,14 +3013,24 @@
         '''(experimental) Indicates if this node is considered a {@link FlagEnum.ASSET}.
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isAsset"))
 
     @builtins.property
+    @jsii.member(jsii_name="isCfnFqn")
+    def is_cfn_fqn(self) -> builtins.bool:
+        '''(experimental) Indicates if node ConstructInfoFqn denotes a ``aws-cdk-lib.*.Cfn*`` construct.
+
+        :see: {@link FlagEnum.CFN_FQN }
+        :stability: experimental
+        '''
+        return typing.cast(builtins.bool, jsii.get(self, "isCfnFqn"))
+
+    @builtins.property
     @jsii.member(jsii_name="isCluster")
     def is_cluster(self) -> builtins.bool:
         '''(experimental) Indicates if this node is considered a {@link FlagEnum.CLUSTER}.
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isCluster"))
@@ -3149,23 +3068,14 @@
         '''(experimental) Indicates if this node is a *leaf* node, which means it does not have children.
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isLeaf"))
 
     @builtins.property
-    @jsii.member(jsii_name="isResourceWrapper")
-    def is_resource_wrapper(self) -> builtins.bool:
-        '''(experimental) Indicates if this node is considered a {@link FlagEnum.RESOURCE_WRAPPER}.
-
-        :stability: experimental
-        '''
-        return typing.cast(builtins.bool, jsii.get(self, "isResourceWrapper"))
-
-    @builtins.property
     @jsii.member(jsii_name="isTopLevel")
     def is_top_level(self) -> builtins.bool:
         '''(experimental) Indicates if node is direct child of the graph root node.
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isTopLevel"))
@@ -3198,15 +3108,15 @@
         return typing.cast(builtins.str, jsii.get(self, "path"))
 
     @builtins.property
     @jsii.member(jsii_name="referencedBy")
     def referenced_by(self) -> typing.List["Node"]:
         '''(experimental) Get list of **Nodes** that *reference this node*.
 
-        :see: {@link Node.reverseReferenceLinks}
+        :see: {@link Node.reverseReferenceLinks }
         :stability: experimental
         '''
         return typing.cast(typing.List["Node"], jsii.get(self, "referencedBy"))
 
     @builtins.property
     @jsii.member(jsii_name="referenceLinks")
     def reference_links(self) -> typing.List["Reference"]:
@@ -3217,15 +3127,15 @@
         return typing.cast(typing.List["Reference"], jsii.get(self, "referenceLinks"))
 
     @builtins.property
     @jsii.member(jsii_name="references")
     def references(self) -> typing.List["Node"]:
         '''(experimental) Get list of **Nodes** that *this node references*.
 
-        :see: {@link Node.referenceLinks}
+        :see: {@link Node.referenceLinks }
         :stability: experimental
         '''
         return typing.cast(typing.List["Node"], jsii.get(self, "references"))
 
     @builtins.property
     @jsii.member(jsii_name="reverseDependencyLinks")
     def reverse_dependency_links(self) -> typing.List[Dependency]:
@@ -3359,49 +3269,43 @@
     def __init__(self, props: IOutputNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IOutputNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__468d8aa0c2c058d6fadc1792cd8fc2eda84138f5f1f19654418418f2f1ee81d0)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isOutputNode")
     @builtins.classmethod
     def is_output_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is an {@link OutputNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__341e7d4025c24323c7b7d0490e6511e71334745d2e727d43dc7a5c846434997c)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isOutputNode", [node]))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, strict: typing.Optional[builtins.bool] = None) -> None:
         '''(experimental) Destroys this node by removing all references and removing this node from the store.
 
         :param strict: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3fcfdefecedfc68bbc9fa94992433c957b6576cf3be5c051b9380c3824336a89)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ATTR_EXPORT_NAME")
     def ATTR_EXPORT_NAME(cls) -> builtins.str:
         '''(experimental) Attribute key where output export name is stored.
@@ -3460,49 +3364,43 @@
     def __init__(self, props: IParameterNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IParameterNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__9638efd25caccc2ef0fa4aaaea89e5d0eb407019fcb019dcf3ccc599bf009186)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isParameterNode")
     @builtins.classmethod
     def is_parameter_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is a {@link ParameterNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8bc764de94d64191057dc0fdddc809d1eae2a13db0ba699099ee63cf23cf4ac3)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isParameterNode", [node]))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, strict: typing.Optional[builtins.bool] = None) -> None:
         '''(experimental) Destroys this node by removing all references and removing this node from the store.
 
         :param strict: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b204a4a9b59958a703a9f5e1ef21ce03e8b7ac7480a39d9f148f40584966989b)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ATTR_TYPE")
     def ATTR_TYPE(cls) -> builtins.str:
         '''(experimental) Attribute key where parameter type is stored.
@@ -3561,65 +3459,59 @@
     def __init__(self, props: IReferenceProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IReferenceProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__084a54c1ab771f992279f9bd45b8b1baa0822bdd4be4755bcb8af2dc8528074a)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isRef")
     @builtins.classmethod
     def is_ref(cls, edge: Edge) -> builtins.bool:
         '''(experimental) Indicates if edge is a **Ref** based {@link Reference} edge.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__066e00209e68c755ee4c72d70c56b15f2859b03ba639a0e3478e5219e5484102)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isRef", [edge]))
 
     @jsii.member(jsii_name="isReference")
     @builtins.classmethod
     def is_reference(cls, edge: Edge) -> builtins.bool:
         '''(experimental) Indicates if edge is a {@link Reference}.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e8a83fcc0e3ce69c8f66a8e13d3c09da598c7a3b369d1e17a8dcdcd35c0d80fd)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isReference", [edge]))
 
     @jsii.member(jsii_name="resolveChain")
-    def resolve_chain(self) -> typing.Mapping[typing.Any, typing.Any]:
+    def resolve_chain(self) -> typing.List[typing.Any]:
         '''(experimental) Resolve reference chain.
 
         :stability: experimental
         '''
-        return typing.cast(typing.Mapping[typing.Any, typing.Any], jsii.invoke(self, "resolveChain", []))
+        return typing.cast(typing.List[typing.Any], jsii.invoke(self, "resolveChain", []))
 
     @jsii.member(jsii_name="resolveTargets")
     def resolve_targets(self) -> typing.List[Node]:
         '''(experimental) Resolve targets by following potential edge chain.
 
-        :see: {@link EdgeChain}
+        :see: {@link EdgeChain }
         :stability: experimental
         '''
         return typing.cast(typing.List[Node], jsii.invoke(self, "resolveTargets", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ATT_TYPE")
     def ATT_TYPE(cls) -> builtins.str:
@@ -3661,33 +3553,29 @@
     def __init__(self, props: IResourceNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IResourceNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c2363d97608132cfa857d387f10cc3dec3f7ef057f1b7b697f4f1d351169ad84)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isResourceNode")
     @builtins.classmethod
     def is_resource_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is a {@link ResourceNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__9335e387ef4acc9195bd97a83a1b45677db2a467d9dc7b2dc07f1f40031caffb)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isResourceNode", [node]))
 
     @jsii.member(jsii_name="mutateCfnResource")
     def mutate_cfn_resource(
         self,
         cfn_resource: typing.Optional[CfnResourceNode] = None,
@@ -3696,33 +3584,29 @@
 
         :param cfn_resource: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(cfn_resource: typing.Optional[CfnResourceNode] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__dff29f6b35258807146e6f9ba684036473f6686ef00dd5f4a4f164560b7fb119)
             check_type(argname="argument cfn_resource", value=cfn_resource, expected_type=type_hints["cfn_resource"])
         return typing.cast(None, jsii.invoke(self, "mutateCfnResource", [cfn_resource]))
 
     @jsii.member(jsii_name="mutateRemoveChild")
     def mutate_remove_child(self, node: Node) -> builtins.bool:
         '''(experimental) Remove a *child* node from *this node*.
 
         :param node: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__be21910448f5008c76f791bbf31865edd9143efc14428eec72f980f5f9bfbf68)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveChild", [node]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="ATT_WRAPPED_CFN_PROPS")
     def ATT_WRAPPED_CFN_PROPS(cls) -> builtins.str:
         '''(experimental) Attribute key for cfn properties.
@@ -3746,26 +3630,35 @@
         '''(experimental) Indicates if this resource is owned by cdk (defined in cdk library).
 
         :stability: experimental
         '''
         return typing.cast(builtins.bool, jsii.get(self, "isCdkOwned"))
 
     @builtins.property
+    @jsii.member(jsii_name="isWrapper")
+    def is_wrapper(self) -> builtins.bool:
+        '''(experimental) Indicates if Resource wraps a single CfnResource.
+
+        :stability: experimental
+        '''
+        return typing.cast(builtins.bool, jsii.get(self, "isWrapper"))
+
+    @builtins.property
     @jsii.member(jsii_name="cfnProps")
     def cfn_props(self) -> typing.Optional[_PlainObject_c976ebcc]:
         '''(experimental) Get the cfn properties from the L1 resource that this L2 resource wraps.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[_PlainObject_c976ebcc], jsii.get(self, "cfnProps"))
 
     @builtins.property
     @jsii.member(jsii_name="cfnResource")
     def cfn_resource(self) -> typing.Optional[CfnResourceNode]:
-        '''(experimental) Get the L1 cdk resource that this L2 resource wraps.
+        '''(experimental) Get the default/primary CfnResource that this Resource wraps.
 
         :stability: experimental
         '''
         return typing.cast(typing.Optional[CfnResourceNode], jsii.get(self, "cfnResource"))
 
     @builtins.property
     @jsii.member(jsii_name="cfnType")
@@ -3785,130 +3678,131 @@
     '''(experimental) RootNode represents the root of the store tree.
 
     :stability: experimental
     '''
 
     def __init__(self, store: "Store") -> None:
         '''
-        :param store: -
+        :param store: Reference to the store.
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(store: Store) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__70c74c57319631ae3a6bb90226d9dbc9d41fce0ce074d2922b491ba4a94d8a4c)
             check_type(argname="argument store", value=store, expected_type=type_hints["store"])
         jsii.create(self.__class__, self, [store])
 
     @jsii.member(jsii_name="isRootNode")
     @builtins.classmethod
     def is_root_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is a {@link RootNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__7cd2de0d05c272cac06eb9293a536eb9bad5fd419027bb74b57daa38deb7e724)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isRootNode", [node]))
 
     @jsii.member(jsii_name="findAll")
     def find_all(
         self,
         options: typing.Optional[IFindNodeOptions] = None,
     ) -> typing.List[Node]:
         '''(experimental) Return this construct and all of its sub-nodes in the given order.
 
         Optionally filter nodes based on predicate.
+        **The root not is excluded from list**
 
         :param options: -
 
         :stability: experimental
         :inheritdoc: **The root not is excluded from list**
         '''
         if __debug__:
-            def stub(options: typing.Optional[IFindNodeOptions] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b7e4ec539b0da7d44f4c03b42ef3d5181b4a7ef9449b782a8ffa7ddfdff0b13e)
             check_type(argname="argument options", value=options, expected_type=type_hints["options"])
         return typing.cast(typing.List[Node], jsii.invoke(self, "findAll", [options]))
 
     @jsii.member(jsii_name="mutateCollapse")
     def mutate_collapse(self) -> None:
-        '''(experimental) > {@link RootNode} does not support this mutation.
+        '''(experimental) Collapses all sub-nodes of *this node* into *this node*.
+
+        .. epigraph::
+
+           {@link RootNode} does not support this mutation
 
         :stability: experimental
         :inheritdoc: true
         :throws: Error does not support
         '''
         return typing.cast(None, jsii.invoke(self, "mutateCollapse", []))
 
     @jsii.member(jsii_name="mutateCollapseTo")
     def mutate_collapse_to(self, _ancestor: Node) -> Node:
-        '''(experimental) > {@link RootNode} does not support this mutation.
+        '''(experimental) Collapses *this node* into *an ancestor* > {@link RootNode} does not support this mutation.
 
         :param _ancestor: -
 
         :stability: experimental
         :inheritdoc: true
         :throws: Error does not support
         '''
         if __debug__:
-            def stub(_ancestor: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__5c834f108ee6961b2028e6e8e49394b37c6f4f9b84cb5c942da26d10ff9af80f)
             check_type(argname="argument _ancestor", value=_ancestor, expected_type=type_hints["_ancestor"])
         return typing.cast(Node, jsii.invoke(self, "mutateCollapseTo", [_ancestor]))
 
     @jsii.member(jsii_name="mutateCollapseToParent")
     def mutate_collapse_to_parent(self) -> Node:
-        '''(experimental) > {@link RootNode} does not support this mutation.
+        '''(experimental) Collapses *this node* into *it's parent node* > {@link RootNode} does not support this mutation.
 
         :stability: experimental
         :inheritdoc: true
         :throws: Error does not support
         '''
         return typing.cast(Node, jsii.invoke(self, "mutateCollapseToParent", []))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, _strict: typing.Optional[builtins.bool] = None) -> None:
-        '''(experimental) > {@link RootNode} does not support this mutation.
+        '''(experimental) Destroys this node by removing all references and removing this node from the store.
+
+        .. epigraph::
+
+           {@link RootNode} does not support this mutation
 
         :param _strict: -
 
         :stability: experimental
         :inheritdoc: true
         :throws: Error does not support
         '''
         if __debug__:
-            def stub(_strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__83c1ae906a7e0caed6efd885dc9a196395e2b5f63f3160ea34c03faf22ac9457)
             check_type(argname="argument _strict", value=_strict, expected_type=type_hints["_strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [_strict]))
 
     @jsii.member(jsii_name="mutateHoist")
     def mutate_hoist(self, _new_parent: Node) -> None:
-        '''(experimental) > {@link RootNode} does not support this mutation.
+        '''(experimental) Hoist *this node* to an *ancestor* by removing it from its current parent node and in turn moving it to the ancestor.
+
+        .. epigraph::
+
+           {@link RootNode} does not support this mutation
 
         :param _new_parent: -
 
         :stability: experimental
         :inheritdoc: true
         :throws: Error does not support
         '''
         if __debug__:
-            def stub(_new_parent: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ddf799ef2e1c7016825dcc9f6dca273a9c27eb61714556e8a01eaf3f12e47325)
             check_type(argname="argument _new_parent", value=_new_parent, expected_type=type_hints["_new_parent"])
         return typing.cast(None, jsii.invoke(self, "mutateHoist", [_new_parent]))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="PATH")
     def PATH(cls) -> builtins.str:
         '''(experimental) Fixed path of root.
@@ -3940,176 +3834,154 @@
     def __init__(self, props: IStackNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: IStackNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8561c6913224897aa431f468a2799f52adcfd1ed17da963d9aeb6870be12f018)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isStackNode")
     @builtins.classmethod
     def is_stack_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is a {@link StackNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__810fda21c589e5baf8944505f48ffec2b6afc34712cf50ddfd38d29d9b964a08)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isStackNode", [node]))
 
     @jsii.member(jsii_name="of")
     @builtins.classmethod
     def of(cls, node: Node) -> "StackNode":
         '''(experimental) Gets the {@link StackNode} containing a given resource.
 
         :param node: -
 
         :stability: experimental
         :throws: Error is node is not contained in a stack
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3ddb225e5316ad05600109c743ef33b78aceeadcc2877127402a658120f43a1c)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast("StackNode", jsii.sinvoke(cls, "of", [node]))
 
     @jsii.member(jsii_name="addOutput")
     def add_output(self, node: OutputNode) -> None:
         '''(experimental) Associate {@link OutputNode} with this stack.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: OutputNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0c7610929a215a6b477c0bf837f43bd457957c845841df6b746b43e96314992b)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "addOutput", [node]))
 
     @jsii.member(jsii_name="addParameter")
     def add_parameter(self, node: ParameterNode) -> None:
         '''(experimental) Associate {@link ParameterNode} with this stack.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: ParameterNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__5acff93bffed07ac3c30ad3ef4f0a14d7ab9b3b5b59367da263c6e522fb3940f)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "addParameter", [node]))
 
     @jsii.member(jsii_name="findOutput")
     def find_output(self, logical_id: builtins.str) -> OutputNode:
         '''(experimental) Find {@link OutputNode} with *logicalId* defined by this stack.
 
         :param logical_id: -
 
         :stability: experimental
         :throws: Error is no output found matching *logicalId*
         '''
         if __debug__:
-            def stub(logical_id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__aa2152445d4abfd4ae264fb45f727c25666df1af6155ea23590c15ac45ca4d78)
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
         return typing.cast(OutputNode, jsii.invoke(self, "findOutput", [logical_id]))
 
     @jsii.member(jsii_name="findParameter")
     def find_parameter(self, parameter_id: builtins.str) -> ParameterNode:
         '''(experimental) Find {@link ParameterNode} with *parameterId* defined by this stack.
 
         :param parameter_id: -
 
         :stability: experimental
         :throws: Error is no parameter found matching *parameterId*
         '''
         if __debug__:
-            def stub(parameter_id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e683328da929f0b97266b4aca2bd8ec2d63fc72dc2a031465e501c804ab6e13f)
             check_type(argname="argument parameter_id", value=parameter_id, expected_type=type_hints["parameter_id"])
         return typing.cast(ParameterNode, jsii.invoke(self, "findParameter", [parameter_id]))
 
     @jsii.member(jsii_name="mutateDestroy")
     def mutate_destroy(self, strict: typing.Optional[builtins.bool] = None) -> None:
         '''(experimental) Destroys this node by removing all references and removing this node from the store.
 
         :param strict: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(strict: typing.Optional[builtins.bool] = None) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8c0a3f408552229076061809cc1ad18095abf412b4e718e719eddaf98b2a5739)
             check_type(argname="argument strict", value=strict, expected_type=type_hints["strict"])
         return typing.cast(None, jsii.invoke(self, "mutateDestroy", [strict]))
 
     @jsii.member(jsii_name="mutateHoist")
     def mutate_hoist(self, new_parent: Node) -> None:
         '''(experimental) Hoist *this node* to an *ancestor* by removing it from its current parent node and in turn moving it to the ancestor.
 
         :param new_parent: -
 
         :stability: experimental
         :inheritdoc: true
         '''
         if __debug__:
-            def stub(new_parent: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__55244d05fa1c7fa5fd1d2fc2372749d065fcc2436e56c6528efd469f4f012b5e)
             check_type(argname="argument new_parent", value=new_parent, expected_type=type_hints["new_parent"])
         return typing.cast(None, jsii.invoke(self, "mutateHoist", [new_parent]))
 
     @jsii.member(jsii_name="mutateRemoveOutput")
     def mutate_remove_output(self, node: OutputNode) -> builtins.bool:
         '''(experimental) Disassociate {@link OutputNode} from this stack.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: OutputNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__d6285b599f0367a174c9b747c7cfcfc297817ac7d5b02bcb86d0cee9104d2d9e)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveOutput", [node]))
 
     @jsii.member(jsii_name="mutateRemoveParameter")
     def mutate_remove_parameter(self, node: ParameterNode) -> builtins.bool:
         '''(experimental) Disassociate {@link ParameterNode} from this stack.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: ParameterNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__44d1e084de384ffe73669819d166d6e6480c70a9b7c26506aff947b4ccfd1ec4)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveParameter", [node]))
 
     @builtins.property
     @jsii.member(jsii_name="exports")
     def exports(self) -> typing.List[OutputNode]:
         '''(experimental) Get all **exported** {@link OutputNode}s defined by this stack.
@@ -4159,81 +4031,71 @@
     def __init__(self, props: ITypedNodeProps) -> None:
         '''
         :param props: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(props: ITypedNodeProps) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__73cab0d8aa0605b046b2d83d061191632f54f9d43cffd0344687426ccaa59701)
             check_type(argname="argument props", value=props, expected_type=type_hints["props"])
         jsii.create(self.__class__, self, [props])
 
     @jsii.member(jsii_name="isStageNode")
     @builtins.classmethod
     def is_stage_node(cls, node: Node) -> builtins.bool:
         '''(experimental) Indicates if node is a {@link StageNode}.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4be3d70b88f1b0ff06aa71076b2fc6512388a20a783bed64bf35db542ecc4b38)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.sinvoke(cls, "isStageNode", [node]))
 
     @jsii.member(jsii_name="of")
     @builtins.classmethod
     def of(cls, node: Node) -> "StageNode":
         '''(experimental) Gets the {@link StageNode} containing a given resource.
 
         :param node: -
 
         :stability: experimental
         :throws: Error is node is not contained in a stage
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__48a0c44022838184955a6d9f2cba2f81e20528fc2ac8aa7d7a0f6005797c4e99)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast("StageNode", jsii.sinvoke(cls, "of", [node]))
 
     @jsii.member(jsii_name="addStack")
     def add_stack(self, stack: StackNode) -> None:
         '''(experimental) Associate a {@link StackNode} with this stage.
 
         :param stack: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(stack: StackNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__235267f539ec2ba5698ef2d3f9d200a7270099e98d317a8160b0a6fe9534b05a)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
         return typing.cast(None, jsii.invoke(self, "addStack", [stack]))
 
     @jsii.member(jsii_name="mutateRemoveStack")
     def mutate_remove_stack(self, stack: StackNode) -> builtins.bool:
         '''(experimental) Disassociate {@link StackNode} from this stage.
 
         :param stack: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(stack: StackNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__cfc4b92a49675847b47feb1590f66a67164240c338b4905e9f2aaf50277df660)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveStack", [stack]))
 
     @builtins.property
     @jsii.member(jsii_name="stacks")
     def stacks(self) -> typing.List[StackNode]:
         '''(experimental) Gets all stacks contained by this stage.
@@ -4259,29 +4121,25 @@
     ) -> None:
         '''
         :param allow_destructive_mutations: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                allow_destructive_mutations: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e6071d61384d22ebee92d5050bf75a3a2c099a0e3e43cd8a1f9855af5afe58ec)
             check_type(argname="argument allow_destructive_mutations", value=allow_destructive_mutations, expected_type=type_hints["allow_destructive_mutations"])
         jsii.create(self.__class__, self, [allow_destructive_mutations])
 
     @jsii.member(jsii_name="fromSerializedStore")
     @builtins.classmethod
     def from_serialized_store(
         cls,
         *,
-        edges: typing.Sequence[typing.Union[_Edge_211392d6, typing.Dict[str, typing.Any]]],
-        tree: typing.Union[_Node_bc073df3, typing.Dict[str, typing.Any]],
+        edges: typing.Sequence[typing.Union[_Edge_211392d6, typing.Dict[builtins.str, typing.Any]]],
+        tree: typing.Union[_Node_bc073df3, typing.Dict[builtins.str, typing.Any]],
         version: builtins.str,
     ) -> "Store":
         '''(experimental) Builds store from serialized store data.
 
         :param edges: (experimental) List of edges.
         :param tree: (experimental) Node tree.
         :param version: (experimental) Store version.
@@ -4299,62 +4157,54 @@
         '''(experimental) Add **edge** to the store.
 
         :param edge: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__4f279f4eca65dce0d7e1312c61b0f08aeeaf5f801034c003d5149c9adfb19647)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(None, jsii.invoke(self, "addEdge", [edge]))
 
     @jsii.member(jsii_name="addNode")
     def add_node(self, node: Node) -> None:
         '''(experimental) Add **node** to the store.
 
         :param node: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8b4b65f46e249f8df6aa49ca0eadd929438204d7b8e1e2cc5b0e782e3e9a6b97)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(None, jsii.invoke(self, "addNode", [node]))
 
     @jsii.member(jsii_name="addStack")
     def add_stack(self, stack: StackNode) -> None:
         '''(experimental) Add **stack** node to the store.
 
         :param stack: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(stack: StackNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__a470952503b834cf06aaf22156aa54e848467d7c340b0cbd985103fdaaeb333b)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
         return typing.cast(None, jsii.invoke(self, "addStack", [stack]))
 
     @jsii.member(jsii_name="addStage")
     def add_stage(self, stage: StageNode) -> None:
         '''(experimental) Add **stage** to the store.
 
         :param stage: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(stage: StageNode) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0a1eeae7977161b856a5610e6f566729a2ab89a8940adebc9b536fc0c0daacc4)
             check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
         return typing.cast(None, jsii.invoke(self, "addStage", [stage]))
 
     @jsii.member(jsii_name="clone")
     def clone(
         self,
         allow_destructive_mutations: typing.Optional[builtins.bool] = None,
@@ -4364,19 +4214,15 @@
         :param allow_destructive_mutations: Indicates if destructive mutations are allowed; defaults to ``true``
 
         :return: Returns a clone of the store that allows destructive mutations
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                allow_destructive_mutations: typing.Optional[builtins.bool] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b868d40d441434984ca5b2d6e701aeb1a1f5db194812c8746b0b44d65e08c158)
             check_type(argname="argument allow_destructive_mutations", value=allow_destructive_mutations, expected_type=type_hints["allow_destructive_mutations"])
         return typing.cast("Store", jsii.invoke(self, "clone", [allow_destructive_mutations]))
 
     @jsii.member(jsii_name="computeLogicalUniversalId")
     def compute_logical_universal_id(
         self,
         stack: StackNode,
@@ -4389,149 +4235,161 @@
 
         :param stack: -
         :param logical_id: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(stack: StackNode, logical_id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ca2bb6e1af58945082681e65524c50737f44c93a7701345bcff8c287a6d47a6a)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
         return typing.cast(builtins.str, jsii.invoke(self, "computeLogicalUniversalId", [stack, logical_id]))
 
+    @jsii.member(jsii_name="findNodeByImportArn")
+    def find_node_by_import_arn(self, value: typing.Any) -> typing.Optional[Node]:
+        '''(experimental) Attempts to lookup the {@link Node} associated with a given *import arn token*.
+
+        :param value: Import arn value, which is either object to tokenize or already tokenized string.
+
+        :return: Returns matching {@link Node } if found, otherwise undefined.
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__2c8fddf4de9a1b3f490080c3e3a7d883bfd2a42197676f76c285ec5ed8ba3acb)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(typing.Optional[Node], jsii.invoke(self, "findNodeByImportArn", [value]))
+
     @jsii.member(jsii_name="findNodeByLogicalId")
     def find_node_by_logical_id(
         self,
         stack: StackNode,
         logical_id: builtins.str,
     ) -> Node:
         '''(experimental) Find node within given **stack** with given *logicalId*.
 
         :param stack: -
         :param logical_id: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(stack: StackNode, logical_id: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0b0e8720f3f8d29fb8f935dd7670a3162ccad53d41bdc17d074d084878bc53c2)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
         return typing.cast(Node, jsii.invoke(self, "findNodeByLogicalId", [stack, logical_id]))
 
     @jsii.member(jsii_name="findNodeByLogicalUniversalId")
     def find_node_by_logical_universal_id(self, uid: builtins.str) -> Node:
         '''(experimental) Find node by **universal** *logicalId* (``<stack>:<logicalId>``).
 
         :param uid: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(uid: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__5692654cee964ec073a85ab0fc354208184a7e31f1d53fc37e1135208d06c139)
             check_type(argname="argument uid", value=uid, expected_type=type_hints["uid"])
         return typing.cast(Node, jsii.invoke(self, "findNodeByLogicalUniversalId", [uid]))
 
     @jsii.member(jsii_name="getEdge")
     def get_edge(self, uuid: builtins.str) -> Edge:
         '''(experimental) Get stored **edge** by UUID.
 
         :param uuid: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(uuid: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__f6337aec154d7b7c30df409802bb9b65b050e58eb529da6904feb187571820e3)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
         return typing.cast(Edge, jsii.invoke(self, "getEdge", [uuid]))
 
     @jsii.member(jsii_name="getNode")
     def get_node(self, uuid: builtins.str) -> Node:
         '''(experimental) Get stored **node** by UUID.
 
         :param uuid: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(uuid: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__37ae39c9dbbe89389f0891ee760db2cde58966f12365de9ae0fdf76580c5f779)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
         return typing.cast(Node, jsii.invoke(self, "getNode", [uuid]))
 
     @jsii.member(jsii_name="getStack")
     def get_stack(self, uuid: builtins.str) -> StackNode:
         '''(experimental) Get stored **stack** node by UUID.
 
         :param uuid: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(uuid: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__b5f45b2ecc1808c4501ec02302b2819629f58df64c8d414665fa585845fa56ac)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
         return typing.cast(StackNode, jsii.invoke(self, "getStack", [uuid]))
 
     @jsii.member(jsii_name="getStage")
     def get_stage(self, uuid: builtins.str) -> StageNode:
         '''(experimental) Get stored **stage** node by UUID.
 
         :param uuid: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(uuid: builtins.str) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__dd3bece2511c783049540686b74bd123c2d37c3edd0c5bf63843ad4d6ae28654)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
         return typing.cast(StageNode, jsii.invoke(self, "getStage", [uuid]))
 
     @jsii.member(jsii_name="mutateRemoveEdge")
     def mutate_remove_edge(self, edge: Edge) -> builtins.bool:
         '''(experimental) Remove **edge** from the store.
 
         :param edge: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(edge: Edge) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__6544890573554e16b1a9cde6583c011c33ebf4931b9a6e1c2947135de9cdb582)
             check_type(argname="argument edge", value=edge, expected_type=type_hints["edge"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveEdge", [edge]))
 
     @jsii.member(jsii_name="mutateRemoveNode")
     def mutate_remove_node(self, node: Node) -> builtins.bool:
         '''(experimental) Remove **node** from the store.
 
         :param node: -
 
         :stability: experimental
         :destructive: true
         '''
         if __debug__:
-            def stub(node: Node) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e6abcd76bb62a3d0fa3f2332b0648937acc8b52903cee2cb88c40020f175896e)
             check_type(argname="argument node", value=node, expected_type=type_hints["node"])
         return typing.cast(builtins.bool, jsii.invoke(self, "mutateRemoveNode", [node]))
 
+    @jsii.member(jsii_name="recordImportArn")
+    def record_import_arn(self, arn_token: builtins.str, resource: Node) -> None:
+        '''(experimental) Records arn tokens from imported resources (eg: ``s3.Bucket.fromBucketArn()``) that are used for resolving references.
+
+        :param arn_token: -
+        :param resource: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a5d35134a98c2990472ef42459ceb5cefe469098ae1030a5540803e3b84e934b)
+            check_type(argname="argument arn_token", value=arn_token, expected_type=type_hints["arn_token"])
+            check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
+        return typing.cast(None, jsii.invoke(self, "recordImportArn", [arn_token, resource]))
+
     @jsii.member(jsii_name="recordLogicalId")
     def record_logical_id(
         self,
         stack: StackNode,
         logical_id: builtins.str,
         resource: Node,
     ) -> None:
@@ -4540,21 +4398,15 @@
         :param stack: -
         :param logical_id: -
         :param resource: -
 
         :stability: experimental
         '''
         if __debug__:
-            def stub(
-                stack: StackNode,
-                logical_id: builtins.str,
-                resource: Node,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__36b1b85e7270585b5ab9b82f399c4303ef8a04f133d6e5a9217ee87928df92bc)
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
             check_type(argname="argument resource", value=resource, expected_type=type_hints["resource"])
         return typing.cast(None, jsii.invoke(self, "recordLogicalId", [stack, logical_id, resource]))
 
     @jsii.member(jsii_name="serialize")
     def serialize(self) -> _GraphStore_ffbd5720:
@@ -4709,7 +4561,817 @@
     "RootNode",
     "StackNode",
     "StageNode",
     "Store",
 ]
 
 publication.publish()
+
+def _typecheckingstub__0ea8733837e9bb40c0c1ec64c6feb23f2ed1eb8273206106202412f46230febc(
+    props: IAppNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bc02148277079718cf5c2f39c016f5b52c973f922c600de573dfe478f1099ea8(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4c00aba2e4c442b0b145e9d63dacde89d6cad17d0bca8108c310f8b64e92b4be(
+    props: IAttributeReferenceProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4bafcead49197db174341aefc0d5b06356f41cc6ec4cabc8fac26198d34a7c77(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cd84a9b7a0cf09d1574c06e6f4d90abcb54ce21eb50a1ddbdfff201bfbc29b91(
+    props: IBaseEntityProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__913d0433bc5941f0e59ee1edd8c046080f32987b0ab6c5e19bc266fe027bf146(
+    key: builtins.str,
+    value: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__033b704f8a3c2f15a71de50e0db70b6f64c4b7e621236182d7afa37d2d368613(
+    flag: _FlagEnum_af90e158,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cd7e4b19c50d04193a5603d24e18130fd0ce75cc5f857918800659670b7b1f2a(
+    metadata_type: builtins.str,
+    data: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__144a4bdde601cb81c22f5fbfce2338b613a871b555081164aa45293a33462c97(
+    key: builtins.str,
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__04a459899bd329d2e4da70421ba17a31f77418a63fdc6bd5f9f961a28646d657(
+    data: IBaseEntityDataProps,
+    overwrite: typing.Optional[builtins.bool] = None,
+    apply_flags: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c0d83a5d6b8bda51859f759127513a969f1857e948919d6ddb6d356a8f0f4f83(
+    metadata_type: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3834b50954aaca507835cac1f164e2d1138952543da9236359ef21d6ab4d98ef(
+    key: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1363a79f63c40b917b308f8b4729b20d5f6487075463e75700b9635b24564164(
+    key: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__64b3d7ba1056459f4e688ea0a44d03ec6261908f53a39f49b0f2efdf5bdad6d5(
+    key: builtins.str,
+    value: typing.Any = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__39e58d1c8b02a0e3dff78d26530288d9f6ccc04c3ec96cef394e1975b1572b1a(
+    flag: _FlagEnum_af90e158,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4928bedd38550599d6ca3f869e7168cd1f62e843c4be593ef78a6937899eda16(
+    metadata_type: builtins.str,
+    data: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ddcfff79d83e7452bec9439ed35aca725ab7baaac4652a3f897fc3b7f0300ee2(
+    key: builtins.str,
+    value: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__df8536147c5294b85dcf0b4564016e283be874d48b901226622ed863f48d99fc(
+    key: builtins.str,
+    value: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a8e3c2cf27179bb2c32917aa8a4cdc4f81bb829323dfae17b926d2d78030ec15(
+    key: builtins.str,
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ba4fd8a0a02bae9f886b47c9eb0f948c4d98d60935d19cd5ca6a568b276ce4fb(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e911cbd53a062053f329bf8f21a964493c96016d01a786631899820c452ab446(
+    props: ICfnResourceNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4d16082b017b42d002eb6b446987841f2b7bac243a65193dedb18a6561c2a89f(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a3bd9dbf3af183f7178d5e6bfbc05cb2eb158af66809077e88ac2843e729c088(
+    resource: ResourceNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c8126e1c5d05510fb78c69f5b3a92603095a2ba3936b17a1623aded85e07bce8(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e3a832ab6009d6f06c0cc05ec3e9e8daf8cb0d99eff297417f90fd6fe8abdae3(
+    props: ITypedEdgeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a55827c31e3f0c190debbad285924c8e16583aec1492518472f16ea8b115e0b2(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__565a79591863a77e6f20b2cee05753f8fc6dc34f127886a605b534322b17129d(
+    props: IEdgeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__387eb08fb3ad1478680d570ef24f6a2880477cbd5ba3b4dcded22d2af555ac3e(
+    chain: typing.Sequence[typing.Any],
+    predicate: IEdgePredicate,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3c528f43aad9061a4a97f99a7f632c278fa4c84f06b8d3409fdbdfdaa3087015(
+    chain: typing.Sequence[typing.Any],
+    predicate: IEdgePredicate,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b071eb51a19132929d9d74150028aa4a0a1878c6c0a676ed59b43918ffdab592(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b485c5bcae6dc3fe89a85d85dd95031030180a125e969944f3cdc29bc26c988b(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9aea030ae019edff51a5a1ac1e8043cc7338c3da1903beb257e15a787ddfc08b(
+    _strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2cb143b5341533709729ec323073f11266b6753ebc21ef3738fe819546f3936f(
+    direction: _EdgeDirectionEnum_26ef4ba3,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c8a24c3128555e01a36b640f5816c7c4c8535e403966bdba1f21a26d9c4f8dc3(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0c3acaa20c79aa2c0c3260a60a9d720b03bfd685f7ee524732d24eec7844705e(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__878edd6fd09a1e14434186a5bcddbf91e475feec0e2163aad3930537d644a5f9(
+    value: typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc, typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, _PlainObject_c976ebcc]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__85ea2e1dd1bb8c898b74a5b3df6a209a1b7f5c45c6021ce1f7799f142115dfb0(
+    value: typing.Optional[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__72f92b9a5013d310afd14008b47a2b1b0f49dd8d6196d7b881ff314a4f327606(
+    value: typing.Optional[_NodeTypeEnum_d56eed04],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e128cc9136dc85835714e718c2e64263b54381b317d8e2fb25eac37a0dbe09a3(
+    value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b3e2686c736d7bbb5d02fc501bba4a79340cf0aaeb7e5166705d58d75a7ce901(
+    value: typing.Optional[IEdgePredicate],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7d06982107e5638704f17753180695706a67f521fe486ba6864ad966be2b926d(
+    value: typing.Optional[builtins.bool],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5c6c3ca546a80bddaa40e8e8125d2f18d4e694c6278b34d505f1a6886e57f0eb(
+    value: typing.Optional[_constructs_77d1e7e8.ConstructOrder],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f987a29e8c2569b783057aaaae9c7dc03ff37161dedd81262b64d5d75befe441(
+    value: typing.Optional[INodePredicate],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3bca673777e2ac574585bbe0366364c386fb5557588e28399e965e8ae60cecf6(
+    value: typing.Optional[_ReferenceTypeEnum_f84a272a],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__178bc7d96fdc0715984a68df870e2d280353e17e9a9aea73dd6310fbc7b28287(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2d0a05e2350bf80bc0a81226a87e97cbbea288c0621085ca0e5bb28cb252e50c(
+    value: typing.Optional[_NodeTypeEnum_d56eed04],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ca857bdc964fa7f62d5fd74d38056d8272dca6ede1e00732f7035612d2245f87(
+    value: typing.Optional[_NodeTypeEnum_d56eed04],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7db191189b140e450105ccbbdb4a26978d3b48093677c5add42077123d463e37(
+    props: ITypedEdgeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d29bb2e1c3c371d810d65ed1a6bd689b3ef6de75564f8ef5a79833d151e8e250(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e7ac6ad89768d3478915aafced62faf74e307c3ca7aa61e6db1a16c6a73963ec(
+    props: INestedStackNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3dc08a1f205bc85166f446d3fe57ff0c8ea632094a9c0ed3f512fbec7c0c181c(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6ae5c4fc3b8838fbd562ba92bb108ecf140f5d59d8196f11647b1c24c744d1fa(
+    new_parent: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3828ead8bf86124c90920b21db316c8d96f4bde4c2509d9306b65e1e483cb803(
+    props: INodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__660e5266dcbccc6d68a1d665d5643f01fb811bca791da508b8406b1efea26218(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__950a47b2f30805881fb396a1678934ae556f3922893543466c1492d83b151e4c(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7920f9005a933cb465d01ab88083ace4be3c276a4522d4a25d07b888425572d3(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9919e8d8cb3b44c75cf59828f105875f4171e2024238efd84c1a118fb5514c99(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__92ca223a5acf7697dc45ed9734aa2cacb08f6cd3b4db410734ad231276cbfcd9(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4d7a1df56f19469cb4d9cb54f0940240ce497ecab57f4496d6960193aa3edfa9(
+    predicate: INodePredicate,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3de1fad418cfe5f4719dc84ed7bba9d9adc9beac216010e2526dee0cfbdb209f(
+    options: typing.Optional[IFindNodeOptions] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6d03cf83f5642506a7afbefaed492487101ef6ebc1d3cb2c986b164dcbdddd79(
+    options: typing.Optional[IFindEdgeOptions] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__88395df03122aa635fb6f4597f050e985a0b4e55a16c5349adaa2448d38269fd(
+    predicate: INodePredicate,
+    max: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0371b61ddfb489c7f038cbadceaa548fb06394017828b31e7d9206aea6260a4f(
+    id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1a7491d537c9ab799bce5d2ab30cffcb5310005cc132ed3f7ec71f6dbdd42415(
+    predicate: IEdgePredicate,
+    reverse: typing.Optional[builtins.bool] = None,
+    follow: typing.Optional[builtins.bool] = None,
+    direct: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8b0d0271faf5cdefcbaac49f7d8d077ad73e5e0575e996c71aeafbfa9f4fb213(
+    predicate: IEdgePredicate,
+    reverse: typing.Optional[builtins.bool] = None,
+    follow: typing.Optional[builtins.bool] = None,
+    direct: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__52a9cf6162894ad371b2be534f47cd170b0286b91525fc353614c491769c1ac4(
+    key: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fbf0509ec81421028b36f5fc628975eaf4b3174ae9db597feb70ef1211d6d23d(
+    id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__328f00d8bbc774b58559a9bc2e3705be60b5fed106c181bdc43ad7ff230fbe93(
+    reverse: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a2010858ae6af994e0c04bcd399cca1662e3caa6dc5fccc2f74bd8e3975e5a41(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9fea04ff2f6aca6c7074518194316a202ea683acfb7d4edceb7d2f026ef771ce(
+    ancestor: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b3043d164cfb82d3cf4029f11e63febb27c3b10077624c5ef03d086a1b62b562(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__607e9fc2abbc1b5eccb854daaa8a1ca6750284575a23065ca7c145185a0c2173(
+    ancestor: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__507e828ffc35a034c5da26332531323a871b4818e34d5a95a49ee3e9468578c1(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c90bf585a9bfeb5a8e8430ec071e0807b1431d2c6e3b71fb3f4c1eae62ec1f71(
+    new_parent: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__98fcaba69666753f2c565722884fc3a0f6bccabf1301835f0408de885aad908d(
+    new_parent: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__78fbc6d51eee317e9641c7eeb83f0201859c2425cc2bcbd5ed47fa7210226e53(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e3763bcb6869549f2191966731ecc8ddb6470740f6a0af951d2660ce138c1f02(
+    link: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c0b8e3af21a48815eeb6cb406e9d94490aa14ed0d60a16d9a05bbb0a1e84f573(
+    link: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__468d8aa0c2c058d6fadc1792cd8fc2eda84138f5f1f19654418418f2f1ee81d0(
+    props: IOutputNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__341e7d4025c24323c7b7d0490e6511e71334745d2e727d43dc7a5c846434997c(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3fcfdefecedfc68bbc9fa94992433c957b6576cf3be5c051b9380c3824336a89(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9638efd25caccc2ef0fa4aaaea89e5d0eb407019fcb019dcf3ccc599bf009186(
+    props: IParameterNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8bc764de94d64191057dc0fdddc809d1eae2a13db0ba699099ee63cf23cf4ac3(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b204a4a9b59958a703a9f5e1ef21ce03e8b7ac7480a39d9f148f40584966989b(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__084a54c1ab771f992279f9bd45b8b1baa0822bdd4be4755bcb8af2dc8528074a(
+    props: IReferenceProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__066e00209e68c755ee4c72d70c56b15f2859b03ba639a0e3478e5219e5484102(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e8a83fcc0e3ce69c8f66a8e13d3c09da598c7a3b369d1e17a8dcdcd35c0d80fd(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c2363d97608132cfa857d387f10cc3dec3f7ef057f1b7b697f4f1d351169ad84(
+    props: IResourceNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__9335e387ef4acc9195bd97a83a1b45677db2a467d9dc7b2dc07f1f40031caffb(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dff29f6b35258807146e6f9ba684036473f6686ef00dd5f4a4f164560b7fb119(
+    cfn_resource: typing.Optional[CfnResourceNode] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__be21910448f5008c76f791bbf31865edd9143efc14428eec72f980f5f9bfbf68(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__70c74c57319631ae3a6bb90226d9dbc9d41fce0ce074d2922b491ba4a94d8a4c(
+    store: Store,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7cd2de0d05c272cac06eb9293a536eb9bad5fd419027bb74b57daa38deb7e724(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b7e4ec539b0da7d44f4c03b42ef3d5181b4a7ef9449b782a8ffa7ddfdff0b13e(
+    options: typing.Optional[IFindNodeOptions] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5c834f108ee6961b2028e6e8e49394b37c6f4f9b84cb5c942da26d10ff9af80f(
+    _ancestor: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__83c1ae906a7e0caed6efd885dc9a196395e2b5f63f3160ea34c03faf22ac9457(
+    _strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ddf799ef2e1c7016825dcc9f6dca273a9c27eb61714556e8a01eaf3f12e47325(
+    _new_parent: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8561c6913224897aa431f468a2799f52adcfd1ed17da963d9aeb6870be12f018(
+    props: IStackNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__810fda21c589e5baf8944505f48ffec2b6afc34712cf50ddfd38d29d9b964a08(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3ddb225e5316ad05600109c743ef33b78aceeadcc2877127402a658120f43a1c(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0c7610929a215a6b477c0bf837f43bd457957c845841df6b746b43e96314992b(
+    node: OutputNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5acff93bffed07ac3c30ad3ef4f0a14d7ab9b3b5b59367da263c6e522fb3940f(
+    node: ParameterNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__aa2152445d4abfd4ae264fb45f727c25666df1af6155ea23590c15ac45ca4d78(
+    logical_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e683328da929f0b97266b4aca2bd8ec2d63fc72dc2a031465e501c804ab6e13f(
+    parameter_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8c0a3f408552229076061809cc1ad18095abf412b4e718e719eddaf98b2a5739(
+    strict: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__55244d05fa1c7fa5fd1d2fc2372749d065fcc2436e56c6528efd469f4f012b5e(
+    new_parent: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d6285b599f0367a174c9b747c7cfcfc297817ac7d5b02bcb86d0cee9104d2d9e(
+    node: OutputNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__44d1e084de384ffe73669819d166d6e6480c70a9b7c26506aff947b4ccfd1ec4(
+    node: ParameterNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__73cab0d8aa0605b046b2d83d061191632f54f9d43cffd0344687426ccaa59701(
+    props: ITypedNodeProps,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4be3d70b88f1b0ff06aa71076b2fc6512388a20a783bed64bf35db542ecc4b38(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__48a0c44022838184955a6d9f2cba2f81e20528fc2ac8aa7d7a0f6005797c4e99(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__235267f539ec2ba5698ef2d3f9d200a7270099e98d317a8160b0a6fe9534b05a(
+    stack: StackNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cfc4b92a49675847b47feb1590f66a67164240c338b4905e9f2aaf50277df660(
+    stack: StackNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e6071d61384d22ebee92d5050bf75a3a2c099a0e3e43cd8a1f9855af5afe58ec(
+    allow_destructive_mutations: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4f279f4eca65dce0d7e1312c61b0f08aeeaf5f801034c003d5149c9adfb19647(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8b4b65f46e249f8df6aa49ca0eadd929438204d7b8e1e2cc5b0e782e3e9a6b97(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a470952503b834cf06aaf22156aa54e848467d7c340b0cbd985103fdaaeb333b(
+    stack: StackNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0a1eeae7977161b856a5610e6f566729a2ab89a8940adebc9b536fc0c0daacc4(
+    stage: StageNode,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b868d40d441434984ca5b2d6e701aeb1a1f5db194812c8746b0b44d65e08c158(
+    allow_destructive_mutations: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__ca2bb6e1af58945082681e65524c50737f44c93a7701345bcff8c287a6d47a6a(
+    stack: StackNode,
+    logical_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__2c8fddf4de9a1b3f490080c3e3a7d883bfd2a42197676f76c285ec5ed8ba3acb(
+    value: typing.Any,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0b0e8720f3f8d29fb8f935dd7670a3162ccad53d41bdc17d074d084878bc53c2(
+    stack: StackNode,
+    logical_id: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__5692654cee964ec073a85ab0fc354208184a7e31f1d53fc37e1135208d06c139(
+    uid: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__f6337aec154d7b7c30df409802bb9b65b050e58eb529da6904feb187571820e3(
+    uuid: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__37ae39c9dbbe89389f0891ee760db2cde58966f12365de9ae0fdf76580c5f779(
+    uuid: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b5f45b2ecc1808c4501ec02302b2819629f58df64c8d414665fa585845fa56ac(
+    uuid: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dd3bece2511c783049540686b74bd123c2d37c3edd0c5bf63843ad4d6ae28654(
+    uuid: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__6544890573554e16b1a9cde6583c011c33ebf4931b9a6e1c2947135de9cdb582(
+    edge: Edge,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e6abcd76bb62a3d0fa3f2332b0648937acc8b52903cee2cb88c40020f175896e(
+    node: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a5d35134a98c2990472ef42459ceb5cefe469098ae1030a5540803e3b84e934b(
+    arn_token: builtins.str,
+    resource: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__36b1b85e7270585b5ab9b82f399c4303ef8a04f133d6e5a9217ee87928df92bc(
+    stack: StackNode,
+    logical_id: builtins.str,
+    resource: Node,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py` & `aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,50 +8,25 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from .._jsii import *
 
-import constructs
+import constructs as _constructs_77d1e7e8
 from .. import (
     ConstructInfo as _ConstructInfo_e912d4bb,
     EdgeDirectionEnum as _EdgeDirectionEnum_26ef4ba3,
     EdgeTypeEnum as _EdgeTypeEnum_1b13d7ee,
     FlagEnum as _FlagEnum_af90e158,
     NodeTypeEnum as _NodeTypeEnum_d56eed04,
 )
 
 
 @jsii.data_type(
-    jsii_type="@aws-prototyping-sdk/cdk-graph.SerializedGraph.Attributes",
-    jsii_struct_bases=[],
-    name_mapping={},
-)
-class Attributes:
-    def __init__(self) -> None:
-        '''(experimental) Serializable attributes mapping.
-
-        :stability: experimental
-        '''
-        self._values: typing.Dict[str, typing.Any] = {}
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "Attributes(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
     jsii_type="@aws-prototyping-sdk/cdk-graph.SerializedGraph.Edge",
     jsii_struct_bases=[Entity],
     name_mapping={
         "uuid": "uuid",
         "attributes": "attributes",
         "flags": "flags",
         "metadata": "metadata",
@@ -63,18 +38,18 @@
     },
 )
 class Edge(Entity):
     def __init__(
         self,
         *,
         uuid: builtins.str,
-        attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
+        attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]]]]]]] = None,
         flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-        metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-        tags: typing.Optional[typing.Union["Tags", typing.Dict[str, typing.Any]]] = None,
+        metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         direction: _EdgeDirectionEnum_26ef4ba3,
         edge_type: _EdgeTypeEnum_1b13d7ee,
         source: builtins.str,
         target: builtins.str,
     ) -> None:
         '''(experimental) Serializable graph edge entity.
 
@@ -86,43 +61,26 @@
         :param direction: (experimental) Indicates the direction in which the edge is directed.
         :param edge_type: (experimental) Type of edge.
         :param source: (experimental) UUID of edge **source** node (tail).
         :param target: (experimental) UUID of edge **target** node (head).
 
         :stability: experimental
         '''
-        if isinstance(attributes, dict):
-            attributes = Attributes(**attributes)
-        if isinstance(tags, dict):
-            tags = Tags(**tags)
         if __debug__:
-            def stub(
-                *,
-                uuid: builtins.str,
-                attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
-                flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-                metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-                tags: typing.Optional[typing.Union[Tags, typing.Dict[str, typing.Any]]] = None,
-                direction: _EdgeDirectionEnum_26ef4ba3,
-                edge_type: _EdgeTypeEnum_1b13d7ee,
-                source: builtins.str,
-                target: builtins.str,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__0df02c65dc4810873a004e52f214df46ce43efc61f582498a0f1af1abd6f2f7d)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
             check_type(argname="argument attributes", value=attributes, expected_type=type_hints["attributes"])
             check_type(argname="argument flags", value=flags, expected_type=type_hints["flags"])
             check_type(argname="argument metadata", value=metadata, expected_type=type_hints["metadata"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument direction", value=direction, expected_type=type_hints["direction"])
             check_type(argname="argument edge_type", value=edge_type, expected_type=type_hints["edge_type"])
             check_type(argname="argument source", value=source, expected_type=type_hints["source"])
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "uuid": uuid,
             "direction": direction,
             "edge_type": edge_type,
             "source": source,
             "target": target,
         }
         if attributes is not None:
@@ -141,52 +99,56 @@
         :stability: experimental
         '''
         result = self._values.get("uuid")
         assert result is not None, "Required property 'uuid' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def attributes(self) -> typing.Optional[Attributes]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]]:
         '''(experimental) Serializable entity attributes.
 
-        :see: {@link Attributes}
+        :see: {@link Attributes }
         :stability: experimental
         '''
         result = self._values.get("attributes")
-        return typing.cast(typing.Optional[Attributes], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]], result)
 
     @builtins.property
     def flags(self) -> typing.Optional[typing.List[_FlagEnum_af90e158]]:
         '''(experimental) Serializable entity flags.
 
-        :see: {@link FlagEnum}
+        :see: {@link FlagEnum }
         :stability: experimental
         '''
         result = self._values.get("flags")
         return typing.cast(typing.Optional[typing.List[_FlagEnum_af90e158]], result)
 
     @builtins.property
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Serializable entity metadata.
 
-        :see: {@link Metadata}
+        :see: {@link Metadata }
         :stability: experimental
         '''
         result = self._values.get("metadata")
-        return typing.cast(typing.Optional[typing.List[constructs.MetadataEntry]], result)
+        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]], result)
 
     @builtins.property
-    def tags(self) -> typing.Optional["Tags"]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Serializable entity tags.
 
-        :see: {@link Tags}
+        :see: {@link Tags }
         :stability: experimental
         '''
         result = self._values.get("tags")
-        return typing.cast(typing.Optional["Tags"], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def direction(self) -> _EdgeDirectionEnum_26ef4ba3:
         '''(experimental) Indicates the direction in which the edge is directed.
 
         :stability: experimental
         '''
@@ -248,50 +210,37 @@
     },
 )
 class Entity:
     def __init__(
         self,
         *,
         uuid: builtins.str,
-        attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
+        attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]]]]]]] = None,
         flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-        metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-        tags: typing.Optional[typing.Union["Tags", typing.Dict[str, typing.Any]]] = None,
+        metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     ) -> None:
         '''(experimental) Serializable graph entity.
 
         :param uuid: (experimental) Universally unique identity.
         :param attributes: (experimental) Serializable entity attributes.
         :param flags: (experimental) Serializable entity flags.
         :param metadata: (experimental) Serializable entity metadata.
         :param tags: (experimental) Serializable entity tags.
 
         :stability: experimental
         '''
-        if isinstance(attributes, dict):
-            attributes = Attributes(**attributes)
-        if isinstance(tags, dict):
-            tags = Tags(**tags)
         if __debug__:
-            def stub(
-                *,
-                uuid: builtins.str,
-                attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
-                flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-                metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-                tags: typing.Optional[typing.Union[Tags, typing.Dict[str, typing.Any]]] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__54acd3ac36d2232ab6ff52b62125889be84254bc3d141b1d2f66b7fc481a4ca6)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
             check_type(argname="argument attributes", value=attributes, expected_type=type_hints["attributes"])
             check_type(argname="argument flags", value=flags, expected_type=type_hints["flags"])
             check_type(argname="argument metadata", value=metadata, expected_type=type_hints["metadata"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "uuid": uuid,
         }
         if attributes is not None:
             self._values["attributes"] = attributes
         if flags is not None:
             self._values["flags"] = flags
         if metadata is not None:
@@ -306,52 +255,56 @@
         :stability: experimental
         '''
         result = self._values.get("uuid")
         assert result is not None, "Required property 'uuid' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def attributes(self) -> typing.Optional[Attributes]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]]:
         '''(experimental) Serializable entity attributes.
 
-        :see: {@link Attributes}
+        :see: {@link Attributes }
         :stability: experimental
         '''
         result = self._values.get("attributes")
-        return typing.cast(typing.Optional[Attributes], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]], result)
 
     @builtins.property
     def flags(self) -> typing.Optional[typing.List[_FlagEnum_af90e158]]:
         '''(experimental) Serializable entity flags.
 
-        :see: {@link FlagEnum}
+        :see: {@link FlagEnum }
         :stability: experimental
         '''
         result = self._values.get("flags")
         return typing.cast(typing.Optional[typing.List[_FlagEnum_af90e158]], result)
 
     @builtins.property
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Serializable entity metadata.
 
-        :see: {@link Metadata}
+        :see: {@link Metadata }
         :stability: experimental
         '''
         result = self._values.get("metadata")
-        return typing.cast(typing.Optional[typing.List[constructs.MetadataEntry]], result)
+        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]], result)
 
     @builtins.property
-    def tags(self) -> typing.Optional["Tags"]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Serializable entity tags.
 
-        :see: {@link Tags}
+        :see: {@link Tags }
         :stability: experimental
         '''
         result = self._values.get("tags")
-        return typing.cast(typing.Optional["Tags"], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
@@ -366,41 +319,34 @@
     jsii_struct_bases=[],
     name_mapping={"edges": "edges", "tree": "tree", "version": "version"},
 )
 class GraphStore:
     def __init__(
         self,
         *,
-        edges: typing.Sequence[typing.Union[Edge, typing.Dict[str, typing.Any]]],
-        tree: typing.Union["Node", typing.Dict[str, typing.Any]],
+        edges: typing.Sequence[typing.Union[Edge, typing.Dict[builtins.str, typing.Any]]],
+        tree: typing.Union["Node", typing.Dict[builtins.str, typing.Any]],
         version: builtins.str,
     ) -> None:
         '''(experimental) Serializable graph store.
 
         :param edges: (experimental) List of edges.
         :param tree: (experimental) Node tree.
         :param version: (experimental) Store version.
 
         :stability: experimental
         '''
         if isinstance(tree, dict):
             tree = Node(**tree)
         if __debug__:
-            def stub(
-                *,
-                edges: typing.Sequence[typing.Union[Edge, typing.Dict[str, typing.Any]]],
-                tree: typing.Union[Node, typing.Dict[str, typing.Any]],
-                version: builtins.str,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__e4ca501b1eec315a1be7b939f76d554171e56023ac6ebe0df98f41720cf7732d)
             check_type(argname="argument edges", value=edges, expected_type=type_hints["edges"])
             check_type(argname="argument tree", value=tree, expected_type=type_hints["tree"])
             check_type(argname="argument version", value=version, expected_type=type_hints["version"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "edges": edges,
             "tree": tree,
             "version": version,
         }
 
     @builtins.property
     def edges(self) -> typing.List[Edge]:
@@ -577,24 +523,24 @@
     },
 )
 class Node(Entity):
     def __init__(
         self,
         *,
         uuid: builtins.str,
-        attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
+        attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union["PlainObject", typing.Dict[builtins.str, typing.Any]]]]]]] = None,
         flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-        metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-        tags: typing.Optional[typing.Union["Tags", typing.Dict[str, typing.Any]]] = None,
+        metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         id: builtins.str,
         node_type: _NodeTypeEnum_d56eed04,
         path: builtins.str,
         cfn_type: typing.Optional[builtins.str] = None,
-        children: typing.Optional[typing.Mapping[builtins.str, typing.Union["Node", typing.Dict[str, typing.Any]]]] = None,
-        construct_info: typing.Optional[typing.Union[_ConstructInfo_e912d4bb, typing.Dict[str, typing.Any]]] = None,
+        children: typing.Optional[typing.Mapping[builtins.str, typing.Union["Node", typing.Dict[builtins.str, typing.Any]]]] = None,
+        construct_info: typing.Optional[typing.Union[_ConstructInfo_e912d4bb, typing.Dict[builtins.str, typing.Any]]] = None,
         edges: typing.Optional[typing.Sequence[builtins.str]] = None,
         logical_id: typing.Optional[builtins.str] = None,
         parent: typing.Optional[builtins.str] = None,
         stack: typing.Optional[builtins.str] = None,
     ) -> None:
         '''(experimental) Serializable graph node entity.
 
@@ -612,41 +558,18 @@
         :param edges: (experimental) List of edge UUIDs where this node is the **source**.
         :param logical_id: (experimental) Logical id of the node, which is only unique within containing stack.
         :param parent: (experimental) UUID of node parent.
         :param stack: (experimental) UUID of node stack.
 
         :stability: experimental
         '''
-        if isinstance(attributes, dict):
-            attributes = Attributes(**attributes)
-        if isinstance(tags, dict):
-            tags = Tags(**tags)
         if isinstance(construct_info, dict):
             construct_info = _ConstructInfo_e912d4bb(**construct_info)
         if __debug__:
-            def stub(
-                *,
-                uuid: builtins.str,
-                attributes: typing.Optional[typing.Union[Attributes, typing.Dict[str, typing.Any]]] = None,
-                flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
-                metadata: typing.Optional[typing.Sequence[typing.Union[constructs.MetadataEntry, typing.Dict[str, typing.Any]]]] = None,
-                tags: typing.Optional[typing.Union[Tags, typing.Dict[str, typing.Any]]] = None,
-                id: builtins.str,
-                node_type: _NodeTypeEnum_d56eed04,
-                path: builtins.str,
-                cfn_type: typing.Optional[builtins.str] = None,
-                children: typing.Optional[typing.Mapping[builtins.str, typing.Union[Node, typing.Dict[str, typing.Any]]]] = None,
-                construct_info: typing.Optional[typing.Union[_ConstructInfo_e912d4bb, typing.Dict[str, typing.Any]]] = None,
-                edges: typing.Optional[typing.Sequence[builtins.str]] = None,
-                logical_id: typing.Optional[builtins.str] = None,
-                parent: typing.Optional[builtins.str] = None,
-                stack: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__8eb3630d79e99f0ae81184cf2ff8774c192cbdb5151e011c14f7204b530f2fdf)
             check_type(argname="argument uuid", value=uuid, expected_type=type_hints["uuid"])
             check_type(argname="argument attributes", value=attributes, expected_type=type_hints["attributes"])
             check_type(argname="argument flags", value=flags, expected_type=type_hints["flags"])
             check_type(argname="argument metadata", value=metadata, expected_type=type_hints["metadata"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument node_type", value=node_type, expected_type=type_hints["node_type"])
@@ -654,15 +577,15 @@
             check_type(argname="argument cfn_type", value=cfn_type, expected_type=type_hints["cfn_type"])
             check_type(argname="argument children", value=children, expected_type=type_hints["children"])
             check_type(argname="argument construct_info", value=construct_info, expected_type=type_hints["construct_info"])
             check_type(argname="argument edges", value=edges, expected_type=type_hints["edges"])
             check_type(argname="argument logical_id", value=logical_id, expected_type=type_hints["logical_id"])
             check_type(argname="argument parent", value=parent, expected_type=type_hints["parent"])
             check_type(argname="argument stack", value=stack, expected_type=type_hints["stack"])
-        self._values: typing.Dict[str, typing.Any] = {
+        self._values: typing.Dict[builtins.str, typing.Any] = {
             "uuid": uuid,
             "id": id,
             "node_type": node_type,
             "path": path,
         }
         if attributes is not None:
             self._values["attributes"] = attributes
@@ -694,52 +617,56 @@
         :stability: experimental
         '''
         result = self._values.get("uuid")
         assert result is not None, "Required property 'uuid' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
-    def attributes(self) -> typing.Optional[Attributes]:
+    def attributes(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]]:
         '''(experimental) Serializable entity attributes.
 
-        :see: {@link Attributes}
+        :see: {@link Attributes }
         :stability: experimental
         '''
         result = self._values.get("attributes")
-        return typing.cast(typing.Optional[Attributes], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject", typing.List[typing.Union[builtins.str, jsii.Number, builtins.bool, "PlainObject"]]]]], result)
 
     @builtins.property
     def flags(self) -> typing.Optional[typing.List[_FlagEnum_af90e158]]:
         '''(experimental) Serializable entity flags.
 
-        :see: {@link FlagEnum}
+        :see: {@link FlagEnum }
         :stability: experimental
         '''
         result = self._values.get("flags")
         return typing.cast(typing.Optional[typing.List[_FlagEnum_af90e158]], result)
 
     @builtins.property
-    def metadata(self) -> typing.Optional[typing.List[constructs.MetadataEntry]]:
+    def metadata(
+        self,
+    ) -> typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]]:
         '''(experimental) Serializable entity metadata.
 
-        :see: {@link Metadata}
+        :see: {@link Metadata }
         :stability: experimental
         '''
         result = self._values.get("metadata")
-        return typing.cast(typing.Optional[typing.List[constructs.MetadataEntry]], result)
+        return typing.cast(typing.Optional[typing.List[_constructs_77d1e7e8.MetadataEntry]], result)
 
     @builtins.property
-    def tags(self) -> typing.Optional["Tags"]:
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''(experimental) Serializable entity tags.
 
-        :see: {@link Tags}
+        :see: {@link Tags }
         :stability: experimental
         '''
         result = self._values.get("tags")
-        return typing.cast(typing.Optional["Tags"], result)
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def id(self) -> builtins.str:
         '''(experimental) Node id within parent (unique only between parent child nodes).
 
         :stability: experimental
         '''
@@ -849,61 +776,90 @@
 )
 class PlainObject:
     def __init__(self) -> None:
         '''(experimental) Serializable plain object value (JSII supported).
 
         :stability: experimental
         '''
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
         return "PlainObject(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-@jsii.data_type(
-    jsii_type="@aws-prototyping-sdk/cdk-graph.SerializedGraph.Tags",
-    jsii_struct_bases=[],
-    name_mapping={},
-)
-class Tags:
-    def __init__(self) -> None:
-        '''(experimental) Serializable dictionary of tags (key value pairs).
-
-        :stability: experimental
-        '''
-        self._values: typing.Dict[str, typing.Any] = {}
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "Tags(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
 __all__ = [
-    "Attributes",
     "Edge",
     "Entity",
     "GraphStore",
     "ISerializableEdge",
     "ISerializableEntity",
     "ISerializableGraphStore",
     "ISerializableNode",
     "Node",
     "PlainObject",
-    "Tags",
 ]
 
 publication.publish()
+
+def _typecheckingstub__0df02c65dc4810873a004e52f214df46ce43efc61f582498a0f1af1abd6f2f7d(
+    *,
+    uuid: builtins.str,
+    attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]]]]]]] = None,
+    flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
+    metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    direction: _EdgeDirectionEnum_26ef4ba3,
+    edge_type: _EdgeTypeEnum_1b13d7ee,
+    source: builtins.str,
+    target: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__54acd3ac36d2232ab6ff52b62125889be84254bc3d141b1d2f66b7fc481a4ca6(
+    *,
+    uuid: builtins.str,
+    attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]]]]]]] = None,
+    flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
+    metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e4ca501b1eec315a1be7b939f76d554171e56023ac6ebe0df98f41720cf7732d(
+    *,
+    edges: typing.Sequence[typing.Union[Edge, typing.Dict[builtins.str, typing.Any]]],
+    tree: typing.Union[Node, typing.Dict[builtins.str, typing.Any]],
+    version: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8eb3630d79e99f0ae81184cf2ff8774c192cbdb5151e011c14f7204b530f2fdf(
+    *,
+    uuid: builtins.str,
+    attributes: typing.Optional[typing.Mapping[builtins.str, typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]], typing.Sequence[typing.Union[builtins.str, jsii.Number, builtins.bool, typing.Union[PlainObject, typing.Dict[builtins.str, typing.Any]]]]]]] = None,
+    flags: typing.Optional[typing.Sequence[_FlagEnum_af90e158]] = None,
+    metadata: typing.Optional[typing.Sequence[typing.Union[_constructs_77d1e7e8.MetadataEntry, typing.Dict[builtins.str, typing.Any]]]] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    id: builtins.str,
+    node_type: _NodeTypeEnum_d56eed04,
+    path: builtins.str,
+    cfn_type: typing.Optional[builtins.str] = None,
+    children: typing.Optional[typing.Mapping[builtins.str, typing.Union[Node, typing.Dict[builtins.str, typing.Any]]]] = None,
+    construct_info: typing.Optional[typing.Union[_ConstructInfo_e912d4bb, typing.Dict[builtins.str, typing.Any]]] = None,
+    edges: typing.Optional[typing.Sequence[builtins.str]] = None,
+    logical_id: typing.Optional[builtins.str] = None,
+    parent: typing.Optional[builtins.str] = None,
+    stack: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO` & `aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-prototyping-sdk.cdk-graph
-Version: 0.12.26
+Version: 0.19.56
 Summary: @aws-prototyping-sdk/cdk-graph
 Home-page: https://github.com/aws/aws-prototyping-sdk
 Author: AWS APJ COPE<apj-cope@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/aws/aws-prototyping-sdk
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -280,9 +280,7 @@
 * [ ] Find alternative synthesis solution that doesn't utilize CDK internals
 * [ ] Support custom Nodes and Edges
 * [ ] Improve logging, bookkeeping, and debugging
 * [ ] Implement store upgrade solution
 * [ ] Battle test the implementation against several plugins
 * [ ] Battle test the implementation in all target languages (currently tested in Typescript, but vended in all PDK supported languages)
 * [ ] Receive community feedback to validate approach
-
-
```

### Comparing `aws_prototyping_sdk.cdk_graph-0.12.26/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt` & `aws_prototyping_sdk.cdk_graph-0.19.56/src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/aws_prototyping_sdk.cdk_graph.egg-info/SOURCES.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/dependency_links.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/requires.txt
 src/aws_prototyping_sdk.cdk_graph.egg-info/top_level.txt
 src/aws_prototyping_sdk/cdk_graph/__init__.py
 src/aws_prototyping_sdk/cdk_graph/py.typed
 src/aws_prototyping_sdk/cdk_graph/_jsii/__init__.py
-src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.12.26.jsii.tgz
+src/aws_prototyping_sdk/cdk_graph/_jsii/cdk-graph@0.19.56.jsii.tgz
 src/aws_prototyping_sdk/cdk_graph/graph/__init__.py
 src/aws_prototyping_sdk/cdk_graph/serialized_graph/__init__.py
```

