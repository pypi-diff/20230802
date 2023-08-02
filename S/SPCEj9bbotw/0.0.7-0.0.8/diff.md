# Comparing `tmp/SPCEj9bbotw-0.0.7.tar.gz` & `tmp/SPCEj9bbotw-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPCEj9bbotw-0.0.7.tar", last modified: Wed Aug  2 08:47:47 2023, max compression
+gzip compressed data, was "SPCEj9bbotw-0.0.8.tar", last modified: Wed Aug  2 17:08:42 2023, max compression
```

## Comparing `SPCEj9bbotw-0.0.7.tar` & `SPCEj9bbotw-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/
--rw-rw-rw-   0        0        0       58 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.043589 SPCEj9bbotw-0.0.7/SPCEj9bbotw/
--rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_.py
--rw-rw-rw-   0        0        0       25 2023-08-02 08:47:18.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/__init__.py
--rw-rw-rw-   0        0        0     5316 2023-08-02 08:45:53.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_main.py
--rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/_matrix.py
--rw-rw-rw-   0        0        0     8870 2023-08-01 16:21:48.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/kernels.py
--rw-rw-rw-   0        0        0     6787 2023-08-01 16:22:43.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer.py
--rw-rw-rw-   0        0        0     6788 2023-08-02 08:45:50.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer_matrix.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:47:47.052307 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/
--rw-rw-rw-   0        0        0       58 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-02 08:47:46.000000 SPCEj9bbotw-0.0.7/SPCEj9bbotw.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 08:47:47.053307 SPCEj9bbotw-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      134 2023-08-02 08:47:09.000000 SPCEj9bbotw-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.755973 SPCEj9bbotw-0.0.8/
+-rw-rw-rw-   0        0        0       58 2023-08-02 17:08:42.754973 SPCEj9bbotw-0.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.737970 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/
+-rw-rw-rw-   0        0        0       58 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-02 17:08:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.743971 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/
+-rw-rw-rw-   0        0        0       25 2023-08-02 16:59:55.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-08-02 17:07:17.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/_main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.748972 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/
+-rw-rw-rw-   0        0        0     3024 2023-08-02 08:32:13.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_.py
+-rw-rw-rw-   0        0        0        0 2023-08-02 17:03:01.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/__init__.py
+-rw-rw-rw-   0        0        0     3025 2023-08-02 08:30:42.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_matrix.py
+-rw-rw-rw-   0        0        0     2917 2023-08-02 16:51:39.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_plot.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:08:42.753974 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/
+-rw-rw-rw-   0        0        0       75 2023-08-02 17:06:27.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9055 2023-08-02 16:34:50.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/kernels.py
+-rw-rw-rw-   0        0        0     6764 2023-08-02 10:18:20.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0     6989 2023-08-02 17:02:05.000000 SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer_matrix.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 17:08:42.755973 SPCEj9bbotw-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-08-02 16:59:18.000000 SPCEj9bbotw-0.0.8/setup.py
```

### Comparing `SPCEj9bbotw-0.0.7/SPCEj9bbotw/_.py` & `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.7/SPCEj9bbotw/_matrix.py` & `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/functions/_matrix.py`

 * *Files identical despite different names*

### Comparing `SPCEj9bbotw-0.0.7/SPCEj9bbotw/kernels.py` & `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import cupy as cp
 
