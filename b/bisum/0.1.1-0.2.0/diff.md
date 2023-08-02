# Comparing `tmp/bisum-0.1.1.tar.gz` & `tmp/bisum-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/julio/Desktop/bisum/dist/.tmp-z71p3ngb/bisum-0.1.1.tar", last modified: Thu Jul 27 00:30:05 2023, max compression
+gzip compressed data, was "/home/julio/Desktop/bisum/dist/.tmp-a9s02k8y/bisum-0.2.0.tar", last modified: Wed Aug  2 00:15:16 2023, max compression
```

## Comparing `bisum-0.1.1.tar` & `bisum-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/
--rw-rw-r--   0 julio     (1000) julio     (1000)     1071 2023-07-26 22:53:26.000000 bisum-0.1.1/LICENSE
--rw-rw-r--   0 julio     (1000) julio     (1000)       26 2023-07-26 23:40:19.000000 bisum-0.1.1/MANIFEST.in
--rw-rw-r--   0 julio     (1000) julio     (1000)     2030 2023-07-27 00:30:05.000000 bisum-0.1.1/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)     1387 2023-07-27 00:29:17.000000 bisum-0.1.1/README.md
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum/
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-26 22:53:26.000000 bisum-0.1.1/bisum/__init__.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     3345 2023-07-26 23:58:42.000000 bisum-0.1.1/bisum/bisum.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     2246 2023-07-26 23:59:03.000000 bisum-0.1.1/bisum/dense_intra.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     6508 2023-07-26 22:53:26.000000 bisum-0.1.1/bisum/generic_functions.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     5560 2023-07-26 23:59:24.000000 bisum-0.1.1/bisum/labels.py
--rw-rw-r--   0 julio     (1000) julio     (1000)    10331 2023-07-27 00:20:46.000000 bisum-0.1.1/bisum/sparse_intra.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     9238 2023-07-26 23:59:35.000000 bisum-0.1.1/bisum/tensor_to_matrix.py
--rw-rw-r--   0 julio     (1000) julio     (1000)     9689 2023-07-26 23:59:41.000000 bisum-0.1.1/bisum/tensordot.py
-drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/
--rw-rw-r--   0 julio     (1000) julio     (1000)     2030 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/PKG-INFO
--rw-rw-r--   0 julio     (1000) julio     (1000)      356 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/SOURCES.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/dependency_links.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/requires.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-07-27 00:30:05.000000 bisum-0.1.1/bisum.egg-info/top_level.txt
--rw-rw-r--   0 julio     (1000) julio     (1000)       79 2023-07-27 00:30:05.000000 bisum-0.1.1/setup.cfg
--rw-rw-r--   0 julio     (1000) julio     (1000)     1586 2023-07-27 00:06:38.000000 bisum-0.1.1/setup.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-08-02 00:15:16.000000 bisum-0.2.0/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1071 2023-07-26 22:53:26.000000 bisum-0.2.0/LICENSE
+-rw-rw-r--   0 julio     (1000) julio     (1000)       26 2023-07-26 23:40:19.000000 bisum-0.2.0/MANIFEST.in
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3909 2023-08-02 00:15:16.000000 bisum-0.2.0/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1548 2023-08-02 00:03:29.000000 bisum-0.2.0/README.md
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1730 2023-08-01 23:30:24.000000 bisum-0.2.0/bisum/__init__.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3584 2023-07-31 19:12:48.000000 bisum-0.2.0/bisum/bisum.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     2633 2023-07-31 19:28:47.000000 bisum-0.2.0/bisum/dense_intra.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     6508 2023-07-26 22:53:26.000000 bisum-0.2.0/bisum/generic_functions.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     5636 2023-07-31 19:47:53.000000 bisum-0.2.0/bisum/labels.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)    10484 2023-08-02 00:06:59.000000 bisum-0.2.0/bisum/sparse_intra.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     9238 2023-07-26 23:59:35.000000 bisum-0.2.0/bisum/tensor_to_matrix.py
+-rw-rw-r--   0 julio     (1000) julio     (1000)     9720 2023-08-01 23:56:55.000000 bisum-0.2.0/bisum/tensordot.py
+drwxrwxr-x   0 julio     (1000) julio     (1000)        0 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/
+-rw-rw-r--   0 julio     (1000) julio     (1000)     3909 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/PKG-INFO
+-rw-rw-r--   0 julio     (1000) julio     (1000)      352 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/SOURCES.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        1 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/dependency_links.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/requires.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)        6 2023-08-02 00:15:16.000000 bisum-0.2.0/bisum.egg-info/top_level.txt
+-rw-rw-r--   0 julio     (1000) julio     (1000)     1327 2023-08-02 00:12:25.000000 bisum-0.2.0/pyproject.toml
+-rw-rw-r--   0 julio     (1000) julio     (1000)       38 2023-08-02 00:15:16.000000 bisum-0.2.0/setup.cfg
```

### Comparing `bisum-0.1.1/LICENSE` & `bisum-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bisum-0.1.1/README.md` & `bisum-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-# bisum
+# bisum --- PyTorch Sparse-Tensor Partial-Trace
+
+[![CI](https://github.com/jcandane/bisum/actions/workflows/gh-ci.yaml/badge.svg)](https://github.com/jcandane/bisum/actions/workflows/gh-ci.yaml)
 
-PyTorch Sparse-Tensor Partial-Trace
 This program traces 2 sparse-tensor (torch.tensor objects) via 3 Tracing-Prescription:
 1. {einsum} string (like numpy, str, labelling each tensor axis)
 2. ncon (used in the tensor-network community, list of 1d int torch.tensor, labelling each tensor axis)
 3. adjacency-matrix (as in numpy.tensordot, (2,n) 2d int torch.tensor, with n being the number of indices idenified between the two tensors)
 
 ## API
 
 Let's begin by initializing the 2 tensors, we can initialize random-sparse-tensors 
 ```python
-from bisum.bisum import bisum
 import torch
+from bisum import bisum
 
 shape_A = torch.tensor([8,7,7,4,11,6])
 shape_B = torch.tensor([9,7,3,7,11,8])
 A = torch.rand(shape_A)
 B = torch.rand(shape_B)
 ```
 
 Suppose we would like to compute the following partial-trace/tensor-contraction $C_{njwl} = A_{iksndj} B_{wklsdi}$:
 ```python
 C_einsum = bisum("iksndj, wklsdi -> njwl", A, B)
 C_ncon   = bisum([[-1,-2,-3,4,-5,6],[1,-2,3,-3,-5,-1]], A, B)
 C_adjmat = bisum(torch.tensor([[0,1,2,4],[5,1,3,4]]), A, B)
 
-print( torch.allclose(C_einsum, C_ncon) and torch.allclose(C_ncon, C_adjmat) )
+print(torch.allclose(C_einsum, C_ncon) and torch.allclose(C_ncon, C_adjmat))
 ```
 while the pure tensor-product, $\otimes$ is:
 ```python
+import numpy as np
+
 C_einsum = bisum("abcdef, ghijkl", A, B)
 C_ncon   = bisum([], A, B)
 C_adjmat = bisum(torch.tensor([]), A, B)
 
-print( np.allclose(C_einsum, C_ncon) and np.allclose(C_ncon, C_adjmat) )
+print(np.allclose(C_einsum, C_ncon) and np.allclose(C_ncon, C_adjmat))
 ```
 
 ## Install
 
 ```bash
 pip install bisum
 ```
```

### Comparing `bisum-0.1.1/bisum/bisum.py` & `bisum-0.2.0/bisum/bisum.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 
 def bisum(Rx, a, b):
     """
 
     """
     if torch.is_tensor(Rx): # and Rx.shape[0]==2:  # is adj.matrix (no post transpose nor slice) 
         if (not a.is_sparse) and (not b.is_sparse): ## both dense
-            c = torch.tensordot(a, b, dims=Rx)
+            if torch.numel(Rx)==0:
+                c = torch.tensordot(a, b, dims=0)
+            else:
+                c = torch.tensordot(a, b, dims=Rx)
         else:
             if (a.is_sparse) and (b.is_sparse):
                 c = ss_tensordot(a, b, dims=Rx)
             else:
                 c = sd_tensordot(a, b, dims=Rx)
 
     else:
@@ -37,15 +40,18 @@
             else:
                 raise ValueError("tracing instructions are not valid")
 
         if (not a.is_sparse) and (not b.is_sparse): ## both dense
             a = den_tensor_intraTr(a, LHS[0], inTr[0])
             b = den_tensor_intraTr(b, LHS[1], inTr[1])
 
-            c = torch.tensordot(a, b, dims=adjmat)
+            if torch.numel(adjmat)==0:
+                c = torch.tensordot(a, b, dims=0)
+            else:
+                c = torch.tensordot(a, b, dims=adjmat)
 
             c = den_post_intraTr(c, rhs)
             c = den_post_trans(c, rhs, RHS) #for dense
         else:
             if a.is_sparse and b.is_sparse: ## both sparse
                 
                 a_index, a_data, a_shape = spa_tensor_intraTr_(a, LHS[0], inTr[0])
@@ -70,10 +76,10 @@
                     a = den_tensor_intraTr(a, LHS[0], inTr[0])
                     #b = spa_tensor_intraTr(b, LHS[1], inTr[1]) ##!!!
                     b_index, b_data, b_shape = spa_tensor_intraTr_(b, LHS[1], inTr[1])
 
                     #c = sd_tensordot(a, b, dims=adjmat) ##!!!
                     c = ds_tensordot_(a, b_index, b_data, b_shape, dims=adjmat)
                     
-                    c = den_post_intraTr(c, rhs)
+                    c = den_post_intraTr(c, rhs) ### if empty skip...
                     c = den_post_trans(c, rhs, RHS)
     return c
```

### Comparing `bisum-0.1.1/bisum/dense_intra.py` & `bisum-0.2.0/bisum/dense_intra.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 This contains functions for processing dense tensor intra-operations (slicing & tracing).
 """
 
 import torch
 from .generic_functions import first_occurrence_mask, pytorch_delete, iargsort
 
+@torch.jit.script
+def remove_ones(a):
+    new_shape = torch.tensor( a.shape, dtype=torch.int64 , device=a.device)
+    new_shape = new_shape[new_shape!=1]
+    return a.reshape([int(i.item()) for i in new_shape])
+
 ### given LHS && intra-traces compute reduced/sliced sparse-tensor
 @torch.jit.script
 def den_post_trans(a, rhs, RHS):
     if torch.numel(RHS)>0:
         rhs=rhs[first_occurrence_mask(rhs)]
         j  = torch.argsort(rhs)
         k  = torch.argsort(RHS)
@@ -24,26 +30,31 @@
     """
     GIVEN : a (torch.tensor{dense})
             label (1d-int-torch.tensor)
             intratrace (1d-int-torch.tensor)
     GET   : a (torch.tensor{dense}, intratraced and sliced)
             label (1d-int-torch.tensor, with duplicates and intraTr removed, keeping org. order)
     """
-    if torch.numel(label)>0: ## if not empty, its a tensor....
+    a = remove_ones(a) ### remove axes which have dimension 1
+    b = torch.unique(label)
+    if (b.shape == label.shape): ## no repeats proceed
+        return a
+    #if torch.numel(label)>0: ## if not empty, its a tensor....
+    else:
         in_string = ""
         for i in label:
             in_string+=chr(i)
 
         out_string = ""
         label = label[first_occurrence_mask(label)]
         for i in label:
             out_string+=chr(i)
         return torch.einsum(in_string + "->" + out_string, a) #, label
-    else: ## its a scalar return itself
-        return a
+    #else: ## its a scalar return itself
+    #    return a
 
 @torch.jit.script
 def den_tensor_intraTr(a, label, intratrace):
     """
     GIVEN : a (torch.tensor{dense})
             label (1d-int-torch.tensor)
             intratrace (1d-int-torch.tensor)
```

### Comparing `bisum-0.1.1/bisum/generic_functions.py` & `bisum-0.2.0/bisum/generic_functions.py`

 * *Files identical despite different names*

### Comparing `bisum-0.1.1/bisum/labels.py` & `bisum-0.2.0/bisum/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,34 @@
             RHS (1d-int-torch.tensor labelling external indices of output tensor)
             intratraces (List[1d-int-torch.tensors] labelling each tensor, in intra-interal-indices)
     """
 
     liststring    = einsum_string.replace(" ","").split("->") ## this is a list (at most 2 entries: LHS, RHS)
     if len(liststring)==2: ## RHS given
         LHS = liststring[0].split(",")
-        LHS = [torch.tensor([ord(char) for char in word], device=device) for word in LHS]
-        RHS =  torch.tensor([ord(char) for char in liststring[1]], device=device)
+        LHS = [torch.tensor([ord(char) for char in word], dtype=torch.int64, device=device) for word in LHS]
+        RHS =  torch.tensor([ord(char) for char in liststring[1]], dtype=torch.int64, device=device)
 
         global_internal, counts = torch.unique(torch.concat([torch.unique(lhs) for lhs in LHS]), return_counts=True)
         global_internal = global_internal[counts == len(LHS)]
         not_these       = torch.concat([global_internal, RHS]) ## for intraintersect
 
         intratraces=[] ## over each value of
         for lhs in LHS:
             unique_values, counts = torch.unique(lhs, return_counts=True) ## intra-dupes
             unique_values = unique_values[torch.all(torch.ne(unique_values.unsqueeze(1), not_these.unsqueeze(0)),1)]
             intratraces.append( torch.unique(unique_values) )
 
     else: #if len(liststring)==1: ## no RHS, go reg. convention (repeats are dummies)
         LHS = liststring[0].split(",") ## should be at most 2-here
-        LHS = [torch.tensor([ord(char) for char in word], device=device) for word in LHS]
+        LHS = [torch.tensor([ord(char) for char in word], dtype=torch.int64, device=device) for word in LHS]
 
         ### build RHS-label
         RHS   = liststring[0].replace(",","")
-        RHS   = torch.tensor([ord(char) for char in RHS], device=device)
+        RHS   = torch.tensor([ord(char) for char in RHS], dtype=torch.int64, device=device)
         unique_values, counts = torch.unique(RHS, return_counts=True)
         dupes = unique_values[counts > 1]     # Filter-out duplicate values, gather
         mask  = torch.logical_not(torch.any(torch.eq(RHS.unsqueeze(1), dupes.unsqueeze(0)), 1))
         RHS   = RHS[mask] ## in org. order
 
         global_internal, counts = torch.unique(torch.concat([torch.unique(lhs) for lhs in LHS]), return_counts=True)
         global_internal = global_internal[counts == len(LHS)]
```

### Comparing `bisum-0.1.1/bisum/sparse_intra.py` & `bisum-0.2.0/bisum/sparse_intra.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,29 +241,30 @@
 
             return index, data, shape_
         else:
             #data = torch.unsqueeze(torch.unsqueeze(data, 0),0) ## !!!!
             #return torch.zeros_like(data[:,:,0], dtype=torch.int64), torch.sum(data), torch.ones_like(data[:,0,0]) ###!!!
             return torch.zeros((1,1), device=index.device, dtype=index.dtype), torch.sum(torch.unsqueeze(data, 0), dim=1), torch.ones(1, device=shape_.device, dtype=shape_.dtype) #
 
-
-#@torch.jit.script
+@torch.jit.script
 def spa_post_trans_(index, data, shape_, rhs, RHS):
-    rhs=rhs[first_occurrence_mask(rhs)]
-    j = torch.argsort(rhs)
-    k = torch.argsort(RHS)
-    ik= iargsort(k)
-    m = j[ik]
-
-    cc= index[m,:]
-    s = shape_[m]
-    n = lexsort( cc )
-
-    return torch.sparse_coo_tensor( cc[:,n] , data[n], [int(i.item()) for i in s]) ## .type(torch.LongTensor) not needed
-
+    if torch.numel(RHS)>0:
+        rhs=rhs[first_occurrence_mask(rhs)]
+        j = torch.argsort(rhs)
+        k = torch.argsort(RHS)
+        ik= iargsort(k)
+        m = j[ik]
+
+        cc= index[m,:]
+        s = shape_[m]
+        n = lexsort( cc )
+
+        return torch.sparse_coo_tensor( cc[:,n] , data[n], [int(i.item()) for i in s])
+    else: ## a is a scalar (cannot permute)
+        return torch.sparse_coo_tensor( index , data, [int(i.item()) for i in shape_])
 
 
 ### TESTS
 #from uniform_random_sparse_tensor import uniform_random_sparse_tensor
 
 #shape = torch.tensor([2,2,2,3])
 #A = uniform_random_sparse_tensor(torch.prod(shape), shape)
```

### Comparing `bisum-0.1.1/bisum/tensor_to_matrix.py` & `bisum-0.2.0/bisum/tensor_to_matrix.py`

 * *Files identical despite different names*

### Comparing `bisum-0.1.1/bisum/tensordot.py` & `bisum-0.2.0/bisum/tensordot.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,17 +189,16 @@
     GET   : c (torch.tensor{dense} XOR torch.tensor{sparse} is just direct-product)
     """
     if dims.numel()==0: ## directproduct
         c = ds_outer_(a, b_index, b_data, b_shape)
     else: ## directintersection
         # a is dense && b is sparse
         m_A, exlabel_A = dn_tensor_to_matrix(a, dims[0], left=False ) ## True
-        m_B, exlabel_B = rawsp_tensor_to_matrix(b_index, b_data, b_shape, dims[1], left=False)
+        m_B, exlabel_B = rawsp_tensor_to_matrix(b_index, b_data, b_shape, dims[1], left=True)
         
-        #m_B, exlabel_B = sp_tensor_to_matrix(b, dims[1], left=True ) ## False
         c = m_B @ m_A ### SPARSE is first??!?
         c = c.T.reshape( [ int(i) for i in torch.concat([torch.flatten(exlabel_B), torch.flatten(exlabel_A)])])
     return c
 
 @torch.jit.script
 def sd_tensordot_(a_index, a_data, a_shape, b, dims=None):
     """
@@ -210,9 +209,10 @@
     """
     if dims.numel()==0: ## directproduct
         c = sd_outer_(a_index, a_data, a_shape, b)
     else: ## directintersection
         m_A, exlabel_A = rawsp_tensor_to_matrix(a_index, a_data, a_shape, dims[0], left=True ) ## True
         m_B, exlabel_B = dn_tensor_to_matrix(b, dims[1], left=False  ) ## False
         c = m_A @ m_B ## Sparse is 1st
-        c = c.reshape([int(i) for i in torch.concat([exlabel_A, exlabel_B])])
+        #c = c.reshape([int(i) for i in torch.concat([exlabel_A, exlabel_B])])
+        c = c.reshape( [ int(i) for i in torch.concat([torch.flatten(exlabel_B), torch.flatten(exlabel_A)])])
     return c
```

