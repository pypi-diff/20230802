# Comparing `tmp/zuko-0.2.2.tar.gz` & `tmp/zuko-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zuko-0.2.2.tar", last modified: Thu Jul 13 20:54:20 2023, max compression
+gzip compressed data, was "zuko-0.3.0.tar", last modified: Wed Aug  2 20:01:55 2023, max compression
```

## Comparing `zuko-0.2.2.tar` & `zuko-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.2.2/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     4779 2023-07-13 20:54:20.248591 zuko-0.2.2/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     4050 2023-07-09 10:11:29.000000 zuko-0.2.2/README.md
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-09 09:28:21.000000 zuko-0.2.2/requirements.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-07-13 20:54:20.248591 zuko-0.2.2/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-07-09 09:28:21.000000 zuko-0.2.2/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.244591 zuko-0.2.2/tests/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2975 2023-07-13 20:10:54.000000 zuko-0.2.2/tests/test_flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     3066 2023-07-09 09:28:21.000000 zuko-0.2.2/tests/test_transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     2792 2023-07-13 11:22:12.000000 zuko-0.2.2/tests/test_utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/zuko/
--rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-07-13 20:13:15.000000 zuko-0.2.2/zuko/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    20798 2023-07-09 09:28:21.000000 zuko-0.2.2/zuko/distributions.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    34260 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/flows.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     9073 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/nn.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    27008 2023-07-13 20:10:54.000000 zuko-0.2.2/zuko/transforms.py
--rw-rw-r--   0 francois  (1001) francois  (1001)    13559 2023-07-13 20:00:04.000000 zuko-0.2.2/zuko/utils.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-13 20:54:20.248591 zuko-0.2.2/zuko.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     4779 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      399 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-07-13 20:54:20.000000 zuko-0.2.2/zuko.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2022-12-13 12:43:25.000000 zuko-0.3.0/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5377 2023-08-02 20:01:55.282693 zuko-0.3.0/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4648 2023-08-02 20:00:36.000000 zuko-0.3.0/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-07-09 09:28:21.000000 zuko-0.3.0/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      823 2023-08-02 20:01:55.282693 zuko-0.3.0/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       72 2023-07-09 09:28:21.000000 zuko-0.3.0/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.278693 zuko-0.3.0/tests/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1550 2023-07-09 09:28:21.000000 zuko-0.3.0/tests/test_distributions.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2966 2023-08-02 20:00:36.000000 zuko-0.3.0/tests/test_flows.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1138 2023-07-09 09:28:21.000000 zuko-0.3.0/tests/test_nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3167 2023-08-02 20:00:36.000000 zuko-0.3.0/tests/test_transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2792 2023-07-13 11:22:12.000000 zuko-0.3.0/tests/test_utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.278693 zuko-0.3.0/zuko/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      177 2023-08-02 20:01:09.000000 zuko-0.3.0/zuko/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    20790 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/distributions.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/zuko/flows/
+-rw-rw-r--   0 francois  (1001) francois  (1001)      273 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     7482 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/autoregressive.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3959 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/continuous.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4057 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/core.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4964 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/coupling.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4199 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/gaussianization.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1989 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/mixture.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9948 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/neural.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1359 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/polynomial.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     3060 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/flows/spline.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     9073 2023-07-13 20:10:54.000000 zuko-0.3.0/zuko/nn.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    28089 2023-08-02 20:00:36.000000 zuko-0.3.0/zuko/transforms.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)    13559 2023-08-01 12:27:42.000000 zuko-0.3.0/zuko/utils.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-08-02 20:01:55.282693 zuko-0.3.0/zuko.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     5377 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      623 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       28 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        5 2023-08-02 20:01:55.000000 zuko-0.3.0/zuko.egg-info/top_level.txt
```

### Comparing `zuko-0.2.2/LICENSE` & `zuko-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/PKG-INFO` & `zuko-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.2.2
+Version: 0.3.0
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -17,17 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
-Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
+Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -63,25 +63,25 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | c*)
 x = flow(c_star).sample((64,))
 ```
 
-Alternatively, flows can be built as custom `FlowModule` objects.
+Alternatively, flows can be built as custom `Flow` objects.
 
 ```python
-from zuko.flows import FlowModule, MaskedAutoregressiveTransform, Unconditional
+from zuko.flows import Flow, MaskedAutoregressiveTransform, Unconditional
 from zuko.distributions import DiagNormal
-from zuko.transforms import PermutationTransform
+from zuko.transforms import RotationTransform
 
