# Comparing `tmp/SPCEj9bbotw-0.0.6.tar.gz` & `tmp/SPCEj9bbotw-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.6.tar", last modified: Wed Aug  2 04:31:54 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.0.7.tar", last modified: Wed Aug  2 08:47:47 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.6.tar` & `SPCEj9bbotw-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:31:54.833641 SPCEj9bbotw-0.0.6/
--rw-rw-rw-   0        0        0       58 2023-08-02 04:31:54.833641 SPCEj9bbotw-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 04:31:54.819637 SPCEj9bbotw-0.0.6/SPCEj9bbotw/
--rw-rw-rw-   0        0        0     3028 2023-06-14 07:31:18.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw/_.py
--rw-rw-rw-   0        0        0       25 2023-08-02 04:31:45.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw/__init__.py
--rw-rw-rw-   0        0        0     5214 2023-08-02 04:30:29.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw/_main.py
--rw-rw-rw-   0        0        0     8870 2023-08-01 16:21:48.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw/kernels.py
--rw-rw-rw-   0        0        0     6787 2023-08-01 16:22:43.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw/optimizer.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:31:54.831642 SPCEj9bbotw-0.0.6/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-02 04:31:54.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-08-02 04:31:54.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:31:54.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 04:31:54.000000 SPCEj9bbotw-0.0.6/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 04:31:54.833641 SPCEj9bbotw-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-08-02 04:31:36.000000 SPCEj9bbotw-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/
+-rw-rw-rw-   0        0        0       58 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.043589 SPCEj9bbotw-0.0.7/SPCEj9bbotw/
+-rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_.py
+-rw-rw-rw-   0        0        0       25 2023-08-02 08:47:18.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/__init__.py
+-rw-rw-rw-   0        0        0     5316 2023-08-02 08:45:53.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_main.py
+-rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_matrix.py
+-rw-rw-rw-   0        0        0     8870 2023-08-01 16:21:48.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/kernels.py
+-rw-rw-rw-   0        0        0     6787 2023-08-01 16:22:43.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer.py
+-rw-rw-rw-   0        0        0     6788 2023-08-02 08:45:50.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer_matrix.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.052307 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-08-02 08:47:09.000000 SPCEj9bbotw-0.0.7/setup.py
```

### Comparing `SPCEj9bbotw-0.0.6/SPCEj9bbotw/_.py` & `SPCEj9bbotw-0.0.7/SPCEj9bbotw/_.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,16 @@
 class sparse:
     def __init__(self):
         return
     
     def block(data, blocksize, n):
         indptr = np.arange(n+1)
         indices = np.arange(n)
-        return sp.bsr_array((data,indices, indptr), blocksize=blocksize, shape=n*np.array(blocksize)).tocsr()      
+        return sp.bsr_array((data,indices, indptr), blocksize=blocksize, shape=n*np.array(blocksize)).tocsr()
+
 
 class INDEX:
     def __init__(self):
         return
     
     def IDXV(tf_n):  #return index arr for vec
         idxv = []
```

### Comparing `SPCEj9bbotw-0.0.6/SPCEj9bbotw/_main.py` & `SPCEj9bbotw-0.0.7/SPCEj9bbotw/_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
-# from SPCEj9bbotw.kernels import *
-# from SPCEj9bbotw.optimizer import *
-from optimizer import gpu_optimizer
-from kernels import ker_main_
+from SPCEj9bbotw.kernels import *
+from optimizer_matrix import *
+
+# from SPCEj9bbotw.optimizer_matrix import *
+# from optimizer import gpu_optimizer
+# from kernels import ker_main_
 import time
 import matplotlib.pyplot as plt
 
 def plot(optimizer):
     y = cp.asnumpy(optimizer.y_gpu)
     # print(type(optimizer.y_gpu))
     u = optimizer.scale['u']@(y.reshape(-1,11)[:,:3]).T
@@ -100,15 +102,15 @@
     axes[2,2].set_title(r'$x \ dynamics$')
 
 
     print('required fuel', np.exp(z[0]) - np.exp(z[-1]))
     plt.show()
 
 
-x_0 =np.array([2, 2, 1.5, -0.3, 0, 0])[:,np.newaxis]
+x_0 =np.array([2, 2, 1.5, 0, 0, 0])[:,np.newaxis]
 x_des = np.zeros(6)
 n = 50
 dt = 0.1
 
 init_cond = {'m_0': 0.03, 'm_f': 0.003, 'rho1': 9.5*0.03, 'rho2': 9.9*0.03, 'T_max': 24000, 'alpha': 5e-9, 
             'theta': np.deg2rad(90)}
 g = np.array([-9.81, 0, 0])
@@ -125,21 +127,24 @@
 
 stream = cp.cuda.Stream()
 func_gpu = ker_main_(n)
 
 
 optimizer = gpu_optimizer(x_0, n, dt, 20, init_cond, g, ang_vel, 1000, func_gpu)
 
-for i in range(45):
+for i in range(1):
+    t1 = time.time()
     optimizer.next_opt(x_0, n, init_cond)
     optimizer.scaling((scl_pos, scl_vel, scl_u, scl_sig, scl_z))
     optimizer.make_mtrx()
     optimizer.init_gpu()
     optimizer.admm_main()
-    print(i)
+    t2 = time.time()
+    
+    print(i, t2 - t1)
     acc_cmd = cp.asnumpy(optimizer.acc_cmd_gpu)[:,np.newaxis]
     acc_cmd[:3,:] = optimizer.scale['u']@acc_cmd[:3,:]
     acc_cmd[-1,:] = optimizer.scale['sig']*acc_cmd[-1,:]
     
     
     x_0 = optimizer.A@x_0 + optimizer.B@(acc_cmd[:3,:] + g[:,np.newaxis])
     init_cond['m_0'] = np.exp(np.log(init_cond['m_0']) - init_cond['alpha']*dt*acc_cmd[-1,0])
@@ -151,11 +156,13 @@
     #     a = input('')
     #     print(cp.asnumpy(optimizer.y_gpu))
     # print('start', x_0)
     # print(i, n, x_0, init_cond['m_0'])
     # print(acc_cmd)
 optimizer.epoch = 0
 optimizer.admm_main()
+
+
 # print(cp.asnumpy(optimizer.y_gpu))
 plot(optimizer)
     # a = input('')
```

### Comparing `SPCEj9bbotw-0.0.6/SPCEj9bbotw/kernels.py` & `SPCEj9bbotw-0.0.7/SPCEj9bbotw/kernels.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.6/SPCEj9bbotw/optimizer.py` & `SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer.py`

 * *Files identical despite different names*

