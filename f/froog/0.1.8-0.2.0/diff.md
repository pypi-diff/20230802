# Comparing `tmp/froog-0.1.8.tar.gz` & `tmp/froog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froog-0.1.8.tar", last modified: Fri Jul 28 04:16:39 2023, max compression
+gzip compressed data, was "froog-0.2.0.tar", last modified: Wed Aug  2 01:29:54 2023, max compression
```

## Comparing `froog-0.1.8.tar` & `froog-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.246644 froog-0.1.8/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.1.8/LICENSE
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2640 2023-07-28 04:16:39.246517 froog-0.1.8/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2315 2023-07-28 03:27:43.000000 froog-0.1.8/README.md
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.244341 froog-0.1.8/froog/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.1.8/froog/__init__.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2104 2023-07-28 03:55:03.000000 froog-0.1.8/froog/gradcheck.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1259 2023-07-28 03:37:44.000000 froog-0.1.8/froog/nn.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)    12095 2023-07-28 03:42:14.000000 froog-0.1.8/froog/ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1986 2023-07-27 02:41:00.000000 froog-0.1.8/froog/optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4114 2023-07-28 03:49:20.000000 froog-0.1.8/froog/tensor.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2710 2023-07-28 02:45:00.000000 froog-0.1.8/froog/utils.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.245040 froog-0.1.8/froog.egg-info/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2640 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/PKG-INFO
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      382 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/SOURCES.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/dependency_links.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/requires.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-07-28 04:16:39.000000 froog-0.1.8/froog.egg-info/top_level.txt
--rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-07-28 04:16:39.246683 froog-0.1.8/setup.cfg
--rw-r--r--   0 kevinbuhler   (501) staff       (20)      851 2023-07-28 04:16:31.000000 froog-0.1.8/setup.py
-drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-07-28 04:16:39.246210 froog-0.1.8/tests/
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.1.8/tests/test_conv_speed.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-28 03:41:52.000000 froog-0.1.8/tests/test_mnist.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     3556 2023-07-28 03:26:43.000000 froog-0.1.8/tests/test_ops.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.1.8/tests/test_optim.py
--rw-r--r--   0 kevinbuhler   (501) staff       (20)     2604 2023-07-27 02:41:36.000000 froog-0.1.8/tests/test_tensor.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.071290 froog-0.2.0/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       31 2023-07-16 20:10:22.000000 froog-0.2.0/LICENSE
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2995 2023-08-02 01:29:54.071153 froog-0.2.0/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2670 2023-08-02 00:11:34.000000 froog-0.2.0/README.md
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.069563 froog-0.2.0/froog/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       57 2023-07-26 06:32:22.000000 froog-0.2.0/froog/__init__.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2417 2023-07-30 06:46:05.000000 froog-0.2.0/froog/gradcheck.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1882 2023-07-28 16:42:26.000000 froog-0.2.0/froog/nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)    14381 2023-07-30 19:25:09.000000 froog-0.2.0/froog/ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4902 2023-07-30 21:07:16.000000 froog-0.2.0/froog/ops_gpu.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2355 2023-07-30 06:46:05.000000 froog-0.2.0/froog/optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     7230 2023-08-02 01:26:16.000000 froog-0.2.0/froog/tensor.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3079 2023-07-30 01:43:20.000000 froog-0.2.0/froog/utils.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.070204 froog-0.2.0/froog.egg-info/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2995 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/PKG-INFO
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      416 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/SOURCES.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        1 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/dependency_links.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       15 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/requires.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)        6 2023-08-02 01:29:54.000000 froog-0.2.0/froog.egg-info/top_level.txt
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)       38 2023-08-02 01:29:54.071326 froog-0.2.0/setup.cfg
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)      851 2023-08-02 01:29:38.000000 froog-0.2.0/setup.py
+drwxr-xr-x   0 kevinbuhler   (501) staff       (20)        0 2023-08-02 01:29:54.070968 froog-0.2.0/tests/
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     3172 2023-07-28 03:44:46.000000 froog-0.2.0/tests/test_conv_speed.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4256 2023-07-28 03:41:52.000000 froog-0.2.0/tests/test_mnist.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1043 2023-07-28 04:44:12.000000 froog-0.2.0/tests/test_nn.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     4717 2023-07-30 19:28:07.000000 froog-0.2.0/tests/test_ops.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     1987 2023-07-27 02:40:39.000000 froog-0.2.0/tests/test_optim.py
+-rw-r--r--   0 kevinbuhler   (501) staff       (20)     2618 2023-07-30 06:46:05.000000 froog-0.2.0/tests/test_tensor.py
```

### Comparing `froog-0.1.8/PKG-INFO` & `froog-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.8
+Version: 0.2.0
 Summary: a beautifully compact machine-learning library
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
   <br/>
-  froog: fast real-time optimization of gradients 
+  FROOG: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
   <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 <!-- the goal of froog is to make a neural network libary to power any type of device from enterprise to small home robotics -->
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
+<!-- grug say never be not improving tooling  -->
+<!-- ml toolkit -->
 
-froog is extremely simple, with a goal of running ml on any device, by any human, easily and efficiently
+FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
@@ -51,33 +53,42 @@
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolutions
 - Avg & Max pooling
 - <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">More</a> 
 
+### Ready-to-Go Models
+- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">EfficientNet-B0</a> 
+
+<!-- Here’s an example, to give you an impression: -->
+
 # Bounties
 Want to help but don't know where to start? Here are some bounties for you to claim
 #### Small   <!-- ez money  -->
 - binary cross entropy
 - flatten
 - batch_norm
 - div
 - pow
 - dropout 
 #### Medium  <!-- mid tier -->
 - start doing ops with opencl
+- einsum convs
 - simplify how context and gradients are handled
-- efficient net
 #### Large <!-- EXPERT LEVEL!!!  -->
+- ability training on FROOG!!!!
+- float16 support
 - transformers
 - stable diffusion
 - winograd convs
