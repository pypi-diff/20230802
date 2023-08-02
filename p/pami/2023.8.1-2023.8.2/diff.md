# Comparing `tmp/pami-2023.8.1.tar.gz` & `tmp/pami-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.8.1.tar", last modified: Wed Aug  2 06:58:53 2023, max compression
+gzip compressed data, was "pami-2023.8.2.tar", last modified: Wed Aug  2 08:22:08 2023, max compression
```

## Comparing `pami-2023.8.1.tar` & `pami-2023.8.2.tar`

### file list

```diff
@@ -1,434 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.140717 pami-2023.8.1/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.1/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.947667 pami-2023.8.1/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.947872 pami-2023.8.1/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.953224 pami-2023.8.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.956819 pami-2023.8.1/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.963111 pami-2023.8.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/CoMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/CoMinePlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.963289 pami-2023.8.1/PAMI/coveragePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.967331 pami-2023.8.1/PAMI/coveragePattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/coveragePattern/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/coveragePattern/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.970185 pami-2023.8.1/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.977092 pami-2023.8.1/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4192 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.977517 pami-2023.8.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.988550 pami-2023.8.1/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15604 2023-08-01 14:39:54.000000 pami-2023.8.1/PAMI/extras/dbStats/sequencialDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.1/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9436 2023-08-02 06:55:18.000000 pami-2023.8.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.989307 pami-2023.8.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.990025 pami-2023.8.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.994239 pami-2023.8.1/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.1/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2423 2023-08-02 03:21:50.000000 pami-2023.8.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996127 pami-2023.8.1/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996407 pami-2023.8.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996830 pami-2023.8.1/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.998177 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.998347 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.004169 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13292 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21358 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.004349 pami-2023.8.1/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.012896 pami-2023.8.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13219 2023-07-29 17:09:30.000000 pami-2023.8.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12611 2023-07-29 17:09:30.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13190 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13538 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20301 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.017391 pami-2023.8.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.024507 pami-2023.8.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13299 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14252 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12925 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14001 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11538 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13872 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10731 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.025037 pami-2023.8.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25156 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.029527 pami-2023.8.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5605 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13545 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11987 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16531 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.030067 pami-2023.8.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.030218 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.034156 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25498 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.036077 pami-2023.8.1/PAMI/fuzzyFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.041173 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20910 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26294 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.043286 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.049189 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27153 2023-07-29 15:37:17.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.051688 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.055973 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.056128 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.059811 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23711 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.059980 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.060433 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.060599 pami-2023.8.1/PAMI/georeferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.064819 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.065093 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.065243 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.072557 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.074303 pami-2023.8.1/PAMI/highUtilityFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.077832 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.078033 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.082919 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.083136 pami-2023.8.1/PAMI/highUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.086752 pami-2023.8.1/PAMI/highUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.087258 pami-2023.8.1/PAMI/highUtilityPattern/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.087927 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.088201 pami-2023.8.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.091485 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.091930 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.092082 pami-2023.8.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.092857 pami-2023.8.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.093013 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.097974 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.100666 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.101348 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.101568 pami-2023.8.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.102717 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.103241 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.103778 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.104194 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.107777 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.107936 pami-2023.8.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.108391 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.108522 pami-2023.8.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.112061 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.112556 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.113178 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.113682 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.116176 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5378 2023-07-28 05:41:12.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24444 2023-07-28 13:21:57.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.117435 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.117885 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.118333 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.118569 pami-2023.8.1/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.119009 pami-2023.8.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.119204 pami-2023.8.1/PAMI/relativeFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.120652 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.120795 pami-2023.8.1/PAMI/relativeHighUtilityPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121180 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121312 pami-2023.8.1/PAMI/sequence/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequence/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121400 pami-2023.8.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121960 pami-2023.8.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.124101 pami-2023.8.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.124193 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.127151 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.127638 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.128066 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.128213 pami-2023.8.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.129688 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.129827 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.132365 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.132491 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.133627 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.134120 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.135105 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.135244 pami-2023.8.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.136755 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.137049 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.138189 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.138337 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.139683 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61264 2023-08-02 06:58:53.140553 pami-2023.8.1/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    60579 2023-08-02 03:21:50.000000 pami-2023.8.1/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.140287 pami-2023.8.1/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    61264 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15371 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-02 06:58:53.140760 pami-2023.8.1/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1401 2023-08-02 06:58:45.000000 pami-2023.8.1/setup.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.893487 pami-2023.8.2/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    35149 2023-08-02 08:17:35.000000 pami-2023.8.2/LICENSE
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/AssociationRules/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/AssociationRules/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13175 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    12870 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13078 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    12384 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6455 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      139 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/correlatedPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24834 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26312 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6065 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/coveragePattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/coveragePattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13863 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    15929 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7018 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/DF2DB/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2178 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2243 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1607 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4192 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4917 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     9942 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3607 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3359 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3741 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3794 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/dbStats/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13043 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    15604 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/sequencialDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    14610 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     9436 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13229 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    10040 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    11775 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5195 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5925 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5919 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5803 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.869486 pami-2023.8.2/PAMI/extras/generateDatabase/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2877 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7092 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3444 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3593 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/extras/graph/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1429 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2954 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1143 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1753 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2428 2023-08-02 08:19:10.000000 pami-2023.8.2/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/extras/image2Database/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/extras/imageProcessing/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4582 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/extras/neighbours/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2834 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2651 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3031 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     3214 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2178 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2332 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2297 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2555 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1887 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1860 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2126 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2079 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     2265 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1827 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      473 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13292 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21358 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6766 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13219 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    12611 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13190 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13538 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    20301 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7733 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/closed/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19938 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6445 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6564 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13299 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    14252 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    12925 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    14001 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    11538 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13872 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    10731 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25156 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6436 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5605 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    13545 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    11987 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    16531 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/frequentPattern/topk/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    14742 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4575 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.873487 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25498 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6635 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    20910 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26294 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6450 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24180 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27153 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6580 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27023 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    32449 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6618 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    23711 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26218 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6668 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19950 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6774 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    20059 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19117 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6680 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6676 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19894 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6165 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    35398 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6081 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    39928 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6181 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    32744 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24844 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26560 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5053 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    16478 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.877487 pami-2023.8.2/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5053 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    16480 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    29434 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    33678 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5195 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6718 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27644 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    34623 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5955 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    35216 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6625 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/localPeriodicPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    32664 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21999 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21120 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     8378 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    22994 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    22318 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5913 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27316 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21102 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5392 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    50844 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4195 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24330 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    17878 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5572 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21069 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5595 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    28482 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4261 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7837 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    17705 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26067 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5550 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.881487 pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27518 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6652 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    15591 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25146 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24942 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    16311 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    33244 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      726 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6525 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    21540 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6538 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6564 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19356 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    17474 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    28740 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7873 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5378 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    24444 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    18066 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6898 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4583 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    17235 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/recurringPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/recurringPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26300 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6632 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26215 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4261 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    33570 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7391 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/sequence/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/sequence/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/sequentialPatternMining/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:35.000000 pami-2023.8.2/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    41062 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6554 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    22592 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6279 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.885486 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    16326 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25134 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    17903 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7258 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26386 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7177 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    14997 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6766 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25974 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    26009 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    18710 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27060 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27823 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    25507 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    19046 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4962 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    28817 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     5005 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      727 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    31092 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    31324 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6551 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27481 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6693 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    23859 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     6737 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    27228 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     7555 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    29074 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     4782 2023-08-02 08:17:36.000000 pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    61263 2023-08-02 08:22:08.889486 pami-2023.8.2/PKG-INFO
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    60578 2023-08-02 08:17:36.000000 pami-2023.8.2/README.md
+drwxr-xr-x   0 nakamura  (1003) nakamura  (1003)        0 2023-08-02 08:22:08.889486 pami-2023.8.2/pami.egg-info/
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    61263 2023-08-02 08:22:08.000000 pami-2023.8.2/pami.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)    15371 2023-08-02 08:22:08.000000 pami-2023.8.2/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        1 2023-08-02 08:22:08.000000 pami-2023.8.2/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)      189 2023-08-02 08:22:08.000000 pami-2023.8.2/pami.egg-info/requires.txt
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)        5 2023-08-02 08:22:08.000000 pami-2023.8.2/pami.egg-info/top_level.txt
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)       38 2023-08-02 08:22:08.893487 pami-2023.8.2/setup.cfg
+-rw-r--r--   0 nakamura  (1003) nakamura  (1003)     1402 2023-08-02 08:21:24.000000 pami-2023.8.2/setup.py
```

### Comparing `pami-2023.8.1/LICENSE` & `pami-2023.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.8.2/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.8.2/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.8.2/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.8.2/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.8.2/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/correlatedPattern/__init__.py` & `pami-2023.8.2/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/correlatedPattern/basic/CoMine.py` & `pami-2023.8.2/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/correlatedPattern/basic/CoMinePlus.py` & `pami-2023.8.2/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.8.2/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/coveragePattern/basic/CMine.py` & `pami-2023.8.2/PAMI/coveragePattern/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/coveragePattern/basic/CPPG.py` & `pami-2023.8.2/PAMI/coveragePattern/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/coveragePattern/basic/abstract.py` & `pami-2023.8.2/PAMI/coveragePattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.8.2/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.8.2/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.8.2/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.8.2/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.8.2/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.8.2/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.8.2/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.8.2/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/sequencialDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/sequencialDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.8.2/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.8.2/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.8.2/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.8.2/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.8.2/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.8.2/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.8.2/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.8.2/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.8.2/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.8.2/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.8.2/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.8.2/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.8.2/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.8.2/PAMI/extras/graph/visualizePatterns.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             GHex = hex(G)[2:]
             BHex = hex(B)[2:]
 
             line = line.split(":")
             freq = line[-1]
             freq = "Frequency: " + freq.strip()
             line = line[:-1]
