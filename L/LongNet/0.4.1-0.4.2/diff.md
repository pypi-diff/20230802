# Comparing `tmp/LongNet-0.4.1.tar.gz` & `tmp/LongNet-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.4.1.tar", last modified: Mon Jul 17 19:55:20 2023, max compression
+gzip compressed data, was "LongNet-0.4.2.tar", last modified: Wed Aug  2 15:17:42 2023, max compression
```

## Comparing `LongNet-0.4.1.tar` & `LongNet-0.4.2.tar`

### file list

```diff
@@ -1,59 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 19:55:10.000000 LongNet-0.4.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/Transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionV2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionv5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/torchscale/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/torchscale/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/component/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/droppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/feedforward_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/multiway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/relative_position_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/component/xmoe/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/global_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/moe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xpos_relative_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/model/BEiT3.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-17 19:55:20.961530 LongNet-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-17 19:55:10.000000 LongNet-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:55:20.961530 LongNet-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 19:55:10.000000 LongNet-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-17 19:55:10.000000 LongNet-0.4.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:17:42.646302 LongNet-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 15:17:30.000000 LongNet-0.4.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:17:42.646302 LongNet-0.4.2/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:17:42.646302 LongNet-0.4.2/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DilatedAttentionV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DilatedAttentionv5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/MultiHead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23295 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10259 2023-08-02 15:17:30.000000 LongNet-0.4.2/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:17:42.646302 LongNet-0.4.2/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 15:17:42.000000 LongNet-0.4.2/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-02 15:17:42.000000 LongNet-0.4.2/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:17:42.000000 LongNet-0.4.2/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 15:17:42.000000 LongNet-0.4.2/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 15:17:42.000000 LongNet-0.4.2/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-08-02 15:17:42.646302 LongNet-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14368 2023-08-02 15:17:30.000000 LongNet-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:17:42.646302 LongNet-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 15:17:30.000000 LongNet-0.4.2/setup.py
```

### Comparing `LongNet-0.4.1/LICENSE` & `LongNet-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.1/LongNet/Transformer.py` & `LongNet-0.4.2/LongNet/Transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-import math
 import functools
 from itertools import zip_longest
 
 import torch
 import torch.nn.functional as F
-from torch import nn, einsum
+from torch import nn
 
-from einops import rearrange, reduce, repeat, pack, unpack
+from einops import rearrange, repeat, pack, unpack
 from einops.layers.torch import Rearrange
 
 from beartype import beartype
 from beartype.typing import Tuple, Union
 
 # from LongNet_pytorch.attfend import Attend
 from LongNet.attention import DilatedAttention as Attention
@@ -160,15 +159,15 @@
                 FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
         self.norm = RMSNorm(dim)
 
     def forward(self, x):
         n = x.shape[-2]
-        rotary_emb = self.rotary_emb(n) if exists(self.rotary_emb) else None
+        self.rotary_emb(n) if exists(self.rotary_emb) else None
 
         for attn, ff in self.layers:
             x = attn(token_shift(x)) + x  # rotary_emb removed as it's not supported in DilatedAttention
             x = ff(token_shift(x)) + x
 
         return self.norm(x)
 
@@ -307,15 +306,14 @@
         return self.to_logits(tokens)
 
     def forward(self, ids, return_loss = False):
         batch = ids.shape[0]
 
         assert ids.ndim in {2, self.stages + 1}
         flattened_dims = ids.ndim == 2
-        ids_orig_ndim = ids.ndim
 
         if ids.numel() == 0:
             return self.forward_empty(ids.shape[0])
 
         if flattened_dims:
             # allow for ids to be given in the shape of (batch, seq)
             # in which case it will be auto-padded to the next nearest multiple of depth seq len
```

### Comparing `LongNet-0.4.1/LongNet/attend.py` & `LongNet-0.4.2/LongNet/attend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-from torch._C import dtype
-# !pip install torch
-# !pip install einops
 
-import math
 from collections import namedtuple
 from functools import wraps
 from packaging import version
 
 import torch
 from torch import nn, einsum, Tensor
 import torch.nn.functional as F
@@ -202,36 +198,7 @@
 
         # aggregate values
 
         out = einsum(f"b h i j, {kv_einsum_eq} -> b h i d", attn, v)
 
         return out
     
-import torch
-from collections import namedtuple
-from einops import rearrange
-
-EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
-
-class FlashMHA(nn.Module):
-    def __init__(self, embed_dim, num_heads, bias=True, batch_first=True, dropout=0.0,
-                 causal=False, device=None, dtype=None) -> None:
-        assert batch_first
-        factory_kwargs = {'device': device, 'dtype': dtype}
-        super().__init__()
-        self.embed_dim = embed_dim
-        self.causal = causal
-
-        self.num_heads = num_heads
-        assert self.embed_dim % num_heads == 0, "self.kdim must be divisible by num_heads"
-        self.head_dim = self.embed_dim // num_heads
-        assert self.head_dim % 8 == 0 and self.head_dim <= 128, "Only support head_dim <= 128 and divisible by 8"
-
-        self.Wqkv = nn.Linear(embed_dim, 3 * embed_dim, bias=bias, **factory_kwargs)
-        self.inner_attn = FlashAttention(dropout=dropout, causal=causal)
-        self.out_proj = nn.Linear(embed_dim, embed_dim, bias=bias, **factory_kwargs)
-
-    def forward(self, query, key, value):
-        qkv = self.Wqkv(query)
-        q, k, v = rearrange(qkv, 'b s (three h d) -> three b s h d', three=3, h=self.num_heads, d=self.head_dim).unbind(dim=0)
-        context = self.inner_attn(q, k, v)
-        return self.out_proj(rearrange(context, 'b s h d -> b s (h d)'))
```

### Comparing `LongNet-0.4.1/LongNet/attention.py` & `LongNet-0.4.2/LongNet/iterations/DynamicDilatedAttention.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,135 +1,99 @@
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
-from torch.nn.parallel import DataParallel
 
 from LongNet.utils import XPOS, RelativePositionBias