-- MPS support
-- CUDA support
+- GPU Support
+  - MPS
+  - CUDA
+  - OpenCL
 
 # Contributing
 Here are the rules for contributing:
 * increase simplicity
 * increase efficiency
 * increase functionality
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.8 Summary: a beautifully compact
+Metadata-Version: 2.1 Name: froog Version: 0.2.0 Summary: a beautifully compact
 machine-learning library Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # froog [unit test badge]
                                [froog the frog]
-               froog: fast real-time optimization of gradients
+               FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
-    froog is extremely simple, with a goal of running ml on any device, by any
-human, easily and efficiently # Installation ```bash pip install froog ``` ###
-Overview of Features - Tensors - Automatic Differentiation - Forward and
-backward passes - Input/gradient shape-tracking - MNIST example - 2D
-Convolutions (im2col) - Numerical gradient checking - The most common
-optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
-Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolutions - Avg
-& Max pooling - More # Bounties Want to help but don't know where to start?
-Here are some bounties for you to claim #### Small  - binary cross entropy -
-flatten - batch_norm - div - pow - dropout #### Medium  - start doing ops with
-opencl - simplify how context and gradients are handled - efficient net ####
-Large  - transformers - stable diffusion - winograd convs - MPS support - CUDA
-support # Contributing Here are the rules for contributing: * increase
-simplicity * increase efficiency * increase functionality more info on
-contributing
+      FROOG is a neural network framework that is actually **SIMPLE** with the
+goal of running machine learning on any device --> easily and efficiently. #
+Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
+Automatic Differentiation - Forward and backward passes - Input/gradient shape-
+tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
+checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
+- Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
+Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
+B0  # Bounties Want to help but don't know where to start? Here are some
+bounties for you to claim #### Small  - binary cross entropy - flatten -
+batch_norm - div - pow - dropout #### Medium  - start doing ops with opencl -
+einsum convs - simplify how context and gradients are handled #### Large  -
+ability training on FROOG!!!! - float16 support - transformers - stable
+diffusion - winograd convs - GPU Support - MPS - CUDA - OpenCL # Contributing
+Here are the rules for contributing: * increase simplicity * increase
+efficiency * increase functionality more info on contributing
```

### Comparing `froog-0.1.8/README.md` & `froog-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
   <br/>
-  froog: fast real-time optimization of gradients 
+  FROOG: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
   <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 <!-- the goal of froog is to make a neural network libary to power any type of device from enterprise to small home robotics -->
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
+<!-- grug say never be not improving tooling  -->
+<!-- ml toolkit -->
 
-froog is extremely simple, with a goal of running ml on any device, by any human, easily and efficiently
+FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
@@ -39,33 +41,42 @@
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolutions
 - Avg & Max pooling
 - <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">More</a> 
 
+### Ready-to-Go Models
+- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">EfficientNet-B0</a> 
+
+<!-- Here’s an example, to give you an impression: -->
+
 # Bounties
 Want to help but don't know where to start? Here are some bounties for you to claim
 #### Small   <!-- ez money  -->
 - binary cross entropy
 - flatten
 - batch_norm
 - div
 - pow
 - dropout 
 #### Medium  <!-- mid tier -->
 - start doing ops with opencl
+- einsum convs
 - simplify how context and gradients are handled
-- efficient net
 #### Large <!-- EXPERT LEVEL!!!  -->
+- ability training on FROOG!!!!
+- float16 support
 - transformers
 - stable diffusion
 - winograd convs
-- MPS support
-- CUDA support
+- GPU Support
+  - MPS
+  - CUDA
+  - OpenCL
 
 # Contributing
 Here are the rules for contributing:
 * increase simplicity
 * increase efficiency
 * increase functionality
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
 # froog [unit test badge]
                                [froog the frog]
-               froog: fast real-time optimization of gradients
+               FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
-    froog is extremely simple, with a goal of running ml on any device, by any
-human, easily and efficiently # Installation ```bash pip install froog ``` ###
-Overview of Features - Tensors - Automatic Differentiation - Forward and
-backward passes - Input/gradient shape-tracking - MNIST example - 2D
-Convolutions (im2col) - Numerical gradient checking - The most common
-optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
-Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolutions - Avg
-& Max pooling - More # Bounties Want to help but don't know where to start?
-Here are some bounties for you to claim #### Small  - binary cross entropy -
-flatten - batch_norm - div - pow - dropout #### Medium  - start doing ops with
-opencl - simplify how context and gradients are handled - efficient net ####
-Large  - transformers - stable diffusion - winograd convs - MPS support - CUDA
-support # Contributing Here are the rules for contributing: * increase
-simplicity * increase efficiency * increase functionality more info on
-contributing
+      FROOG is a neural network framework that is actually **SIMPLE** with the
+goal of running machine learning on any device --> easily and efficiently. #
+Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
+Automatic Differentiation - Forward and backward passes - Input/gradient shape-
+tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
+checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
+- Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
+Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
+B0  # Bounties Want to help but don't know where to start? Here are some
+bounties for you to claim #### Small  - binary cross entropy - flatten -
+batch_norm - div - pow - dropout #### Medium  - start doing ops with opencl -
+einsum convs - simplify how context and gradients are handled #### Large  -
+ability training on FROOG!!!! - float16 support - transformers - stable
+diffusion - winograd convs - GPU Support - MPS - CUDA - OpenCL # Contributing
+Here are the rules for contributing: * increase simplicity * increase
+efficiency * increase functionality more info on contributing
```

### Comparing `froog-0.1.8/froog/gradcheck.py` & `froog-0.2.0/froog/gradcheck.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,31 @@
+#  _______  ______    _______  _______  _______ 
+# |       ||    _ |  |       ||       ||       |
+# |    ___||   | ||  |   _   ||   _   ||    ___|
+# |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
+# |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
+# |   |    |   |  | ||       ||       ||   |_| |
+# |___|    |___|  |_||_______||_______||_______|
+#
+
 import numpy as np
 from froog.tensor import Tensor
 from froog.utils import mask_like
 
 def jacobian(model, input):
   output = model(input)
 
   ji = input.data.reshape(-1).shape[-1]  # jacobian of input
   jo = output.data.reshape(-1).shape[-1] # jacobian of output
   J = np.zeros((jo, ji), dtype=np.float32)
 
   for o in range(jo):
     o_scalar = Tensor(mask_like(output.data, o, 1.)).mul(output).sum()
     o_scalar.backward()