-            print(start + "\t" + line[0])
+            print(str(start) + "\t" + line[0])
             points = line[0].split("\t")
             points = [x for x in points if x != ""]
             points = [x.strip("Point()") for x in points]
             for i in range(len(points)):
                 temp = points[i].split()
                 lat.append(float(temp[0]))
                 long.append(float(temp[1]))
```

### Comparing `pami-2023.8.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.8.2/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.8.2/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py` & `pami-2023.8.2/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/plotPointOnMap.py` & `pami-2023.8.2/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.8.2/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.8.2/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.8.2/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/extras/topKPatterns.py` & `pami-2023.8.2/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/__init__.py` & `pami-2023.8.2/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.8.2/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.8.2/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.8.2/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.8.2/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.8.2/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.8.2/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.8.2/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py` & `pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py` & `pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py` & `pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py` & `pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.8.2/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py` & `pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py` & `pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py` & `pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/basic/EFIM.py` & `pami-2023.8.2/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/basic/HMiner.py` & `pami-2023.8.2/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/basic/UPGrowth.py` & `pami-2023.8.2/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/basic/efimParallel.py` & `pami-2023.8.2/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/parallel/abstract.py` & `pami-2023.8.2/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPattern/parallel/efimparallel.py` & `pami-2023.8.2/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/HUPMS.py` & `pami-2023.8.2/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py` & `pami-2023.8.2/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/abstract.py` & `pami-2023.8.2/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.8.2/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.8.2/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.8.2/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py` & `pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py` & `pami-2023.8.2/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.8.2/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.8.2/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py` & `pami-2023.8.2/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/relativeFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py` & `pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.8.2/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.8.2/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.8.2/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.8.2/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.8.2/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py` & `pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py` & `pami-2023.8.2/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py` & `pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.8.2/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.2/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/PKG-INFO` & `pami-2023.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: gpu
 Provides-Extra: spark
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 [![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
@@ -88,15 +88,15 @@
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
 ### 1. Mining interesting patterns from transactional databases
-1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
+1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
 | FP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/FPGrowth.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>           |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 | ECLAT  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLAT.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>                 |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelECLAT.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>       |
 | ECLAT-bitSet <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLATbitset.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                                     |
```

### Comparing `pami-2023.8.1/README.md` & `pami-2023.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
 ### 1. Mining interesting patterns from transactional databases
-1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
+1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
 | FP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/FPGrowth.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>           |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 | ECLAT  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLAT.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>                 |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelECLAT.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>       |
 | ECLAT-bitSet <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLATbitset.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                                     |
```

### Comparing `pami-2023.8.1/pami.egg-info/PKG-INFO` & `pami-2023.8.2/pami.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayLab/PAMI
 Author: Rage Uday Kiran
 Author-email: uday.rage@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: gpu
 Provides-Extra: spark
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
 [![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 [![Documentation Status](https://readthedocs.org/projects/pami-1/badge/?version=latest)](https://pami-1.readthedocs.io/en/latest/?badge=latest)
@@ -88,15 +88,15 @@
   Uninstallation
   
        pip uninstall pami 
        
 # Tutorials 
 
 ### 1. Mining interesting patterns from transactional databases
-1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
+1. Frequent pattern mining: [Sample](https://udaylab.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                      | Closed                                                                                                                                                                                                                                       | Maximal                                                                                                                                                                                                                                                     | Top-k                                                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                                             |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Apriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/Apriori.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>              | CHARM <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/closed/CHARM.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | maxFP-growth  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/maximal/MaxFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | FAE <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/topk/FAE.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> | cudaAprioriGCT | parallelApriori <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelApriori.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |
 | FP-growth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/FPGrowth.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>           |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelFPGrowth.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a> |
 | ECLAT  <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLAT.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>                 |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/pyspark/parallelECLAT.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>       |
 | ECLAT-bitSet <a target="_blank" href="https://colab.research.google.com/github/UdayLab/PAMI/blob/main/notebooks/frequentPattern/basic/ECLATbitset.ipynb"> <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> </a>   |                                                                                                                                                                                                                                              |                                                                                                                                                                                                                                                             |                                                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                                     |
```

### Comparing `pami-2023.8.1/pami.egg-info/SOURCES.txt` & `pami-2023.8.2/pami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pami-2023.8.1/setup.py` & `pami-2023.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pami',
-    version='2023.08.1',
+    version='2023.08.02',
     author='Rage Uday Kiran',
     author_email='uday.rage@gmail.com',
     description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
     url='https://github.com/udayLab/PAMI',
```