-def ker_main_(N):
+def ker_main_(N, NR_epoch):
     num_thread = int(11*N)
     str_ = r"""
     #define _X (blockDim.x * blockIdx.x + threadIdx.x)
     #define _Y (blockDim.y * blockIdx.y + threadIdx.y)    
     #define _Coor (_X + _Y*gridDim.x*blockDim.x)
     #include <cooperative_groups.h>
     namespace cg = cooperative_groups;
@@ -41,15 +41,15 @@
 
     __device__ float buff_w["""+ repr(num_thread) +r"""]={0.0} ;
 
     __device__ float buff["""+ repr(num_thread) +r"""]={0.0} ;
 
     __device__ float ys["""+ repr(num_thread) +r"""] ={0.0};
 
-    __device__ int NR_epoch = 1000;
+    __device__ int NR_epoch = """+repr(NR_epoch)+r""";
 
     __device__ int NR_eps = 0.001;
     
     //__device__ SCALE scale ={0, 10, 1, 1, 100, 10, 0.1, 0.1*0.2*24000, 0.1*0.8*24000};
     
 
     __device__ float NR_f(float x, float a, float b, float rho, float c){
@@ -158,14 +158,17 @@
         
         //SCALE scale;
         
         float scl_z = scales[0];
         float scl_coeff_exp_lb = scales[1];
         float scl_coeff_exp_ub = scales[2];
         float scl_coeff_cone = scales[3];
+        float scl_coeff_poiniting = scales[4];
+        
+        
 
         IDXS idxs;
         idxs.u = 11*idx; idxs.x = 11*idx+3; idxs.sig = 11*idx+9; idxs.z = 11*idx+10;
 
         IDXS res_idxs;
         res_idxs.u = 11*res_idx; res_idxs.x = 11*res_idx+3; res_idxs.sig = 11*res_idx+9; res_idxs.z = 11*res_idx+10;
         
@@ -202,16 +205,18 @@
         /*-----------------------------------------------------------------*/
         for(int iter_=0; iter_ < epoch; iter_++){
             if(idx < len_dual){
                 buff[idx] = w[idx] - ys[idx];
             }
             sync(grid);
                 
-            
-            buff_y[idx] = y_fix[idx] + func_matmulvec(&tilde_C[len_dual*idx], buff, len_dual);
+            if(idx < 11*N){
+                buff_y[idx] = y_fix[idx] + func_matmulvec(&tilde_C[len_dual*idx], buff, len_dual);
+                
+            }
         
             sync(grid);
 
             /*-----------------projection--------------------------------------*/
 
             /*-----------------linear inequality--------------------------------------------*/
             
@@ -222,17 +227,17 @@
             }
             else if(N <= idx && idx < 2*N){
                 buff_w[idx] = - buff_y[res_idxs.z]  + z_ub[res_idx+1] + ys[idx];
                 proj_lb(&buff_w[idx], 0);
                 ys[idx] = ys[idx]  -buff_y[res_idxs.z] +z_ub[res_idx+1] - buff_w[idx];
             }
             else if(2*N <= idx && idx < 3*N){
-                buff_w[idx] = buff_y[res_idxs.u] - 0*buff_y[res_idxs.sig] + ys[idx];
+                buff_w[idx] = buff_y[res_idxs.u] - scl_coeff_poiniting*buff_y[res_idxs.sig] + ys[idx];
                 proj_lb(&buff_w[idx], 0);
-                ys[idx] = ys[idx] + buff_y[res_idxs.u] - 0*buff_y[res_idxs.sig] - buff_w[idx];
+                ys[idx] = ys[idx] + buff_y[res_idxs.u] - scl_coeff_poiniting*buff_y[res_idxs.sig] - buff_w[idx];
             }
 
             /*-----------------socbp----------------------------------*/
             else if(3*N <= idx && idx < 4*N){
                 for(int i=0; i < 3; i++){
                     th_proj1[i] = buff_y[res_idxs.u+i] + th_ys[i];
                 }
```

### Comparing `SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer.py` & `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
-from SPCEj9bbotw._ import *
+from _ import *
 
 
 '''
 coefficient matrix of primal variable is calculated by cupy inverse function.
 '''
 class gpu_optimizer:
     def __init__(self, x_0, n, dt, rho, cond, g, ang_vel, epoch, func_gpu):
@@ -136,23 +136,23 @@
 
         q_tilde = sp.vstack([self.zeta, sp.csr_array((4*self.n,1)), self.b3])
         self.y_fix = sp.csr_array(sp.vstack([-h + self.rho*self.tC@q_tilde, self.beta]))
         self.y_fix_gpu = self.tilde_C_gpu[:11*self.n, :]@cp.array(self.y_fix.toarray().astype(np.float32))        
         self.tilde_C_gpu = self.tilde_C_gpu[:11*self.n, :11*self.n]@cp.array((self.rho*self.tC).toarray().astype(np.float32))
         
     def init_gpu(self):
-        self.y_gpu =  cp.array(np.zeros((11,self.n, 1)).astype(np.float32))
+        # self.y_gpu =  cp.array(p.zeros((11,self.n, 1)).astype(np.float32))
         self.acc_cmd_gpu = cp.array(np.zeros(4).astype(np.float32) )
         self.z_lb_gpu = cp.array(self.z_lb_scl.astype(np.float32))
         self.z_ub_gpu = cp.array(self.z_ub_scl.astype(np.float32))
         self.N_gpu = np.int32(self.n)
         self.scale_gpu = cp.array(np.array([self.scale['z'], self.scale['inv/sig']*self.cond['rho1'], 
                                             self.scale['inv/sig']*self.cond['rho2'],
                                             self.scale['inv/sig']*self.scale['u'][0,0]]).astype(np.float32))
         
     def admm_main(self):
-        self.func_main_((1, 11, 1), (1, self.n, 1), (self.y_gpu, self.y_fix_gpu, self.tilde_C_gpu, 
+        self.func_main_((1, 11, 1), (1, self.n, 1), (self.y_fix_gpu, self.tilde_C_gpu, 
                                                      self.z_lb_gpu, self.z_ub_gpu, self.N_gpu, self.epoch, 
                                                      self.acc_cmd_gpu, self.scale_gpu))
```

### Comparing `SPCEj9bbotw-0.0.7/SPCEj9bbotw/optimizer_matrix.py` & `SPCEj9bbotw-0.0.8/SPCEj9bbotw_/optimizer/optimizer_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import numpy as np
 import numpy.linalg as lg
 import cupy as cp
-from _matrix import *
+from functions._matrix import *
 
 
 '''
-coefficient matrix of primal variable is calculated by cupy inverse function.
+- sparse matrix type ver 
+- coefficient matrix of primal variable is calculated by cupy inverse function.
+- y_gpu just only for result plot
 '''
+
 class gpu_optimizer:
     def __init__(self, x_0, n, dt, rho, cond, g, ang_vel, epoch, func_gpu):
         self.x_0 = x_0
         self.n = n
         self.dt = dt
         self.rho = rho
         self.g = g
         self.ang_vel = ang_vel
         self.cond = cond
         self.epoch = np.int32(epoch)
         self.eps_r = 0.001
         self.eps_s = 0.001
         self.func_main_ = func_gpu
-        # self.make_mtrx/()
-        # self.init_gpu()
-        # self.func_GPU()
         
-        # self.func_main_ = ker_main_(self.n)///
         
     def next_opt(self, x_0, n, cond):
         self.x_0 = x_0
         self.n = n
         self.cond = cond
         
         
@@ -96,14 +95,15 @@
 
         tmp2 = np.zeros((self.n,1,3))
         tmp2[:,:,-1] = -1
         tmp2 = sparse.block(tmp2, (1,3), self.n)
 
         tmp3 = np.zeros((self.n,1,3))
         tmp3[:,:,0] = 1
+        tmp3[:,:,1] = -self.scale['inv/u'][0,0]*np.cos(self.cond['theta'])
         tmp3 = sparse.block(tmp3, (1,3), self.n)
 
 
         self.gamma = sp.vstack([tmp1, tmp2, tmp3])
         self.gamma = sp.csr_matrix(self.gamma)@transformation.extract((3,11), [0,9,10], self.n)
         self.tgamma = self.gamma.T
         ###############################################################################################
@@ -130,29 +130,32 @@
         self.tilde_C_gpu = cp.linalg.inv(self.tilde_C_gpu)
         
 
         ##fixed matrix for updating y
         h = sp.csr_array((11*self.n,1))
         h[-1] = -1*10
 
-        q_tilde = sp.vstack([self.zeta, sp.csr_array((4*self.n,1)), self.b3])
-        self.y_fix = sp.csr_array(sp.vstack([-h + self.rho*self.tC@q_tilde, self.beta]))
+        q_tilde = sp.vstack([self.zeta, sp.csr_matrix((4*self.n,1)), self.b3])
+        self.y_fix = sp.csr_matrix(sp.vstack([-h + self.rho*self.tC@q_tilde, self.beta]))
         self.y_fix_gpu = self.tilde_C_gpu[:11*self.n, :]@cp.array(self.y_fix.toarray().astype(np.float32))        
         self.tilde_C_gpu = self.tilde_C_gpu[:11*self.n, :11*self.n]@cp.array((self.rho*self.tC).toarray().astype(np.float32))
         
     def init_gpu(self):
         self.y_gpu =  cp.array(np.zeros((11,self.n, 1)).astype(np.float32))
         self.acc_cmd_gpu = cp.array(np.zeros(4).astype(np.float32) )
         self.z_lb_gpu = cp.array(self.z_lb_scl.astype(np.float32))
         self.z_ub_gpu = cp.array(self.z_ub_scl.astype(np.float32))
         self.N_gpu = np.int32(self.n)
-        self.scale_gpu = cp.array(np.array([self.scale['z'], self.scale['inv/sig']*self.cond['rho1'], 
-                                            self.scale['inv/sig']*self.cond['rho2'],
-                                            self.scale['inv/sig']*self.scale['u'][0,0]]).astype(np.float32))
+        
+        coeff_poiniting_scl = self.scale['inv/u'][0,0]*np.cos(self.cond['theta'])
+        self.coeff_var_gpu = cp.array(np.array([self.scale['z'], self.scale['inv/sig']*self.cond['rho1'], 
+                                                self.scale['inv/sig']*self.cond['rho2'],
+                                                self.scale['inv/sig']*self.scale['u'][0,0], 
+                                                coeff_poiniting_scl]).astype(np.float32))
         
     def admm_main(self):
         self.func_main_((1, 11, 1), (1, self.n, 1), (self.y_gpu, self.y_fix_gpu, self.tilde_C_gpu, 
                                                      self.z_lb_gpu, self.z_ub_gpu, self.N_gpu, self.epoch, 
-                                                     self.acc_cmd_gpu, self.scale_gpu))
+                                                     self.acc_cmd_gpu, self.coeff_var_gpu))
```