-    for i, grad in enumerate(input.grad.reshape(-1)):
+    for i, grad in enumerate(input.grad.data.reshape(-1)):
       J[o,i] = grad
   return J
 
 def numerical_jacobian(model, input, eps = 1e-6):
 #     """
 #     https://timvieira.github.io/blog/post/2017/04/21/how-to-test-gradient-implementations/
 #     Computes :
@@ -32,22 +41,22 @@
 
   ji = input.data.reshape(-1).shape[-1]
   jo = output.data.reshape(-1).shape[-1]
   NJ = np.zeros((jo, ji), dtype=np.float32)
 
   for i in range(ji):
     eps_perturb = mask_like(input.data, i, mask_value = eps)
-    for o in range(jo):
 
-      output_perturb_add = model(Tensor(input.data + eps_perturb)).data.reshape(-1)[o]
-      output_perturb_sub = model(Tensor(input.data - eps_perturb)).data.reshape(-1)[o]
+    output_perturb_add = model(Tensor(input.data + eps_perturb)).data.reshape(-1)
+    output_perturb_sub = model(Tensor(input.data - eps_perturb)).data.reshape(-1)
+
+    grad_approx = ((output_perturb_add) - (output_perturb_sub)) / (2*eps) # CDM: (f(x + h) - f(x - h)) / (2 * h)
 
-      grad_approx = ((output_perturb_add) - (output_perturb_sub)) / (2*eps) # CDM: (f(x + h) - f(x - h)) / (2 * h)
+    NJ[:,i] = grad_approx
 