-
 from LongNet.attend import FlashAttention
 
+# Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
 
-#add alibi, qk layer norm, one write head, multihway, 
-class DilatedAttention(nn.Module):
-    """
-    Dilated Attention Module.
-
-    Arguments:
-        d_model: The dimension of the attention layers.
-        num_heads: The number of attention heads.
-        dilation_rate: The dilation rate for dilated attention.
-        segment_size: The segment size for dilated attention.
-        dropout (optional): The dropout probability. Default: 0.0
-        casual (optional): If set to True, the attention mechanism is casual. Default: False
-        use_xpos (optional): If set to True, xpos is used for positional encoding. Default: False
-        use_rel_pos_bias (optional): If set to True, relative position bias is used in the attention mechanism. Default: False
-
-    Usage:
-        The `DilatedAttention` class can be used as a module for neural networks and is especially suited for transformer architectures.
-
-        Example:
-            attention = DilatedAttention(d_model=512, num_heads=8, dilation_rate=2, segment_size=64, use_xpos=True, use_rel_pos_bias=True)
-            output = attention(input_tensor)
-
-        This will return the output tensor after applying dilated attention. The `use_xpos` and `use_rel_pos_bias` parameters allow for switching on positional encoding and relative positional bias respectively.
-    """
-    def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
-        super(DilatedAttention, self).__init__()
+
+class DynamicDilatedAttention(nn.Module):
+    def __init__(self, d_model, num_heads, num_rates, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
+        super(DynamicDilatedAttention, self).__init__()
         self.d_model = d_model
         self.num_heads = num_heads
+        self.casual = casual  # Define this before FlashAttention
 
-        self.dilation_rate = dilation_rate
-        self.segment_size = segment_size
+        # Generate geometric sequences for dilation rates and segment sizes
+        self.dilation_rates = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
+        self.segment_sizes = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
 
+        self.attention = [FlashAttention(causal=self.casual, dropout=dropout).to(device) for _ in range(num_rates)] # Corrected here]
         self.dropout = nn.Dropout(dropout)
-        self.casual = casual
 
         self.use_xpos = use_xpos
         self.use_rel_pos_bias = use_rel_pos_bias
 
-        self.attention = FlashAttention(causal=self.casual, dropout=dropout).to(device)
-
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
         if use_rel_pos_bias:
             self.relative_bias = RelativePositionBias(num_buckets=32, max_distance=128, n_heads=num_heads)
 
-        #head offsets
-        self.head_offsets = nn.Parameter(torch.randn(num_heads, d_model))
+        self.softmax = nn.Softmax(dim=-1)
 
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
-
+    
     def forward(self, x):
+        # Get batch size, sequence length and model dimension
         batch_size, seq_len, _ = x.shape
+        print(f'x.shape: {x.shape}')  # Print the shape of the input tensor
 
         if self.use_xpos:
             x = self.xpos(x)
-        
-        # Split and sparsify
-        x = x.view(batch_size, -1, self.segment_size, self.d_model)
-        x = x[:, :, :: self.dilation_rate, :]
-
-        # Perform attention
-        attn_output = self.attention(x, x, x)
-
-        #if use rel pos => apply relative positioning bias 
-        if self.use_rel_pos_bias:
-            attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
-        # if casual create a mask and apply to the output
-        if self.casual:
-            mask = self.get_mask(attn_output.size(1), attn_output.size(1))
-            attn_output = attn_output.masked_fill(mask, float('-inf'))
+        # Initialize tensor to store outputs
+        outputs = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
+        print(f'outputs.shape: {outputs.shape}')  # Print the shape of the outputs tensor
 
-        # apply dropout
-        attn_output = self.dropout(attn_output)
+        # Initialize tensor to store softmax denominators
+        softmax_denominators = torch.zeros((batch_size, seq_len, self.num_heads), device=device, dtype=dtype)
 
-        # Scatter and concatenate 
-        attn_output = attn_output.reshape(batch_size, -1, self.d_model)
-        return attn_output
+        for head_idx, attention in enumerate(self.attention):
+            dilation_rate = self.dilation_rates[head_idx]
+            segment_size = self.segment_sizes[head_idx]
 
+            for offset in range(dilation_rate):
+                x_ = x[:, offset::dilation_rate, :]  # Apply offset for each head
+                x_ = x_.contiguous().view(batch_size, -1, segment_size, self.d_model)
+                print(f'x_.shape: {x_.shape}')  # Print the shape of the reshaped input tensor
 
-class MultiHeadDilatedAttention:
-    def __init__():
-        pass
+                attn_output, attn_weights, *_ = attention(x_, x_, x_)  # Collect all additional return values into a list
+                print(f'attn_output.shape: {attn_output.shape}')  # Print the shape of the attention output tensor
 
+                if self.use_rel_pos_bias:
+                    attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
+                if self.casual:
+                    mask = self.get_mask(attn_output.size(1), attn_output.size(1))
+                    attn_output = attn_output.masked_fill(mask, float('-inf'))
 
+                attn_output = self.dropout(attn_output)
 
+                # Prepare output for addition
+                attn_output_reshaped = attn_output.contiguous().view(batch_size, -1, self.d_model)
+                print(f'attn_output_reshaped.shape: {attn_output_reshaped.shape}')  # Print the shape of the reshaped attention output tensor
 
+                # Prepare the slice of outputs for addition
+                outputs_slice = outputs[:, offset::dilation_rate, :attn_output.shape[1]*dilation_rate]
+                print(f'outputs_slice.shape: {outputs_slice.shape}')  # Print the shape of the slice of outputs
 
+                # Add output to the corresponding positions in the outputs tensor
+                outputs_slice += attn_output_reshaped
+                print(f'outputs.shape after addition: {outputs.shape}')  # Print the shape of the outputs tensor after addition
 
-class LongNetTransformer(nn.Module):
-    def __init__(self, d_model, num_heads, dilation_rates, segment_sizes):
-        super(LongNetTransformer, self).__init__()
-        assert len(dilation_rates) == len(segment_sizes), "dilation_rates and segment_sizes should have the same length"
 
+                # Add softmax denominators to the corresponding positions in the softmax_denominators tensor
+                softmax_denominators[:, offset::dilation_rate, :attn_output.shape[1]*dilation_rate] += attn_weights.sum(dim=-1)
 
-        self.d_model = d_model
-        self.num_heads = num_heads
-        self.dilation_rates = dilation_rates
-        self.segment_sizes = segment_sizes
-        
-        self.dilated_attention_layers = nn.ModuleList(
-            [DilatedAttention(d_model, num_heads, dilation_rate, segment_size)]
-            for dilation_rate, segment_size in zip(dilation_rates, segment_sizes)
-        )
-
-    def forward(self, x):
-        #accumlate outputs from different layers
-        outputs = []
-
-        #process each dilated attention layer
-        for i in range(len(self.dilated_attention_layers)):
-            output = self.dilated_attention_layers[i](x)
-            outputs.append(output)
+        # Calculate the weights for the different dilated attentions
+        weights = self.softmax(softmax_denominators)
 
-        #combine the outputs
-        output = torch.sum(torch.stack(outputs), dim=0)
+        # Apply the weights to the outputs
+        outputs_weighted = weights * outputs
 
-        return output
-    
+        return outputs_weighted
```

### Comparing `LongNet-0.4.1/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.4.2/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.4.2/LongNet/iterations/DilatedAttentionOP.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
 from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.4.2/LongNet/iterations/DilatedAttentionOld.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
 from LongNet.attend import FlashAttention
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DilatedAttentionV2.py` & `LongNet-0.4.2/LongNet/iterations/DilatedAttentionV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 from torch.nn.parallel import DataParallel
 
 from LongNet.utils import XPOS, RelativePositionBias
 
 from LongNet.attend import FlashAttention
 
 device = "cuda:0"
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DilatedAttentionv5.py` & `LongNet-0.4.2/LongNet/iterations/DilatedAttentionv5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 import math
 
 #distributed dilated attention based on second iteration
-import torch.distributed as dist
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
-from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attend import FlashMHA
 import time
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.4.2/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #distributed dilated attention based on second iteration
 import torch.distributed as dist
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
 from LongNet.attend import FlashMHA
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.4.2/LongNet/iterations/topk.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,156 @@
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attend import FlashAttention
+from LongNet.attend import FlashMHA
+
 
 # Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
+class TopKAttention(nn.Module):
+    def __init__(self, k):
+        super(TopKAttention, self).__init__()
+        self.k = k 
+
+    def forward(self, Q, K, V):
+        attention_scores = torch.matmul(Q, K.transpose(-2, -1)) # calculate attention scores
+        top_k_scores, top_k_indices = torch.topk(attention_scores, self.k, dim=-1) # select topk scores and their indices
+        top_k_scores = torch.nn.functional.softmax(top_k_scores, dim=-1) # apply softmax to get attention weights
+        top_k_values = torch.gather(V, -2, top_k_indices) # gather corresponding values
+        torch.matmul(top_k_scores, top_k_values) # calculate attention output
+
+
+# Define the attention module
+class DilatedAttention(nn.Module):
+    def __init__(self, d_model, num_heads, dilation_rate, top_k, segment_size, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
+        super(DilatedAttention, self).__init__()
+        
+        # Initialize parameters
+        self.d_model = d_model               # model dimension
+        self.num_heads = num_heads           # number of attention heads
+        self.dilation_rate = dilation_rate   # dilation rate
+        self.segment_size = segment_size     # segment size
+        self.top_k_attention = TopKAttention(top_k)
 
+        # Initialize attention for each head with dilation
+        self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
 
-class DynamicDilatedAttention(nn.Module):
-    def __init__(self, d_model, num_heads, num_rates, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
-        super(DynamicDilatedAttention, self).__init__()
-        self.d_model = d_model
-        self.num_heads = num_heads
-        self.casual = casual  # Define this before FlashAttention
-
-        # Generate geometric sequences for dilation rates and segment sizes
-        self.dilation_rates = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
-        self.segment_sizes = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
-
-        self.attention = [FlashAttention(causal=self.casual, dropout=dropout).to(device) for _ in range(num_rates)] # Corrected here]
+        # Initialize dropout layer
         self.dropout = nn.Dropout(dropout)
+        
+        # If casual attention is used
+        self.casual = casual
 
+        # If using positional encoding
         self.use_xpos = use_xpos
+
+        # If using relative positional bias
         self.use_rel_pos_bias = use_rel_pos_bias
 
+        # If using positional encoding, initialize it
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
+
+        # If using relative positional bias, initialize it
         if use_rel_pos_bias:
             self.relative_bias = RelativePositionBias(num_buckets=32, max_distance=128, n_heads=num_heads)
 
+        # Initialize softmax for later use in weights
         self.softmax = nn.Softmax(dim=-1)
 
+    # Function to get mask for casual attention
     def get_mask(self, i, j):
         return torch.ones((i, j), device=device, dtype=torch.bool).triu(j - i + 2)
-    
+
+    # Forward function
     def forward(self, x):
         # Get batch size, sequence length and model dimension
         batch_size, seq_len, _ = x.shape
-        print(f'x.shape: {x.shape}')  # Print the shape of the input tensor
 
+        # If using positional encoding, add it
         if self.use_xpos:
             x = self.xpos(x)
 
-        # Initialize tensor to store outputs
-        outputs = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
-        print(f'outputs.shape: {outputs.shape}')  # Print the shape of the outputs tensor
+        # Initialize list to store outputs from each attention head
+        all_head_outputs = []
+        
+        # For each attention head
+        for head_idx, attention in enumerate(self.attentions):
+            # Calculate offset for this head
+            offset = head_idx % self.dilation_rate
+
+            # Apply offset and segment for this head
+            x_ = x[:, offset::self.dilation_rate, :]
+            x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
+
+            # Pass through attention
+            attn_output, _ = attention(x_, x_, x_)
+            
+            # If using relative positional bias, add it
+            if self.use_rel_pos_bias:
+                attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
+
+            # If using casual attention, apply mask
+            if self.casual:
+                mask = self.get_mask(attn_output.size(1), attn_output.size(1))
+                attn_output = attn_output.masked_fill(mask, float('-inf'))
+
+            # Apply dropout
+            attn_output = self.dropout(attn_output)
+
+            # Resize back to original size
+            attn_output_resized = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
+            attn_output_resized[:, offset::self.dilation_rate, :] = attn_output.contiguous().view(batch_size, -1, self.d_model)
+            
+            # Append output to list of all outputs
+            all_head_outputs.append(attn_output_resized)
 
-        # Initialize tensor to store softmax denominators
-        softmax_denominators = torch.zeros((batch_size, seq_len, self.num_heads), device=device, dtype=dtype)
+        # Calculate the weights for the different dilated attentions
+        weights = self.softmax(torch.tensor([1.0 / self.dilation_rate for _ in range(self.dilation_rate)], device=device, dtype=dtype))
 
-        for head_idx, attention in enumerate(self.attention):
-            dilation_rate = self.dilation_rates[head_idx]
-            segment_size = self.segment_sizes[head_idx]
+        # Apply the weights to the outputs of the different heads
+        outputs_weighted = sum(w * out for w, out in zip(weights, all_head_outputs))
 
-            for offset in range(dilation_rate):
-                x_ = x[:, offset::dilation_rate, :]  # Apply offset for each head
-                x_ = x_.contiguous().view(batch_size, -1, segment_size, self.d_model)
-                print(f'x_.shape: {x_.shape}')  # Print the shape of the reshaped input tensor
+        # Return the weighted outputs
+        return outputs_weighted
 
-                attn_output, attn_weights, *_ = attention(x_, x_, x_)  # Collect all additional return values into a list
-                print(f'attn_output.shape: {attn_output.shape}')  # Print the shape of the attention output tensor
 
-                if self.use_rel_pos_bias:
-                    attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
-                if self.casual:
-                    mask = self.get_mask(attn_output.size(1), attn_output.size(1))
-                    attn_output = attn_output.masked_fill(mask, float('-inf'))
 
-                attn_output = self.dropout(attn_output)
 
-                # Prepare output for addition
-                attn_output_reshaped = attn_output.contiguous().view(batch_size, -1, self.d_model)
-                print(f'attn_output_reshaped.shape: {attn_output_reshaped.shape}')  # Print the shape of the reshaped attention output tensor
 
-                # Prepare the slice of outputs for addition
-                outputs_slice = outputs[:, offset::dilation_rate, :attn_output.shape[1]*dilation_rate]
-                print(f'outputs_slice.shape: {outputs_slice.shape}')  # Print the shape of the slice of outputs
 
-                # Add output to the corresponding positions in the outputs tensor
-                outputs_slice += attn_output_reshaped
-                print(f'outputs.shape after addition: {outputs.shape}')  # Print the shape of the outputs tensor after addition
 
+class LongNetTransformer(nn.Module):
+    def __init__(self, d_model, num_heads, dilation_rates, segment_sizes):
+        super(LongNetTransformer, self).__init__()
+        assert len(dilation_rates) == len(segment_sizes), "dilation_rates and segment_sizes should have the same length"
 
-                # Add softmax denominators to the corresponding positions in the softmax_denominators tensor
-                softmax_denominators[:, offset::dilation_rate, :attn_output.shape[1]*dilation_rate] += attn_weights.sum(dim=-1)
 
-        # Calculate the weights for the different dilated attentions
-        weights = self.softmax(softmax_denominators)
+        self.d_model = d_model
+        self.num_heads = num_heads
+        self.dilation_rates = dilation_rates
+        self.segment_sizes = segment_sizes
+        
+        self.dilated_attention_layers = nn.ModuleList(
+            [DilatedAttention(d_model, num_heads, dilation_rate, segment_size)]
+            for dilation_rate, segment_size in zip(dilation_rates, segment_sizes)
+        )
+
+    def forward(self, x):
+        #accumlate outputs from different layers
+        outputs = []
+
+        #process each dilated attention layer
+        for i in range(len(self.dilated_attention_layers)):
+            output = self.dilated_attention_layers[i](x)
+            outputs.append(output)
 
-        # Apply the weights to the outputs
-        outputs_weighted = weights * outputs
+        #combine the outputs
+        output = torch.sum(torch.stack(outputs), dim=0)
 
-        return outputs_weighted
+        return output
+
```

### Comparing `LongNet-0.4.1/LongNet/iterations/MultiModal.py` & `LongNet-0.4.2/LongNet/iterations/MultiModal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import torch 
 import torch.nn as nn
-import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
 from LongNet.attend import FlashMHA
 
 device = "cuda:0"
 dtype=torch.float16
```

### Comparing `LongNet-0.4.1/LongNet/training.py` & `LongNet-0.4.2/LongNet/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,82 +1,76 @@
 import math
 import multiprocessing
 import os
 from datetime import timedelta
+
 from functools import partial
 from itertools import chain
 
 import torch
 from torch.distributed.fsdp import (
     FullyShardedDataParallel,
     MixedPrecision,
     BackwardPrefetch,
     ShardingStrategy,
 )
 from accelerate import Accelerator
+
 from accelerate.utils import (DummyOptim, DummyScheduler,
                               InitProcessGroupKwargs)
-from datasets import concatenate_datasets, load_dataset
+from datasets import load_dataset
 from lion_pytorch import Lion
-from torch.nn import LayerNorm
 
 from torch.nn import LayerNorm
-
 from torch.distributed.algorithms._checkpoint.checkpoint_wrapper import (
     CheckpointImpl, apply_activation_checkpointing, checkpoint_wrapper)
-
 from torch.distributed.fsdp.wrap import (
-    transformer_auto_wrap_policy,
+    transformer_auto_wrap_policy
 )
 
 
 from torch.optim import AdamW
 from torch.utils.data import DataLoader
 from tqdm import tqdm
+
 from transformers import (AutoTokenizer, default_data_collator,
                           get_cosine_schedule_with_warmup,
                           get_linear_schedule_with_warmup, set_seed)
+from LongNet.utils import StableAdamWUnfused
+from LongNet.model import Decoder, LongNet
 
 
+import bitsandbytes as bnb
 
-# INTEGRATE LONGNET selector + stable8bitfusedadam
-
-# from LongNet.torchscale.torchscale.architecture.decoder import Decoder
-from torchscale import Decoder
-from utils import StableAdamWUnfused
-from model import LongNet
-############ SETUP CONFIG
-# import torch.distributed as dist
 
-# dist.init_process_group(backend='nccl', init_method="env://")
 
-################
 
 class CFG:
-    BATCH_SIZE: int = 3
+    BATCH_SIZE = 3
     GRADIENT_ACCUMULATE_EVERY: int = 1
     SEED: int = 42
     LEARNING_RATE: float = 3e-4
     WEIGHT_DECAY: float = 0.1
     SEQ_LEN: int = 8192
     NUM_CPU: int = multiprocessing.cpu_count()
     USE_DEEPSPEED: bool = True
-    USE_FSDP: bool = False
-    USE_PRETOKENIZED: bool = False
-    USE_ACTIVATION_CHECKPOINTING: bool = False
-    RESUME_FROM_CHECKPOINT: str = None
+    USE_FSDP: bool = True
+    USE_PRETOKENIZED: bool = True
+    USE_ACTIVATION_CHECKPOINTING: bool = True
+    RESUME_FROM_CHECKPOINT: str = False
     CHECKPOINTING_STEPS: int = 1000
-    OUTPUT_DIR: str = "YOUR_OUTPUT_DIR"
-    ENTITY_NAME: str = "YOUR_ENTITY_NAME" #wandb
+    OUTPUT_DIR: str = 'checkpoints/' # Folder
+    ENTITY_NAME: str = "LongNet"
 
 
 # helpers
 
 
 def print_num_params(model, accelerator: Accelerator):
+    # n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     n_params = sum(p.numel() for p in model.parameters() if p.requires_grad)
     accelerator.print(f"Number of parameters in model: {n_params}")
 
 
 # activation checkpointing
 
 
@@ -90,17 +84,17 @@
 
     Args:
         model (Module): The model to which to apply activation checkpointing.
         offload_to_cpu (bool, optional): Whether to offload the activations to CPU. Defaults to False.
         accelerator (Accelerator, optional): The Accelerate library accelerator. Defaults to None.
     """
     if accelerator is not None:
-        accelerator.print(f"Using activation checkpointing")
-    #maybe error here in decoder, use parallel transformer block
-    check_fn = lambda submodule: isinstance(submodule, Decoder)
+        accelerator.print("Using activation checkpointing")
+    def check_fn(submodule):
+        return isinstance(submodule, Decoder)
     non_reentrant_wrapper = partial(
         checkpoint_wrapper,
         offload_to_cpu=offload_to_cpu,
         checkpoint_impl=CheckpointImpl.NO_REENTRANT,
     )
     apply_activation_checkpointing(
         model, checkpoint_wrapper_fn=non_reentrant_wrapper, check_fn=check_fn
@@ -374,14 +368,18 @@
         optimizer = AdamW(grouped_params, lr=learning_rate, betas=(beta_1, beta_2),)
     elif optimizer_type == "deepspeed":
         optimizer = DummyOptim(grouped_params, lr=learning_rate, betas=(beta_1, beta_2),)
     elif optimizer_type == "stable_adamw":
         optimizer = StableAdamWUnfused(
             grouped_params, lr=learning_rate, betas=(beta_1, beta_2),
         )
+    elif optimizer_type=="Adam8bit":
+        optimizer = bnb.optim.Adam8bit(grouped_params, lr=learning_rate, betas=(beta_1, beta_2))
+    elif optimizer_type=="Lion8Bit":
+        optimizer = bnb.optim.Lion8bit(grouped_params, lr=learning_rate, betas=(beta_1, beta_2))
     else:
         raise ValueError(
             "Invalid optimizer_type. Expected 'lion', 'adamw', 'deepspeed' or 'stable_adamw', got: {}".format(
                 optimizer_type
             )
         )
 
@@ -437,21 +435,21 @@
         group_texts, batched=True, num_proc=CFG.NUM_CPU,
     )
 
     return train_dataset
 
 #switch to falconwebdataset
 def build_pre_tokenized():
-    d0 = load_dataset("conceptofmind/c4_0-to-20_neox_with_eos_8k", split="train")
-    d1 = load_dataset("conceptofmind/c4_21-to-40_neox_with_eos_8k", split="train")
-    d2 = load_dataset("conceptofmind/c4_41-to-60_neox_with_eos_8k", split="train")
-    d3 = load_dataset("conceptofmind/c4_61-to-80_neox_with_eos_8k", split="train")
-    d4 = load_dataset("conceptofmind/c4_81-to-100_neox_with_eos_8k", split="train")
-    train_dataset = concatenate_datasets([d0, d1, d2, d3, d4])
-    return train_dataset
+    d0 = load_dataset("conceptofmind/c4_0-to-20_neox_with_eos_8k", split="train[:10]")
+    # d1 = load_dataset("conceptofmind/c4_21-to-40_neox_with_eos_8k", split="train")
+    # d2 = load_dataset("conceptofmind/c4_41-to-60_neox_with_eos_8k", split="train")
+    # d3 = load_dataset("conceptofmind/c4_61-to-80_neox_with_eos_8k", split="train")
+    # d4 = load_dataset("conceptofmind/c4_81-to-100_neox_with_eos_8k", split="train")
+    # train_dataset = concatenate_datasets([d0, d1, d2, d3, d4])
+    return d0
 
 
 
 def Train():
     # accelerator
 
     timeout = InitProcessGroupKwargs(timeout=timedelta(seconds=1_000_000))
@@ -478,18 +476,15 @@
 
     accelerator.print(f"Total GPUS: {accelerator.num_processes}")
 
     # set seed
 
     set_seed(CFG.SEED)
 
-
-    # model = LongNet.to(accelerator.device)
-    # model = AutoModelForCausalLM.from_pretrained("YOUR MODEL", load_in_4bit=True, device_map="auto").to(accelerator.device)
-    LongNet().to(accelerator.device)
+    model = LongNet().to(accelerator.device)
 
     print_num_params(model, accelerator)
 
     if CFG.USE_FSDP:
         model = fsdp(
             model,
             mp="fp16",
@@ -516,15 +511,15 @@
 
     optim = decoupled_optimizer(
         model=model,
         learning_rate=CFG.LEARNING_RATE, 
         weight_decay=CFG.WEIGHT_DECAY, 
         beta_1=0.90, 
         beta_2=0.95, 
-        optimizer_type='deepspeed',  
+        optimizer_type='Adam8bit',  
         use_fsdp=True,
         accelerator=accelerator
     )
 
     # Determine number of training steps
 
     max_train_steps = math.ceil(len(train_loader) / CFG.GRADIENT_ACCUMULATE_EVERY)
@@ -642,9 +637,24 @@
         unwrapped_model = accelerator.unwrap_model(model)
         with accelerator.main_process_first():
             accelerator.save(
                 unwrapped_model.state_dict(), f"{CFG.OUTPUT_DIR}/final/final_model.pt"
             )
 
 
-if __name__ == "__main__":
+def main():
+    os.environ['MASTER_ADDR'] # = 'localhost'
+    os.environ['MASTER_PORT'] #= '9994'
+    
+    # # [CRITICAL] Pay attention to this when scaling to multiple GPUs and clusters
+    
+    # # Pay attention to this, use "accelerate config"
+
+    os.environ['RANK']       #= str(0) # Number of nodes (servers)
+    os.environ['WORLD_SIZE'] #= str(torch.cuda.device_count())
+
+    torch.distributed.init_process_group()
+    
+    Train()
+
+if __name__ == '__main__':
     main()
```

### Comparing `LongNet-0.4.1/LongNet/utils.py` & `LongNet-0.4.2/LongNet/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import numpy as np
 import torch
 
 # This is the unfused version of StableAdamW. It is slower than the fused version (coming).
 
 
 class StableAdamWUnfused(torch.optim.Optimizer):
     def __init__(
@@ -33,17 +32,16 @@
 
         print("Using StableAdamWUnfused-v1")
 
     def __setstate__(self, state):
         super(StableAdamWUnfused, self).__setstate__(state)
 
     def step(self, closure=None):
-        loss = None
         if closure is not None:
-            loss = closure()
+            closure()
 
         for group in self.param_groups:
             lr = group["lr"]
             weight_decay = group["weight_decay"]
             beta1 = group["beta1"]
             beta2 = group["beta2"]
             step = group["step"]
@@ -175,15 +173,14 @@
             self.compute_bias(qlen, klen, step)
             .repeat(batch_size, 1, 1, 1)
             .view(-1, qlen, klen)
         )
 
 
 
-import numpy as np
 import torch
 import torch.nn as nn
 
 def fixed_pos_embedding(x):
     seq_len, dim = x.shape
     inv_freq = 1.0 / (10000 ** (torch.arange(0, dim) / dim))
     sinusoid_inp = (
@@ -237,7 +234,77 @@
             cos = cos[-length:]
         
         if downscale:
             scale = 1 / scale
 
         x = apply_rotary_pos_emb(x, sin, cos, scale)
         return x
+
+
+import math
+from typing import List, Tuple, Union, Optional
+
+import torch
+
+def SparsifyIndices(
+    x: torch.Tensor, ws: List[int], rs: List[int], head_idx: int
+) -> Tuple[int, torch.Tensor, Optional[torch.Tensor]]:
+    b, n, c = x.size()
+
+    x_indices = torch.arange(0, n, dtype=torch.long, device=x.device)[None, :, None]
+
+    num_subatt = sum([int(math.ceil(n / w)) for w in ws])
+    max_subatt_n = min(n, max([w // r for w, r in zip(ws, rs)]))
+
+    sparse_indices = -1*torch.ones((b, num_subatt * max_subatt_n, c), device=x.device, dtype=torch.int64)
+
+    subatt_idx = 0
+    for w, r in zip(ws, rs):
+        for segment_indices in torch.split(x_indices, w, 1):
+            offset = head_idx % r
+            cur_sparse_indices = segment_indices[:, offset::r, :]
+            start_idx = subatt_idx*max_subatt_n
+            end_idx = start_idx+cur_sparse_indices.shape[1]
+            sparse_indices[:, start_idx:end_idx] = cur_sparse_indices
+            subatt_idx += 1
+
+    if -1 in sparse_indices:
+        padding_mask = sparse_indices[:, :, 0] != -1
+
+        # to allow gather work for batching
+        sparse_indices[~padding_mask] = 0
+
+        # combine batch and subattention dims
+        padding_mask = padding_mask.view((-1, max_subatt_n))
+    else:
+        padding_mask = None
+
+    return max_subatt_n, sparse_indices, padding_mask
+
+
+def MixOutputs(
+    out_shape: Tuple[int, int, int],
+    out_dtype: torch.dtype,
+    out_device: Union[torch.device, str],
+    a_os: torch.Tensor,
+    a_denoms: torch.Tensor,
+    a_indices: torch.Tensor,
+) -> torch.Tensor:
+    # calculate sums of softmax denominators
+    att_denom_sums = torch.zeros((out_shape[0], out_shape[1]), device=out_device)
+    att_denom_sums.scatter_add_(1, a_indices[:, :, 0], a_denoms)
+
+    # select attention softmax denominator sums for current sparse indices
+    sparse_att_denom_sum = torch.gather(att_denom_sums, 1, a_indices[:, :, 0])
+
+    # compute alphas
+    alphas = torch.divide(a_denoms, sparse_att_denom_sum)[:, :, None]
+
+    out = torch.zeros(out_shape, dtype=out_dtype, device=out_device)
+
+    out.scatter_add_(
+        1,
+        a_indices[:, :, :out.shape[2]],
+        torch.multiply(a_os, alphas),
+    )
+
+    return out
```

### Comparing `LongNet-0.4.1/LongNet.egg-info/PKG-INFO` & `LongNet-0.4.2/LongNet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.4.1
+Version: 0.4.2
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.4.1/PKG-INFO` & `LongNet-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.4.1
+Version: 0.4.2
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.4.1/README.md` & `LongNet-0.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,16 @@
-# Agora
-This implementation of LongNet is brought to you by Agora, we're an all-new open source AI research organization with 1,500+ AI researchers all striving to advance Humanity!
-
-![Agora banner](agora-banner-water.png)
-
-[Join us and help contribute to LongNet and or recieve FAST support in the Agora discord!](https://discord.gg/qUtxnK2NMf)
-
 # LongNet: Scaling Transformers to 1,000,000,000 Tokens
+![LongNetBanner](longnet.jpg)
 
 This is an open source implementation for the paper [LongNet: Scaling Transformers to 1,000,000,000 Tokens](https://arxiv.org/abs/2307.02486) by Jiayu Ding, Shuming Ma, Li Dong, Xingxing Zhang, Shaohan Huang, Wenhui Wang, Furu Wei. The LongNet is a Transformer variant designed to scale sequence length up to more than 1 billion tokens without sacrificing performance on shorter sequences.
 
-## Introduction
-
-Scaling sequence length has become a critical bottleneck in the era of large language models. However, existing methods struggle with either computational complexity or model expressivity, rendering the maximum sequence length restricted. In this paper, they introduce LongNet, a Transformer variant that can scale sequence length to more than 1 billion tokens, without sacrificing the performance on shorter sequences. Specifically, they propose dilated attention, which expands the attentive field exponentially as the distance grows.
 
-## Features
-LongNet has significant advantages:
-1. It has a linear computation complexity and a logarithm dependency between tokens.
-2. It can be served as a distributed trainer for extremely long sequences.
-3. Its dilated attention is a drop-in replacement for standard attention, which can be seamlessly integrated with the existing Transformer-based optimization.
-
-Experiment results demonstrate that LongNet yields strong performance on both long-sequence modeling and general language tasks. Their work opens up new possibilities for modeling very long sequences, e.g., treating a whole corpus or even the entire Internet as a sequence.
-
-Here's the updated usage and installation section with two methods: git clone or pip install LongNet:
+### News 📰
+* **This implementation of LongNet is brought to you by Agora, we're an all-new open source AI research organization with 1,500+ AI researchers all striving to advance Humanity!** **[Join us and help contribute to LongNet and or recieve FAST support in the Agora discord!](https://discord.gg/qUtxnK2NMf)**
+* **[Execute tasks and help accelerate AI research with the project board](https://github.com/users/kyegomez/projects/3/views/2)**
 
 ## Installation
 
 You can install LongNet using one of the following methods:
 
 ### Method 1: Git Clone
 
@@ -95,14 +80,28 @@
 # Forward pass
 outputs = attention(inputs)
 
 # Print the output shape
 print(outputs.shape)  # Expected: [batch_size, seq_len, d_model]
 ```
 
+## Introduction
+
+Scaling sequence length has become a critical bottleneck in the era of large language models. However, existing methods struggle with either computational complexity or model expressivity, rendering the maximum sequence length restricted. In this paper, they introduce LongNet, a Transformer variant that can scale sequence length to more than 1 billion tokens, without sacrificing the performance on shorter sequences. Specifically, they propose dilated attention, which expands the attentive field exponentially as the distance grows.
+
+## Features
+LongNet has significant advantages:
+1. It has a linear computation complexity and a logarithm dependency between tokens.
+2. It can be served as a distributed trainer for extremely long sequences.
+3. Its dilated attention is a drop-in replacement for standard attention, which can be seamlessly integrated with the existing Transformer-based optimization.
+
+Experiment results demonstrate that LongNet yields strong performance on both long-sequence modeling and general language tasks. Their work opens up new possibilities for modeling very long sequences, e.g., treating a whole corpus or even the entire Internet as a sequence.
+
+Here's the updated usage and installation section with two methods: git clone or pip install LongNet:
+
 # Documentation
 
 * [Click here for the model documentation](docs/DOCUMENTATION.md)
 
 # Training the Model
 * We're still working on the model configuation as closely in the paper as possible. There are 2 methods, one is `accelerate` and the other `from LongNet import Train`
 
@@ -289,25 +288,24 @@
 [Share LongNet Repository](https://github.com/kyegomez/LongNet)
 
 
 
 
 # Roadmap
 
-* Test and evaluate and patch.
+* Recreate the sparsification mechanism
 
-* And, create an interation of `DilatedAttention` with `FlashBlocksparseMHA`
+* Recreate the gathering mechanism
 
-* Create a multi-modal `DilationAttention` with multiway, sub layernorm, and xpos, sub layernorm, QK Layernorm, One write query head maybe
+* Implement FlashAttention2.0
 
-* Integrate Alibi and xpos for even further ridicoulus length extrapolation
+* Implement Distributed Setup
 
-* Recreate in Triton or Jax for ultra mega speed boost
+*  create the all-gather operation in the backward that becomes a reduce-scatter operation
 
-* Integrate [Dynamic sparse flash attention](https://github.com/epfml/dynamic-sparse-flash-attention/blob/main/runtime-experiments/timeperf-hash-and-qk-sparse.ipynb) with DilatedAttention
 
 
 ## Citation
 ```
 @inproceedings{ding2023longnet,
   title={LongNet: Scaling Transformers to 1,000,000,000 Tokens},
   author={Ding, Jiayu and Ma, Shuming and Dong, Li and Zhang, Xingxing and Huang, Shaohan and Wang, Wenhui and Wei, Furu},
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `LongNet-0.4.1/setup.py` & `LongNet-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.4.1',
+  version = '0.4.2',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

