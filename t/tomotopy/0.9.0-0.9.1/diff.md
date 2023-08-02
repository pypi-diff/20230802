# Comparing `tmp/tomotopy-0.9.0.tar.gz` & `tmp/tomotopy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tomotopy-0.9.0.tar", last modified: Tue Aug  4 15:26:33 2020, max compression
+gzip compressed data, was "dist/tomotopy-0.9.1.tar", last modified: Sat Aug  8 09:33:02 2020, max compression
```

## Comparing `tomotopy-0.9.0.tar` & `tomotopy-0.9.1.tar`

### file list

```diff
@@ -1,478 +1,478 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/
--rw-r--r--   0 root         (0) root         (0)       38 2020-08-04 15:26:33.000000 tomotopy-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/TopicModel/
--rw-r--r--   0 root         (0) root         (0)      455 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PLDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)    19396 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HPAModel.hpp
--rw-r--r--   0 root         (0) root         (0)      563 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/SLDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)      398 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HDPModel.cpp
--rw-r--r--   0 root         (0) root         (0)      417 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HLDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)      427 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PLDA.h
--rw-r--r--   0 root         (0) root         (0)     1454 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/GDMR.h
--rw-r--r--   0 root         (0) root         (0)    19326 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HDPModel.hpp
--rw-r--r--   0 root         (0) root         (0)     1341 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HLDA.h
--rw-r--r--   0 root         (0) root         (0)    21110 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HLDAModel.hpp
--rw-r--r--   0 root         (0) root         (0)     1598 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PA.h
--rw-r--r--   0 root         (0) root         (0)     2202 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DMR.h
--rw-r--r--   0 root         (0) root         (0)     7269 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LLDAModel.hpp
--rw-r--r--   0 root         (0) root         (0)    10006 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/CTModel.hpp
--rw-r--r--   0 root         (0) root         (0)     4328 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LDA.h
--rw-r--r--   0 root         (0) root         (0)    16267 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PAModel.hpp
--rw-r--r--   0 root         (0) root         (0)     2070 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/SLDA.h
--rw-r--r--   0 root         (0) root         (0)      642 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DTM.h
--rw-r--r--   0 root         (0) root         (0)      381 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/CTModel.cpp
--rw-r--r--   0 root         (0) root         (0)      383 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PAModel.cpp
--rw-r--r--   0 root         (0) root         (0)     1260 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/CT.h
--rw-r--r--   0 root         (0) root         (0)    18634 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/MGLDAModel.hpp
--rw-r--r--   0 root         (0) root         (0)      436 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DMRModel.cpp
--rw-r--r--   0 root         (0) root         (0)     2349 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DT.h
--rw-r--r--   0 root         (0) root         (0)      555 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/MGLDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)      556 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HPAModel.cpp
--rw-r--r--   0 root         (0) root         (0)    15838 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/GDMRModel.hpp
--rw-r--r--   0 root         (0) root         (0)     2095 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HDP.h
--rw-r--r--   0 root         (0) root         (0)    13807 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LDACVB0Model.hpp
--rw-r--r--   0 root         (0) root         (0)      525 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/GDMRModel.cpp
--rw-r--r--   0 root         (0) root         (0)    20234 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/TopicModel.hpp
--rw-r--r--   0 root         (0) root         (0)    19174 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DTModel.hpp
--rw-r--r--   0 root         (0) root         (0)      379 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LLDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)     1862 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LLDA.h
--rw-r--r--   0 root         (0) root         (0)     3042 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/MGLDA.h
--rw-r--r--   0 root         (0) root         (0)      388 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LDAModel.cpp
--rw-r--r--   0 root         (0) root         (0)      788 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/HPA.h
--rw-r--r--   0 root         (0) root         (0)    15542 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/SLDAModel.hpp
--rw-r--r--   0 root         (0) root         (0)     8112 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/PLDAModel.hpp
--rw-r--r--   0 root         (0) root         (0)      522 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DTModel.cpp
--rw-r--r--   0 root         (0) root         (0)    13176 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/DMRModel.hpp
--rw-r--r--   0 root         (0) root         (0)    34195 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/TopicModel/LDAModel.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/Utils/
--rw-r--r--   0 root         (0) root         (0)     3206 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/slp.hpp
--rw-r--r--   0 root         (0) root         (0)    11996 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/tvector.hpp
--rw-r--r--   0 root         (0) root         (0)     3499 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/AliasMethod.hpp
--rw-r--r--   0 root         (0) root         (0)     4652 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/Trie.hpp
--rw-r--r--   0 root         (0) root         (0)     5205 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/LBFGS.h
--rw-r--r--   0 root         (0) root         (0)     4350 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/sample.hpp
--rw-r--r--   0 root         (0) root         (0)     4257 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/ThreadPool.hpp
--rw-r--r--   0 root         (0) root         (0)     2762 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/TruncMultiNormal.hpp
--rw-r--r--   0 root         (0) root         (0)     5055 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/PolyaGamma.hpp
--rw-r--r--   0 root         (0) root         (0)    16752 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/PolyaGammaHybrid.hpp
--rw-r--r--   0 root         (0) root         (0)     6954 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/Utils.hpp
--rw-r--r--   0 root         (0) root         (0)     1690 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/LUT.hpp
--rw-r--r--   0 root         (0) root         (0)    23184 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/avx_mathfun.h
--rw-r--r--   0 root         (0) root         (0)     1550 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/Dictionary.h
--rw-r--r--   0 root         (0) root         (0)   197065 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/rtnorm.hpp
--rw-r--r--   0 root         (0) root         (0)     2275 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/avx_gamma.h
--rw-r--r--   0 root         (0) root         (0)      584 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/exception.h
--rw-r--r--   0 root         (0) root         (0)     8881 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/math.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/Utils/LBFGS/
--rw-r--r--   0 root         (0) root         (0)     3659 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/LBFGS/LineSearchBracketing.h
--rw-r--r--   0 root         (0) root         (0)     3326 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/LBFGS/LineSearchBacktracking.h
--rw-r--r--   0 root         (0) root         (0)     7737 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/LBFGS/Param.h
--rw-r--r--   0 root         (0) root         (0)     1359 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/text.hpp
--rw-r--r--   0 root         (0) root         (0)    22082 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/serializer.hpp
--rw-r--r--   0 root         (0) root         (0)    21675 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/sse_mathfun.h
--rw-r--r--   0 root         (0) root         (0)     1719 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/MultiNormalDistribution.hpp
--rw-r--r--   0 root         (0) root         (0)     5156 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/EigenAddonOps.hpp
--rw-r--r--   0 root         (0) root         (0)     2119 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Utils/sse_gamma.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/python/
--rw-r--r--   0 root         (0) root         (0)      221 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/label.h
--rw-r--r--   0 root         (0) root         (0)     7144 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_HDP.cpp
--rw-r--r--   0 root         (0) root         (0)    11555 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/PyUtils.h
--rw-r--r--   0 root         (0) root         (0)    16320 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_DT.cpp
--rw-r--r--   0 root         (0) root         (0)    26451 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_LDA.cpp
--rw-r--r--   0 root         (0) root         (0)     7509 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_CT.cpp
--rw-r--r--   0 root         (0) root         (0)    10707 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/module.h
--rw-r--r--   0 root         (0) root         (0)     7257 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_HPA.cpp
--rw-r--r--   0 root         (0) root         (0)    11013 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_MGLDA.cpp
--rw-r--r--   0 root         (0) root         (0)    13129 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_label.cpp
--rw-r--r--   0 root         (0) root         (0)    20283 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_main.cpp
--rw-r--r--   0 root         (0) root         (0)     6541 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/label_docs.h
--rw-r--r--   0 root         (0) root         (0)    13865 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_SLDA.cpp
--rw-r--r--   0 root         (0) root         (0)     9753 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_PLDA.cpp
--rw-r--r--   0 root         (0) root         (0)     7846 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_HLDA.cpp
--rw-r--r--   0 root         (0) root         (0)    14132 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_GDMR.cpp
--rw-r--r--   0 root         (0) root         (0)    13788 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_PA.cpp
--rw-r--r--   0 root         (0) root         (0)    10720 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_LLDA.cpp
--rw-r--r--   0 root         (0) root         (0)    11120 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/py_DMR.cpp
--rw-r--r--   0 root         (0) root         (0)   130619 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/python/docs.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/src/Labeling/
--rw-r--r--   0 root         (0) root         (0)     9159 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Labeling/FoRelevance.cpp
--rw-r--r--   0 root         (0) root         (0)      822 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Labeling/Labeler.h
--rw-r--r--   0 root         (0) root         (0)     2367 2020-08-04 15:26:16.000000 tomotopy-0.9.0/src/Labeling/FoRelevance.h
--rw-r--r--   0 root         (0) root         (0)    18047 2020-08-04 15:26:16.000000 tomotopy-0.9.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     3722 2020-08-04 15:26:16.000000 tomotopy-0.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/EigenRand/
--rw-r--r--   0 root         (0) root         (0)      406 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Macro.h
--rw-r--r--   0 root         (0) root         (0)    12126 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/doc.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/EigenRand/Dists/
--rw-r--r--   0 root         (0) root         (0)    24242 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Dists/Discrete.h
--rw-r--r--   0 root         (0) root         (0)     3371 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Dists/GammaPoisson.h
--rw-r--r--   0 root         (0) root         (0)    18387 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Dists/NormalExp.h
--rw-r--r--   0 root         (0) root         (0)     3038 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Dists/Basic.h
--rw-r--r--   0 root         (0) root         (0)      305 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/EigenRand
--rw-r--r--   0 root         (0) root         (0)    45286 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/Core.h
--rw-r--r--   0 root         (0) root         (0)    14831 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/PacketRandomEngine.h
--rw-r--r--   0 root         (0) root         (0)    24878 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/MorePacketMath.h
--rw-r--r--   0 root         (0) root         (0)     9439 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/RandUtils.h
--rw-r--r--   0 root         (0) root         (0)     6655 2020-08-04 15:26:25.000000 tomotopy-0.9.0/include/EigenRand/PacketFilter.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/
--rw-r--r--   0 root         (0) root         (0)     1371 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SparseCholesky
--rw-r--r--   0 root         (0) root         (0)      122 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Dense
--rw-r--r--   0 root         (0) root         (0)     1676 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/PaStiXSupport
--rw-r--r--   0 root         (0) root         (0)     1206 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Cholesky
--rw-r--r--   0 root         (0) root         (0)     1629 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SVD
--rw-r--r--   0 root         (0) root         (0)     2483 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/OrderingMethods
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 root         (0) root         (0)    24010 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 root         (0) root         (0)     6898 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 root         (0) root         (0)    22248 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Cholesky/
--rw-r--r--   0 root         (0) root         (0)    24480 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 root         (0) root         (0)    18395 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 root         (0) root         (0)     3974 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SVD/
--rw-r--r--   0 root         (0) root         (0)    15957 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SVD/UpperBidiagonalization.h
--rw-r--r--   0 root         (0) root         (0)    32949 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 root         (0) root         (0)    48778 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 root         (0) root         (0)    12740 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 root         (0) root         (0)     5099 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 root         (0) root         (0)    16396 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 root         (0) root         (0)    62266 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 root         (0) root         (0)     5229 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 root         (0) root         (0)    17202 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 root         (0) root         (0)    11405 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/QR/
--rw-r--r--   0 root         (0) root         (0)     2993 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
--rw-r--r--   0 root         (0) root         (0)     4662 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 root         (0) root         (0)    24881 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 root         (0) root         (0)    20805 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 root         (0) root         (0)    14022 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 root         (0) root         (0)    25478 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/QR/FullPivHouseholderQR.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 root         (0) root         (0)    22307 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 root         (0) root         (0)    34345 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 root         (0) root         (0)     3650 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 root         (0) root         (0)    23586 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 root         (0) root         (0)    33674 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 root         (0) root         (0)    12558 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 root         (0) root         (0)    17176 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 root         (0) root         (0)     9715 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 root         (0) root         (0)    20288 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 root         (0) root         (0)    17021 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 root         (0) root         (0)    14351 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 root         (0) root         (0)     5539 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 root         (0) root         (0)     4178 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 root         (0) root         (0)    22944 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 root         (0) root         (0)    22444 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/Tridiagonalization.h
--rw-r--r--   0 root         (0) root         (0)     4104 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Jacobi/
--rw-r--r--   0 root         (0) root         (0)    15902 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/
--rw-r--r--   0 root         (0) root         (0)    32152 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 root         (0) root         (0)     8423 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 root         (0) root         (0)    14815 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 root         (0) root         (0)     8063 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 root         (0) root         (0)     6191 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Umeyama.h
--rw-r--r--   0 root         (0) root         (0)     7773 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 root         (0) root         (0)     3639 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 root         (0) root         (0)     8949 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 root         (0) root         (0)     6877 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 root         (0) root         (0)    20539 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Homogeneous.h
--rwxr-xr-x   0 root         (0) root         (0)     6324 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 root         (0) root         (0)    11961 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 root         (0) root         (0)     8308 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/ParametrizedLine.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 root         (0) root         (0)     5387 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/arch/Geometry_SSE.h
--rw-r--r--   0 root         (0) root         (0)    60514 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Geometry/Transform.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/misc/
--rw-r--r--   0 root         (0) root         (0)     2913 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/Image.h
--rwxr-xr-x   0 root         (0) root         (0)  1058368 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 root         (0) root         (0)     2742 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 root         (0) root         (0)    30560 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/blas.h
--rw-r--r--   0 root         (0) root         (0)     1748 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 root         (0) root         (0)     7834 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/lapack.h
--rw-r--r--   0 root         (0) root         (0)      474 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 root         (0) root         (0)    20032 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/
--rw-r--r--   0 root         (0) root         (0)     6990 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 root         (0) root         (0)    11507 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 root         (0) root         (0)     3877 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 root         (0) root         (0)    19067 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 root         (0) root         (0)    21123 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 root         (0) root         (0)     4525 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 root         (0) root         (0)     5282 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 root         (0) root         (0)    12800 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Ref.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/
--rw-r--r--   0 root         (0) root         (0)      607 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 root         (0) root         (0)     4400 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 root         (0) root         (0)    27944 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/UnaryFunctors.h
--rw-r--r--   0 root         (0) root         (0)    18263 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 root         (0) root         (0)     8229 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 root         (0) root         (0)     6284 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 root         (0) root         (0)     8256 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 root         (0) root         (0)     7073 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 root         (0) root         (0)     7239 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Map.h
--rw-r--r--   0 root         (0) root         (0)     5595 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 root         (0) root         (0)    24212 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 root         (0) root         (0)     8074 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Visitor.h
--rw-r--r--   0 root         (0) root         (0)     9136 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 root         (0) root         (0)     3369 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 root         (0) root         (0)    21646 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 root         (0) root         (0)    23213 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 root         (0) root         (0)    45180 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 root         (0) root         (0)     4200 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 root         (0) root         (0)    29441 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 root         (0) root         (0)     4769 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 root         (0) root         (0)    21959 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 root         (0) root         (0)     6795 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 root         (0) root         (0)     3400 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 root         (0) root         (0)     4365 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/SolverBase.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/
--rw-r--r--   0 root         (0) root         (0)     6105 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 root         (0) root         (0)    81534 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 root         (0) root         (0)    13979 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 root         (0) root         (0)     4066 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 root         (0) root         (0)    13743 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 root         (0) root         (0)    20403 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 root         (0) root         (0)    19632 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 root         (0) root         (0)    26808 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 root         (0) root         (0)     6368 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 root         (0) root         (0)     6907 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 root         (0) root         (0)    14722 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 root         (0) root         (0)    11198 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 root         (0) root         (0)    15188 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 root         (0) root         (0)    18478 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 root         (0) root         (0)     5017 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 root         (0) root         (0)     6513 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 root         (0) root         (0)     5741 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverVector.h
--rw-r--r--   0 root         (0) root         (0)     5209 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 root         (0) root         (0)    10571 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 root         (0) root         (0)     4905 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 root         (0) root         (0)     9901 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 root         (0) root         (0)     2683 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 root         (0) root         (0)    27420 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 root         (0) root         (0)    17852 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 root         (0) root         (0)     9234 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 root         (0) root         (0)     7692 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 root         (0) root         (0)    14386 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 root         (0) root         (0)     1697 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 root         (0) root         (0)     9597 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 root         (0) root         (0)     2720 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Assign.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/
--rwxr-xr-x   0 root         (0) root         (0)    15722 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/BlasUtil.h
--rwxr-xr-x   0 root         (0) root         (0)     3981 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 root         (0) root         (0)    21579 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/Constants.h
--rw-r--r--   0 root         (0) root         (0)    40579 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/Memory.h
--rw-r--r--   0 root         (0) root         (0)       85 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 root         (0) root         (0)    34198 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/XprHelper.h
--rw-r--r--   0 root         (0) root         (0)      856 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 root         (0) root         (0)    36570 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/Macros.h
--rwxr-xr-x   0 root         (0) root         (0)     4026 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 root         (0) root         (0)    10518 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 root         (0) root         (0)    14150 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 root         (0) root         (0)    20586 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 root         (0) root         (0)    14777 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 root         (0) root         (0)      970 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 root         (0) root         (0)     4249 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 root         (0) root         (0)    14245 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 root         (0) root         (0)    49497 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 root         (0) root         (0)     6020 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Select.h
--rw-r--r--   0 root         (0) root         (0)     7593 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 root         (0) root         (0)    18064 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Block.h
--rw-r--r--   0 root         (0) root         (0)    10222 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 root         (0) root         (0)    22185 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 root         (0) root         (0)    13910 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 root         (0) root         (0)     7076 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/IO.h
--rw-r--r--   0 root         (0) root         (0)    38153 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/AssignEvaluator.h
--rw-r--r--   0 root         (0) root         (0)    12666 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 root         (0) root         (0)     3519 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 root         (0) root         (0)     6379 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Random.h
--rw-r--r--   0 root         (0) root         (0)     3582 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 root         (0) root         (0)     7235 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Product.h
--rw-r--r--   0 root         (0) root         (0)    40865 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 root         (0) root         (0)     5619 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 root         (0) root         (0)     3462 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 root         (0) root         (0)     5705 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 root         (0) root         (0)    10991 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 root         (0) root         (0)     5689 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 root         (0) root         (0)     8179 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 root         (0) root         (0)    37234 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 root         (0) root         (0)     3865 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Stride.h
--rwxr-xr-x   0 root         (0) root         (0)    12479 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Assign_MKL.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 root         (0) root         (0)    15366 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/Complex.h
--rwxr-xr-x   0 root         (0) root         (0)    32283 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)     4418 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 root         (0) root         (0)     1194 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/TypeCasting.h
--rw-r--r--   0 root         (0) root         (0)    18037 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 root         (0) root         (0)    27841 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)    17776 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/MathFunctions.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 root         (0) root         (0)     1989 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 root         (0) root         (0)     1746 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 root         (0) root         (0)     5509 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
--rw-r--r--   0 root         (0) root         (0)     4240 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 root         (0) root         (0)    10744 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)    23528 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 root         (0) root         (0)     2387 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 root         (0) root         (0)    35538 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 root         (0) root         (0)     1759 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/TypeCasting.h
--rw-r--r--   0 root         (0) root         (0)    19426 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/Complex.h
--rwxr-xr-x   0 root         (0) root         (0)    35843 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)    18888 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/MathFunctions.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 root         (0) root         (0)    17706 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 root         (0) root         (0)    28726 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)     2846 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/MathFunctions.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 root         (0) root         (0)    50985 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)    15733 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 root         (0) root         (0)    16443 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rwxr-xr-x   0 root         (0) root         (0)    37671 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
--rw-r--r--   0 root         (0) root         (0)    10797 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 root         (0) root         (0)     6775 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 root         (0) root         (0)    31424 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 root         (0) root         (0)    12115 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/Array.h
--rw-r--r--   0 root         (0) root         (0)    62197 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Core/CoreEvaluators.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/StlSupport/
--rw-r--r--   0 root         (0) root         (0)     2809 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/StlSupport/details.h
--rw-r--r--   0 root         (0) root         (0)     5330 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 root         (0) root         (0)     5117 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 root         (0) root         (0)     4147 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/StlSupport/StdList.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/Householder/
--rw-r--r--   0 root         (0) root         (0)     5345 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 root         (0) root         (0)     4481 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 root         (0) root         (0)    20603 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/
--rw-r--r--   0 root         (0) root         (0)     6582 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 root         (0) root         (0)     2049 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 root         (0) root         (0)     4979 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 root         (0) root         (0)     4974 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 root         (0) root         (0)     3681 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 root         (0) root         (0)     4545 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 root         (0) root         (0)     4303 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 root         (0) root         (0)     7601 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 root         (0) root         (0)     6712 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 root         (0) root         (0)    10022 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 root         (0) root         (0)     2889 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
--rw-r--r--   0 root         (0) root         (0)     4181 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 root         (0) root         (0)     5723 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 root         (0) root         (0)    10216 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 root         (0) root         (0)     9028 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 root         (0) root         (0)     8486 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 root         (0) root         (0)    27866 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/
--rw-r--r--   0 root         (0) root         (0)     2191 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 root         (0) root         (0)    14831 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 root         (0) root         (0)     8080 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 root         (0) root         (0)    12487 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 root         (0) root         (0)     6437 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 root         (0) root         (0)     3080 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 root         (0) root         (0)    25592 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 root         (0) root         (0)     7049 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 root         (0) root         (0)     8704 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 root         (0) root         (0)    15492 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 root         (0) root         (0)    12589 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 root         (0) root         (0)     6485 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 root         (0) root         (0)     4424 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 root         (0) root         (0)     4711 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 root         (0) root         (0)     1699 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 root         (0) root         (0)    17923 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 root         (0) root         (0)     5808 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 root         (0) root         (0)     8164 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 root         (0) root         (0)    12720 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 root         (0) root         (0)    25840 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 root         (0) root         (0)     9657 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/TriangularSolver.h
--rw-r--r--   0 root         (0) root         (0)    13178 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 root         (0) root         (0)     8110 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 root         (0) root         (0)     7329 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 root         (0) root         (0)     3175 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 root         (0) root         (0)    10537 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 root         (0) root         (0)     6602 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 root         (0) root         (0)    25715 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 root         (0) root         (0)    52373 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 root         (0) root         (0)     1107 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseFuzzy.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 root         (0) root         (0)     6755 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 root         (0) root         (0)     9289 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 root         (0) root         (0)     7762 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 root         (0) root         (0)    15062 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 root         (0) root         (0)     4158 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
--rw-r--r--   0 root         (0) root         (0)    15234 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 root         (0) root         (0)     7253 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 root         (0) root         (0)    11527 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/LU/
--rw-r--r--   0 root         (0) root         (0)     3057 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 root         (0) root         (0)    15064 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 root         (0) root         (0)    32803 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 root         (0) root         (0)     3555 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
--rw-r--r--   0 root         (0) root         (0)    21478 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/PartialPivLU.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/LU/arch/
--rw-r--r--   0 root         (0) root         (0)    13669 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/plugins/
--rw-r--r--   0 root         (0) root         (0)    13132 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 root         (0) root         (0)     6375 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 root         (0) root         (0)    37403 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 root         (0) root         (0)     4828 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 root         (0) root         (0)    16929 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 root         (0) root         (0)     5621 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 root         (0) root         (0)     2937 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/MetisSupport/
--rw-r--r--   0 root         (0) root         (0)     4588 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/include/Eigen/src/SparseQR/
--rw-r--r--   0 root         (0) root         (0)    28373 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/src/SparseQR/SparseQR.h
--rw-r--r--   0 root         (0) root         (0)     1382 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/UmfPackSupport
--rw-r--r--   0 root         (0) root         (0)      797 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/StdDeque
--rw-r--r--   0 root         (0) root         (0)      694 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1162 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SPQRSupport
--rw-r--r--   0 root         (0) root         (0)     1317 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/QR
--rw-r--r--   0 root         (0) root         (0)     1900 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/CholmodSupport
--rw-r--r--   0 root         (0) root         (0)     2243 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SuperLUSupport
--rw-r--r--   0 root         (0) root         (0)     1822 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Eigenvalues
--rw-r--r--   0 root         (0) root         (0)      803 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/StdVector
--rw-r--r--   0 root         (0) root         (0)      939 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Jacobi
--rw-r--r--   0 root         (0) root         (0)     2050 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Geometry
--rwxr-xr-x   0 root         (0) root         (0)     1116 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/PardisoSupport
--rw-r--r--   0 root         (0) root         (0)    17961 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Core
--rw-r--r--   0 root         (0) root         (0)      874 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Householder
--rw-r--r--   0 root         (0) root         (0)      945 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 root         (0) root         (0)     1713 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SparseLU
--rw-r--r--   0 root         (0) root         (0)     2240 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SparseCore
--rw-r--r--   0 root         (0) root         (0)     2083 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 root         (0) root         (0)     1433 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/LU
--rw-r--r--   0 root         (0) root         (0)      919 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Sparse
--rw-r--r--   0 root         (0) root         (0)       35 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/Eigen
--rw-r--r--   0 root         (0) root         (0)      991 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/MetisSupport
--rw-r--r--   0 root         (0) root         (0)     1222 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/SparseQR
--rw-r--r--   0 root         (0) root         (0)      726 2020-08-04 15:26:24.000000 tomotopy-0.9.0/include/Eigen/StdList
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15967 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       48 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       25 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)    21962 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-04 15:26:33.000000 tomotopy-0.9.0/tomotopy/
--rw-r--r--   0 root         (0) root         (0)       21 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/_version.py
--rw-r--r--   0 root         (0) root         (0)     7326 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14722 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/_summary.py
--rw-r--r--   0 root         (0) root         (0)      782 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/label.py
--rw-r--r--   0 root         (0) root         (0)    14285 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/utils.py
--rw-r--r--   0 root         (0) root         (0)     2553 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/auto_labeling_code_with_porter.rst
--rw-r--r--   0 root         (0) root         (0)    20900 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/documentation.rst
--rw-r--r--   0 root         (0) root         (0)    24491 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/documentation.kr.rst
--rw-r--r--   0 root         (0) root         (0)     2244 2020-08-04 15:26:16.000000 tomotopy-0.9.0/tomotopy/auto_labeling_code.rst
--rw-r--r--   0 root         (0) root         (0)      100 2020-08-04 15:26:16.000000 tomotopy-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    21962 2020-08-04 15:26:33.000000 tomotopy-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)    22109 2020-08-08 09:33:02.000000 tomotopy-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      100 2020-08-08 09:32:45.000000 tomotopy-0.9.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/Labeling/
+-rw-r--r--   0 root         (0) root         (0)     9159 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Labeling/FoRelevance.cpp
+-rw-r--r--   0 root         (0) root         (0)      822 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Labeling/Labeler.h
+-rw-r--r--   0 root         (0) root         (0)     2367 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Labeling/FoRelevance.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/Utils/
+-rw-r--r--   0 root         (0) root         (0)     8881 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/math.h
+-rw-r--r--   0 root         (0) root         (0)   197065 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/rtnorm.hpp
+-rw-r--r--   0 root         (0) root         (0)     1690 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/LUT.hpp
+-rw-r--r--   0 root         (0) root         (0)     4652 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/Trie.hpp
+-rw-r--r--   0 root         (0) root         (0)     4380 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/sample.hpp
+-rw-r--r--   0 root         (0) root         (0)    23184 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/avx_mathfun.h
+-rw-r--r--   0 root         (0) root         (0)    16752 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/PolyaGammaHybrid.hpp
+-rw-r--r--   0 root         (0) root         (0)     2275 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/avx_gamma.h
+-rw-r--r--   0 root         (0) root         (0)    21675 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/sse_mathfun.h
+-rw-r--r--   0 root         (0) root         (0)    22082 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/serializer.hpp
+-rw-r--r--   0 root         (0) root         (0)     5055 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/PolyaGamma.hpp
+-rw-r--r--   0 root         (0) root         (0)     5205 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/LBFGS.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/Utils/LBFGS/
+-rw-r--r--   0 root         (0) root         (0)     3326 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/LBFGS/LineSearchBacktracking.h
+-rw-r--r--   0 root         (0) root         (0)     7737 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/LBFGS/Param.h
+-rw-r--r--   0 root         (0) root         (0)     3659 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/LBFGS/LineSearchBracketing.h
+-rw-r--r--   0 root         (0) root         (0)     6954 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/Utils.hpp
+-rw-r--r--   0 root         (0) root         (0)     1719 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/MultiNormalDistribution.hpp
+-rw-r--r--   0 root         (0) root         (0)     2119 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/sse_gamma.h
+-rw-r--r--   0 root         (0) root         (0)     3499 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/AliasMethod.hpp
+-rw-r--r--   0 root         (0) root         (0)     1550 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/Dictionary.h
+-rw-r--r--   0 root         (0) root         (0)      584 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/exception.h
+-rw-r--r--   0 root         (0) root         (0)     2762 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/TruncMultiNormal.hpp
+-rw-r--r--   0 root         (0) root         (0)    11996 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/tvector.hpp
+-rw-r--r--   0 root         (0) root         (0)     4257 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/ThreadPool.hpp
+-rw-r--r--   0 root         (0) root         (0)     1359 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/text.hpp
+-rw-r--r--   0 root         (0) root         (0)     5156 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/EigenAddonOps.hpp
+-rw-r--r--   0 root         (0) root         (0)     3206 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/Utils/slp.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/TopicModel/
+-rw-r--r--   0 root         (0) root         (0)      522 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DTModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      436 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DMRModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      398 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HDPModel.cpp
+-rw-r--r--   0 root         (0) root         (0)    21110 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HLDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)      788 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HPA.h
+-rw-r--r--   0 root         (0) root         (0)      525 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/GDMRModel.cpp
+-rw-r--r--   0 root         (0) root         (0)    15838 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/GDMRModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    20264 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/TopicModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    10006 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/CTModel.hpp
+-rw-r--r--   0 root         (0) root         (0)     2202 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DMR.h
+-rw-r--r--   0 root         (0) root         (0)      388 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LDAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      455 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PLDAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)     4328 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LDA.h
+-rw-r--r--   0 root         (0) root         (0)     1862 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LLDA.h
+-rw-r--r--   0 root         (0) root         (0)      642 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DTM.h
+-rw-r--r--   0 root         (0) root         (0)     1260 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/CT.h
+-rw-r--r--   0 root         (0) root         (0)    19326 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HDPModel.hpp
+-rw-r--r--   0 root         (0) root         (0)     2349 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DT.h
+-rw-r--r--   0 root         (0) root         (0)     2095 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HDP.h
+-rw-r--r--   0 root         (0) root         (0)      383 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      427 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PLDA.h
+-rw-r--r--   0 root         (0) root         (0)     8112 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PLDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    19174 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DTModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    13176 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/DMRModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    19396 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HPAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)     1598 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PA.h
+-rw-r--r--   0 root         (0) root         (0)      563 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/SLDAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)    18634 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/MGLDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)    16267 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/PAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)      381 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/CTModel.cpp
+-rw-r--r--   0 root         (0) root         (0)    13807 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LDACVB0Model.hpp
+-rw-r--r--   0 root         (0) root         (0)     1454 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/GDMR.h
+-rw-r--r--   0 root         (0) root         (0)     3042 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/MGLDA.h
+-rw-r--r--   0 root         (0) root         (0)     1341 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HLDA.h
+-rw-r--r--   0 root         (0) root         (0)      417 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HLDAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      555 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/MGLDAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)    34290 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)     2070 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/SLDA.h
+-rw-r--r--   0 root         (0) root         (0)    15542 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/SLDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)     7269 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LLDAModel.hpp
+-rw-r--r--   0 root         (0) root         (0)      556 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/HPAModel.cpp
+-rw-r--r--   0 root         (0) root         (0)      379 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/TopicModel/LLDAModel.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/src/python/
+-rw-r--r--   0 root         (0) root         (0)     7846 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_HLDA.cpp
+-rw-r--r--   0 root         (0) root         (0)    26451 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_LDA.cpp
+-rw-r--r--   0 root         (0) root         (0)    11555 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/PyUtils.h
+-rw-r--r--   0 root         (0) root         (0)    11120 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_DMR.cpp
+-rw-r--r--   0 root         (0) root         (0)    13788 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_PA.cpp
+-rw-r--r--   0 root         (0) root         (0)      221 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/label.h
+-rw-r--r--   0 root         (0) root         (0)    10707 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/module.h
+-rw-r--r--   0 root         (0) root         (0)     7144 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_HDP.cpp
+-rw-r--r--   0 root         (0) root         (0)    13129 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_label.cpp
+-rw-r--r--   0 root         (0) root         (0)   131022 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/docs.h
+-rw-r--r--   0 root         (0) root         (0)     7566 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_CT.cpp
+-rw-r--r--   0 root         (0) root         (0)    11013 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_MGLDA.cpp
+-rw-r--r--   0 root         (0) root         (0)     7257 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_HPA.cpp
+-rw-r--r--   0 root         (0) root         (0)    14132 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_GDMR.cpp
+-rw-r--r--   0 root         (0) root         (0)     9753 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_PLDA.cpp
+-rw-r--r--   0 root         (0) root         (0)    20283 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_main.cpp
+-rw-r--r--   0 root         (0) root         (0)    13865 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_SLDA.cpp
+-rw-r--r--   0 root         (0) root         (0)    16320 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_DT.cpp
+-rw-r--r--   0 root         (0) root         (0)     6541 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/label_docs.h
+-rw-r--r--   0 root         (0) root         (0)    10720 2020-08-08 09:32:45.000000 tomotopy-0.9.1/src/python/py_LLDA.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15967 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)    22109 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       48 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/
+-rw-r--r--   0 root         (0) root         (0)      122 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Dense
+-rw-r--r--   0 root         (0) root         (0)      919 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Sparse
+-rw-r--r--   0 root         (0) root         (0)       35 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Eigen
+-rw-r--r--   0 root         (0) root         (0)      726 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/StdList
+-rw-r--r--   0 root         (0) root         (0)     2243 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SuperLUSupport
+-rwxr-xr-x   0 root         (0) root         (0)     1116 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/PardisoSupport
+-rw-r--r--   0 root         (0) root         (0)      797 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/StdDeque
+-rw-r--r--   0 root         (0) root         (0)     2483 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/OrderingMethods
+-rw-r--r--   0 root         (0) root         (0)     2083 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/IterativeLinearSolvers
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 root         (0) root         (0)    34345 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 root         (0) root         (0)    20032 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/StlSupport/
+-rw-r--r--   0 root         (0) root         (0)     4147 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 root         (0) root         (0)     5117 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 root         (0) root         (0)     5330 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 root         (0) root         (0)     2809 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 root         (0) root         (0)    62266 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 root         (0) root         (0)    16396 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 root         (0) root         (0)     5229 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 root         (0) root         (0)    15062 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 root         (0) root         (0)     7253 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 root         (0) root         (0)    15234 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 root         (0) root         (0)    11527 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 root         (0) root         (0)     4158 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+-rw-r--r--   0 root         (0) root         (0)     7762 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 root         (0) root         (0)     9289 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 root         (0) root         (0)     6755 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/
+-rw-r--r--   0 root         (0) root         (0)    21646 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 root         (0) root         (0)    40865 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)     7239 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 root         (0) root         (0)    21123 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 root         (0) root         (0)    31424 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 root         (0) root         (0)     5689 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 root         (0) root         (0)    12115 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 root         (0) root         (0)     6379 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 root         (0) root         (0)    10991 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/MapBase.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/
+-rw-r--r--   0 root         (0) root         (0)    14722 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 root         (0) root         (0)    18478 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     9901 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 root         (0) root         (0)     6368 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)    13979 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 root         (0) root         (0)    81534 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 root         (0) root         (0)     6907 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)    19632 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     4905 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 root         (0) root         (0)    20403 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     5017 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)     4066 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 root         (0) root         (0)    26808 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 root         (0) root         (0)     5209 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)    10571 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)    15188 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 root         (0) root         (0)    13743 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)     6105 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 root         (0) root         (0)     5741 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverVector.h
+-rw-r--r--   0 root         (0) root         (0)    11198 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)     6513 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 root         (0) root         (0)     7593 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 root         (0) root         (0)    13910 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     4525 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 root         (0) root         (0)     9597 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 root         (0) root         (0)     6775 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 root         (0) root         (0)     8179 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 root         (0) root         (0)     3400 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 root         (0) root         (0)    12800 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 root         (0) root         (0)    14245 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 root         (0) root         (0)     5595 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 root         (0) root         (0)     8074 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Visitor.h
+-rw-r--r--   0 root         (0) root         (0)    27420 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 root         (0) root         (0)     7235 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 root         (0) root         (0)     6795 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 root         (0) root         (0)     7076 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 root         (0) root         (0)     6020 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 root         (0) root         (0)     5705 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Fuzzy.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 root         (0) root         (0)     2846 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    17706 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 root         (0) root         (0)    28726 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 root         (0) root         (0)    10797 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    16443 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rwxr-xr-x   0 root         (0) root         (0)    37671 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 root         (0) root         (0)     4418 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    15366 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rwxr-xr-x   0 root         (0) root         (0)    32283 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 root         (0) root         (0)     2387 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)     4240 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 root         (0) root         (0)    35538 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 root         (0) root         (0)    10744 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 root         (0) root         (0)     5509 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+-rw-r--r--   0 root         (0) root         (0)    23528 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/Half.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 root         (0) root         (0)    18888 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    19426 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/Complex.h
+-rwxr-xr-x   0 root         (0) root         (0)    35843 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 root         (0) root         (0)     1759 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 root         (0) root         (0)     1989 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 root         (0) root         (0)     1746 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 root         (0) root         (0)    15733 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    50985 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 root         (0) root         (0)    17776 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 root         (0) root         (0)    18037 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 root         (0) root         (0)    27841 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 root         (0) root         (0)     1194 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+-rw-r--r--   0 root         (0) root         (0)     7073 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 root         (0) root         (0)    19067 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 root         (0) root         (0)    23213 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 root         (0) root         (0)    62197 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 root         (0) root         (0)     4249 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/BooleanRedux.h
+-rwxr-xr-x   0 root         (0) root         (0)    12479 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 root         (0) root         (0)    24212 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 root         (0) root         (0)     3462 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 root         (0) root         (0)    10222 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 root         (0) root         (0)     3519 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 root         (0) root         (0)     2720 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 root         (0) root         (0)    17852 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 root         (0) root         (0)    29441 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 root         (0) root         (0)     9234 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 root         (0) root         (0)     3582 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 root         (0) root         (0)    11507 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 root         (0) root         (0)    49497 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 root         (0) root         (0)    37234 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     3877 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 root         (0) root         (0)     1697 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 root         (0) root         (0)      970 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 root         (0) root         (0)     2683 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 root         (0) root         (0)     3369 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 root         (0) root         (0)    22185 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 root         (0) root         (0)     9136 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 root         (0) root         (0)     3865 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 root         (0) root         (0)     4200 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 root         (0) root         (0)     5619 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 root         (0) root         (0)     8256 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 root         (0) root         (0)    21959 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 root         (0) root         (0)     5282 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/CwiseUnaryView.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/
+-rw-r--r--   0 root         (0) root         (0)       85 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 root         (0) root         (0)      856 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 root         (0) root         (0)    34198 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/XprHelper.h
+-rwxr-xr-x   0 root         (0) root         (0)     4026 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/MKL_support.h
+-rwxr-xr-x   0 root         (0) root         (0)    20586 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 root         (0) root         (0)    36570 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/Macros.h
+-rwxr-xr-x   0 root         (0) root         (0)    15722 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 root         (0) root         (0)    10518 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 root         (0) root         (0)    40579 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/Memory.h
+-rw-r--r--   0 root         (0) root         (0)    14150 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 root         (0) root         (0)    21579 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 root         (0) root         (0)     3981 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 root         (0) root         (0)    18064 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 root         (0) root         (0)     6990 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 root         (0) root         (0)     4769 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/ForceAlignedAccess.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/
+-rw-r--r--   0 root         (0) root         (0)     8229 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 root         (0) root         (0)     4400 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 root         (0) root         (0)    18263 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 root         (0) root         (0)      607 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 root         (0) root         (0)     6284 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 root         (0) root         (0)    27944 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/functors/UnaryFunctors.h
+-rw-r--r--   0 root         (0) root         (0)    14386 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 root         (0) root         (0)     4365 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 root         (0) root         (0)     7692 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 root         (0) root         (0)    12666 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 root         (0) root         (0)    38153 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/AssignEvaluator.h
+-rw-r--r--   0 root         (0) root         (0)    45180 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 root         (0) root         (0)    14777 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Core/Transpose.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/
+-rw-r--r--   0 root         (0) root         (0)    10022 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     7601 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 root         (0) root         (0)     4979 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 root         (0) root         (0)     9028 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 root         (0) root         (0)     5723 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 root         (0) root         (0)     4181 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 root         (0) root         (0)     6712 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 root         (0) root         (0)     8486 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 root         (0) root         (0)     6582 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 root         (0) root         (0)     3681 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 root         (0) root         (0)    27866 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 root         (0) root         (0)     4974 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 root         (0) root         (0)     4303 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 root         (0) root         (0)     2049 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 root         (0) root         (0)     2889 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+-rw-r--r--   0 root         (0) root         (0)     4545 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 root         (0) root         (0)    10216 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Householder/
+-rw-r--r--   0 root         (0) root         (0)    20603 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Householder/HouseholderSequence.h
+-rw-r--r--   0 root         (0) root         (0)     5345 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 root         (0) root         (0)     4481 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Householder/BlockHouseholder.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/misc/
+-rw-r--r--   0 root         (0) root         (0)     2742 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/Kernel.h
+-rwxr-xr-x   0 root         (0) root         (0)  1058368 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 root         (0) root         (0)     1748 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 root         (0) root         (0)     7834 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/lapack.h
+-rw-r--r--   0 root         (0) root         (0)     2913 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 root         (0) root         (0)    30560 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 root         (0) root         (0)      474 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SparseQR/
+-rw-r--r--   0 root         (0) root         (0)    28373 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 root         (0) root         (0)    22307 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SVD/
+-rw-r--r--   0 root         (0) root         (0)    15957 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SVD/UpperBidiagonalization.h
+-rw-r--r--   0 root         (0) root         (0)    12740 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 root         (0) root         (0)    32949 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 root         (0) root         (0)    48778 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 root         (0) root         (0)     5099 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/plugins/
+-rw-r--r--   0 root         (0) root         (0)    16929 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 root         (0) root         (0)     6375 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 root         (0) root         (0)     4828 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 root         (0) root         (0)    13132 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 root         (0) root         (0)    37403 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 root         (0) root         (0)     2937 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 root         (0) root         (0)     5621 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Jacobi/
+-rw-r--r--   0 root         (0) root         (0)    15902 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 root         (0) root         (0)    17202 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/
+-rw-r--r--   0 root         (0) root         (0)     6191 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Umeyama.h
+-rw-r--r--   0 root         (0) root         (0)     7773 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 root         (0) root         (0)    32152 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 root         (0) root         (0)    60514 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 root         (0) root         (0)     8063 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 root         (0) root         (0)     8949 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 root         (0) root         (0)    20539 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Homogeneous.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 root         (0) root         (0)     5387 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+-rw-r--r--   0 root         (0) root         (0)    11961 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 root         (0) root         (0)     8423 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 root         (0) root         (0)     8308 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 root         (0) root         (0)    14815 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 root         (0) root         (0)     3639 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 root         (0) root         (0)     6877 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Rotation2D.h
+-rwxr-xr-x   0 root         (0) root         (0)     6324 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Geometry/Scaling.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 root         (0) root         (0)    22248 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 root         (0) root         (0)    11405 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/
+-rw-r--r--   0 root         (0) root         (0)    14831 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 root         (0) root         (0)     4711 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 root         (0) root         (0)     7329 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 root         (0) root         (0)     2191 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     5808 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 root         (0) root         (0)     8110 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 root         (0) root         (0)    12589 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 root         (0) root         (0)    12720 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 root         (0) root         (0)    13178 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 root         (0) root         (0)     3175 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 root         (0) root         (0)     6602 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 root         (0) root         (0)    17923 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 root         (0) root         (0)     7049 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 root         (0) root         (0)     8164 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 root         (0) root         (0)    25592 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 root         (0) root         (0)     4424 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 root         (0) root         (0)     9657 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/TriangularSolver.h
+-rw-r--r--   0 root         (0) root         (0)     1699 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 root         (0) root         (0)     1107 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 root         (0) root         (0)    12487 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 root         (0) root         (0)     8080 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 root         (0) root         (0)    25840 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 root         (0) root         (0)     6485 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 root         (0) root         (0)    52373 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 root         (0) root         (0)     3080 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 root         (0) root         (0)    25715 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 root         (0) root         (0)    15492 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 root         (0) root         (0)    10537 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 root         (0) root         (0)     8704 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 root         (0) root         (0)     6437 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseTriangularView.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 root         (0) root         (0)     5539 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 root         (0) root         (0)     4178 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)    17021 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 root         (0) root         (0)    23586 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 root         (0) root         (0)     3650 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)    17176 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 root         (0) root         (0)     4104 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)     9715 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 root         (0) root         (0)    20288 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 root         (0) root         (0)    12558 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 root         (0) root         (0)    33674 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 root         (0) root         (0)    22944 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 root         (0) root         (0)    14351 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 root         (0) root         (0)    22444 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/QR/
+-rw-r--r--   0 root         (0) root         (0)    25478 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 root         (0) root         (0)    20805 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 root         (0) root         (0)    14022 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 root         (0) root         (0)     2993 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)    24881 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 root         (0) root         (0)     4662 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/Cholesky/
+-rw-r--r--   0 root         (0) root         (0)    18395 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 root         (0) root         (0)     3974 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)    24480 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/Cholesky/LDLT.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 root         (0) root         (0)    24010 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 root         (0) root         (0)     6898 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 root         (0) root         (0)     4588 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/LU/
+-rw-r--r--   0 root         (0) root         (0)    32803 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 root         (0) root         (0)    15064 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 root         (0) root         (0)     3057 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/Determinant.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/Eigen/src/LU/arch/
+-rw-r--r--   0 root         (0) root         (0)    13669 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/arch/Inverse_SSE.h
+-rw-r--r--   0 root         (0) root         (0)     3555 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+-rw-r--r--   0 root         (0) root         (0)    21478 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 root         (0) root         (0)    17961 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Core
+-rw-r--r--   0 root         (0) root         (0)      803 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/StdVector
+-rw-r--r--   0 root         (0) root         (0)     1713 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SparseLU
+-rw-r--r--   0 root         (0) root         (0)      694 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      874 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Householder
+-rw-r--r--   0 root         (0) root         (0)     1222 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SparseQR
+-rw-r--r--   0 root         (0) root         (0)     1900 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/CholmodSupport
+-rw-r--r--   0 root         (0) root         (0)      945 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 root         (0) root         (0)     1629 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SVD
+-rw-r--r--   0 root         (0) root         (0)      939 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Jacobi
+-rw-r--r--   0 root         (0) root         (0)     1382 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/UmfPackSupport
+-rw-r--r--   0 root         (0) root         (0)     2050 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Geometry
+-rw-r--r--   0 root         (0) root         (0)     1676 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/PaStiXSupport
+-rw-r--r--   0 root         (0) root         (0)     1162 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SPQRSupport
+-rw-r--r--   0 root         (0) root         (0)     2240 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SparseCore
+-rw-r--r--   0 root         (0) root         (0)     1822 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Eigenvalues
+-rw-r--r--   0 root         (0) root         (0)     1317 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/QR
+-rw-r--r--   0 root         (0) root         (0)     1206 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/Cholesky
+-rw-r--r--   0 root         (0) root         (0)     1371 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/SparseCholesky
+-rw-r--r--   0 root         (0) root         (0)      991 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/MetisSupport
+-rw-r--r--   0 root         (0) root         (0)     1433 2020-08-08 09:32:53.000000 tomotopy-0.9.1/include/Eigen/LU
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/EigenRand/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/include/EigenRand/Dists/
+-rw-r--r--   0 root         (0) root         (0)     3371 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Dists/GammaPoisson.h
+-rw-r--r--   0 root         (0) root         (0)    18387 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Dists/NormalExp.h
+-rw-r--r--   0 root         (0) root         (0)     3038 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Dists/Basic.h
+-rw-r--r--   0 root         (0) root         (0)    24242 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Dists/Discrete.h
+-rw-r--r--   0 root         (0) root         (0)    45286 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Core.h
+-rw-r--r--   0 root         (0) root         (0)      305 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/EigenRand
+-rw-r--r--   0 root         (0) root         (0)    24878 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/MorePacketMath.h
+-rw-r--r--   0 root         (0) root         (0)     9439 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/RandUtils.h
+-rw-r--r--   0 root         (0) root         (0)      406 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/Macro.h
+-rw-r--r--   0 root         (0) root         (0)    14960 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/PacketRandomEngine.h
+-rw-r--r--   0 root         (0) root         (0)     6655 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/PacketFilter.h
+-rw-r--r--   0 root         (0) root         (0)    12126 2020-08-08 09:32:54.000000 tomotopy-0.9.1/include/EigenRand/doc.h
+-rw-r--r--   0 root         (0) root         (0)       38 2020-08-08 09:33:02.000000 tomotopy-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    18162 2020-08-08 09:32:45.000000 tomotopy-0.9.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     3722 2020-08-08 09:32:45.000000 tomotopy-0.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-08 09:33:02.000000 tomotopy-0.9.1/tomotopy/
+-rw-r--r--   0 root         (0) root         (0)      782 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/label.py
+-rw-r--r--   0 root         (0) root         (0)    24689 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/documentation.kr.rst
+-rw-r--r--   0 root         (0) root         (0)    14285 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/auto_labeling_code.rst
+-rw-r--r--   0 root         (0) root         (0)    15222 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/_summary.py
+-rw-r--r--   0 root         (0) root         (0)       21 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/_version.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/auto_labeling_code_with_porter.rst
+-rw-r--r--   0 root         (0) root         (0)    21015 2020-08-08 09:32:45.000000 tomotopy-0.9.1/tomotopy/documentation.rst
```

### Comparing `tomotopy-0.9.0/src/TopicModel/HPAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/HPAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/SLDAModel.cpp` & `tomotopy-0.9.1/src/TopicModel/SLDAModel.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/GDMR.h` & `tomotopy-0.9.1/src/TopicModel/GDMR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HDPModel.hpp` & `tomotopy-0.9.1/src/TopicModel/HDPModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HLDA.h` & `tomotopy-0.9.1/src/TopicModel/HLDA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HLDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/HLDAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/PA.h` & `tomotopy-0.9.1/src/TopicModel/PA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/DMR.h` & `tomotopy-0.9.1/src/TopicModel/DMR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/LLDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/LLDAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/CTModel.hpp` & `tomotopy-0.9.1/src/TopicModel/CTModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/LDA.h` & `tomotopy-0.9.1/src/TopicModel/LDA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/PAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/PAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/SLDA.h` & `tomotopy-0.9.1/src/TopicModel/SLDA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/DTM.h` & `tomotopy-0.9.1/src/TopicModel/DTM.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/CT.h` & `tomotopy-0.9.1/src/TopicModel/CT.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/MGLDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/MGLDAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/DT.h` & `tomotopy-0.9.1/src/TopicModel/DT.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/MGLDAModel.cpp` & `tomotopy-0.9.1/src/TopicModel/MGLDAModel.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HPAModel.cpp` & `tomotopy-0.9.1/src/TopicModel/HPAModel.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/GDMRModel.hpp` & `tomotopy-0.9.1/src/TopicModel/GDMRModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HDP.h` & `tomotopy-0.9.1/src/TopicModel/HDP.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/LDACVB0Model.hpp` & `tomotopy-0.9.1/src/TopicModel/LDACVB0Model.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/GDMRModel.cpp` & `tomotopy-0.9.1/src/TopicModel/GDMRModel.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/TopicModel.hpp` & `tomotopy-0.9.1/src/TopicModel/TopicModel.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
 	class TopicModel : public _Interface
 	{
 		friend class Document;
 	public:
 		using DocType = _DocType;
 	protected:
 		_RandGen rg;
+		std::vector<_RandGen> localRG;
 		std::vector<Vid> words;
 		std::vector<uint32_t> wOffsetByDoc;
 
 		std::vector<DocType> docs;
 		std::vector<uint64_t> vocabCf;
 		std::vector<uint64_t> vocabDf;
 		size_t globalStep = 0;
@@ -428,15 +429,15 @@
 
 		int restoreFromTrainingError(const exception::TrainingError& e, ThreadPool& pool, _ModelState* localData, _RandGen* rgs)
 		{
 			throw e;
 		}
 
 	public:
-		TopicModel(const _RandGen& _rg) : rg(_rg)
+		TopicModel(size_t _rg) : rg(_rg)
 		{
 		}
 
 		size_t getNumDocs() const override
 		{ 
 			return docs.size(); 
 		}
@@ -493,18 +494,22 @@
 			if (numWorkers == 1 || (_Flags & flags::shared_state)) ps = ParallelScheme::none;
 			if (!cachedPool || cachedPool->getNumWorkers() != numWorkers)
 			{
 				cachedPool = make_unique<ThreadPool>(numWorkers);
 			}
 
 			std::vector<_ModelState> localData;
-			std::vector<_RandGen> localRG;
+
+			while(localRG.size() < numWorkers)
+			{
+				localRG.emplace_back(rg());
+			}
+
 			for (size_t i = 0; i < numWorkers; ++i)
 			{
-				localRG.emplace_back(_RandGen{rg()});
 				if(ps == ParallelScheme::copy_merge) localData.emplace_back(static_cast<_Derived*>(this)->globalState);
 			}
 
 			if (ps == ParallelScheme::partition)
 			{
 				localData.resize(numWorkers);
 				static_cast<_Derived*>(this)->updatePartition(*cachedPool, globalState, localData.data(), docs.begin(), docs.end(),
```

### Comparing `tomotopy-0.9.0/src/TopicModel/DTModel.hpp` & `tomotopy-0.9.1/src/TopicModel/DTModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/LLDA.h` & `tomotopy-0.9.1/src/TopicModel/LLDA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/MGLDA.h` & `tomotopy-0.9.1/src/TopicModel/MGLDA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/HPA.h` & `tomotopy-0.9.1/src/TopicModel/HPA.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/SLDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/SLDAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/PLDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/PLDAModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/DTModel.cpp` & `tomotopy-0.9.1/src/TopicModel/DTModel.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/DMRModel.hpp` & `tomotopy-0.9.1/src/TopicModel/DMRModel.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/TopicModel/LDAModel.hpp` & `tomotopy-0.9.1/src/TopicModel/LDAModel.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -15,36 +15,41 @@
 * Newman, D., Asuncion, A., Smyth, P., & Welling, M. (2009). Distributed algorithms for topic models. Journal of Machine Learning Research, 10(Aug), 1801-1828.
 
 Term Weighting Scheme is based on following paper:
 * Wilson, A. T., & Chew, P. A. (2010, June). Term weighting schemes for latent dirichlet allocation. In human language technologies: The 2010 annual conference of the North American Chapter of the Association for Computational Linguistics (pp. 465-473). Association for Computational Linguistics.
 
 */
 
+#ifdef TMT_SCALAR_RNG
 #define TMT_SWITCH_TW(TW, SRNG, MDL, ...) do{\
-		/*if(SRNG){\
+		{\
 			switch (TW){\
 			case TermWeight::one:\
 				return new MDL<TermWeight::one, ScalarRandGen>(__VA_ARGS__);\
 			case TermWeight::idf:\
 				return new MDL<TermWeight::idf, ScalarRandGen>(__VA_ARGS__);\
 			case TermWeight::pmi:\
 				return new MDL<TermWeight::pmi, ScalarRandGen>(__VA_ARGS__);\
 			}\
 		}\
-		else*/{\
+		return nullptr; } while(0)
+#else
+#define TMT_SWITCH_TW(TW, SRNG, MDL, ...) do{\
+		{\
 			switch (TW){\
 			case TermWeight::one:\
 				return new MDL<TermWeight::one, RandGen>(__VA_ARGS__);\
 			case TermWeight::idf:\
 				return new MDL<TermWeight::idf, RandGen>(__VA_ARGS__);\
 			case TermWeight::pmi:\
 				return new MDL<TermWeight::pmi, RandGen>(__VA_ARGS__);\
 			}\
 		}\
 		return nullptr; } while(0)
+#endif
 
 #define GETTER(name, type, field) type get##name() const override { return field; }
 
 namespace tomoto
 {
 	template<TermWeight _tw>
 	struct ModelStateLDA
```

### Comparing `tomotopy-0.9.0/src/Utils/slp.hpp` & `tomotopy-0.9.1/src/Utils/slp.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/tvector.hpp` & `tomotopy-0.9.1/src/Utils/tvector.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/AliasMethod.hpp` & `tomotopy-0.9.1/src/Utils/AliasMethod.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/Trie.hpp` & `tomotopy-0.9.1/src/Utils/Trie.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/LBFGS.h` & `tomotopy-0.9.1/src/Utils/LBFGS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/sample.hpp` & `tomotopy-0.9.1/src/Utils/sample.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -103,17 +103,18 @@
 				arr[i + 1] += acc;
 				arr[i + 2] += acc;
 				arr[i + 3] += acc;
 
 				acc = arr[i + 3];
 			}
 
-			for (int i = n4; i < n; ++i)
+			if (!n4) n4 = 1;
+			for (size_t i = n4; i < n; ++i)
 			{
-				arr[i] += acc;
+				arr[i] += arr[i - 1];
 			}
 		}
 #endif
 
 		template<class RealIt, class Random>
 		inline size_t sampleFromDiscrete(RealIt begin, RealIt end, Random& rg)
 		{
```

### Comparing `tomotopy-0.9.0/src/Utils/ThreadPool.hpp` & `tomotopy-0.9.1/src/Utils/ThreadPool.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/TruncMultiNormal.hpp` & `tomotopy-0.9.1/src/Utils/TruncMultiNormal.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/PolyaGamma.hpp` & `tomotopy-0.9.1/src/Utils/PolyaGamma.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/PolyaGammaHybrid.hpp` & `tomotopy-0.9.1/src/Utils/PolyaGammaHybrid.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/Utils.hpp` & `tomotopy-0.9.1/src/Utils/Utils.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/LUT.hpp` & `tomotopy-0.9.1/src/Utils/LUT.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/avx_mathfun.h` & `tomotopy-0.9.1/src/Utils/avx_mathfun.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/Dictionary.h` & `tomotopy-0.9.1/src/Utils/Dictionary.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/rtnorm.hpp` & `tomotopy-0.9.1/src/Utils/rtnorm.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/avx_gamma.h` & `tomotopy-0.9.1/src/Utils/avx_gamma.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/exception.h` & `tomotopy-0.9.1/src/Utils/exception.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/math.h` & `tomotopy-0.9.1/src/Utils/math.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/LBFGS/LineSearchBracketing.h` & `tomotopy-0.9.1/src/Utils/LBFGS/LineSearchBracketing.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/LBFGS/LineSearchBacktracking.h` & `tomotopy-0.9.1/src/Utils/LBFGS/LineSearchBacktracking.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/LBFGS/Param.h` & `tomotopy-0.9.1/src/Utils/LBFGS/Param.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/text.hpp` & `tomotopy-0.9.1/src/Utils/text.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/serializer.hpp` & `tomotopy-0.9.1/src/Utils/serializer.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/sse_mathfun.h` & `tomotopy-0.9.1/src/Utils/sse_mathfun.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/MultiNormalDistribution.hpp` & `tomotopy-0.9.1/src/Utils/MultiNormalDistribution.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/EigenAddonOps.hpp` & `tomotopy-0.9.1/src/Utils/EigenAddonOps.hpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Utils/sse_gamma.h` & `tomotopy-0.9.1/src/Utils/sse_gamma.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_HDP.cpp` & `tomotopy-0.9.1/src/python/py_HDP.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/PyUtils.h` & `tomotopy-0.9.1/src/python/PyUtils.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_DT.cpp` & `tomotopy-0.9.1/src/python/py_DT.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_LDA.cpp` & `tomotopy-0.9.1/src/python/py_LDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_CT.cpp` & `tomotopy-0.9.1/src/python/py_CT.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,17 @@
 	{ nullptr }
 };
 
 
 static PyGetSetDef CT_getseters[] = {
 	{ (char*)"num_beta_sample", (getter)CT_getNumBetaSample, (setter)CT_setNumBetaSample, CT_num_beta_sample__doc__, nullptr },
 	{ (char*)"num_tmn_sample", (getter)CT_getNumTMNSample, (setter)CT_setNumTMNSample, CT_num_tmn_sample__doc__, nullptr },
-	{ (char*)"prior_mean", (getter)CT_getPriorMean, nullptr, CT_get_prior_mean__doc__, nullptr },
-	{ (char*)"prior_cov", (getter)CT_getPriorCov, nullptr, CT_get_prior_cov__doc__, nullptr },
+	{ (char*)"prior_mean", (getter)CT_getPriorMean, nullptr, CT_prior_mean__doc__, nullptr },
+	{ (char*)"prior_cov", (getter)CT_getPriorCov, nullptr, CT_prior_cov__doc__, nullptr },
+	{ (char*)"alpha", nullptr, nullptr, CT_alpha__doc__, nullptr },
 	{ nullptr },
 };
 
 
 PyTypeObject CT_type = {
 	PyVarObject_HEAD_INIT(nullptr, 0)
 	"tomotopy.CTModel",             /* tp_name */
```

### Comparing `tomotopy-0.9.0/src/python/module.h` & `tomotopy-0.9.1/src/python/module.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_HPA.cpp` & `tomotopy-0.9.1/src/python/py_HPA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_MGLDA.cpp` & `tomotopy-0.9.1/src/python/py_MGLDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_label.cpp` & `tomotopy-0.9.1/src/python/py_label.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_main.cpp` & `tomotopy-0.9.1/src/python/py_main.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/label_docs.h` & `tomotopy-0.9.1/src/python/label_docs.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_SLDA.cpp` & `tomotopy-0.9.1/src/python/py_SLDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_PLDA.cpp` & `tomotopy-0.9.1/src/python/py_PLDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_HLDA.cpp` & `tomotopy-0.9.1/src/python/py_HLDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_GDMR.cpp` & `tomotopy-0.9.1/src/python/py_GDMR.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_PA.cpp` & `tomotopy-0.9.1/src/python/py_PA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_LLDA.cpp` & `tomotopy-0.9.1/src/python/py_LLDA.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/py_DMR.cpp` & `tomotopy-0.9.1/src/python/py_DMR.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/python/docs.h` & `tomotopy-0.9.1/src/python/docs.h`

 * *Files 0% similar despite different names*

```diff
@@ -1106,27 +1106,31 @@
 ----------
 topic_id : int
     토픽을 가리키는 [0, `k`) 범위의 정수
 )"");
 
 DOC_SIGNATURE_EN_KO(HDP_convert_to_lda__doc__,
 	"convert_to_lda(self, topic_threshold=0.0)",
-	u8R""(Convert the current HDP model to equivalent LDA model and return `(new_lda_model, new_topic_id)`.
+	u8R""(.. versionadded:: 0.8.0
+
+Convert the current HDP model to equivalent LDA model and return `(new_lda_model, new_topic_id)`.
 Topics with proportion less than `topic_threshold` are removed in `new_lda_model`.
 
 `new_topic_id` is an array of length `HDPModel.k` and `new_topic_id[i]` indicates a topic id of new LDA model, equivalent to topic `i` of original HDP model.
 If topic `i` of original HDP model is not alive or is removed in LDA model, `new_topic_id[i]` would be `-1`.
 
 Parameters
 ----------
 topic_threshold : float
     Topics with proportion less than this value is removed in new LDA model.
     The default value is 0, and it means no topic except not alive is removed.
 )"",
-u8R""(현재의 HDP 모델을 동등한 LDA모델로 변환하고, `(new_lda_mode, new_topic_id)`를 반환합니다.
+u8R""(.. versionadded:: 0.8.0
+
+현재의 HDP 모델을 동등한 LDA모델로 변환하고, `(new_lda_mode, new_topic_id)`를 반환합니다.
 이 때 `topic_threshold`보다 작은 비율의 토픽은 `new_lda_model`에서 제거됩니다.
 
 `new_topic_id`는 길이 `HDPModel.k`의 배열이며, `new_topic_id[i]`는 새 LDA 모델에서 원 HDP 모델의 토픽 `i`와 동등한 토픽의 id를 가리킵니다.
 만약 원 HDP 모델의 토픽 `i`가 유효하지 않거나, 새 LDA 모델에서 제거된 것이라면, `new_topic_id[i]`는 `-1`이 됩니다.
 
 Parameters
 ----------
@@ -1792,15 +1796,15 @@
 
 
 /*
 	class CT
 */
 
 DOC_SIGNATURE_EN_KO(CT___init____doc__,
-	"CTModel(tw=TermWeight.ONE, min_cf=0, min_df=0, rm_top=0, k=1, alpha=0.1, eta=0.01, seed=None, corpus=None, transform=None)",
+	"CTModel(tw=TermWeight.ONE, min_cf=0, min_df=0, rm_top=0, k=1, smoothing_alpha=0.1, eta=0.01, seed=None, corpus=None, transform=None)",
 	u8R""(.. versionadded:: 0.2.0
 This type provides Correlated Topic Model (CTM) and its implementation is based on following papers:
 	
 > * Blei, D., & Lafferty, J. (2006). Correlated topic models. Advances in neural information processing systems, 18, 147.
 > * Mimno, D., Wallach, H., & McCallum, A. (2008, December). Gibbs sampling for logistic normal topic models with graph-based priors. In NIPS Workshop on Analyzing Graphs (Vol. 61).
 
 Parameters
@@ -1917,22 +1921,29 @@
 
 If your model shows biased topic correlations, increasing this value may be helpful.)"",
 	u8R""(절단된 다변수 정규분포에서 표본을 추출하기 위한 반복 횟수, 기본값은 5.
 
 만약 결과에서 토픽 간 상관관계가 편향되게 나올 경우 이 값을 키우면 편향을 해소하는 데에 도움이 될 수 있습니다.
 )"");
 
-DOC_VARIABLE_EN_KO(CT_get_prior_mean__doc__,
+DOC_VARIABLE_EN_KO(CT_prior_mean__doc__,
 	u8R""(the mean of prior logistic-normal distribution for the topic distribution (read-only))"",
 	u8R""(토픽의 사전 분포인 로지스틱 정규 분포의 평균 벡터 (읽기전용))"");
 
-DOC_VARIABLE_EN_KO(CT_get_prior_cov__doc__,
+DOC_VARIABLE_EN_KO(CT_prior_cov__doc__,
 	u8R""(the covariance matrix of prior logistic-normal distribution the for topic distribution (read-only))"",
 	u8R""(토픽의 사전 분포인 로지스틱 정규 분포의 공분산 행렬 (읽기전용))"");
 
+DOC_VARIABLE_EN_KO(CT_alpha__doc__,
+    u8R""(This property is not available in `CTModel`. Use `CTModel.prior_mean` and `CTModel.prior_cov` instead.
+
+.. versionadded:: 0.9.1)"",
+    u8R""(이 프로퍼티는 `CTModel`에서 사용불가합니다. 대신 `CTModel.prior_mean`와 `CTModel.prior_cov`를 사용하십시오.
+
+.. versionadded:: 0.9.1)"");
 
 /*
 	class SLDA
 */
 DOC_SIGNATURE_EN_KO(SLDA___init____doc__,
 	"SLDAModel(tw=TermWeight.ONE, min_cf=0, min_df=0, rm_top=0, k=1, vars='', alpha=0.1, eta=0.01, mu=[], nu_sq=[], glm_param=[], seed=None, corpus=None, transform=None)",
 	u8R""(This type provides supervised Latent Dirichlet Allocation(sLDA) topic model and its implementation is based on following papers:
```

### Comparing `tomotopy-0.9.0/src/Labeling/FoRelevance.cpp` & `tomotopy-0.9.1/src/Labeling/FoRelevance.cpp`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Labeling/Labeler.h` & `tomotopy-0.9.1/src/Labeling/Labeler.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/src/Labeling/FoRelevance.h` & `tomotopy-0.9.1/src/Labeling/FoRelevance.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/README.rst` & `tomotopy-0.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 * Pachinko Allocation (`tomotopy.PAModel`)
 * Hierarchical PA (`tomotopy.HPAModel`)
 * Correlated Topic Model (`tomotopy.CTModel`)
 * Dynamic Topic Model (`tomotopy.DTModel`).
 
 Please visit https://bab2min.github.io/tomotopy to see more information.
 
-The most recent version of tomotopy is 0.9.0.
+The most recent version of tomotopy is 0.9.1.
 
 Getting Started
 ---------------
 You can install tomotopy easily using pip. (https://pypi.org/project/tomotopy/)
 ::
 
     $ pip install --upgrade pip
@@ -257,14 +257,18 @@
 License
 ---------
 `tomotopy` is licensed under the terms of MIT License, 
 meaning you can use it for any reasonable purpose and remain in complete ownership of all the documentation you produce.
 
 History
 -------
+* 0.9.1 (2020-08-08)
+    * Memory leaks of version 0.9.0 was fixed.
+    * `tomotopy.CTModel.summary()` was fixed.
+
 * 0.9.0 (2020-08-04)
     * The `tomotopy.LDAModel.summary()` method, which prints human-readable summary of the model, has been added.
     * The random number generator of package has been replaced with `EigenRand`_. It speeds up the random number generation and solves the result difference between platforms.
     * Due to above, even if `seed` is the same, the model training result may be different from the version before 0.9.0.
     * Fixed a training error in `tomotopy.HDPModel`.
     * `tomotopy.DMRModel.alpha` now shows Dirichlet prior of per-document topic distribution by metadata.
     * `tomotopy.DTModel.get_count_by_topics()` has been modified to return a 2-dimensional `ndarray`.
```

### Comparing `tomotopy-0.9.0/setup.py` & `tomotopy-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/doc.h` & `tomotopy-0.9.1/include/EigenRand/doc.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/Dists/Discrete.h` & `tomotopy-0.9.1/include/EigenRand/Dists/Discrete.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/Dists/GammaPoisson.h` & `tomotopy-0.9.1/include/EigenRand/Dists/GammaPoisson.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/Dists/NormalExp.h` & `tomotopy-0.9.1/include/EigenRand/Dists/NormalExp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/Dists/Basic.h` & `tomotopy-0.9.1/include/EigenRand/Dists/Basic.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/Core.h` & `tomotopy-0.9.1/include/EigenRand/Core.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/PacketRandomEngine.h` & `tomotopy-0.9.1/include/EigenRand/PacketRandomEngine.h`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,18 @@
 				aligned = (Ty*)(((size_t)memory + alignment) & ~(alignment - 1));
 			}
 
 			void deallocate()
 			{
 				if (memory)
 				{
+					for (size_t i = 0; i < length; ++i)
+					{
+						aligned[i].~Ty();
+					}
 					std::free(memory);
 					memory = nullptr;
 					aligned = nullptr;
 				}
 			}
 
 			void* memory = nullptr;
@@ -447,22 +451,24 @@
 		public:
 			using result_type = UIntType;
 
 			ParallelRandomEngineAdaptor(size_t seed = BaseRng::default_seed)
 			{
 				for (int i = 0; i < num_parallel; ++i)
 				{
+					rngs[i].~BaseRng();
 					new (&rngs[i]) BaseRng{ seed + i * u64_stride };
 				}
 			}
 
 			ParallelRandomEngineAdaptor(const BaseRng& o)
 			{
 				for (int i = 0; i < num_parallel; ++i)
 				{
+					rngs[i].~BaseRng();
 					new (&rngs[i]) BaseRng{ o };
 				}
 			}
 
 			ParallelRandomEngineAdaptor(const ParallelRandomEngineAdaptor&) = default;
 			ParallelRandomEngineAdaptor(ParallelRandomEngineAdaptor&&) = default;
```

### Comparing `tomotopy-0.9.0/include/EigenRand/MorePacketMath.h` & `tomotopy-0.9.1/include/EigenRand/MorePacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/RandUtils.h` & `tomotopy-0.9.1/include/EigenRand/RandUtils.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/EigenRand/PacketFilter.h` & `tomotopy-0.9.1/include/EigenRand/PacketFilter.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SparseCholesky` & `tomotopy-0.9.1/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/PaStiXSupport` & `tomotopy-0.9.1/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Cholesky` & `tomotopy-0.9.1/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SVD` & `tomotopy-0.9.1/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/OrderingMethods` & `tomotopy-0.9.1/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `tomotopy-0.9.1/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Cholesky/LDLT.h` & `tomotopy-0.9.1/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Cholesky/LLT.h` & `tomotopy-0.9.1/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SVD/UpperBidiagonalization.h` & `tomotopy-0.9.1/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SVD/JacobiSVD.h` & `tomotopy-0.9.1/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SVD/BDCSVD.h` & `tomotopy-0.9.1/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SVD/SVDBase.h` & `tomotopy-0.9.1/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Amd.h` & `tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/OrderingMethods/Ordering.h` & `tomotopy-0.9.1/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `tomotopy-0.9.1/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `tomotopy-0.9.1/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/ColPivHouseholderQR.h` & `tomotopy-0.9.1/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `tomotopy-0.9.1/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/HouseholderQR.h` & `tomotopy-0.9.1/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/QR/FullPivHouseholderQR.h` & `tomotopy-0.9.1/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `tomotopy-0.9.1/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `tomotopy-0.9.1/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealQZ.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/RealSchur.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/EigenSolver.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Jacobi/Jacobi.h` & `tomotopy-0.9.1/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Quaternion.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/AngleAxis.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/AlignedBox.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/RotationBase.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Umeyama.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Translation.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/EulerAngles.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/OrthoMethods.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Rotation2D.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Homogeneous.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Scaling.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Hyperplane.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/ParametrizedLine.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Geometry/Transform.h` & `tomotopy-0.9.1/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/Image.h` & `tomotopy-0.9.1/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/lapacke.h` & `tomotopy-0.9.1/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/Kernel.h` & `tomotopy-0.9.1/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/blas.h` & `tomotopy-0.9.1/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/RealSvd2x2.h` & `tomotopy-0.9.1/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/misc/lapack.h` & `tomotopy-0.9.1/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `tomotopy-0.9.1/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ConditionEstimator.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Dot.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CwiseUnaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Matrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/GeneralProduct.h` & `tomotopy-0.9.1/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CoreIterators.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CwiseUnaryView.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Ref.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/TernaryFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/StlFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/UnaryFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/BinaryFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/NullaryFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `tomotopy-0.9.1/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CwiseTernaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Reverse.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Map.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Replicate.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/DenseCoeffsBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Visitor.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/SolveTriangular.h` & `tomotopy-0.9.1/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/MathFunctionsImpl.h` & `tomotopy-0.9.1/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/PermutationMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/MatrixBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/PlainObjectBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ReturnByValue.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/VectorwiseOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ForceAlignedAccess.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/DenseStorage.h` & `tomotopy-0.9.1/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Solve.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/NestByValue.h` & `tomotopy-0.9.1/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/SolverBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointProduct.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularSolverVector.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/Parallelizer.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `tomotopy-0.9.1/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Swap.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/DenseBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Redux.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/NumTraits.h` & `tomotopy-0.9.1/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/StableNorm.h` & `tomotopy-0.9.1/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Transpositions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Diagonal.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Assign.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/BlasUtil.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/Constants.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/Memory.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/XprHelper.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/Macros.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/MKL_support.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/StaticAssert.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/ForwardDeclarations.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/util/Meta.h` & `tomotopy-0.9.1/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Transpose.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/DiagonalProduct.h` & `tomotopy-0.9.1/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/BooleanRedux.h` & `tomotopy-0.9.1/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/SelfAdjointView.h` & `tomotopy-0.9.1/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ProductEvaluators.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Select.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CwiseBinaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Block.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/GlobalFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/GenericPacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/BandMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/IO.h` & `tomotopy-0.9.1/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/AssignEvaluator.h` & `tomotopy-0.9.1/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/DiagonalMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Inverse.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Random.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/NoAlias.h` & `tomotopy-0.9.1/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Product.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/EigenBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/VectorBlock.h` & `tomotopy-0.9.1/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Fuzzy.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/MapBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CommaInitializer.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ArrayBase.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/TriangularMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Stride.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Assign_MKL.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/Default/Settings.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/Half.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `tomotopy-0.9.1/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/ArrayWrapper.h` & `tomotopy-0.9.1/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CwiseNullaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/Array.h` & `tomotopy-0.9.1/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Core/CoreEvaluators.h` & `tomotopy-0.9.1/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/StlSupport/details.h` & `tomotopy-0.9.1/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/StlSupport/StdVector.h` & `tomotopy-0.9.1/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/StlSupport/StdDeque.h` & `tomotopy-0.9.1/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/StlSupport/StdList.h` & `tomotopy-0.9.1/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Householder/Householder.h` & `tomotopy-0.9.1/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Householder/BlockHouseholder.h` & `tomotopy-0.9.1/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/Householder/HouseholderSequence.h` & `tomotopy-0.9.1/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLUImpl.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseLU/SparseLU.h` & `tomotopy-0.9.1/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseVector.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseAssign.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseTriangularView.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDot.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseBlock.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseProduct.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseRef.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMap.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseColEtree.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSolverBase.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseRedux.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/CompressedStorage.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/TriangularSolver.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseView.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparsePermutation.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseTranspose.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/AmbiVector.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseUtil.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseMatrix.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseCore/SparseFuzzy.h` & `tomotopy-0.9.1/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `tomotopy-0.9.1/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/Determinant.h` & `tomotopy-0.9.1/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/InverseImpl.h` & `tomotopy-0.9.1/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/FullPivLU.h` & `tomotopy-0.9.1/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `tomotopy-0.9.1/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/PartialPivLU.h` & `tomotopy-0.9.1/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/LU/arch/Inverse_SSE.h` & `tomotopy-0.9.1/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/BlockMethods.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `tomotopy-0.9.1/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/MetisSupport/MetisSupport.h` & `tomotopy-0.9.1/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/src/SparseQR/SparseQR.h` & `tomotopy-0.9.1/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/UmfPackSupport` & `tomotopy-0.9.1/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/StdDeque` & `tomotopy-0.9.1/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/CMakeLists.txt` & `tomotopy-0.9.1/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SPQRSupport` & `tomotopy-0.9.1/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/QR` & `tomotopy-0.9.1/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/CholmodSupport` & `tomotopy-0.9.1/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SuperLUSupport` & `tomotopy-0.9.1/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Eigenvalues` & `tomotopy-0.9.1/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/StdVector` & `tomotopy-0.9.1/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Jacobi` & `tomotopy-0.9.1/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Geometry` & `tomotopy-0.9.1/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/PardisoSupport` & `tomotopy-0.9.1/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Core` & `tomotopy-0.9.1/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Householder` & `tomotopy-0.9.1/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/QtAlignedMalloc` & `tomotopy-0.9.1/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SparseLU` & `tomotopy-0.9.1/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SparseCore` & `tomotopy-0.9.1/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/IterativeLinearSolvers` & `tomotopy-0.9.1/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/LU` & `tomotopy-0.9.1/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/Sparse` & `tomotopy-0.9.1/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/MetisSupport` & `tomotopy-0.9.1/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/SparseQR` & `tomotopy-0.9.1/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/include/Eigen/StdList` & `tomotopy-0.9.1/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy.egg-info/SOURCES.txt` & `tomotopy-0.9.1/tomotopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy.egg-info/PKG-INFO` & `tomotopy-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tomotopy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tomoto, The Topic Modeling Tool for Python
 Home-page: https://github.com/bab2min/tomotopy
 Author: bab2min
 Author-email: bab2min@gmail.com
 License: MIT License
 Description: What is tomotopy?
         ------------------
@@ -22,15 +22,15 @@
         * Hierarchical LDA (`tomotopy.HLDAModel`)
         * Multi Grain LDA (`tomotopy.MGLDAModel`) 
         * Pachinko Allocation (`tomotopy.PAModel`)
         * Hierarchical PA (`tomotopy.HPAModel`)
         * Correlated Topic Model (`tomotopy.CTModel`)
         * Dynamic Topic Model (`tomotopy.DTModel`).
         
-        The most recent version of tomotopy is 0.9.0.
+        The most recent version of tomotopy is 0.9.1.
         
         .. image:: https://badge.fury.io/py/tomotopy.svg
         
         Getting Started
         ---------------
         You can install tomotopy easily using pip. (https://pypi.org/project/tomotopy/)
         ::
@@ -255,14 +255,18 @@
         License
         ---------
         `tomotopy` is licensed under the terms of MIT License, 
         meaning you can use it for any reasonable purpose and remain in complete ownership of all the documentation you produce.
         
         History
         -------
+        * 0.9.1 (2020-08-08)
+            * Memory leaks of version 0.9.0 was fixed.
+            * `tomotopy.CTModel.summary()` was fixed.
+        
         * 0.9.0 (2020-08-04)
             * The `tomotopy.LDAModel.summary()` method, which prints human-readable summary of the model, has been added.
             * The random number generator of package has been replaced with [EigenRand]. It speeds up the random number generation and solves the result difference between platforms.
             * Due to above, even if `seed` is the same, the model training result may be different from the version before 0.9.0.
             * Fixed a training error in `tomotopy.HDPModel`.
             * `tomotopy.DMRModel.alpha` now shows Dirichlet prior of per-document topic distribution by metadata.
             * `tomotopy.DTModel.get_count_by_topics()` has been modified to return a 2-dimensional `ndarray`.
```

### Comparing `tomotopy-0.9.0/tomotopy/__init__.py` & `tomotopy-0.9.1/tomotopy/__init__.py`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy/_summary.py` & `tomotopy-0.9.1/tomotopy/_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,14 @@
     import tomotopy as tp
     print('| tw: TermWeight.{}'.format(tp.TermWeight(v).name), file=file)
 
 def initial_params_info_version_LDAModel(mdl, v, file):
     import tomotopy as tp
     print('| trained in version {}'.format(v), file=file)
 
-
 def initial_params_info_vars_SLDAModel(mdl, v, file):
     import tomotopy as tp
     var_type = {'l':'linear', 'b':'binary'}
     print('| vars: {}'.format(', '.join(map(var_type.__getitem__, v))), file=file)
 
 def params_info_LDAModel(mdl, file):
     print('| alpha (Dirichlet prior on the per-document topic distributions)\n'
@@ -198,14 +197,22 @@
 
 def params_info_DTModel(mdl, file):
     print('| alpha (Dirichlet prior on the per-document topic distributions for each timepoint)\n'
         '|  {}'.format(_format_numpy(mdl.alpha, '|  ')), file=file)
     print('| phi (Dirichlet prior on the per-time&topic word distribution)\n'
         '|  ...', file=file)
 
+def params_info_CTModel(mdl, file):
+    print('| prior_mean (Prior mean of Logit-normal for the per-document topic distributions)\n'
+        '|  {}'.format(_format_numpy(mdl.prior_mean, '|  ')), file=file)
+    print('| prior_cov (Prior covariance of Logit-normal for the per-document topic distributions)\n'
+        '|  {}'.format(_format_numpy(mdl.prior_cov, '|  ')), file=file)
+    print('| eta (Dirichlet prior on the per-topic word distribution)\n'
+        '|  {:.5}'.format(mdl.eta), file=file)
+
 def topics_info_LDAModel(mdl, file, topic_word_top_n):
     topic_cnt = mdl.get_count_by_topics()
     for k in range(mdl.k):
         words = ' '.join(w for w, _ in mdl.get_topic_words(k, top_n=topic_word_top_n))
         print('| #{} ({}) : {}'.format(k, topic_cnt[k], words), file=file)
 
 def topics_info_HDPModel(mdl, file, topic_word_top_n):
```

### Comparing `tomotopy-0.9.0/tomotopy/label.py` & `tomotopy-0.9.1/tomotopy/label.py`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy/utils.py` & `tomotopy-0.9.1/tomotopy/utils.py`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy/auto_labeling_code_with_porter.rst` & `tomotopy-0.9.1/tomotopy/auto_labeling_code_with_porter.rst`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/tomotopy/documentation.rst` & `tomotopy-0.9.1/tomotopy/documentation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 * Hierarchical LDA (`tomotopy.HLDAModel`)
 * Multi Grain LDA (`tomotopy.MGLDAModel`) 
 * Pachinko Allocation (`tomotopy.PAModel`)
 * Hierarchical PA (`tomotopy.HPAModel`)
 * Correlated Topic Model (`tomotopy.CTModel`)
 * Dynamic Topic Model (`tomotopy.DTModel`).
 
-The most recent version of tomotopy is 0.9.0.
+The most recent version of tomotopy is 0.9.1.
 
 .. image:: https://badge.fury.io/py/tomotopy.svg
 
 Getting Started
 ---------------
 You can install tomotopy easily using pip. (https://pypi.org/project/tomotopy/)
 ::
@@ -293,14 +293,18 @@
 License
 ---------
 `tomotopy` is licensed under the terms of MIT License, 
 meaning you can use it for any reasonable purpose and remain in complete ownership of all the documentation you produce.
 
 History
 -------
+* 0.9.1 (2020-08-08)
+    * Memory leaks of version 0.9.0 was fixed.
+    * `tomotopy.CTModel.summary()` was fixed.
+
 * 0.9.0 (2020-08-04)
     * The `tomotopy.LDAModel.summary()` method, which prints human-readable summary of the model, has been added.
     * The random number generator of package has been replaced with [EigenRand]. It speeds up the random number generation and solves the result difference between platforms.
     * Due to above, even if `seed` is the same, the model training result may be different from the version before 0.9.0.
     * Fixed a training error in `tomotopy.HDPModel`.
     * `tomotopy.DMRModel.alpha` now shows Dirichlet prior of per-document topic distribution by metadata.
     * `tomotopy.DTModel.get_count_by_topics()` has been modified to return a 2-dimensional `ndarray`.
```

### Comparing `tomotopy-0.9.0/tomotopy/documentation.kr.rst` & `tomotopy-0.9.1/tomotopy/documentation.kr.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 * Hierarchical LDA (`tomotopy.HLDAModel`)
 * Multi Grain LDA (`tomotopy.MGLDAModel`) 
 * Pachinko Allocation (`tomotopy.PAModel`)
 * Hierarchical PA (`tomotopy.HPAModel`)
 * Correlated Topic Model (`tomotopy.CTModel`)
 * Dynamic Topic Model (`tomotopy.DTModel`)
 
-tomotopy의 가장 최신버전은 0.9.0 입니다.
+tomotopy의 가장 최신버전은 0.9.1 입니다.
 
 .. image:: https://badge.fury.io/py/tomotopy.svg
 
 시작하기
 ---------------
 다음과 같이 pip를 이용하면 tomotopy를 쉽게 설치할 수 있습니다. (https://pypi.org/project/tomotopy/)
 ::
@@ -290,14 +290,18 @@
 
 라이센스
 ---------
 `tomotopy`는 MIT License 하에 배포됩니다.
 
 역사
 -------
+* 0.9.1 (2020-08-08)
+    * 0.9.0 버전의 메모리 누수 문제가 해결되었습니다.
+    * `tomotopy.CTModel.summary()`가 잘못된 결과를 출력하는 문제가 해결되었습니다.
+
 * 0.9.0 (2020-08-04)
     * 모델의 상태를 알아보기 쉽게 출력해주는 `tomotopy.LDAModel.summary()` 메소드가 추가되었습니다.
     * 난수 생성기를 [EigenRand]로 대체하여 생성 속도를 높이고 플랫폼 간의 결과 차이를 해소하였습니다.
     * 이로 인해 `seed`가 동일해도 모델 학습 결과가 0.9.0 이전 버전과 달라질 수 있습니다.
     * `tomotopy.HDPModel`에서 간헐적으로 발생하는 학습 오류를 수정했습니다.
     * 이제 `tomotopy.DMRModel.alpha`가 메타데이터별 토픽 분포의 사전 파라미터를 보여줍니다.
     * `tomotopy.DTModel.get_count_by_topics()`가 2차원 `ndarray`를 반환하도록 수정되었습니다.
```

### Comparing `tomotopy-0.9.0/tomotopy/auto_labeling_code.rst` & `tomotopy-0.9.1/tomotopy/auto_labeling_code.rst`

 * *Files identical despite different names*

### Comparing `tomotopy-0.9.0/PKG-INFO` & `tomotopy-0.9.1/tomotopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tomotopy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tomoto, The Topic Modeling Tool for Python
 Home-page: https://github.com/bab2min/tomotopy
 Author: bab2min
 Author-email: bab2min@gmail.com
 License: MIT License
 Description: What is tomotopy?
         ------------------
@@ -22,15 +22,15 @@
         * Hierarchical LDA (`tomotopy.HLDAModel`)
         * Multi Grain LDA (`tomotopy.MGLDAModel`) 
         * Pachinko Allocation (`tomotopy.PAModel`)
         * Hierarchical PA (`tomotopy.HPAModel`)
         * Correlated Topic Model (`tomotopy.CTModel`)
         * Dynamic Topic Model (`tomotopy.DTModel`).
         
-        The most recent version of tomotopy is 0.9.0.
+        The most recent version of tomotopy is 0.9.1.
         
         .. image:: https://badge.fury.io/py/tomotopy.svg
         
         Getting Started
         ---------------
         You can install tomotopy easily using pip. (https://pypi.org/project/tomotopy/)
         ::
@@ -255,14 +255,18 @@
         License
         ---------
         `tomotopy` is licensed under the terms of MIT License, 
         meaning you can use it for any reasonable purpose and remain in complete ownership of all the documentation you produce.
         
         History
         -------
+        * 0.9.1 (2020-08-08)
+            * Memory leaks of version 0.9.0 was fixed.
+            * `tomotopy.CTModel.summary()` was fixed.
+        
         * 0.9.0 (2020-08-04)
             * The `tomotopy.LDAModel.summary()` method, which prints human-readable summary of the model, has been added.
             * The random number generator of package has been replaced with [EigenRand]. It speeds up the random number generation and solves the result difference between platforms.
             * Due to above, even if `seed` is the same, the model training result may be different from the version before 0.9.0.
             * Fixed a training error in `tomotopy.HDPModel`.
             * `tomotopy.DMRModel.alpha` now shows Dirichlet prior of per-document topic distribution by metadata.
             * `tomotopy.DTModel.get_count_by_topics()` has been modified to return a 2-dimensional `ndarray`.
```