-      NJ[o][i] = grad_approx
   return NJ
 
 def gradcheck(model, input, eps = 1e-06, atol = 1e-5, rtol = 0.001):
   """
   Checks whether computed gradient is close to numerical approximation of the Jacobian
   Params:
     model       : froog model
```

### Comparing `froog-0.1.8/froog/ops.py` & `froog-0.2.0/froog/ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,28 @@
+#  _______  ______    _______  _______  _______ 
+# |       ||    _ |  |       ||       ||       |
+# |    ___||   | ||  |   _   ||   _   ||    ___|
+# |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
+# |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
+# |   |    |   |  | ||       ||       ||   |_| |
+# |___|    |___|  |_||_______||_______||_______|
+
 import numpy as np
 from froog.tensor import Function, register
 from froog.utils import im2col, col2im
 
-# *********** Elementary Functions ***********
-# Add, Mul, ReLU, Dot, Sum, Conv2D, Reshape 
-# grad_output is the gradient of the loss with respect to the output of the operation.
-
-# ******* core ops *******
+# *****************************************************
+#     ____  ___   _____ __________   ____  ____  _____
+#    / __ )/   | / ___//  _/ ____/  / __ \/ __ \/ ___/
+#   / __  / /| | \__ \ / // /      / / / / /_/ /\__ \ 
+#  / /_/ / ___ |___/ // // /___   / /_/ / ____/___/ / 
+# /_____/_/  |_/____/___/\____/   \____/_/    /____/  
+#
+# **************** Basic Operations ***************
+# - grad_output is the gradient of the loss with respect to the output of the operation.
 
 class Add(Function):# x.add(y)
   @staticmethod     # @staticmethod doesn't require an instance of Add to work, so you can do x.add(y)
   def forward(ctx, x, y):
     return x + y
   
   @staticmethod
@@ -36,84 +48,101 @@
 
   @staticmethod
   def backward(ctx, grad_output):
     x, y = ctx.saved_tensors
     return y * grad_output, x * grad_output
 register("mul", Mul)
 
+class Sum(Function):
+  """
+  reduce op
+  reduces its input tensor to a single value by summing all the elements
+  """
+  @staticmethod
+  def forward(ctx, input):
+    ctx.save_for_backward(input)
+    return np.array([input.sum()])
+
+  @staticmethod
+  def backward(ctx, grad_output):
+    (input,) = ctx.saved_tensors
+    return grad_output * np.ones_like(input)
+register("sum", Sum)
+
 class Pow(Function): # x.pow(y)
   @staticmethod
   def forward(ctx, x, y):
     ctx.save_for_backward(x, y)
     return x ** y
   
   @staticmethod
   def backward(ctx, grad_output):
     x, y = ctx.saved_tensors
     return y * (x**(y-1.0)) * grad_output, (x**y) * np.log(x) * grad_output # power rule, d/dx (y^x)
 register("pow", Pow)
 
+
+# *******************************               
+#    ______________  _____  ___
+#   / ____/ ____/  |/  /  |/  /
+#  / / __/ __/ / /|_/ / /|_/ / 
+# / /_/ / /___/ /  / / /  / /  
+# \____/_____/_/  /_/_/  /_/   
+# 
+# ******* GEMM ops *******          
+                             
 class Dot(Function):  # x.dot(y)
   @staticmethod
   def forward(ctx, input, weight):
     ctx.save_for_backward(input, weight)
     return input.dot(weight)
 
   @staticmethod
   def backward(ctx, grad_output):
     input, weight = ctx.saved_tensors
     grad_input = grad_output.dot(weight.T)
     grad_weight = grad_output.T.dot(input).T
     return grad_input, grad_weight
 register('dot', Dot)
+register('matmul', Dot)
 
-class Sum(Function):
-  """
-  reduce op
-  reduces its input tensor to a single value by summing all the elements
-  """
-  @staticmethod
-  def forward(ctx, input):
-    ctx.save_for_backward(input)
-    return np.array([input.sum()])
-
-  @staticmethod
-  def backward(ctx, grad_output):
-    (input,) = ctx.saved_tensors
-    return grad_output * np.ones_like(input)
-register("sum", Sum)
-
-# ******* nn ops *******
 
+# ***********************************************************
+#    _____ ______  _______  __    ______   ____  ____  _____
+#   / ___//  _/  |/  / __ \/ /   / ____/  / __ \/ __ \/ ___/
+#   \__ \ / // /|_/ / /_/ / /   / __/    / / / / /_/ /\__ \ 
+#  ___/ // // /  / / ____/ /___/ /___   / /_/ / ____/___/ / 
+# /____/___/_/  /_/_/   /_____/_____/   \____/_/    /____/  
+#
+# ************************ nn ops ***********************              
+                                                          
 class ReLU(Function): 
   @staticmethod
   def forward(ctx, input):
     ctx.save_for_backward(input)
-    return np.maximum(input, 0) # relu(x) = max(0,x)
+    return np.maximum(input, 0)                     # relu(x) = max(0,x)
 
   @staticmethod
   def backward(ctx, grad_output):
     input, = ctx.saved_tensors
     grad_input = grad_output * (input >= 0)
     return grad_input
 register("relu", ReLU)
 
 class Sigmoid(Function): 
   @staticmethod
   def forward(ctx, input):
     ctx.save_for_backward(input)
-    with np.warnings.catch_warnings():           # TODO: stable sigmoid? does the overflow matter?
-      np.warnings.filterwarnings('ignore')
-      ret = 1/(1 + np.exp(-input))               # sigmoid(x) = 1 / (1 + exp(-x))
+    ret = 1/(1 + np.exp(-input))                    # sigmoid(x) = 1 / (1 + exp(-x))
     return ret 
 
   @staticmethod
   def backward(ctx, grad_output):
     ret, = ctx.saved_tensors
-    grad_input = grad_output * (ret * (1 - ret)) # just take the derivative of sigmoid
+    grad_input = grad_output * (ret * (1 - ret))    # just take the derivative of sigmoid
     return grad_input
 register("sigmoid", Sigmoid)
 
 class Reshape(Function):
   @staticmethod
   def forward(ctx, x, shape):
     ctx.save_for_backward(x.shape)
@@ -155,68 +184,81 @@
 
   @staticmethod
   def backward(ctx, grad_output):
     (output,) = ctx.saved_tensors
     return grad_output - np.exp(output) * grad_output.sum(axis=1).reshape((-1, 1))
 register("logsoftmax", LogSoftmax)
 
-# ************* conv ops *************
 
-class Conv2D(Function): 
+# *************************************************
+#    __________  _   ___    __   ____  ____  _____
+#   / ____/ __ \/ | / / |  / /  / __ \/ __ \/ ___/
+#  / /   / / / /  |/ /| | / /  / / / / /_/ /\__ \ 
+# / /___/ /_/ / /|  / | |/ /  / /_/ / ____/___/ / 
+# \____/\____/_/ |_/  |___/   \____/_/    /____/  
+#
+# ****************** conv ops *****************
+
+class Conv2D(Function): # TODO: understand group splits
   @staticmethod
   def forward(ctx, x, w, stride=1, groups=1):
     """
     https://github.com/vdumoulin/conv_arithmetic/blob/master/README.md
     WARNING: doesn't handle padding or strides yet
     Args:
       x.shape[0] 									  --> number of input examples (batch size)
       cout 			 								    --> number of output channels
       x.shape[2]-(H-1)					 	  --> non-padded height of conv output, need to subtract because this is an unpadded conv
       x.shape[3]-(W-1)						  --> width of output
     Shape: 
       (a, b, c, d)(e, f, g, h)      --> (a, e, c-(g-1), d-(h-1)) 
       in general, output x and y = [(W−K+2P)/S]+1
     """
-    if type(ctx.stride) == int:                                                          # ctx stores function params
+    if type(ctx.stride) == int:                                                                           # ctx stores function params
       ctx.stride = (ctx.stride, ctx.stride)
 
     cout, cin, H, W = w.shape
 
-    if groups > 1:                                                                       # allows grouped convolutions 
-      w = np.repeat(w, groups, axis=1) / groups                                          # TODO: why does this work?
-
-    tw = w.reshape(cout, -1).T                                                           # slice of kernel 
+    tw = w.reshape(cout, -1).T                                                                            # slice of kernel 
     y_stride, x_stride = ctx.stride
-    bs, oy, ox = x.shape[0], (x.shape[2]-(H-y_stride))//y_stride, (x.shape[3]-(W-x_stride))//x_stride
-    ctx.save_for_backward(x, w)
 
-    ret = np.zeros((bs, cout, oy, ox), dtype=w.dtype)
+    bs,cin_,oy,ox = x.shape[0], x.shape[1], (x.shape[2]-(H-y_stride))//y_stride, (x.shape[3]-(W-x_stride))//x_stride
+    assert cin*ctx.groups == cin_                                                                         # ensures that the channel dimensions match appropriately for grouping
+    assert cout % ctx.groups == 0                                                                         # ensures that the number of output channels can be evenly divided among the groups
+    g_w_chans = cout//ctx.groups                                                                          # number of output channels per group
 
-    for Y in range(oy):                                                                  # non_padded_height of output
-      for X in range(ox):                                                                # non_padded_width  of output
-        iY, iX = Y*y_stride, X*x_stride                                    
-        tx = x[:, :, iY:iY+H, iX:iX+W].reshape(bs, -1)
-        ret[:, :, Y, X] = tx.dot(tw)
+    ctx.save_for_backward(x, w)
+    ret = np.zeros((bs, cout, oy, ox), dtype=w.dtype)
+    
+    for g in range(ctx.groups):
+      tw = w[g*g_w_chans:(g*g_w_chans+g_w_chans)].reshape(g_w_chans, -1).T                                # transformed kernel weights
+      for Y in range(oy):
+        for X in range(ox):
+          iY,iX = Y*y_stride, X*x_stride
+          tx = x[:, g*cin:(g*cin+cin), iY:iY+H, iX:iX+W].reshape(bs, -1)
+          ret[:, g*g_w_chans:(g*g_w_chans+g_w_chans), Y, X] += tx.dot(tw)
     return ret
 
   @staticmethod
   def backward(ctx, grad_output):
-    x, conv_kernel = ctx.saved_tensors
-    cout, cin, H, W = conv_kernel.shape
-    dx, dw = np.zeros_like(x), np.zeros_like(conv_kernel)
-    tw = conv_kernel.reshape(cout, -1)                                                   # transformed kernel weights
+    x, w = ctx.saved_tensors
+    cout, cin, H, W = w.shape
+    dx, dw = np.zeros_like(x), np.zeros_like(w)                                         
     y_stride, x_stride = ctx.stride
+    g_w_chans = cout//ctx.groups
 
-    for Y in range(grad_output.shape[2]):
-      for X in range(grad_output.shape[3]):
-        iY,iX = Y*y_stride, X*x_stride
-        gg = grad_output[:, :, Y, X]                                                     # current multiply element in chain rule
-        tx = x[:, :, iY:iY+H, iX:iX+W].reshape(x.shape[0], -1)                           # slice of tensor at current conv op                                                                                # 
-        dw += gg.T.dot(tx).reshape(dw.shape)                                             # gradient with respect to input 
-        dx[:, :, iY:iY+H, iX:iX+W] += gg.dot(tw).reshape(dx.shape[0], dx.shape[1], H, W) # accumulate gradient with respect to weights 
+    for g in range(ctx.groups):
+      tw = w[g*g_w_chans:(g*g_w_chans+g_w_chans)].reshape(g_w_chans, -1)
+      for Y in range(grad_output.shape[2]):
+        for X in range(grad_output.shape[3]):
+          iY,iX = Y*y_stride, X*x_stride
+          gg = grad_output[:, g*g_w_chans:(g*g_w_chans+g_w_chans), Y, X]                                  # current multiply element in chain rule
+          tx = x[:, g*cin:(g*cin+cin), iY:iY+H, iX:iX+W].reshape(x.shape[0], -1)                          # slice of tensor at current conv op        
+          dw[g*g_w_chans:(g*g_w_chans+g_w_chans)] += gg.T.dot(tx).reshape((g_w_chans,cin,H,W))            # gradient with respect to input
+          dx[:, g*cin:(g*cin+cin), iY:iY+H, iX:iX+W] += gg.dot(tw).reshape(dx.shape[0], cin, H, W)        # accumulate gradient with respect to weights 
     return dx, dw
 register('conv2d', Conv2D)
 
 
 class im2ColConv(Function):
   """
   uses im2col
