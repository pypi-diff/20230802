# Comparing `tmp/sequential_calibrationWithSA-0.0.7-py3-none-any.whl.zip` & `tmp/sequential_calibrationWithSA-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 2809 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       19 b- defN 23-Jan-23 23:40 sequential_calibrationWithSA/__init__.py
+Zip file size: 2888 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       19 b- defN 23-Aug-02 20:17 sequential_calibrationWithSA/__init__.py
 -rw-rw-rw-  2.0 fat       40 b- defN 22-Dec-29 00:17 sequential_calibrationWithSA/ex.py
--rw-rw-rw-  2.0 fat      374 b- defN 23-Feb-09 00:23 sequential_calibrationWithSA/seqC.py
+-rw-rw-rw-  2.0 fat      375 b- defN 23-Aug-02 20:17 sequential_calibrationWithSA/seqC.py
 -rw-rw-rw-  2.0 fat       72 b- defN 22-Dec-30 18:54 sequntial_calibrationWithSA/VSA.py
 -rw-rw-rw-  2.0 fat       17 b- defN 22-Dec-30 18:52 sequntial_calibrationWithSA/__init__.py
 -rw-rw-rw-  2.0 fat       40 b- defN 22-Dec-29 00:17 sequntial_calibrationWithSA/ex.py
--rw-rw-rw-  2.0 fat      325 b- defN 23-Feb-09 00:26 sequential_calibrationWithSA-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Feb-09 00:26 sequential_calibrationWithSA-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       29 b- defN 23-Feb-09 00:26 sequential_calibrationWithSA-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      928 b- defN 23-Feb-09 00:26 sequential_calibrationWithSA-0.0.7.dist-info/RECORD
-10 files, 1941 bytes uncompressed, 1171 bytes compressed:  39.7%
+-rw-rw-rw-  2.0 fat      325 b- defN 23-Aug-02 20:30 sequential_calibrationWithSA-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Aug-02 20:30 sequential_calibrationWithSA-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Aug-02 20:30 sequential_calibrationWithSA-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      928 b- defN 23-Aug-02 20:30 sequential_calibrationWithSA-0.0.9.dist-info/RECORD
+10 files, 1942 bytes uncompressed, 1250 bytes compressed:  35.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: sequntial_calibrationWithSA/__init__.py
 Comment: 
 
 Filename: sequntial_calibrationWithSA/ex.py
 Comment: 
 
-Filename: sequential_calibrationWithSA-0.0.7.dist-info/METADATA
+Filename: sequential_calibrationWithSA-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: sequential_calibrationWithSA-0.0.7.dist-info/WHEEL
+Filename: sequential_calibrationWithSA-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: sequential_calibrationWithSA-0.0.7.dist-info/top_level.txt
+Filename: sequential_calibrationWithSA-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: sequential_calibrationWithSA-0.0.7.dist-info/RECORD
+Filename: sequential_calibrationWithSA-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sequential_calibrationWithSA/seqC.py

```diff
@@ -10,60 +10,34 @@
 function
 1) VSA
 2) Calibration
 3) 
 '''
 
 
-# In[1]:
+# ## 1) Calibration
+
+# In[ ]:
 
 
-import numpy as np
 
 
-# ## 1) VSA-Variance based SA
 
 # In[4]:
 
 
 def VSA(msg):
-    print(msg + "asd")
+    print(msg + "asdef")
     print(np.zeros(3))
 
 
-# In[ ]:
-
-
-
-
-
-# In[ ]:
-
-
-
-
-
-# In[ ]:
-
-
-
-
-
-# ## 2) Calibration
-
-# In[6]:
-
-
-
-
-
-# In[ ]:
-
-
-
-
+# ### 방법
+# 
+# - 시뮬레이션을 돌린다.
+# - GSA하는 법 소개 -> 다른 package 소개
+# - SEQ돌리기
 
 # In[ ]:
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `sequential_calibrationWithSA-0.0.7.dist-info/RECORD` & `sequential_calibrationWithSA-0.0.9.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 sequential_calibrationWithSA/__init__.py,sha256=wx4nDyM7Oh9u2h7SwFSZYSASVxY2DzrKbSiObCjLiv8,19
 sequential_calibrationWithSA/ex.py,sha256=DdNqXI34M38GG2gjIC61t9CzJtnDmpmd1u0TcsFG1Vo,40
-sequential_calibrationWithSA/seqC.py,sha256=LvZyYRPkQuLQAADDXo3sU2_2R57KEZiqNFcvwG6h2oA,374
+sequential_calibrationWithSA/seqC.py,sha256=1PpK2Lob-9E7ylq0ISy7k3m1J-cxhvMKyWGUZ_qyJcE,375
 sequntial_calibrationWithSA/VSA.py,sha256=gBfStee2Dwh_n2JJv-Atem4jC02tfLuOMEgAH1yckKo,72
 sequntial_calibrationWithSA/__init__.py,sha256=RmCFu4XhOZAe9nhbTVvNrGedWE5A25wIcwSxFN_zU-w,17
 sequntial_calibrationWithSA/ex.py,sha256=DdNqXI34M38GG2gjIC61t9CzJtnDmpmd1u0TcsFG1Vo,40
-sequential_calibrationWithSA-0.0.7.dist-info/METADATA,sha256=w_2uHnZsGuSy_dwLEPlXUht1pZ5_bg0MM_P3wNNjkdA,325
-sequential_calibrationWithSA-0.0.7.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-sequential_calibrationWithSA-0.0.7.dist-info/top_level.txt,sha256=0n4JGJ9fE4UhRbHL5Cjid7m1jMb2TUIoNTQPJJeWwdI,29
-sequential_calibrationWithSA-0.0.7.dist-info/RECORD,,
+sequential_calibrationWithSA-0.0.9.dist-info/METADATA,sha256=pFuuHueX7fODiTNJGMb4fo3KRZc5g0zyvDWEqV_ttng,325
+sequential_calibrationWithSA-0.0.9.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+sequential_calibrationWithSA-0.0.9.dist-info/top_level.txt,sha256=0n4JGJ9fE4UhRbHL5Cjid7m1jMb2TUIoNTQPJJeWwdI,29
+sequential_calibrationWithSA-0.0.9.dist-info/RECORD,,
```