-flow = FlowModule(
+flow = Flow(
     transforms=[
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
-        Unconditional(PermutationTransform, torch.randperm(3), buffer=True),
+        Unconditional(RotationTransform, torch.randn(3, 3)),
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
     ],
     base=Unconditional(
         DiagNormal,
         torch.zeros(3),
         torch.ones(3),
         buffer=True,
@@ -91,18 +91,21 @@
 
 For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
+| `GMM`   | -    | [Gaussian Mixture Model](https://wikipedia.org/wiki/Mixture_model#Gaussian_mixture_model) |
+| `NICE`  | 2014 | [Non-linear Independent Components Estimation](https://arxiv.org/abs/1410.8516) |
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
 | `NCSF`  | 2020 | [Normalizing Flows on Tori and Spheres](https://arxiv.org/abs/2002.02428) |
 | `SOSPF` | 2019 | [Sum-of-Squares Polynomial Flow](https://arxiv.org/abs/1905.02325) |
 | `NAF`   | 2018 | [Neural Autoregressive Flows](https://arxiv.org/abs/1804.00779) |
 | `UNAF`  | 2019 | [Unconstrained Monotonic Neural Networks](https://arxiv.org/abs/1908.05164) |
 | `CNF`   | 2018 | [Neural Ordinary Differential Equations](https://arxiv.org/abs/1806.07366) |
+| `GF`    | 2020 | [Gaussianization Flows](https://arxiv.org/abs/2003.01941) |
 
 ## Contributing
 
 If you have a question, an issue or would like to contribute, please read our [contributing guidelines](https://github.com/francois-rozet/zuko/blob/master/CONTRIBUTING.md).
```

### Comparing `zuko-0.2.2/README.md` & `zuko-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
-Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
+Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -44,25 +44,25 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | c*)
 x = flow(c_star).sample((64,))
 ```
 
-Alternatively, flows can be built as custom `FlowModule` objects.
+Alternatively, flows can be built as custom `Flow` objects.
 
 ```python
-from zuko.flows import FlowModule, MaskedAutoregressiveTransform, Unconditional
+from zuko.flows import Flow, MaskedAutoregressiveTransform, Unconditional
 from zuko.distributions import DiagNormal
-from zuko.transforms import PermutationTransform
+from zuko.transforms import RotationTransform
 
-flow = FlowModule(
+flow = Flow(
     transforms=[
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
-        Unconditional(PermutationTransform, torch.randperm(3), buffer=True),
+        Unconditional(RotationTransform, torch.randn(3, 3)),
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
     ],
     base=Unconditional(
         DiagNormal,
         torch.zeros(3),
         torch.ones(3),
         buffer=True,
@@ -72,18 +72,21 @@
 
 For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
+| `GMM`   | -    | [Gaussian Mixture Model](https://wikipedia.org/wiki/Mixture_model#Gaussian_mixture_model) |
+| `NICE`  | 2014 | [Non-linear Independent Components Estimation](https://arxiv.org/abs/1410.8516) |
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
 | `NCSF`  | 2020 | [Normalizing Flows on Tori and Spheres](https://arxiv.org/abs/2002.02428) |
 | `SOSPF` | 2019 | [Sum-of-Squares Polynomial Flow](https://arxiv.org/abs/1905.02325) |
 | `NAF`   | 2018 | [Neural Autoregressive Flows](https://arxiv.org/abs/1804.00779) |
 | `UNAF`  | 2019 | [Unconstrained Monotonic Neural Networks](https://arxiv.org/abs/1908.05164) |
 | `CNF`   | 2018 | [Neural Ordinary Differential Equations](https://arxiv.org/abs/1806.07366) |
+| `GF`    | 2020 | [Gaussianization Flows](https://arxiv.org/abs/2003.01941) |
 
 ## Contributing
 
 If you have a question, an issue or would like to contribute, please read our [contributing guidelines](https://github.com/francois-rozet/zuko/blob/master/CONTRIBUTING.md).
```

### Comparing `zuko-0.2.2/setup.cfg` & `zuko-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/tests/test_distributions.py` & `zuko-0.3.0/tests/test_distributions.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/tests/test_flows.py` & `zuko-0.3.0/tests/test_flows.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,117 +4,123 @@
 import torch
 
 from functools import partial
 from torch import randn
 from zuko.flows import *
 
 
+torch.set_default_dtype(torch.float64)
+
+
 def test_flows(tmp_path):
-    flows = [
-        GMM(3, 5),
-        MAF(3, 5),
-        NSF(3, 5),
-        SOSPF(3, 5),
-        NAF(3, 5),
-        UNAF(3, 5),
-        GCF(3, 5),
-        CNF(3, 5),
+    Fs = [
+        GMM,
+        NICE,
+        MAF,
+        NSF,
+        SOSPF,
+        NAF,
+        UNAF,
+        CNF,
+        GF,
     ]
 
-    for flow in flows:
+    for F in Fs:
+        flow = F(3, 5)
+
         # Evaluation of log_prob
         x, c = randn(256, 3), randn(5)
         log_p = flow(c).log_prob(x)
 
-        assert log_p.shape == (256,), flow
-        assert log_p.requires_grad, flow
+        assert log_p.shape == (256,), F
+        assert log_p.requires_grad, F
 
         flow.zero_grad(set_to_none=True)
         loss = -log_p.mean()
         loss.backward()
 
         for p in flow.parameters():
-            assert p.grad is not None, flow
+            assert p.grad is not None, F
 
         # Sampling
         x = flow(c).sample((32,))
 
-        assert x.shape == (32, 3), flow
+        assert x.shape == (32, 3), F
 
         # Reparameterization trick
         if flow(c).has_rsample:
             x = flow(c).rsample()
 
             flow.zero_grad(set_to_none=True)
             loss = x.square().sum().sqrt()
             loss.backward()
 
             for p in flow.parameters():
-                assert p.grad is not None, flow
+                assert p.grad is not None, F
 
         # Invertibility
-        if isinstance(flow, FlowModule):
+        if isinstance(flow, Flow):
             x, c = randn(256, 3), randn(256, 5)
             t = flow(c).transform
             z = t.inv(t(x))
 
-            assert torch.allclose(x, z, atol=1e-4), flow
+            assert torch.allclose(x, z, atol=1e-4), F
 
         # Saving
         torch.save(flow, tmp_path / 'flow.pth')
 
         # Loading
         flow_bis = torch.load(tmp_path / 'flow.pth')
 
         x, c = randn(3), randn(5)
 
         seed = torch.seed()
         log_p = flow(c).log_prob(x)
         torch.manual_seed(seed)
         log_p_bis = flow_bis(c).log_prob(x)
 
-        assert torch.allclose(log_p, log_p_bis), flow
+        assert torch.allclose(log_p, log_p_bis), F
 
         # Printing
-        assert repr(flow), flow
+        assert repr(flow), F
 
 
 def test_triangular_transforms():
     Ts = [
         ElementWiseTransform,
+        GeneralCouplingTransform,
         MaskedAutoregressiveTransform,
         partial(MaskedAutoregressiveTransform, passes=2),
         NeuralAutoregressiveTransform,
         partial(NeuralAutoregressiveTransform, passes=2),
         UnconstrainedNeuralAutoregressiveTransform,
-        GeneralCouplingTransform,
     ]
 
     for T in Ts:
         # Without context
         t = T(3)
         x = randn(3)
         y = t()(x)
 
         assert y.shape == x.shape, t
         assert y.requires_grad, t
-        assert torch.allclose(t().inv(y), x, atol=1e-4), t
+        assert torch.allclose(t().inv(y), x, atol=1e-4), T
 
         # With context
         t = T(3, 5)
         x, c = randn(256, 3), randn(5)
         y = t(c)(x)
 
-        assert y.shape == x.shape, t
-        assert y.requires_grad, t
-        assert torch.allclose(t(c).inv(y), x, atol=1e-4), t
+        assert y.shape == x.shape, T
+        assert y.requires_grad, T
+        assert torch.allclose(t(c).inv(y), x, atol=1e-4), T
 
         # Jacobian
         t = T(7)
         x = randn(7)
         y = t()(x)
 
         J = torch.autograd.functional.jacobian(t(), x)
         ladj = torch.linalg.slogdet(J).logabsdet
 
-        assert torch.allclose(t().log_abs_det_jacobian(x, y), ladj, atol=1e-4), t
-        assert torch.allclose(J.diag().abs().log().sum(), ladj, atol=1e-4), t
+        assert torch.allclose(t().log_abs_det_jacobian(x, y), ladj, atol=1e-4), T
+        assert torch.allclose(J.diag().abs().log().sum(), ladj, atol=1e-4), T
```

### Comparing `zuko-0.2.2/tests/test_nn.py` & `zuko-0.3.0/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/tests/test_transforms.py` & `zuko-0.3.0/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 import torch
 
 from torch import randn
 from torch.distributions import *
 from zuko.transforms import *
 
 
+torch.set_default_dtype(torch.float64)
+
+
 def test_univariate_transforms():
     ts = [
         IdentityTransform(),
         CosTransform(),
         SinTransform(),
         SoftclipTransform(),
         CircularShiftTransform(),
         MonotonicAffineTransform(randn(256), randn(256)),
         MonotonicRQSTransform(randn(256, 8), randn(256, 8), randn(256, 7)),
         MonotonicTransform(lambda x: x**3),
+        GaussianizationTransform(randn(256, 8), randn(256, 8)),
         UnconstrainedMonotonicTransform(lambda x: torch.exp(-x**2) + 1e-2, randn(256)),
         SOSPolynomialTransform(randn(256, 2, 4), randn(256)),
     ]
 
     for t in ts:
         # Call
         if hasattr(t.domain, 'lower_bound'):
             x = torch.linspace(t.domain.lower_bound + 1e-2, t.domain.upper_bound - 1e-2, 256)
         else:
-            x = torch.linspace(-4.999, 4.999, 256)
+            x = torch.linspace(-5.0, 5.0, 256)
 
         y = t(x)
 
         assert x.shape == y.shape, t
 
         # Inverse
         z = t.inv(y)
@@ -67,16 +71,16 @@
 
 def test_multivariate_transforms():
     A, B = torch.randn(5, 16), torch.randn(16, 5)
     f = lambda t, x: torch.sigmoid(x @ A) @ B
 
     ts = [
         FreeFormJacobianTransform(f, 0.0, 1.0),
-        LULinearTransform(randn(5, 5)),
         PermutationTransform(torch.randperm(5)),
+        RotationTransform(randn(5, 5)),
     ]
 
     for t in ts:
         # Shapes
         x = randn(256, 5)
         y = t(x)
```

### Comparing `zuko-0.2.2/tests/test_utils.py` & `zuko-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/zuko/distributions.py` & `zuko-0.3.0/zuko/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,15 +479,15 @@
     def cdf(self, x: Tensor) -> Tensor:
         return self.uniform.cdf(self.base.cdf(x))
 
     def log_prob(self, x: Tensor) -> Tensor:
         return self.uniform.log_prob(self.base.cdf(x)) + self.base.log_prob(x)
 
     def rsample(self, shape: Size = ()) -> Tensor:
-        return self.base.icdf(torch.clip(self.uniform.rsample(shape), 1e-6, 1 - 1e-6))
+        return self.base.icdf((1 - 2e-6) * self.uniform.rsample(shape) + 1e-6)
 
 
 class Sort(Distribution):
     r"""Creates a distribution for a :math:`n`-d random variable :math:`X`, whose elements
     :math:`X_i` are :math:`n` draws from a base distribution :math:`p(Z)`, ordered
     such that :math:`X_i \leq X_{i + 1}`.
```

### Comparing `zuko-0.2.2/zuko/nn.py` & `zuko-0.3.0/zuko/nn.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/zuko/transforms.py` & `zuko-0.3.0/zuko/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,31 @@
     'CosTransform',
     'SinTransform',
     'SoftclipTransform',
     'CircularShiftTransform',
     'MonotonicAffineTransform',
     'MonotonicRQSTransform',
     'MonotonicTransform',
+    'GaussianizationTransform',
     'UnconstrainedMonotonicTransform',
     'SOSPolynomialTransform',
-    'FreeFormJacobianTransform',
     'AutoregressiveTransform',
     'CouplingTransform',
-    'LULinearTransform',
+    'FreeFormJacobianTransform',
     'PermutationTransform',
+    'RotationTransform',
 ]
 
 import math
 import torch
 import torch.nn.functional as F
 
 from textwrap import indent
 from torch import Tensor, BoolTensor, LongTensor, Size
-from torch.distributions import *
+from torch.distributions import Transform
 from torch.distributions import constraints
 from torch.distributions.utils import _sum_rightmost
 from typing import *
 
 from .utils import bisection, broadcast, gauss_legendre, odeint
 
 
@@ -283,23 +284,23 @@
 
     .. math:: f(x) = \frac{x}{1 + \left| \frac{x}{B} \right|}
 
     Arguments:
         bound: The codomain bound :math:`B`.
     """
 
-    domain = constraints.real
-    codomain = constraints.real
     bijective = True
     sign = +1
 
-    def __init__(self, bound: float = 5.0, **kwargs):
+    def __init__(self, bound: float = 1.0, **kwargs):
         super().__init__(**kwargs)
 
         self.bound = bound
+        self.domain = constraints.real
+        self.codomain = constraints.interval(-bound, bound)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(bound={self.bound})'
 
     def _call(self, x: Tensor) -> Tensor:
         return x / (1 + abs(x / self.bound))
 
@@ -319,22 +320,22 @@
         This transformation is only bijective over its domain :math:`[-B, B]` as
         :math:`f(x) = f(x + 2kB)` for all :math:`k \in \mathbb{Z}`.
 
     Arguments:
         bound: The domain bound :math:`B`.
     """
 
-    domain = constraints.real
-    codomain = constraints.real
     bijective = True
 
-    def __init__(self, bound: float = 5.0, **kwargs):
+    def __init__(self, bound: float = 1.0, **kwargs):
         super().__init__(**kwargs)
 
         self.bound = bound
+        self.domain = constraints.interval(-bound, bound)
+        self.codomain = constraints.interval(-bound, bound)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(bound={self.bound})'
 
     def _call(self, x: Tensor) -> Tensor:
         return torch.remainder(x, 2 * self.bound) - self.bound
 
@@ -342,19 +343,19 @@
         return torch.remainder(y, 2 * self.bound) - self.bound
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
         return torch.zeros_like(x)
 
 
 class MonotonicAffineTransform(Transform):
-    r"""Creates a transformation :math:`f(x) = \alpha x + \beta`.
+    r"""Creates a transformation :math:`f(x) = \exp(a) x + b`.
 
     Arguments:
-        shift: The shift term :math:`\beta`, with shape :math:`(*,)`.
-        scale: The unconstrained scale factor :math:`\alpha`, with shape :math:`(*,)`.
+        shift: The shift term :math:`b`, with shape :math:`(*,)`.
+        scale: The unconstrained scale factor :math:`a`, with shape :math:`(*,)`.
         slope: The minimum slope of the transformation.
     """
 
     domain = constraints.real
     codomain = constraints.real
     bijective = True
     sign = +1
@@ -413,21 +414,21 @@
     ):
         super().__init__(**kwargs)
 
         widths = widths / (1 + abs(2 * widths / math.log(slope)))
         heights = heights / (1 + abs(2 * heights / math.log(slope)))
         derivatives = derivatives / (1 + abs(derivatives / math.log(slope)))
 
-        widths = 2 * F.softmax(widths, dim=-1)
-        heights = 2 * F.softmax(heights, dim=-1)
-        derivatives = derivatives.exp()
-
-        self.horizontal = bound * torch.cumsum(F.pad(widths, (1, 0), value=-1), dim=-1)
-        self.vertical = bound * torch.cumsum(F.pad(heights, (1, 0), value=-1), dim=-1)
-        self.derivatives = F.pad(derivatives, (1, 1), value=1)
+        widths = F.pad(F.softmax(widths, dim=-1), (1, 0), value=0)
+        heights = F.pad(F.softmax(heights, dim=-1), (1, 0), value=0)
+        derivatives = F.pad(derivatives, (1, 1), value=0)
+
+        self.horizontal = bound * (2 * torch.cumsum(widths, dim=-1) - 1)
+        self.vertical = bound * (2 * torch.cumsum(heights, dim=-1) - 1)
+        self.derivatives = torch.exp(derivatives)
 
     def __repr__(self) -> str:
         return f'{self.__class__.__name__}(bins={self.bins})'
 
     @property
     def bins(self) -> int:
         return self.horizontal.shape[-1] - 1
@@ -526,15 +527,15 @@
     bijective = True
     sign = +1
 
     def __init__(
         self,
         f: Callable[[Tensor], Tensor],
         phi: Iterable[Tensor] = (),
-        bound: float = 5.0,
+        bound: float = 10.0,
         eps: float = 1e-6,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.f = f
         self.phi = tuple(filter(lambda p: p.requires_grad, phi))
@@ -556,22 +557,66 @@
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
         _, ladj = self.call_and_ladj(x)
         return ladj
 
     def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
         with torch.enable_grad():
-            x = x.requires_grad_()
+            x = x.view_as(x).requires_grad_()  # shallow copy
             y = self.f(x)
 
         jacobian = torch.autograd.grad(y, x, torch.ones_like(y), create_graph=True)[0]
 
         return y, jacobian.log()
 
 
+class GaussianizationTransform(MonotonicTransform):
+    r"""Creates a gaussianization transformation.
+
+    .. math:: f(x) = \Phi^{-1}
+        \left( \frac{1}{K} \sum_{i=1}^K \Phi(\exp(a_i) x + b_i) \right)
+
+    where :math:`\Phi` is the cumulative distribution function (CDF) of the standard
+    normal :math:`\mathcal{N}(0, 1)`.
+
+    References:
+        | Gaussianization (Chen et al., 2000)
+        | https://papers.nips.cc/paper/1856-gaussianization
+
+    Arguments:
+        shift: The shift terms :math:`b`, with shape :math:`(*, K)`.
+        scale: The unconstrained scale factors :math:`a`, with shape :math:`(*, K)`.
+        kwargs: Keyword arguments passed to :class:`MonotonicTransform`.
+    """
+
+    domain = constraints.real
+    codomain = constraints.real
+    bijective = True
+    sign = +1
+
+    def __init__(
+        self,
+        shift: Tensor,
+        scale: Tensor,
+        **kwargs,
+    ):
+        super().__init__(self.f, phi=(shift, scale), **kwargs)
+
+        self.shift = shift
+        self.scale = torch.exp(scale)
+
+    def f(self, x: Tensor) -> Tensor:
+        x = x[..., None] * self.scale + self.shift
+        x = torch.erf(x / math.sqrt(2))
+        x = torch.mean(x, dim=-1) * (1 - 1e-6)
+        x = torch.erfinv(x) * math.sqrt(2)
+
+        return x
+
+
 class UnconstrainedMonotonicTransform(MonotonicTransform):
     r"""Creates a monotonic transformation :math:`f(x)` by integrating a positive
     univariate function :math:`g(x)`.
 
     .. math:: f(x) = \int_0^x g(u) ~ du + C
 
     The definite integral is estimated by a :math:`n`-point Gauss-Legendre quadrature.
@@ -619,15 +664,15 @@
 
 class SOSPolynomialTransform(UnconstrainedMonotonicTransform):
     r"""Creates a sum-of-squares (SOS) polynomial transformation.
 
     The transformation :math:`f(x)` is expressed as the primitive integral of the
     sum of :math:`K` squared polynomials of degree :math:`L`.
 
-    .. math:: f(x) = \int_0^x \sum_{i = 1}^K
+    .. math:: f(x) = \int_0^x \frac{1}{K} \sum_{i = 1}^K
         \left( 1 + \sum_{j = 0}^L a_{i,j} ~ u^j \right)^2 ~ du + C
 
     References:
         | Sum-of-Squares Polynomial Flow (Jaini et al., 2019)
         | https://arxiv.org/abs/1905.02325
 
     Arguments:
@@ -648,114 +693,24 @@
         self.i = torch.arange(a.shape[-1]).to(a.device)
 
     def g(self, x: Tensor) -> Tensor:
         x = x / self.bound
         x = x[..., None] ** self.i
         p = 1 + self.a @ x[..., None]
 
-        return p.squeeze(dim=-1).square().sum(dim=-1)
-
-
-class FreeFormJacobianTransform(Transform):
-    r"""Creates a free-form Jacobian transformation.
-
-    The transformation is the integration of a system of first-order ordinary
-    differential equations
-
-    .. math:: x(t_1) = x_0 + \int_{t_0}^{t_1} f_\phi(t, x(t)) ~ dt .
-
-    References:
-        | FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl et al., 2018)
-        | https://arxiv.org/abs/1810.01367
-
-    Arguments:
-        f: A system of first-order ODEs :math:`f_\phi`.
-        t0: The initial integration time :math:`t_0`.
-        t1: The final integration time :math:`t_1`.
-        phi: The parameters :math:`\phi` of :math:`f_\phi`.
-        exact: Whether the exact log-determinant of the Jacobian or an unbiased
-            stochastic estimate thereof is calculated.
-    """
-
-    domain = constraints.real_vector
-    codomain = constraints.real_vector
-    bijective = True
-
-    def __init__(
-        self,
-        f: Callable[[Tensor, Tensor], Tensor],
-        t0: Union[float, Tensor] = 0.0,
-        t1: Union[float, Tensor] = 1.0,
-        phi: Iterable[Tensor] = (),
-        exact: bool = True,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-
-        self.f = f
-        self.t0 = t0
-        self.t1 = t1
-        self.phi = tuple(filter(lambda p: p.requires_grad, phi))
-        self.exact = exact
-        self.trace_scale = 1e-2  # relax jacobian tolerances
-
-    def _call(self, x: Tensor) -> Tensor:
-        return odeint(self.f, x, self.t0, self.t1, self.phi)
-
-    @property
-    def inv(self) -> Transform:
-        return FreeFormJacobianTransform(
-            f=self.f,
-            t0=self.t1,
-            t1=self.t0,
-            phi=self.phi,
-            exact=self.exact,
-        )
-
-    def _inverse(self, y: Tensor) -> Tensor:
-        return odeint(self.f, y, self.t1, self.t0, self.phi)
-
-    def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
-        _, ladj = self.call_and_ladj(x)
-        return ladj
-
-    def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
-        if self.exact:
-            I = torch.eye(x.shape[-1], dtype=x.dtype, device=x.device)
-            I = I.expand(*x.shape, x.shape[-1]).movedim(-1, 0)
-        else:
-            eps = torch.randn_like(x)
-
-        def f_aug(t: Tensor, x: Tensor, ladj: Tensor) -> Tensor:
-            with torch.enable_grad():
-                x = x.requires_grad_()
-                dx = self.f(t, x)
-
-            if self.exact:
-                jacobian = torch.autograd.grad(dx, x, I, create_graph=True, is_grads_batched=True)[0]
-                trace = torch.einsum('i...i', jacobian)
-            else:
-                epsjp = torch.autograd.grad(dx, x, eps, create_graph=True)[0]
-                trace = (epsjp * eps).sum(dim=-1)
-
-            return dx, trace * self.trace_scale
-
-        ladj = torch.zeros_like(x[..., 0])
-        y, ladj = odeint(f_aug, (x, ladj), self.t0, self.t1, self.phi)
-
-        return y, ladj * (1 / self.trace_scale)
+        return p.squeeze(dim=-1).square().mean(dim=-1)
 
 
 class AutoregressiveTransform(Transform):
     r"""Transform via an autoregressive scheme.
 
-    .. math:: y_i = f(x_i; x_{<i})
+    .. math:: y_i = f(x_i | x_{<i})
 
     Arguments:
-        meta: A meta function which returns a transformation :math:`f`.
+        meta: A function which returns a transformation :math:`f` given :math:`x`.
         passes: The number of passes for the inverse transformation.
     """
 
     domain = constraints.real_vector
     codomain = constraints.real_vector
     bijective = True
 
@@ -789,19 +744,19 @@
 
 
 class CouplingTransform(Transform):
     r"""Transform via a coupling scheme.
 
     .. math::
         y_a & = x_a \\
-        y_b & = f(x_b; x_a)
+        y_b & = f(x_b | x_a)
 
     Arguments:
-        meta: A meta function which returns a transformation :math:`f`.
-        mask: A coupling mask defining the split $x \mapsto (x_a, x_b)$.
+        meta: A function which returns a transformation :math:`f` given :math:`x_a`.
+        mask: A coupling mask defining the split :math:`x \to (x_a, x_b)`.
     """
 
     domain = constraints.real_vector
     codomain = constraints.real_vector
     bijective = True
 
     def __init__(
@@ -848,52 +803,102 @@
         x_a, x_b = self.split(x)
         y_b, ladj = self.meta(x_a).call_and_ladj(x_b)
         y = self.merge(x_a, y_b, x.shape)
 
         return y, ladj
 
 
-class LULinearTransform(Transform):
-    r"""Creates a transformation :math:`f(x) = L U x`.
+class FreeFormJacobianTransform(Transform):
+    r"""Creates a free-form Jacobian transformation.
+
+    The transformation is the integration of a system of first-order ordinary
+    differential equations
+
+    .. math:: x(t_1) = x_0 + \int_{t_0}^{t_1} f_\phi(t, x(t)) ~ dt .
+
+    References:
+        | FFJORD: Free-form Continuous Dynamics for Scalable Reversible Generative Models (Grathwohl et al., 2018)
+        | https://arxiv.org/abs/1810.01367
 
     Arguments:
-        LU: A matrix whose lower and upper triangular parts are the non-zero elements
-            of :math:`L` and :math:`U`, with shape :math:`(*, D, D)`.
+        f: A system of first-order ODEs :math:`f_\phi`.
+        t0: The initial integration time :math:`t_0`.
+        t1: The final integration time :math:`t_1`.
+        phi: The parameters :math:`\phi` of :math:`f_\phi`.
+        exact: Whether the exact log-determinant of the Jacobian or an unbiased
+            stochastic estimate thereof is calculated.
     """
 
     domain = constraints.real_vector
     codomain = constraints.real_vector
     bijective = True
 
-    def __init__(self, LU: Tensor, **kwargs):
+    def __init__(
+        self,
+        f: Callable[[Tensor, Tensor], Tensor],
+        t0: Union[float, Tensor] = 0.0,
+        t1: Union[float, Tensor] = 1.0,
+        phi: Iterable[Tensor] = (),
+        exact: bool = True,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
 
-        I = torch.eye(LU.shape[-1], dtype=LU.dtype, device=LU.device)
-
-        self.L = torch.tril(LU, diagonal=-1) + I
-        self.U = torch.triu(LU, diagonal=+1) + I
+        self.f = f
+        self.t0 = t0
+        self.t1 = t1
+        self.phi = tuple(filter(lambda p: p.requires_grad, phi))
+        self.exact = exact
+        self.trace_scale = 1e-2  # relax jacobian tolerances
 
     def _call(self, x: Tensor) -> Tensor:
-        return (self.L @ self.U @ x.unsqueeze(-1)).squeeze(-1)
+        return odeint(self.f, x, self.t0, self.t1, self.phi)
+
+    @property
+    def inv(self) -> Transform:
+        return FreeFormJacobianTransform(
+            f=self.f,
+            t0=self.t1,
+            t1=self.t0,
+            phi=self.phi,
+            exact=self.exact,
+        )
 
     def _inverse(self, y: Tensor) -> Tensor:
-        return torch.linalg.solve_triangular(
-            self.U,
-            torch.linalg.solve_triangular(
-                self.L,
-                y.unsqueeze(-1),
-                upper=False,
-                unitriangular=True,
-            ),
-            upper=True,
-            unitriangular=True,
-        ).squeeze(-1)
+        return odeint(self.f, y, self.t1, self.t0, self.phi)
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
-        return x.new_zeros(x.shape[:-1])
+        _, ladj = self.call_and_ladj(x)
+        return ladj
+
+    def call_and_ladj(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+        if self.exact:
+            I = torch.eye(x.shape[-1], dtype=x.dtype, device=x.device)
+            I = I.expand(*x.shape, x.shape[-1]).movedim(-1, 0)
+        else:
+            eps = torch.randn_like(x)
+
+        def f_aug(t: Tensor, x: Tensor, ladj: Tensor) -> Tensor:
+            with torch.enable_grad():
+                x = x.view_as(x).requires_grad_()  # shallow copy
+                dx = self.f(t, x)
+
+            if self.exact:
+                jacobian = torch.autograd.grad(dx, x, I, create_graph=True, is_grads_batched=True)[0]
+                trace = torch.einsum('i...i', jacobian)
+            else:
+                epsjp = torch.autograd.grad(dx, x, eps, create_graph=True)[0]
+                trace = (epsjp * eps).sum(dim=-1)
+
+            return dx, trace * self.trace_scale
+
+        ladj = torch.zeros_like(x[..., 0])
+        y, ladj = odeint(f_aug, (x, ladj), self.t0, self.t1, self.phi)
+
+        return y, ladj * (1 / self.trace_scale)
 
 
 class PermutationTransform(Transform):
     r"""Creates a transformation that permutes the elements.
 
     Arguments:
         order: The permutation order, with shape :math:`(*, D)`.
@@ -921,7 +926,37 @@
         return x[..., self.order]
 
     def _inverse(self, y: Tensor) -> Tensor:
         return y[..., torch.argsort(self.order)]
 
     def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
         return x.new_zeros(x.shape[:-1])
+
+
+class RotationTransform(Transform):
+    r"""Creates a rotation transformation :math:`f(x) = R x`.
+
+    .. math:: R = \exp(A - A^T)
+
+    Because :math:`A - A^T` is skew-symmetric, :math:`R` is orthogonal.
+
+    Arguments:
+        A: A square matrix :math:`A`, with shape :math:`(*, D, D)`.
+    """
+
+    domain = constraints.real_vector
+    codomain = constraints.real_vector
+    bijective = True
+
+    def __init__(self, A: Tensor, **kwargs):
+        super().__init__(**kwargs)
+
+        self.R = torch.linalg.matrix_exp(A - A.mT)
+
+    def _call(self, x: Tensor) -> Tensor:
+        return x @ self.R
+
+    def _inverse(self, y: Tensor) -> Tensor:
+        return y @ self.R.mT
+
+    def log_abs_det_jacobian(self, x: Tensor, y: Tensor) -> Tensor:
+        return x.new_zeros(x.shape[:-1])
```

### Comparing `zuko-0.2.2/zuko/utils.py` & `zuko-0.3.0/zuko/utils.py`

 * *Files identical despite different names*

### Comparing `zuko-0.2.2/zuko.egg-info/PKG-INFO` & `zuko-0.3.0/zuko.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zuko
-Version: 0.2.2
+Version: 0.3.0
 Summary: Normalizing flows in PyTorch
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
 Project-URL: Documentation, https://zuko.readthedocs.io
 Project-URL: Source, https://github.com/francois-rozet/zuko
 Project-URL: Tracker, https://github.com/francois-rozet/zuko/issues
 Keywords: torch,normalizing flows,probability,density,generative,deep learning
@@ -17,17 +17,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Zuko's banner](https://raw.githubusercontent.com/francois-rozet/zuko/master/docs/images/banner.svg)
 
 # Zuko - Normalizing flows in PyTorch
 
-Zuko is a Python package that implements normalizing flows in PyTorch. It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`.
+Zuko is a Python package that implements normalizing flows in [PyTorch](https://pytorch.org). It relies as much as possible on distributions and transformations already provided by PyTorch. Unfortunately, the `Distribution` and `Transform` classes of `torch` are not sub-classes of `torch.nn.Module`, which means you cannot send their internal tensors to GPU with `.to('cuda')` or retrieve their parameters with `.parameters()`. Worse, the concepts of conditional distribution and transformation, which are essential for probabilistic inference, are impossible to express.
 
-To solve this problem, `zuko` defines two abstract classes: `DistributionModule` and `TransformModule`. The former is any `Module` whose forward pass returns a `Distribution` and the latter is any `Module` whose forward pass returns a `Transform`. A normalizing flow is just a `DistributionModule` which contains a list of `TransformModule` and a base `DistributionModule`. This design allows for flows that behave like distributions while retaining the benefits of `Module`. It also makes the implementations easier to understand and extend.
+To solve these problems, `zuko` defines two abstract modules, `DistributionFactory` and `TransformFactory`, which represent parameterized recipes for building distributions and transformations, respectively. To condition a distribution or transformation simply means to consider the condition/context as part of the recipe, similar to [Pyro](http://pyro.ai)'s `ConditionalTransformModule`. A normalizing flow is a special `DistributionFactory` that contains a sequence of `TransformFactory` and a base `DistributionFactory`. This design enables flows to act like distributions while retaining features inherent to modules, such as trainable parameters. It also makes the implementations easier to understand and extend.
 
 > In the [Avatar](https://wikipedia.org/wiki/Avatar:_The_Last_Airbender) cartoon, [Zuko](https://wikipedia.org/wiki/Zuko) is a powerful firebender 🔥
 
 ## Installation
 
 The `zuko` package is available on [PyPI](https://pypi.org/project/zuko), which means it is installable via `pip`.
 
@@ -63,25 +63,25 @@
     loss.backward()
     optimizer.step()
 
 # Sample 64 points x ~ p(x | c*)
 x = flow(c_star).sample((64,))
 ```
 
-Alternatively, flows can be built as custom `FlowModule` objects.
+Alternatively, flows can be built as custom `Flow` objects.
 
 ```python
-from zuko.flows import FlowModule, MaskedAutoregressiveTransform, Unconditional
+from zuko.flows import Flow, MaskedAutoregressiveTransform, Unconditional
 from zuko.distributions import DiagNormal
-from zuko.transforms import PermutationTransform
+from zuko.transforms import RotationTransform
 
-flow = FlowModule(
+flow = Flow(
     transforms=[
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
-        Unconditional(PermutationTransform, torch.randperm(3), buffer=True),
+        Unconditional(RotationTransform, torch.randn(3, 3)),
         MaskedAutoregressiveTransform(3, 5, hidden_features=[128] * 3),
     ],
     base=Unconditional(
         DiagNormal,
         torch.zeros(3),
         torch.ones(3),
         buffer=True,
@@ -91,18 +91,21 @@
 
 For more information, check out the documentation at [zuko.readthedocs.io](https://zuko.readthedocs.io).
 
 ### Available flows
 
 | Class   | Year | Reference |
 |:-------:|:----:|-----------|
+| `GMM`   | -    | [Gaussian Mixture Model](https://wikipedia.org/wiki/Mixture_model#Gaussian_mixture_model) |
+| `NICE`  | 2014 | [Non-linear Independent Components Estimation](https://arxiv.org/abs/1410.8516) |
 | `MAF`   | 2017 | [Masked Autoregressive Flow for Density Estimation](https://arxiv.org/abs/1705.07057) |
 | `NSF`   | 2019 | [Neural Spline Flows](https://arxiv.org/abs/1906.04032) |
 | `NCSF`  | 2020 | [Normalizing Flows on Tori and Spheres](https://arxiv.org/abs/2002.02428) |
 | `SOSPF` | 2019 | [Sum-of-Squares Polynomial Flow](https://arxiv.org/abs/1905.02325) |
 | `NAF`   | 2018 | [Neural Autoregressive Flows](https://arxiv.org/abs/1804.00779) |
 | `UNAF`  | 2019 | [Unconstrained Monotonic Neural Networks](https://arxiv.org/abs/1908.05164) |
 | `CNF`   | 2018 | [Neural Ordinary Differential Equations](https://arxiv.org/abs/1806.07366) |
+| `GF`    | 2020 | [Gaussianization Flows](https://arxiv.org/abs/2003.01941) |
 
 ## Contributing
 
 If you have a question, an issue or would like to contribute, please read our [contributing guidelines](https://github.com/francois-rozet/zuko/blob/master/CONTRIBUTING.md).
```