@@ -242,32 +284,40 @@
     gg = np.moveaxis(grad_output, [0,1,2,3], [1,0,2,3]).reshape(cout, -1)  # order correctly
     dw = gg.dot(tx).reshape(w.shape)                                       # compute gradient of weight
     dxi = gg.T.dot(tw)                                                     # compute gradient of input
     dx = col2im(dxi, H, W, oy+(H-1), ox+(W-1))                             # turn columns back into image shape
     return dx, dw
 register('im2col2dconv', im2ColConv)
 
-# ************* pooling ops *************
+
+# *************************************************
+#     ____  ____  ____  __       ____  ____  _____
+#    / __ \/ __ \/ __ \/ /      / __ \/ __ \/ ___/
+#   / /_/ / / / / / / / /      / / / / /_/ /\__ \ 
+#  / ____/ /_/ / /_/ / /___   / /_/ / ____/___/ / 
+# /_/    \____/\____/_____/   \____/_/    /____/  
+#
+# **************** pooling ops ***************
 
 def stack_for_pool(x, pool_y, pool_x):
   my, mx = (x.shape[2]//pool_y)*pool_y, (x.shape[3]//pool_x)*pool_x        # ensures input tensor can be evenly divided into 2x2 blocks for max pooling
   stack = []
   cropped_x = x[:, :, :my, :mx]                                            # crop input so 2x2 max pool can be taken
   for Y in range(pool_y):
       for X in range(pool_x):
         stack.append(cropped_x[:, :, Y::pool_y, X::pool_x][None])          # ::2 so 2x2 goes to next pool, [None] is numpy way to add an extra dimension so we can concatenate
   return np.concatenate(stack, axis=0)                                     # put all into one row
 
 
 def unstack_for_pool(fxn, s, py, px):
-  max_y, max_x = (s[2]//py)*py, (s[3]//px)*px                               # get shape that allows (pool_size_y,pool_size_x) max pool
+  max_y, max_x = (s[2]//py)*py, (s[3]//px)*px                              # get shape that allows (pool_size_y,pool_size_x) max pool
   for Y in range(py):
     for X in range(px):
       level_w_new_grad = fxn(Y*px+X)
-      if X == 0 and Y == 0:                                                 # pool of zero size
+      if X == 0 and Y == 0:                                                # pool of zero size
         ret = np.zeros(s, dtype=level_w_new_grad.dtype)
       ret[:, :, Y:max_y:py, X:max_x:px] = level_w_new_grad
   return ret
 
 
 class MaxPool2D(Function):
   @staticmethod
@@ -297,15 +347,15 @@
     stack = stack_for_pool(x, *kernel_size)
     ctx.save_for_backward(x.shape)
     return np.mean(stack, axis=0)
 
   @staticmethod
   def backward(ctx, grad_output):
     s, = ctx.saved_tensors
-    py, px = ctx.kernel_size                                               # TODO: where does kernel_size come from?
+    py, px = ctx.kernel_size                                  # TODO: where does kernel_size come from?
     my, mx = (s[2]//py)*py, (s[3]//px)*px
     ret = np.zeros(s, dtype=grad_output.dtype)
     for Y in range(py):
       for X in range(px):
-        ret[:, :, Y:my:py, X:mx:px] = grad_output / py / px # divide by avg of pool, e.g. for 2x2 pool /= 4
+        ret[:, :, Y:my:py, X:mx:px] = grad_output / py / px   # divide by avg of pool, e.g. for 2x2 pool /= 4
     return ret
 register('avg_pool2d', AvgPool2D)
```

### Comparing `froog-0.1.8/froog/utils.py` & `froog-0.2.0/froog/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,45 @@
+#  _______  ______    _______  _______  _______ 
+# |       ||    _ |  |       ||       ||       |
+# |    ___||   | ||  |   _   ||   _   ||    ___|
+# |   |___ |   |_||_ |  | |  ||  | |  ||   | __ 
+# |    ___||    __  ||  |_|  ||  |_|  ||   ||  |
+# |   |    |   |  | ||       ||       ||   |_| |
+# |___|    |___|  |_||_______||_______||_______|
+
 import numpy as np
 from functools import lru_cache
 
 def dense_layer(*tensor_size):
   # TODO: why dividing by sqrt?
   ret = np.random.uniform(-1., 1., size=tensor_size)/np.sqrt(np.prod(tensor_size)) # random init weights
   return ret.astype(np.float32)
 
 def fetch(url):
   print(f"fetching {url}...")
-  import requests, os, hashlib
-  fp = os.path.join("/tmp", hashlib.md5(url.encode('utf-8')).hexdigest())
+  import requests, os, hashlib, tempfile
+  fp = os.path.join(tempfile.gettempdir(), hashlib.md5(url.encode('utf-8')).hexdigest())
   if os.path.isfile(fp):
     with open(fp, "rb") as f:
       dat = f.read()
   else:
     with open(fp, "wb") as f:
       dat = requests.get(url).content
       f.write(dat)
   return dat
 
+def fetch_mnist():
+  import gzip
+  parse = lambda dat: np.frombuffer(gzip.decompress(dat), dtype=np.uint8).copy()
+  X_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
+  Y_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz"))[8:]
+  X_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
+  Y_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz"))[8:]
+  return X_train, Y_train, X_test, Y_test
+
 def mask_like(like, mask_inx, mask_value=1.0):
   mask = np.zeros_like(like).reshape(-1) # flatten
   mask[mask_inx] = mask_value            # fill 
   return mask.reshape(like.shape)
 
 @lru_cache
 def get_im2col_index(oy, ox, cin, H, W):
@@ -59,17 +76,8 @@
   oy, ox = OY-(H-1), OX-(W-1)
   bs = tx.shape[0] // (oy * ox)
   channels_in = tx.shape[1] // (H * W)
 
   ridx = rearrange_col2im_index(oy, ox, channels_in, H, W)
   # -1 has to be 0s
   x = np.pad(tx.reshape(bs, -1), ((0,0),(0,1)))[:, ridx].sum(axis=2)
-  return x.reshape(bs, channels_in, OY, OX)
-
-def fetch_mnist():
-  import gzip
-  parse = lambda dat: np.frombuffer(gzip.decompress(dat), dtype=np.uint8).copy()
-  X_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
-  Y_train = parse(fetch("http://yann.lecun.com/exdb/mnist/train-labels-idx1-ubyte.gz"))[8:]
-  X_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-images-idx3-ubyte.gz"))[0x10:].reshape((-1, 28, 28))
-  Y_test = parse(fetch("http://yann.lecun.com/exdb/mnist/t10k-labels-idx1-ubyte.gz"))[8:]
-  return X_train, Y_train, X_test, Y_test
+  return x.reshape(bs, channels_in, OY, OX)
```

### Comparing `froog-0.1.8/froog.egg-info/PKG-INFO` & `froog-0.2.0/froog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 Metadata-Version: 2.1
 Name: froog
-Version: 0.1.8
+Version: 0.2.0
 Summary: a beautifully compact machine-learning library
 Author: Kevin Buhler
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # froog <img src="https://github.com/kevbuh/froog/actions/workflows/test.yml/badge.svg" alt="unit test badge" >
 <div align="center" >
-  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="300">
+  <img src="https://raw.githubusercontent.com/kevbuh/froog/main/assets/froog.png" alt="froog the frog" height="200">
   <br/>
-  froog: fast real-time optimization of gradients 
+  FROOG: fast real-time optimization of gradients 
   <br/>
   a beautifully compact machine-learning library
   <br/>
   <a href="https://github.com/kevbuh/froog">homepage</a> | <a href="https://github.com/kevbuh/froog/tree/main/docs">documentation</a> | <a href="https://pypi.org/project/froog/">pip</a>
   <br/>
   <br/>
 </div>
 
 <!-- modern ml development is unintuitive, time consuming, and unaccessible. why not make it possible for anyone to build? -->
 <!-- the goal of froog is to make a neural network libary to power any type of device from enterprise to small home robotics -->
 <!-- machine learning is like making a lego. you combine standardized pieces, of all shapes and sizes, to create anything you imagine -->
 <!-- froog is making those essential building blocks. -->
+<!-- grug say never be not improving tooling  -->
+<!-- ml toolkit -->
 
-froog is extremely simple, with a goal of running ml on any device, by any human, easily and efficiently
+FROOG is a neural network framework that is actually **SIMPLE** with the goal of running machine learning on any device --> easily and efficiently.
 
 # Installation
 ```bash
 pip install froog
 ```
 
 ### Overview of Features
@@ -51,33 +53,42 @@
 - Sum
 - ReLU
 - Log Softmax
 - 2D Convolutions
 - Avg & Max pooling
 - <a href="https://github.com/kevbuh/froog/blob/main/froog/ops.py">More</a> 
 
+### Ready-to-Go Models
+- <a href="https://github.com/kevbuh/froog/blob/main/models/efficientnet.py">EfficientNet-B0</a> 
+
+<!-- Here’s an example, to give you an impression: -->
+
 # Bounties
 Want to help but don't know where to start? Here are some bounties for you to claim
 #### Small   <!-- ez money  -->
 - binary cross entropy
 - flatten
 - batch_norm
 - div
 - pow
 - dropout 
 #### Medium  <!-- mid tier -->
 - start doing ops with opencl
+- einsum convs
 - simplify how context and gradients are handled
-- efficient net
 #### Large <!-- EXPERT LEVEL!!!  -->
+- ability training on FROOG!!!!
+- float16 support
 - transformers
 - stable diffusion
 - winograd convs
-- MPS support
-- CUDA support
+- GPU Support
+  - MPS
+  - CUDA
+  - OpenCL
 
 # Contributing
 Here are the rules for contributing:
 * increase simplicity
 * increase efficiency
 * increase functionality
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,25 +1,26 @@
-Metadata-Version: 2.1 Name: froog Version: 0.1.8 Summary: a beautifully compact
+Metadata-Version: 2.1 Name: froog Version: 0.2.0 Summary: a beautifully compact
 machine-learning library Author: Kevin Buhler License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
 File: LICENSE # froog [unit test badge]
                                [froog the frog]
-               froog: fast real-time optimization of gradients
+               FROOG: fast real-time optimization of gradients
                 a beautifully compact machine-learning library
                         homepage | documentation | pip
 
-    froog is extremely simple, with a goal of running ml on any device, by any
-human, easily and efficiently # Installation ```bash pip install froog ``` ###
-Overview of Features - Tensors - Automatic Differentiation - Forward and
-backward passes - Input/gradient shape-tracking - MNIST example - 2D
-Convolutions (im2col) - Numerical gradient checking - The most common
-optimizers (SGD, Adam, RMSProp) ### Math Operations - Scalar-Matrix
-Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D Convolutions - Avg
-& Max pooling - More # Bounties Want to help but don't know where to start?
-Here are some bounties for you to claim #### Small  - binary cross entropy -
-flatten - batch_norm - div - pow - dropout #### Medium  - start doing ops with
-opencl - simplify how context and gradients are handled - efficient net ####
-Large  - transformers - stable diffusion - winograd convs - MPS support - CUDA
-support # Contributing Here are the rules for contributing: * increase
-simplicity * increase efficiency * increase functionality more info on
-contributing
+      FROOG is a neural network framework that is actually **SIMPLE** with the
+goal of running machine learning on any device --> easily and efficiently. #
+Installation ```bash pip install froog ``` ### Overview of Features - Tensors -
+Automatic Differentiation - Forward and backward passes - Input/gradient shape-
+tracking - MNIST example - 2D Convolutions (im2col) - Numerical gradient
+checking - The most common optimizers (SGD, Adam, RMSProp) ### Math Operations
+- Scalar-Matrix Multiplication - Dot Product - Sum - ReLU - Log Softmax - 2D
+Convolutions - Avg & Max pooling - More ### Ready-to-Go Models - EfficientNet-
+B0  # Bounties Want to help but don't know where to start? Here are some
+bounties for you to claim #### Small  - binary cross entropy - flatten -
+batch_norm - div - pow - dropout #### Medium  - start doing ops with opencl -
+einsum convs - simplify how context and gradients are handled #### Large  -
+ability training on FROOG!!!! - float16 support - transformers - stable
+diffusion - winograd convs - GPU Support - MPS - CUDA - OpenCL # Contributing
+Here are the rules for contributing: * increase simplicity * increase
+efficiency * increase functionality more info on contributing
```

### Comparing `froog-0.1.8/setup.py` & `froog-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='froog',
-      version='0.1.8',
+      version='0.2.0',
       description='a beautifully compact machine-learning library',
       author='Kevin Buhler',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['froog'],
       classifiers=[
```

### Comparing `froog-0.1.8/tests/test_conv_speed.py` & `froog-0.2.0/tests/test_conv_speed.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.8/tests/test_mnist.py` & `froog-0.2.0/tests/test_mnist.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.8/tests/test_ops.py` & `froog-0.2.0/tests/test_ops.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,107 @@
 import numpy as np
-from froog.tensor import Tensor
+from froog.tensor import Tensor, GPU
 import torch
 import unittest
 import timeit
 import functools
 
-def helper_test_op(shape, torch_func, froog_func, atol=1e-7, grad_atol=1e-7):
+def helper_test_op(shape, torch_func, froog_func, atol=1e-7, grad_atol=1e-7, gpu=False, forward_only=False):
   torch_tensors = [torch.rand(x, requires_grad=True) for x in shape]
   froog_tensors = [Tensor(x.detach().numpy()) for x in torch_tensors]
 
+  if gpu:
+    froog_tensors = [x.to_gpu() for x in froog_tensors]
+
   out = torch_func(*torch_tensors)
   ret = froog_func(*froog_tensors)
   
-  np.testing.assert_allclose(ret.data, out.detach().numpy(), atol=atol)
+  np.testing.assert_allclose(ret.to_cpu().data, out.detach().numpy(), atol=atol)
 
-  out.mean().backward()
-  ret.mean().backward()
+  if not forward_only:
+    out.mean().backward()
+    ret.mean().backward()
 
-  for t, tt in zip(torch_tensors, froog_tensors):
-    np.testing.assert_allclose(t.grad, tt.grad, atol=grad_atol)
+    for t, tt in zip(torch_tensors, froog_tensors):
+      np.testing.assert_allclose(t.grad, tt.grad.to_cpu().data, atol=grad_atol)
 
   # test for speed
   # forward passes
-  torch_fwd = timeit.Timer(functools.partial(torch_func, *torch_tensors)).timeit(5) * 1000/5
-  froog_fwd = timeit.Timer(functools.partial(froog_func, *froog_tensors)).timeit(5) * 1000/5
+    torch_fwd = timeit.Timer(functools.partial(torch_func, *torch_tensors)).timeit(5) * 1000/5
+    froog_fwd = timeit.Timer(functools.partial(froog_func, *froog_tensors)).timeit(5) * 1000/5
 
   # backward passes
-  torch_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), torch_func, torch_tensors)).timeit(5) * 1000/5
-  froog_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), froog_func, froog_tensors)).timeit(5) * 1000/5
+  if not forward_only:
+    torch_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), torch_func, torch_tensors)).timeit(5) * 1000/5
+    froog_fbp = timeit.Timer(functools.partial(lambda f,x: f(*x).mean().backward(), froog_func, froog_tensors)).timeit(5) * 1000/5
+  else:
+    torch_fbp, froog_fbp = np.nan, np.nan
 
   print(f"shape: {repr(shape) : >32} torch/froog fwd: {torch_fwd:.2f}/{froog_fwd:.2f} ms ({float(froog_fwd/torch_fwd):.2f}x slower) bp: {torch_fbp - torch_fwd:.2f}/{froog_fbp - froog_fwd:.2f} ms ({float((froog_fbp - froog_fwd)/(torch_fbp - torch_fwd)):.2f}x slower)")
 
 
 class TestOps(unittest.TestCase):
+  # **************** Add ****************
   def test_add(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add)
+  @unittest.skipUnless(GPU, "Requires GPU")
+  def test_gpu_add(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add, gpu=True)
+  # **************** Sub ****************
   def test_sub(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub)
+  # **************** Mul ****************
   def test_mul(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul)
+  @unittest.skipUnless(GPU, "Requires GPU")
+  def test_gpu_mul(self):
+    helper_test_op([(45,65), (45,65)], lambda x,y: x*y, Tensor.mul, gpu=True)
+  # **************** Dot ****************
+  @unittest.skipUnless(GPU, "Requires GPU")
+  def test_gpu_dot(self):
+    helper_test_op([(3,4), (4,5)], lambda x,y: x.matmul(y), Tensor.dot, atol=1e-5, gpu=True)
+  # **************** Div ****************
   def test_div(self):
-    # TODO: why needs more tolerance?
-    helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div, atol=5e-5, grad_atol=2e-5)
+    helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div, atol=1e-3, grad_atol=1e-3)
+  # **************** Pow ****************
   def test_pow(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x**y, Tensor.pow)
+  # **************** Sqrt ****************
   def test_sqrt(self):
     helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt)
-    
+  # **************** Conv ****************
   def test_conv2d(self):
     for bs in [1,8]:
       for cin in [1,2,3]:
-        for H in [2,3,5]:
-          for W in [2,3,5]:
-            helper_test_op([(bs,cin,10,7), (4,cin,H,W)], 
-                    lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
-                    lambda x,w: Tensor.conv2d(x,w).relu(), 
-                    atol=2e-5, 
-                    grad_atol=2e-6)
-            
-  # TODO: doesn't work for anything but (2,2)
+        for groups in [1,3] if cin == 3 else [1]:
+          for H in [2,5]:
+            for W in [2,3,5]:
+              helper_test_op([(bs,cin,11,28), (6,cin//groups,H,W)],
+                lambda x,w: torch.nn.functional.conv2d(x,w,groups=groups).relu(),
+                lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=2e-5, grad_atol=2e-6)
+  def test_strided_conv2d(self):
+    bs = 4
+    cin = 3
+    H,W = 3,3
+    helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
+                    lambda x,w: torch.nn.functional.conv2d(x,w,stride=2).relu(),
+                    lambda x,w: Tensor.conv2d(x,w,stride=2).relu(),
+                    atol=2e-5, grad_atol=2e-6)
+    helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
+                    lambda x,w: torch.nn.functional.conv2d(x,w,stride=(2,1)).relu(),
+                    lambda x,w: Tensor.conv2d(x,w,stride=(2,1)).relu(),
+                    atol=2e-5, grad_atol=2e-6)
+
+  # **************** Max Pool ****************
   def test_maxpool_sizes(self):
     for size in [(2,2), (3,3), (3,2), (5,5), (5,1)]:
       helper_test_op([(32,2,110,28)],
         lambda x: torch.nn.functional.max_pool2d(x, kernel_size=size),
         lambda x: Tensor.max_pool2d(x, kernel_size=size))
-
   def test_maxpool2x2(self):
     helper_test_op([(32,2,110,28)], lambda x: torch.nn.functional.max_pool2d(x, (2,2)), Tensor.max_pool2d)
-
+  # **************** Avg Pool ****************
   def test_avgpool2x2(self):
     helper_test_op([(32,2,111,28)], lambda x: torch.nn.functional.avg_pool2d(x, (2,2)), Tensor.avg_pool2d)
 
-  def test_strided_conv2d(self):
-    bs = 4
-    cin = 3
-    H,W = 3,3
-    helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
-      lambda x,w: torch.nn.functional.conv2d(x,w,stride=2).relu(),
-      lambda x,w: Tensor.conv2d(x,w,stride=2).relu(), atol=2e-5, grad_atol=2e-6)
-    helper_test_op([(bs,cin,11,28), (4,cin,H,W)],
-      lambda x,w: torch.nn.functional.conv2d(x,w,stride=(2,1)).relu(),
-      lambda x,w: Tensor.conv2d(x,w,stride=(2,1)).relu(), atol=2e-5, grad_atol=2e-6)
-
 if __name__ == '__main__':
   unittest.main(verbosity=2)
```

### Comparing `froog-0.1.8/tests/test_optim.py` & `froog-0.2.0/tests/test_optim.py`

 * *Files identical despite different names*

### Comparing `froog-0.1.8/tests/test_tensor.py` & `froog-0.2.0/tests/test_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 import torch
 import unittest
-from froog.tensor import Tensor
+from froog.tensor import Tensor, GPU
 from froog.gradcheck import numerical_jacobian, gradcheck, jacobian
 
 x_init = np.random.randn(1,3).astype(np.float32)
 W_init = np.random.randn(3,3).astype(np.float32)
 m_init = np.random.randn(1,3).astype(np.float32)
 
 class TestTensor(unittest.TestCase):
-
   def test_jacobian(self):
     W = np.random.RandomState(1337).random((10, 5))
     x = np.random.RandomState(7331).random((1, 10)) - 0.5
 
     torch_x = torch.tensor(x, requires_grad=True)
     torch_W = torch.tensor(W, requires_grad=True)
     torch_func = lambda x: torch.nn.functional.log_softmax(x.matmul(torch_W).relu(), dim=1)
@@ -33,15 +32,15 @@
       x = Tensor(x_init)
       W = Tensor(W_init)
       m = Tensor(m_init)
       out = x.dot(W).relu()
       out = out.logsoftmax()
       out = out.mul(m).add(m).sum()
       out.backward()
-      return out.data, x.grad, W.grad
+      return out.data, x.grad.data, W.grad.data
 
     def test_pytorch():
       x = torch.tensor(x_init, requires_grad=True)
       W = torch.tensor(W_init, requires_grad=True)
       m = torch.tensor(m_init)
       out = x.matmul(W).relu()
       out = torch.nn.functional.log_softmax(out, dim=1)
```

