# Comparing `tmp/pami-2023.7.7.tar.gz` & `tmp/pami-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.7.7.tar", last modified: Tue Jul 18 12:23:34 2023, max compression
+gzip compressed data, was "pami-2023.8.1.tar", last modified: Wed Aug  2 06:58:53 2023, max compression
```

## Comparing `pami-2023.7.7.tar` & `pami-2023.8.1.tar`

### file list

```diff
@@ -1,434 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.306139 pami-2023.7.7/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.7/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213420 pami-2023.7.7/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213780 pami-2023.7.7/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215229 pami-2023.7.7/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215381 pami-2023.7.7/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.216924 pami-2023.7.7/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.217089 pami-2023.7.7/PAMI/coveragePatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.218352 pami-2023.7.7/PAMI/coveragePatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.219319 pami-2023.7.7/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221044 pami-2023.7.7/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221516 pami-2023.7.7/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.223716 pami-2023.7.7/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.225281 pami-2023.7.7/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.227961 pami-2023.7.7/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231441 pami-2023.7.7/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231576 pami-2023.7.7/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231920 pami-2023.7.7/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.232234 pami-2023.7.7/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233791 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2280 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2257 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2509 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2124 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2075 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233937 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235273 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235589 pami-2023.7.7/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.237534 pami-2023.7.7/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.238433 pami-2023.7.7/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.240335 pami-2023.7.7/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.241160 pami-2023.7.7/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.242453 pami-2023.7.7/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243543 pami-2023.7.7/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243784 pami-2023.7.7/PAMI/frequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.244809 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245067 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245890 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.246160 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247438 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247699 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.248928 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249301 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249802 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.250466 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251507 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251792 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.252874 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.254340 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255007 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255910 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256357 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256630 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257531 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257812 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261273 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261803 pami-2023.7.7/PAMI/highUtilityPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.264098 pami-2023.7.7/PAMI/highUtilityPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265044 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16481 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265480 pami-2023.7.7/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.266895 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267687 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267930 pami-2023.7.7/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269128 pami-2023.7.7/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269369 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270382 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270633 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271619 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271849 pami-2023.7.7/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.273903 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.274936 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.275960 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.276849 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277438 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277755 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278324 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278541 pami-2023.7.7/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279293 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279512 pami-2023.7.7/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.281487 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.282417 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.283856 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19727 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.284826 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285069 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285761 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286394 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286673 pami-2023.7.7/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287396 pami-2023.7.7/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287636 pami-2023.7.7/PAMI/relativeFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288407 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288643 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289267 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289510 pami-2023.7.7/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.290707 pami-2023.7.7/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291328 pami-2023.7.7/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291420 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.292688 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293628 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293913 pami-2023.7.7/PAMI/streams/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294014 pami-2023.7.7/PAMI/streams/frequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294626 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31851 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7792 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295292 pami-2023.7.7/PAMI/streams/highUtility/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295424 pami-2023.7.7/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298349 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298597 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.299797 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300033 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300646 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300913 pami-2023.7.7/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.301700 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302005 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302627 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.303017 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.304367 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.305978 pami-2023.7.7/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34480 2023-07-07 08:24:43.000000 pami-2023.7.7/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.305715 pami-2023.7.7/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15099 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      102 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-18 12:23:34.306190 pami-2023.7.7/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1289 2023-07-18 12:22:32.000000 pami-2023.7.7/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.140717 pami-2023.8.1/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-07-24 10:04:09.000000 pami-2023.8.1/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.947667 pami-2023.8.1/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.947872 pami-2023.8.1/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.953224 pami-2023.8.1/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13175 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12870 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13078 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6455 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.956819 pami-2023.8.1/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.963111 pami-2023.8.1/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24834 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/CoMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26312 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/CoMinePlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6065 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.963289 pami-2023.8.1/PAMI/coveragePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.967331 pami-2023.8.1/PAMI/coveragePattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13863 2023-07-25 12:32:03.000000 pami-2023.8.1/PAMI/coveragePattern/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15929 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/coveragePattern/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7018 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/coveragePattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.970185 pami-2023.8.1/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.977092 pami-2023.8.1/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4192 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.977517 pami-2023.8.1/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.988550 pami-2023.8.1/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15604 2023-08-01 14:39:54.000000 pami-2023.8.1/PAMI/extras/dbStats/sequencialDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14610 2023-07-30 05:40:09.000000 pami-2023.8.1/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9436 2023-08-02 06:55:18.000000 pami-2023.8.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.989307 pami-2023.8.1/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.990025 pami-2023.8.1/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.994239 pami-2023.8.1/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1429 2023-07-28 06:47:15.000000 pami-2023.8.1/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1143 2023-08-02 06:55:18.000000 pami-2023.8.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2423 2023-08-02 03:21:50.000000 pami-2023.8.1/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996127 pami-2023.8.1/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996407 pami-2023.8.1/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.996830 pami-2023.8.1/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2651 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.998177 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2332 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2297 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2555 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2126 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2079 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:52.998347 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.004169 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13292 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21358 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.004349 pami-2023.8.1/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.012896 pami-2023.8.1/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13219 2023-07-29 17:09:30.000000 pami-2023.8.1/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12611 2023-07-29 17:09:30.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13190 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13538 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20301 2023-07-26 05:11:46.000000 pami-2023.8.1/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.017391 pami-2023.8.1/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19938 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.024507 pami-2023.8.1/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13299 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14252 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12925 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14001 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11538 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13872 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10731 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.025037 pami-2023.8.1/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25156 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.029527 pami-2023.8.1/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5605 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13545 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11987 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16531 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.030067 pami-2023.8.1/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14742 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.030218 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.034156 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25498 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.036077 pami-2023.8.1/PAMI/fuzzyFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.041173 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20910 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26294 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.043286 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.049189 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24180 2023-07-29 15:37:17.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27153 2023-07-29 15:37:17.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.051688 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.055973 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27023 2023-07-29 15:44:25.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32449 2023-07-29 15:44:25.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.056128 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.059811 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23711 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26218 2023-07-28 04:20:39.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.059980 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.060433 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.060599 pami-2023.8.1/PAMI/georeferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.064819 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20059 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19117 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.065093 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.065243 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.072557 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19894 2023-07-29 16:51:12.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.074303 pami-2023.8.1/PAMI/highUtilityFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.077832 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35398 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.078033 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.082919 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39928 2023-07-29 16:07:24.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.083136 pami-2023.8.1/PAMI/highUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.086752 pami-2023.8.1/PAMI/highUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32744 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24844 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26560 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16478 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.087258 pami-2023.8.1/PAMI/highUtilityPattern/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16480 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPattern/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.087927 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilityPatternsInStreams/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.088201 pami-2023.8.1/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.091485 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27644 2023-07-29 16:07:24.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.091930 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.092082 pami-2023.8.1/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.092857 pami-2023.8.1/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.093013 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.097974 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22994 2023-07-29 11:47:49.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.100666 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.101348 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.101568 pami-2023.8.1/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.102717 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.103241 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.103778 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.104194 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.107777 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26067 2023-07-29 16:46:35.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.107936 pami-2023.8.1/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.108391 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.108522 pami-2023.8.1/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.112061 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.112556 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.113178 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19356 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.113682 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.116176 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-28 05:36:37.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5378 2023-07-28 05:41:12.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24444 2023-07-28 13:21:57.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.117435 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.117885 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.118333 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.118569 pami-2023.8.1/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.119009 pami-2023.8.1/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.119204 pami-2023.8.1/PAMI/relativeFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.120652 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26215 2023-08-01 01:42:22.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.120795 pami-2023.8.1/PAMI/relativeHighUtilityPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121180 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33570 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121312 pami-2023.8.1/PAMI/sequence/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequence/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121400 pami-2023.8.1/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.121960 pami-2023.8.1/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.124101 pami-2023.8.1/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.124193 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.127151 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16326 2023-07-29 11:25:56.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25134 2023-07-29 11:57:55.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17903 2023-07-29 11:57:55.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.127638 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.128066 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14997 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6766 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.128213 pami-2023.8.1/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.129688 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.129827 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.132365 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28817 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5005 2023-07-25 07:30:57.000000 pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.132491 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.133627 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31092 2023-07-29 11:28:40.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31324 2023-07-29 11:28:40.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.134120 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.135105 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.135244 pami-2023.8.1/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.136755 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23859 2023-07-29 11:29:36.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.137049 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.138189 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.138337 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.139683 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29074 2023-07-29 11:29:37.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-07-24 10:04:09.000000 pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61264 2023-08-02 06:58:53.140553 pami-2023.8.1/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    60579 2023-08-02 03:21:50.000000 pami-2023.8.1/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-08-02 06:58:53.140287 pami-2023.8.1/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    61264 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15371 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      189 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-08-02 06:58:52.000000 pami-2023.8.1/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-08-02 06:58:53.140760 pami-2023.8.1/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1401 2023-08-02 06:58:45.000000 pami-2023.8.1/setup.py
```

### Comparing `pami-2023.7.7/LICENSE` & `pami-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.8.1/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,130 @@
 from PAMI.AssociationRules.basic import abstract as _ab
 
-
+class Confidence:
+    
+    def __init__(self, patterns, singleItems, threshold):
+        """
+        :param inputFile: input file name or path
+        :type inputFile: str
+        :param sep:
+        """
+        self._frequentPatterns = patterns
+        self._singleItems = singleItems
+        self._threshold = threshold
+        self._finalPatterns = {}
+        
+    def _generation(self, prefix, suffix):
+        if len(suffix) == 1:
+            conf = self._generaeWithConfidence(prefix, suffix[0])
+        for i in range(len(suffix)):
+            suffix1 = suffix[:i] + suffix[i+1:]
+            prefix1 = prefix + ' ' + suffix[i]
+            for j in range(i+1, len(suffix)):
+                self._generaeWithConfidence(prefix + ' ' + suffix[i], suffix[j])
+                #self._generation(prefix+ ' ' +suffix[i], suffix[i+1:]) 
+            self._generation(prefix1, suffix1)
+            
+    def _generaeWithConfidence(self, lhs, rhs):
+        s = lhs + '\t' + rhs
+        if self._frequentPatterns.get(s) == None:
+            return 0
+        minimum = self._frequentPatterns[s]
+        conflhs = minimum / self._frequentPatterns[lhs]
+        confrhs = minimum / self._frequentPatterns[rhs]
+        if conflhs >= self._threshold:
+            s1 = lhs + '->' + rhs
+            self._finalPatterns[s1] = conflhs
+        if confrhs >= self._threshold:
+            s1 = rhs + '->' + lhs
+            self._finalPatterns[s1] = confrhs
+            
+    def run(self):
+        for i in range(len(self._singleItems)):
+            suffix = self._singleItems[:i] + self._singleItems[i+1:]
+            prefix = self._singleItems[i]
+            for j in range(i+1, len(self._singleItems)):
+                self._generaeWithConfidence(self._singleItems[i], self._singleItems[j])
+            self._generation(prefix, suffix)
+    
+    
+    
+class Lift:
+    
+    def __init__(self, patterns, singleItems, threshold):
+        """
+        :param inputFile: input file name or path
+        :type inputFile: str
+        :param sep:
+        """
+        self._frequentPatterns = patterns
+        self._singleItems = singleItems
+        self._threshold = threshold
+        self._finalPatterns = {}
+        
+    def _generation(self, prefix, suffix):
+        if len(suffix) == 1:
+            self._generateWithLift(prefix, suffix[0])
+        for i in range(len(suffix)):
+            suffix1 = suffix[:i] + suffix[i+1:]
+            prefix1 = prefix + ' ' + suffix[i]
+            for j in range(i+1, len(suffix)):
+                self._generateWithLift(prefix + ' ' + suffix[i], suffix[j])
+                #self._generation(prefix+ ' ' +suffix[i], suffix[i+1:]) 
+            self._generation(prefix1, suffix1)
+            
+    def _generateWithLift(self, lhs, rhs):
+        s = lhs + '\t' + rhs
+        if self._frequentPatterns.get(s) == None:
+            return 0
+        minimum = self._frequentPatterns[s]
+        conflhs = minimum / self._frequentPatterns[lhs]
+        confrhs = minimum / self._frequentPatterns[rhs]
+        liftlhs = conflhs / self._frequentPatterns[rhs] * self._frequentPatterns[lhs]
+        rightrhs = confrhs / self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
+        if liftlhs >= self._threshold:
+            s1 = lhs + '->' + rhs
+            self._finalPatterns[s1] = conflhs
+        if rightrhs >= self._threshold:
+            s1 = rhs + '->' + lhs
+            self._finalPatterns[s1] = confrhs
+            
+    def run(self):
+        for i in range(len(self._singleItems)):
+            suffix = self._singleItems[:i] + self._singleItems[i+1:]
+            prefix = self._singleItems[i]
+            for j in range(i+1, len(self._singleItems)):
+                self._generateWithLift(self._singleItems[i], self._singleItems[j])
+            self._generation(prefix, suffix)
+    
+    
+    
 class Leverage:
-
+    
     def __init__(self, patterns, singleItems, threshold):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._frequentPatterns = patterns
         self._singleItems = singleItems
         self._threshold = threshold
         self._finalPatterns = {}
-
+        
     def _generation(self, prefix, suffix):
         if len(suffix) == 1:
             conf = self._generateWithLeverage(prefix, suffix[0])
         for i in range(len(suffix)):
-            suffix1 = suffix[:i] + suffix[i + 1:]
+            suffix1 = suffix[:i] + suffix[i+1:]
             prefix1 = prefix + ' ' + suffix[i]
-            for j in range(i + 1, len(suffix)):
+            for j in range(i+1, len(suffix)):
                 self._generateWithLeverage(prefix + ' ' + suffix[i], suffix[j])
             self._generation(prefix1, suffix1)
-
+            
     def _generateWithLeverage(self, lhs, rhs):
         s = lhs + '\t' + rhs
         if self._frequentPatterns.get(s) == None:
             return 0
         minimum = self._frequentPatterns[s]
         conflhs = minimum / self._frequentPatterns[lhs]
         confrhs = minimum / self._frequentPatterns[rhs]
@@ -35,53 +132,51 @@
         rightrhs = confrhs - self._frequentPatterns[lhs] * self._frequentPatterns[rhs]
         if liftlhs >= self._threshold:
             s1 = lhs + '->' + rhs
             self._finalPatterns[s1] = conflhs
         if rightrhs >= self._threshold:
             s1 = rhs + '->' + lhs
             self._finalPatterns[s1] = confrhs
-
+            
     def run(self):
         for i in range(len(self._singleItems)):
-            suffix = self._singleItems[:i] + self._singleItems[i + 1:]
+            suffix = self._singleItems[:i] + self._singleItems[i+1:]
             prefix = self._singleItems[i]
-            for j in range(i + 1, len(self._singleItems)):
+            for j in range(i+1, len(self._singleItems)):
                 conf = self._generateWithLeverage(self._singleItems[i], self._singleItems[j])
             self._generation(prefix, suffix)
 
-
-class ARWithLeverage:
+class RuleMiner:
     """
-        Association Rules.
-
-
+    temporalDatabaseStats is class to get stats of database.
         Attributes:
         ----------
         frequentPattern : list or dict
             list
         measure: condition to calculate the strength of rule
             str
         threshold: condition to satisfy
             int
         Methods:
         -------
         startMine()
     """
 
-    def __init__(self, iFile, threshold, sep):
+    def __init__(self, iFile, measure, threshold, sep):
         """
         :param inputFile: input file name or path
         :type inputFile: str
         :param sep:
         """
         self._iFile = iFile
+        self._measure = measure
         self._threshold = threshold
         self._finalPatterns = {}
         self._sep = sep
-
+    
     def _readPatterns(self):
         self._frequentPatterns = {}
         k = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             pattern, sup = [], []
             if self._iFile.empty:
                 print("its empty..")
@@ -118,25 +213,34 @@
                     print("File Not Found")
                     quit()
         return k
 
     def startMine(self):
         self._startTime = _ab._time.time()
         k = self._readPatterns()
-        a = Leverage(self._frequentPatterns, k, self._threshold)
-        a.run()
-        self._finalPatterns = a._finalPatterns
+        if self._measure == 'confidence':
+            a = Confidence(self._frequentPatterns, k, self._threshold)
+            a.run()
+            self._finalPatterns = a._finalPatterns
+        if self._measure == 'lift':
+            a = Lift(self._frequentPatterns, k, self._threshold)
+            a.run()
+            self._finalPatterns = a._finalPatterns
+        if self._measure == 'leverage':
+            a = Leverage(self._frequentPatterns, k, self._threshold)
+            a.run()
+            self._finalPatterns = a._finalPatterns
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Association rules successfully  generated from frequent patterns ")
-
+    
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
@@ -194,26 +298,24 @@
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
+        if len(_ab._sys.argv) == 6:
+            _ap = RuleMiner(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = ARWithLeverage(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
-        if len(_ab._sys.argv) == 4:
-            _ap = ARWithLeverage(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = RuleMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         print("Total number of Association Rules:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = ARWithLeverage('patterns.txt', 0.8, '\t')
+        _ap = RuleMiner('sensorOutput.txt', "lift", 0.5, '\t')
         _ap.startMine()
         _ap.save('output.txt')
         _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
```

### Comparing `pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
@@ -38,21 +37,21 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _AssociationRules(_ABC):
+class _fuzzyFrequentPattenrs(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-       Attributes:
-       ----------
+    Attributes :
+    ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -68,16 +67,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+    Methods :
+    -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -87,36 +86,36 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, threshold, sep="\t"):
+    def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
-        self._threshold = threshold
-        self._finalPatterns = {}
-        self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+        self._minSup = minSup
         self._startTime = float()
         self._endTime = float()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        self._oFile = str()
+        self._finalPatterns = {}
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -150,18 +149,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-        pass
+
 
     @_abstractmethod
     def printResults(self):
-        """ To print result of the execution"""
+        """ To print all the results of execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.7/PAMI/correlatedPattern/__init__.py` & `pami-2023.8.1/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py` & `pami-2023.8.1/PAMI/relativeFrequentPattern/basic/RSFPGrowth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,37 @@
-# CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database.
-#
+
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#             from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
+#     from PAMI.relativeFrequentPattern import RSFPGrowth as alg
 #
-#             obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
+#     obj = alg.RSFPGrowth(iFile, minSup, __minRatio)
 #
-#             obj.startMine()
+#     obj.startMine()
 #
-#             Rules = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#             print("Total number of  Patterns:", len(Patterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#             obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
-#             Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#             memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getmemoryUSS()
 #
-#             print("Total Memory in USS:", memUSS)
+#     print("Total Memory in USS:", memUSS)
 #
-#             memRSS = obj.getMemoryRSS()
+#     memRSS = obj.getMemoryRSS()
 #
-#             print("Total Memory in RSS", memRSS)
+#     print("Total Memory in RSS", memRSS)
 #
-#             run = obj.getRuntime()
+#     run = obj.getRuntime()
 #
-#             print("Total ExecutionTime in seconds:", run)
-
-
-
+#     print("Total ExecutionTime in seconds:", run)
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -49,72 +45,79 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.correlatedPattern.basic import abstract as _ab
+from PAMI.relativeFrequentPattern.basic import abstract as _ab
+
 
 class _Node:
     """
-    A class used to represent the node of frequentPatternTree
-
+        A class used to represent the node of frequentPatterntree
 
-    Attributes :
+    Attributes:
     ----------
-        itemId : int
+        itemId: int
             storing item of a node
-        counter : int
+        counter: int
             To maintain the support of node
-        parent : node
+        parent: node
             To maintain the parent of every node
-        child : list
+        child: list
             To maintain the children of node
         nodeLink : node
             Points to the node with same itemId
 
-    Methods :
+    Methods:
     -------
 
         getChild(itemName)
-            returns the node with same itemName from frequentPatternTree
+            returns the node with same itemName from frequentPatterntree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
         self.nodeLink = None
 
-    def getChild(self, id1):
+    def getChild(self, itemName):
+        """ Retrieving the child from the tree
+
+            :param itemName: name of the child
+            :type itemName: list
+            :return: returns the node with same itemName from frequentPatternTree
+            :rtype: None or Node
+
+        """
         for i in self.child:
-            if i.itemId == id1:
+            if i.itemId == itemName:
                 return i
         return None
 
 
 class _Tree:
     """
         A class used to represent the frequentPatternGrowth tree structure
 
-    Attributes :
+    Attributes:
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
         mapItemLastNodes : dictionary
             representing the map that indicates the last node for each item
         root : Node
             representing the root Node in a tree
 
-
-    Methods :
+    Methods:
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
             creating transaction as a branch in frequentPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
@@ -127,150 +130,144 @@
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
-        """
-        adding transaction into tree
+        """adding transaction into tree
 
-        :param transaction : it represents the one transactions in database
-        :type transaction : list
+        :param transaction: it represents the one transactions in database
+        :type transaction: list
         """
 
+        # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
-            if child is None:
+            if not child:
                 newNode = _Node()
                 newNode.itemId = i
                 newNode.parent = current
                 current.child.append(newNode)
                 self.fixNodeLinks(i, newNode)
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
-        """
-        Fixing node link for the newNode that inserted into frequentPatternTree
+        """Fixing node link for the newNode that inserted into frequentPatternTree
 
         :param item: it represents the item of newNode
-        :type item : int
-        :param newNode : it represents the newNode that inserted in frequentPatternTree
-        :type newNode : Node
+        :type item: int
+        :param newNode: it represents the newNode that inserted in frequentPatternTree
+        :type newNode: Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
-        """
-        This method is to find the details of parent,children,support of Node
+        """Print the details of Node in frequentPatternTree
 
         :param root: it represents the Node in frequentPatternTree
         :type root: Node
 
-        
         """
 
-        if root.child is None:
+        # this method is used print the details of tree
+        if not root.child:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
-    def createHeaderList(self, mapSupport, minSup):
-        """
-        To create the headerList
+    def createHeaderList(self, __mapSupport, minSup):
+        """To create the headerList
 
-        :param mapSupport : it represents the items with their supports
-        :type mapSupport : dictionary
-        :param minSup : it represents the minSup
-        :param minSup : float
+        :param __mapSupport: it represents the items with their supports
+        :type __mapSupport: dictionary
+        :param minSup: it represents the minSup
+        :param minSup: float
         """
-        
+        # the frequentPatternTree always maintains the header table to start the mining from leaf nodes
         t1 = []
-        for x, y in mapSupport.items():
+        for x, y in __mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.headerList = [i for i in t1 if i in itemSetBuffer]
+        __itemSetBuffer = [k for k, v in sorted(__mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.headerList = [i for i in t1 if i in __itemSetBuffer]
 
-    def addPrefixPath(self, prefix, mapSupportBeta, minSup):
-        """
-        To construct the conditional tree with prefix paths of a node in frequentPatternTree
+    def addPrefixPath(self, prefix, __mapSupportBeta, minSup):
+        """To construct the conditional tree with prefix paths of a node in frequentPatternTree
 
-        :param prefix : it represents the prefix items of a Node
-        :type prefix : list
-        :param mapSupportBeta : it represents the items with their supports
-        :param mapSupportBeta : dictionary
-        :param minSup : to check the item meets with minSup
-        :param minSup : float
+        :param prefix: it represents the prefix items of a Node
+        :type prefix: list
+        :param __mapSupportBeta: it represents the items with their supports
+        :param __mapSupportBeta: dictionary
+        :param minSup: to check the item meets with minSup
+        :param minSup: float
         """
+        # this method is used to add prefix paths in conditional trees of frequentPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
-            if mapSupportBeta.get(pathItem.itemId) >= minSup:
+            if __mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
-                if child is None:
+                if not child:
                     newNode = _Node()
                     newNode.itemId = pathItem.itemId
                     newNode.parent = current
                     newNode.counter = pathCount
                     current.child.append(newNode)
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CPGrowth(_ab._correlatedPatterns):
+class RSFPGrowth(_ab._frequentPatterns):
     """
-    :Description: CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database. It is based on the traditional Fpgrowth Algorithm, this algorithm uses breadth-first search technique to find the correlated Frequent patterns in transactional database.
-
-    :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  minSup: int or float or str :
-                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-    :param minAllConf: str : Name of Neighbourhood file name
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
+    Description:
+    -------------
 
+        Algorithm to find all items with relative support from given dataset
 
-
-    :Attributes:
-
+    Reference:
+    -----------
+        'Towards Efficient Discovery of Frequent Patterns with Relative Support' R. Uday Kiran and
+               Masaru Kitsuregawa, http://comad.in/comad2012/pdf/kiran.pdf
+
+    Attributes:
+    -------------
+        iFile : file
+            Name of the Input file to mine complete set of frequent patterns
+        oFile : file
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
-        minSup : int
+        minSup : float
             The user given minSup
-        minAllConf: float
-            The user given minimum all confidence Ratio(should be in range of 0 to 1)
+        minRS : float
+            The user given minRS
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
             it represents the total no of transactions
         tree : class
@@ -280,400 +277,433 @@
         finalPatterns : dict
             it represents to store the patterns
         itemSetBuffer : list
             it represents the store the items in mining
         maxPatternLength : int
            it represents the constraint for pattern length
 
+    Methods:
+    --------
+        startMine()
+            Mining process will start from here
+        getFrequentPatterns()
+            Complete set of patterns will be retrieved with this function
+        save(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getmemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        check(line)
+            To check the delimiter used in the user input file
+        creatingItemSets(fileName)
+            Scans the dataset or dataframes and stores in list format
+        frequentOneItem()
+            Extracts the one-frequent patterns from transactions
+        saveAllCombination(tempBuffer,s,position,prefix,prefixLength)
+            Forms all the combinations between prefix and tempBuffer lists with support(s)
+        saveItemSet(pattern,support)
+            Stores all the frequent patterns with their respective support
+        frequentPatternGrowthGenerate(frequentPatternTree,prefix,port)
+            Mining the frequent patterns by forming conditional frequentPatternTrees to particular prefix item.
+            __mapSupport represents the 1-length items with their respective support
+
 
     **Methods to execute code on terminal**
-    ----------------------------------------
 
             Format:
-                      >>> python3 CSPGrowth.py <inputFile> <outputFile> <neighbourFile> <minSup> <minAllConf> <sep>
+                      >>>  python3 RSFPGrowth.py <inputFile> <outputFile> <minSup> <__minRatio>
             Example:
-                      >>>  python3 CSPGrowth.py sampleTDB.txt output.txt sampleN.txt 0.25 0.2
+                      >>>  python3 RSFPGrowth.py sampleDB.txt patterns.txt 0.23 0.2
+
+            .. note:: maxPer and minPS will be considered in percentage of database transactions
 
-                     .. note:: minSup will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
-    --------------------------------------------------------------------------------
+
     .. code-block:: python
 
-            from PAMI.correlatedSpatialPattern.basic import CSPGrowth as alg
+            from PAMI.relativeFrequentPattern import RSFPGrowth as alg
 
-            obj = alg.CSPGrowth(iFile, frequentPatternsFile, measure, threshold)
+            obj = alg.RSFPGrowth(iFile, minSup, __minRatio)
 
             obj.startMine()
 
-            Rules = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-            print("Total number of  Patterns:", len(Patterns))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.savePatterns(oFile)
+            obj.save(oFile)
 
             Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+            memUSS = obj.getmemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
-    ----------------------------------------
-             The complete program was written by B.Sai Chitra under the supervision of Professor Rage Uday Kiran.
+
+             The complete program was written by   Sai Chitra.B   under the supervision of Professor Rage Uday Kiran.
 
         """
 
-    _startTime = float()
-    _endTime = float()
-    _minSup = float()
-    _finalPatterns = {}
+    __startTime = float()
+    __endTime = float()
+    _minSup = str()
+    _minRS = float()
+    __finalPatterns = {}
     _iFile = " "
     _oFile = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _minAllConf = 0.0
-    _Database = []
-    _mapSupport = {}
-    _lno = 0
-    _tree = str()
-    _itemSetBuffer = None
-    _fpNodeTempBuffer = []
-    _itemSetCount = 0
-    _maxPatternLength = 1000
-    _sep = "\t"
-
-    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
-        super().__init__(iFile, minSup, minAllConf, sep)
+    _sep = " "
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __mapSupport = {}
+    __lno = 0
+    __tree = _Tree()
+    __itemSetBuffer = None
+    __fpNodeTempBuffer = []
+    __itemSetCount = 0
+    __maxPatternLength = 1000
+
+    def __init__(self, iFile, minSup, minRS, sep='\t'):
+        super().__init__(iFile, minSup, minRS, sep)
+        self.__finalPatterns = {}
 
-    def _creatingItemSets(self):
+    def __creatingItemSets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
+            Storing the complete transactions of the __Database/input file in a __Database variable
+
 
             """
-        self._Database = []
+        self.__Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
+                self.__Database = self._iFile['Transactions'].tolist()
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(temp)
+                    self.__Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _getRatio(self, prefix, prefixLength, s):
-        """
-            A Function to get itemSet Ratio
-            :param prefix:the path
-            :type prefix: list
-            :param prefixLength: length
-            :type prefixLength:int
-            :s :current ratio
-            :type s:float
-            :return: minAllConf of prefix
-            :rtype:float
-        """
-        maximums = 0
-        for ele in range(prefixLength):
-            i = prefix[ele]
-            if maximums < self._mapSupport.get(i):
-                maximums = self._mapSupport.get(i)
-        return s / maximums
-
-    def _frequentOneItem(self):
+    def __frequentOneItem(self):
         """Generating One frequent items sets
 
         """
-        self._mapSupport = {}
-        for i in self._Database:
+        self.__mapSupport = {}
+        for i in self.__Database:
             for j in i:
-                if j not in self._mapSupport:
-                    self._mapSupport[j] = 1
+                if j not in self.__mapSupport:
+                    self.__mapSupport[j] = 1
                 else:
-                    self._mapSupport[j] += 1
+                    self.__mapSupport[j] += 1
 
-    def _saveItemSet(self, prefix, prefixLength, support):
+    def __saveItemSet(self, prefix, prefixLength, support, ratio):
         """To save the frequent patterns mined form frequentPatternTree
 
         :param prefix: the frequent pattern
         :type prefix: list
-        :param prefixLength : the length of a frequent pattern
-        :type prefixLength : int
+        :param prefixLength: the length of a frequent pattern
+        :type prefixLength: int
         :param support: the support of a pattern
-        :type support :  int
-        :The frequent patterns are update into global variable finalPatterns
+        :type support:  int
         """
-        allconf = self._getRatio(prefix, prefixLength, support)
-        if allconf < self._minAllConf:
-            return
-        l = []
+
+        sample = []
         for i in range(prefixLength):
-            l.append(prefix[i])
-        self._itemSetCount += 1
-        self._finalPatterns[tuple(l)] = [support, allconf]
-    
-    def _convert(self, value):
-        """
-        to convert the type of user specified minSup value
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (len(self._Database) * value)
-            else:
-                value = int(value)
-        return value
+            sample.append(prefix[i])
+        self.__itemSetCount += 1
+        self.__finalPatterns[tuple(sample)] = str(support) + " : " + str(ratio)
 
-    def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
+    def __saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
         """Generating all the combinations for items in single branch in frequentPatternTree
 
         :param tempBuffer: items in a list
         :type tempBuffer: list
-        :param s : support at leaf node of a branch
-        :param position : the length of a tempBuffer
-        :type position : int
-        :param prefix : it represents the list of leaf node
-        :type prefix : list
-        :param prefixLength : the length of prefix
-        :type prefixLength :int
-        
+        :param s: support at leaf node of a branch
+        :param position: the length of a tempBuffer
+        :type position: int
+        :param prefix: it represents the list of leaf node
+        :type prefix: list
+        :param prefixLength: the length of prefix
+        :type prefixLength: int
+
         """
         max1 = 1 << position
         for i in range(1, max1):
             newPrefixLength = prefixLength
             for j in range(position):
                 isSet = i & (1 << j)
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
-            self._saveItemSet(prefix, newPrefixLength, s)
-
-    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport):
-        """
+            ratio = s / self.__mapSupport[self.__getMinItem(prefix, newPrefixLength)]
+            if ratio >= self._minRS:
+                self.__saveItemSet(prefix, newPrefixLength, s, ratio)
 
-        Mining the fp tree
+    def __frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, __mapSupport, minConf):
+        """Mining the fp tree
 
         :param frequentPatternTree: it represents the frequentPatternTree
         :type frequentPatternTree: class Tree
-        :param prefix : it represents a empty list and store the patterns that are mined
-        :type prefix : list
-        :param param prefixLength : the length of prefix
-        :type prefixLength :int
-        :param mapSupport : it represents the support of item
-        :type mapSupport : dictionary
-
+        :param prefix: it represents a empty list and store the patterns that are mined
+        :type prefix: list
+        :param param prefixLength: the length of prefix
+        :type prefixLength: int
+        :param __mapSupport : it represents the support of item
+        :type __mapSupport : dictionary
         """
-
         singlePath = True
         position = 0
         s = 0
         if len(frequentPatternTree.root.child) > 1:
             singlePath = False
         else:
             currentNode = frequentPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
-                self._fpNodeTempBuffer.insert(position, currentNode)
+                self.__fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
-            self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
+            self.__saveAllCombinations(self.__fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
             for i in reversed(frequentPatternTree.headerList):
                 item = i
-                support = mapSupport[i]
+                support = __mapSupport[i]
+                CminSup = max(self._minSup, support * self._minRS)
                 betaSupport = support
                 prefix.insert(prefixLength, item)
-                self._saveItemSet(prefix, prefixLength + 1, betaSupport)
-                if prefixLength + 1 < self._maxPatternLength:
+                max1 = self.__getMinItem(prefix, prefixLength)
+                if self.__mapSupport[max1] > self.__mapSupport[item]:
+                    max1 = item
+                ratio = support / self.__mapSupport[max1]
+                if ratio >= self._minRS:
+                    self.__saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
+                if prefixLength + 1 < self.__maxPatternLength:
                     prefixPaths = []
                     path = frequentPatternTree.mapItemNodes.get(item)
-                    mapSupportBeta = {}
+                    __mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
-                            prefixPath = []
-                            prefixPath.append(path)
+                            prefixPath = [path]
                             pathCount = path.counter
                             parent1 = path.parent
-                            while parent1.itemId != -1:
-                                prefixPath.append(parent1)
-                                if mapSupportBeta.get(parent1.itemId) is None:
-                                    mapSupportBeta[parent1.itemId] = pathCount
-                                else:
-                                    mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
-                                parent1 = parent1.parent
-                            prefixPaths.append(prefixPath)
+                            if __mapSupport.get(parent1.itemId) >= CminSup:
+                                while parent1.itemId != -1:
+                                    mins = CminSup
+                                    if __mapSupport.get(parent1.itemId) >= mins:
+                                        prefixPath.append(parent1)
+                                        if __mapSupportBeta.get(parent1.itemId) is None:
+                                            __mapSupportBeta[parent1.itemId] = pathCount
+                                        else:
+                                            __mapSupportBeta[parent1.itemId] = __mapSupportBeta[
+                                                                                   parent1.itemId] + pathCount
+                                        parent1 = parent1.parent
+                                    else:
+                                        break
+                                prefixPaths.append(prefixPath)
                         path = path.nodeLink
-                    treeBeta = _Tree()
+                    __treeBeta = _Tree()
                     for k in prefixPaths:
-                        treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
-                    if len(treeBeta.root.child) > 0:
-                        treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
-    
-    def startMine(self):
+                        __treeBeta.addPrefixPath(k, __mapSupportBeta, self._minSup)
+                    if len(__treeBeta.root.child) > 0:
+                        __treeBeta.createHeaderList(__mapSupportBeta, self._minSup)
+                        self.__frequentPatternGrowthGenerate(__treeBeta, prefix, prefixLength + 1, __mapSupportBeta,
+                                                           minConf)
+
+    def __convert(self, value):
+        """
+        to convert the type of user specified __minSup value
+        :param value: user specified __minSup value
+        :return: converted type
         """
-        main method to start
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self.__Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+                value = (len(self.__Database) * value)
+            else:
+                value = int(value)
+        return value
 
+    def startMine(self):
         """
-        self._startTime = _ab._time.time()
+            main program to start the operation
+        """
+
+        self.__startTime = _ab._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
-        self._tree = _Tree()
-        self._finalPatterns = {}
-        self._frequentOneItem()
-        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
-        _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        for i in self._Database:
-            _transaction = []
+        if self._minSup is None:
+            raise Exception("Please enter the Minimum Support")
+        self.__creatingItemSets()
+        self._minSup = self.__convert(self._minSup)
+        self._minRS = float(self._minRS)
+        self.__frequentOneItem()
+        self.__finalPatterns = {}
+        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup}
+        __itemSetBuffer = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        for i in self.__Database:
+            transaction = []
             for j in i:
-                if j in _itemSetBuffer:
-                    _transaction.append(j)
-            _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
-            self._tree.addTransaction(_transaction)
-        self._tree.createHeaderList(self._mapSupport, self._minSup)
-        if len(self._tree.headerList) > 0:
-            self._itemSetBuffer = []
-            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
-        print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
-        self._endTime = _ab._time.time()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
+                if j in __itemSetBuffer:
+                    transaction.append(j)
+            transaction.sort(key=lambda val: self.__mapSupport[val], reverse=True)
+            self.__tree.addTransaction(transaction)
+        self.__tree.createHeaderList(self.__mapSupport, self._minSup)
+        if len(self.__tree.headerList) > 0:
+            self.__itemSetBuffer = []
+            self.__frequentPatternGrowthGenerate(self.__tree, self.__itemSetBuffer, 0, self.__mapSupport, self._minRS)
+        print("Relative support frequent patterns were generated successfully using RSFPGrowth algorithm")
+        self.__endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.__memoryRSS = float()
+        self.__memoryUSS = float()
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
-        """
-        Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryUSS
+        return self.__memoryUSS
 
     def getMemoryRSS(self):
-        """
-        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.__memoryRSS
 
-    def getRuntime(self):
+    def __getMinItem(self, prefix, prefixLength):
         """
-        Calculating the total amount of runtime taken by the mining process
+            returns the minItem from prefix
+        """
+        minItem = prefix[0]
+        for i in range(prefixLength):
+            if self.__mapSupport[minItem] > self.__mapSupport[prefix[i]]:
+                minItem = prefix[i]
+        return minItem
+
+    def getRuntime(self):
+        """Calculating the total amount of runtime taken by the mining process
 
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self._endTime - self._startTime
+        return self.__endTime - self.__startTime
 
     def getPatternsAsDataFrame(self):
-        """
-
-        Storing final frequent patterns in a dataframe
+        """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
-            pat = " "
+        for a, b in self.__finalPatterns.items():
+            pattern = str()
             for i in a:
-                pat += str(i) + " "
-            data.append([pat, b[0], b[1]])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
+                pattern = pattern + i + " "
+            data.append([pattern, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """
-        Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
-        for x, y in self._finalPatterns.items():
-            pat = ""
+        self.__oFile = outFile
+        writer = open(self.__oFile, 'w+')
+        for x, y in self.__finalPatterns.items():
+            pattern = str()
             for i in x:
-                pat += str(i) + "\t"
-            patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
-            writer.write("%s \n" % patternsAndSupport)
+                pattern = pattern + i + "\t"
+            s1 = pattern.strip() + ": " + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
-        """
-        Function to send the set of frequent patterns after completion of the mining process
+        """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
         :rtype: dict
         """
-        return self._finalPatterns
+        res = dict()
+        for x, y in self.__finalPatterns.items():
+            pattern = str()
+            for i in x:
+                pattern = pattern + i + "\t"
+            s1 = str(y)
+            res[pattern] = s1
+        return res
 
     def printResults(self):
-        print("Total number of Correlated Patterns:", len(self.getPatterns()))
+        print("Total number of Relative Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = RSFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = RSFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
-        print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in seconds:", _ap.getRuntime())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py` & `pami-2023.8.1/PAMI/correlatedPattern/basic/CoMinePlus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
+# CPGrowthPlus is one of the efficient algorithm to discover Correlated patterns in a transactional database.
 #
 #  **Importing this algorithm into a python program**
 #   -----------------------------------------------
 #
-#                 from PAMI.coveragePattern.basic import CPPG as alg
+#                 from PAMI.correlatedPattern.basic import CPGrowthPlus as alg
 #
-#                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
+#                 obj = alg.CPGrowthPlus(iFile, minSup, minAllConf, sep)
 #
 #                 obj.startMine()
 #
-#                 coveragePatterns = obj.getPatterns()
+#                 correlatedPattern = obj.getPatterns()
 #
-#                 print("Total number of coverage Patterns:", len(coveragePatterns))
+#                 print("Total number of correlated Patterns:", len(correlatedPattern))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -25,17 +25,14 @@
 #
 #                 print("Total Memory in RSS", memRSS)
 #
 #                 run = obj.getRuntime()
 #
 #                 print("Total ExecutionTime in seconds:", run)
 
-
-
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -49,18 +46,17 @@
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 """
 
 from PAMI.correlatedPattern.basic import abstract as _ab
 
 
-
 class _Node:
     """
-        A class used to represent the node of frequentPatternTree
+        A class used to represent the node of correlatedPatternTree
 
     Attributes :
     ----------
         itemId: int
             storing item of a node
         counter: int
             To maintain the support of node
@@ -71,15 +67,15 @@
         nodeLink : node
             Points to the node with same itemId
 
     Methods :
     -------
 
         getChild(itemName)
-            returns the node with same itemName from frequentPatternTree
+            returns the node with same itemName from correlatedPatternTree
     """
 
     def __init__(self):
         self.itemId = -1
         self.counter = 1
         self.parent = None
         self.child = []
@@ -87,27 +83,27 @@
 
     def getChild(self, itemName):
         """
         Retrieving the child from the tree
 
             :param itemName: name of the child
             :type itemName: list
-            :return: returns the node with same itemName from frequentPatternTree
+            :return: returns the node with same itemName from correlatedPatternTree
             :rtype: list
 
         """
         for i in self.child:
             if i.itemId == itemName:
                 return i
         return None
 
 
 class _Tree:
     """
-        A class used to represent the frequentPatternGrowth tree structure
+        A class used to represent the correlatedPatternGrowth tree structure
 
     Attributes :
     ----------
         headerList : list
             storing the list of items in tree sorted in ascending of their supports
         mapItemNodes : dictionary
             storing the nodes with same item name
@@ -117,34 +113,34 @@
             representing the root Node in a tree
 
     Methods :
     -------
         createHeaderList(items,minSup)
             takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in frequentPatternTree
+            creating transaction as a branch in correlatedPatternTree
         fixNodeLinks(item,newNode)
             To create the link for nodes with same item
         printTree(Node)
-            gives the details of node in frequentPatternGrowth tree
+            gives the details of node in correlatedPatternGrowth tree
         addPrefixPath(prefix,port,minSup)
            It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
     def addTransaction(self, transaction):
         """
         Adding a transaction into a tree
 
-        :param transaction: it represents the one transactions in database
+        :param transaction: it represents a transaction in a database
         :type transaction: list
         """
 
         # This method taken a transaction as input and returns the tree
         current = self.root
         for i in transaction:
             child = current.getChild(i)
@@ -157,80 +153,78 @@
                 current = newNode
             else:
                 child.counter += 1
                 current = child
 
     def fixNodeLinks(self, item, newNode):
         """
-        Fixing node link for the newNode that inserted into frequentPatternTree
+        Fixing node link for the newNode that inserted into correlatedPatternTree
 
         :param item: it represents the item of newNode
         :type item: int
-        :param newNode: it represents the newNode that inserted in frequentPatternTree
+        :param newNode: it represents the newNode that inserted in correlatedPatternTree
         :type newNode: Node
 
         """
         if item in self.mapItemLastNodes.keys():
             lastNode = self.mapItemLastNodes[item]
             lastNode.nodeLink = newNode
         self.mapItemLastNodes[item] = newNode
         if item not in self.mapItemNodes.keys():
             self.mapItemNodes[item] = newNode
 
     def printTree(self, root):
         """
 
-        Print the details of Node in frequentPatternTree
+        Print the details of Node in correlatedPatternTree
 
-        :param root: it represents the Node in frequentPatternTree
+        :param root: it represents the Node in correlatedPatternTree
         :type root: Node
 
         """
-
         # this method is used print the details of tree
         if not root.child:
             return
         else:
             for i in root.child:
                 print(i.itemId, i.counter, i.parent.itemId)
                 self.printTree(i)
 
     def createHeaderList(self, mapSupport, minSup):
         """
-
         To create the headerList
 
         :param mapSupport: it represents the items with their supports
         :type mapSupport: dictionary
         :param minSup: it represents the minSup
         :param minSup: float
 
         """
-        # the frequentPatternTree always maintains the header table to start the mining from leaf nodes
+        # the correlatedPatternTree always maintains the header table to start the mining from leaf nodes
         t1 = []
         for x, y in mapSupport.items():
             if y >= minSup:
                 t1.append(x)
-        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda val: val[1], reverse=True)]
         self.headerList = [i for i in t1 if i in itemSetBuffer]
 
     def addPrefixPath(self, prefix, mapSupportBeta, minSup):
         """
 
-        To construct the conditional tree with prefix paths of a node in frequentPatternTree
+        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
 
         :param prefix: it represents the prefix items of a Node
         :type prefix: list
         :param mapSupportBeta: it represents the items with their supports
         :param mapSupportBeta: dictionary
         :param minSup: to check the item meets with minSup
         :param minSup: float
 
         """
-        # this method is used to add prefix paths in conditional trees of frequentPatternTree
+        # this method is used to add prefix paths in conditional trees of correlatedPatternTree
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
             if mapSupportBeta.get(pathItem.itemId) >= minSup:
                 child = current.getChild(pathItem.itemId)
@@ -243,29 +237,27 @@
                     current = newNode
                     self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
                     child.counter += pathCount
                     current = child
 
 
-class CPGrowthPlus(_ab._correlatedPatterns):
+class CoMinePlus(_ab._correlatedPatterns):
     """ 
-    :Description:    CPGrowthPlus is one of the efficient algorithm to discover Correlated frequent patterns in a transactional database.
-                     Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that
-                     have support within specified interval.
+    :Description:    CoMinePlus is one of the efficient algorithm to discover correlated patterns in a transactional database. Using Item Support Intervals technique which is generating correlated patterns of higher order by combining only with items that have support within specified interval.
 
     :Reference:
         Uday Kiran R., Kitsuregawa M. (2012) Efficient Discovery of Correlated Patterns in Transactional Databases Using Items’ Support Intervals.
         In: Liddle S.W., Schewe KD., Tjoa A.M., Zhou X. (eds) Database and Expert Systems Applications. DEXA 2012. Lecture Notes in Computer Science, vol 7446. Springer, Berlin, Heidelberg.
         https://doi.org/10.1007/978-3-642-32600-4_18
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of correlated patterns
     :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
+                   Name of the output file to store complete set of correlated patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  minAllConf: str :
                    Name of Neighbourhood file name
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
@@ -301,39 +293,39 @@
         maxPatternLength : int
            it represents the constraint for pattern length
 
     **Methods to execute code on terminal**
     ---------------------------------------
 
             Format:
-                      >>>  python3 CPPG.py <inputFile> <outputFile> <minRF> <minCS> <maxOR> <'\t'>
+                      >>>  python3 CoMinePlus.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
 
             Example:
-                      >>>   python3 CPPG.py sampleTDB.txt patterns.txt 0.4 0.7 0.5 ','
+                      >>>   python3 CoMinePlus.py sampleTDB.txt patterns.txt 0.4 0.5 ','
 
 
 
     **Importing this algorithm into a python program**
     -----------------------------------------------------------------
 
     .. code-block:: python
 
-                from PAMI.coveragePattern.basic import CPPG as alg
+                from PAMI.correlatedPattern.basic import CoMinePlus as alg
 
-                obj = alg.CPPG(iFile, minRF, minCS, maxOR)
+                obj = alg.CoMinePlus(iFile, minSup, minAllConf, sep)
 
                 obj.startMine()
 
-                coveragePatterns = obj.getPatterns()
+                correlatedPatterns = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePatterns))
+                print("Total number of correlated patterns:", len(correlatedPatterns))
 
                 obj.save(oFile)
 
-                Df = obj.getPatternsAsDataFrame()
+                df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
                 print("Total Memory in USS:", memUSS)
 
                 memRSS = obj.getMemoryRSS()
 
@@ -367,22 +359,30 @@
     _itemSetBuffer = None
     _fpNodeTempBuffer = []
     _itemSetCount = 0
     _maxPatternLength = 1000
     _sep = "\t"
 
     def __init__(self, iFile, minSup, minAllConf, sep="\t"):
+        """
+        param iFile: input file name
+        type iFile: str or DataFrame or url
+        param minSup: user-specified minimum support
+        type minSup: int or float
+        param minAllConf: user-specified minimum all confidence
+        type minAllConf: float
+        param sep: delimiter of input file
+        type sep : str
+        """
         super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
-
-
-            """
+        """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
@@ -403,50 +403,50 @@
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _frequentOneItem(self):
+    def _correlatedOneItem(self):
         """
-        Generating One frequent items sets
+        Generating One correlated items sets
 
         """
         self._mapSupport = {}
         for i in self._Database:
             for j in i:
                 if j not in self._mapSupport:
                     self._mapSupport[j] = 1
                 else:
                     self._mapSupport[j] += 1
 
     def _saveItemSet(self, prefix, prefixLength, support, ratio):
         """
-        To save the frequent patterns mined form frequentPatternTree
+        To save the correlated patterns mined form correlatedPatternTree
 
-        :param prefix: the frequent pattern
+        :param prefix: the correlated pattern
         :type prefix: list
-        :param prefixLength: the length of a frequent pattern
+        :param prefixLength: the length of a correlated pattern
         :type prefixLength: int
         :param support: the support of a pattern
         :type support:  int
         """
 
         sample = []
         for i in range(prefixLength):
             sample.append(prefix[i])
         self._itemSetCount += 1
         self._finalPatterns[tuple(sample)] = [support, ratio]
 
     def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
         """
-        Generating all the combinations for items in single branch in frequentPatternTree
+        Generating all the combinations for items in single branch in correlatedPatternTree
 
-        :param tempBuffer: items in a list
+        :param tempBuffer: items in a single branch
         :type tempBuffer: list
         :param s: support at leaf node of a branch
         :param position: the length of a tempBuffer
         :type position: int
         :param prefix: it represents the list of leaf node
         :type prefix: list
         :param prefixLength: the length of prefix
@@ -461,73 +461,73 @@
                 if isSet > 0:
                     prefix.insert(newPrefixLength, tempBuffer[j].itemId)
                     newPrefixLength += 1
             ratio = s/self._mapSupport[self._getMaxItem(prefix, newPrefixLength)]
             if ratio >= self._minAllConf:
                 self._saveItemSet(prefix, newPrefixLength, s, ratio)
 
-    def _frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, mapSupport, minConf):
+    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport, minConf):
         """
         Mining the fp tree
 
-        :param frequentPatternTree: it represents the frequentPatternTree
-        :type frequentPatternTree: class Tree
-        :param prefix: it represents a empty list and store the patterns that are mined
+        :param correlatedPatternTree: it represents the correlatedPatternTree
+        :type correlatedPatternTree: class Tree
+        :param prefix: it represents an empty list and store the patterns that are mined
         :type prefix: list
         :param param prefixLength: the length of prefix
         :type prefixLength: int
         :param mapSupport : it represents the support of item
         :type mapSupport : dictionary
         """
         singlePath = True
         position = 0
         s = 0
-        if len(frequentPatternTree.root.child) > 1:
+        if len(correlatedPatternTree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = frequentPatternTree.root.child[0]
+            currentNode = correlatedPatternTree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
                 self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
             self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(frequentPatternTree.headerList):
+            for i in reversed(correlatedPatternTree.headerList):
                 item = i
                 support = mapSupport[i]
                 low = max(int(_ab._math.floor(mapSupport[i]*self._minAllConf)), self._minSup)
                 high = max(int(_ab._math.floor(mapSupport[i]/minConf)), self._minSup)
-                betaSupport = support              
+                betaSupport = support
                 prefix.insert(prefixLength, item)
                 max1 = self._getMaxItem(prefix, prefixLength)
                 if self._mapSupport[max1] < self._mapSupport[item]:
                     max1 = item
                 ratio = support / self._mapSupport[max1]
                 if ratio >= self._minAllConf:
                     self._saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
                 if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = frequentPatternTree.mapItemNodes.get(item)
+                    path = correlatedPatternTree.mapItemNodes.get(item)
                     mapSupportBeta = {}
                     while path is not None:
                         if path.parent.itemId != -1:
                             prefixPath = [path]
                             pathCount = path.counter
                             parent1 = path.parent
                             if mapSupport.get(parent1.itemId) >= low and mapSupport.get(parent1.itemId) <= high:
                                 while parent1.itemId != -1:
-                                    allconf = int(support/max(mapSupport.get(parent1.itemId), support))
-                                    if mapSupport.get(parent1.itemId) >= allconf:
+                                    all_conf = int(support/max(mapSupport.get(parent1.itemId), support))
+                                    if mapSupport.get(parent1.itemId) >= all_conf:
                                         prefixPath.append(parent1)
                                         if mapSupportBeta.get(parent1.itemId) is None:
                                             mapSupportBeta[parent1.itemId] = pathCount
                                         else:
                                             mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
                                         parent1 = parent1.parent
                                     else:
@@ -535,15 +535,15 @@
                                 prefixPaths.append(prefixPath)
                         path = path.nodeLink
                     treeBeta = _Tree()
                     for k in prefixPaths:
                         treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
                     if len(treeBeta.root.child) > 0:
                         treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        self._frequentPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
+                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta, minConf)
 
     def _convert(self, value):
         """
         to convert the type of user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
@@ -569,28 +569,28 @@
             raise Exception("Please enter the file path or file name:")
         if self._minSup is None:
             raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
         self._finalPatterns = {}
         self._tree = _Tree()
         self._minSup = self._convert(self._minSup)
-        self._frequentOneItem()
+        self._correlatedOneItem()
         self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
         _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in self._Database:
             _transaction = []
             for j in i:
                 if j in _itemSetBuffer:
                     _transaction.append(j)
             _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
             self._tree.addTransaction(_transaction)
         self._tree.createHeaderList(self._mapSupport, self._minSup)
         if len(self._tree.headerList) > 0:
             self._itemSetBuffer = []
-            self._frequentPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
+            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport, self._minAllConf)
         print("Correlated Frequent patterns were generated successfully using CorrelatedPatternGrowth algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryRSS = float()
         self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
@@ -617,31 +617,31 @@
 
     def _getMaxItem(self, prefix, prefixLength):
         maxItem = prefix[0]
         for i in range(prefixLength):
             if self._mapSupport[maxItem] < self._mapSupport[prefix[i]]:
                 maxItem = prefix[i]
         return maxItem
-    
+
     def getRuntime(self):
         """
         Calculating the total amount of runtime taken by the mining process
 
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """
-        Storing final frequent patterns in a dataframe
+        Storing final correlated patterns in a dataframe
 
-        :return: returning frequent patterns in a dataframe
+        :return: returning correlated patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             pat = " "
@@ -649,53 +649,56 @@
                 pat += str(i) + " "
             data.append([pat, b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
         """
-        Complete set of frequent patterns will be loaded in to a output file
+        Complete set of correlated patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
+        :param outFile: name of the outputfile
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             pattern = str()
             for i in x:
                 pattern = pattern + i + "\t"
             s1 = str(pattern.strip()) + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """
-        Function to send the set of frequent patterns after completion of the mining process
+        Function to send the set of correlated patterns after completion of the mining process
 
-        :return: returning frequent patterns
+        :return: returning correlated patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """
+        function to print the result after completing the process
+        """
         print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = CPGrowthPlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
-            _ap = CPGrowthPlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
+            _ap = CoMinePlus(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
         _correlatedPatterns = _ap.getPatterns()
         print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.8.1/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/correlatedPattern/basic/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import sys as _sys
 import math as _math
 
 
 class _correlatedPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+    """ This abstract base class defines the variables and methods that every correlated pattern mining algorithm must
         employ in PAMI
 
 
     Attributes :
     ----------
         iFile : str
             Input file name or path of the input file
@@ -50,15 +50,15 @@
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of frequent patterns
+            Name of the output file to store complete set of correlated patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
     Methods :
     -------
@@ -110,31 +110,31 @@
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of frequent patterns generated will be retrieved from this function"""
+        """Complete set of correlated patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of frequent patterns will be saved in to an output file from this function
+        """Complete set of correlated patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of correlated patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
```

### Comparing `pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py` & `pami-2023.8.1/PAMI/coveragePattern/basic/CMine.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 #
 #                 from PAMI.coveragePattern.basic import CMine as alg
 #
 #                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 #
 #                 obj.startMine()
 #
-#                 coveragePatterns = obj.getPatterns()
+#                 coveragePattern = obj.getPatterns()
 #
-#                 print("Total number of coverage Patterns:", len(coveragePatterns))
+#                 print("Total number of coverage Patterns:", len(coveragePattern))
 #
 #                 obj.save(oFile)
 #
 #                 Df = obj.getPatternsAsDataFrame()
 #
 #                 memUSS = obj.getMemoryUSS()
 #
@@ -46,26 +46,26 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 
 
 
-from PAMI.coveragePatterns.basic import abstract as _ab
+from PAMI.coveragePattern.basic import abstract as _ab
 
 class CMine(_ab._coveragePatterns):
     """
 
     :Description:  CMine algorithms aims to discover the coverage patterns in transactional databases.
 
     :Reference:    Bhargav Sripada, Polepalli Krishna Reddy, Rage Uday Kiran:
                    Coverage patterns for efficient banner advertisement placement. WWW (Companion Volume) 2011: 131-132
                    https://dl.acm.org/doi/10.1145/1963192.1963259
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minRF: float:
                    Controls the minimum number of transactions in which every item must appear in a database.
     :param  minCS: float:
                    Controls the minimum number of transactions in which at least one time within a pattern must appear in a database.
     :param  maxOR: float:
@@ -111,17 +111,17 @@
 
                 from PAMI.coveragePattern.basic import CMine as alg
 
                 obj = alg.CMine(iFile, minRF, minCS, maxOR, seperator)
 
                 obj.startMine()
 
-                coveragePatterns = obj.getPatterns()
+                coveragePattern = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePatterns))
+                print("Total number of coverage Patterns:", len(coveragePattern))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
@@ -222,23 +222,23 @@
                     tidData[item] = [self._lno]
                 else:
                     tidData[item].append(self._lno)
         coverageTidData = {k: v for k, v in tidData.items() if len(v) / len(self._Database) >= self._minRF}
         coverageTidData = dict(sorted(coverageTidData.items(), reverse=True, key=lambda x: len(x[1])))
         return coverageTidData
 
-    def tidToBitset(self,itemset):
+    def tidToBitset(self,item_set):
         """
         This function converts tid list to bitset.
-        :param itemset:
+        :param item_set:
         :return:
         """
         bitset = {}
 
-        for k,v in itemset.items():
+        for k,v in item_set.items():
             bitset[k] = 0b1
             bitset[k] = (bitset[k] << int(v[0])) | 0b1
             for i in range(1,len(v)):
                 diff = int(v[i]) - int(v[i-1])
                 bitset[k] = (bitset[k] << diff) | 0b1
             bitset[k] = (bitset[k] << (self._lno - int(v[i])))
         return bitset
@@ -247,28 +247,28 @@
         """
         This function generate coverage pattern about prefix.
         :param prefix: String
         :param tidData: list
         :return:
         """
         # variables to store coverage item set and
-        itemset = prefix[0]
+        item_set = prefix[0]
 
         # Get the length of tidData
         length = len(tidData)
         for i in range(length):
             tid = prefix[1] & tidData[i][1]
             tid1 = prefix[1] | tidData[i][1]
             andCount = bin(tid).count("1") - 1
             orCount = bin(tid1).count("1") - 1
             if orCount/len(self._Database) >= self._minCS and andCount / len(str(prefix[1])) <= self._maxOR:
-                coverageItemset = itemset + '\t' + tidData[i][0]
+                coverageItem_set = item_set + '\t' + tidData[i][0]
                 if orCount / len(self._Database) >= self._minRF:
-                    self._finalPatterns[coverageItemset] = andCount
-                self.genPatterns((coverageItemset,tid),tidData[i+1:length])
+                    self._finalPatterns[coverageItem_set] = andCount
+                self.genPatterns((coverageItem_set,tid),tidData[i+1:length])
 
     def generateAllPatterns(self,coverageItems):
         """
         This function generates all coverage patterns.
         :param coverageItems: coverage items
         :return:
         """
@@ -335,16 +335,16 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of coverage patterns will be loaded in to a output file
-        :param outFile: name of the output file
+        """Complete set of coverage patterns will be loaded in to an output file
+        :param outFile: name of the outputfile
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
@@ -353,14 +353,17 @@
         """ Function to send the set of coverage patterns after completion of the mining process
         :return: returning coverage patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """
+         This function is used to print the result
+        """
         print("Total number of Coverage Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__=="__main__":
@@ -373,13 +376,8 @@
         _ap.startMine()
         print("Total number of coverage Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = CPPG('sample.txt', 0.4, 0.7, 0.5, ' ')
-        _ap.startMine()
-        print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
-        _ap.save('output.txt')
-        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py` & `pami-2023.8.1/PAMI/coveragePattern/basic/CPPG.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# CPPG  algorithm discovers coverage patterns in a transactional database.
+# CPPG algorithm discovers coverage patterns in a transactional database.
 #
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------
 #
 #             from PAMI.coveragePattern.basic import CPPG as alg
 #
 #             obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 #
 #             obj.startMine()
 #
-#             coveragePatterns = obj.getPatterns()
+#             coveragePattern = obj.getPatterns()
 #
-#             print("Total number of coverage Patterns:", len(coveragePatterns))
+#             print("Total number of coverage Patterns:", len(coveragePattern))
 #
 #             obj.save(oFile)
 #
 #             Df = obj.getPatternsAsDataFrame()
 #
 #             memUSS = obj.getMemoryUSS()
 #
@@ -45,15 +45,15 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from PAMI.coveragePatterns.basic import abstract as _ab
+from PAMI.coveragePattern.basic import abstract as _ab
 
 
 _maxPer = float()
 _minSup = float()
 _lno = int()
 
 
@@ -63,15 +63,15 @@
     :Description:  CPPG  algorithm discovers coverage patterns in a transactional database.
 
     :Reference:     Gowtham Srinivas, P.; Krishna Reddy, P.; Trinath, A. V.; Bhargav, S.; Uday Kiran, R. (2015).
                     Mining coverage patterns from transactional databases. Journal of Intelligent Information Systems, 45(3), 423–439.
                     https://link.springer.com/article/10.1007/s10844-014-0318-3
 
     :param  iFile: str :
-           Name of the Input file to mine complete set of frequent patterns
+           Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minRF: float:
                    Controls the minimum number of transactions in which every item must appear in a database.
     :param  minCS: float:
                    Controls the minimum number of transactions in which at least one time within a pattern must appear in a database.
     :param  maxOR: float:
@@ -120,17 +120,17 @@
 
                 from PAMI.coveragePattern.basic import CPPG as alg
 
                 obj = alg.CPPG(iFile, minRF, minCS, maxOR)
 
                 obj.startMine()
 
-                coveragePatterns = obj.getPatterns()
+                coveragePattern = obj.getPatterns()
 
-                print("Total number of coverage Patterns:", len(coveragePatterns))
+                print("Total number of coverage Patterns:", len(coveragePattern))
 
                 obj.save(oFile)
 
                 Df = obj.getPatternsAsDataFrame()
 
                 memUSS = obj.getMemoryUSS()
 
@@ -294,15 +294,15 @@
 
         if len(new_freqList) > 0:
             self._generateFrequentPatterns(new_freqList)
 
     def _savePeriodic(self, itemSet):
         """ To convert the ranks of items in to their original item names
 
-            :param itemSet: frequent pattern
+            :param itemSet: frequent patterns
             :return: frequent pattern with original item names
         """
         t1 = str()
         for i in itemSet:
             t1 = t1 + self._rankedUp[i] + "\t"
         return t1
 
@@ -403,17 +403,17 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b[0], b[1]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Periodicity'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of periodic-frequent patterns will be loaded in to a output file
+        """Complete set of periodic-frequent patterns will be loaded in to an output file
 
-        :param outFile: name of the output file
+        :param outFile: name of the outputfile
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(len(y))
             writer.write("%s \n" % s1)
@@ -423,14 +423,17 @@
 
         :return: returning periodic-frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """
+           Function used to print the result
+        """
         print("Total number of Coverage Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
@@ -443,13 +446,8 @@
         _ap.startMine()
         print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = CPPG('sample.txt', 0.4, 0.7, 0.5, ' ')
-        _ap.startMine()
-        print("Total number of Coverage Patterns:", len(_ap.getPatterns()))
-        _ap.save('output.txt')
-        _ap.printResults()
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/recurringPattern/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,53 +8,49 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
-import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
-class _coveragePatterns(_ABC):
+class _recurringPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
         employ in PAMI
 
        Attributes
         ----------
         iFile : str
             Input file name or path of the input file
-        minCS: int or float or str
-            The user can specify minCS either in count or proportion of database size.
-            If the program detects the data type of minCS is integer, then it treats minCS is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: minCS=10 will be treated as integer, while minCS=10.0 will be treated as float
-        maxOR: int or float or str
-            The user can specify maxOR either in count or proportion of database size.
-            If the program detects the data type of maxOR is integer, then it treats maxOR is expressed in count.
+        
+        maxPer: int or float or str
+            The user can specify maxPer either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
-            Example: maxOR=10 will be treated as integer, while maxOR=10.0 will be treated as float
-        minRF: int or float or str
-            The user can specify minRF either in count or proportion of database size.
-            If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        minPS: int or float or str
+            The user can specify minPS either in count or proportion of database size.
+            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
+            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
+        minRec: int or float or str
+            The user has to specify minRec in count.
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -81,43 +77,43 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minRF, minCS, maxOR, sep = '\t'):
+    def __init__(self, iFile, maxPer, minPS, minRec,sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param maxPer: The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         :type maxPer: int or float or str
-        :param sep: separator used in user specified input file
+        :param sep: the separator used in the database
         :type sep: str
         """
 
         self._iFile = iFile
-        self._minCS = minCS
-        self._minRF = minRF
-        self._maxOR = maxOR
+        self._minPS = minPS
+        self._maxPer = maxPer
+        self._minRec = minRec
         self._sep = sep
+        self._oFile = str()
         self._finalPatterns = {}
         self._startTime = float()
         self._endTime = float()
         self._memoryRSS = float()
         self._memoryUSS = float()
-        self._oFile = " "
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -158,10 +154,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print the results of the execution"""
+        """ To print all the results of execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.8.1/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.8.1/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.8.1/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,23 +48,23 @@
 
         """
 
         self.outputFile = outputFile
         with open(outputFile, 'w') as f:
              if self.condition not in condition_operator:
                 print('Condition error')
-            else:
+             else:
                 for tid in self.tids:
                     transaction = [item for item in self.items if condition_operator[self.condition](self.inputDF.at[tid, item], self.thresholdValue)]
                     if len(transaction) > 1:
                         f.write(f'{transaction[0]}')
                         for item in transaction[1:]:
                             f.write(f'\t{item}')
                     elif len(transaction) == 1:
-                        f.write(f'{transaction}')
+                        f.write(f'{transaction[0]}')
                     else:
                         continue
                     f.write('\n')
 
 
 
 
@@ -86,15 +86,15 @@
                     transaction = [item for item in self.items if condition_operator[self.condition](self.inputDF.at[tid, item], self.thresholdValue)]
                     if len(transaction) > 1:
                         f.write(f'{tid}')
                         for item in transaction:
                             f.write(f',{item}')
                     elif len(transaction) == 1:
                         f.write(f'{tid}')
-                        f.write(f',{transaction}')
+                        f.write(f',{transaction[0]}')
                     else:
                         continue
                     f.write('\n')
 
             
 
     def createUtility(self, outputFile):
```

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.8.1/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.8.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.8.1/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.8.1/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 import pandas as pd
 import validators
 import numpy as np
 from urllib.request import urlopen
 import PAMI.extras.graph.plotLineGraphFromDictionary as plt
 
 
-class temporalDatabaseStats:
+class uncertainTemporalDatabaseStats:
     """
-        Description:
-        -------------
-            temporalDatabaseStats is class to get stats of database.
+        :Description: temporalDatabaseStats is class to get stats of database.
 
         Attributes:
-        ----------
+        -----------
         inputFile : file
             input file path
         database : dict
             store time stamp and its transaction
         lengthList : list
             store size of all transaction
         timeStampCount : dict
             number of transactions per time stamp
         periodList : list
             all period list in the database
         sep : str
             separator in file. Default is tab space.
 
         Methods:
-        -------
+        --------
         run()
             execute readDatabase function
         readDatabase()
             read database from input file
         getDatabaseSize()
             get the size of database
         getMinimumTransactionLength()
@@ -96,27 +94,27 @@
         if isinstance(self.inputFile, str):
             if validators.url(self.inputFile):
                 data = urlopen(self.inputFile)
                 for line in data:
                     numberOfTransaction += 1
                     line.strip()
                     line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self.sep)]
-                    temp = [x for x in temp if x]
+                    temp = line.split(':')
+                    temp1 = [i.rstrip() for i in temp[0].split(self.sep)]
                     self.database[numberOfTransaction] = temp[1:]
                     self.timeStampCount[int(temp[0])] = self.timeStampCount.get(int(line[0]), 0)
                     self.timeStampCount[int(temp[0])] += 1
             else:
                 try:
                     with open(self.inputFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             numberOfTransaction += 1
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self.sep)]
-                            temp = [x for x in temp if x]
+                            line = line.strip()
+                            temp1 = line.split(':')
+                            temp = [i for i in temp1[0].split(self.sep)]
                             if len(temp) > 0:
                                 self.database[numberOfTransaction] = temp[1:]
                                 self.timeStampCount[int(temp[0])] = self.timeStampCount.get(int(line[0]), 0)
                                 self.timeStampCount[int(temp[0])] += 1
                 except IOError:
                     print("File Not Found")
                     quit()
@@ -339,36 +337,15 @@
 
             'Transactions': [['a', 'd', 'e'], ['b', 'a', 'f', 'g', 'h'], ['b', 'a', 'd', 'f'], ['b', 'a', 'c'],
                              ['a', 'd', 'g', 'k'],
 
                              ['b', 'd', 'g', 'c', 'i'], ['b', 'd', 'g', 'e', 'j']]}
 
     data = pd.DataFrame.from_dict(data)
-    obj = temporalDatabaseStats('spatiotemporal_T20I6D100K.txt', ',')
+    obj = uncertainTemporalDatabaseStats('uncertain_Temporal_BMS1.csv', '\t')
     import PAMI.extras.graph.plotLineGraphFromDictionary as plt
 
     obj.run()
     obj.printStats()
     obj.plotGraphs()
-    '''print(f'Database size : {obj.getDatabaseSize()}')
-    print(f'Minimum Transaction Size : {obj.getMinimumTransactionLength()}')
-    print(f'Average Transaction Size : {obj.getAverageTransactionLength()}')
-    print(f'Maximum Transaction Size : {obj.getMaximumTransactionLength()}')
-    print(f'Standard Deviation Transaction Size : {obj.getStandardDeviationTransactionLength()}')
-    print(f'Variance : {obj.getVarianceTransactionLength()}')
-    print(f'Sparsity : {obj.getSparsity()}')
-    print(f'Number of items : {obj.getTotalNumberOfItems()}')
-    print(f'Minimum period : {obj.getMinimumPeriod()}')
-    print(f'Average period : {obj.getAveragePeriod()}')
-    print(f'Maximum period : {obj.getMaximumPeriod()}')
-    itemFrequencies = obj.getSortedListOfItemFrequencies()
-    transactionLength = obj.getTransanctionalLengthDistribution()
-    numberOfTransactionPerTimeStamp = obj.getNumberOfTransactionsPerTimestamp()
-    # obj.save(itemFrequencies, 'itemFrequency.csv')
-    # obj.save(transactionLength, 'transactionSize.csv')
-    # obj.save(numberOfTransactionPerTimeStamp, 'numberOfTransaction.csv')
-    plt.plotLineGraphFromDictionary(itemFrequencies, 100, 'itemFrequencies', 'item rank', 'frequency')
-    plt.plotLineGraphFromDictionary(transactionLength, 100, 'transaction length', 'transaction length', 'frequency')
-    plt.plotLineGraphFromDictionary(numberOfTransactionPerTimeStamp, 100)'''
-
```

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         :param inputFile: input file name or path
         :type inputFile: str
         """
         self.inputFile = inputFile
         self.lengthList = []
         self.sep = sep
         self.database = {}
+        self.itemFrequencies = {}
 
     def run(self):
         self.readDatabase()
 
     def readDatabase(self):
         """
         read database from input file and store into database and size of each transaction.
@@ -175,15 +176,16 @@
         :return: item frequencies
         """
         itemFrequencies = {}
         for tid in self.database:
             for item in self.database[tid]:
                 itemFrequencies[item] = itemFrequencies.get(item, 0)
                 itemFrequencies[item] += 1
-        return {k: v for k, v in sorted(itemFrequencies.items(), key=lambda x: x[1], reverse=True)}
+        self.itemFrequencies = {k: v for k, v in sorted(itemFrequencies.items(), key=lambda x: x[1], reverse=True)}
+        return self.itemFrequencies
     
     def getFrequenciesInRange(self):
         fre = self.getSortedListOfItemFrequencies()
         rangeFrequencies = {}
         maximum = max([i for i in fre.values()])
         values = [int(i*maximum/6) for i in range(1,6)]
         va = len({key: val for key, val in fre.items() if val > 0 and val < values[0]})
@@ -223,32 +225,31 @@
         print(f'Average Transaction Size : {self.getAverageTransactionLength()}')
         print(f'Maximum Transaction Size : {self.getMaximumTransactionLength()}')
         print(f'Standard Deviation Transaction Size : {self.getStandardDeviationTransactionLength()}')
         print(f'Variance in Transaction Sizes : {self.getVarianceTransactionLength()}')
         print(f'Sparsity : {self.getSparsity()}')
   
     def plotGraphs(self):
-        itemFrequencies = self.getFrequenciesInRange()
+        # itemFrequencies = self.getFrequenciesInRange()
         transactionLength = self.getTransanctionalLengthDistribution()
-        plt.plotLineGraphFromDictionary(itemFrequencies, 100, 'Frequency', 'No of items', 'frequency')
-        plt.plotLineGraphFromDictionary(transactionLength, 100, 'transaction length', 'transaction length', 'frequency')
+        plt.plotLineGraphFromDictionary(self.itemFrequencies, 100, 0, 'Frequency', 'No of items', 'frequency')
+        plt.plotLineGraphFromDictionary(transactionLength, 100, 0, 'transaction length', 'transaction length', 'frequency')
 
 
 if __name__ == '__main__':
     data = {'tid': [1, 2, 3, 4, 5, 6, 7],
 
             'Transactions': [['a', 'd', 'e'], ['b', 'a', 'f', 'g', 'h'], ['b', 'a', 'd', 'f'], ['b', 'a', 'c'],
                              ['a', 'd', 'g', 'k'],
 
                              ['b', 'd', 'g', 'c', 'i'], ['b', 'd', 'g', 'e', 'j']]}
 
     # data = pd.DataFrame.from_dict('transactional_T10I4D100K.csv')
-    import PAMI.extras.graph.plotLineGraphFromDictionary as plt
-
-    # obj = transactionalDatabaseStats(data)
-    obj = transactionalDatabaseStats('transactional_BMS1.txt', ',')
+    import pandas as pd
+    # obj = transactionalDatabaseStats('transactional_BMS1.txt', ',')
+    obj = transactionalDatabaseStats(pd.DataFrame(data))
     obj.run()
     obj.printStats()
     obj.plotGraphs()
```

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 import pandas as pd
 import validators
 import numpy as np
 from urllib.request import urlopen
 import PAMI.extras.graph.plotLineGraphFromDictionary as plt
 
 
-class uncertainTemporalDatabaseStats:
+class temporalDatabaseStats:
     """
-        :Description: temporalDatabaseStats is class to get stats of database.
+        Description:
+        -------------
+            temporalDatabaseStats is class to get stats of database.
 
         Attributes:
-        -----------
+        ----------
         inputFile : file
             input file path
         database : dict
             store time stamp and its transaction
         lengthList : list
             store size of all transaction
         timeStampCount : dict
             number of transactions per time stamp
         periodList : list
             all period list in the database
         sep : str
             separator in file. Default is tab space.
 
         Methods:
-        --------
+        -------
         run()
             execute readDatabase function
         readDatabase()
             read database from input file
         getDatabaseSize()
             get the size of database
         getMinimumTransactionLength()
@@ -67,14 +69,15 @@
         """
         self.inputFile = inputFile
         self.database = {}
         self.lengthList = []
         self.timeStampCount = {}
         self.periodList = []
         self.sep = sep
+        self.periods = {}
 
     def run(self):
         self.readDatabase()
 
     def readDatabase(self):
         """
         read database from input file and store into database and size of each transaction.
@@ -94,52 +97,51 @@
         if isinstance(self.inputFile, str):
             if validators.url(self.inputFile):
                 data = urlopen(self.inputFile)
                 for line in data:
                     numberOfTransaction += 1
                     line.strip()
                     line = line.decode("utf-8")
-                    temp = line.split(':')
-                    temp1 = [i.rstrip() for i in temp[0].split(self.sep)]
+                    temp = [i.rstrip() for i in line.split(self.sep)]
+                    temp = [x for x in temp if x]
                     self.database[numberOfTransaction] = temp[1:]
                     self.timeStampCount[int(temp[0])] = self.timeStampCount.get(int(line[0]), 0)
                     self.timeStampCount[int(temp[0])] += 1
             else:
                 try:
                     with open(self.inputFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             numberOfTransaction += 1
-                            line = line.strip()
-                            temp1 = line.split(':')
-                            temp = [i for i in temp1[0].split(self.sep)]
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self.sep)]
+                            temp = [x for x in temp if x]
                             if len(temp) > 0:
                                 self.database[numberOfTransaction] = temp[1:]
                                 self.timeStampCount[int(temp[0])] = self.timeStampCount.get(int(line[0]), 0)
                                 self.timeStampCount[int(temp[0])] += 1
                 except IOError:
                     print("File Not Found")
                     quit()
         self.lengthList = [len(s) for s in self.database.values()]
         timeStampList = sorted(list(self.database.keys()))
         preTimeStamp = 0
         for ts in timeStampList:
             self.periodList.append(int(ts) - preTimeStamp)
             preTimeStamp = ts
-
-        # for line in self.Database:
-        #     numberOfTransaction += 1
-        #     self.database[numberOfTransaction] = line[1:]
-        #     self.timeStampCount[int(line[0])] = self.timeStampCount.get(int(line[0]), 0)
-        #     self.timeStampCount[int(line[0])] += 1
-        # self.lengthList = [len(s) for s in self.database.values()]
-        # timeStampList = sorted(list(self.timeStampCount.keys()))
-        # preTimeStamp = 0
-        # for ts in timeStampList:
-        #     self.periodList.append(int(ts)-preTimeStamp)
-        #     preTimeStamp = ts
+            
+        for x, y in self.database.items():
+            for i in y:
+                if i not in self.periods:
+                    self.periods[i] = [x, x]
+                else:
+                    self.periods[i][0] = max(self.periods[i][0], x - self.periods[i][1])
+                    self.periods[i][1] = x
+        for key in self.periods:
+            self.periods[key][0] = max(self.periods[key][0], abs(len(self.database) - self.periods[key][1]))
+        self.periods = {k: v[0] for k, v in self.periods.items()}
 
     def getDatabaseSize(self):
         """
         get the size of database
         :return: data base size
         """
         return len(self.database)
@@ -245,14 +247,27 @@
         va = len({key: val for key, val in fre.items() if val > 0 and val < values[0]})
         rangeFrequencies[va] = values[0]
         for i in range(1,len(values)):
             
             va = len({key: val for key, val in fre.items() if val < values[i] and val > values[i-1]})
             rangeFrequencies[va] = values[i]
         return rangeFrequencies
+    
+    def getPeriodsInRange(self):
+        fre = {k: v for k, v in sorted(self.periods.items(), key=lambda x: x[1])}
+        rangePeriods = {}
+        maximum = max([i for i in fre.values()])
+        values = [int(i*maximum/6) for i in range(1,6)]
+        #print(maximum)
+        va = len({key: val for key, val in fre.items() if val > 0 and val < values[0]})
+        rangePeriods[va] = values[0]
+        for i in range(1,len(values)):
+            va = len({key: val for key, val in fre.items() if val < values[i] and val > values[i-1]})
+            rangePeriods[va] = values[i]
+        return rangePeriods
 
     def getTransanctionalLengthDistribution(self):
         """
         get transaction length
         :return: transaction length
         """
         transactionLength = {}
@@ -269,35 +284,56 @@
         :param outputFile: output file name or path to store
         :type outputFile: str
         """
         with open(outputFile, 'w') as f:
             for key, value in data.items():
                 f.write(f'{key}\t{value}\n')
 
-    def getMinimumPeriod(self):
+    def getMinimumInterArrivalPeriod(self):
         """
-        get the minimum period
-        :return: minimum period
+        get the minimum inter arrival period
+        :return: minimum inter arrival period
         """
         return min(self.periodList)
 
-    def getAveragePeriod(self):
+    def getAverageInterArrivalPeriod(self):
         """
-        get the average period. It is sum of all period divided by number of period.
-        :return: average period
+        get the average inter arrival period. It is sum of all period divided by number of period.
+        :return: average inter arrival period
         """
         totalPeriod = sum(self.periodList)
         return totalPeriod / len(self.periodList)
 
-    def getMaximumPeriod(self):
+    def getMaximumInterArrivalPeriod(self):
         """
-        get the maximum period
-        :return: maximum period
+        get the maximum inter arrival period
+        :return: maximum inter arrival period
         """
         return max(self.periodList)
+    
+    def getMinimumPeriodOfItem(self):
+        """
+        get the minimum period of the item
+        :return: minimum period
+        """
+        return min([i for i in self.periods.values()])
+    
+    def getAveragePeriodOfItem(self):
+        """
+        get the average period of the item
+        :return: average period
+        """
+        return sum([i for i in self.periods.values()]) / len(self.periods)
+    
+    def getMaximumPeriodOfItem(self):
+        """
+        get the maximum period of the item
+        :return: maximum period
+        """
+        return max([i for i in self.periods.values()])
 
     def getStandardDeviationPeriod(self):
         """
         get the standard deviation period
         :return: standard deviation period
         """
         return statistics.pstdev(self.periodList)
@@ -312,40 +348,33 @@
    
     def printStats(self):
         print(f'Database size : {self.getDatabaseSize()}')
         print(f'Number of items : {self.getTotalNumberOfItems()}')
         print(f'Minimum Transaction Size : {self.getMinimumTransactionLength()}')
         print(f'Average Transaction Size : {self.getAverageTransactionLength()}')
         print(f'Maximum Transaction Size : {self.getMaximumTransactionLength()}')
-        print(f'Minimum period : {self.getMinimumPeriod()}')
-        print(f'Average period : {self.getAveragePeriod()}')
-        print(f'Maximum period : {self.getMaximumPeriod()}')
+        print(f'Minimum Inter Arrival Period : {self.getMinimumInterArrivalPeriod()}')
+        print(f'Average Inter Arrival Period : {self.getAverageInterArrivalPeriod()}')
+        print(f'Maximum Inter Arrival Period : {self.getMaximumInterArrivalPeriod()}')
+        print(f'Minimum periodicity : {self.getMinimumPeriodOfItem()}')
+        print(f'Average periodicity : {self.getAveragePeriodOfItem()}')
+        print(f'Maximum periodicicty : {self.getMaximumPeriodOfItem()}')
         print(f'Standard Deviation Transaction Size : {self.getStandardDeviationTransactionLength()}')
         print(f'Variance : {self.getVarianceTransactionLength()}')
         print(f'Sparsity : {self.getSparsity()}')
   
     def plotGraphs(self):
         itemFrequencies = self.getFrequenciesInRange()
         transactionLength = self.getTransanctionalLengthDistribution()
+        itemPeriods = self.getPeriodsInRange()
         #numberOfTransactionPerTimeStamp = self.getNumberOfTransactionsPerTimestamp()
-        plt.plotLineGraphFromDictionary(itemFrequencies, 100, 'Frequency', 'no of items', 'frequency')
+        plt.plotLineGraphFromDictionary(itemFrequencies, 80, 'Frequency', 'no of items', 'frequency')
+        #plt.plotLineGraphFromDictionary(itemPeriods, 50, 'Periodicity', 'no of items', 'periodicity')
         plt.plotLineGraphFromDictionary(transactionLength, 100, 'transaction length', 'transaction length', 'frequency')
         #plt.plotLineGraphFromDictionary(numberOfTransactionPerTimeStamp, 100)
 
 
 if __name__ == '__main__':
-    data = {'ts': [1, 1, 3, 4, 5, 6, 7],
-
-            'Transactions': [['a', 'd', 'e'], ['b', 'a', 'f', 'g', 'h'], ['b', 'a', 'd', 'f'], ['b', 'a', 'c'],
-                             ['a', 'd', 'g', 'k'],
-
-                             ['b', 'd', 'g', 'c', 'i'], ['b', 'd', 'g', 'e', 'j']]}
-
-    data = pd.DataFrame.from_dict(data)
-    obj = uncertainTemporalDatabaseStats('uncertain_Temporal_BMS1.csv', '\t')
-    import PAMI.extras.graph.plotLineGraphFromDictionary as plt
-
+    obj = temporalDatabaseStats(sys.argv[1], sys.argv[2])
     obj.run()
     obj.printStats()
     obj.plotGraphs()
-
-
```

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.8.1/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.8.1/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.8.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.8.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.8.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.8.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.8.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.8.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.8.1/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.8.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.8.1/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,31 +10,31 @@
         store input data as dict
 
     Methods:
     -------
     plotLineGraph()
         draw line graph of input data. input data's key is x and value is y.
     """
-    def __init__(self, data, percentage=100, title='', xlabel='', ylabel=''):
+    def __init__(self, data, end=100, start=0, title='', xlabel='', ylabel=''):
 
         """
         draw line graph. Plot the input data key as x and value as y
-        :param percentage: percentage of graph to plot
-        :type percentage: int
+        :param end: end of graph to plot
+        :type end: int
+        :param start: start fo graph to plot
+        :type start: int
         :param title: title of graph
         :type title: str
         :param xlabel: xlabel of graph
         :type xlabel: str
         :param ylabel: ylabel of grapth
         :type ylabel: str
         """
-        numberOfGraphToPlot = int(len(data) * percentage / 100)
-        x = tuple(data.keys())[:numberOfGraphToPlot]
-        y = tuple(data.values())[:numberOfGraphToPlot]
-        fig = plt.figure()
-        ax = fig.add_subplot(1, 1, 1)
+        end = int(len(data) * end / 100)
+        start = int(len(data) * start / 100)
+        x = tuple(data.keys())[start:end]
+        y = tuple(data.values())[start:end]
+        fig, ax = plt.subplots()
+        ax.plot(x, y)
         ax.set_title(title)
         ax.set_xlabel(xlabel)
-        ax.set_ylabel(ylabel)
-        ax.plot(x, y)
-        #plt.plot(x, y)
-        plt.show()
+        ax.set_ylabel(ylabel)
```

### Comparing `pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.8.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.8.1/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.8.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/plotPointOnMap.py` & `pami-2023.8.1/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.8.1/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.8.1/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,65 +4,65 @@
 
 class createSyntheticGeoreferentialTemporal:
     """
         This class create synthetic geo-referential temporal database. 
 
         Attribute:
         ----------
-        transactions : pandas.DataFrame
+        totalTransactions : int
             No of transactions
-        items : int or float
+        noOfItems : int or float
             No of items
-        avgTransaction : str
+        avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        getGeoreferentialTemporalDatabase(outputFile)
-            Create geo-referential temporal database store into outputFile
+        createGeoreferentialTemporalDatabase(outputFile)
+            Create geo-referential temporal database and store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._transactions = transactions
-        self._items = items
-        self._avgTransaction = avgTransaction
+        self._totalTransactions = transactions
+        self._noOfItems = items
+        self._avgTransactionLength = avgTransaction
     
     def createGeoreferentialTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
         count = 1
-        for i in range(self._items):
-            lat = _rd.randint(1, self._items)
-            lon = _rd.randint(1, self._items)
+        for i in range(self._noOfItems):
+            lat = _rd.randint(1, self._noOfItems)
+            lon = _rd.randint(1, self._noOfItems)
             if lat == lon:
-                lon = _rd.randint(1, self._items)
+                lon = _rd.randint(1, self._noOfItems)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._transactions):
-            length = _rd.randint(1, self._avgTransaction + 20)
+        for i in range(self._totalTransactions):
+            length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str(count)
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             count += 1
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTemporal(100000, 870, 10)
     _ap.createGeoreferentialTemporalDatabase("T10_geo_temp.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,64 +4,64 @@
 
 class createSyntheticGeoreferentialTransaction:
     """
         This class create synthetic geo-referential transaction database. 
 
         Attribute:
         ----------
-        transactions : pandas.DataFrame
+        totalTransactions : int
             No of transactions
-        items : int or float
+        items : int 
             No of items
-        avgTransaction : str
+        avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        getGeoreferentialTransactionDatabase(outputFile)
-            Create geo-referential transactional database store into outputFile
+        createGeoreferentialTransactionDatabase(outputFile)
+            Create geo-referential transactional database and store into outputFile
 
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._transactions = transactions
-        self._items = items
-        self._avgTransaction = avgTransaction
+        self._totalTransactions = transactions
+        self._noOfItems = items
+        self._avgTransactionLength = avgTransaction
     
     def createGeoreferentialTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._items):
-            lat = _rd.randint(1, self._items)
-            lon = _rd.randint(1, self._items)
+        for i in range(self._noOfItems):
+            lat = _rd.randint(1, self._noOfItems)
+            lon = _rd.randint(1, self._noOfItems)
             if lat == lon:
-                lon = _rd.randint(1, self._items)
+                lon = _rd.randint(1, self._noOfItems)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._transactions):
-            length = _rd.randint(1, self._avgTransaction + 20)
+        for i in range(self._totalTransactions):
+            length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 st = st + str(item) + '\t'
             writer.write("%s \n" % st)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialTransaction(100000, 870, 10)
     _ap.createGeoreferentialTransactionalDatabase("T10_geo.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import random as _rd
 import sys as _sys
 
 
 class createSyntheticGeoreferentialUncertainTransaction:
     """
-        This class create synthetic geo-referential uncertain transaction database. 
+        This class is to create synthetic geo-referential uncertain transaction database. 
 
         Attribute:
         ----------
-        transactions : pandas.DataFrame
+        totalTransactions : int
             No of transactions
-        items : int or float
+        noOfItems : int 
             No of items
-        avgTransaction : str
+        avgTransactionLength : int
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
         --------
-        getGeoreferentialuncertainTransactionDatabase(outputFile)
+        createGeoreferentialuncertainTransactionDatabase(outputFile)
             Create geo-referential transactional database store into outputFile
 
         Credits:
         ---------
              The complete program was written by  P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
 
 
 
 
     """
     
     def __init__(self, transactions, items, avgTransaction):
-        self._transactions = transactions
-        self._items = items
-        self._avgTransaction = avgTransaction
+        self._totalTransactions = transactions
+        self._noOfItems = items
+        self._avgTransactionLength = avgTransaction
     
     def createGeoreferentialUncertainTransactionalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
         """
         writer = open(outputFile, 'w+')
         items = []
-        for i in range(self._items):
-            lat = _rd.randint(1, self._items)
-            lon = _rd.randint(1, self._items)
+        for i in range(self._noOfItems):
+            lat = _rd.randint(1, self._noOfItems)
+            lon = _rd.randint(1, self._noOfItems)
             if lat == lon:
-                lon = _rd.randint(1, self._items)
+                lon = _rd.randint(1, self._noOfItems)
             stt = '(' + str(lat) + ' ' + str(lon) + ')'
             items.append(stt)
-        for i in range(self._transactions):
-            length = _rd.randint(1, self._avgTransaction + 20)
+        for i in range(self._totalTransactions):
+            length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str()
             st1 = str()
             for i in range(length):
                 rd = _rd.randint(0, len(items) - 1)
                 item = items[rd]
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
@@ -68,8 +68,8 @@
             writer.write("%s \n" % st1)
             
 if __name__ == "__main__":
     _ap = str()
     _ap = createSyntheticGeoreferentialUncertainTransaction(100000, 870, 10)
     _ap.createGeoreferentialUncertainTransactionalDatabase("T10_geo_un.txt")
 else:
-    print("Error! The number of input parameters do not match the total number of parameters provided")
+    print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic temporal database. 
 
         Attribute:
         ----------
         totalTransactions : int
             Total no of transactions
-        items : int 
+        noOfItems : int 
             No of items
         avgTransactionLength : int
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Methods:
@@ -29,15 +29,15 @@
 
 
     """
     
     def __init__(self, totalTransactions, items, avgTransaction):
         self._totalTransactions = totalTransactions
         self._items = items
-        self._avgTransactionLength = avgTransactionLength
+        self._avgTransactionLength = avgTransaction
     
     def createUncertainTemporalDatabase(self, outputFile):
         """
         create transactional database and return outputFileName
         :param outputFile: file name or path to store database
         :type outputFile: str
         :return: outputFile name
@@ -45,15 +45,15 @@
         writer = open(outputFile, 'w+')
         count = 1
         for i in range(self._totalTransactions):
             length = _rd.randint(1, self._avgTransactionLength + 20)
             st = str(count) + '\t'
             st1 = str()
             for i in range(length):
-                item = _rd.randint(1, self._items)
+                item = _rd.randint(1, self._noOfItems)
                 probability = _rd.uniform(0, 1)
                 st = st + str(item) + '\t'
                 st1 = st1 + str(probability) + '\t'
             writer.write("%s:" % st)
             writer.write("%s \n" % st1)
             count += 1
```

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
         This class create synthetic transaction database. 
 
         Attribute:
         ----------
         totalTransactions : int
             No of transactions
-        items : int 
+        noOfItems : int 
             No of items
         avgTransactionLength : str
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
```

### Comparing `pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py` & `pami-2023.8.1/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         ----------
         totalTransactions : int
             No of transactions
         noOfItems : int 
             No of items
         maxUtilRange: int
             Maximum utility range
-        avgTransactionLength : str
+        avgTransactionLength : int
             The length of average transaction
         outputFile: str
             Name of the output file.
 
         Nethods:
         --------
         createUtilitylDatabase(outputFile)
```

### Comparing `pami-2023.7.7/PAMI/extras/topKPatterns.py` & `pami-2023.8.1/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,31 @@
-# FT-Apriori is one of the fundamental algorithm to discover fault tolerant frequent patterns in a transactional database.
-#
+# VBFTMine is one of the fundamental algorithm to discover fault-tolerant frequent patterns in a uncertain transactional database based on bitset representation.
 #
 # **Importing this algorithm into a python program**
-# ----------------------------------------------------------------
-#
-#     from PAMI.uncertainCorrelatedPattern.basic import CFFI as alg
+# ---------------------------------------------------
 #
-#     obj = alg.CFFI("input.txt", 2, 0.4)
+# import PAMI.uncertainFaultTolerantFrequentPattern.basic.VBFTMine as alg
 #
-#     obj.startMine()
+# obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
 #
-#     Patterns = obj.getPatterns()
+# obj.startMine()
 #
-#     print("Total number of Correlated Fuzzy Frequent Patterns:", len(Patterns))
+# faultTolerantFrequentPattern = obj.getPatterns()
 #
-#     obj.savePatterns("outputFile")
+# print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPattern))
 #
-#     memUSS = obj.getMemoryUSS()
+# obj.save(oFile)
 #
-#     print("Total Memory in USS:", memUSS)
+# Df = obj.getPatternInDataFrame()
 #
-#     memRSS = obj.getMemoryRSS()
+# print("Total Memory in USS:", obj.getMemoryUSS())
 #
-#     print("Total Memory in RSS", memRSS)
+# print("Total Memory in RSS", obj.getMemoryRSS())
 #
-#     run = obj.getRuntime
-#
-#     print("Total ExecutionTime in seconds:", run)
-
+# print("Total ExecutionTime in seconds:", obj.getRuntime())
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
@@ -42,39 +36,43 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
+import numpy as _np
 from PAMI.faultTolerantFrequentPattern.basic import abstract as _ab
 
-class FTApriori(_ab._faultTolerantFrequentPatterns):
+class VBFTMine(_ab._faultTolerantFrequentPatterns):
     """
     
-    :Description:   FT-Apriori is one of the fundamental algorithm to discover fault tolerant frequent patterns in a transactional database.
-                    This program employs apriori property (or downward closure property) to  reduce the search space effectively.
-
-    :Reference:       Pei, Jian & Tung, Anthony & Han, Jiawei. (2001). Fault-Tolerant Frequent Pattern Mining: Problems and Challenges.
-
+    :Description:  VBFTMine is one of the fundamental algorithm to discover fault tolerant frequent patterns in a uncertain transactional database based on
+                   bitset representation.
+                   This program employs apriori property (or downward closure property) to  reduce the search space effectively.
+
+    :Reference:         Koh, JL., Yo, PW. (2005). An Efficient Approach for Mining Fault-Tolerant Frequent Patterns Based on Bit Vector Representations.
+                        In: Zhou, L., Ooi, B.C., Meng, X. (eds) Database Systems for Advanced Applications. DASFAA 2005. Lecture Notes in Computer Science,
+                        vol 3453. Springer, Berlin, Heidelberg. https://doi.org/10.1007/11408079_51
     :param  iFile: str :
            Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: float or int or str :
                     The user can specify minSup either in count or proportion of database size.
                     If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
                     Otherwise, it will be treated as float.
                     Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
     :param  itemSup: int or float :
                     Frequency of an item
-    :param minLength: int :
+    :param minLength: int
                     minimum length of a pattern
     :param faultTolerance: int
 
+
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
     :Attributes:
 
         startTime : float
@@ -90,70 +88,69 @@
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
         Database : list
           To store the transactions of a database in list
-    
-        
-    **Methods to execute code on terminal**
-    ---------------------------------------
-    
-            Format:
-                      >>>    python3 FTApriori.py <inputFile> <outputFile> <minSup> <itemSup> <minLength> <faultTolerance>
-            Example:
-                      >>>    python3 FTApriori.py sampleDB.txt patterns.txt 10.0 3.0 3 1
-    
-            .. note:: minSup will be considered in times of minSup and count of database transactions
-    
-    **Importing this algorithm into a python program**
-    ----------------------------------------------------------------
+
+
+    Executing the code on terminal:
+    -------------------------------
+
+        Format:
+        --------
+            >>> python3 VBFTMine.py <inputFile> <outputFile> <minSup> <itemSup> <minLength> <faultTolerance>
+
+        Examples:
+        ---------
+            >>> python3 VBFTMine.py sampleDB.txt patterns.txt 10.0 3.0 3 1  (minSup will be considered in times of minSup and count of database transactions)
+
+
+    Sample run of the importing code:
+    ---------------------------------
     .. code-block:: python
     
-            from PAMI.uncertainCorrelatedPattern.basic import CFFI as alg
-    
-            obj = alg.CFFI("input.txt", 2, 0.4)
-    
-            obj.startMine()
-    
-            Patterns = obj.getPatterns()
-    
-            print("Total number of Correlated Fuzzy Frequent Patterns:",  len(Patterns))
-    
-            obj.savePatterns("outputFile")
-    
-            memUSS = obj.getMemoryUSS()
-    
-            print("Total Memory in USS:",  memUSS)
-    
-            memRSS = obj.getMemoryRSS()
-    
-            print("Total Memory in RSS",  memRSS)
-    
-            run = obj.getRuntime
-    
-            print("Total ExecutionTime in seconds:",  run)
-    
-    **Credits:**
-    ----------------
-             The complete program was written by  P.Likhitha under the supervision of Professor Rage Uday Kiran.
+        import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
+
+        obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
+
+        obj.startMine()
+
+        faultTolerantFrequentPattern = obj.getPatterns()
+
+        print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPattern))
+
+        obj.save(oFile)
+
+        Df = obj.getPatternInDataFrame()
+
+        print("Total Memory in USS:", obj.getMemoryUSS())
+
+        print("Total Memory in RSS", obj.getMemoryRSS())
+
+        print("Total ExecutionTime in seconds:", obj.getRuntime())
+
+    Credits:
+    --------
+        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
         """
 
     _minSup = float()
     _itemSup = float()
     _minLength = int()
     _faultTolerance = int()
     _startTime = float()
     _endTime = float()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
+    _plist = []
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _mapSupport = {}
 
     def _creatingItemSets(self):
         """
@@ -184,14 +181,17 @@
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
+                            for i in temp:
+                                if i not in self._plist:
+                                    self._plist.append(i)
                             self._Database.append(set(temp))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _convert(self, value):
         """
@@ -209,113 +209,114 @@
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _Count(self, k):
-        count = 0
-        items = []
-        k = list(k)
-        n = len(k) - self._faultTolerance
-        c = _ab._itertools.combinations(k, n)
-        count = 0
-        for j in c:
-            j = list(j)
-            for i in self._Database:
-                if set(j).issubset(i):
-                    count += 1
-                    items.append(i)
-        items = list(set(map(tuple, items)))
-        return len(items), items
-
-    def _oneLengthFrequentItems(self):
-        self._mapSupport = {}
-        for li in self._Database:
-            for i in li:
-                if i not in self._mapSupport:
-                    self._mapSupport[i] = 1
-                else:
-                    self._mapSupport[i] += 1
-        self._mapSupport = {k:v for k, v in self._mapSupport.items() if v >= self._itemSup}
-
-    def _countItemSupport(self, itemset):
-        tids = {}
-        res = True
-        # for i in itemset:
-        #     for k in transactions:
-        #         if i in k:
-        #             if i not in tids:
-        #                 tids[i] = 1
-        #             else:
-        #                 tids[i] += 1
+    def _Count(self, tids):
         count = 0
-        for x in self._Database:
-            print(x, itemset, set(x) & set(itemset), abs(len(itemset) - len(set(x) & set(itemset))))
-            if abs(len(itemset) - len(set(x) & set(itemset))) <= self._faultTolerance:
+        for i in tids:
+            if i == 1:
                 count += 1
-        # for x, y in tids.items():
-        #     if y < self._itemSup:
-        #         res = False
         return count
 
-    def _getFaultPatterns(self):
-        l = [k for k, v in self._mapSupport.items()]
-        for i in range(0, len(l)+1):
-            c = _ab._itertools.combinations(l, i)
-            for j in c:
-                #support, items = self._Count(j)
-                #print(support, items)
-                res = self._countItemSupport(j)
-                print(j, res)
-                if len(j) >= self._minLength and res >= self._minSup:
-                    self._finalPatterns[tuple(j)] = res
+    def _save(self, prefix, suffix, tidsetx):
+        if (prefix == None):
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        prefix = list(set(prefix))
+        prefix.sort()
+        val = self._Count(tidsetx)
+        if len(prefix) > self._faultTolerance:
+            self._finalPatterns[tuple(prefix)] = val
+
+    def _processEquivalenceClass(self, prefix, itemsets, tidsets):
+        if (len(itemsets) == 1):
+            i = itemsets[0]
+            tidi = tidsets[0]
+            self._save(prefix, [i], tidi)
+            return
+        for i in range(len(itemsets)):
+            itemx = itemsets[i]
+            if (itemx == None):
+                continue
+            tidsetx = tidsets[i]
+            classItemsets = []
+            classtidsets = []
+            itemsetx = [itemx]
+            for j in range(i + 1, len(itemsets)):
+                itemj = itemsets[j]
+                tidsetj = tidsets[j]
+                y = list(_np.array(tidsetx) & _np.array(tidsetj))
+                total = self._Count(y)
+                if total >= self._minSup:
+                    classItemsets.append(itemj)
+                    classtidsets.append(y)
+            if (len(classItemsets) > 0):
+                newprefix = list(set(itemsetx)) + prefix
+                self._processEquivalenceClass(newprefix, classItemsets, classtidsets)
+            self._save(prefix, list(set(itemsetx)), tidsetx)
+
+    def _oneLengthFrequentItems(self):
+        """ To calculate the one Length items"""
+        Vector = {}
+        items = []
+        for i in self._Database:
+            for j in self._plist:
+                count = 0
+                if j in i:
+                    count = 1
+                if j in Vector:
+                    Vector[j].append(count)
+                else:
+                    Vector[j] = [count]
+        for x, y in Vector.items():
+            v = self._Count(y)
+            if v >= self._itemSup:
+                items.append(x)
+        return Vector, items
 
     def startMine(self):
         """
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         self._itemSup = self._convert(self._itemSup)
         self._minLength = int(self._minLength)
         self._faultTolerance = int(self._faultTolerance)
-        self._oneLengthFrequentItems()
-        #l = [k for k, v in self._mapSupport.items()]
-        # for i in range(len(l)):
-        #     for j in range(i + 1, len(l)):
-        #         x, y = l[i], l[j]
-        #         li = [x, y]
-        #         count = 0
-        #         tids = {x: 0, y: 0}
-        #         for k in self._Database:
-        #             if x in k and y in k:
-        #                 count += 1
-        #             if x in k and y not in k:
-        #                 count += 1
-        #             if x not in k and y in k:
-        #                 count += 1
-        #         # re = True
-        #         # for x, y in tids.items():
-        #         #     if y < self._itemSup:
-        #         #         re = False
-        #         print(li, count)
-        #     if len(li) > self._faultTolerance:
-        #         self._finalPatterns[tuple(li)] = count
-        self._getFaultPatterns()
+        Vector, plist = self._oneLengthFrequentItems()
+        for i in range(len(plist)):
+            itemx = plist[i]
+            tidsetx = Vector[itemx]
+            itemsetx = [itemx]
+            itemsets = []
+            tidsets = []
+            for j in range(i + 1, len(plist)):
+                itemj = plist[j]
+                tidsetj = Vector[itemj]
+                y1 = list(_np.array(tidsetx) | _np.array(tidsetj))
+                total = self._Count(y1)
+                if total >= self._minSup:
+                    itemsets.append(itemj)
+                    tidsets.append(y1)
+            if (len(itemsets) > 0):
+                self._processEquivalenceClass(itemsetx, itemsets, tidsets)
+            self._save(None, itemsetx, tidsetx)
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Fault-Tolerant Frequent patterns were generated successfully using FTApriori algorithm ")
+        print("Fault-Tolerant Frequent patterns were generated successfully using VBFTMine algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
@@ -355,14 +356,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             s = str()
             for i in a:
                 s = s + i + ' '
             data.append([s, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
@@ -383,33 +385,33 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of Fault-Tolerant Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 7 or len(_ab._sys.argv) == 8:
         if len(_ab._sys.argv) == 8:
-            _ap = FTApriori(_ab._sys.argv[1], _ab._sys.argv[3],  _ab._sys.argv[4],
+            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3],  _ab._sys.argv[4],
                             _ab._sys.argv[5], _ab._sys.argv[6], _ab._sys.argv[7],)
         if len(_ab._sys.argv) == 7:
-            _ap = FTApriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = FTApriori('/Users/Likhitha/Downloads/fault/sample4.txt', 5, 3, 2, 1, ' ')
+        _ap = VBFTMine('/Users/Likhitha/Downloads/fault/sample4.txt', 5, 3, 2, 1, ' ')
         _ap.startMine()
         _ap.printResults()
         print(_ap.getPatternsAsDataFrame())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+# FTFPGrowth algorithm aims to discover all fault-tolerant frequent patterns that may exist in a transactional database.
+#
 # **Importing this algorithm into a python program**
 # --------------------------------------------------
 #
-#     from PAMI.frequentPattern.basic import FPGrowth as alg
+#     from PAMI.faultTolerantFrequentPattern.basic import FTFPGrowth as alg
 #
-#     obj = alg.FPGrowth(iFile, minSup)
+#     obj = alg.FTFPGrowth(inputFile,minSup,itemSup,minLength,faultTolerance)
 #
 #     obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#     faultTolerantFrequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of fault-tolerant frequent patterns:", len(faultTolerantFrequentPatterns))
 #
 #     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
@@ -85,15 +87,15 @@
         self.parent = None
         self.children = children
 
     def addChild(self, node):
         """
             Retrieving the child from the tree
 
-            :param node: Children node
+            :param node: Child Node
             :type node: Node
             :return: Updates the children nodes and parent nodes
 
         """
         self.children[node.itemId] = node
         node.parent = self
 
@@ -128,15 +130,15 @@
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
     def addTransaction(self, transaction, count):
         """adding transaction into tree
 
-        :param transaction: it represents the one transactions in database
+        :param transaction: it represents the one transaction in database
 
         :type transaction: list
 
         :param count: frequency of item
 
         :type count: int
         """
@@ -247,15 +249,15 @@
 
 class FTFPGrowth(_fp._faultTolerantFrequentPatterns):
     """
     Description:
     ------------
        FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database.
        It stores the database in compressed fp-tree decreasing the memory usage and extracts the
-       patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+       patterns from tree.It employs downward closure property to  reduce the search space effectively.
 
     Reference :
     ---------
        Han, J., Pei, J., Yin, Y. et al. Mining Frequent Patterns without Candidate Generation: A Frequent-Pattern
        Tree Approach. Data  Mining and Knowledge Discovery 8, 53–87 (2004). https://doi.org/10.1023
 
     Attributes :
@@ -294,15 +296,15 @@
     Methods :
     -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
+            Complete set of frequent patterns will be loaded in to an output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
@@ -324,23 +326,23 @@
 
 
 
     Sample run of the importing code:
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.frequentPattern.basic import FPGrowth as alg
+        from PAMI.faultTolerantFrequentPattern.basic import FTFPGrowth as alg
 
-        obj = alg.FPGrowth(iFile, minSup)
+        obj = alg.FTFPGrowth(inputFile,minSup,itemSup,minLength,faultTolerance)
 
         obj.startMine()
 
-        frequentPatterns = obj.getPatterns()
+        patterns = obj.getPatterns()
 
-        print("Total number of Frequent Patterns:", len(frequentPatterns))
+        print("Total number of Frequent Patterns:", len(patterns))
 
         obj.save(oFile)
 
         Df = obj.getPatternInDataFrame()
 
         memUSS = obj.getMemoryUSS()
 
@@ -590,15 +592,15 @@
         data = []
         for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py` & `pami-2023.8.1/PAMI/frequentPattern/topk/FAE.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-# VBFTMine is one of the fundamental algorithm to discover fault tolerant frequent patterns in a uncertain transactional database based on bitset representation.
+
+
+# Top - K is and algorithm to discover top frequent patterns in a transactional database.
 #
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------
+# ---------------------------------------------------------
+#
+#         import PAMI.frequentPattern.topK.FAE as alg
+#
+#         obj = alg.FAE(iFile, K)
 #
-# import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
+#         obj.startMine()
 #
-# obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
+#         topKFrequentPatterns = obj.getPatterns()
 #
-# obj.startMine()
+#         print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 #
-# faultTolerantFrequentPatterns = obj.getPatterns()
+#         obj.save(oFile)
 #
-# print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
+#         Df = obj.getPatternInDataFrame()
 #
-# obj.save(oFile)
+#         memUSS = obj.getMemoryUSS()
 #
-# Df = obj.getPatternInDataFrame()
+#         print("Total Memory in USS:", memUSS)
 #
-# print("Total Memory in USS:", obj.getMemoryUSS())
+#         memRSS = obj.getMemoryRSS()
 #
-# print("Total Memory in RSS", obj.getMemoryRSS())
+#         print("Total Memory in RSS", memRSS)
 #
-# print("Total ExecutionTime in seconds:", obj.getRuntime())
+#         run = obj.getRuntime()
+#
+#         print("Total ExecutionTime in seconds:", run)
 
+#
+#
+#
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -36,47 +47,35 @@
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-import numpy as _np
-from PAMI.faultTolerantFrequentPattern.basic import abstract as _ab
+from PAMI.frequentPattern.topk import abstract as _ab
 
-class VBFTMine(_ab._faultTolerantFrequentPatterns):
+
+class FAE(_ab._frequentPatterns):
     """
-    
-    :Description:  VBFTMine is one of the fundamental algorithm to discover fault tolerant frequent patterns in a uncertain transactional database based on
-                   bitset representation.
-                   This program employs apriori property (or downward closure property) to  reduce the search space effectively.
-
-    :Reference:         Koh, JL., Yo, PW. (2005). An Efficient Approach for Mining Fault-Tolerant Frequent Patterns Based on Bit Vector Representations.
-                        In: Zhou, L., Ooi, B.C., Meng, X. (eds) Database Systems for Advanced Applications. DASFAA 2005. Lecture Notes in Computer Science,
-                        vol 3453. Springer, Berlin, Heidelberg. https://doi.org/10.1007/11408079_51
+    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
+
+
+    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
+                  https://ieeexplore.ieee.org/document/4370261
     :param  iFile: str :
-           Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
-    :param  minSup: float or int or str :
-                    The user can specify minSup either in count or proportion of database size.
-                    If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-                    Otherwise, it will be treated as float.
-                    Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-    :param  itemSup: int or float :
-                    Frequency of an item
-    :param minLength: int
-                    minimum length of a pattern
-    :param faultTolerance: int
-
-
+    :param  k: int :
+                    User specified count of top frequent patterns
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
 
+
     :Attributes:
 
         startTime : float
           To record the start time of the mining process
 
         endTime : float
           To record the completion time of the mining process
@@ -86,244 +85,271 @@
 
         memoryUSS : float
           To store the total amount of USS memory consumed by the program
 
         memoryRSS : float
           To store the total amount of RSS memory consumed by the program
 
-        Database : list
-          To store the transactions of a database in list
+        finalPatterns : dict
+            it represents to store the patterns
 
 
-    Executing the code on terminal:
-    -------------------------------
+    **Methods to execute code on terminal**
+    ----------------------------------------
 
         Format:
-        --------
-            >>> python3 VBFTMine.py <inputFile> <outputFile> <minSup> <itemSup> <minLength> <faultTolerance>
+
+           >>> python3 FAE.py <inputFile> <outputFile> <K>
 
         Examples:
-        ---------
-            >>> python3 VBFTMine.py sampleDB.txt patterns.txt 10.0 3.0 3 1  (minSup will be considered in times of minSup and count of database transactions)
+
+           >>> python3 FAE.py sampleDB.txt patterns.txt 10
 
 
-    Sample run of the importing code:
-    ---------------------------------
+    **Importing this algorithm into a python program**
+    ---------------------------------------------------------
     .. code-block:: python
-    
-        import PAMI.faultTolerantFrequentPattern.basic.VBFTMine as alg
 
-        obj = alg.VBFTMine(iFile, minSup, itemSup, minLength, faultTolerance)
+        import PAMI.frequentPattern.topK.FAE as alg
+
+        obj = alg.FAE(iFile, K)
 
         obj.startMine()
 
-        faultTolerantFrequentPatterns = obj.getPatterns()
+        topKFrequentPatterns = obj.getPatterns()
 
-        print("Total number of Fault Tolerant Frequent Patterns:", len(faultTolerantFrequentPatterns))
+        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
 
         obj.save(oFile)
 
         Df = obj.getPatternInDataFrame()
 
-        print("Total Memory in USS:", obj.getMemoryUSS())
+        memUSS = obj.getMemoryUSS()
+
+        print("Total Memory in USS:", memUSS)
 
-        print("Total Memory in RSS", obj.getMemoryRSS())
+        memRSS = obj.getMemoryRSS()
 
-        print("Total ExecutionTime in seconds:", obj.getRuntime())
+        print("Total Memory in RSS", memRSS)
+
+        run = obj.getRuntime()
+
+        print("Total ExecutionTime in seconds:", run)
 
     Credits:
     --------
         The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
-        """
+    """
 
-    _minSup = float()
-    _itemSup = float()
-    _minLength = int()
-    _faultTolerance = int()
     _startTime = float()
     _endTime = float()
+    _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _plist = []
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _mapSupport = {}
+    _tidList = {}
+    _minimum = int()
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
-
         """
+
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            temp = []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                temp = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
 
-            for k in temp:
-                self._Database.append(set(k))
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._Database.append(set(temp))
+                    self._Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            for i in temp:
-                                if i not in self._plist:
-                                    self._plist.append(i)
-                            self._Database.append(set(temp))
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def _convert(self, value):
+    def _frequentOneItem(self):
+        """
+        Generating one frequent patterns
+        """
+        candidate = {}
+        self._tidList = {}
+        for i in range(len(self._Database)):
+            for j in self._Database[i]:
+                if j not in candidate:
+                    candidate[j] = 1
+                    self._tidList[j] = [i]
+                else:
+                    candidate[j] += 1
+                    self._tidList[j].append(i)
+        self._finalPatterns = {}
+        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+        for i in plist:
+            if len(self._finalPatterns) >= self._k:
+                break
+            else:
+                self._finalPatterns[i] = candidate[i]
+        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+        plist = list(self._finalPatterns.keys())
+        return plist
+
+    def _save(self, prefix, suffix, tidSetI):
+        """Saves the patterns that satisfy the periodic frequent property.
+
+            :param prefix: the prefix of a pattern
+            :type prefix: list
+            :param suffix: the suffix of a patterns
+            :type suffix: list
+            :param tidSetI: the timestamp of a patterns
+            :type tidSetI: list
         """
-        To convert the user specified minSup value
 
-        :param value: user specified minSup value
+        if prefix is None:
+            prefix = suffix
+        else:
+            prefix = prefix + suffix
+        val = len(tidSetI)
+        sample = str()
+        for i in prefix:
+            sample = sample + i + "\t"
+        if len(self._finalPatterns) < self._k:
+            if val > self._minimum:
+                self._finalPatterns[sample] = val
+                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
+                self._minimum = min([i for i in self._finalPatterns.values()])
+        else:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
+                if val > y:
+                    del self._finalPatterns[x]
+                    self._finalPatterns[sample] = val
+                    self._finalPatterns = {k: v for k, v in
+                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
+                                                     reverse=True)}
+                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    return
+
+    def _Generation(self, prefix, itemSets, tidSets):
+        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
+
+            :param prefix:  main equivalence prefix
+            :type prefix: periodic-frequent item or pattern
+            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
+                            and frequent with their timestamps
+            :type itemSets: list
+            :param tidSets: timestamps of the items in the argument itemSets
+            :type tidSets: list
+
+
+                    """
+        if len(itemSets) == 1:
+            i = itemSets[0]
+            tidI = tidSets[0]
+            self._save(prefix, [i], tidI)
+            return
+        for i in range(len(itemSets)):
+            itemI = itemSets[i]
+            if itemI is None:
+                continue
+            tidSetI = tidSets[i]
+            classItemSets = []
+            classTidSets = []
+            itemSetX = [itemI]
+            for j in range(i + 1, len(itemSets)):
+                itemJ = itemSets[j]
+                tidSetJ = tidSets[j]
+                y = list(set(tidSetI).intersection(tidSetJ))
+                if len(y) >= self._minimum:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
+            newPrefix = list(set(itemSetX)) + prefix
+            self._Generation(newPrefix, classItemSets, classTidSets)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
+    def _convert(self, value):
+        """
+        to convert the type of user specified minSup value
+        :param value: user specified minSup value
         :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
-                value = (len(self._Database) * value)
+                value = ((len(self._Database)) * value)
             else:
                 value = int(value)
         return value
 
-    def _Count(self, tids):
-        count = 0
-        for i in tids:
-            if i == 1:
-                count += 1
-        return count
-
-    def _save(self, prefix, suffix, tidsetx):
-        if (prefix == None):
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        prefix = list(set(prefix))
-        prefix.sort()
-        val = self._Count(tidsetx)
-        if len(prefix) > self._faultTolerance:
-            self._finalPatterns[tuple(prefix)] = val
-
-    def _processEquivalenceClass(self, prefix, itemsets, tidsets):
-        if (len(itemsets) == 1):
-            i = itemsets[0]
-            tidi = tidsets[0]
-            self._save(prefix, [i], tidi)
-            return
-        for i in range(len(itemsets)):
-            itemx = itemsets[i]
-            if (itemx == None):
-                continue
-            tidsetx = tidsets[i]
-            classItemsets = []
-            classtidsets = []
-            itemsetx = [itemx]
-            for j in range(i + 1, len(itemsets)):
-                itemj = itemsets[j]
-                tidsetj = tidsets[j]
-                y = list(_np.array(tidsetx) & _np.array(tidsetj))
-                total = self._Count(y)
-                if total >= self._minSup:
-                    classItemsets.append(itemj)
-                    classtidsets.append(y)
-            if (len(classItemsets) > 0):
-                newprefix = list(set(itemsetx)) + prefix
-                self._processEquivalenceClass(newprefix, classItemsets, classtidsets)
-            self._save(prefix, list(set(itemsetx)), tidsetx)
-
-    def _oneLengthFrequentItems(self):
-        """ To calculate the one Length items"""
-        Vector = {}
-        items = []
-        for i in self._Database:
-            for j in self._plist:
-                count = 0
-                if j in i:
-                    count = 1
-                if j in Vector:
-                    Vector[j].append(count)
-                else:
-                    Vector[j] = [count]
-        for x, y in Vector.items():
-            v = self._Count(y)
-            if v >= self._itemSup:
-                items.append(x)
-        return Vector, items
-
     def startMine(self):
         """
-            Frequent pattern mining process will start from here
+            Main function of the program
+
         """
-        self._Database = []
         self._startTime = _ab._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._k is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
-        self._itemSup = self._convert(self._itemSup)
-        self._minLength = int(self._minLength)
-        self._faultTolerance = int(self._faultTolerance)
-        Vector, plist = self._oneLengthFrequentItems()
+        self._k = self._convert(self._k)
+        plist = self._frequentOneItem()
         for i in range(len(plist)):
-            itemx = plist[i]
-            tidsetx = Vector[itemx]
-            itemsetx = [itemx]
-            itemsets = []
-            tidsets = []
+            itemI = plist[i]
+            tidSetI = self._tidList[itemI]
+            itemSetX = [itemI]
+            itemSets = []
+            tidSets = []
             for j in range(i + 1, len(plist)):
-                itemj = plist[j]
-                tidsetj = Vector[itemj]
-                y1 = list(_np.array(tidsetx) | _np.array(tidsetj))
-                total = self._Count(y1)
-                if total >= self._minSup:
-                    itemsets.append(itemj)
-                    tidsets.append(y1)
-            if (len(itemsets) > 0):
-                self._processEquivalenceClass(itemsetx, itemsets, tidsets)
-            self._save(None, itemsetx, tidsetx)
+                itemJ = plist[j]
+                tidSetJ = self._tidList[itemJ]
+                y1 = list(set(tidSetI).intersection(tidSetJ))
+                if len(y1) >= self._minimum:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
+            self._Generation(itemSetX, itemSets, tidSets)
+        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Fault-Tolerant Frequent patterns were generated successfully using VBFTMine algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-        :return: returning USS memory consumed by the mining process
+                    :return: returning USS memory consumed by the mining process
 
-        :rtype: float
+                    :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
@@ -351,67 +377,59 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            s = str()
-            for i in a:
-                s = s + i + ' '
-            data.append([s, b])
+            data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
-        # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s = str()
-            for i in x:
-                s = s + i + '\t'
-            s1 = s.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+            patternsAndSupport = x.strip() + ":" + str(y)
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
-        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+    def printTOPK(self):
+        """ this function is used to print the results
+        """
+        print("Top K Frequent  Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 7 or len(_ab._sys.argv) == 8:
-        if len(_ab._sys.argv) == 8:
-            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3],  _ab._sys.argv[4],
-                            _ab._sys.argv[5], _ab._sys.argv[6], _ab._sys.argv[7],)
-        if len(_ab._sys.argv) == 7:
-            _ap = VBFTMine(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
+        if len(_ab._sys.argv) == 5:
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = VBFTMine('/Users/Likhitha/Downloads/fault/sample4.txt', 5, 3, 2, 1, ' ')
-        _ap.startMine()
-        _ap.printResults()
-        print(_ap.getPatternsAsDataFrame())
         print("Error! The number of input parameters do not match the total number of parameters provided")
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/closed/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,32 +22,29 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-import functools as _functools
-import itertools as _itertools
 
 
-class _faultTolerantFrequentPatterns(_ABC):
+class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
@@ -88,15 +85,15 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, itemSup, minLength, faultTolerance, sep="\t"):
+    def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -104,27 +101,20 @@
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._itemSup = itemSup
-        self._minLength = minLength
-        self._faultTolerance = faultTolerance
         self._finalPatterns = {}
         self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
-
-        """Variable to store USS memory consumed by the program"""
-
-
+        self._memoryRSS = float()
+        self._memoryUSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -158,12 +148,19 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
+
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
+
+    @_abstractmethod
+    def printResults(self):
+        """ To print results of the execution."""
+
+        pass
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/__init__.py` & `pami-2023.8.1/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/Apriori.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -282,35 +282,35 @@
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using Apriori algorithm ")
 
-    def getMemoryUSS(self):
+    def getMemoryUSS(self) -> float:
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self):
+    def getMemoryRSS(self) -> float:
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self):
+    def getRuntime(self) -> float:
         """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
@@ -329,15 +329,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -351,29 +351,33 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """
+        this function is used to print the result
+
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = Apriori(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = Apriori(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_ap._sys.argv) == 4 or len(_ap._sys.argv) == 5:
+        if len(_ap._sys.argv) == 5:
+            _ap = Apriori(_ap._sys.argv[1], _ap._sys.argv[3], _ap._sys.argv[4])
+        if len(_ap._sys.argv) == 4:
+            _ap = Apriori(_ap._sys.argv[1], _ap._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
+        _ap.save(_ap._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -54,15 +54,15 @@
 
     :Description: ECLAT is one of the fundamental algorithm to discover frequent patterns in a transactional database.
 
     :Reference:  Mohammed Javeed Zaki: Scalable Algorithms for Association Mining. IEEE Trans. Knowl. Data Eng. 12(3):
             372-390 (2000), https://ieeexplore.ieee.org/document/846291
 
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
 
@@ -271,35 +271,35 @@
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
         print("Frequent patterns were generated successfully using ECLAT algorithm")
 
-    def getMemoryUSS(self):
+    def getMemoryUSS(self) -> float:
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryUSS
 
-    def getMemoryRSS(self):
+    def getMemoryRSS(self) -> float:
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
         :return: returning RSS memory consumed by the mining process
 
         :rtype: float
         """
 
         return self._memoryRSS
 
-    def getRuntime(self):
+    def getRuntime(self) -> float:
         """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
@@ -317,15 +317,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -339,14 +339,17 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """Function used to print the results
+
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """
     :Description:   ECLATDiffset uses diffset to extract the frequent patterns in a transactional database.
 
     :Reference:  KDD '03: Proceedings of the ninth ACM SIGKDD international conference on Knowledge discovery and data mining
             August 2003 Pages 326–335 https://doi.org/10.1145/956750.956788
             
     :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
+                   Name of the Input file to mine complete set of frequent pattern's
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
                    The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
     :param  sep: str :
                    This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
      
@@ -329,15 +329,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b[0]])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -336,16 +336,16 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
-        :param outFile: name of the output file
+        """Complete set of frequent patterns will be loaded in to an output file
+        :param outFile: name of the outputfile
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
@@ -354,14 +354,16 @@
         """ Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """ this function is used to print the result
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 if __name__=="__main__":
     _ap = str()
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+# FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It  employs downward closure property to  reduce the search space effectively.
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #     from PAMI.frequentPattern.basic import FPGrowth as alg
 #
 #     obj = alg.FPGrowth(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -131,15 +131,15 @@
         self.root = _Node(None, {})
         self.summaries = {}
         self.info = {}
 
     def addTransaction(self, transaction, count):
         """adding transaction into tree
 
-        :param transaction: it represents the one transactions in database
+        :param transaction: it represents the one transaction in database
 
         :type transaction: list
 
         :param count: frequency of item
 
         :type count: int
         """
@@ -247,15 +247,15 @@
                 for q in conditionalTree.generatePatterns(pattern):
                     yield q
 
 
 class FPGrowth(_fp._frequentPatterns):
     """
 
-    :Description:   FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+    :Description:   FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 
     :Reference:  Han, J., Pei, J., Yin, Y. et al. Mining Frequent Patterns without Candidate Generation: A Frequent-Pattern
            Tree Approach. Data  Mining and Knowledge Discovery 8, 53–87 (2004). https://doi.org/10.1023
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
@@ -575,15 +575,15 @@
         data = []
         for a, b in self.__finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.8.1/PAMI/frequentPattern/closed/CHARM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# CHARM is an algorithm to discover closed frequent patterns in a transactional database. Closed frequent patterns are patterns if there exists no superset that has the same support count as this original itemset. This algorithm employs depth-first search technique to find the complete set of closed frequent patterns in a
+# CHARM is an algorithm to discover closed frequent patterns in a transactional database. Closed frequent patterns are patterns if there exists no superset that has the same support count as this original itemset . This algorithm employs depth-first search technique to find the complete set of closed frequent patterns in a
 #
 #  **Importing this algorithm into a python program**
 #  --------------------------------------------------------------
 #
 #
-#             from PAMI.frequentPattern.closed import closed as alg
+#             from PAMI.frequentPattern.closed import CHARM as alg
 #
-#             obj = alg.Closed(iFile, minSup)
+#             obj = alg.CHARM(iFile, minSup)
 #
 #             obj.startMine()
 #
 #             frequentPatterns = obj.getPatterns()
 #
 #             print("Total number of Closed Frequent Patterns:", len(frequentPatterns))
 #
@@ -120,17 +120,17 @@
             .. note:: minSup will be considered in percentage of database transactions
 
 
     **Importing this algorithm into a python program**
     --------------------------------------------------------------
     .. code-block:: python
 
-            from PAMI.frequentPattern.closed import closed as alg
+            from PAMI.frequentPattern.closed import CHARM as alg
 
-            obj = alg.Closed(iFile, minSup)
+            obj = alg.CHARM(iFile, minSup)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Closed Frequent Patterns:", len(frequentPatterns))
 
@@ -349,15 +349,14 @@
 
             :type itemSets: list
 
             :param tidSets: timestamps of the items in the argument itemSets
 
             :type tidSets: list
 
-
         """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
         if len(itemSets) == 2:
@@ -501,15 +500,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -524,14 +523,16 @@
 
         :rtype: dict
         """
 
         return self._finalPatterns
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Closed Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/maximal/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         self._finalPatterns = {}
         self._oFile = str()
         self._startTime = float()
         self._endTime = float()
         self._memoryRSS = float()
         self._memoryUSS = float()
 
+
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
@@ -157,10 +158,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print results of the execution."""
+        """To print the statistics."""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py` & `pami-2023.8.1/PAMI/frequentPattern/cuda/cuApriori.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -154,31 +154,15 @@
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
 
-    _sumKernel = _ab._cp.RawKernel(r'''
 
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
-
-    ''', 'sumKernel')
 
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
@@ -231,15 +215,23 @@
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
     
-    def arraysAndItems(self):
+    def _arraysAndItems(self):
+        """ 
+        Convert the items into arrays for cupy and store them in a dictionary variable
+
+        :return: dictionary variable
+        
+        """
+
+
         ArraysAndItems = {}
 
         for i in range(len(self._Database)):
             for j in self._Database[i]:
                 j = tuple([j])
                 if j not in ArraysAndItems:
                     ArraysAndItems[j] = [i]
@@ -262,15 +254,15 @@
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
 
-        ArraysAndItems = self.arraysAndItems()
+        ArraysAndItems = self._arraysAndItems()
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 # print(i, "/", len(ArraysAndItems), end="\r")
@@ -337,15 +329,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -359,14 +351,17 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """
+        this function is used to print results
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in s:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py` & `pami-2023.8.1/PAMI/frequentPattern/cuda/cuAprioriBit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -357,15 +357,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -379,14 +379,15 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """this function is used to print the result"""
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py` & `pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclat.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,32 +154,14 @@
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
 
-    _sumKernel = _ab._cp.RawKernel(r'''
-
-    #define uint32_t unsigned int
-
-    extern "C" __global__
-
-    void sumKernel(uint32_t *d_a, uint32_t *sum, uint32_t numElements)
-    {
-        uint32_t i = blockDim.x * blockIdx.x + threadIdx.x;
-        if (i < numElements)
-        {  
-            atomicAdd(&sum[0], __popc(d_a[i]));
-        }
-        return;    
-    }
-
-    ''', 'sumKernel')
-
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
 
         """
@@ -231,15 +213,21 @@
             if '.' in value:
                 value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
     
-    def arraysAndItems(self):
+    def _arraysAndItems(self):
+        """ 
+        Convert the items into arrays for cupy and store them in a dictionary variable
+
+        :return: dictionary variable
+        
+        """
         ArraysAndItems = {}
 
         for i in range(len(self._Database)):
             for j in self._Database[i]:
                 j = tuple([j])
                 if j not in ArraysAndItems:
                     ArraysAndItems[j] = [i]
@@ -262,15 +250,15 @@
             Frequent pattern mining process will start from here
         """
         self._Database = []
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
 
-        ArraysAndItems = self.arraysAndItems()
+        ArraysAndItems = self._arraysAndItems()
 
         while len(ArraysAndItems) > 0:
             # print("Total number of ArraysAndItems:", len(ArraysAndItems))
             newArraysAndItems = {}
             keys = list(ArraysAndItems.keys())
             for i in range(len(ArraysAndItems)):
                 iList = list(keys[i])
@@ -342,15 +330,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -364,14 +352,16 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in s:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py` & `pami-2023.8.1/PAMI/frequentPattern/cuda/cuEclatBit.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -362,15 +362,15 @@
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         # dataFrame = dataFrame.replace(r'\r+|\n+|\t+',' ', regex=True)
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -384,14 +384,16 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
+        """ this function is used to print the result
+        """
         print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.8.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns("patterns")
+#     obj.save("patterns")
 #
 #     Df = obj.getPatternsAsDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -27,18 +27,14 @@
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 #
 #
 
-
-#
-#
-#
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -593,15 +589,15 @@
                 list2.sort()
                 list1.append(list2)
         return list1
 
     @staticmethod
     def _buildTree(data, info):
         """
-        creating the root node as null in fp-tree and and adding all transactions into tree.
+        creating the root node as null in fp-tree and adding all transactions into tree.
         :param data: updated transactions
         :param info: rank of items in transactions
         :return: fp-tree
         """
         rootNode = _Tree()
         rootNode.info = info.copy()
         for i in range(len(data)):
@@ -720,15 +716,15 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
@@ -742,14 +738,18 @@
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
     
     def printResults(self):
+        """
+         this function is used to print the results
+
+        """
         print('Total number of Maximal Frequent Patterns: ' + str(self.getPatterns()))
         print('Runtime: ' + str(self.getRuntime()))
         print('Memory (RSS): ' + str(self.getMemoryRSS()))
         print('Memory (USS): ' + str(self.getMemoryUSS()))
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.8.1/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.8.1/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _defaultdict
+from collections import defaultdict as _dd
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
+import resource as _resource
+import math as _math
 import sys as _sys
-import validators as _validators
-from urllib.request import urlopen as _urlopen
 
 
 class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
@@ -88,34 +88,33 @@
             This function outputs the total runtime of a mining algorithm
 
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
+        :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._finalPatterns = {}
         self._oFile = str()
+        self._finalPatterns = {}
         self._startTime = float()
         self._endTime = float()
-        self._memoryRSS = float()
         self._memoryUSS = float()
-
+        self._memoryRSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -149,19 +148,12 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
-
-    @_abstractmethod
-    def printResults(self):
-        """To print the statistics."""
-
-        pass
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
 
 class _frequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
             employ in PAMI
+
            Attributes:
            ----------
             iFile : str
                 Input file name or path of the input file
             minSup: integer or float or str
                 The user can specify minSup either in count or proportion of database size.
                 If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
@@ -38,14 +39,15 @@
                 Storing the complete set of patterns in a dictionary variable
             oFile : str
                 Name of the output file to store complete set of frequent patterns
             memoryUSS : float
                 To store the total amount of USS memory consumed by the program
             memoryRSS : float
                 To store the total amount of RSS memory consumed by the program
+
            Methods:
            -------
             startMine()
                 Calling this function will start the actual mining process
             getPatterns()
                 This function will output all interesting patterns discovered by an algorithm
             save(oFile)
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Parallel Apriori is an algorithm to discover frequent patterns in a transactional database. This program employs parallel apriori property (or downward closure property) to  reduce the search space effectively.
-
 #
 #
 #  **Importing this algorithm into a python program**
 #  ---------------------------------------------------
 #
 #         import PAMI.frequentPattern.pyspark.parallelApriori as alg
 #
@@ -11,30 +10,29 @@
 #
 #         obj.startMine()
 #
 #         frequentPatterns = obj.getPatterns()
 #
 #         print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#         obj.savePatterns(oFile)
+#         obj.save(oFile)
 #
 #         Df = obj.getPatternInDataFrame()
 #
 #         memUSS = obj.getMemoryUSS()
 #
 #         print("Total Memory in USS:", memUSS)
 #
 #         memRSS = obj.getMemoryRSS()
 #
 #         print("Total Memory in RSS", memRSS)
 #
 #         run = obj.getRuntime()
 #
 #         print("Total ExecutionTime in seconds:", run)
-
 #
 #
 #
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
@@ -139,16 +137,15 @@
                 run = obj.getRuntime()
     
                 print("Total ExecutionTime in seconds:", run)
     
     
     **Credits:**
     -----------------------------------------
-    
-             The complete program was written by Yudai Masu  under the supervision of Professor Rage Uday Kiran.
+            The complete program was written by Yudai Masu  under the supervision of Professor Rage Uday Kiran.
 
 
     """
 
     _minSup = float()
     _startTime = float()
     _endTime = float()
@@ -197,17 +194,17 @@
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def savePatterns(self, outFile):
+    def save(self, outFile):
         """
-        Complete set of frequent patterns will be loaded in to a output file
+        Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = str(x) + " : " + str(y)
@@ -216,14 +213,23 @@
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
+    
+    def printResults(self):
+        """
+        This method prints all the statistics
+        """
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
     @staticmethod
     def _Mapper(transaction, candidateItemsets):
         """
         Map each candidate itemset of candidateItemsets to (itemset,1) if a candidate itemset is in transaction
 
         :param transaction: a transaction of database
@@ -360,8 +366,7 @@
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
 
-
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -194,35 +194,51 @@
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def savePatterns(self, outFile):
+    def save(self, outFile):
         """
-        Complete set of frequent patterns will be loaded in to a output file
+        Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x + ":" + str(y)
             writer.write("%s \n" % s1)
+            
+    def printResults(self):
+        """
+        This method prints all the statistics
+        """
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
     def getPatterns(self):
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def _genPatterns(self, suffix, pattern, data):
+        """ param suffix:
+            return:
+            param pattern:
+            return:
+            param data:
+            type:
+        """
         freqPatterns = {}
         index = data.index(suffix)
         for i in range(index + 1, len(data)):
             tid = pattern[1].intersection(data[i][1])
             if len(tid) >= self._minSup:
                 freqPattern = pattern[0] + ' ' + data[i][0]
                 freqPatterns[freqPattern] = len(tid)
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.8.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Parallel FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+# Parallel FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 #
 #  **Importing this algorithm into a python program**
 # ----------------------------------------------------
 #
 #     import PAMI.frequentPattern.pyspark.parallelFPGrowth as alg
 #
 #     obj = alg.parallelFPGrowth(iFile, minSup, numWorkers)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.savePatterns(oFile)
+#     obj.save(oFile)
 #
 #     Df = obj.getPatternInDataFrame()
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -52,14 +52,15 @@
 
 
 
 # from pyspark import SparkConf, SparkContext
 from collections import defaultdict
 from PAMI.frequentPattern.pyspark import abstract as _ab
 from operator import add
+from pyspark import SparkConf as _SparkConf, SparkContext as _SparkContext
 
 
 class Node:
     """
         Attribute
         ---------
             item : int
@@ -145,15 +146,15 @@
 
 
 
 
 class parallelFPGrowth(_ab._frequentPatterns):
     """
 
-    :Description: Parallel FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+    :Description: Parallel FPGrowth is one of the fundamental algorithm to discover frequent patterns in a transactional database. It stores the database in compressed fp-tree decreasing the memory usage and extracts the patterns from tree.It employs downward closure property to  reduce the search space effectively.
 
     :Reference: Li, Haoyuan et al. “Pfp: parallel fp-growth for query recommendation.” ACM Conference on Recommender Systems (2008).
 
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
@@ -206,15 +207,15 @@
     
                     obj.startMine()
     
                     frequentPatterns = obj.getPatterns()
     
                     print("Total number of Frequent Patterns:", len(frequentPatterns))
     
-                    obj.savePatterns(oFile)
+                    obj.save(oFile)
     
                     Df = obj.getPatternInDataFrame()
     
                     memUSS = obj.getMemoryUSS()
     
                     print("Total Memory in USS:", memUSS)
     
@@ -254,16 +255,16 @@
 
 
     def startMine(self):
         """Frequent pattern mining process will start from here"""
 
         self._startTime = _ab._time.time()
 
-        conf = SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
-        sc = SparkContext(conf=conf)
+        conf = _SparkConf().setAppName("Parallel FPGrowth").setMaster("local[*]")
+        sc = _SparkContext(conf=conf)
 
         rdd = sc.textFile(self._iFile, self._numPartitions)\
             .map(lambda x: x.rstrip().split('\t'))\
             .persist()
 
         self._lno = rdd.count()
         self._minSup = self._convert(self._minSup)
@@ -401,17 +402,17 @@
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a, b])
             dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataFrame
 
-    def savePatterns(self, outFile):
+    def save(self, outFile):
         """
-        Complete set of frequent patterns will be loaded in to a output file
+        Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             if type(x) == tuple:
@@ -427,14 +428,23 @@
         """
         Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
+    def printResults(self):
+        """ this function is used to print the results
+        """
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:", self.getRuntime())
+
+
     def _convert(self, value):
         """
         To convert the user specified minSup value
         :param value: user specified minSup value
         :return: converted type
         """
         if type(value) is int:
@@ -457,15 +467,15 @@
         if len(_ab._sys.argv) == 6:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         if len(_ab._sys.argv) == 5:
             _ap = parallelFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         _ap.startMine()
         _finalPatterns = _ap.getPatterns()
         print("Total number of Frequent Patterns:", len(_finalPatterns))
-        # _ap.savePatterns(_ab._sys.argv[2])
+        # _ap.save(_ab._sys.argv[2])
         _memUSS = _ap.getMemoryUSS()
         print("Total Memory in USS:", _memUSS)
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-
-
-# Top - K is and algorithm to discover top frequent patterns in a transactional database.
-#
 # **Importing this algorithm into a python program**
-# ---------------------------------------------------------
+# --------------------------------------------------------
 #
-#         import PAMI.frequentPattern.topK.FAE as alg
 #
-#         obj = alg.FAE(iFile, K)
+#     import PAMI.periodicFrequentPattern.kPFPMiner as alg
 #
-#         obj.startMine()
+#     obj = alg.kPFPMiner(iFile, k)
 #
-#         topKFrequentPatterns = obj.getPatterns()
+#     obj.startMine()
 #
-#         print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
+#     periodicFrequentPatterns = obj.getPatterns()
 #
-#         obj.save(oFile)
+#     print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
-#         Df = obj.getPatternInDataFrame()
+#     obj.save(oFile)
 #
-#         memUSS = obj.getMemoryUSS()
+#     Df = obj.getPatternInDataFrame()
 #
-#         print("Total Memory in USS:", memUSS)
+#     memUSS = obj.getMemoryUSS()
 #
-#         memRSS = obj.getMemoryRSS()
+#     print("Total Memory in USS:", memUSS)
 #
-#         print("Total Memory in RSS", memRSS)
-#
-#         run = obj.getRuntime()
-#
-#         print("Total ExecutionTime in seconds:", run)
-
+#     memRSS = obj.getMemoryRSS()
 #
+#     print("Total Memory in RSS", memRSS)
 #
+#     run = obj.getRuntime()
 #
+#     print("Total ExecutionTime in seconds:", run)
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -45,118 +39,143 @@
      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-from PAMI.frequentPattern.topk import abstract as _ab
-
-
-class FAE(_ab._frequentPatterns):
-    """
-    :Description: Top - K is and algorithm to discover top frequent patterns in a transactional database.
-
-
-    :Reference:   Zhi-Hong Deng, Guo-Dong Fang: Mining Top-Rank-K Frequent Patterns: DOI: 10.1109/ICMLC.2007.4370261 · Source: IEEE Xplore
-                  https://ieeexplore.ieee.org/document/4370261
-    :param  iFile: str :
-                   Name of the Input file to mine complete set of frequent patterns
-    :param  oFile: str :
-                   Name of the output file to store complete set of frequent patterns
-    :param  k: int :
-                    User specified count of top frequent patterns
-    :param  sep: str :
-                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
-
-
-
-    :Attributes:
-
-        startTime : float
-          To record the start time of the mining process
-
-        endTime : float
-          To record the completion time of the mining process
-
-        finalPatterns : dict
-          Storing the complete set of patterns in a dictionary variable
-
-        memoryUSS : float
-          To store the total amount of USS memory consumed by the program
+     Copyright (C)  2021 Rage Uday Kiran
 
-        memoryRSS : float
-          To store the total amount of RSS memory consumed by the program
-
-        finalPatterns : dict
-            it represents to store the patterns
-
-
-    **Methods to execute code on terminal**
-    ----------------------------------------
-
-        Format:
-
-           >>> python3 FAE.py <inputFile> <outputFile> <K>
-
-        Examples:
-
-           >>> python3 FAE.py sampleDB.txt patterns.txt 10
-
-
-    **Importing this algorithm into a python program**
-    ---------------------------------------------------------
-    .. code-block:: python
-
-        import PAMI.frequentPattern.topK.FAE as alg
-
-        obj = alg.FAE(iFile, K)
-
-        obj.startMine()
-
-        topKFrequentPatterns = obj.getPatterns()
-
-        print("Total number of Frequent Patterns:", len(topKFrequentPatterns))
-
-        obj.save(oFile)
-
-        Df = obj.getPatternInDataFrame()
-
-        memUSS = obj.getMemoryUSS()
+"""
 
-        print("Total Memory in USS:", memUSS)
 
-        memRSS = obj.getMemoryRSS()
+from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
 
-        print("Total Memory in RSS", memRSS)
 
-        run = obj.getRuntime()
+class kPFPMiner(_ab._periodicFrequentPatterns):
+    """
+        Description:
+        ------------
 
-        print("Total ExecutionTime in seconds:", run)
+            Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
 
-    Credits:
-    --------
-        The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+        Reference:
+        -----------
+            Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
+            Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
+            BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
+
+        Attributes:
+        -----------
+            iFile : str
+                Input file name or path of the input file
+            k: int
+                User specified counte of top-k periodic frequent patterns
+            sep : str
+                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+                However, the users can override their default separator.
+            oFile : str
+                Name of the output file or the path of the output file
+            startTime:float
+                To record the start time of the mining process
+            endTime:float
+                To record the completion time of the mining process
+            finalPatterns: dict
+                Storing the complete set of patterns in a dictionary variable
+            memoryUSS : float
+                To store the total amount of USS memory consumed by the program
+            memoryRSS : float
+                To store the total amount of RSS memory consumed by the program
+
+        Methods:
+        ---------
+            startMine()
+                Mining process will start from here
+            getPatterns()
+                Complete set of patterns will be retrieved with this function
+            savePatterns(oFile)
+                Complete set of frequent patterns will be loaded in to a output file
+            getPatternsAsDataFrame()
+                Complete set of frequent patterns will be loaded in to a dataframe
+            getMemoryUSS()
+                Total amount of USS memory consumed by the mining process will be retrieved from this function
+            getMemoryRSS()
+                Total amount of RSS memory consumed by the mining process will be retrieved from this function
+            getRuntime()
+                Total amount of runtime taken by the mining process will be retrieved from this function
+            creatingItemSets()
+                Scans the dataset or dataframes and stores in list format
+            frequentOneItem()
+                Generates one frequent patterns
+            eclatGeneration(candidateList)
+                It will generate the combinations of frequent items
+            generateFrequentPatterns(tidList)
+                It will generate the combinations of frequent items from a list of items
+
+        Executing the code on terminal:
+        -------------------------------
+
+            Format:
+            ------
+            >>> python3 kPFPMiner.py <inputFile> <outputFile> <k>
+
+            Examples:
+            ---------
+            >>> python3 kPFPMiner.py sampleDB.txt patterns.txt 10
+
+
+        Sample run of the importing code:
+        ---------------------------------
+        .. code-block:: python
+
+            import PAMI.periodicFrequentPattern.kPFPMiner as alg
+
+            obj = alg.kPFPMiner(iFile, k)
+
+            obj.startMine()
+
+            periodicFrequentPatterns = obj.getPatterns()
+
+            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+
+            obj.save(oFile)
+
+            Df = obj.getPatternInDataFrame()
+
+            memUSS = obj.getMemoryUSS()
+
+            print("Total Memory in USS:", memUSS)
+
+            memRSS = obj.getMemoryRSS()
+
+            print("Total Memory in RSS", memRSS)
+
+            run = obj.getRuntime()
+
+            print("Total ExecutionTime in seconds:", run)
+
+        Credits:
+        --------
+            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _startTime = float()
     _endTime = float()
     _k = int()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
     _tidList = {}
-    _minimum = int()
+    lno = int()
+    _maximum = int()
 
     def _creatingItemSets(self):
         """
             Storing the complete transactions of the database/input file in a database variable
 
         """
 
@@ -185,40 +204,63 @@
                             line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
+                    
+    def getPer_Sup(self, tids):
+        tids.sort()
+        cur=0
+        per=list()
+        sup=0
+        #print(tids)
+        for i in range(len(tids)-1):
+            j = i + 1
+            #if tids[j] - cur <= periodicity:
+                #return [0,0]
+            per.append(tids[j] - cur)
+            cur = tids[j]
+        per.append(self.lno - cur)
+        return max(per)
 
     def _frequentOneItem(self):
         """
         Generating one frequent patterns
         """
-        candidate = {}
+        self._mapSupport = {}
         self._tidList = {}
-        for i in range(len(self._Database)):
-            for j in self._Database[i]:
-                if j not in candidate:
-                    candidate[j] = 1
-                    self._tidList[j] = [i]
+        n = 0
+        for line in self._Database:
+            self.lno += 1
+            n = int(line[0])
+            for i in range(1, len(line)):
+                si = line[i]
+                if self._mapSupport.get(si) is None:
+                    self._mapSupport[si] = [1, abs(0 - n), n]
+                    self._tidList[si] = [n]
                 else:
-                    candidate[j] += 1
-                    self._tidList[j].append(i)
-        self._finalPatterns = {}
-        plist = [key for key, value in sorted(candidate.items(), key=lambda x: x[1], reverse=True)]
+                    self._mapSupport[si][0] += 1
+                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
+                    self._mapSupport[si][2] = n
+                    self._tidList[si].append(n)
+        for x, y in self._mapSupport.items():
+            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
+        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
         for i in plist:
             if len(self._finalPatterns) >= self._k:
                 break
             else:
-                self._finalPatterns[i] = candidate[i]
-        self._minimum = min([self._finalPatterns[i] for i in self._finalPatterns.keys()])
+                self._finalPatterns[i] = self._mapSupport[i][1]
+        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
         plist = list(self._finalPatterns.keys())
         return plist
 
+
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
 
             :param prefix: the prefix of a pattern
             :type prefix: list
             :param suffix: the suffix of a patterns
             :type suffix: list
@@ -226,32 +268,32 @@
             :type tidSetI: list
         """
 
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = len(tidSetI)
+        val = self.getPer_Sup(tidSetI)
         sample = str()
         for i in prefix:
-            sample = sample + i + "\t"
+            sample = sample + i + " "
         if len(self._finalPatterns) < self._k:
-            if val > self._minimum:
+            if val < self._maximum:
                 self._finalPatterns[sample] = val
                 self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._minimum = min([i for i in self._finalPatterns.values()])
+                self._maximum = max([i for i in self._finalPatterns.values()])
         else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1]):
-                if val > y:
+            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
+                if val < y:
                     del self._finalPatterns[x]
                     self._finalPatterns[sample] = val
                     self._finalPatterns = {k: v for k, v in
                                               sorted(self._finalPatterns.items(), key=lambda item: item[1],
                                                      reverse=True)}
-                    self._minimum = min([i for i in self._finalPatterns.values()])
+                    self._maximum = max([i for i in self._finalPatterns.values()])
                     return
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
             :param prefix:  main equivalence prefix
             :type prefix: periodic-frequent item or pattern
@@ -276,15 +318,15 @@
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
             for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
                 y = list(set(tidSetI).intersection(tidSetJ))
-                if len(y) >= self._minimum:
+                if self.getPer_Sup(y) <= self._maximum:
                     classItemSets.append(itemJ)
                     classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
             self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def _convert(self, value):
@@ -324,19 +366,19 @@
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i + 1, len(plist)):
                 itemJ = plist[j]
                 tidSetJ = self._tidList[itemJ]
                 y1 = list(set(tidSetI).intersection(tidSetJ))
-                if len(y1) >= self._minimum:
+                if self.getPer_Sup(y1) <= self._maximum:
                     itemSets.append(itemJ)
                     tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print(" TopK frequent patterns were successfully generated using FAE algorithm.")
+        print("kPFPMiner has successfully generated top-k frequent patterns")
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
@@ -377,57 +419,61 @@
 
         :rtype: pd.DataFrame
         """
 
         dataFrame = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a.replace('\t', ' '), b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            data.append([a, b])
+            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
         return dataFrame
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x.strip() + ":" + str(y)
+            patternsAndSupport = x + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printTOPK(self):
-        print("Top K Frequent  Patterns:", len(self.getPatterns()))
+    def printResults(self):
+        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = FAE(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Top K Frequent Patterns:", len(_ap.getPatterns()))
+        _Patterns = _ap.getPatterns()
+        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        _memUSS = _ap.getMemoryUSS()
+        print("Total Memory in USS:", _memUSS)
+        _memRSS = _ap.getMemoryRSS()
+        print("Total Memory in RSS", _memRSS)
+        _run = _ap.getRuntime()
+        print("Total ExecutionTime in ms:", _run)
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.8.1/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py` & `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py` & `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#         from PAMI.frequentSpatialPattern.basic import FSPGrowth as alg
+#         from PAMI.georeferencedFrequentPattern.basic import FSPGrowth as alg
 #
 #         obj = alg.FSPGrowth("sampleTDB.txt", "sampleN.txt", 5)
 #
 #         obj.startMine()
 #
 #         spatialFrequentPatterns = obj.getPatterns()
 #
@@ -42,15 +42,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.frequentSpatialPattern.basic import abstract as _ab
+from PAMI.georeferencedFrequentPattern.basic import abstract as _ab
 
 
 class _Node:
     """
     A class used to represent the node of frequentPatternTree
     Attributes
     ----------
@@ -291,15 +291,15 @@
 
             >>> python3 FSPGrowth.py sampleTDB.txt output.txt sampleN.txt 0.5 (minSup will be considered in percentage of database transactions)
 
     Sample run of importing the code :
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.frequentSpatialPattern.basic import FSPGrowth as alg
+        from PAMI.georeferencedFrequentPattern.basic import FSPGrowth as alg
 
         obj = alg.FSPGrowth("sampleTDB.txt", "sampleN.txt", 5)
 
         obj.startMine()
 
         spatialFrequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py` & `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  **Importing this algorithm into a python program**
 #  ---------------------------------------------------
 #
-#     from PAMI.frequentSpatialPattern.basic import SpatialECLAT as alg
+#     from PAMI.georeferencedFrequentPattern.basic import SpatialECLAT as alg
 #
 #     obj = alg.SpatialECLAT("sampleTDB.txt", "sampleN.txt", 5)
 #
 #     obj.startMine()
 #
 #     spatialFrequentPatterns = obj.getPatterns()
 #
@@ -41,15 +41,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.frequentSpatialPattern.basic import abstract as _ab
+from PAMI.georeferencedFrequentPattern.basic import abstract as _ab
 
 
 class SpatialECLAT(_ab._spatialFrequentPatterns):
     """
     Description:
     --------------
         Spatial Eclat is a Extension of ECLAT algorithm,which  stands for Equivalence Class Clustering and bottom-up
@@ -130,15 +130,15 @@
 
             >>> python3 SpatialECLAT.py sampleTDB.txt output.txt sampleN.txt 0.5 (minSup will be considered in percentage of database transactions)
             
     Sample run of importing the code :
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.frequentSpatialPattern.basic import SpatialECLAT as alg
+        from PAMI.georeferencedFrequentPattern.basic import SpatialECLAT as alg
         
         obj = alg.SpatialECLAT("sampleTDB.txt", "sampleN.txt", 5)
 
         obj.startMine()
 
         spatialFrequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/georeferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
      A class represent a Fuzzy List of an element
 
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -59,16 +59,16 @@
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.IUtils
         self.sumRUtil += element.RUtils
         self.elements.append(element)
 
 
 class Element:
@@ -76,17 +76,17 @@
         A class represents an Element of a fuzzy list
 
     Attributes :
     ----------
         tid : int
             keep tact of transaction id
         IUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         RUtil : float
-            the neighbourhood resting value of an fuzzy item in the transaction
+            the neighbourhood resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, IUtil, RUtil):
         self.tid = tid
         self.IUtils = IUtil
         self.RUtils = RUtil
 
@@ -162,14 +162,18 @@
                     mapOfRegions[t1] = 1
                 else:
                     temp = mapOfRegions[t1]
                     mapOfRegions = temp + 1
 
 
 class _Pair:
+    """
+            A class to store item and it's quantity together
+        """
+
     def __init__(self):
         """
             A Class to Store item and its quantity together
         """
         self.item = 0
         self.quantity = 0
         self.region = 'N'
@@ -372,14 +376,18 @@
                 value = float(value)
                 value = (len(self._transactions) * value)
             else:
                 value = int(value)
         return value
     
     def _creatingItemSets(self):
+        """
+          Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactions, self._fuzzyValues = [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._transactions = self._iFile['Transactions'].tolist()
@@ -651,26 +659,27 @@
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b[0], b[1]])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the result"""
         print("Total number of Fuzzy Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py` & `pami-2023.8.1/PAMI/fuzzyFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py` & `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
+#     from PAMI.fuzzyFrequentPattern import FFIMiner as alg
 #
 #     obj = alg.FFIMiner("input.txt", 2)
 #
 #     obj.startMine()
 #
-#     fuzzyFrequentPatterns = obj.getPatterns()
+#     fuzzyFrequentPattern = obj.getPatterns()
 #
-#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
+#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
 #
 #     obj.save("outputFile")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,27 +42,27 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
+from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -79,16 +79,16 @@
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -103,17 +103,17 @@
         A class represents an Element of a fuzzy list
 
     Attributes:
     ----------
             tid : int
                 keep tact of transaction id
             iUtils: float
-                the utility of an fuzzy item in the transaction
+                the utility of a fuzzy item in the transaction
             rUtils : float
-                the  resting value of an fuzzy item in the transaction
+                the  resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -217,23 +217,23 @@
             >>> python3  FFIMiner.py sampleTDB.txt output.txt 6  (minSup will be considered in support count or frequency)
 
 
     Sample run of importing the code:
     ----------------------------------
     .. code-block:: python
 
-        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
+        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", 2)
 
         obj.startMine()
 
-        fuzzyFrequentPatterns = obj.getPatterns()
+        fuzzyFrequentPattern = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
 
@@ -308,14 +308,18 @@
                 value = float(value)
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemsets(self):
+        """
+         Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactions, self._fuzzyValues, self._Database = [], [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._transactions = self._iFile['Transactions'].tolist()
@@ -546,26 +550,27 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results"""
         print("Total number of Fuzzy Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py` & `pami-2023.8.1/PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,65 @@
+# **Importing this algorithm into a python program**
+# --------------------------------------------------------
+#
+#     from PAMI.fuzzyFrequentPattern import FFIMiner as alg
+#
+#     obj = alg.FFIMiner("input.txt", 2)
+#
+#     obj.startMine()
+#
+#     fuzzyFrequentPattern = obj.getPatterns()
+#
+#     print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
+#
+#     obj.save("outputFile")
+#
+#     memUSS = obj.getMemoryUSS()
+#
+#     print("Total Memory in USS:", memUSS)
+#
+#     memRSS = obj.getMemoryRSS()
+#
+#     print("Total Memory in RSS", memRSS)
+#
+#     run = obj.getRuntime()
+#
+#     print("Total ExecutionTime in seconds:", run)
+
+__copyright__ = """
+ Copyright (C)  2021 Rage Uday Kiran
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
 
-from PAMI.fuzzyFrequentPatterns.basic import abstract as _ab
+"""
+from PAMI.fuzzyFrequentPattern.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -32,16 +76,16 @@
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -56,17 +100,17 @@
         A class represents an Element of a fuzzy list
 
     Attributes:
     ----------
             tid : int
                 keep tact of transaction id
             iUtils: float
-                the utility of an fuzzy item in the transaction
+                the utility of a fuzzy item in the transaction
             rUtils : float
-                the  resting value of an fuzzy item in the transaction
+                the  resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -203,23 +247,23 @@
                                                       (it will consider '\t' as a separator)
 
             python3  FFIMinerMiner.py sampleTDB.txt output.txt 6 , (it consider ',' as a separator)
 
     Sample run of importing the code:
     -------------------------------
 
-        from PAMI.fuzzyFrequentPatterns import FFIMiner as alg
+        from PAMI.fuzzyFrequentPattern import FFIMiner as alg
 
         obj = alg.FFIMiner("input.txt", "fuzzyMembership.txt" 2)
 
         obj.startMine()
 
-        fuzzyFrequentPatterns = obj.getPatterns()
+        fuzzyFrequentPattern = obj.getPatterns()
 
-        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPatterns))
+        print("Total number of Fuzzy Frequent Patterns:", len(fuzzyFrequentPattern))
 
         obj.save("outputFile")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
 
@@ -329,14 +373,18 @@
             print(self._RegionsLabel)
             print(self._RegionsCal)
         except IOError:
             print("File Not Found")
             quit()
 
     def _creatingItemsets(self):
+        """
+         Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactions, self._fuzzyValues, self._Database = [], [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._transactions = self._iFile['Transactions'].tolist()
@@ -369,14 +417,17 @@
                             self._transactions.append([x for x in items])
                             self._fuzzyValues.append([x for x in quantities])
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _Regions(self, quantity):
+        """ param quantity:
+            type quantity:
+        """
         self.list = [0] * len(self._LabelKey)
         if self._RegionsCal[0][0] < quantity <= self._RegionsCal[0][1]:
             self.list[0] = 1
             return
         elif quantity >= self._RegionsCal[-1][0]:
             self.list[-1] = 1
             return
@@ -622,26 +673,28 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Fuzzy Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
@@ -37,20 +38,20 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyFrequentPattenrs(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+class _sequentialPatterns(_ABC):
+    """
+    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
         employ in PAMI
 
-
-    Attributes :
+    Attributes:
     ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
@@ -67,15 +68,15 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods :
+    Methods:
     -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
@@ -83,39 +84,38 @@
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
-
     """
 
     def __init__(self, iFile, minSup, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
+        self._finalPatterns = {}
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
-        self._oFile = str()
-        self._finalPatterns = {}
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -124,15 +124,14 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -149,19 +148,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-
+        pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #     .. code-block:: python
 #
-#         from PAMI.fuzzyFrequentSpatialPattern import FFSPMiner as alg
+#         from PAMI.fuzzyGeoreferencedFrequentPattern import FFSPMiner as alg
 #
 #         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 2)
 #
 #         obj.startMine()
 #
 #         fuzzySpatialFrequentPatterns = obj.getPatterns()
 #
@@ -44,27 +44,27 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.fuzzyFrequentSpatialPattern.basic import abstract as _ab
+from PAMI.fuzzyGeoreferencedFrequentPattern.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -81,16 +81,16 @@
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -105,17 +105,17 @@
         A class represents an Element of a fuzzy list
 
     Attributes :
     ----------
         tid : int
             keep tact of transaction id
         iUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the neighbourhood resting value of an fuzzy item in the transaction
+            the neighbourhood resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -207,25 +207,25 @@
         WriteOut(prefix, prefixLen, item, sumIUtil,period)
             To Store the patten
 
     Executing the code on terminal :
     -----------------------------------
         Format:
 
-            >>> python3 FFSPMiner_old.py <inputFile> <outputFile> <neighbours> <minSup> <sep>
+            >>> python3 FFSPMiner.py <inputFile> <outputFile> <neighbours> <minSup> <sep>
         Examples:
 
-            >>> python3  FFSPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3  (minSup will be considered in support count or frequency)
+            >>> python3  FFSPMiner.py sampleTDB.txt output.txt sampleN.txt 3  (minSup will be considered in support count or frequency)
 
 
     Sample run of importing the code:
     -----------------------------------
     .. code-block:: python
 
-        from PAMI.fuzzyFrequentSpatialPattern import FFSPMiner as alg
+        from PAMI.fuzzyGeoreferencedFrequentPattern import FFSPMiner as alg
 
         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 2)
 
         obj.startMine()
 
         fuzzySpatialFrequentPatterns = obj.getPatterns()
 
@@ -301,14 +301,18 @@
             if '.' in value:
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
+        """
+          Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactions, self._fuzzyValues = [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self.transactions = self._iFile['Transactions'].tolist()
@@ -607,26 +611,27 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self.oFile = outFile
         writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + " : " + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results"""
         print("Total number of Spatial Fuzzy Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,68 @@
-#  Copyright (C)  2021 Rage Uday Kiran
 #
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
+# **Importing this algorithm into a python program**
+# --------------------------------------------------------
+#     .. code-block:: python
 #
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#         from PAMI.fuzzyGeoreferencedFrequentPattern import FFSPMiner as alg
+#
+#         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 2)
+#
+#         obj.startMine()
+#
+#         fuzzySpatialFrequentPatterns = obj.getPatterns()
+#
+#         print("Total number of fuzzy frequent spatial patterns:", len(fuzzySpatialFrequentPatterns))
+#
+#         obj.save("outputFile")
+#
+#         memUSS = obj.getMemoryUSS()
+#
+#         print("Total Memory in USS:", memUSS)
+#
+#         memRSS = obj.getMemoryRSS()
+#
+#         print("Total Memory in RSS", memRSS)
+#
+#         run = obj.getRuntime()
+#
+#         print("Total ExecutionTime in seconds:", run)
+
+__copyright__ = """
+ Copyright (C)  2021 Rage Uday Kiran
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
 
-from PAMI.fuzzyFrequentSpatialPattern.basic import abstract as _ab
+"""
+
+from PAMI.fuzzyGeoreferencedFrequentPattern.basic import abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
 
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -59,16 +79,16 @@
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -83,17 +103,17 @@
         A class represents an Element of a fuzzy list
 
     Attributes :
     ----------
         tid : int
             keep tact of transaction id
         iUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the neighbourhood resting value of an fuzzy item in the transaction
+            the neighbourhood resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -219,27 +239,27 @@
             To find element with same tid as given
         WriteOut(prefix, prefixLen, item, sumIUtil,period)
             To Store the patten
     
     Executing the code on terminal :
     -------
         Format:
-            python3 FFSPMiner_old.py <inputFile> <outputFile> <neighbours> <minSup> <sep>
+            >>> python3 FFSPMiner_old.py <inputFile> <outputFile> <neighbours> <minSup> <sep>
         Examples:
-            python3  FFSPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3  (minSup will be considered in support count or frequency)
+           >>>  python3  FFSPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3  (minSup will be considered in support count or frequency)
 
             python3  FFSPMiner_old.py sampleTDB.txt output.txt sampleN.txt 0.3 (minSup and maxPer will be considered in percentage of database)
                                                             (will consider "\t" as separator in both input and neighbourhood files)
 
             python3  FFSPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3 ,
                                                               (will consider "," as separator in both input and neighbourhood files)
     Sample run of importing the code:
     -------------------------------
         
-        from PAMI.fuzzyFrequentSpatialPattern import FFSPMiner as alg
+        from PAMI.fuzzyGeoreferencedFrequentPattern import FFSPMiner as alg
 
         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 2)
 
         obj.startMine()
 
         fuzzySpatialFrequentPatterns = obj.getPatterns()
 
@@ -319,14 +339,18 @@
             if '.' in value:
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
+        """
+                    Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactions, self._fuzzyValues = [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self.transactions = self._iFile['Transactions'].tolist()
@@ -658,26 +682,28 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self.oFile = outFile
         writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + " : " + str(y)
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Spatial Fuzzy Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py` & `pami-2023.8.1/PAMI/AssociationRules/basic/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-#  Copyright (C)  2021 Rage Uday Kiran
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+__copyright__ = """
+
+ Copyright (C)  2021 Rage Uday Kiran
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+"""
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
@@ -37,21 +41,21 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _fuzzyPartialPattenrs(_ABC):
+class _AssociationRules(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
-    Attributes :
-    ----------
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -67,16 +71,16 @@
         oFile : str
             Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods :
-    -------
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
@@ -86,36 +90,36 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, sep="\t"):
+    def __init__(self, iFile, minConf, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
-        self._minSup = minSup
-        self._startTime = float()
-        self._endTime = float()
+        self._minConf = minConf
+        self._finalPatterns = {}
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
-        self._oFile = str()
-        self._finalPatterns = {}
+        self._startTime = float()
+        self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -149,19 +153,18 @@
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
 
         pass
 
-
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
-
+        pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print result of the execution"""
 
         pass
```

### Comparing `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,21 +65,21 @@
         A class represent a Fuzzy List of an element
 
     Attributes:
     ----------
         item: int
             the item name
         sumLUtil: float
-            the sum of utilities of an fuzzy item in database
+            the sum of utilities of a fuzzy item in database
         sumRUtil: float
             the sum of resting values of a fuzzy item in database
         elements: list
             list of elements contain tid,Utility and resting values of element in each transaction
         maxPeriod: int
-            it represent the max period of a item
+            it represents the max period of a item
 
     Methods:
     -------
         addElement(element)
             Method to add an element to this fuzzy list and update the sums at the same time.
 
         printElement(e)
@@ -94,16 +94,16 @@
         self.elements = []
         self.maxPeriod = 0
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumLUtil += element.lUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
         self.maxPeriod = max(self.maxPeriod, element.period)
 
     def printElement(self):
@@ -119,17 +119,17 @@
         A class represents an Element of a fuzzy list
 
         Attributes:
         ----------
         tid : int
             keep tact of transaction id
         lUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the resting value of an fuzzy item in the transaction
+            the resting value of a fuzzy item in the transaction
         period: int
             represent the period of the element
     """
 
     def __init__(self, tid, iUtil, rUtil, period):
         self.tid = tid
         self.lUtils = iUtil
@@ -228,24 +228,24 @@
         WriteOut(prefix, prefixLen, item, sumIUtil,period)
             To Store the patten
 
     Executing the code on terminal :
     -------
         Format:
         ------
-            python3 FPFPMiner_old.py <inputFile> <outputFile> <minSup> <maxPer> <sep>
+            >>> python3 FPFPMiner.py <inputFile> <outputFile> <minSup> <maxPer> <sep>
 
         Examples:
         ------
-            python3  FPFPMiner_old.py sampleTDB.txt output.txt 2 3 (minSup and maxPer will be considered in support count or frequency)
+            >>> python3  FPFPMiner.py sampleTDB.txt output.txt 2 3 (minSup and maxPer will be considered in support count or frequency)
 
-            python3  FPFPMiner_old.py sampleTDB.txt output.txt 0.25 0.3 (minSup and maxPer will be considered in percentage of database)
+            >>> python3  FPFPMiner.py sampleTDB.txt output.txt 0.25 0.3 (minSup and maxPer will be considered in percentage of database)
                                         (will consider "\t" as separator)
 
-            python3  FPFPMiner_old.py sampleTDB.txt output.txt 2 3  ,(will consider ',' as separator)
+            >>> python3  FPFPMiner.py sampleTDB.txt output.txt 2 3  ,(will consider ',' as separator)
 
 
     Sample run of importing the code:
     -------------------------------
 
         from PAMI.fuzzyPeriodicFrequentPattern.basic import FPFPMiner as alg
 
@@ -330,14 +330,18 @@
             if '.' in value:
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
+        """
+            Storing the complete transactions of the database/input file in a database variable
+
+        """
         data, self._transactions, self._fuzzyValues, ts = [], [], [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'TS' in i:
                 self._ts = self._iFile['TS'].tolist()
@@ -597,26 +601,28 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Fuzzy Periodic-Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,84 @@
-#  Copyright (C)  2021 Rage Uday Kiran
+# Sample run of importing the code:
+#     -------------------------------
 #
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
+#         from PAMI.fuzzyPeriodicFrequentPattern.basic import FPFPMiner as alg
 #
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#         obj =alg.FPFPMiner("input.txt",2,3)
+#
+#         obj.startMine()
+#
+#         periodicFrequentPatterns = obj.getPatterns()
+#
+#         print("Total number of Fuzzy Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#
+#         obj.save("output.txt")
+#
+#         memUSS = obj.getMemoryUSS()
+#
+#         print("Total Memory in USS:", memUSS)
+#
+#         memRSS = obj.getMemoryRSS()
+#
+#         print("Total Memory in RSS", memRSS)
+#
+#         run = obj.getRuntime()
+#
+#         print("Total ExecutionTime in seconds:", run)
+
+
+__copyright__ = """(Copyright (C)  2021 Rage Uday Kiran
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+)"""
+
 
 from PAMI.fuzzyPeriodicFrequentPattern.basic import abstract as _ab
 
 
 class _FFList:
     """
         A class represent a Fuzzy List of an element
 
     Attributes:
     ----------
         item: int
             the item name
         sumLUtil: float
-            the sum of utilities of an fuzzy item in database
+            the sum of utilities of a fuzzy item in database
         sumRUtil: float
             the sum of resting values of a fuzzy item in database
         elements: list
             list of elements contain tid,Utility and resting values of element in each transaction
         maxPeriod: int
-            it represent the max period of a item
+            it represents the max period of a item
 
     Methods:
     -------
         addElement(element)
             Method to add an element to this fuzzy list and update the sums at the same time.
 
         printElement(e)
@@ -63,16 +93,16 @@
         self.elements = []
         self.maxPeriod = 0
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
 
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumLUtil += element.lUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
         self.maxPeriod = max(self.maxPeriod, element.period)
 
     def printElement(self):
@@ -88,17 +118,17 @@
         A class represents an Element of a fuzzy list
 
         Attributes:
         ----------
         tid : int
             keep tact of transaction id
         lUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the resting value of an fuzzy item in the transaction
+            the resting value of a fuzzy item in the transaction
         period: int
             represent the period of the element
     """
 
     def __init__(self, tid, iUtil, rUtil, period):
         self.tid = tid
         self.lUtils = iUtil
@@ -227,19 +257,19 @@
         WriteOut(prefix, prefixLen, item, sumIUtil,period)
             To Store the patten
 
     Executing the code on terminal :
     -------
         Format:
         ------
-            python3 FPFPMiner_old.py <inputFile> <outputFile> <minSup> <maxPer> <sep>
+            >>> python3 FPFPMiner_old.py <inputFile> <outputFile> <minSup> <maxPer> <sep>
 
         Examples:
         ------
-            python3  FPFPMiner_old.py sampleTDB.txt output.txt 2 3 (minSup and maxPer will be considered in support count or frequency)
+            >>> python3  FPFPMiner_old.py sampleTDB.txt output.txt 2 3 (minSup and maxPer will be considered in support count or frequency)
 
             python3  FPFPMiner_old.py sampleTDB.txt output.txt 0.25 0.3 (minSup and maxPer will be considered in percentage of database)
                                         (will consider "\t" as separator)
 
             python3  FPFPMiner_old.py sampleTDB.txt output.txt 2 3  ,(will consider ',' as separator)
 
 
@@ -333,14 +363,18 @@
             if '.' in value:
                 value = (self._dbLen * value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
+        """
+          Storing the complete transactions of the database/input file in a database variable
+
+        """
         data, self._transactions, self._fuzzyValues, ts = [], [], [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'TS' in i:
                 self._ts = self._iFile['TS'].tolist()
@@ -637,26 +671,28 @@
 
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
 
         :param outFile: name of the output file
         :type outFile: file
         """
         self._oFile = outFile
         writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             patternsAndSupport = x.strip() + ":" + str(y[0]) + ":" + str(y[1])
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results
+         """
         print("Total number of Fuzzy Periodic-Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in seconds:", self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.8.1/PAMI/georeferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.fuzzySpatialPeriodicFrequentPattern import FGPFPMiner as alg
+#     from PAMI.fuzzyGeoreferencedPeriodicFrequentPattern import FGPFPMiner as alg
 #
 #     obj = alg.FFSPMiner("input.txt", "neighbours.txt", 3, 4)
 #
 #     obj.startMine()
 #
 #     print("Total number of fuzzy frequent spatial patterns:", len(obj.getPatterns()))
 #
@@ -35,26 +35,26 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-import PAMI.fuzzySpatialPeriodicFrequentPattern.basic.abstract as _ab
+import PAMI.fuzzyGeoreferencedPeriodicFrequentPattern.basic.abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -69,16 +69,16 @@
         self.sumIUtil = 0.0
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -92,17 +92,17 @@
     """
         A class represents an Element of a fuzzy list
     Attributes :
     ----------
         tid : int
             keep tact of transaction id
         iUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the neighbourhood resting value of an fuzzy item in the transaction
+            the neighbourhood resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -191,23 +191,23 @@
             To find element with same tid as given
         WriteOut(prefix, prefixLen, item, sumIUtil,period)
             To Store the patten
     Executing the code on terminal :
     -----------------------------------
         Format:
         -------
-            >>> python3 FGPFPMiner_old.py <inputFile> <outputFile> <neighbours> <minSup> <maxPer> <sep>
+            >>> python3 FGPFPMiner.py <inputFile> <outputFile> <neighbours> <minSup> <maxPer> <sep>
         Examples:
-            >>> python3  FGPFPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3 4  (minSup will be considered in support count or frequency)
+            >>> python3  FGPFPMiner.py sampleTDB.txt output.txt sampleN.txt 3 4  (minSup will be considered in support count or frequency)
            
     Sample run of importing the code:
     --------------------------------------
     .. code-block:: python
     
-        from PAMI.fuzzySpatialPeriodicFrequentPattern import FGPFPMiner as alg
+        from PAMI.fuzzyGeoreferencedPeriodicFrequentPattern import FGPFPMiner as alg
         
         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 3, 4)
         
         obj.startMine()
         
         print("Total number of fuzzy frequent spatial patterns:", len(obj.getPatterns()))
         
@@ -280,14 +280,18 @@
             if '.' in value:
                 value = float(value)
             else:
                 value = int(value)
         return value
 
     def _creatingItemSets(self):
+        """
+                    Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactionsDB, self._fuzzyValuesDB, self._ts = [], [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._transactionsDB = self._iFile['Transactions'].tolist()
@@ -401,16 +405,16 @@
                     else:
                         self._itemSupData[item] = fuzzy_ref
         for item in self._tidList.keys():
             self._tidList[item].append(len(self._transactionsDB) - recent_occur[item][-1])
         del recent_occur
         """
             Using Maximum Scalar Cardinality Value strategy to narrow down search space and generate candidate fuzzy periodic-frequent items. 
-            Step1. Identify the regional representative (region with max support). This is the representative that will be tested to see if its greater than given minsup
-            Step2. prune out all items whose regional support is less than the given minsup
+            Step1. Identify the regional representative (region with max support). This is the representative that will be tested to see if its greater than given minSup
+            Step2. prune out all items whose regional support is less than the given minSup
             Step3. At the end, sort the list of stored Candidate Frequent-Periodic Patterns in ascending order
         """
 
         listOfFFList = []
         mapItemsToFFLIST = {}
         region_label = []
         #self._minSup = self._convert(self._minSup)
@@ -629,26 +633,28 @@
         """ Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPeriodicPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self.oFile = outFile
         keylist = (self._finalPatterns.keys())
         writer = open(self.oFile, 'w+')
         for x in keylist:
             patternsAndSupport = x.strip() + ":" + str(self._finalPatterns[x])
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the result
+        """
         print("Total number of Spatial Fuzzy Periodic-Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
```

### Comparing `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,59 @@
-#  Copyright (C)  2021 Rage Uday Kiran
 #
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
+# **Importing this algorithm into a python program**
+# --------------------------------------------------------
 #
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
+#     from PAMI.fuzzyGeoreferencedPeriodicFrequentPattern import FGPFPMiner as alg
 #
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#     obj = alg.FFSPMiner("input.txt", "neighbours.txt", 3, 4)
 #
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
+#     obj.startMine()
 #
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
+#     print("Total number of fuzzy frequent spatial patterns:", len(obj.getPatterns()))
 #
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#     obj.save("outputFile")
+#
+#     print("Total Memory in USS:", obj.getMemoryUSS())
+#
+#     print("Total Memory in RSS", obj.getMemoryRSS())
+#
+#     print("Total ExecutionTime in seconds:", obj.getRuntime())
+#
+__copyright__ = """
+ Copyright (C)  2021 Rage Uday Kiran
+
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
+
+"""
 import pandas as pd
 import plotly.express as px
-import PAMI.fuzzySpatialPeriodicFrequentPattern.basic.abstract as _ab
+import PAMI.fuzzyGeoreferencedPeriodicFrequentPattern.basic.abstract as _ab
 
 
 class _FFList:
     """
      A class represent a Fuzzy List of an element
     Attributes :
     ----------
          item: int
              the item name
          sumIUtil: float
-             the sum of utilities of an fuzzy item in database
+             the sum of utilities of a fuzzy item in database
          sumRUtil: float
              the sum of resting values of a fuzzy item in database
          elements: list
              a list of elements contain tid,Utility and resting values of element in each transaction
     Methods :
     -------
         addElement(element)
@@ -57,16 +68,16 @@
         self.sumIUtil = 0.0
         self.sumRUtil = 0.0
         self.elements = []
 
     def addElement(self, element):
         """
             A Method that add a new element to FFList
-            :param element: an element to be add to FFList
-            :pram type: Element
+            :param element: an element to be added to FFList
+            :param type: Element
         """
         self.sumIUtil += element.iUtils
         self.sumRUtil += element.rUtils
         self.elements.append(element)
 
     def printElement(self):
         """
@@ -80,17 +91,17 @@
     """
         A class represents an Element of a fuzzy list
     Attributes :
     ----------
         tid : int
             keep tact of transaction id
         iUtils: float
-            the utility of an fuzzy item in the transaction
+            the utility of a fuzzy item in the transaction
         rUtils : float
-            the neighbourhood resting value of an fuzzy item in the transaction
+            the neighbourhood resting value of a fuzzy item in the transaction
     """
 
     def __init__(self, tid, iUtil, rUtil):
         self.tid = tid
         self.iUtils = iUtil
         self.rUtils = rUtil
 
@@ -180,15 +191,15 @@
             python3  FGPFPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3 4  (minSup will be considered in support count or frequency)
             python3  FGPFPMiner_old.py sampleTDB.txt output.txt sampleN.txt 0.3 0.4 (minSup and maxPer will be considered in percentage of database)
                                                             (will consider "\t" as separator in both input and neighbourhood files)
             python3  FGPFPMiner_old.py sampleTDB.txt output.txt sampleN.txt 3 4 ','
                                                               (will consider "," as separator in both input and neighbourhood files)
     Sample run of importing the code:
     -------------------------------
-        from PAMI.fuzzySpatialPeriodicFrequentPattern import FGPFPMiner as alg
+        from PAMI.fuzzyGeoreferencedPeriodicFrequentPattern import FGPFPMiner as alg
         obj = alg.FFSPMiner("input.txt", "neighbours.txt", 3, 4)
         obj.startMine()
         print("Total number of fuzzy frequent spatial patterns:", len(obj.getPatterns()))
         obj.save("outputFile")
         print("Total Memory in USS:", obj.getMemoryUSS())
         print("Total Memory in RSS", obj.getMemoryRSS())
         print("Total ExecutionTime in seconds:", obj.getRuntime())
@@ -284,14 +295,18 @@
                             self._LabelKey[ub_Label.capitalize()] = count
                             count += 1
         except IOError:
             print("File Not Found")
             quit()
 
     def _creatingItemSets(self):
+        """
+        Storing the complete transactions of the database/input file in a database variable
+
+        """
         self._transactionsDB, self._fuzzyValuesDB = [], []
         if isinstance(self._iFile, _ab._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._transactionsDB = self._iFile['Transactions'].tolist()
@@ -366,14 +381,18 @@
                             self._mapItemNeighbours[item] = neigh1
                 except IOError:
                     print(self._nFile)
                     print("File Not Found")
                     quit()
 
     def _Regions(self, quantity):
+        """
+        param quantity:
+        type quantity:
+        """
 
         self._list = [0] * len(self._LabelKey)
         if self._RegionsCal[0][0] < quantity <= self._RegionsCal[0][1]:
             self._list[0] = 1
             return
         elif quantity >= self._RegionsCal[-1][0]:
             self._list[-1] = 1
@@ -431,16 +450,16 @@
                         self._itemSupData[item] = self._fuzzyRegionReferenceMap[fuzzy_ref]
 
         for item in self._tidList.keys():
             self._tidList[item].append(len(self._transactionsDB) - recent_occur[item][-1])
         del recent_occur
         """
             Using Maximum Scalar Cardinality Value strategy to narrow down search space and generate candidate fuzzy periodic-frequent items. 
-            Step1. Identify the regional representative (region with max support). This is the representative that will be tested to see if its greater than given minsup
-            Step2. prune out all items whose regional support is less than the given minsup
+            Step1. Identify the regional representative (region with max support). This is the representative that will be tested to see if its greater than given minSup
+            Step2. prune out all items whose regional support is less than the given minSup
             Step3. At the end, sort the list of stored Candidate Frequent-Periodic Patterns in ascending order
         """
 
         listOfFFList = []
         mapItemsToFFLIST = {}
         region_label = []
         for i in range(0, len(self._RegionsLabel)):
@@ -626,16 +645,16 @@
     def _WriteOut(self, prefix, prefixLen, _FFListObject, sumIUtil):
         """
             To Store the patten
             :param prefix: prefix of itemSet
             :type prefix: list
             :param prefixLen: length of prefix
             :type prefixLen: int
-            :param item: the last item
-            :type item: int
+            :param _FFListObject: the last item
+            :type _FFListObject: int
             :param sumIUtil: sum of utility of itemSet
             :type sumIUtil: float
         """
         item = _FFListObject.item
         self._itemsCnt += 1
         res = ""
         for i in range(0, prefixLen):
@@ -664,26 +683,28 @@
         """ Function to send the set of frequent patterns after completion of the mining process
         :return: returning frequent patterns
         :rtype: dict
         """
         return self._finalPeriodicPatterns
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
+        """Complete set of frequent patterns will be loaded in to an output file
         :param outFile: name of the output file
         :type outFile: file
         """
         self.oFile = outFile
         keylist = (self._finalPatterns.keys())
         writer = open(self.oFile, 'w+')
         for x in keylist:
             patternsAndSupport = x.strip() + ":" + str(self._finalPatterns[x])
             writer.write("%s \n" % patternsAndSupport)
 
     def printResults(self):
+        """ this function is used to print the results
+        """
         print("Total number of Spatial Fuzzy Periodic-Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
     '''def getPatternsAsDataframe(self):
```

### Comparing `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py` & `pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.geoReferenceFrequentPattern.basic import GFPGrowth as alg
+#     from PAMI.uncertainGeoreferenceFrequentPattern.basic import GFPGrowth as alg
 #
 #     obj = alg.GFPGrowth(iFile, nFile, minSup)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -45,15 +45,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 # from geoReferencedFrequentPatterns import abstract as _ab
-from PAMI.geoReferencedFrequentPaterns import abstract as _ab
+from PAMI.uncertainGeoreferencedFrequentPattern.basic import abstract as _ab
 # import abstract as _ab
 
 _minSup = str()
 _neighbourList = {}
 _ab._sys.setrecursionlimit(20000)
 _finalPatterns = {}
 
@@ -296,18 +296,22 @@
             self.removeNode(i)
 
 
 class GFPGrowth(_ab._frequentPatterns):
     """
     Description:
     ------------
-        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
+        GFPGrowth algorithm is used to discover geo-referenced frequent patterns in a uncertain transactional database
         using GFP-Tree.
     Reference:
     -----------
+         Palla Likhitha,Pamalla Veena, Rage, Uday Kiran, Koji Zettsu (2023).
+         "Discovering Geo-referenced Frequent Patterns in Uncertain Geo-referenced
+         Transactional Databases".  PAKDD 2023.
+         https://doi.org/10.1007/978-3-031-33380-4_3
         
     Attributes:
     ----------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
@@ -376,15 +380,15 @@
         ------------
           >>> python3 GFPGrowth.py sampleTDB.txt sampleNeighbor.txt patterns.txt 3    (minSup  will be considered in support count or frequency)
     
     Sample run of importing the code:
     -----------------------------------
      .. code-block:: python
 
-        from PAMI.geoReferenceFrequentPattern.basic import GFPGrowth as alg
+        from PAMI.uncertainGeoreferencedFrequentPattern.basic import GFPGrowth as alg
 
         obj = alg.GFPGrowth(iFile, nFile, minSup)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py` & `pami-2023.8.1/PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,9 +132,7 @@
         pass
       
     @_abstractmethod
     def printResults(self):
         """To print all the statistics"""
 
         pass
-
-
```

### Comparing `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py` & `pami-2023.8.1/PAMI/georeferencedFrequentSequencePattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py` & `pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/HUFIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
+#     from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
 #
 #     ob j =alg.HUFIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -45,15 +45,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.highUtilityFrequentPatterns.basic import abstract as _ab
+from PAMI.highUtilityFrequentPattern.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -396,15 +396,15 @@
 
             >>>  python3 HUFIM.py sampleTDB.txt output.txt 35 20 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityFrequentPatterns.basic import HUFIM as alg
+        from PAMI.highUtilityFrequentPattern.basic import HUFIM as alg
 
         obj=alg.HUFIM("input.txt", 35, 20)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/highUtilityFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
 #
-#         from PAMI.highUtilityFrequentSpatialPattern.basic import SHUFIM as alg
+#         from PAMI.highUtilityGeoreferencedFrequentPattern.basic import SHUFIM as alg
 #
 #         obj=alg.SHUFIM("input.txt","Neighbours.txt",35,20)
 #
 #         obj.startMine()
 #
 #         patterns = obj.getPatterns()
 #
@@ -44,15 +44,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.highUtilityFrequentSpatialPattern.basic import abstract as _ab
+from PAMI.highUtilityGeoreferencedFrequentPattern.basic import abstract as _ab
 from functools import cmp_to_key as _comToKey
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -411,15 +411,15 @@
         ------
           >>> python3 SHUFIM.py sampleTDB.txt output.txt sampleN.txt 35 20 (it will consider "\t" as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityFrequentSpatialPattern.basic import SHUFIM as alg
+        from PAMI.highUtilityGeoreferencedFrequentPattern.basic import SHUFIM as alg
 
         obj=alg.SHUFIM("input.txt","Neighbours.txt",35,20)
 
         obj.startMine()
 
         patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py` & `pami-2023.8.1/PAMI/highUtilityPattern/basic/EFIM.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#         from PAMI.highUtilityPatterns.basic import EFIM as alg
+#         from PAMI.highUtilityPattern.basic import EFIM as alg
 #
 #         obj=alg.EFIM("input.txt",35)
 #
 #         obj.startMine()
 #
 #         Patterns = obj.getPatterns()
 #
@@ -44,15 +44,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPatterns.basic import abstract as _ab
+from PAMI.highUtilityPattern.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -373,15 +373,15 @@
            >>> python3 EFIM sampleTDB.txt output.txt 35  (it will consider "\t" as separator)
            >>> python3 EFIM sampleTDB.txt output.txt 35 , (it will consider "," as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
         
-        from PAMI.highUtilityPatterns.basic import EFIM as alg
+        from PAMI.highUtilityPattern.basic import EFIM as alg
 
         obj=alg.EFIM("input.txt",35)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py` & `pami-2023.8.1/PAMI/highUtilityPattern/basic/HMiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPatterns.basic import HMiner as alg
+#     from PAMI.highUtilityPattern.basic import HMiner as alg
 #
 #     obj = alg.HMiner("input.txt", 35)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPatterns.basic import abstract as _ab
+from PAMI.highUtilityPattern.basic import abstract as _ab
 
 
 class _Element:
     """
     A class represents an Element of a utility list .
     Attributes :
     ----------
@@ -199,15 +199,15 @@
 
             >>> python3 HMiner.py sampleTDB.txt output.txt 35 (separator will be "\t")
 
     Sample run of importing the code:
     --------------------------------------
     .. code-block:: python
 
-        from PAMI.highUtilityPatterns.basic import HMiner as alg
+        from PAMI.highUtilityPattern.basic import HMiner as alg
         
         obj = alg.HMiner("input.txt",35)
         
         obj.startMine()
         
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py` & `pami-2023.8.1/PAMI/highUtilityPattern/basic/UPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityPatterns.basic import UPGrowth as alg
+#     from PAMI.highUtilityPattern.basic import UPGrowth as alg
 #
 #     obj=alg.UPGrowth("input.txt",35)
 #
 #     obj.startMine()
 #
-#     highUtilityPatterns = obj.getPatterns()
+#     highUtilityPattern = obj.getPatterns()
 #
-#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
+#     print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
 #
 #     obj.save("output")
 #
 #     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
@@ -42,15 +42,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPatterns.basic import abstract as _ab
+from PAMI.highUtilityPattern.basic import abstract as _ab
 
 
 class _UPItem:
     """
     A class to represent the UPItem
 
     Attribute :
@@ -379,23 +379,23 @@
         ------------
           >>> python3 UPGrowth sampleTDB.txt output.txt sampleN.txt 35  (it will consider "\t" as separator)
 
     Sample run of importing the code:
     -------------------------------------
     .. code-block:: python
     
-        from PAMI.highUtilityPatterns.basic import UPGrowth as alg
+        from PAMI.highUtilityPattern.basic import UPGrowth as alg
 
         obj=alg.UPGrowth("input.txt",35)
 
         obj.startMine()
 
-        highUtilityPatterns = obj.getPatterns()
+        highUtilityPattern = obj.getPatterns()
 
-        print("Total number of Spatial Frequent Patterns:", len(highUtilityPatterns))
+        print("Total number of Spatial Frequent Patterns:", len(highUtilityPattern))
 
         obj.save("output")
 
         memUSS = obj.getMemoryUSS()
 
         print("Total Memory in USS:", memUSS)
```

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/highUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py` & `pami-2023.8.1/PAMI/highUtilityPattern/basic/efimParallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPatterns.basic import abstract as _ab
+from PAMI.highUtilityPattern.basic import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py` & `pami-2023.8.1/PAMI/highUtilityPattern/parallel/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py` & `pami-2023.8.1/PAMI/highUtilityPattern/parallel/efimparallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.highUtilityPatterns.parallel import abstract as _ab
+from PAMI.highUtilityPattern.parallel import abstract as _ab
 
 class efimParallel(_ab._utilityPatterns):
     """
     Description:
     -----------
     EFIM is one of the fastest algorithm to mine High Utility ItemSets from transactional databases.
```

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.highUtilityFrequentSpatialPattern.basic import HDSHUIM as alg
+#     from PAMI.highUtilityGeoreferencedFrequentPattern.basic import HDSHUIM as alg
 #
 #     obj=alg.HDSHUIM("input.txt","Neighbours.txt",35)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -213,15 +213,15 @@
 
             >>> python3 HDSHUIM.py sampleTDB.txt output.txt sampleN.txt 35 , (separator will be "," in both input and neighbourhood file)
 
     Sample run of importing the code:
     -----------------------------------
     .. code-block:: python
         
-        from PAMI.highUtilityFrequentSpatialPattern.basic import HDSHUIM as alg
+        from PAMI.highUtilityGeoreferencedFrequentPattern.basic import HDSHUIM as alg
 
         obj=alg.HDSHUIM("input.txt","Neighbours.txt",35)
 
         obj.startMine()
 
         Patterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.8.1/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.8.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+
+
+
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
+#     from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowthPlus as alg
 #
-#     from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowth as alg
-#
-#     obj = alg.CFPGrowth(iFile, mIS)
+#     obj = alg.CFPGrowthPlus(iFile, mIS)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -44,19 +46,18 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-
 from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import abstract as _fp
 
 _fp._sys.setrecursionlimit(20000)
-_MIS = {}
+MIS = {}
 
 class _Node:
     """
         A class used to represent the node of frequentPatternTree
 
     Attributes:
     ----------
@@ -225,48 +226,48 @@
         prefix: an empty list
 
         Returns
         -------
         Frequent patterns that are extracted from fp-tree
 
         """
-        global _MIS
+        global MIS
         for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
             pattern = prefix[:]
             pattern.append(i)
             sup = []
             for j in pattern:
-                sup.append(_MIS[j])
+                sup.append(MIS[j])
             if self.info[i] >= min(sup):
                 yield pattern, self.info[i]
             patterns, freq, info = self.getFinalConditionalPatterns(i)
             conditionalTree = _Tree()
             conditionalTree.info = info.copy()
             for pat in range(len(patterns)):
                 conditionalTree.addTransaction(patterns[pat], freq[pat])
             if len(patterns) > 0:
                 for q in conditionalTree.generatePatterns(pattern):
                     yield q
 
 
-class CFPGrowth(_fp._frequentPatterns):
+class CFPGrowthPlus(_fp._frequentPatterns):
     """
-    Description:
-    ------------------
 
-       CFPGrowth is one of the fundamental algorithm to discover frequent patterns based on multiple minimum support in a transactional database.
+    Description:
+    ------------
+       CFPGrowthPlus is one of the fundamental algorithm to discover frequent patterns based on multiple minimum support in a transactional database.
 
-    Reference :
-    ---------
-        Ya-Han Hu and Yen-Liang Chen. 2006. Mining association rules with multiple minimum supports: a new mining algorithm and a support tuning mechanism.
-        Decis. Support Syst. 42, 1 (October 2006), 1–24. https://doi.org/10.1016/j.dss.2004.09.007
+    Reference:
+    ---------------
+        R. Uday Kiran P. Krishna Reddy Novel techniques to reduce search space in multiple minimum supports-based frequent
+        pattern mining algorithms. 11-20 2011 EDBT https://doi.org/10.1145/1951365.1951370
 
 
-    Attributes :
-    ----------
+    Attributes:
+    -------------
         iFile : file
             Input file name or path of the input file
         MIS: file or dictionary
             Multiple minimum supports of all items in the database
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
@@ -288,15 +289,15 @@
             it represents the total no of transactions
         tree : class
             it represents the Tree class
         finalPatterns : dict
             it represents to store the patterns
 
     Methods :
-    ----------------
+    ----------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -309,35 +310,35 @@
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets()
             Scans the dataset or dataframes and stores in list format
         frequentOneItem()
             Extracts the one-frequent patterns from transactions
 
     Executing the code on terminal:
-    ----------------------------------
+    -------------------------------
         Format:
         -------
-            >>> python3 CFPGrowth.py <inputFile> <outputFile>
+            >>> python3 CFPGrowthPlus.py <inputFile> <outputFile> <minSup>
 
         Examples:
         ---------
-            >>> python3 CFPGrowth.py sampleDB.txt patterns.txt MISFile.txt
+            >>> python3 CFPGrowthPlus.py sampleDB.txt patterns.txt MIS
 
-            >>> python3 CFPGrowth.py sampleDB.txt patterns.txt MISFile.txt
+            >>> python3 CFPGrowthPlus.py sampleDB.txt patterns.txt MIS
 
-            >>> python3 CFPGrowth.py sampleTDB.txt output.txt sampleN.txt MIS ',' (it will consider "," as a separator)
+            >>> python3 CFPGrowthPlus.py sampleTDB.txt output.txt sampleN.txt MIS ',' (it will consider "," as a separator)
 
 
     Sample run of the importing code:
     --------------------------------------
+    .. code-block:: python
 
+        from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowthPlus as alg
 
-        from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowth as alg
-
-        obj = alg.CFPGrowth(iFile, mIS)
+        obj = alg.CFPGrowthPlus(iFile, mIS)
 
         obj.startMine()
 
         frequentPatterns = obj.getPatterns()
 
         print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -354,18 +355,18 @@
         print("Total Memory in RSS", memRSS)
 
         run = obj.getRuntime()
 
         print("Total ExecutionTime in seconds:", run)
 
     Credits:
-    -------
+    ---------
         The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
 
-    """
+        """
 
     __startTime = float()
     __endTime = float()
     _MIS = str
     __finalPatterns = {}
     _iFile = " "
     _oFile = " "
@@ -407,17 +408,16 @@
                     temp = [x for x in temp if x]
                     self.__Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line = line.strip()
-                            temp = [i.rstrip() for i in line.split('\t')]
+                            temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            # print(temp)
                             self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _getMISValues(self):
         """
@@ -451,15 +451,14 @@
                 try:
                     with open(self._MIS, 'r', encoding='utf-8') as f:
                         for line in f:
                             line = line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._MISValues[temp[0]] = int(temp[1])
-                    print(len(self._MISValues))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def __convert(self, value):
         """
         to convert the type of user specified minSup value
@@ -483,24 +482,20 @@
     def __frequentOneItem(self):
         """
         Generating One frequent items sets
 
         """
         self.__mapSupport = {}
         for tr in self.__Database:
-            for i in range(len(tr)):
+            for i in range(1, len(tr)):
                 if tr[i] not in self.__mapSupport:
                     self.__mapSupport[tr[i]] = 1
                 else:
                     self.__mapSupport[tr[i]] += 1
-        # for x, y in self.__mapSupport.items():
-        #     print(x, y)
         self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= min(self._MISValues.values())}
-        # for x, y in self.__mapSupport.items():
-        #     print(x, y)
         genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
         return genList
 
     def __updateTransactions(self, itemSet):
         """
         Updates the items in transactions with rank of items according to their support
@@ -564,34 +559,33 @@
         return temp
 
     def startMine(self):
         """
             main program to start the operation
 
         """
-        global _MIS
+        global MIS
         self.__startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         self.__creatingItemSets()
         self._getMISValues()
-        #MIS = self._MISValues
         itemSet = self.__frequentOneItem()
         updatedTransactions = self.__updateTransactions(itemSet)
         for x, y in self.__rank.items():
-            _MIS[y] = self._MISValues[x]
+            MIS[y] = self._MISValues[x]
             self.__rankDup[y] = x
         info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
         __Tree = self.__buildTree(updatedTransactions, info)
         patterns = __Tree.generatePatterns([])
         self.__finalPatterns = {}
         for k in patterns:
             s = self.__savePeriodic(k[0])
             self.__finalPatterns[str(s)] = k[1]
-        print("Frequent patterns were generated successfully using CFPGrowth algorithm")
+        print("Frequent patterns were generated successfully using frequentPatternGrowth algorithm")
         self.__endTime = _fp._time.time()
         self.__memoryUSS = float()
         self.__memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
         self.__memoryUSS = process.memory_full_info().uss
         self.__memoryRSS = process.memory_info().rss
 
@@ -666,29 +660,23 @@
     def printResults(self):
         print("Total number of  Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
+
 if __name__ == "__main__":
     _ap = str()
     if len(_fp._sys.argv) == 4 or len(_fp._sys.argv) == 5:
         if len(_fp._sys.argv) == 5:
-            _ap = CFPGrowth(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4])
+            _ap = CFPGrowthPlus(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4])
         if len(_fp._sys.argv) == 4:
-            _ap = CFPGrowth(_fp._sys.argv[1], _fp._sys.argv[3])
+            _ap = CFPGrowthPlus(_fp._sys.argv[1], _fp._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        _ap = CFPGrowth('/Users/Likhitha/Downloads/Transactional_T10I4D100K-3.csv', '/Users/Likhitha/Downloads/MIS_T10I4D100K_.csv', '\t')
-        _ap.startMine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save('/Users/Likhitha/Downloads/CFPGrowth_output.txt')
-        print("Total Memory in USS:", _ap.getMemoryUSS())
-        print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-
-
-
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowthPlus as alg
 #
-#     obj = alg.CFPGrowthPlus(iFile, mIS)
+#     from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import basic as alg
+#
+#     obj = alg.basic(iFile, mIS)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -46,18 +44,19 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
+
 from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import abstract as _fp
 
 _fp._sys.setrecursionlimit(20000)
-MIS = {}
+_MIS = {}
 
 class _Node:
     """
         A class used to represent the node of frequentPatternTree
 
     Attributes:
     ----------
@@ -226,48 +225,48 @@
         prefix: an empty list
 
         Returns
         -------
         Frequent patterns that are extracted from fp-tree
 
         """
-        global MIS
+        global _MIS
         for i in sorted(self.summaries, key=lambda x: (self.info.get(x), -x)):
             pattern = prefix[:]
             pattern.append(i)
             sup = []
             for j in pattern:
-                sup.append(MIS[j])
+                sup.append(_MIS[j])
             if self.info[i] >= min(sup):
                 yield pattern, self.info[i]
             patterns, freq, info = self.getFinalConditionalPatterns(i)
             conditionalTree = _Tree()
             conditionalTree.info = info.copy()
             for pat in range(len(patterns)):
                 conditionalTree.addTransaction(patterns[pat], freq[pat])
             if len(patterns) > 0:
                 for q in conditionalTree.generatePatterns(pattern):
                     yield q
 
 
-class CFPGrowthPlus(_fp._frequentPatterns):
+class CFPGrowth(_fp._frequentPatterns):
     """
-
     Description:
-    ------------
-       CFPGrowthPlus is one of the fundamental algorithm to discover frequent patterns based on multiple minimum support in a transactional database.
+    ------------------
 
-    Reference:
-    ---------------
-        R. Uday Kiran P. Krishna Reddy Novel techniques to reduce search space in multiple minimum supports-based frequent
-        pattern mining algorithms. 11-20 2011 EDBT https://doi.org/10.1145/1951365.1951370
+       basic is one of the fundamental algorithm to discover frequent patterns based on multiple minimum support in a transactional database.
 
+    Reference :
+    ---------
+        Ya-Han Hu and Yen-Liang Chen. 2006. Mining association rules with multiple minimum supports: a new mining algorithm and a support tuning mechanism.
+        Decis. Support Syst. 42, 1 (October 2006), 1–24. https://doi.org/10.1016/j.dss.2004.09.007
 
-    Attributes:
-    -------------
+
+    Attributes :
+    ----------
         iFile : file
             Input file name or path of the input file
         MIS: file or dictionary
             Multiple minimum supports of all items in the database
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
@@ -289,15 +288,15 @@
             it represents the total no of transactions
         tree : class
             it represents the Tree class
         finalPatterns : dict
             it represents to store the patterns
 
     Methods :
-    ----------
+    ----------------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
@@ -310,35 +309,35 @@
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets()
             Scans the dataset or dataframes and stores in list format
         frequentOneItem()
             Extracts the one-frequent patterns from transactions
 
     Executing the code on terminal:
-    -------------------------------
+    ----------------------------------
         Format:
         -------
-            >>> python3 CFPGrowthPlus.py <inputFile> <outputFile> <minSup>
+            >>> python3 basic.py <inputFile> <outputFile>
 
         Examples:
         ---------
-            >>> python3 CFPGrowthPlus.py sampleDB.txt patterns.txt MIS
+            >>> python3 basic.py sampleDB.txt patterns.txt MISFile.txt
 
-            >>> python3 CFPGrowthPlus.py sampleDB.txt patterns.txt MIS
+            >>> python3 basic.py sampleDB.txt patterns.txt MISFile.txt
 
-            >>> python3 CFPGrowthPlus.py sampleTDB.txt output.txt sampleN.txt MIS ',' (it will consider "," as a separator)
+            >>> python3 basic.py sampleTDB.txt output.txt sampleN.txt MIS ',' (it will consider "," as a separator)
 
 
     Sample run of the importing code:
     --------------------------------------
-    .. code-block:: python
 
-        from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import CFPGrowthPlus as alg
 
-        obj = alg.CFPGrowthPlus(iFile, mIS)
+        from PAMI.multipleMinimumSupportBasedFrequentPattern.basic import basic as alg
+
+        obj = alg.basic(iFile, mIS)
 
         obj.startMine()
 
         frequentPatterns = obj.getPatterns()
 
         print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -355,18 +354,18 @@
         print("Total Memory in RSS", memRSS)
 
         run = obj.getRuntime()
 
         print("Total ExecutionTime in seconds:", run)
 
     Credits:
-    ---------
+    -------
         The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.\n
 
-        """
+    """
 
     __startTime = float()
     __endTime = float()
     _MIS = str
     __finalPatterns = {}
     _iFile = " "
     _oFile = " "
@@ -408,16 +407,17 @@
                     temp = [x for x in temp if x]
                     self.__Database.append(temp)
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
                             line = line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [i.rstrip() for i in line.split('\t')]
                             temp = [x for x in temp if x]
+                            # print(temp)
                             self.__Database.append(temp)
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def _getMISValues(self):
         """
@@ -451,14 +451,15 @@
                 try:
                     with open(self._MIS, 'r', encoding='utf-8') as f:
                         for line in f:
                             line = line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
                             self._MISValues[temp[0]] = int(temp[1])
+                    print(len(self._MISValues))
                 except IOError:
                     print("File Not Found")
                     quit()
 
     def __convert(self, value):
         """
         to convert the type of user specified minSup value
@@ -482,20 +483,24 @@
     def __frequentOneItem(self):
         """
         Generating One frequent items sets
 
         """
         self.__mapSupport = {}
         for tr in self.__Database:
-            for i in range(1, len(tr)):
+            for i in range(len(tr)):
                 if tr[i] not in self.__mapSupport:
                     self.__mapSupport[tr[i]] = 1
                 else:
                     self.__mapSupport[tr[i]] += 1
+        # for x, y in self.__mapSupport.items():
+        #     print(x, y)
         self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= min(self._MISValues.values())}
+        # for x, y in self.__mapSupport.items():
+        #     print(x, y)
         genList = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
         self.__rank = dict([(index, item) for (item, index) in enumerate(genList)])
         return genList
 
     def __updateTransactions(self, itemSet):
         """
         Updates the items in transactions with rank of items according to their support
@@ -559,33 +564,34 @@
         return temp
 
     def startMine(self):
         """
             main program to start the operation
 
         """
-        global MIS
+        global _MIS
         self.__startTime = _fp._time.time()
         if self._iFile is None:
             raise Exception("Please enter the file path or file name:")
         self.__creatingItemSets()
         self._getMISValues()
+        #MIS = self._MISValues
         itemSet = self.__frequentOneItem()
         updatedTransactions = self.__updateTransactions(itemSet)
         for x, y in self.__rank.items():
-            MIS[y] = self._MISValues[x]
+            _MIS[y] = self._MISValues[x]
             self.__rankDup[y] = x
         info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
         __Tree = self.__buildTree(updatedTransactions, info)
         patterns = __Tree.generatePatterns([])
         self.__finalPatterns = {}
         for k in patterns:
             s = self.__savePeriodic(k[0])
             self.__finalPatterns[str(s)] = k[1]
-        print("Frequent patterns were generated successfully using frequentPatternGrowth algorithm")
+        print("Frequent patterns were generated successfully using basic algorithm")
         self.__endTime = _fp._time.time()
         self.__memoryUSS = float()
         self.__memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
         self.__memoryUSS = process.memory_full_info().uss
         self.__memoryRSS = process.memory_info().rss
 
@@ -660,23 +666,29 @@
     def printResults(self):
         print("Total number of  Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
-
 if __name__ == "__main__":
     _ap = str()
     if len(_fp._sys.argv) == 4 or len(_fp._sys.argv) == 5:
         if len(_fp._sys.argv) == 5:
-            _ap = CFPGrowthPlus(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4])
+            _ap = CFPGrowth(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4])
         if len(_fp._sys.argv) == 4:
-            _ap = CFPGrowthPlus(_fp._sys.argv[1], _fp._sys.argv[3])
+            _ap = CFPGrowth(_fp._sys.argv[1], _fp._sys.argv[3])
         _ap.startMine()
         print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = CFPGrowth('/Users/Likhitha/Downloads/Transactional_T10I4D100K-3.csv', '/Users/Likhitha/Downloads/MIS_T10I4D100K_.csv', '\t')
+        _ap.startMine()
+        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save('/Users/Likhitha/Downloads/CFPGrowth_output.txt')
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.partialPeriodicPattern.timeSeries import abstract as _ab
+from PAMI.partialPeriodicPatternInMultipleTimeSeries import abstract as _ab
 
 
 
 _lno = int()
 _periodicSupport = float()
 _period = float()
```

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.8.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
-#     import PAMI.partialPeriodicSpatialPattern.STEclat as alg
+#     import PAMI.georeferencedPartialPeriodicPattern.STEclat as alg
 #
 #     obj = alg.STEclat("sampleTDB.txt", "sampleN.txt", 3, 4)
 #
 #     obj.startMine()
 #
 #     partialPeriodicSpatialPatterns = obj.getPatterns()
 #
@@ -43,15 +43,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.partialPeriodicSpatialPattern.basic import abstract as _ab
+from PAMI.georeferencedPartialPeriodicPattern.basic import abstract as _ab
 
 
 class STEclat(_ab._partialPeriodicSpatialPatterns):
     """
     Description:
     ------------
        PPGrowth is one of the fundamental algorithm to discover periodic-frequent patterns in a transactional database.
@@ -136,15 +136,15 @@
 
             >>> python3 STEclat.py sampleTDB.txt output.txt sampleN.txt 3 2 ',' (it will consider "," as a separator)
 
     Sample run of importing the code :
     -------------------------------
     .. code-block:: python
     
-        import PAMI.partialPeriodicSpatialPattern.STEclat as alg
+        import PAMI.georeferencedPartialPeriodicPattern.STEclat as alg
 
         obj = alg.STEclat("sampleTDB.txt", "sampleN.txt", 3, 4)
 
         obj.startMine()
 
         partialPeriodicSpatialPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,15 @@
             Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingOneItemSets()
-            Scan the database and store the items with their timestamps which are periodic frequent 
-        getPeriodAndSupport()
-            Calculates the support and period for a list of timestamps.
-        Generation()
-            Used to implement prefix class equivalence method to generate the periodic patterns recursively
+
             
 
     **Methods to execute code on terminal**
 
             Format:
                         >>>  python3 PFECLAT.py <inputFile> <outputFile> <minSup>
             Example:
@@ -263,16 +258,14 @@
                     return;
                 }
             }
         }
 
     }
     
-    
-    
     ''', 'supportAndPeriod')
 
     def _convert(self, value):
         """
         To convert the given user specified value
 
         :param value: user specified value
```

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     import PAMI.periodicFrequentPattern.kPFPMiner as alg
+#     from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 #
-#     obj = alg.kPFPMiner(iFile, k)
+#     obj = alg.TUFP(iFile, minSup)
 #
 #     obj.startMine()
 #
-#     periodicFrequentPatterns = obj.getPatterns()
+#     frequentPatterns = obj.getPatterns()
 #
-#     print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+#     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
-#     obj.save(oFile)
+#     obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternInDataFrame()
+#     Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#     memUSS = obj.getmemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
@@ -44,257 +44,314 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.periodicFrequentPattern.topk.kPFPMiner import abstract as _ab
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
 
+_minSup = float()
+_finalPatterns = {}
 
-class kPFPMiner(_ab._periodicFrequentPatterns):
+
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+
+    ...
+
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
     """
-        Description:
-        ------------
 
-            Top - K is and algorithm to discover top periodic-frequent patterns in a temporal database.
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
+
+
+class TUFP(_ab._frequentPatterns):
+    """
+    Description:
+    -------------
+        It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database
+        using CUP-Lists.
+
+    Reference:
+    ----------
+        Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
+        Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
+
+    Attributes:
+    ------------
+        iFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup: float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            To represent the total no of transaction
+        tree : class
+            To represents the Tree class
+        itemSetCount : int
+            To represents the total no of patterns
+        finalPatterns : dict
+            To store the complete patterns
+    Methods:
+    ---------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        storePatternsInFile(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsInDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
-        Reference:
-        -----------
-            Likhitha, P., Ravikumar, P., Kiran, R.U., Watanobe, Y. (2022).
-            Discovering Top-k Periodic-Frequent Patterns in Very Large Temporal Databases. Big Data Analytics.
-            BDA 2022. Lecture Notes in Computer Science, vol 13773. Springer, Cham. https://doi.org/10.1007/978-3-031-24094-2_14
-
-        Attributes:
-        -----------
-            iFile : str
-                Input file name or path of the input file
-            k: int
-                User specified counte of top-k periodic frequent patterns
-            sep : str
-                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-                However, the users can override their default separator.
-            oFile : str
-                Name of the output file or the path of the output file
-            startTime:float
-                To record the start time of the mining process
-            endTime:float
-                To record the completion time of the mining process
-            finalPatterns: dict
-                Storing the complete set of patterns in a dictionary variable
-            memoryUSS : float
-                To store the total amount of USS memory consumed by the program
-            memoryRSS : float
-                To store the total amount of RSS memory consumed by the program
-
-        Methods:
-        ---------
-            startMine()
-                Mining process will start from here
-            getPatterns()
-                Complete set of patterns will be retrieved with this function
-            savePatterns(oFile)
-                Complete set of frequent patterns will be loaded in to a output file
-            getPatternsAsDataFrame()
-                Complete set of frequent patterns will be loaded in to a dataframe
-            getMemoryUSS()
-                Total amount of USS memory consumed by the mining process will be retrieved from this function
-            getMemoryRSS()
-                Total amount of RSS memory consumed by the mining process will be retrieved from this function
-            getRuntime()
-                Total amount of runtime taken by the mining process will be retrieved from this function
-            creatingItemSets()
-                Scans the dataset or dataframes and stores in list format
-            frequentOneItem()
-                Generates one frequent patterns
-            eclatGeneration(candidateList)
-                It will generate the combinations of frequent items
-            generateFrequentPatterns(tidList)
-                It will generate the combinations of frequent items from a list of items
 
-        Executing the code on terminal:
-        -------------------------------
+    **Methods to execute code on terminal**
 
             Format:
-            ------
-            >>> python3 kPFPMiner.py <inputFile> <outputFile> <k>
+                      >>> python3 TUFP.py <inputFile> <outputFile> <minSup>
+            Example:
+                      >>>  python3 TUFP.py sampleTDB.txt patterns.txt 0.6
 
-            Examples:
-            ---------
-            >>> python3 kPFPMiner.py sampleDB.txt patterns.txt 10
+            .. note:: minSup  will be considered in support count or frequency
 
+    **Importing this algorithm into a python program**
 
-        Sample run of the importing code:
-        ---------------------------------
-        .. code-block:: python
+    .. code-block:: python
 
-            import PAMI.periodicFrequentPattern.kPFPMiner as alg
+            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
 
-            obj = alg.kPFPMiner(iFile, k)
+            obj = alg.TUFP(iFile, minSup)
 
             obj.startMine()
 
-            periodicFrequentPatterns = obj.getPatterns()
+            frequentPatterns = obj.getPatterns()
 
-            print("Total number of top-k Periodic Frequent Patterns:", len(periodicFrequentPatterns))
+            print("Total number of Frequent Patterns:", len(frequentPatterns))
 
-            obj.save(oFile)
+            obj.savePatterns(oFile)
 
-            Df = obj.getPatternInDataFrame()
+            Df = obj.getPatternsAsDataFrame()
 
-            memUSS = obj.getMemoryUSS()
+            memUSS = obj.getmemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
-        Credits:
-        --------
-            The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+    **Credits:**
+
+             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
 
     """
 
     _startTime = float()
     _endTime = float()
-    _k = int()
+    _minSup = str()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _tidList = {}
-    lno = int()
-    _maximum = int()
+    _cupList = {}
+    _topk = {}
+    _minimum = 9999
 
     def _creatingItemSets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
-
+            Scans the dataset
         """
-
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
 
             # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-                    
-    def getPer_Sup(self, tids):
-        tids.sort()
-        cur=0
-        per=list()
-        sup=0
-        #print(tids)
-        for i in range(len(tids)-1):
-            j = i + 1
-            #if tids[j] - cur <= periodicity:
-                #return [0,0]
-            per.append(tids[j] - cur)
-            cur = tids[j]
-        per.append(self.lno - cur)
-        return max(per)
 
     def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
+
+                :param self.Database : it represents the one self.Database in database
+
+                :type self.Database : list
         """
-        Generating one frequent patterns
-        """
-        self._mapSupport = {}
-        self._tidList = {}
-        n = 0
-        for line in self._Database:
-            self.lno += 1
-            n = int(line[0])
-            for i in range(1, len(line)):
-                si = line[i]
-                if self._mapSupport.get(si) is None:
-                    self._mapSupport[si] = [1, abs(0 - n), n]
-                    self._tidList[si] = [n]
+
+        mapSupport = {}
+        k = 0
+        for i in self._Database:
+            k += 1
+            for j in i:
+                if j.item not in mapSupport:
+                    mapSupport[j.item] = j.probability
+                    self._cupList[j.item] = {k:j.probability}
                 else:
-                    self._mapSupport[si][0] += 1
-                    self._mapSupport[si][1] = max(self._mapSupport[si][1], abs(n - self._mapSupport[si][2]))
-                    self._mapSupport[si][2] = n
-                    self._tidList[si].append(n)
-        for x, y in self._mapSupport.items():
-            self._mapSupport[x][1] = max(self._mapSupport[x][1], abs(n - self._mapSupport[x][2]))
-        plist = [key for key, value in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        for i in plist:
-            if len(self._finalPatterns) >= self._k:
+                    mapSupport[j.item] += j.probability
+                    self._cupList[j.item].update({k: j.probability})
+        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        k = 0
+        for x, in plist:
+            k +=1
+            if k >= self._minSup:
                 break
-            else:
-                self._finalPatterns[i] = self._mapSupport[i][1]
-        self._maximum = max([self._finalPatterns[i] for i in self._finalPatterns.keys()])
-        plist = list(self._finalPatterns.keys())
+            self._finalPatterns[x] = mapSupport[x]
+        self._minimum = min(list(self._finalPatterns.values()))
         return plist
 
+    @staticmethod
+    def _convert(value):
+        """
+        To convert the type of user specified minSup value
+
+            :param value: user specified minSup value
+
+            :return: converted type minSup value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = float(value)
+        if type(value) is str:
+            if '.' in value:
+                value = float(value)
+            else:
+                value = int(value)
+        return value
 
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
 
             :param prefix: the prefix of a pattern
             :type prefix: list
             :param suffix: the suffix of a patterns
             :type suffix: list
             :param tidSetI: the timestamp of a patterns
-            :type tidSetI: list
+            :type tidSetI: dict
         """
 
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = self.getPer_Sup(tidSetI)
-        sample = str()
-        for i in prefix:
-            sample = sample + i + " "
-        if len(self._finalPatterns) < self._k:
-            if val < self._maximum:
+        val = sum(tidSetI.values())
+        #print(prefix, val)
+        if len(self._finalPatterns) <= self._minSup:
+            sample = str()
+            for i in prefix:
+                sample = sample + i + " "
+            self._finalPatterns[sample] = val
+        if len(self._finalPatterns) == self._minSup:
+            if val > self._minimum:
+                sample = str()
+                for i in prefix:
+                    sample = sample + i + " "
+                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
+                del self._finalPatterns[index]
                 self._finalPatterns[sample] = val
-                self._finalPatterns = {k: v for k, v in sorted(self._finalPatterns.items(), key=lambda item: item[1], reverse=True)}
-                self._maximum = max([i for i in self._finalPatterns.values()])
-        else:
-            for x, y in sorted(self._finalPatterns.items(), key=lambda x: x[1], reverse=True):
-                if val < y:
-                    del self._finalPatterns[x]
-                    self._finalPatterns[sample] = val
-                    self._finalPatterns = {k: v for k, v in
-                                              sorted(self._finalPatterns.items(), key=lambda item: item[1],
-                                                     reverse=True)}
-                    self._maximum = max([i for i in self._finalPatterns.values()])
-                    return
+                self._minimum = min(list(self._finalPatterns.values()))
+        #print(self.finalPatterns, self.minimum, self.minSup)
+
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
 
             :param prefix:  main equivalence prefix
             :type prefix: periodic-frequent item or pattern
             :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
@@ -306,92 +363,77 @@
 
                     """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
-        for i in range(len(itemSets)):
+        for i in range(0, len(itemSets)):
             itemI = itemSets[i]
             if itemI is None:
                 continue
             tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
+            for j in range(i+1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y) <= self._maximum:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
+                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
+                sum2 = sum(list(y.values()))
+                #print(prefix, itemJ, y, sum2)
+                #if sum2 >= self.minimum:
+                self._save(prefix, [itemJ], y)
+                classItemSets.append(itemJ)
+                classTidSets.append(y)
+            #print(itemI, tidSetI, classItemSets)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
-
-    def _convert(self, value):
-        """
-        to convert the type of user specified minSup value
-        :param value: user specified minSup value
-        :return: converted type
-        """
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self._Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = ((len(self._Database)) * value)
-            else:
-                value = int(value)
-        return value
+            #self.save(prefix, list(set(itemSetX)), tidSetI)
 
     def startMine(self):
-        """
-            Main function of the program
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
+
 
         """
+        global _minSup
         self._startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._k is None:
-            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._k = self._convert(self._k)
+        self._minSup = self._convert(self._minSup)
+        _minSup = self._minSup
         plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
-            tidSetI = self._tidList[itemI]
+            tidSetI = self._cupList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
-            for j in range(i + 1, len(plist)):
+            for j in range(i+1, len(plist)):
                 itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = list(set(tidSetI).intersection(tidSetJ))
-                if self.getPer_Sup(y1) <= self._maximum:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
+                tidSetJ = self._cupList[itemJ]
+                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
+                self._save(itemSetX, [itemJ], y1)
+                itemSets.append(itemJ)
+                tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print("kPFPMiner has successfully generated top-k frequent patterns")
+        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
         self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-                    :return: returning USS memory consumed by the mining process
+        :return: returning USS memory consumed by the mining process
 
-                    :rtype: float
+        :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
@@ -401,14 +443,15 @@
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
 
+
         :return: returning total amount of runtime taken by the mining process
 
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
@@ -416,64 +459,67 @@
         """Storing final frequent patterns in a dataframe
 
         :return: returning frequent patterns in a dataframe
 
         :rtype: pd.DataFrame
         """
 
-        dataFrame = {}
+        dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a, b])
-            dataFrame = _ab._pd.DataFrame(data, columns=['Patterns', 'periodicity'])
-        return dataFrame
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+        return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
 
         :param outFile: name of the output file
 
         :type outFile: file
         """
-        self._oFile = outFile
-        writer = open(self._oFile, 'w+')
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            patternsAndSupport = x + ":" + str(y)
-            writer.write("%s \n" % patternsAndSupport)
+            s1 = x + ":" + str(y)
+            writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
 
         :return: returning frequent patterns
 
         :rtype: dict
         """
         return self._finalPatterns
 
-    def printResults(self):
-        print("Total number of  Top-k Periodic Frequent Patterns:", len(self.getPatterns()))
-        print("Total Memory in USS:", self.getMemoryUSS())
-        print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
-
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = kPFPMiner(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
         _Patterns = _ap.getPatterns()
-        print("Total number of top-k periodic frequent patterns:", len(_Patterns))
+        print("Total number of Patterns:", len(_Patterns))
         _ap.save(_ab._sys.argv[2])
         _memUSS = _ap.getMemoryUSS()
         print("Total Memory in USS:", _memUSS)
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
+        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
+        ap.startMine()
+        Patterns = ap.getPatterns()
+        print("Total number of Patterns:", len(Patterns))
+        ap.save("patterns.txt")
+        memUSS = ap.getMemoryUSS()
+        print("Total Memory in USS:", memUSS)
+        memRSS = ap.getMemoryRSS()
+        print("Total Memory in RSS", memRSS)
+        run = ap.getRuntime()
+        print("Total ExecutionTime in ms:", run)'''
         print("Error! The number of input parameters do not match the total number of parameters provided")
-
-
```

### Comparing `pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.8.1/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,49 +8,47 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
+import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 
 
-class _recurringPatterns(_ABC):
+class _periodicFrequentPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
         employ in PAMI
-
        Attributes
         ----------
         iFile : str
             Input file name or path of the input file
-        
+        minSup: int or float or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         maxPer: int or float or str
             The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        minPS: int or float or str
-            The user can specify minPS either in count or proportion of database size.
-            If the program detects the data type of minPS is integer, then it treats minPS is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: minPS=10 will be treated as integer, while minPS=10.0 will be treated as float
-        minRec: int or float or str
-            The user has to specify minRec in count.
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -58,15 +56,14 @@
             Storing the complete set of patterns in a dictionary variable
         oFile : str
             Name of the output file to store complete set of periodic-frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-
         Methods
         -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
@@ -77,43 +74,42 @@
             Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, maxPer, minPS, minRec,sep = '\t'):
+    def __init__(self, iFile, minSup, maxPer, sep = '\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param maxPer: The user can specify maxPer either in count or proportion of database size.
             If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
             Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         :type maxPer: int or float or str
-        :param sep: the separator used in the database
-        :type sep: str
+        :param sep: The user specified seperator used in the input file
+        :type maxPer: str
         """
 
         self._iFile = iFile
-        self._minPS = minPS
+        self._minSup = minSup
         self._maxPer = maxPer
-        self._minRec = minRec
         self._sep = sep
         self._oFile = str()
         self._finalPatterns = {}
+        self._memoryUSS = float()
+        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
-        self._memoryRSS = float()
-        self._memoryUSS = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
@@ -122,15 +118,14 @@
         """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of periodic-frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
@@ -156,8 +151,8 @@
 
         pass
 
     @_abstractmethod
     def printResults(self):
         """ To print all the results of execution"""
 
-        pass
+        pass
```

### Comparing `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.frequentPatternUsingOtherMeasures import RSFPGrowth as alg
+#     from PAMI.uncertainFrequentPattern.basic import UFGrowth as alg
 #
-#     obj = alg.RSFPGrowth(iFile, minSup, __minRatio)
+#     obj = alg.UFGrowth(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -25,15 +24,14 @@
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -45,294 +43,302 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.relativeFrequentPatterns.basic import abstract as _ab
+from PAMI.uncertainFrequentPattern.basic import abstract as _ab
 
+_minSup = str()
+_ab._sys.setrecursionlimit(20000)
+_finalPatterns = {}
 
-class _Node:
+
+class _Item:
     """
-        A class used to represent the node of frequentPatterntree
+    A class used to represent the item with probability in transaction of dataset
+    ...
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
+
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
+
 
+class _Node(object):
+    """
+    A class used to represent the node of frequentPatternTree
+        ...
     Attributes:
     ----------
-        itemId: int
+        item : int
             storing item of a node
-        counter: int
-            To maintain the support of node
-        parent: node
+        probability : int
+            To maintain the expected support of node
+        parent : node
             To maintain the parent of every node
-        child: list
+        children : list
             To maintain the children of node
-        nodeLink : node
-            Points to the node with same itemId
-
     Methods:
     -------
-
-        getChild(itemName)
-            returns the node with same itemName from frequentPatterntree
+        addChild(itemName)
+            storing the children to their respective parent nodes
     """
 
     def __init__(self):
         self.itemId = -1
-        self.counter = 1
-        self.parent = None
+        self.counter = 0
+        self.probability = 0
         self.child = []
+        self.parent = None
         self.nodeLink = None
+        self.expSup = 0
 
-    def getChild(self, itemName):
-        """ Retrieving the child from the tree
-
-            :param itemName: name of the child
-            :type itemName: list
-            :return: returns the node with same itemName from frequentPatternTree
-            :rtype: None or Node
-
-        """
+    def getChild(self, id1):
         for i in self.child:
-            if i.itemId == itemName:
+            if i.itemid == id1:
                 return i
         return None
 
 
-class _Tree:
+class _Tree(object):
     """
-        A class used to represent the frequentPatternGrowth tree structure
-
+    A class used to represent the frequentPatternGrowth tree structure
+    ...
     Attributes:
     ----------
-        headerList : list
-            storing the list of items in tree sorted in ascending of their supports
-        mapItemNodes : dictionary
-            storing the nodes with same item name
-        mapItemLastNodes : dictionary
-            representing the map that indicates the last node for each item
         root : Node
-            representing the root Node in a tree
-
+            Represents the root node of the tree
+        summaries : dictionary
+            storing the nodes with same item name
+        info : dictionary
+            stores the support of items
     Methods:
     -------
-        createHeaderList(items,minSup)
-            takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
             creating transaction as a branch in frequentPatternTree
-        fixNodeLinks(item,newNode)
-            To create the link for nodes with same item
-        printTree(Node)
-            gives the details of node in frequentPatternGrowth tree
-        addPrefixPath(prefix,port,minSup)
-           It takes the items in prefix pattern whose support is >=minSup and construct a subtree
+        addConditionalPattern(prefixPaths, supportOfItems)
+            construct the conditional tree for prefix paths
+        conditionalPatterns(Node)
+            generates the conditional patterns from tree for specific node
+        conditionalTransactions(prefixPaths,Support)
+            takes the prefixPath of a node and support at child of the path and extract the frequent items from
+            prefixPaths and generates prefixPaths with items which are frequent
+        remove(Node)
+            removes the node from tree once after generating all the patterns respective to the node
+        generatePatterns(Node)
+            starts from the root node of the tree and mines the frequent patterns
     """
 
     def __init__(self):
         self.headerList = []
         self.mapItemNodes = {}
         self.mapItemLastNodes = {}
         self.root = _Node()
 
-    def addTransaction(self, transaction):
-        """adding transaction into tree
-
-        :param transaction: it represents the one transactions in database
-        :type transaction: list
-        """
+    def fixNodeLinks(self, item, newNode):
+        if item in self.mapItemLastNodes.keys():
+            lastNode = self.mapItemLastNodes[item]
+            lastNode.nodeLink = newNode
+        self.mapItemLastNodes[item] = newNode
+        if item not in self.mapItemNodes.keys():
+            self.mapItemNodes[item] = newNode
 
-        # This method taken a transaction as input and returns the tree
+    def addTransaction(self, transaction):
+        y = 0
         current = self.root
         for i in transaction:
-            child = current.getChild(i)
-            if not child:
+            child = current.getChild(i.item)
+            if child is None:
                 newNode = _Node()
-                newNode.itemId = i
+                newNode.counter = 1
+                newNode.probability = i.probability
+                newNode.itemId = i.item
+                newNode.expSup = i.probability
                 newNode.parent = current
                 current.child.append(newNode)
-                self.fixNodeLinks(i, newNode)
+                self.fixNodeLinks(i.item, newNode)
                 current = newNode
             else:
-                child.counter += 1
-                current = child
-
-    def fixNodeLinks(self, item, newNode):
-        """Fixing node link for the newNode that inserted into frequentPatternTree
-
-        :param item: it represents the item of newNode
-        :type item: int
-        :param newNode: it represents the newNode that inserted in frequentPatternTree
-        :type newNode: Node
-
-        """
-        if item in self.mapItemLastNodes.keys():
-            lastNode = self.mapItemLastNodes[item]
-            lastNode.nodeLink = newNode
-        self.mapItemLastNodes[item] = newNode
-        if item not in self.mapItemNodes.keys():
-            self.mapItemNodes[item] = newNode
+                if child.probability == i.probability:
+                    child.counter += 1
+                    current = child
+                else:
+                    newNode = _Node()
+                    newNode.counter = 1
+                    newNode.itemId = i.item
+                    newNode.probability = i.probability
+                    newNode.expSup = i.probability
+                    newNode.parent = current
+                    current.child.append(newNode)
+                    self.fixNodeLinks(i.item, newNode)
+                    current = newNode
+        return y
 
     def printTree(self, root):
-        """Print the details of Node in frequentPatternTree
-
-        :param root: it represents the Node in frequentPatternTree
-        :type root: Node
-
-        """
-
-        # this method is used print the details of tree
-        if not root.child:
+        if root.child is []:
             return
         else:
             for i in root.child:
-                print(i.itemId, i.counter, i.parent.itemId)
+                print(i.itemid, i.counter)
                 self.printTree(i)
 
-    def createHeaderList(self, __mapSupport, minSup):
-        """To create the headerList
+    def update(self, mapSup, u1):
+        t1 = []
+        for i in mapSup:
+            if i in u1:
+                t1.append(i)
+        return t1
 
-        :param __mapSupport: it represents the items with their supports
-        :type __mapSupport: dictionary
-        :param minSup: it represents the minSup
-        :param minSup: float
-        """
-        # the frequentPatternTree always maintains the header table to start the mining from leaf nodes
+    def createHeaderList(self, mapSupport, min_sup):
         t1 = []
-        for x, y in __mapSupport.items():
-            if y >= minSup:
+        for x, y in mapSupport.items():
+            if y >= min_sup:
                 t1.append(x)
-        __itemSetBuffer = [k for k, v in sorted(__mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.headerList = [i for i in t1 if i in __itemSetBuffer]
+        mapSup = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.headerList = self.update(mapSup, t1)
 
-    def addPrefixPath(self, prefix, __mapSupportBeta, minSup):
-        """To construct the conditional tree with prefix paths of a node in frequentPatternTree
-
-        :param prefix: it represents the prefix items of a Node
-        :type prefix: list
-        :param __mapSupportBeta: it represents the items with their supports
-        :param __mapSupportBeta: dictionary
-        :param minSup: to check the item meets with minSup
-        :param minSup: float
-        """
-        # this method is used to add prefix paths in conditional trees of frequentPatternTree
+    def addPrefixPath(self, prefix, mapSupportBeta, min_sup):
+        q = 0
         pathCount = prefix[0].counter
         current = self.root
         prefix.reverse()
         for i in range(0, len(prefix) - 1):
             pathItem = prefix[i]
-            if __mapSupportBeta.get(pathItem.itemId) >= minSup:
+            # pathCount=mapSupportBeta.get(pathItem.itemId)
+            if mapSupportBeta.get(pathItem.itemId) >= min_sup:
                 child = current.getChild(pathItem.itemId)
-                if not child:
+                if child is None:
                     newNode = _Node()
-                    newNode.itemId = pathItem.itemId
+                    q += 1
+                    newNode.itemid = pathItem.itemId
+                    if newNode.expSup == 0:
+                        newNode.expSup = pathItem.expSup
+                    newNode.probability = pathItem.probability
                     newNode.parent = current
                     newNode.counter = pathCount
                     current.child.append(newNode)
                     current = newNode
-                    self.fixNodeLinks(pathItem.itemId, newNode)
+                    self.fixNodeLinks(pathItem.itemid, newNode)
                 else:
-                    child.counter += pathCount
-                    current = child
+                    if child.probability == prefix[i].probability:
+                        child.counter += pathCount
+                        child.expSup = child.expSup * pathItem.expSup
+                        current = child
+                    else:
+                        newNode = _Node()
+                        q += 1
+                        newNode.itemId = pathItem.itemId
+                        newNode.probability = pathItem.probability
+                        if newNode.expSup == 0:
+                            newNode.expSup = pathItem.expSup
+                        newNode.parent = current
+                        newNode.counter = pathCount
+                        current.child.append(newNode)
+                        current = newNode
+                        self.fixNodeLinks(pathItem.itemid, newNode)
+        return q
 
 
-class RSFPGrowth(_ab._frequentPatterns):
+class UFGrowth(_ab._frequentPatterns):
     """
     Description:
     -------------
-
-        Algorithm to find all items with relative support from given dataset
-
+        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
+        using PUF-Tree.
     Reference:
     -----------
-        'Towards Efficient Discovery of Frequent Patterns with Relative Support' R. Uday Kiran and
-               Masaru Kitsuregawa, http://comad.in/comad2012/pdf/kiran.pdf
-
+        Carson Kai-Sang Leung, Syed Khairuzzaman Tanbeer, "PUF-Tree: A Compact Tree Structure for Frequent Pattern Mining of Uncertain Data",
+        Pacific-Asia Conference on Knowledge Discovery and Data Mining(PAKDD 2013), https://link.springer.com/chapter/10.1007/978-3-642-37453-1_2
     Attributes:
-    -------------
+    -----------
         iFile : file
-            Name of the Input file to mine complete set of frequent patterns
+            Name of the Input file or path of the input file
         oFile : file
-            Name of the output file to store complete set of frequent patterns
+            Name of the output file or path of the output file
+        minSup: float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
-        minSup : float
-            The user given minSup
-        minRS : float
-            The user given minRS
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            it represents the total no of transactions
+            To represent the total no of transaction
         tree : class
-            it represents the Tree class
+            To represents the Tree class
         itemSetCount : int
-            it represents the total no of patterns
+            To represents the total no of patterns
         finalPatterns : dict
-            it represents to store the patterns
-        itemSetBuffer : list
-            it represents the store the items in mining
-        maxPatternLength : int
-           it represents the constraint for pattern length
-
+            To store the complete patterns
     Methods:
     --------
         startMine()
             Mining process will start from here
-        getFrequentPatterns()
+        getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
-        getmemoryUSS()
+        getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        check(line)
-            To check the delimiter used in the user input file
         creatingItemSets(fileName)
-            Scans the dataset or dataframes and stores in list format
+            Scans the dataset and stores in a list format
         frequentOneItem()
-            Extracts the one-frequent patterns from transactions
-        saveAllCombination(tempBuffer,s,position,prefix,prefixLength)
-            Forms all the combinations between prefix and tempBuffer lists with support(s)
-        saveItemSet(pattern,support)
-            Stores all the frequent patterns with their respective support
-        frequentPatternGrowthGenerate(frequentPatternTree,prefix,port)
-            Mining the frequent patterns by forming conditional frequentPatternTrees to particular prefix item.
-            __mapSupport represents the 1-length items with their respective support
-
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>>  python3 RSFPGrowth.py <inputFile> <outputFile> <minSup> <__minRatio>
+                      >>>  python3 PUFGrowth.py <inputFile> <outputFile> <minSup>
             Example:
-                      >>>  python3 RSFPGrowth.py sampleDB.txt patterns.txt 0.23 0.2
-
-            .. note:: maxPer and minPS will be considered in percentage of database transactions
+                      >>>  python3 PUFGrowth.py sampleTDB.txt patterns.txt 3
 
+            .. note:: minSup  will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.frequentPatternUsingOtherMeasures import RSFPGrowth as alg
+            from PAMI.uncertainFrequentPattern.basic import UFGrowth as alg
 
-            obj = alg.RSFPGrowth(iFile, minSup, __minRatio)
+            obj = alg.UFGrowth(iFile, minSup)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -350,360 +356,316 @@
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
-             The complete program was written by   Sai Chitra.B   under the supervision of Professor Rage Uday Kiran.
-
-        """
+             The complete program was written by P.Likhitha under the supervision of Professor Rage Uday Kiran.
 
-    __startTime = float()
-    __endTime = float()
+    """
+    _startTime = float()
+    _endTime = float()
     _minSup = str()
-    _minRS = float()
-    __finalPatterns = {}
+    _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    __memoryUSS = float()
-    __memoryRSS = float()
-    __Database = []
-    __mapSupport = {}
-    __lno = 0
-    __tree = _Tree()
-    __itemSetBuffer = None
-    __fpNodeTempBuffer = []
-    __itemSetCount = 0
-    __maxPatternLength = 1000
-
-    def __init__(self, iFile, __minSup, __minRS, sep='\t'):
-        super().__init__(iFile, __minSup, __minRS, sep)
-        self.__finalPatterns = {}
-
-    def __creatingItemSets(self):
-        """
-            Storing the complete transactions of the __Database/input file in a __Database variable
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _rank = {}
+    _mapSupport = {}
+    _lno = 0
+    _tree = _Tree()
+    _itemsetBuffer = None
+    _fpNodeTempBuffer = []
+    _maxPatternLength = 1000
+    _itemsetCount = 0
+    _frequentitems = {}
+    _fpnode = 0
+    _conditionalnodes = 0
 
+    def __init__(self, iFile, minSup, sep='\t'):
+        super().__init__(iFile, minSup, sep)
 
-            """
-        self.__Database = []
+    def _creatingItemSets(self):
+        """
+            Scans the uncertain transactional dataset
+        """
+        self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self.__Database = self._iFile['Transactions'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self.__Database.append(temp)
+                    tr = []
+                    for i in temp:
+                        i1 = i.index('(')
+                        i2 = i.index(')')
+                        item = i[0:i1]
+                        probability = float(i[i1 + 1:i2])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self.__Database.append(temp)
+                            tr = []
+                            for i in temp:
+                                i1 = i.index('(')
+                                i2 = i.index(')')
+                                item = i[0:i1]
+                                probability = float(i[i1 + 1:i2])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-
-    def __frequentOneItem(self):
-        """Generating One frequent items sets
 
+    def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
+                :param self.Database : it represents the one self.Database in database
+                :type self.Database : list
         """
-        self.__mapSupport = {}
-        for i in self.__Database:
+
+        mapSupport = {}
+        for i in self._Database:
             for j in i:
-                if j not in self.__mapSupport:
-                    self.__mapSupport[j] = 1
+                if j.item not in mapSupport:
+                    mapSupport[j.item] = j.probability
                 else:
-                    self.__mapSupport[j] += 1
-
-    def __saveItemSet(self, prefix, prefixLength, support, ratio):
-        """To save the frequent patterns mined form frequentPatternTree
-
-        :param prefix: the frequent pattern
-        :type prefix: list
-        :param prefixLength: the length of a frequent pattern
-        :type prefixLength: int
-        :param support: the support of a pattern
-        :type support:  int
-        """
-
-        sample = []
-        for i in range(prefixLength):
-            sample.append(prefix[i])
-        self.__itemSetCount += 1
-        self.__finalPatterns[tuple(sample)] = str(support) + " : " + str(ratio)
-
-    def __saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
-        """Generating all the combinations for items in single branch in frequentPatternTree
-
-        :param tempBuffer: items in a list
-        :type tempBuffer: list
-        :param s: support at leaf node of a branch
-        :param position: the length of a tempBuffer
-        :type position: int
-        :param prefix: it represents the list of leaf node
-        :type prefix: list
-        :param prefixLength: the length of prefix
-        :type prefixLength: int
+                    mapSupport[j.item] += j.probability
+        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
+        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
+        return mapSupport, plist
 
-        """
-        max1 = 1 << position
-        for i in range(1, max1):
-            newPrefixLength = prefixLength
-            for j in range(position):
-                isSet = i & (1 << j)
-                if isSet > 0:
-                    prefix.insert(newPrefixLength, tempBuffer[j].itemId)
-                    newPrefixLength += 1
-            ratio = s / self.__mapSupport[self.__getMinItem(prefix, newPrefixLength)]
-            if ratio >= self._minRS:
-                self.__saveItemSet(prefix, newPrefixLength, s, ratio)
-
-    def __frequentPatternGrowthGenerate(self, frequentPatternTree, prefix, prefixLength, __mapSupport, minConf):
-        """Mining the fp tree
-
-        :param frequentPatternTree: it represents the frequentPatternTree
-        :type frequentPatternTree: class Tree
-        :param prefix: it represents a empty list and store the patterns that are mined
-        :type prefix: list
-        :param param prefixLength: the length of prefix
-        :type prefixLength: int
-        :param __mapSupport : it represents the support of item
-        :type __mapSupport : dictionary
-        """
+    def _ufgrowth(self, tree, prefix, prefixLength, prefixSupport, mapSupport):
+        if prefixLength == self._maxPatternLength:
+            return
         singlePath = True
         position = 0
         s = 0
-        if len(frequentPatternTree.root.child) > 1:
+        if len(tree.root.child) > 1:
             singlePath = False
         else:
-            currentNode = frequentPatternTree.root.child[0]
+            currentNode = tree.root.child[0]
             while True:
                 if len(currentNode.child) > 1:
                     singlePath = False
                     break
-                self.__fpNodeTempBuffer.insert(position, currentNode)
+                self._fpNodeTempBuffer.insert(position, currentNode)
                 s = currentNode.counter
                 position += 1
                 if len(currentNode.child) == 0:
                     break
                 currentNode = currentNode.child[0]
         if singlePath is True:
-            self.__saveAllCombinations(self.__fpNodeTempBuffer, s, position, prefix, prefixLength)
+            self._saveAllcombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
         else:
-            for i in reversed(frequentPatternTree.headerList):
+            for i in reversed(tree.headerList):
                 item = i
-                support = __mapSupport[i]
-                CminSup = max(self._minSup, support * self._minRS)
-                betaSupport = support
+                betaSupport = mapSupport[item]
                 prefix.insert(prefixLength, item)
-                max1 = self.__getMinItem(prefix, prefixLength)
-                if self.__mapSupport[max1] > self.__mapSupport[item]:
-                    max1 = item
-                ratio = support / self.__mapSupport[max1]
-                if ratio >= self._minRS:
-                    self.__saveItemSet(prefix, prefixLength + 1, betaSupport, ratio)
-                if prefixLength + 1 < self.__maxPatternLength:
+                # print prefix,betaSupport
+                self._saveItemset(prefix, prefixLength + 1, betaSupport)
+                if prefixLength + 1 < self._maxPatternLength:
                     prefixPaths = []
-                    path = frequentPatternTree.mapItemNodes.get(item)
-                    __mapSupportBeta = {}
+                    path = tree.mapItemNodes.get(item)
+                    mapSupportBeta = {}
                     while path is not None:
-                        if path.parent.itemId != -1:
-                            prefixPath = [path]
+                        if path.parent.itemid != -1:
+                            prefixPath = []
+                            prefixPath.append(path)
                             pathCount = path.counter
                             parent1 = path.parent
-                            if __mapSupport.get(parent1.itemId) >= CminSup:
-                                while parent1.itemId != -1:
-                                    mins = CminSup
-                                    if __mapSupport.get(parent1.itemId) >= mins:
-                                        prefixPath.append(parent1)
-                                        if __mapSupportBeta.get(parent1.itemId) is None:
-                                            __mapSupportBeta[parent1.itemId] = pathCount
-                                        else:
-                                            __mapSupportBeta[parent1.itemId] = __mapSupportBeta[
-                                                                                   parent1.itemId] + pathCount
-                                        parent1 = parent1.parent
-                                    else:
-                                        break
-                                prefixPaths.append(prefixPath)
+                            while parent1.itemid != -1:
+                                prefixPath.append(parent1)
+                                s = (pathCount * path.expSup) * parent1.probability
+                                if mapSupportBeta.get(parent1.itemid) == None:
+                                    mapSupportBeta[parent1.itemid] = s
+                                else:
+                                    mapSupportBeta[parent1.itemid] = mapSupportBeta[parent1.itemid] + s
+                                parent1 = parent1.parent
+                            prefixPaths.append(prefixPath)
                         path = path.nodeLink
-                    __treeBeta = _Tree()
-                    for k in prefixPaths:
-                        __treeBeta.addPrefixPath(k, __mapSupportBeta, self._minSup)
-                    if len(__treeBeta.root.child) > 0:
-                        __treeBeta.createHeaderList(__mapSupportBeta, self._minSup)
-                        self.__frequentPatternGrowthGenerate(__treeBeta, prefix, prefixLength + 1, __mapSupportBeta,
-                                                           minConf)
-
-    def __convert(self, value):
-        """
-        to convert the type of user specified __minSup value
-        :param value: user specified __minSup value
-        :return: converted type
+                    treeBeta = _Tree()
+                    for i in prefixPaths:
+                        q = treeBeta.addPrefixPath(i, mapSupportBeta, self._minSup)
+                        self._conditionalnodes += q
+                    if len(treeBeta.root.child) > 0:
+                        treeBeta.createHeaderList(mapSupportBeta, self._minSup)
+                        # print(treeBeta.headerList)
+                        self._ufgrowth(treeBeta, prefix, prefixLength + 1, betaSupport, mapSupportBeta)
+
+    def _saveItemset(self, prefix, prefixLength, support):
+        l = []
+        for i in range(prefixLength):
+            l.append(prefix[i])
+        self._itemsetCount += 1
+        l.sort()
+        s = '\t'.join(l)
+        self._finalPatterns[s] = support
+
+    def _saveAllcombinations(self, TempBuffer, s, position, prefix, prefixLength):
+        # support=0
+        max1 = 1 << position
+        for i in range(1, max1):
+            newprefixLength = prefixLength
+            for j in range(position):
+                isset = i & (1 << j)
+                if isset > 0:
+                    prefix.insert(newprefixLength, TempBuffer[j].itemid)
+                    newprefixLength += 1
+                    support = TempBuffer[j].counter
+            self._saveItemset(prefix, newprefixLength, s)
+
+    def _convert(self, value):
+        """
+        To convert the type of user specified minSup value
+            :param value: user specified minSup value
+            :return: converted type minSup value
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = (len(self.__Database) * value)
+            value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
-                value = float(value)
-                value = (len(self.__Database) * value)
+                value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
     def startMine(self):
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
         """
-            main program to start the operation
-        """
-
-        self.__startTime = _ab._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
-        self.__creatingItemSets()
-        self._minSup = self.__convert(self._minSup)
-        self._minRS = float(self._minRS)
-        self.__frequentOneItem()
-        self.__finalPatterns = {}
-        self.__mapSupport = {k: v for k, v in self.__mapSupport.items() if v >= self._minSup}
-        __itemSetBuffer = [k for k, v in sorted(self.__mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        for i in self.__Database:
+        global minSup
+        self._startTime = _ab._time.time()
+        self._creatingItemSets()
+        self._minSup = self._convert(self._minSup)
+        minSup = self._minSup
+        self._finalPatterns = {}
+        _mapSupport, plist = self._frequentOneItem()
+        for i in self._Database:
             transaction = []
             for j in i:
-                if j in __itemSetBuffer:
+                if _mapSupport.get(j.item) >= self._minSup:
                     transaction.append(j)
-            transaction.sort(key=lambda val: self.__mapSupport[val], reverse=True)
-            self.__tree.addTransaction(transaction)
-        self.__tree.createHeaderList(self.__mapSupport, self._minSup)
-        if len(self.__tree.headerList) > 0:
-            self.__itemSetBuffer = []
-            self.__frequentPatternGrowthGenerate(self.__tree, self.__itemSetBuffer, 0, self.__mapSupport, self._minRS)
-        print("Relative support frequent patterns were generated successfully using RSFPGrowth algorithm")
-        self.__endTime = _ab._time.time()
+            transaction.sort(key=lambda val: _mapSupport[val.item], reverse=True)
+            o = self._tree.addTransaction(transaction)
+        self._tree.createHeaderList(_mapSupport, self._minSup)
+        if len(self._tree.headerList) > 0:
+            self._itemsetBuffer = []
+            # self.fpNodeTempBuffer=[]
+            self._ufgrowth(self._tree, self._itemsetBuffer, 0, self._lno, _mapSupport)
+        print("Frequent patterns were generated from uncertain databases successfully using UF algorithm")
+        self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self.__memoryRSS = float()
-        self.__memoryUSS = float()
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
+        self._memoryUSS = float()
+        self.memoryRSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self.memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryUSS
+        return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.__memoryRSS
-
-    def __getMinItem(self, prefix, prefixLength):
-        """
-            returns the minItem from prefix
-        """
-        minItem = prefix[0]
-        for i in range(prefixLength):
-            if self.__mapSupport[minItem] > self.__mapSupport[prefix[i]]:
-                minItem = prefix[i]
-        return minItem
+        return self.memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
-
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
-        return self.__endTime - self.__startTime
+        return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self.__finalPatterns.items():
-            pattern = str()
-            for i in a:
-                pattern = pattern + i + " "
-            data.append([pattern, b])
+        for a, b in self._finalPatterns.items():
+            data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
-
         :param outFile: name of the output file
         :type outFile: file
         """
-        self.__oFile = outFile
-        writer = open(self.__oFile, 'w+')
-        for x, y in self.__finalPatterns.items():
-            pattern = str()
-            for i in x:
-                pattern = pattern + i + "\t"
-            s1 = pattern.strip() + ": " + str(y)
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
         :rtype: dict
         """
-        res = dict()
-        for x, y in self.__finalPatterns.items():
-            pattern = str()
-            for i in x:
-                pattern = pattern + i + "\t"
-            s1 = str(y)
-            res[pattern] = s1
-        return res
+        return self._finalPatterns
 
     def printResults(self):
-        print("Total number of Relative Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
-        if len(_ab._sys.argv) == 6:
-            _ap = RSFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = RSFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = UFGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+        if len(_ab._sys.argv) == 4:
+            _ap = UFGrowth(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        print("Total number of Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Uncertain Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/relativeFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py` & `pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/RHUIM.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
+#     from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
 #
 #     obj = alg.RHUIM("input.txt", 35, 20)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
@@ -46,15 +46,15 @@
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
 
-from PAMI.relativeHighUtilityPatterns.basic import abstract as _ab
+from PAMI.relativeHighUtilityPattern.basic import abstract as _ab
 
 
 class _Transaction:
     """
         A class to store Transaction of a database
 
     Attributes:
@@ -379,15 +379,15 @@
                       >>>  python3 RHUIM.py sampleTDB.txt output.txt 35 20
 
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.relativeHighUtilityPatterns.basic import RHUIM as alg
+            from PAMI.relativeHighUtilityPattern.basic import RHUIM as alg
 
             obj=alg.RHUIM("input.txt", 35, 20)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
```

### Comparing `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/relativeHighUtilityPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.8.1/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.8.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
+import itertools as _itertools
 
 
-class _sequentialPatterns(_ABC):
-    """
-    This abstract base class defines the variables and methods that every frequent pattern mining algorithm in sequential databases must
+class _faultTolerantFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every fault-tolerant frequent pattern mining algorithm must
         employ in PAMI
 
-    Attributes:
-    ----------
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
         minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -62,39 +63,40 @@
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of frequent patterns
+            Name of the output file to store complete set of fault-tolerant frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-    Methods:
-    -------
+       Methods:
+       -------
         startMine()
             Calling this function will start the actual mining process
         getPatterns()
             This function will output all interesting patterns discovered by an algorithm
         save(oFile)
             This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
             The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
             This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
+
     """
 
-    def __init__(self, iFile, minSup, sep="\t"):
+    def __init__(self, iFile, minSup, itemSup, minLength, faultTolerance, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
@@ -102,45 +104,53 @@
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
+        self._itemSup = itemSup
+        self._minLength = minLength
+        self._faultTolerance = faultTolerance
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
+        """Variable to store USS memory consumed by the program"""
+
+
+
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of frequent patterns generated will be retrieved from this function"""
+        """Complete set of fault-tolerant frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of frequent patterns will be saved in to an output file from this function
+        """Complete set of fault-tolerant frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of fault-tolerant frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
@@ -153,13 +163,7 @@
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
-
-    @_abstractmethod
-    def printResults(self):
-        """ To print result of the execution"""
-
-        pass
```

### Comparing `pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.8.1/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.8.1/PAMI/uncertainFaultTolerantFrequentPattern/abstract.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,33 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
-from collections import defaultdict as _dd
+from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
-import resource as _resource
-import math as _math
 import sys as _sys
+import validators as _validators
+from urllib.request import urlopen as _urlopen
+import functools as _functools
+import itertools as _itertools
 
 
-class _frequentPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+class _faultTolerantFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every fault-tolerant frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
@@ -60,15 +63,15 @@
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of frequent patterns
+            Name of the output file to store complete set of fault-tolerant frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
        Methods:
        -------
@@ -85,62 +88,69 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, minSup, sep="\t"):
+    def __init__(self, iFile, minSup, itemSup, minLength, faultTolerance, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._sep = sep
         self._minSup = minSup
-        self._oFile = str()
+        self._itemSup = itemSup
+        self._minLength = minLength
+        self._faultTolerance = faultTolerance
         self._finalPatterns = {}
-        self._startTime = float()
-        self._endTime = float()
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
+        self._startTime = float()
+        self._endTime = float()
+
+        """Variable to store USS memory consumed by the program"""
+
+
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of frequent patterns generated will be retrieved from this function"""
+        """Complete set of fault-tolerant frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of frequent patterns will be saved in to an output file from this function
+        """Complete set of fault-tolerant frequent patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of fault-tolerant frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
```

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.stablePeriodicFrequentPattern.basic import SPPECLAT as alg
+#     from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
 #
 #     obj = alg.PFPECLAT("../basic/sampleTDB.txt", 5, 3, 3)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
@@ -137,26 +137,26 @@
             Used to implement prefix class equivalence method to generate the periodic patterns recursively
 
 
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>>   python3 SPPECLAT.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
+                      >>>   python3 basic.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
 
             Example:
-                      >>>    python3 SPPECLAT.py sampleDB.txt patterns.txt 10.0 4.0 2.0
+                      >>>    python3 basic.py sampleDB.txt patterns.txt 10.0 4.0 2.0
 
             .. note:: constraints will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-                    from PAMI.stablePeriodicFrequentPattern.basic import SPPECLAT as alg
+                    from PAMI.stablePeriodicFrequentPattern.basic import basic as alg
 
                     obj = alg.PFPECLAT("../basic/sampleTDB.txt", 5, 3, 3)
 
                     obj.startMine()
 
                     Patterns = obj.getPatterns()
 
@@ -330,15 +330,15 @@
         self._createSPPList()
         self._endTime = _ab._time.time()
         self._memoryUSS = float()
         self._memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Stable Periodic Frequent patterns were generated successfully using SPPECLAT algorithm ")
+        print("Stable Periodic Frequent patterns were generated successfully using basic algorithm ")
 
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
 
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
```

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.stablePeriodicFrequentPattern.basic import SPPGrowth as alg
+#     from PAMI.stablePeriodicFrequentPattern.basic import topk as alg
 #
-#     obj = alg.SPPGrowth(iFile, minSup, maxPer, maxLa)
+#     obj = alg.topk(iFile, minSup, maxPer, maxLa)
 #
 #     obj.startMine()
 #
 #     Patterns = obj.getPatterns()
 #
 #     print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
 #
@@ -334,27 +334,27 @@
         convert()
             to convert the user specified value
 
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>>   python3 SPPGrowth.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
+                      >>>   python3 topk.py <inputFile> <outputFile> <minSup> <maxPer> <maxLa>
             Example:
-                      >>>  python3 SPPGrowth.py sampleTDB.txt patterns.txt 0.3 0.4 0.3
+                      >>>  python3 topk.py sampleTDB.txt patterns.txt 0.3 0.4 0.3
 
             .. note:: constraints will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.stablePeriodicFrequentPattern.basic import SPPGrowth as alg
+            from PAMI.stablePeriodicFrequentPattern.basic import topk as alg
 
-            obj = alg.SPPGrowth(iFile, minSup, maxPer, maxLa)
+            obj = alg.topk(iFile, minSup, maxPer, maxLa)
 
             obj.startMine()
 
             Patterns = obj.getPatterns()
 
             print("Total number of Stable Periodic Frequent Patterns:", len(Patterns))
 
@@ -577,15 +577,15 @@
             self._finalPatterns[sample] = i[1]
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Stable Periodic Frequent patterns were generated successfully using SPPGrowth algorithm ")
+        print("Stable Periodic Frequent patterns were generated successfully using topk algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
```

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,15 +395,15 @@
             self._finalPatterns[sample] = i[1]
         self._endTime = time.time()
         process = psutil.Process(os.getpid())
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
-        print("Stable Periodic Frequent patterns were generated successfully using SPPGrowth algorithm ")
+        print("Stable Periodic Frequent patterns were generated successfully using topk algorithm ")
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
 
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
@@ -478,16 +478,16 @@
         _memUSS = _ap.getMemoryUSS()
         print("Total Memory in USS:", _memUSS)
         _memRSS = _ap.getMemoryRSS()
         print("Total Memory in RSS", _memRSS)
         _run = _ap.getRuntime()
         print("Total ExecutionTime in ms:", _run)
     else:
-        '''ap = SPPGrowth('https://www.u-aizu.ac.jp/~udayrage/datasets/temporalDatabases/temporal_retail.csv', 0.001, 0.005, 0.004)
-        #ap = SPPGrowth('/Users/likhitha/Downloads/contextPrefixSpan.txt', 3, 6, 2, ' ')
+        '''ap = topk('https://www.u-aizu.ac.jp/~udayrage/datasets/temporalDatabases/temporal_retail.csv', 0.001, 0.005, 0.004)
+        #ap = topk('/Users/likhitha/Downloads/contextPrefixSpan.txt', 3, 6, 2, ' ')
         ap.startMine()
         Patterns = ap.getPatterns()
         print("Total number of Frequent Patterns:", len(Patterns))
         ap.save('/Users/Likhitha/Downloads/output')
         memUSS = ap.getMemoryUSS()
         print("Total Memory in USS:", memUSS)
         memRSS = ap.getMemoryRSS()
```

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.8.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py` & `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/SHUGrowth.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,718 +1,923 @@
-__copyright__ = """
 #  Copyright (C)  2021 Rage Uday Kiran
 #
 #      This program is free software: you can redistribute it and/or modify
 #      it under the terms of the GNU General Public License as published by
 #      the Free Software Foundation, either version 3 of the License, or
 #      (at your option) any later version.
 #
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
 
+import abstract as _hus
+import pandas as pd
+from functools import reduce
+from operator import and_ 
 
-import abstract as _fp
+_minSup = str()
+_hus._sys.setrecursionlimit(20000)
 
-_fp._sys.setrecursionlimit(20000)
 
 class _Node:
     """
-    This class represents a node in the FP-tree
+        A class used to represent a node in the SHU tree
 
-    Attributes:
-    ----------
-        itemId : str
-            The item name of the node
+        Attributes
+        ----------
+            itemName : str
+                name of the item
 
-        counter : int
-            The support count of the item
+            utility : int
+                utility of the item
 
-        parent : Node
-            The parent node of the current node
+            children : dict
+                dictionary of children of the node
 
-        children : dict
-            The dictionary of children of the current node
+            next : _Node
+                pointer to the next node with same item in the tree
 
-        tail : list
-            The tail of the current node denoting the support count in each batch
+            batchIndex : int
+                index of the batch with respect to window to which the node belongs
+            
+            utility : list
+                list of utilities of the node with respect to each batch in the window
 
-        next : Node
-            The next node of the current node
+            parent : _Node
+                pointer to the parent of the node
 
-        
-        Methods:
+        Methods
         -------
 
-        addChild(node) 
-            Adds a child node to the current node
+            addUtility(utility, batchIndex)
+                Adds utility to the node at specified batch index
 
-        shiftTail()
-            Shifts the tail of the current node during the removal of the batch
+            removeUtility(utility)
+                Removes utility from the node
 
-        addSupportCount(count)
-            Adds the support count to the current node
+            shiftUtility()
+                Shifts the utility values of the node to the left useful for removing the oldest batch information
 
+            shiftTail()
+                Shifts the tail values of the node to the left useful for removing the oldest batch information
     """
-    def __init__(self, item, supportCount):
-        self.itemId = item
-        self.counter = supportCount
+
+    def __init__(self, itemName, utility, batchSize, batchIndex):
+        self.itemName = itemName
+        self.utility = [0 for _ in range(batchSize)]
+        self.children = dict()
+        self.next = None
+        self.batchIndex = batchIndex
+        self.utility[batchIndex] = utility
         self.parent = None
-        self.children = {}
         self.tail = None
-        self.next = None
 
-    def addChild(self, node):
+    def addUtility(self, utility, batchIndex):
         """
-            Adds a child node to the current node
+            Adds utility to the node
 
-            :param node: The child node to be added
-            :type node: Node
+            Parameters
+            ----------
+                utility : int
+                    Net utility value to be added
+
+                batchIndex : int
+                    index of the batch with respect to window to which the node belongs
         """
-        self.children[node.itemId] = node
-        node.parent = self
 
-    def shiftTail(self):
+        self.utility[batchIndex] += utility
+
+    def removeUtility(self, utility):
         """
-            Shifts the tail of the current node during the removal of the batch
+            Removes utility from the node
+
+            Parameters
+            ----------
+                utility : int
+                    Net utility value to be removed
         """
-        self.tail.pop(0)
-        self.tail.append(0)
 
-    def addSupportCount(self, count):
+        self.utility -= utility
+
+    def shiftUtility(self):
+        """
+            Shifts the utility values of the node to the left
         """
-            Adds the support count to the current node
+        self.utility.pop(0)
+        self.utility.append(0)
 
-            :param count: The support count to be added
-            :type count: int
+    def shiftTail(self):
+        """
+            Shifts the tail pointer of the node to the left
         """
-        self.counter += count
 
-class _HeaderTable:
+        if(self.tail is not None):
+            self.tail.pop(0)
+            self.tail.append(False)
+
 
+class _HeaderTable:
     """
-        This class represents the header table of the FP-tree
+        A class used to represent the header table of the SHU tree
 
-        Attributes:
+        Attributes
         ----------
             table : dict
-                The dictionary of items and their support count with node pointer
+                dictionary of items as keys and list of utility and pointer to the node in the tree as values
+                representing the header table
 
             orderedItems : list
-                The list of items in the header table in the order of their support count
+                list of items in the header table in lexicographical order
 
-        Methods:
+        Methods
         -------
-            updateSupportCount(item, count, node)
-                Updates the support count with the node pointer of the item in the header table
+            updateUtility(item, utility, node)
+                Updates the utility of the item with node pointer in the header table
 
-            addSupportCount(item, count)
-                Adds the support count of the item in the header table
+            addUtility(item, utility)
+                Adds utility to the item in the header table
 
-            removeSupportCount(item, count)
-                Removes the support count of the item in the header table
+            removeUtility(item, utility)
+                Removes utility from the item in the header table
 
             itemOrdering()
-                Orders the items in the header table in the order of their support count
-
-            orderTransaction(transaction)
-                Orders the items in the transaction in the order of their support count
-
+                Orders the items in the header table in lexicographical order
     """
 
     def __init__(self):
-        self.table = {}
-        self.orderedItems = []
+        self.table = dict()
+        self.orderedItems = list()
 
-    def updateSupportCount(self, item, count, node):
+    def updateUtility(self, item, utility, node):
         """
-            Updates the support count with the node pointer of the item in the header table
+            Updates the utility of the item in the header table
 
-            :param item: The item whose support count is to be updated
-            :type item: str
-            :param count: The support count to be added
-            :type count: int
-            :param node: The node pointer to be added
-            :type node: Node
+            Parameters
+            ----------
+                item : str
+                    name of the item to which utility needs to be updated
+
+                utility : int
+                    Net utility of the item to be updated
+
+                node : _Node
+                    pointer to the node in the tree to which the item belongs
         """
+
         if item in self.table:
-            self.table[item][0] += count
+            self.table[item][0] += utility
             tempNode = self.table[item][1]
-            while tempNode.next != None:
+
+            while tempNode.next is not None:
                 tempNode = tempNode.next
+            
             tempNode.next = node
-        else:
-            self.table[item] = [count, node]
 
+        else:
+            self.table[item] = [utility, node]
+    
         self.itemOrdering()
 
-    def addSupportCount(self, item, count):
+    def addUtility(self, item, utility):
         """
-            Adds the support count of the item in the header table
+            Adds utility to the item in the header table
 
-            :param item: The item whose support count is to be added
-            :type item: str
-            :param count: The support count to be added
-            :type count: int
-        """
-        if item in self.table:
-            self.table[item][0] += count
-    
-    def removeSupportCount(self, item, count):
-        """
-            Removes the support count of the item in the header table
+            Parameters
+            ----------
+                item : str
+                    name of the item to which utility needs to be added
 
-            :param item: The item whose support count is to be removed
-            :type item: str
-            :param count: The support count to be removed
-            :type count: int
+                utility : int
+                    Net utility of the item to be added
         """
-        if item in self.table:
-            self.table[item][0] -= count
-            if(self.table[item][0] == 0):
-                del self.table[item]
+        self.table[item][0] += utility
     
-    def itemOrdering(self):
-        """
-            Orders the items in the header table in the order of their support count
+
+    def removeUtility(self, item, utility):
         """
-        self.orderedItems = list(sorted(self.table.keys(), key=lambda x: self.table[x][0]))
+            Removes utility from the item in the header table
+
+            Parameters
+            ----------
+                item : str
+                    name of the item to which utility needs to be removed
 
-    def orderTransaction(self, transaction):
+                utility : int
+                    Net utility of the item to be removed
         """
-            Orders the items in the transaction in the order of their support count
+        self.table[item][0] -= utility
 
-            :param transaction: The transaction to be ordered
-            :type transaction: list
+        if self.table[item][0] == 0:
+            del self.table[item]
 
-            :return: The ordered transaction
-            :rtype: list
+        self.itemOrdering()
+
+    def itemOrdering(self):
         """
-        return sorted(transaction, key=lambda x: self.table[x][0] if x in self.table else 1, reverse=True)
+            Orders the items in the header table in lexicographical order
+        """        
+        self.orderedItems = list(sorted(self.table.keys()))
+
+class _SHUTree:
 
-class _CPSTree:
     """
-        Class representing the CPSTree
+        A class used to represent the SHU tree
 
-        Attributes:
+        Attributes
         ----------
-            root : Node
-                The root node of the CPSTree
+            root : _Node
+                root node of the tree
+
+            headerTable : _HeaderTable
+                header table of the tree
 
-            headerTable : HeaderTable
-                The header table of the CPSTree
+            batchSize : int
+                size of the batch
 
             windowSize : int
-                The window size used for analyzing the data stream
+                size of the window
 
-            paneSize : int
-                The pane size used in each window for analyzing the data stream
+            batchIndex : int
+                index of the current batch with respect to window
 
-            curBatchIndex : int
-                The current batch index of the data stream
+            windowUtility : int
+                utility of the current window
 
-        Methods:
-        -------
+            localTree : bool
+                flag to indicate whether the tree is local useful for prefix/conditional tree generation
 
-            addTransaction(transaction, restructuring = False, supportValue = None, tailNode = None)
-                Adds the transaction to the CPSTree
+        Methods
+        -------
+            addTransaction(transaction, utility)
+                Adds transaction to the tree
 
-            updateBranch(node, count)
-                Updates the branch of the node with the support count useful while removing the oldest batch
+            tailUtilities(root)
+                Returns the tail utilities of the tree
 
             removeBatch()
-                Removes the oldest batch from the CPSTree
+                Removes the oldest batch from the tree
+
+            removeBatchUtility()
+                Removes the utility of the oldest batch from each subtree
 
     """
 
-    def __init__(self, windowSize, paneSize):
-        self.root = _Node(None, 0)
+    def __init__(self, batchSize, windowSize, localTree = False):
+        self.root = _Node(None, 0, batchSize, 0)
         self.headerTable = _HeaderTable()
+        self.batchSize = batchSize
         self.windowSize = windowSize
-        self.paneSize = paneSize
-        self.curBatchIndex = 0
+        self.batchIndex = 0
+        self.windowUtility = 0
+        self.localTree = localTree
 
-    def addTransaction(self, transaction, restructuring = False, supportValue = None, tailNode = None):
+    def addTransaction(self, transaction, utility, itemUtility = None):
         """
-            Adds the transaction to the CPSTree
+            Adds transaction to the tree
 
-            :param transaction: The transaction to be added
-            :type transaction: list
-            :param restructuring: Flag to indicate whether the transaction is added during restructuring
-            :type restructuring: bool
-            :param supportValue: The support count of the items in the transaction useful during restructuring
-            :type supportValue: dict
-            :param tailNode: The tail node of the transaction useful during restructuring
-            :type tailNode: Node
-        """
-        curNode = self.root
+            Parameters
+            ----------
+                transaction : list
+                    list of items in the transaction
 
-        if restructuring is False:
-            transaction = self.headerTable.orderTransaction(transaction)
+                utility : int
+                    Net utility of the transaction
 
-        for item in transaction:
-            if item in curNode.children:
+        """
+        # print("Transaction", transaction, itemUtility, self.localTree)
+        transaction.sort(key = lambda x: x[0])
+        currentNode = self.root
+        self.windowUtility += utility
 
-                if supportValue is None:
-                    curNode.children[item].addSupportCount(1)
-                    self.headerTable.addSupportCount(item, 1)
-                else:
-                    curNode.children[item].addSupportCount(supportValue[item])
-                    self.headerTable.addSupportCount(item, supportValue[item])
-                
-                curNode = curNode.children[item]
+        curUtility = 0
+        for iter in range(len(transaction)):
+            
+            item = transaction[iter]
+
+            if(self.localTree is False):
+                curUtility += itemUtility[iter]
             else:
+                curUtility = itemUtility[iter]
 
-                if supportValue is None:
-                    newNode = _Node(item, 1)
-                    self.headerTable.updateSupportCount(item, 1, newNode)
+            
+            if item in currentNode.children:
+                currentNode = currentNode.children[item]
+                currentNode.addUtility(curUtility, self.batchIndex)
+
+                if(self.localTree is False):
+                    self.headerTable.addUtility(item, curUtility)
 
                 else:
-                    newNode = _Node(item, supportValue[item])
-                    self.headerTable.updateSupportCount(item, supportValue[item], newNode)
+                    self.headerTable.addUtility(item, utility)
 
-                curNode.addChild(newNode)
-                newNode.parent = curNode
-                curNode = newNode
-
-        if curNode.tail is None:
-            curNode.tail = [0] * self.windowSize
-
-        if restructuring is False:
-            if supportValue is None:
-                curNode.tail[self.curBatchIndex] = 1
             else:
-                curNode.tail[self.curBatchIndex] = supportValue[item]
+                newNode = _Node(item, curUtility, self.batchSize, self.batchIndex)
+                currentNode.children[item] = newNode
+                newNode.parent = currentNode
 
+                if(self.localTree is False):
+                    self.headerTable.updateUtility(item, curUtility, newNode)
 
-        if tailNode is not None and curNode.tail is None:
-            curNode.tail = tailNode.copy()
+                else:
+                    self.headerTable.updateUtility(item, utility, newNode)
+                
+                currentNode = newNode
 
-        if tailNode is not None and curNode.tail is not None:
-            for i in range(len(tailNode)):
-                curNode.tail[i] += tailNode[i]
-            
+        currentNode.tail = [False for _ in range(self.batchSize)]
+        currentNode.tail[self.batchIndex] = True
 
-    def updateBranch(self, curNode, curSupport):
+    def tailUtilities(self, root):
         """
-            Updates the branch of the node with the support count useful while removing the oldest batch
-
-            :param curNode: The node whose branch is to be updated
-            :type curNode: Node
-            :param curSupport: The support count of the node to be updated
-            :type curSupport: int
+            Calculates the utility of the tail of the node
+            
+            Parameters
+            ----------
+                root : _Node
+                    pointer to the node in the tree
+
+            Returns
+            -------
+                netUtility : int
+                    utility of the tail of the node
         """
-        if(curNode.itemId is None):
-            return
 
-        curNode.addSupportCount(-curSupport)
-        parentNode = curNode.parent
+        if(root is None):
+            return 0
 
-        if(curNode.counter == 0):
-            if(self.headerTable.table[curNode.itemId][1] == curNode):
-                self.headerTable.table[curNode.itemId][1] = curNode.next
+        if(root.tail is not None):
+            return root.utility[0]
 
-            else:
-                prev = self.headerTable.table[curNode.itemId][1]
-                while(prev is not None and prev.next != curNode):
-                    prev = prev.next
+        netUtility = 0
+        for item in root.children:
+            netUtility += self.tailUtilities(root.children[item])
 
-                prev.next = curNode.next
+        return netUtility
 
-            del curNode.parent.children[curNode.itemId]
+    def removeBatch(self):
 
-        self.headerTable.removeSupportCount(curNode.itemId, curSupport)
-        self.updateBranch(parentNode, curSupport)
+        """
+            Removes the oldest batch from the tree
+        """
 
+        currentNode = self.root
 
-    def removeBatch(self):
+        curChilds = list(currentNode.children.keys())
+
+        for child in curChilds:
+            self.windowUtility -= self.tailUtilities(currentNode.children[child])
+            self.removeBatchUtility(currentNode.children[child])
+
+            if(sum(currentNode.children[child].utility) == 0):
+                del currentNode.children[child]
+
+
+    def removeBatchUtility(self, tempNode = None):
+        
         """
-            Removes the oldest batch from the CPSTree by recursively iterating over the tree
+            Removes the utility of the oldest batch from each subtree
+
+            Parameters
+            ----------
+                tempNode : _Node
+                    pointer to the node in the tree
+
         """
-        root = self.root
-        curItems = list(self.headerTable.table.keys())
-        for item in curItems:
-            curNode = self.headerTable.table[item][1]
-            while curNode is not None:
-                if curNode.tail is not None:
-                    curSupport = curNode.tail[0]
+        if tempNode is None:
+            return
+
+        for item in tempNode.children:
+            self.removeBatchUtility(tempNode.children[item])
+
+        curBatchUtility = tempNode.utility[0]
+        tempNode.shiftUtility()
+        tempNode.shiftTail()
+
+        if(sum(tempNode.utility) == 0):
+            if(tempNode.itemName in self.headerTable.table):
+                curNode = self.headerTable.table[tempNode.itemName][1]
+
+                if(curNode == tempNode):
+                    self.headerTable.table[tempNode.itemName][1] = tempNode.next
 
-                    if(curSupport != 0):
-                        self.updateBranch(curNode, curSupport)
-                    curNode.shiftTail()
+                else:
+                    while(curNode != None and curNode.next != tempNode):
+                        curNode = curNode.next
+
+                    if(curNode != None):
+                        curNode.next = tempNode.next
 
-                curNode = curNode.next
+                del tempNode.tail
+        
+        self.headerTable.removeUtility(tempNode.itemName, curBatchUtility)
 
+        curChilds = list(tempNode.children.keys())
+        for child in curChilds:
+            if(sum(tempNode.children[child].utility) == 0):
+                del tempNode.children[child]
 
-class FrequentPatternStreamMining(_fp._frequentPatternsStream):
+    
+class SHUGrowth(_hus._highUtilityPatternStreamMining):
     """
-        Description:
-        -------------
+        High-utility pattern mining over data stream is one of the challenging problems in data stream mining.
+        SHUGrowth is an algorithm that discovers high-utility patterns from data streams without rebuilding the tree.
+        It stores the database of the current window in form of SHUTree and adjusts the tree based on upcoming
+        transactions removing the oldest batch. It is an optimized varaint of HUPMS algorithm.
 
-            Sliding window-based frequent pattern mining over data streams is one of basic data stream mining tasks.
-            The goal is to find all frequent patterns in a sliding window over a data stream. It stores the complete
-            database in form of FP-Tree but adjusts the tree structure based on the upcoming transactions and removes
-            the oldest batch from the tree. This creates a sliding window over the data stream. The adjusting FP-tree
-            structure is called CPSTree. It is a modified version of the existing FP-Tree structure.
-
-        Reference : 
-        ------------
-            Syed Khairuzzaman Tanbeer and Chowdhury Farhan Ahmed and Byeong-Soo Jeong and Young-Koo Lee : Sliding 
-            window-based frequent pattern mining over data streams. Information Sciences Vol 179, 3843 - 3865, 2009.
-            https://doi.org/10.1016/j.ins.2009.07.012
-
-        Attributes : 
-        ------------
-            iFile : str
-                The input file name or path
-
-            minSup : float or int or str
-                The user can specify minSup either in count or proportion of database size.
-                If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-                Otherwise, it will be treated as float.
-                Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-
-            sep : str
-                This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
-                However, the users can override their default separator.
+        References
+        ----------
+            Chowdhury Farhan Ahmed and Syed Khairuzzaman Tanbeer and Byeong-Soo Jeong and Ho-Jin Choi : High utility 
+            pattern mining over data streams with sliding window technique. Expert Systems with Applications Vol 57, 
+            214 - 231, 2016. https://doi.org/10.1016/j.eswa.2016.03.001
 
-            windowSize : int
-                The size of the sliding window. It specifies the number of panes to be considered for mining frequent patterns.
 
-            paneSize : int
-                The size of the pane. It specifies the number of transactions to be considered for mining frequent patterns in each pane.
+        Attributes:
+        ----------
 
-            oFile : str
-                The output file name or path
+            __startTime : float
+                start time of the mining process
 
-            startTime : float
-                The start time of the mining process
+            __endTime : float
+                end time of the mining process
 
-            endTime : float
-                The end time of the mining process
+            _minUtil : str
+                minimum utility threshold
 
-            finalPatterns : dict
-                The dictionary containing the mined frequent patterns from each window.
+            __finalPatterns : dict
+                dictionary of the final patterns generated in each window
 
-            memoryUSS : float
-                The memory usage of the program in User Space
+            _iFile : str
+                input file name
 
-            memoryRSS : float
-                The memory usage of the program in Resident Set Size
+            _oFile : str
+                output file name
 
-            Database : list
-                The list containing the complete transactions of the database/input file
+            _sep : str
+                seperator of the input file
 
-            tree : CPSTree
-                The CPSTree structure used to mine frequent patterns from the data stream
+            __memoryUSS : float
+                memory usage of the algorithm in user space
 
+            __memoryRSS : float
+                memory usage of the algorithm in resident set size
 
-        Methods :
-        ---------
-            creatingItemSets()
-                Loads the complete transactions of the database/input file in a database variable.
+            __transactions : list
+                list of transactions in the database
 
-            convert(value):
-                Converts the minSup from different formats in absolute count.
+            __utilities : list
+                list of utilities of each item of a transaction in the database
 
-            getRestructuredTree(tree):
-                Restructures the tree by removing the oldest batch from the tree and updating the new batch in the tree.
+            __utilitySum : list
+                list of utility sum of each transaction in the database
 
-            getBranches(root, restructuredTree, originalTree, curBranch):
-                Gets the branches of the tree and updates it to the restructured tree.
+            __tree : _SHUTree
+                SHU tree of the current window
 
-            printTree():
-                Prints the CPSTree structure.
+            __windowSize : int
+                The size of the sliding window. It specifies the number of panes to be considered for mining patterns.
 
-            createPrefixBranch(root):
-                Creates the branches of the prefix tree.
+            __paneSize : int
+                The size of the pane. It specifies the number of transactions to be considered for mining in each pane.
 
-            createConditionalTree(root, transactions, minSup):
-                Creates the conditional tree from the prefix tree by removing items with support less than minSup.
+            
 
-            itemSetGeneration(root, minSup, candidatePattern, curItemset):
-                Generates the frequent itemsets by creating a conditional tree and mining patterns from it.
+        Methods:
+        -------
+            _createItemsets()
+                Storing the complete transactions of the database/input file in a transaction variable with their utilities.
 
+            minPathUtil(nodeIndex, stack)
+                Calculates the minimum utility of the path from the root to the ends of the tree
             
-            getMemoryRSS():
-                Gets the memory usage of the program in Resident Set Size.
+            createPrefixBranch(root)
+                Creates the prefix branch of the current SHU-Tree for construction of prefix tree
 
-            getMemoryUSS():
-                Gets the memory usage of the program in User Space.
+            fixUtility(root)
+                Fixes the utility of the nodes in the tree by merging the utility values
 
-            getPatterns():
-                Gets the mined frequent patterns from each window.
+            createConditionalTree(root, transactions, minUtil)
+                Creates the conditional tree for the given prefix tree
 
-            getPatternsAsDataFrame():
-                Gets the mined frequent patterns from each window as a pandas dataframe.
+            contains(superset, subset)
+                Checks if the superset contains the subset
 
-            getRuntime():
-                Gets the runtime of the program.
+            treeGenerations(root, netUtil, candidatePattern, curItem)
+                Generates the tree of the high utility patterns
 
-            printResults():
-                Prints the overall stasticts of the mining process.
+            startMine()
+                Starts the mining process
 
-            save():
-                Saves the mined frequent patterns in a file.
+            printTree(root, level)
+                Prints the SHU-tree in a readable format
 
-            startMine():
-                Starts the mining process by loading the input database and creating CPS Tree over each window.
+            getMemoryRSS()
+                Returns the memory usage of the algorithm in resident set size
+
+            getMemoryUSS()
+                Returns the memory usage of the algorithm in user space
+
+            getPatterns()
+                Returns the final patterns generated in each window
+
+            getPatternsAsDataFrame()
+                Returns the final patterns generated in each window as a pandas dataframe
+
+            getRuntime()
+                Returns the runtime of the algorithm
+
+            printResults()
+                Prints the statistics of the mining process
+
+            save()
+                Saves the patterns generated from each window in a file
+            
 
-        
         Executing the code on terminal:
         -------------------------------
 
             Format:
-            --------
-                python3 CPSTree.py <inputFile> <outputFile> <minSup> <windowSize> <paneSize> <separator>
+            -------
+                python3 SHUGrowth.py <inputFile> <outputFile> <minUtil> <windowSize> <paneSize> <separator>
 
             Example:
-            ---------
+            --------
 
-                python3 CPSTree.py retail.txt output.txt 0.5 100 1000 ',' (Here minimum support is 50% of the database size
+                python3 SHUGrowth.py retail.txt output.txt 107 100 1000 ',' (Here minimum utility is 107,
+                                                                            Window size is 100 and pane size is 1000
+                                                                            The separator is comma for the input file)
 
         Credits:
         --------
 
             The code is written by Vipul Chhabra under the supervision of Prof. Rage Uday Kiran.
-
+    
     """
 
     __startTime = float()
     __endTime = float()
-    _minSup = str()
+    _minUtil = str()
     __finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     __memoryUSS = float()
     __memoryRSS = float()
-    __Database = []
+    __transactions = []
+    __utilities = []
+    __utilitySum = []
     __tree = None
     __windowSize = 0
     __paneSize = 0
 
-    def __init__(self, iFile, oFile, minSup, windowSize, paneSize, sep='\t'):
-        super().__init__(iFile, minSup, windowSize, paneSize, sep)
+    def __init__(self, iFile, oFile, minUtil, windowSize, paneSize, sep = ","):
+        super().__init__(iFile, minUtil, windowSize, paneSize, sep)
         self._oFile = oFile
 
-    def __creatingItemSets(self):
+    def _createItemsets(self):
         """
-            Storing the complete transactions of the database/input file in a database variable
+            Storing the complete transactions of the database/input file in a transaction variable
         """
-        self.__Database = []
-        if isinstance(self._iFile, _fp._pd.DataFrame):
+        self._transactions, self._utilities, self._utilitySum = [], [], []
+        if isinstance(self._iFile, _hus._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self.__Database = self._iFile['Transactions'].tolist()
-
+                self._transactions = self._iFile['Transactions'].tolist()
+            if 'Utilities' in i:
+                self._utilities = self._iFile['Utilities'].tolist()
+            if 'UtilitySum' in i:
+                self._utilitySum = self._iFile['UtilitySum'].tolist()
         if isinstance(self._iFile, str):
-            if _fp._validators.url(self._iFile):
-                data = _fp._urlopen(self._iFile)
+            if _hus._validators.url(self._iFile):
+                data = _hus._urlopen(self._iFile)
                 for line in data:
-                    line.strip()
                     line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    self.__Database.append(temp)
+                    line = line.split("\n")[0]
+                    parts = line.split(":")
+                    items = parts[0].split(self._sep)
+                    self.__transactions.append([x for x in items if x])
+                    utilities = parts[2].split(self._sep)
+                    utilities = [float(x) for x in utilities]
+                    self.__utilities.append(utilities)
+                    self.__utilitySum.append(int(parts[1]))
             else:
                 try:
                     with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
-                            line.strip()
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            self.__Database.append(temp)
+                            line = line.split("\n")[0]
+                            parts = line.split(":")
+                            items = parts[0].split(self._sep)
+                            self._transactions.append([x for x in items if x])
+                            utilities = parts[2].split(self._sep)
+                            utilities = [float(x) for x in utilities]
+                            self._utilities.append(utilities)
+                            self._utilitySum.append(float(parts[1]))
                 except IOError:
                     print("File Not Found")
                     quit()
 
-    def __convert(self, value):
+    def minPathUtil(self, nodeIndex, stack):
         """
-            to convert the type of user specified minSup value
+            Calculates the minimum utility of the path from the root to the ends of the tree
 
-            :param value: user specified minSup value
+            Parameters
+            ----------
+                nodeIndex : int
+                    index of the node in the stack
 
-            :return: converted type
-        """
+                stack : list
+                    list of the nodes in the prefix branch
 
-        if type(value) is int:
-            value = int(value)
-        if type(value) is float:
-            value = (len(self.__Database) * value)
-        if type(value) is str:
-            if '.' in value:
-                value = float(value)
-                value = (self.__paneSize * self.__windowSize * value)
-            else:
-                value = int(value)
-        return value
-    
-    def getRestructuredTree(self,tree):
+            Returns
+            -------
+                minUtil : int
+                    minimum utility of the path from the root to the ends of the tree
         """
-            Restructures the tree by removing the oldest batch from the tree and updating the new batch in the tree.
 
-            :param tree: Existing CPSTree object to be restructured
+        minUtil = 0
+        activeBatch = [i for i, e in enumerate(stack[0].utility) if e != 0]
+
+        for batch in activeBatch:
+            if(stack[nodeIndex + 1].tail == None or stack[nodeIndex + 1].tail[batch] == False):
+                minUtil += (stack[nodeIndex].utility[batch] - stack[nodeIndex + 1].utility[batch])
             
-            :return: restructuredTree: CPSTree object after performing branch sorting
-        """
-        restructuredTree = _CPSTree(tree.windowSize, tree.paneSize)
-        self.getBranches(tree.root, restructuredTree, tree)
-        restructuredTree.curBatchIndex = tree.curBatchIndex
-        return restructuredTree
+        return minUtil
+        
 
-    def getBranches(self,root, restructuredTree, origTree, curBranch = []):
+    def createPrefixBranch(self, root):
         """
-            Gets the branches of the tree and updates it to the restructured tree.
+            Creates the prefix branch of the node
 
-            :param root: CPSTreeNode object for the root of the original tree
-            :param restructuredTree: CPSTree object
-            :param origTree: CPSTree object for the original tree
-            :param curBranch: list of CPSTreeNode objects that needs to be sorted
+            Parameters
+            ----------
+                root : _Node
+                    pointer to the root node of the sub-tree
+
+            Returns
+            -------
+                stack : list
+                    list of the nodes in prefix branch
+
+                curUtil : int
+                    utility of the prefix branch
         """
+        stack = []
 
-        if(root is None):
-            return
+        while(root is not None):
+            stack.append(root)
+            root = root.parent
 
-        for childItem in root.children:
-            updatedBranch = curBranch.copy()
-            updatedBranch.append(root.children[childItem])
-            self.getBranches(root.children[childItem], restructuredTree, origTree, updatedBranch)
-
-        if(len(root.children) == 0 or root.tail is not None):
-            finalBranch = curBranch.copy()
-            supportCount = {}
-
-            for node in finalBranch:
-                supportCount[node.itemId] = sum(finalBranch[-1].tail)
-
-            curTrans = [node.itemId for node in finalBranch]
-            curTrans = origTree.headerTable.orderTransaction(curTrans)
-            restructuredTree.addTransaction(curTrans, restructuring=True, supportValue=supportCount, tailNode = finalBranch[-1].tail)
-    
-    def printTree(self, root, level = 0):
-        """
-            Prints the tree in a readable format.
+        chosenItemset = stack[0]
+        lastUtil = sum(chosenItemset.utility)
+        curBacthes = [i for i, e in enumerate(chosenItemset.utility) if e != 0]
 
-            :param root: CPSTreeNode object for the root of the tree
-            :param level: Current level of the root node
-        """
+        otherUtilites = []
 
-        print('  ' * level, level, root.itemId, root.counter, root.parent.itemId if root.parent else None )
-        
-        if(len(root.children) == 0 or root.tail != None):
-            print('  ' * (level + 1), level + 1, root.tail)
-        
-        for child in root.children.values():
-            self.printTree(child, level + 1)
+        for i in range(1, len(stack)-1):
+            curItemset = stack[i]
+            epu = lastUtil
 
-    def createPrefixBranch(self, root):
-        """
-            Creates the prefix branch for the given node.
+            for j in range(i-1, 0, -1):
+                epu -= self.minPathUtil(j, stack)
+            
+            otherUtilites.append(epu)
 
-            :param root: CPSTreeNode object for the root of the tree
+        return stack, lastUtil, otherUtilites
 
-            :return: prefixBranch: list of CPSTreeNode objects for the prefix branch
+    def fixUtility(self, root):
         """
+            Fixes the utility of the nodes in the tree by merging the utility values
 
-        stack = []
-        while(root is not None):
-            stack.append(root)
-            root = root.parent
+            Parameters
+            ----------
+                root : _Node
+                    pointer to the root node of the sub-tree
+        """
+        
+        if(root is None):
+            return
+        
+        if(len(root.utility) > 1):
+            root.utility = [sum(root.utility)]
 
-        chosenItemset = stack[0]
-        lastSupport = chosenItemset.counter
-        return stack, lastSupport
+        for child in root.children:
+            self.fixUtility(root.children[child])
 
-    def createConditionalTree(self, root, transactions, minSupport):
+    def createConditionalTree(self, root, transactions, minUtil):
         """
-            Creates the conditional tree for the given node.
+            Creates the conditional tree for the given prefix tree
 
-            :param root: CPSTreeNode object for the root of the tree for which conditional tree needs to be created
-            :param transactions: list of transactions which needs to be added to the conditional tree
-            :param minSupport: minimum support value for the conditional tree
+            Parameters
+            ----------
+                root : _Node
+                    pointer to the root node of the prefix tree
 
-            :return: conditionalTree: CPSTree object for the conditional tree
-        """    
-    
+                transactions : list
+                    list of transactions in prefix tree
+
+                minUtil : int
+                    minimum utility threshold
+
+            Returns
+            -------
+                tempTree : _SHUTree
+                    conditional tree for the given prefix tree
+        """
+        
         for transaction in transactions:
             for item in transaction["transaction"]:
-                if root.headerTable.table[item][0] < minSupport:
+                if(root.headerTable.table[item][0] < minUtil):
+                    itemIndex = transaction["transaction"].index(item)
                     transaction["transaction"].remove(item)
+                    del transaction["itemwiseUtility"][itemIndex]
 
-        conditionalTree = _CPSTree(1, 1)
-
+        tempTree = _SHUTree(1, 1, True)
         for transaction in transactions:
-            if(len(transaction["transaction"]) > 0):
-                conditionalTree.addTransaction(transaction["transaction"], restructuring=True, supportValue=transaction["support"])
-
-        return conditionalTree      
+            if(len(transaction["transaction"]) != 0):
+                tempTree.addTransaction(transaction["transaction"], transaction["utility"], transaction["itemwiseUtility"])
 
-    def itemSetGeneration(self, root, minSupport, candidatePattern, curItem = []):
 
+        return tempTree
+    
+    def contains(self, superset, subset):
         """
-            Generates the candidate patterns for the given CPS Tree.
+            Checks if the superset contains the subset
 
-            :param root: CPSTreeNode object for the root of the tree for which itemset needs to be generated
-            :param minSupport: minimum support value for the conditional tree
-            :param candidatePattern: list of candidate patterns generated
-            :param curItem: list of CPSTreeNode objects for the current itemset
-
-            :return: candidatePattern: list of candidate patterns
+            Parameters
+            ----------
+                superset : list
+                    list of items in the superset
+
+                subset : list
+                    list of items in the subset
+
+            Returns
+            -------
+                bool
+                    True if superset contains subset, False otherwise
+        """
+     
+        return reduce(and_, [i in superset for i in subset])
+
+    def treeGenerations(self, root, netUtil, candidatePattern, curItem = []):
+        """
+            Generates the tree of the high utility patterns
+
+            Parameters
+            ----------
+                root : _Node
+                    pointer to the root of the tree
+                netUtil : int
+                    Net utility of the transaction
+                candidatePattern : list
+                    Candidate patterns generated with utility
+                curItem : list
+                    List of items in the current itemsets
         """
-        if(root is None or root.root is None):
+
+        if(root is None):
             return
 
-        for item in root.headerTable.orderedItems:
-            if root.headerTable.table[item][0] >= minSupport:
+
+        for item in reversed(root.headerTable.orderedItems):
+            if(root.headerTable.table[item][0] >= netUtil):
                 prefixBranches = []
-                tempNode = root.headerTable.table[item][1]
 
-                while(tempNode is not None):
-                    curPrefixBranch, netSupport = self.createPrefixBranch(tempNode)
-                    tempBranch = [node.itemId for node in curPrefixBranch]
-                    supportCount = {}
-                    for each_item_node in curPrefixBranch:
-                        supportCount[each_item_node.itemId] = netSupport
+                tempNode = root.headerTable.table[item][1]
 
-                    prefixBranches.append([tempBranch, supportCount])
+                while tempNode is not None:
+                    curPrefixBranch, lastUtil, otherUtilites = self.createPrefixBranch(tempNode)
+                    prefixBranches.append([curPrefixBranch, lastUtil, otherUtilites])
                     tempNode = tempNode.next
-
-                prefixTree = _CPSTree(1, 1)
+                
+                prefixTree = _SHUTree(1, 1, True)
                 completeTransactions = []
 
                 for branch in prefixBranches:
                     transaction = []
-                    for nodeIndex in range(len(branch[0])-2,0,-1):
-                        transaction.append(branch[0][nodeIndex])
-                    
-                    prefixTree.addTransaction(transaction, restructuring=True, supportValue=branch[1])
-                    completeTransactions.append({"transaction": transaction, "support": branch[1]})
+                    utilities = []
+                    for idx in range(len(branch[2])-1, -1, -1):
+                        transaction.append(branch[0][(idx + 1)].itemName)
+                        utilities.append(branch[2][idx])
+
+                    prefixTree.addTransaction(transaction, branch[1], utilities)
+
+                    completeTransactions.append({"transaction" : transaction, "utility" : branch[1], "itemwiseUtility" : utilities})
+
+                conditionalTree = self.createConditionalTree(prefixTree, completeTransactions, netUtil)
 
-                conditionalTree = self.createConditionalTree(prefixTree, completeTransactions, minSupport)
                 newItemset = curItem.copy()
                 newItemset.append(item)
 
                 if(len(newItemset) not in candidatePattern):
-                    candidatePattern[len(newItemset)] = [{"pattern" : newItemset, "support" : root.headerTable.table[item][0]}]
+                    candidatePattern[len(newItemset)] = [newItemset]
 
                 else:
-                    candidatePattern[len(newItemset)].append({"pattern" : newItemset, "support" : root.headerTable.table[item][0]})
+                    candidatePattern[len(newItemset)].append(newItemset)
 
-                if(len(conditionalTree.headerTable.table) > 0):
-                    self.itemSetGeneration(conditionalTree, minSupport, candidatePattern, newItemset)
+                if(len(conditionalTree.headerTable.table) != 0):
+                    self.treeGenerations(conditionalTree, netUtil, candidatePattern, newItemset)
 
 
+    def startMine(self):
+        """
+            This function will start the mining process
+        """
+        global _minUtil
+        self.__startTime = _hus._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._minUtil is None:
+            raise Exception("Please enter the Minimum Support")
+        if self._windowSize is None:
+            raise Exception("Please enter the Window Size")
+        if self._paneSize is None:
+            raise Exception("Please enter the Pane Size")
+        self.__windowSize = int(self._windowSize)
+        self.__paneSize = int(self._paneSize)
+        
+        self._createItemsets()
+        self._minUtil = float(self._minUtil)
+        self.__tree = _SHUTree(self.__windowSize, self.__paneSize)
+        
+        transactionwiseUtility = []
+
+        for i in range(len(self._transactions)):
+            curTrans = {}
+            for j in range(len(self._transactions[i])):
+                curTrans[self._transactions[i][j]] = self._utilities[i][j]
+            transactionwiseUtility.append(curTrans)
+
+        for i in range(0, self.__windowSize):
+            self.__tree.batchIndex = i
+            for j in range(0, self.__paneSize):
+                self.__tree.addTransaction(self._transactions[i * self.__paneSize + j], self._utilitySum[i * self.__paneSize + j], self._utilities[i * self.__paneSize + j])
+
+        startIndex = 0
+        endIndex = self.__windowSize * self.__paneSize
+
+        while(endIndex <= len(self._transactions)):
+            
+            filteredItemsets = {}
+            
+            self.treeGenerations(self.__tree, self._minUtil, filteredItemsets)
+
+            results = []
+
+            for itemSetLen in filteredItemsets:
+                for itemSet in filteredItemsets[itemSetLen]:
+                    itemSetUtility = 0
+                    for transId in range(startIndex, endIndex):
+                        if(self.contains(list(transactionwiseUtility[transId].keys()), itemSet)):
+                            for item in itemSet:
+                                itemSetUtility += transactionwiseUtility[transId][item]
+                        
+                    if(itemSetUtility >= self._minUtil):
+                        results.append([itemSet, itemSetUtility])
+
+            self.__finalPatterns[(startIndex, endIndex)] = results
+
+            if(endIndex >= len(self._transactions)):
+                break
+
+            self.__tree.removeBatch()
+
+            for i in range(0, self.__paneSize):
+                self.__tree.addTransaction(self._transactions[endIndex + i], self._utilitySum[endIndex + i], self._utilities[endIndex + i])
+
+            startIndex += self.__paneSize
+            endIndex += self.__paneSize
+
+        self.__endTime = _hus._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
+        process = _hus._psutil.Process(_hus._os.getpid())
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
+
+    def printTree(self, root, level = 0):
+        """
+            Prints the tree in a readable format.
+
+            :param root: CPSTreeNode object for the root of the tree
+            :param level: Current level of the root node
+        """
+
+        print('  ' * level, level, root.itemName, root.utility, root.parent.itemName if root.parent else None )
+        
+        if(root.tail is not None):
+            print('  ' * (level + 1), level + 1, root.tail)
+
+        for child in root.children.values():
+            self.printTree(child, level + 1)
+
     def getMemoryRSS(self):
         """
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
 
             :return: returning RSS memory consumed by the mining process
 
             :rtype: float
@@ -750,15 +955,15 @@
 
         dataframe = {}
         data = []
         for x, y in self.__finalPatterns.items():
             for pattern in y:
                 patternString = ' '.join(pattern[0])
                 data.append([x[0], x[1], patternString, pattern[1]])
-        dataframe = _fp._pd.DataFrame(data, columns=['Window Start Index', 'Window End Index', 'Pattern', 'Support'])
+        dataframe = pd.DataFrame(data, columns=['Window Start Index', 'Window End Index', 'Pattern', 'Utility'])
         return dataframe
 
     def getRuntime(self):
         """
             Total amount of time taken by the mining process will be retrieved from this function
 
             :return: returning time taken by the mining process
@@ -779,101 +984,33 @@
         print("Total ExecutionTime in ms:", self.getRuntime())
 
 
     def save(self):
         """
         Complete set of frequent patterns will be loaded in to a output file
         """
-
+        print("Output file name", self._oFile)
         writer = open(self._oFile, 'w+')
         for x, y in self.__finalPatterns.items():
             writer.write("Window Start Index : %s , End Index : %s \n" % (x[0], x[1]))
             for pattern in y:
                 patternString = '\t'.join(pattern[0])
                 patternString += '\t' + ":" + '\t' + str(pattern[1])
                 writer.write("%s \n" % patternString)
 
-    def startMine(self):
-        """
-            This function will start the mining process
-        """
-        global _minSup
-        self.__startTime = _fp._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minSup is None:
-            raise Exception("Please enter the Minimum Support")
-        if self._windowSize is None:
-            raise Exception("Please enter the Window Size")
-        if self._paneSize is None:
-            raise Exception("Please enter the Pane Size")
-        self.__windowSize = int(self._windowSize)
-        self.__paneSize = int(self._paneSize)
-
-        self.__creatingItemSets()
-        self._minSup = self.__convert(self._minSup)
-        self.__tree = _CPSTree(self.__windowSize, self.__paneSize)
-
-        for i in range(0, self.__windowSize):
-            self.__tree.curBatchIndex = i
-            for j in range(0, self.__paneSize):
-                    self.__tree.addTransaction(self.__Database[i * self.__paneSize + j])
-            self.__tree = self.getRestructuredTree(self.__tree)
-
-
-        startIndex = 0
-        endIndex = self.__windowSize * self.__paneSize
-
-        while endIndex <= len(self.__Database):
-            print("Start Index: ", startIndex, "End Index: ", endIndex)
-            self.printTree(self.__tree.root)
-
-            patterns = {}
-            self.itemSetGeneration(self.__tree, self._minSup, patterns)
-
-            for patternLength in patterns:
-                for pattern in patterns[patternLength]:
-
-                    if((startIndex, endIndex) not in self.__finalPatterns):
-                        self.__finalPatterns[(startIndex, endIndex)] = []
-                    self.__finalPatterns[(startIndex, endIndex)].append((pattern["pattern"], pattern["support"]))
-
-            if(endIndex == len(self.__Database)):
-                break
-
-            self.__tree.removeBatch()
-
-            for i in range(0, self.__paneSize):
-                    self.__tree.addTransaction(self.__Database[endIndex + i])
-
-            self.__tree = self.getRestructuredTree(self.__tree)
-            startIndex += self.__paneSize
-            endIndex += self.__paneSize
-
-
-
-        self.__endTime = _fp._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
-        process = _fp._psutil.Process(_fp._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
-
-
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
-        if len(_fp._sys.argv) == 7:
-            _ap = FrequentPatternStreamMining(_fp._sys.argv[1], _fp._sys.argv[2], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
-        if len(_fp._sys.argv) == 6:
-            _ap = FrequentPatternStreamMining(_fp._sys.argv[1], _fp._sys.argv[2], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
+    if len(_hus._sys.argv) == 6 or len(_hus._sys.argv) == 7:
+        if len(_hus._sys.argv) == 7:
+            _ap = SHUGrowth(_hus._sys.argv[1], _hus._sys.argv[2], _hus._sys.argv[3], _hus._sys.argv[4], _hus._sys.argv[5], _hus._sys.argv[6])
+        if len(_hus._sys.argv) == 6:
+            _ap = SHUGrowth(_hus._sys.argv[1], _hus._sys.argv[2], _hus._sys.argv[3], _hus._sys.argv[4], _hus._sys.argv[5])
         _ap.startMine()
-        print("Total number of Frequent Patterns:", len( _ap.getPatterns()))
-
-        print(_ap.getPatternsAsDataFrame().to_csv("result.csv", index = False, sep='\t'))
+        print("Total number of Windows Processes:", len( _ap.getPatterns()))
+        _ap.getPatternsAsDataFrame().to_csv("result.csv", index = False, sep='\t')
         _ap.save()
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py` & `pami-2023.8.1/PAMI/coveragePattern/basic/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,224 +1,168 @@
-__copyright__ = """
 #  Copyright (C)  2021 Rage Uday Kiran
 #
 #      This program is free software: you can redistribute it and/or modify
 #      it under the terms of the GNU General Public License as published by
 #      the Free Software Foundation, either version 3 of the License, or
 #      (at your option) any later version.
 #
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
 
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
+import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
-import functools as _functools
 
 
-class _frequentPatternsStream(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
+class _coveragePatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every coverage pattern mining algorithm must
         employ in PAMI
 
-
-       Attributes:
-       ----------
+       Attributes
+        ----------
         iFile : str
             Input file name or path of the input file
-        minSup: integer or float or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        minCS: int or float or str
+            The user can specify minCS either in count or proportion of database size.
+            If the program detects the data type of minCS is integer, then it treats minCS is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minCS=10 will be treated as integer, while minCS=10.0 will be treated as float
+        maxOR: int or float or str
+            The user can specify maxOR either in count or proportion of database size.
+            If the program detects the data type of maxOR is integer, then it treats maxOR is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxOR=10 will be treated as integer, while maxOR=10.0 will be treated as float
+        minRF: int or float or str
+            The user can specify minRF either in count or proportion of database size.
+            If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator
-        startTime:float
+            However, the users can override their default separator.
+        startTime: float
             To record the start time of the algorithm
-        endTime:float
+        endTime: float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of frequent patterns
+            Name of the output file to store complete set of coverage patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
 
-       Methods:
-       -------
+        Methods
+        -------
         startMine()
-            Calling this function will start the actual mining process
+            Mining process will start from here
         getPatterns()
-            This function will output all interesting patterns discovered by an algorithm
+            Complete set of patterns will be retrieved with this function
         save(oFile)
-            This function will store the discovered patterns in an output file specified by the user
+            Complete set of coverage patterns will be loaded in to a output file
         getPatternsAsDataFrame()
-            The function outputs the patterns generated by an algorithm as a data frame
+            Complete set of coverage patterns will be loaded in to data frame
         getMemoryUSS()
-            This function outputs the total amount of USS memory consumed by a mining algorithm
+            Total amount of USS memory consumed by the program will be retrieved from this function
         getMemoryRSS()
-            This function outputs the total amount of RSS memory consumed by a mining algorithm
+            Total amount of RSS memory consumed by the program will be retrieved from this function
         getRuntime()
-            This function outputs the total runtime of a mining algorithm
-
+            Total amount of runtime taken by the program will be retrieved from this function
     """
 
-    def __init__(self, iFile, minSup, windowSize, paneSize, sep="\t"):
+    def __init__(self, iFile, minRF, minCS, maxOR, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str or DataFrame
-        :param minSup: The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        :type iFile: str
+        :param minRF: The user can specify minimum relative frequency either in count or proportion of database size.
+            If the program detects the data type of minRF is integer, then it treats minRF is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minRF=10 will be treated as integer, while minRF=10.0 will be treated as float
+        :type minRF: int or float or str
+        :param minCS: The user can specify minimum coverage support either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        :type minSup: int or float or str
-        :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        :param maxOR: The user can specify maximum overlap ratio either in count or proportion of database size.
+        :type maxOR: int or float or str
+        :param sep: separator used in user specified input file
         :type sep: str
         """
 
         self._iFile = iFile
+        self._minCS = minCS
+        self._minRF = minRF
+        self._maxOR = maxOR
         self._sep = sep
-        self._minSup = minSup
-        self._windowSize = windowSize
-        self._paneSize = paneSize
         self._finalPatterns = {}
-        self._oFile = str()
-        self._memoryUSS = float()
-        self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
-
-    '''@abstractmethod
-    def iFile(self):
-        """Variable to store the input file path/file name"""
-
-        pass
-
-    @abstractmethod
-    def minSup(self):
-        """Variable to store the user-specified minimum support value"""
-
-        pass
-
-    @abstractmethod
-    def sep(self):
-        """Variable to store the user-specified minimum support value"""
-
-        pass
-
-    @abstractmethod
-    def startTime(self):
-        """Variable to store the start time of the mining process"""
-
-        pass
-
-    @abstractmethod
-    def endTime(self):
-        """Variable to store the end time of the complete program"""
-
-        pass
-
-    @abstractmethod
-    def memoryUSS(self):
-        """Variable to store USS memory consumed by the program"""
-
-        pass
-
-    @abstractmethod
-    def memoryRSS(self):
-        """Variable to store RSS memory consumed by the program"""
-
-        pass
-
-    @abstractmethod
-    def finalPatterns(self):
-        """Variable to store the complete set of patterns in a dictionary"""
-
-        pass
-
-    @abstractmethod
-    def oFile(self):
-        """Variable to store the name of the output file to store the complete set of frequent patterns"""
-
-        pass'''
+        self._memoryRSS = float()
+        self._memoryUSS = float()
+        self._oFile = " "
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of frequent patterns generated will be retrieved from this function"""
+        """Complete set of coverage patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of frequent patterns will be saved in to an output file from this function
+        """Complete set of coverage patterns will be saved in to an output file from this function
 
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of coverage patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
-
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print result of the execution"""
+        """ To print the results of the execution"""
 
         pass
```

### Comparing `pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py` & `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/HUPMS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py` & `pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,1016 +1,765 @@
-#  Copyright (C)  2021 Rage Uday Kiran
+# **Importing this algorithm into a python program**
+# --------------------------------------------------------
 #
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
 #
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
+#     from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 #
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-import abstract as _hus
-import pandas as pd
-from functools import reduce
-from operator import and_ 
-
-_minSup = str()
-_hus._sys.setrecursionlimit(20000)
+#     obj = alg.basic(iFile, wFile, expSup, expWSup)
+#
+#     obj.startMine()
+#
+#     Patterns = obj.getPatterns()
+#
+#     print("Total number of  Patterns:", len(Patterns))
+#
+#     obj.savePatterns(oFile)
+#
+#     Df = obj.getPatternsAsDataFrame()
+#
+#     memUSS = obj.getMemoryUSS()
+#
+#     print("Total Memory in USS:", memUSS)
+#
+#     memRSS = obj.getMemoryRSS()
+#
+#     print("Total Memory in RSS", memRSS)
+#
+#     run = obj.getRuntime()
+#
+#     print("Total ExecutionTime in seconds:", run)
 
 
-class _Node:
-    """
-        A class used to represent a node in the SHU tree
+__copyright__ = """
+ Copyright (C)  2021 Rage Uday Kiran
 
-        Attributes
-        ----------
-            itemName : str
-                name of the item
+     This program is free software: you can redistribute it and/or modify
+     it under the terms of the GNU General Public License as published by
+     the Free Software Foundation, either version 3 of the License, or
+     (at your option) any later version.
 
-            utility : int
-                utility of the item
+     This program is distributed in the hope that it will be useful,
+     but WITHOUT ANY WARRANTY; without even the implied warranty of
+     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+     GNU General Public License for more details.
 
-            children : dict
-                dictionary of children of the node
+     You should have received a copy of the GNU General Public License
+     along with this program.  If not, see <https://www.gnu.org/licenses/>.
+     Copyright (C)  2021 Rage Uday Kiran
 
-            next : _Node
-                pointer to the next node with same item in the tree
+"""
 
-            batchIndex : int
-                index of the batch with respect to window to which the node belongs
-            
-            utility : list
-                list of utilities of the node with respect to each batch in the window
+from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
 
-            parent : _Node
-                pointer to the parent of the node
+_expSup = str()
+_expWSup = str()
+_weights = {}
+_finalPatterns = {}
+_ab._sys.setrecursionlimit(20000)
 
-        Methods
-        -------
 
-            addUtility(utility, batchIndex)
-                Adds utility to the node at specified batch index
+class _Item:
+    """
+    A class used to represent the item with probability in transaction of dataset
+    ...
+    Attributes:
+    __________
+        item : int or word
+            Represents the name of the item
+        probability : float
+            Represent the existential probability(likelihood presence) of an item
+    """
 
-            removeUtility(utility)
-                Removes utility from the node
+    def __init__(self, item, probability):
+        self.item = item
+        self.probability = probability
 
-            shiftUtility()
-                Shifts the utility values of the node to the left useful for removing the oldest batch information
 
-            shiftTail()
-                Shifts the tail values of the node to the left useful for removing the oldest batch information
+class _Node(object):
+    """
+    A class used to represent the node of frequentPatternTree
+        ...
+    Attributes:
+    ----------
+        item : int
+            storing item of a node
+        probability : int
+            To maintain the expected support of node
+        parent : node
+            To maintain the parent of every node
+        children : list
+            To maintain the children of node
+    Methods:
+    -------
+        addChild(itemName)
+            storing the children to their respective parent nodes
     """
 
-    def __init__(self, itemName, utility, batchSize, batchIndex):
-        self.itemName = itemName
-        self.utility = [0 for _ in range(batchSize)]
-        self.children = dict()
-        self.next = None
-        self.batchIndex = batchIndex
-        self.utility[batchIndex] = utility
+    def __init__(self, item, children):
+        self.item = item
+        self.probability = 1
+        self.children = children
         self.parent = None
-        self.tail = None
-
-    def addUtility(self, utility, batchIndex):
-        """
-            Adds utility to the node
-
-            Parameters
-            ----------
-                utility : int
-                    Net utility value to be added
-
-                batchIndex : int
-                    index of the batch with respect to window to which the node belongs
-        """
-
-        self.utility[batchIndex] += utility
-
-    def removeUtility(self, utility):
-        """
-            Removes utility from the node
-
-            Parameters
-            ----------
-                utility : int
-                    Net utility value to be removed
-        """
-
-        self.utility -= utility
-
-    def shiftUtility(self):
-        """
-            Shifts the utility values of the node to the left
-        """
-        self.utility.pop(0)
-        self.utility.append(0)
-
-    def shiftTail(self):
-        """
-            Shifts the tail pointer of the node to the left
-        """
 
-        if(self.tail is not None):
-            self.tail.pop(0)
-            self.tail.append(False)
+    def addChild(self, node):
+        self.children[node.item] = node
+        node.parent = self
 
 
-class _HeaderTable:
+class _Tree(object):
     """
-        A class used to represent the header table of the SHU tree
-
-        Attributes
-        ----------
-            table : dict
-                dictionary of items as keys and list of utility and pointer to the node in the tree as values
-                representing the header table
-
-            orderedItems : list
-                list of items in the header table in lexicographical order
-
-        Methods
-        -------
-            updateUtility(item, utility, node)
-                Updates the utility of the item with node pointer in the header table
-
-            addUtility(item, utility)
-                Adds utility to the item in the header table
-
-            removeUtility(item, utility)
-                Removes utility from the item in the header table
-
-            itemOrdering()
-                Orders the items in the header table in lexicographical order
+    A class used to represent the frequentPatternGrowth tree structure
+    ...
+    Attributes:
+    ----------
+        root : Node
+            Represents the root node of the tree
+        summaries : dictionary
+            storing the nodes with same item name
+        info : dictionary
+            stores the support of items
+    Methods:
+    -------
+        addTransaction(transaction)
+            creating transaction as a branch in frequentPatternTree
+        addConditionalPattern(prefixPaths, supportOfItems)
+            construct the conditional tree for prefix paths
+        conditionalPatterns(Node)
+            generates the conditional patterns from tree for specific node
+        conditionalTransactions(prefixPaths,Support)
+            takes the prefixPath of a node and support at child of the path and extract the frequent items from
+            prefixPaths and generates prefixPaths with items which are frequent
+        remove(Node)
+            removes the node from tree once after generating all the patterns respective to the node
+        generatePatterns(Node)
+            starts from the root node of the tree and mines the frequent patterns
     """
 
     def __init__(self):
-        self.table = dict()
-        self.orderedItems = list()
-
-    def updateUtility(self, item, utility, node):
-        """
-            Updates the utility of the item in the header table
-
-            Parameters
-            ----------
-                item : str
-                    name of the item to which utility needs to be updated
-
-                utility : int
-                    Net utility of the item to be updated
-
-                node : _Node
-                    pointer to the node in the tree to which the item belongs
-        """
-
-        if item in self.table:
-            self.table[item][0] += utility
-            tempNode = self.table[item][1]
-
-            while tempNode.next is not None:
-                tempNode = tempNode.next
-            
-            tempNode.next = node
-
-        else:
-            self.table[item] = [utility, node]
-    
-        self.itemOrdering()
-
-    def addUtility(self, item, utility):
-        """
-            Adds utility to the item in the header table
-
-            Parameters
-            ----------
-                item : str
-                    name of the item to which utility needs to be added
-
-                utility : int
-                    Net utility of the item to be added
-        """
-        self.table[item][0] += utility
-    
-
-    def removeUtility(self, item, utility):
-        """
-            Removes utility from the item in the header table
-
-            Parameters
-            ----------
-                item : str
-                    name of the item to which utility needs to be removed
-
-                utility : int
-                    Net utility of the item to be removed
-        """
-        self.table[item][0] -= utility
-
-        if self.table[item][0] == 0:
-            del self.table[item]
-
-        self.itemOrdering()
-
-    def itemOrdering(self):
+        self.root = _Node(None, {})
+        self.summaries = {}
+        self.info = {}
+
+    def addTransaction(self, transaction):
+        """adding transaction into tree
+            :param transaction : it represents the one self.Database in database
+            :type transaction : list
         """
-            Orders the items in the header table in lexicographical order
-        """        
-        self.orderedItems = list(sorted(self.table.keys()))
 
-class _SHUTree:
-
-    """
-        A class used to represent the SHU tree
-
-        Attributes
-        ----------
-            root : _Node
-                root node of the tree
-
-            headerTable : _HeaderTable
-                header table of the tree
-
-            batchSize : int
-                size of the batch
-
-            windowSize : int
-                size of the window
-
-            batchIndex : int
-                index of the current batch with respect to window
-
-            windowUtility : int
-                utility of the current window
-
-            localTree : bool
-                flag to indicate whether the tree is local useful for prefix/conditional tree generation
-
-        Methods
-        -------
-            addTransaction(transaction, utility)
-                Adds transaction to the tree
-
-            tailUtilities(root)
-                Returns the tail utilities of the tree
-
-            removeBatch()
-                Removes the oldest batch from the tree
-
-            removeBatchUtility()
-                Removes the utility of the oldest batch from each subtree
-
-    """
-
-    def __init__(self, batchSize, windowSize, localTree = False):
-        self.root = _Node(None, 0, batchSize, 0)
-        self.headerTable = _HeaderTable()
-        self.batchSize = batchSize
-        self.windowSize = windowSize
-        self.batchIndex = 0
-        self.windowUtility = 0
-        self.localTree = localTree
-
-    def addTransaction(self, transaction, utility, itemUtility = None):
-        """
-            Adds transaction to the tree
-
-            Parameters
-            ----------
-                transaction : list
-                    list of items in the transaction
-
-                utility : int
-                    Net utility of the transaction
-
-        """
-        # print("Transaction", transaction, itemUtility, self.localTree)
-        transaction.sort(key = lambda x: x[0])
         currentNode = self.root
-        self.windowUtility += utility
-
-        curUtility = 0
-        for iter in range(len(transaction)):
-            
-            item = transaction[iter]
-
-            if(self.localTree is False):
-                curUtility += itemUtility[iter]
-            else:
-                curUtility = itemUtility[iter]
-
-            
-            if item in currentNode.children:
-                currentNode = currentNode.children[item]
-                currentNode.addUtility(curUtility, self.batchIndex)
-
-                if(self.localTree is False):
-                    self.headerTable.addUtility(item, curUtility)
-
+        for i in range(len(transaction)):
+            if transaction[i].item not in currentNode.children:
+                newNode = _Node(transaction[i].item, {})
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    newNode.probability = transaction[i].probability
                 else:
-                    self.headerTable.addUtility(item, utility)
-
-            else:
-                newNode = _Node(item, curUtility, self.batchSize, self.batchIndex)
-                currentNode.children[item] = newNode
-                newNode.parent = currentNode
-
-                if(self.localTree is False):
-                    self.headerTable.updateUtility(item, curUtility, newNode)
-
+                    newNode.probability = max(lp) * transaction[i].probability
+                currentNode.addChild(newNode)
+                if transaction[i].item in self.summaries:
+                    self.summaries[transaction[i].item].append(newNode)
                 else:
-                    self.headerTable.updateUtility(item, utility, newNode)
-                
+                    self.summaries[transaction[i].item] = [newNode]
                 currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i].item]
+                l1 = i - 1
+                lp = []
+                while l1 >= 0:
+                    lp.append(transaction[l1].probability)
+                    l1 -= 1
+                if len(lp) == 0:
+                    currentNode.probability += transaction[i].probability
+                else:
+                    currentNode.probability += max(lp) * transaction[i].probability
 
-        currentNode.tail = [False for _ in range(self.batchSize)]
-        currentNode.tail[self.batchIndex] = True
-
-    def tailUtilities(self, root):
-        """
-            Calculates the utility of the tail of the node
-            
-            Parameters
-            ----------
-                root : _Node
-                    pointer to the node in the tree
-
-            Returns
-            -------
-                netUtility : int
-                    utility of the tail of the node
-        """
-
-        if(root is None):
-            return 0
-
-        if(root.tail is not None):
-            return root.utility[0]
-
-        netUtility = 0
-        for item in root.children:
-            netUtility += self.tailUtilities(root.children[item])
-
-        return netUtility
-
-    def removeBatch(self):
-
-        """
-            Removes the oldest batch from the tree
+    def addConditionalPattern(self, transaction, sup):
+        """constructing conditional tree from prefixPaths
+            :param transaction : it represents the one self.Database in database
+            :type transaction : list
+            :param sup : support of prefixPath taken at last child of the path
+            :type sup : int
         """
 
+        # This method takes transaction, support and constructs the conditional tree
         currentNode = self.root
-
-        curChilds = list(currentNode.children.keys())
-
-        for child in curChilds:
-            self.windowUtility -= self.tailUtilities(currentNode.children[child])
-            self.removeBatchUtility(currentNode.children[child])
-
-            if(sum(currentNode.children[child].utility) == 0):
-                del currentNode.children[child]
-
-
-    def removeBatchUtility(self, tempNode = None):
-        
-        """
-            Removes the utility of the oldest batch from each subtree
-
-            Parameters
-            ----------
-                tempNode : _Node
-                    pointer to the node in the tree
-
-        """
-        if tempNode is None:
-            return
-
-        for item in tempNode.children:
-            self.removeBatchUtility(tempNode.children[item])
-
-        curBatchUtility = tempNode.utility[0]
-        tempNode.shiftUtility()
-        tempNode.shiftTail()
-
-        if(sum(tempNode.utility) == 0):
-            if(tempNode.itemName in self.headerTable.table):
-                curNode = self.headerTable.table[tempNode.itemName][1]
-
-                if(curNode == tempNode):
-                    self.headerTable.table[tempNode.itemName][1] = tempNode.next
-
+        for i in range(len(transaction)):
+            if transaction[i] not in currentNode.children:
+                newNode = _Node(transaction[i], {})
+                newNode.probability = sup
+                currentNode.addChild(newNode)
+                if transaction[i] in self.summaries:
+                    self.summaries[transaction[i]].append(newNode)
                 else:
-                    while(curNode != None and curNode.next != tempNode):
-                        curNode = curNode.next
+                    self.summaries[transaction[i]] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i]]
+                currentNode.probability += sup
 
-                    if(curNode != None):
-                        curNode.next = tempNode.next
+    def conditionalPatterns(self, alpha):
+        """generates all the conditional patterns of respective node
+            :param alpha : it represents the Node in tree
+            :type alpha : _Node
+        """
+
+        # This method generates conditional patterns of node by traversing the tree
+        finalPatterns = []
+        sup = []
+        for i in self.summaries[alpha]:
+            s = i.probability
+            set2 = []
+            while i.parent.item is not None:
+                set2.append(i.parent.item)
+                i = i.parent
+            if len(set2) > 0:
+                set2.reverse()
+                finalPatterns.append(set2)
+                sup.append(s)
+        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
+        return finalPatterns, support, info
+
+    def removeNode(self, nodeValue):
+        """removing the node from tree
+            :param nodeValue : it represents the node in tree
+            :type nodeValue : node
+        """
+
+        for i in self.summaries[nodeValue]:
+            del i.parent.children[nodeValue]
+
+    def conditionalTransactions(self, condPatterns, support):
+        """ It generates the conditional patterns with frequent items
+                :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
+                :type condPatterns : list
+                :support : the support of conditional pattern in tree
+                :support : int
+        """
+
+        global _expSup, _expWSup
+        pat = []
+        sup = []
+        count = {}
+        for i in range(len(condPatterns)):
+            for j in condPatterns[i]:
+                if j in count:
+                    count[j] += support[i]
+                else:
+                    count[j] = support[i]
+        updatedDict = {}
+        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
+        count = 0
+        for p in condPatterns:
+            p1 = [v for v in p if v in updatedDict]
+            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
+            if len(trans) > 0:
+                pat.append(trans)
+                sup.append(support[count])
+                count += 1
+        return pat, sup, updatedDict
+
+    def generatePatterns(self, prefix):
+        """generates the patterns
+            :param prefix : forms the combination of items
+            :type prefix : list
+        """
+
+        global _finalPatterns, _expSup, _expWSup, _weights
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
+            pattern = prefix[:]
+            pattern.append(i)
+            weight = 0
+            for k in pattern:
+                weight = weight + _weights[k]
+            weight = weight/len(pattern)
+            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
+                _finalPatterns[tuple(pattern)] = self.info.get(i)
+                patterns, support, info = self.conditionalPatterns(i)
+                conditionalTree = _Tree()
+                conditionalTree.info = info.copy()
+                for pat in range(len(patterns)):
+                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
+                if len(patterns) > 0:
+                    conditionalTree.generatePatterns(pattern)
+            self.removeNode(i)
 
-                del tempNode.tail
-        
-        self.headerTable.removeUtility(tempNode.itemName, curBatchUtility)
-
-        curChilds = list(tempNode.children.keys())
-        for child in curChilds:
-            if(sum(tempNode.children[child].utility) == 0):
-                del tempNode.children[child]
 
-    
-class SHUGrowth(_hus._highUtilityPatternStreamMining):
+class WUFIM(_ab._weightedFrequentPatterns):
     """
-        High-utility pattern mining over data stream is one of the challenging problems in data stream mining.
-        SHUGrowth is an algorithm that discovers high-utility patterns from data streams without rebuilding the tree.
-        It stores the database of the current window in form of SHUTree and adjusts the tree based on upcoming
-        transactions removing the oldest batch. It is an optimized varaint of HUPMS algorithm.
-
-        References
-        ----------
-            Chowdhury Farhan Ahmed and Syed Khairuzzaman Tanbeer and Byeong-Soo Jeong and Ho-Jin Choi : High utility 
-            pattern mining over data streams with sliding window technique. Expert Systems with Applications Vol 57, 
-            214 - 231, 2016. https://doi.org/10.1016/j.eswa.2016.03.001
-
-
-        Attributes:
-        ----------
-
-            __startTime : float
-                start time of the mining process
-
-            __endTime : float
-                end time of the mining process
-
-            _minUtil : str
-                minimum utility threshold
-
-            __finalPatterns : dict
-                dictionary of the final patterns generated in each window
-
-            _iFile : str
-                input file name
-
-            _oFile : str
-                output file name
-
-            _sep : str
-                seperator of the input file
-
-            __memoryUSS : float
-                memory usage of the algorithm in user space
-
-            __memoryRSS : float
-                memory usage of the algorithm in resident set size
-
-            __transactions : list
-                list of transactions in the database
-
-            __utilities : list
-                list of utilities of each item of a transaction in the database
-
-            __utilitySum : list
-                list of utility sum of each transaction in the database
-
-            __tree : _SHUTree
-                SHU tree of the current window
-
-            __windowSize : int
-                The size of the sliding window. It specifies the number of panes to be considered for mining patterns.
-
-            __paneSize : int
-                The size of the pane. It specifies the number of transactions to be considered for mining in each pane.
-
-            
-
-        Methods:
-        -------
-            _createItemsets()
-                Storing the complete transactions of the database/input file in a transaction variable with their utilities.
-
-            minPathUtil(nodeIndex, stack)
-                Calculates the minimum utility of the path from the root to the ends of the tree
-            
-            createPrefixBranch(root)
-                Creates the prefix branch of the current SHU-Tree for construction of prefix tree
-
-            fixUtility(root)
-                Fixes the utility of the nodes in the tree by merging the utility values
-
-            createConditionalTree(root, transactions, minUtil)
-                Creates the conditional tree for the given prefix tree
+    Description:
+    -------------
+        It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database
+        using PUF-Tree.
+
+    Reference:
+    ------------
+        Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases, In book: Machine Learning and Data Mining in Pattern Recognition
+        Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
+
+    Attributes:
+    ------------
+        iFile : file
+            Name of the Input file or path of the input file
+        wFile : file
+            Name of the Input file or path of the input file
+        oFile : file
+            Name of the output file or path of the output file
+        minSup: float or int or str
+            The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        sep : str
+            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            However, the users can override their default separator.
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
+        startTime:float
+            To record the start time of the mining process
+        endTime:float
+            To record the completion time of the mining process
+        Database : list
+            To store the transactions of a database in list
+        mapSupport : Dictionary
+            To maintain the information of item and their frequency
+        lno : int
+            To represent the total no of transaction
+        tree : class
+            To represents the Tree class
+        itemSetCount : int
+            To represents the total no of patterns
+        finalPatterns : dict
+            To store the complete patterns
+    Methods:
+    ---------
+        startMine()
+            Mining process will start from here
+        getPatterns()
+            Complete set of patterns will be retrieved with this function
+        save(oFile)
+            Complete set of frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of frequent patterns will be loaded in to a dataframe
+        getMemoryUSS()
+            Total amount of USS memory consumed by the mining process will be retrieved from this function
+        getMemoryRSS()
+            Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        getRuntime()
+            Total amount of runtime taken by the mining process will be retrieved from this function
+        creatingItemSets(fileName)
+            Scans the dataset and stores in a list format
+        frequentOneItem()
+            Extracts the one-length frequent patterns from database
+        updateTransactions()
+            Update the transactions by removing non-frequent items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
+        startMine()
+            Mining process will start from this function
 
-            contains(superset, subset)
-                Checks if the superset contains the subset
+    **Methods to execute code on terminal**
 
-            treeGenerations(root, netUtil, candidatePattern, curItem)
-                Generates the tree of the high utility patterns
+        Format:
+                  >>>  python3 basic.py <inputFile> <outputFile> <minSup>
+        Example:
+                  >>>  python3 basic.py sampleTDB.txt patterns.txt 3
 
-            startMine()
-                Starts the mining process
+                 .. note:: minSup  will be considered in support count or frequency
 
-            printTree(root, level)
-                Prints the SHU-tree in a readable format
+    **Importing this algorithm into a python program**
 
-            getMemoryRSS()
-                Returns the memory usage of the algorithm in resident set size
+.. code-block:: python
 
-            getMemoryUSS()
-                Returns the memory usage of the algorithm in user space
+        from PAMI.weightedUncertainFrequentPattern.basic import basic as alg
 
-            getPatterns()
-                Returns the final patterns generated in each window
+        obj = alg.basic(iFile, wFile, expSup, expWSup)
 
-            getPatternsAsDataFrame()
-                Returns the final patterns generated in each window as a pandas dataframe
+        obj.startMine()
 
-            getRuntime()
-                Returns the runtime of the algorithm
+        Patterns = obj.getPatterns()
 
-            printResults()
-                Prints the statistics of the mining process
+        print("Total number of  Patterns:", len(Patterns))
 
-            save()
-                Saves the patterns generated from each window in a file
-            
+        obj.savePatterns(oFile)
 
-        Executing the code on terminal:
-        -------------------------------
+        Df = obj.getPatternsAsDataFrame()
 
-            Format:
-            -------
-                python3 SHUGrowth.py <inputFile> <outputFile> <minUtil> <windowSize> <paneSize> <separator>
+        memUSS = obj.getMemoryUSS()
 
-            Example:
-            --------
+        print("Total Memory in USS:", memUSS)
 
-                python3 SHUGrowth.py retail.txt output.txt 107 100 1000 ',' (Here minimum utility is 107,
-                                                                            Window size is 100 and pane size is 1000
-                                                                            The separator is comma for the input file)
+        memRSS = obj.getMemoryRSS()
 
-        Credits:
-        --------
+        print("Total Memory in RSS", memRSS)
 
-            The code is written by Vipul Chhabra under the supervision of Prof. Rage Uday Kiran.
-    
-    """
+        run = obj.getRuntime()
 
-    __startTime = float()
-    __endTime = float()
-    _minUtil = str()
-    __finalPatterns = {}
+        print("Total ExecutionTime in seconds:", run)
+   """
+    _startTime = float()
+    _endTime = float()
+    _minSup = str()
+    _finalPatterns = {}
     _iFile = " "
+    _wFile = " "
     _oFile = " "
     _sep = " "
-    __memoryUSS = float()
-    __memoryRSS = float()
-    __transactions = []
-    __utilities = []
-    __utilitySum = []
-    __tree = None
-    __windowSize = 0
-    __paneSize = 0
-
-    def __init__(self, iFile, oFile, minUtil, windowSize, paneSize, sep = ","):
-        super().__init__(iFile, minUtil, windowSize, paneSize, sep)
-        self._oFile = oFile
-
-    def _createItemsets(self):
-        """
-            Storing the complete transactions of the database/input file in a transaction variable
-        """
-        self._transactions, self._utilities, self._utilitySum = [], [], []
-        if isinstance(self._iFile, _hus._pd.DataFrame):
+    _memoryUSS = float()
+    _memoryRSS = float()
+    _Database = []
+    _rank = {}
+    _expSup = float()
+    _expWSup = float()
+
+    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t'):
+        super().__init__(iFile, wFile, expSup, expWSup, sep)
+
+    def _creatingItemSets(self):
+        """
+            Scans the uncertain transactional dataset
+        """
+        self._Database = []
+        if isinstance(self._iFile, _ab._pd.DataFrame):
+            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
-                self._transactions = self._iFile['Transactions'].tolist()
-            if 'Utilities' in i:
-                self._utilities = self._iFile['Utilities'].tolist()
-            if 'UtilitySum' in i:
-                self._utilitySum = self._iFile['UtilitySum'].tolist()
+                self._Database = self._iFile['Transactions'].tolist()
+            if 'uncertain' in i:
+                uncertain = self._iFile['uncertain'].tolist()
+            for k in range(len(data)):
+                tr = []
+                for j in range(len(data[k])):
+                    product = _Item(data[k][j], uncertain[k][j])
+                    tr.append(product)
+                self._Database.append(tr)
+
+            # print(self.Database)
         if isinstance(self._iFile, str):
-            if _hus._validators.url(self._iFile):
-                data = _hus._urlopen(self._iFile)
+            if _ab._validators.url(self._iFile):
+                data = _ab._urlopen(self._iFile)
                 for line in data:
                     line = line.decode("utf-8")
-                    line = line.split("\n")[0]
-                    parts = line.split(":")
-                    items = parts[0].split(self._sep)
-                    self.__transactions.append([x for x in items if x])
-                    utilities = parts[2].split(self._sep)
-                    utilities = [float(x) for x in utilities]
-                    self.__utilities.append(utilities)
-                    self.__utilitySum.append(int(parts[1]))
+                    line = line.strip()
+                    line = [i for i in line.split(':')]
+                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                    temp1 = [x for x in temp1 if x]
+                    temp2 = [x for x in temp2 if x]
+                    tr = []
+                    for i in range(len(temp1)):
+                        item = temp1[i]
+                        probability = float(temp2[i])
+                        product = _Item(item, probability)
+                        tr.append(product)
+                    self._Database.append(tr)
             else:
                 try:
-                    with open(self._iFile, 'r', encoding='utf-8') as f:
+                    with open(self._iFile, 'r') as f:
                         for line in f:
-                            line = line.split("\n")[0]
-                            parts = line.split(":")
-                            items = parts[0].split(self._sep)
-                            self._transactions.append([x for x in items if x])
-                            utilities = parts[2].split(self._sep)
-                            utilities = [float(x) for x in utilities]
-                            self._utilities.append(utilities)
-                            self._utilitySum.append(float(parts[1]))
+                            line = line.strip()
+                            line = [i for i in line.split(':')]
+                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
+                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
+                            temp1 = [x for x in temp1 if x]
+                            temp2 = [x for x in temp2 if x]
+                            tr = []
+                            for i in range(len(temp1)):
+                                item = temp1[i]
+                                probability = float(temp2[i])
+                                product = _Item(item, probability)
+                                tr.append(product)
+                            self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
-                    quit()
-
-    def minPathUtil(self, nodeIndex, stack):
-        """
-            Calculates the minimum utility of the path from the root to the ends of the tree
-
-            Parameters
-            ----------
-                nodeIndex : int
-                    index of the node in the stack
-
-                stack : list
-                    list of the nodes in the prefix branch
-
-            Returns
-            -------
-                minUtil : int
-                    minimum utility of the path from the root to the ends of the tree
-        """
-
-        minUtil = 0
-        activeBatch = [i for i, e in enumerate(stack[0].utility) if e != 0]
-
-        for batch in activeBatch:
-            if(stack[nodeIndex + 1].tail == None or stack[nodeIndex + 1].tail[batch] == False):
-                minUtil += (stack[nodeIndex].utility[batch] - stack[nodeIndex + 1].utility[batch])
-            
-        return minUtil
-        
-
-    def createPrefixBranch(self, root):
-        """
-            Creates the prefix branch of the node
-
-            Parameters
-            ----------
-                root : _Node
-                    pointer to the root node of the sub-tree
-
-            Returns
-            -------
-                stack : list
-                    list of the nodes in prefix branch
-
-                curUtil : int
-                    utility of the prefix branch
-        """
-        stack = []
-
-        while(root is not None):
-            stack.append(root)
-            root = root.parent
-
-        chosenItemset = stack[0]
-        lastUtil = sum(chosenItemset.utility)
-        curBacthes = [i for i, e in enumerate(chosenItemset.utility) if e != 0]
 
-        otherUtilites = []
-
-        for i in range(1, len(stack)-1):
-            curItemset = stack[i]
-            epu = lastUtil
-
-            for j in range(i-1, 0, -1):
-                epu -= self.minPathUtil(j, stack)
-            
-            otherUtilites.append(epu)
-
-        return stack, lastUtil, otherUtilites
-
-    def fixUtility(self, root):
+    def _scanningWeights(self):
         """
-            Fixes the utility of the nodes in the tree by merging the utility values
-
-            Parameters
-            ----------
-                root : _Node
-                    pointer to the root node of the sub-tree
-        """
-        
-        if(root is None):
-            return
-        
-        if(len(root.utility) > 1):
-            root.utility = [sum(root.utility)]
-
-        for child in root.children:
-            self.fixUtility(root.children[child])
-
-    def createConditionalTree(self, root, transactions, minUtil):
+            Scans the uncertain transactional dataset
         """
-            Creates the conditional tree for the given prefix tree
-
-            Parameters
-            ----------
-                root : _Node
-                    pointer to the root node of the prefix tree
-
-                transactions : list
-                    list of transactions in prefix tree
-
-                minUtil : int
-                    minimum utility threshold
-
-            Returns
-            -------
-                tempTree : _SHUTree
-                    conditional tree for the given prefix tree
-        """
-        
-        for transaction in transactions:
-            for item in transaction["transaction"]:
-                if(root.headerTable.table[item][0] < minUtil):
-                    itemIndex = transaction["transaction"].index(item)
-                    transaction["transaction"].remove(item)
-                    del transaction["itemwiseUtility"][itemIndex]
-
-        tempTree = _SHUTree(1, 1, True)
-        for transaction in transactions:
-            if(len(transaction["transaction"]) != 0):
-                tempTree.addTransaction(transaction["transaction"], transaction["utility"], transaction["itemwiseUtility"])
-
+        self._weights = {}
+        if isinstance(self._wFile, _ab._pd.DataFrame):
+            weights, data = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                data = self._wFile['items'].tolist()
+            if 'weights' in i:
+                weights = self._wFile['weights'].tolist()
+            for k in range(len(data)):
+                self._weights[data[k]] = int(float(weights[k]))
+
+            # print(self.Database)
+        if isinstance(self._wFile, str):
+            if _ab._validators.url(self._wFile):
+                data = _ab._urlopen(self._wFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._weights[temp[0]] = int(float(temp[1]))
+            else:
+                try:
+                    with open(self._wFile, 'r') as f:
+                        for line in f:
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._weights[temp[0]] = float(temp[1])
+                except IOError:
+                    print("File Not Found")
 
-        return tempTree
-    
-    def contains(self, superset, subset):
+    def _frequentOneItem(self):
+        """takes the self.Database and calculates the support of each item in the dataset and assign the
+            ranks to the items by decreasing support and returns the frequent items list
+                :param self.Database : it represents the one self.Database in database
+                :type self.Database : list
         """
-            Checks if the superset contains the subset
 
-            Parameters
-            ----------
-                superset : list
-                    list of items in the superset
-
-                subset : list
-                    list of items in the subset
-
-            Returns
-            -------
-                bool
-                    True if superset contains subset, False otherwise
-        """
-     
-        return reduce(and_, [i in superset for i in subset])
+        mapSupport = {}
+        for i in self._Database:
+            for j in i:
+                if j.item not in mapSupport:
+                    if self._weights.get(j.item) is not None:
+                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
+                else:
+                    mapSupport[j.item][0] += j.probability
+        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
+        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
+        return mapSupport, plist
+
+    @staticmethod
+    def _buildTree(data, info):
+        """it takes the self.Database and support of each item and construct the main tree with setting root
+            node as null
+                :param data : it represents the one self.Database in database
+                :type data : list
+                :param info : it represents the support of each item
+                :type info : dictionary
+        """
+
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(data)):
+            rootNode.addTransaction(data[i])
+        return rootNode
+
+    def _updateTransactions(self, dict1):
+        """remove the items which are not frequent from self.Database and updates the self.Database with rank of items
+            :param dict1 : frequent items with support
+            :type dict1 : dictionary
+        """
+
+        list1 = []
+        for tr in self._Database:
+            list2 = []
+            for i in range(0, len(tr)):
+                if tr[i].item in dict1:
+                    list2.append(tr[i])
+            if len(list2) >= 2:
+                basket = list2
+                basket.sort(key=lambda val: self.rank[val.item])
+                list2 = basket
+                list1.append(list2)
+        return list1
+
+    @staticmethod
+    def _check(i, x):
+        """To check the presence of item or pattern in transaction
+                :param x: it represents the pattern
+                :type x : list
+                :param i : represents the uncertain self.Database
+                :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
+
+    def _convert(self, value):
+        """
+        To convert the type of user specified minSup value
+            :param value: user specified minSup value
+            :return: converted type minSup value
+        """
+        if type(value) is int:
+            value = int(value)
+        if type(value) is float:
+            value = (len(self._Database) * value)
+        if type(value) is str:
+            if '.' in value:
+                value = (len(self._Database) * value)
+            else:
+                value = int(value)
+        return value
 
-    def treeGenerations(self, root, netUtil, candidatePattern, curItem = []):
+    def _removeFalsePositives(self):
         """
-            Generates the tree of the high utility patterns
-
-            Parameters
-            ----------
-                root : _Node
-                    pointer to the root of the tree
-                netUtil : int
-                    Net utility of the transaction
-                candidatePattern : list
-                    Candidate patterns generated with utility
-                curItem : list
-                    List of items in the current itemsets
+            To remove the false positive patterns generated in frequent patterns
+            :return: patterns with accurate probability
         """
-
-        if(root is None):
-            return
-
-
-        for item in reversed(root.headerTable.orderedItems):
-            if(root.headerTable.table[item][0] >= netUtil):
-                prefixBranches = []
-
-                tempNode = root.headerTable.table[item][1]
-
-                while tempNode is not None:
-                    curPrefixBranch, lastUtil, otherUtilites = self.createPrefixBranch(tempNode)
-                    prefixBranches.append([curPrefixBranch, lastUtil, otherUtilites])
-                    tempNode = tempNode.next
-                
-                prefixTree = _SHUTree(1, 1, True)
-                completeTransactions = []
-
-                for branch in prefixBranches:
-                    transaction = []
-                    utilities = []
-                    for idx in range(len(branch[2])-1, -1, -1):
-                        transaction.append(branch[0][(idx + 1)].itemName)
-                        utilities.append(branch[2][idx])
-
-                    prefixTree.addTransaction(transaction, branch[1], utilities)
-
-                    completeTransactions.append({"transaction" : transaction, "utility" : branch[1], "itemwiseUtility" : utilities})
-
-                conditionalTree = self.createConditionalTree(prefixTree, completeTransactions, netUtil)
-
-                newItemset = curItem.copy()
-                newItemset.append(item)
-
-                if(len(newItemset) not in candidatePattern):
-                    candidatePattern[len(newItemset)] = [newItemset]
-
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
                 else:
-                    candidatePattern[len(newItemset)].append(newItemset)
-
-                if(len(conditionalTree.headerTable.table) != 0):
-                    self.treeGenerations(conditionalTree, netUtil, candidatePattern, newItemset)
-
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            weight = 0
+            for i in x:
+                weight += self._weights[i]
+            weight = weight / len(x)
+            if weight * y >= self._expWSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
 
     def startMine(self):
+        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
+            by counting the original support of a patterns
         """
-            This function will start the mining process
-        """
-        global _minUtil
-        self.__startTime = _hus._time.time()
-        if self._iFile is None:
-            raise Exception("Please enter the file path or file name:")
-        if self._minUtil is None:
-            raise Exception("Please enter the Minimum Support")
-        if self._windowSize is None:
-            raise Exception("Please enter the Window Size")
-        if self._paneSize is None:
-            raise Exception("Please enter the Pane Size")
-        self.__windowSize = int(self._windowSize)
-        self.__paneSize = int(self._paneSize)
-        
-        self._createItemsets()
-        self._minUtil = float(self._minUtil)
-        self.__tree = _SHUTree(self.__windowSize, self.__paneSize)
-        
-        transactionwiseUtility = []
-
-        for i in range(len(self._transactions)):
-            curTrans = {}
-            for j in range(len(self._transactions[i])):
-                curTrans[self._transactions[i][j]] = self._utilities[i][j]
-            transactionwiseUtility.append(curTrans)
-
-        for i in range(0, self.__windowSize):
-            self.__tree.batchIndex = i
-            for j in range(0, self.__paneSize):
-                self.__tree.addTransaction(self._transactions[i * self.__paneSize + j], self._utilitySum[i * self.__paneSize + j], self._utilities[i * self.__paneSize + j])
-
-        startIndex = 0
-        endIndex = self.__windowSize * self.__paneSize
-
-        while(endIndex <= len(self._transactions)):
-            
-            filteredItemsets = {}
-            
-            self.treeGenerations(self.__tree, self._minUtil, filteredItemsets)
-
-            results = []
-
-            for itemSetLen in filteredItemsets:
-                for itemSet in filteredItemsets[itemSetLen]:
-                    itemSetUtility = 0
-                    for transId in range(startIndex, endIndex):
-                        if(self.contains(list(transactionwiseUtility[transId].keys()), itemSet)):
-                            for item in itemSet:
-                                itemSetUtility += transactionwiseUtility[transId][item]
-                        
-                    if(itemSetUtility >= self._minUtil):
-                        results.append([itemSet, itemSetUtility])
-
-            self.__finalPatterns[(startIndex, endIndex)] = results
-
-            if(endIndex >= len(self._transactions)):
-                break
-
-            self.__tree.removeBatch()
-
-            for i in range(0, self.__paneSize):
-                self.__tree.addTransaction(self._transactions[endIndex + i], self._utilitySum[endIndex + i], self._utilities[endIndex + i])
-
-            startIndex += self.__paneSize
-            endIndex += self.__paneSize
-
-        self.__endTime = _hus._time.time()
-        self.__memoryUSS = float()
-        self.__memoryRSS = float()
-        process = _hus._psutil.Process(_hus._os.getpid())
-        self.__memoryUSS = process.memory_full_info().uss
-        self.__memoryRSS = process.memory_info().rss
-
-    def printTree(self, root, level = 0):
-        """
-            Prints the tree in a readable format.
-
-            :param root: CPSTreeNode object for the root of the tree
-            :param level: Current level of the root node
-        """
-
-        print('  ' * level, level, root.itemName, root.utility, root.parent.itemName if root.parent else None )
-        
-        if(root.tail is not None):
-            print('  ' * (level + 1), level + 1, root.tail)
-
-        for child in root.children.values():
-            self.printTree(child, level + 1)
-
-    def getMemoryRSS(self):
-        """
-            Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
-            :return: returning RSS memory consumed by the mining process
-
-            :rtype: float
-        """
-        return self.__memoryRSS
+        global _expSup, _expWSup, _weights, _finalPatterns
+        self._startTime = _ab._time.time()
+        self._Database, self._weights = [], {}
+        self._creatingItemSets()
+        self._scanningWeights()
+        _weights = self._weights
+        self._expSup = float(self._expSup)
+        self._expWSup = float(self._expWSup)
+        _expSup = self._expSup
+        _expWSup = self._expWSup
+        self._finalPatterns = {}
+        mapSupport, plist = self._frequentOneItem()
+        self.Database1 = self._updateTransactions(mapSupport)
+        info = {k: v for k, v in mapSupport.items()}
+        Tree1 = self._buildTree(self.Database1, info)
+        Tree1.generatePatterns([])
+        self._removeFalsePositives()
+        print("Weighted Frequent patterns were generated  successfully using basic algorithm")
+        self._endTime = _ab._time.time()
+        process = _ab._psutil.Process(_ab._os.getpid())
+        self._memoryUSS = float()
+        self.memoryRSS = float()
+        self._memoryUSS = process.memory_full_info().uss
+        self.memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
+        """Total amount of USS memory consumed by the mining process will be retrieved from this function
+        :return: returning USS memory consumed by the mining process
+        :rtype: float
         """
-            Total amount of USS memory consumed by the mining process will be retrieved from this function
 
-            :return: returning USS memory consumed by the mining process
+        return self._memoryUSS
 
-            :rtype: float
-        """
-        return self.__memoryUSS
-
-    def getPatterns(self):
+    def getMemoryRSS(self):
+        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        :return: returning RSS memory consumed by the mining process
+        :rtype: float
         """
-            Returns the frequent patterns generated by the mining process over the complete datastream.
 
-            :return: returning frequent patterns generated by the mining process
+        return self.memoryRSS
 
-            :rtype: dict
-        """
-        return self.__finalPatterns
-
-    def getPatternsAsDataFrame(self):
+    def getRuntime(self):
+        """Calculating the total amount of runtime taken by the mining process
+        :return: returning total amount of runtime taken by the mining process
+        :rtype: float
         """
-            Stores the final patterns generated by the mining process in a dataframe.
 
-            :return: returning dataframe containing the final patterns generated by the mining process
+        return self._endTime - self._startTime
 
-            :rtype: pandas.DataFrame
+    def getPatternsAsDataFrame(self):
+        """Storing final frequent patterns in a dataframe
+        :return: returning frequent patterns in a dataframe
+        :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for x, y in self.__finalPatterns.items():
-            for pattern in y:
-                patternString = ' '.join(pattern[0])
-                data.append([x[0], x[1], patternString, pattern[1]])
-        dataframe = pd.DataFrame(data, columns=['Window Start Index', 'Window End Index', 'Pattern', 'Utility'])
+        for a, b in self._finalPatterns.items():
+            s = str()
+            for i in a:
+                s = s + i + " "
+            data.append([s, b])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def getRuntime(self):
-        """
-            Total amount of time taken by the mining process will be retrieved from this function
+    def save(self, outFile):
+        """Complete set of frequent patterns will be loaded in to a output file
+        :param outFile: name of the output file
+        :type outFile: file
+        """
+        self.oFile = outFile
+        writer = open(self.oFile, 'w+')
+        for x, y in self._finalPatterns.items():
+            s = str()
+            for i in x:
+                s = s + i + "\t"
+            s1 = s.strip() + ":" + str(y)
+            writer.write("%s \n" % s1)
 
-            :return: returning time taken by the mining process
-
-            :rtype: float
+    def getPatterns(self):
+        """ Function to send the set of frequent patterns after completion of the mining process
+        :return: returning frequent patterns
+        :rtype: dict
         """
-
-        return self.__endTime - self.__startTime
+        return self._finalPatterns
 
     def printResults(self):
-        """
-            Prints the stats of the mining process
-
-        """
-        print("Total number of Windows Processed:", len(self.getPatterns()))
+        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:", self.getRuntime())
-
-
-    def save(self):
-        """
-        Complete set of frequent patterns will be loaded in to a output file
-        """
-        print("Output file name", self._oFile)
-        writer = open(self._oFile, 'w+')
-        for x, y in self.__finalPatterns.items():
-            writer.write("Window Start Index : %s , End Index : %s \n" % (x[0], x[1]))
-            for pattern in y:
-                patternString = '\t'.join(pattern[0])
-                patternString += '\t' + ":" + '\t' + str(pattern[1])
-                writer.write("%s \n" % patternString)
+        print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_hus._sys.argv) == 6 or len(_hus._sys.argv) == 7:
-        if len(_hus._sys.argv) == 7:
-            _ap = SHUGrowth(_hus._sys.argv[1], _hus._sys.argv[2], _hus._sys.argv[3], _hus._sys.argv[4], _hus._sys.argv[5], _hus._sys.argv[6])
-        if len(_hus._sys.argv) == 6:
-            _ap = SHUGrowth(_hus._sys.argv[1], _hus._sys.argv[2], _hus._sys.argv[3], _hus._sys.argv[4], _hus._sys.argv[5])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+        if len(_ab._sys.argv) == 6:
+            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
-        print("Total number of Windows Processes:", len( _ap.getPatterns()))
-        _ap.getPatternsAsDataFrame().to_csv("result.csv", index = False, sep='\t')
-        _ap.save()
+        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+        _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        for k in [120, 140, 160, 180, 200]:
+            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
+                        k, 500, '\t')
+            _ap.startMine()
+            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
+            print("Total Memory in USS:", _ap.getMemoryUSS())
+            print("Total Memory in RSS", _ap.getMemoryRSS())
+            print("Total ExecutionTime in ms:", _ap.getRuntime())
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/streams/highUtility/abstract.py` & `pami-2023.8.1/PAMI/highUtilityPatternsInStreams/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+#     from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
 #
-#     obj = alg.TUFP(iFile, minSup)
+#     obj = alg.UVEclat(iFile, minSup)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -24,14 +24,15 @@
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -43,51 +44,50 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-
+import operator as _operator
 from PAMI.uncertainFrequentPattern.basic import abstract as _ab
 
+
 _minSup = float()
 _finalPatterns = {}
 
 
 class _Item:
     """
     A class used to represent the item with probability in transaction of dataset
-
     ...
-
     Attributes:
     __________
         item : int or word
             Represents the name of the item
         probability : float
             Represent the existential probability(likelihood presence) of an item
     """
 
     def __init__(self, item, probability):
         self.item = item
         self.probability = probability
 
 
-class TUFP(_ab._frequentPatterns):
+class UVEclat(_ab._frequentPatterns):
     """
     Description:
     -------------
-        It is one of the fundamental algorithm to discover top-k frequent patterns in a uncertain transactional database
-        using CUP-Lists.
-
+        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
+        using PUF-Tree.
     Reference:
     ----------
-        Tuong Le, Bay Vo, Van-Nam Huynh, Ngoc Thanh Nguyen, Sung Wook Baik 5, "Mining top-k frequent patterns from uncertain databases",
-        Springer Science+Business Media, LLC, part of Springer Nature 2020, https://doi.org/10.1007/s10489-019-01622-1
+    Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
+    SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
+    https://doi.org/10.1145/1982185.1982399
 
     Attributes:
     ------------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
@@ -135,40 +135,33 @@
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets(fileName)
             Scans the dataset and stores in a list format
         frequentOneItem()
             Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
 
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>> python3 TUFP.py <inputFile> <outputFile> <minSup>
+                      >>> python3 uveclat.py <inputFile> <outputFile> <minSup>
             Example:
-                      >>>  python3 TUFP.py sampleTDB.txt patterns.txt 0.6
+                      >>>  python3 uveclat.py sampleTDB.txt patterns.txt 3
 
             .. note:: minSup  will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import TUFP as alg
+            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+
+            obj = alg.UVEclat(iFile, minSup)
 
-            obj = alg.TUFP(iFile, minSup)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -186,31 +179,29 @@
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
-             The complete program was written by   P.Likhitha   under the supervision of Professor Rage Uday Kiran.
+         The complete program was written by   P.Likhitha    under the supervision of Professor Rage Uday Kiran.
 
     """
-
     _startTime = float()
     _endTime = float()
     _minSup = str()
     _finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _cupList = {}
-    _topk = {}
-    _minimum = 9999
+    _tidList = {}
+    _rank = {}
 
     def _creatingItemSets(self):
         """
             Scans the dataset
         """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
@@ -264,262 +255,269 @@
                             self._Database.append(tr)
                 except IOError:
                     print("File Not Found")
 
     def _frequentOneItem(self):
         """takes the self.Database and calculates the support of each item in the dataset and assign the
             ranks to the items by decreasing support and returns the frequent items list
-
-                :param self.Database : it represents the one self.Database in database
-
-                :type self.Database : list
         """
 
         mapSupport = {}
         k = 0
         for i in self._Database:
             k += 1
             for j in i:
                 if j.item not in mapSupport:
-                    mapSupport[j.item] = j.probability
-                    self._cupList[j.item] = {k:j.probability}
+                    mapSupport[str(j.item)] = j.probability
+                    self._tidList[str(j.item)] = {k: j.probability}
                 else:
-                    mapSupport[j.item] += j.probability
-                    self._cupList[j.item].update({k: j.probability})
-        plist = [k for k,v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        k = 0
-        for x, in plist:
-            k +=1
-            if k >= self._minSup:
-                break
-            self._finalPatterns[x] = mapSupport[x]
-        self._minimum = min(list(self._finalPatterns.values()))
-        return plist
+                    mapSupport[str(j.item)] += j.probability
+                    self._tidList[str(j.item)].update({k: j.probability})
+        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
+        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
+        return list(plist.keys())
+
+    @staticmethod
+    def _check(i, x):
+        """To check the presence of item or pattern in transaction
+                :param x: it represents the pattern
+                :type x : list
+                :param i : represents the uncertain self.Database
+                :type i : list
+        """
+
+        # This method taken a transaction as input and returns the tree
+        for m in x:
+            k = 0
+            for n in i:
+                if m == n.item:
+                    k += 1
+            if k == 0:
+                return 0
+        return 1
 
     @staticmethod
     def _convert(value):
         """
         To convert the type of user specified minSup value
-
             :param value: user specified minSup value
-
             :return: converted type minSup value
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = float(value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
             else:
                 value = int(value)
         return value
 
+    def _removeFalsePositives(self):
+        """
+            To remove the false positive patterns generated in frequent patterns
+            :return: patterns with accurate probability
+        """
+        global _finalPatterns
+        periods = {}
+        for i in self._Database:
+            for x, y in _finalPatterns.items():
+                if len(x) == 1:
+                    periods[x] = y
+                else:
+                    s = 1
+                    check = self._check(i, x)
+                    if check == 1:
+                        for j in i:
+                            if j.item in x:
+                                s *= j.probability
+                        if x in periods:
+                            periods[x] += s
+                        else:
+                            periods[x] = s
+        for x, y in periods.items():
+            if y >= self._minSup:
+                sample = str()
+                for i in x:
+                    sample = sample + i + "\t"
+                self._finalPatterns[sample] = y
+
+    @staticmethod
+    def _Intersection(tidSetx, tidSetY):
+        tids = []
+        support = []
+        tidDict = {}
+        for x, y in tidSetx.items():
+            for x1, y1 in tidSetY.items():
+                if x == x1:
+                    tids.append(x)
+                    support.append(y * y1)
+                    tidDict.update({x: y * y1})
+        return tidDict
+
+    def _calculateExpSup(self, tidList):
+        return sum(tidList.values())
+
     def _save(self, prefix, suffix, tidSetI):
         """Saves the patterns that satisfy the periodic frequent property.
-
             :param prefix: the prefix of a pattern
             :type prefix: list
             :param suffix: the suffix of a patterns
             :type suffix: list
             :param tidSetI: the timestamp of a patterns
             :type tidSetI: dict
         """
 
+        global _finalPatterns
         if prefix is None:
             prefix = suffix
         else:
             prefix = prefix + suffix
-        val = sum(tidSetI.values())
-        #print(prefix, val)
-        if len(self._finalPatterns) <= self._minSup:
-            sample = str()
-            for i in prefix:
-                sample = sample + i + " "
-            self._finalPatterns[sample] = val
-        if len(self._finalPatterns) == self._minSup:
-            if val > self._minimum:
-                sample = str()
-                for i in prefix:
-                    sample = sample + i + " "
-                index = list(self._finalPatterns.keys())[list(self._finalPatterns.values()).index(self._minimum)]
-                del self._finalPatterns[index]
-                self._finalPatterns[sample] = val
-                self._minimum = min(list(self._finalPatterns.values()))
-        #print(self.finalPatterns, self.minimum, self.minSup)
-
+        val = self._calculateExpSup(tidSetI)
+        _finalPatterns[tuple(prefix)] = val
 
     def _Generation(self, prefix, itemSets, tidSets):
         """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-
             :param prefix:  main equivalence prefix
             :type prefix: periodic-frequent item or pattern
             :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
                             and frequent with their timestamps
             :type itemSets: list
             :param tidSets: timestamps of the items in the argument itemSets
             :type tidSets: list
-
-
                     """
         if len(itemSets) == 1:
             i = itemSets[0]
             tidI = tidSets[0]
             self._save(prefix, [i], tidI)
             return
-        for i in range(0, len(itemSets)):
+        for i in range(len(itemSets)):
             itemI = itemSets[i]
             if itemI is None:
                 continue
             tidSetI = tidSets[i]
             classItemSets = []
             classTidSets = []
             itemSetX = [itemI]
-            for j in range(i+1, len(itemSets)):
+            for j in range(i + 1, len(itemSets)):
                 itemJ = itemSets[j]
                 tidSetJ = tidSets[j]
-                y = {key: tidSetJ[key] * tidSetI.get(key, 0) for key in tidSetJ.keys()}
-                sum2 = sum(list(y.values()))
-                #print(prefix, itemJ, y, sum2)
-                #if sum2 >= self.minimum:
-                self._save(prefix, [itemJ], y)
-                classItemSets.append(itemJ)
-                classTidSets.append(y)
-            #print(itemI, tidSetI, classItemSets)
+                y = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y) >= self._minSup:
+                    classItemSets.append(itemJ)
+                    classTidSets.append(y)
             newPrefix = list(set(itemSetX)) + prefix
             self._Generation(newPrefix, classItemSets, classTidSets)
-            #self.save(prefix, list(set(itemSetX)), tidSetI)
+            self._save(prefix, list(set(itemSetX)), tidSetI)
 
     def startMine(self):
         """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
             by counting the original support of a patterns
-
-
         """
         global _minSup
         self._startTime = _ab._time.time()
         self._creatingItemSets()
         self._minSup = self._convert(self._minSup)
         _minSup = self._minSup
         plist = self._frequentOneItem()
         for i in range(len(plist)):
             itemI = plist[i]
-            tidSetI = self._cupList[itemI]
+            tidSetI = self._tidList[itemI]
             itemSetX = [itemI]
             itemSets = []
             tidSets = []
             for j in range(i+1, len(plist)):
                 itemJ = plist[j]
-                tidSetJ = self._cupList[itemJ]
-                y1 = {key: tidSetJ[key] * tidSetI.get(key, 0)  for key in tidSetJ.keys()}
-                self._save(itemSetX, [itemJ], y1)
-                itemSets.append(itemJ)
-                tidSets.append(y1)
+                tidSetJ = self._tidList[itemJ]
+                y1 = self._Intersection(tidSetI, tidSetJ)
+                if self._calculateExpSup(y1) >= self._minSup:
+                    itemSets.append(itemJ)
+                    tidSets.append(y1)
             self._Generation(itemSetX, itemSets, tidSets)
-        print("Top-K Frequent patterns were generated from uncertain databases successfully using TUFP algorithm")
+            self._save(None, itemSetX, tidSetI)
+        self._removeFalsePositives()
+        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
         self._endTime = _ab._time.time()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryUSS = float()
         self._memoryRSS = float()
+        self._memoryUSS = float()
         self._memoryUSS = process.memory_full_info().uss
         self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
-
         :return: returning USS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
-
         :return: returning RSS memory consumed by the mining process
-
         :rtype: float
         """
 
         return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
-
-
         :return: returning total amount of runtime taken by the mining process
-
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
-
         :return: returning frequent patterns in a dataframe
-
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            data.append([a, b])
+            data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def save(self, outFile):
+    def save(self, oFile):
         """Complete set of frequent patterns will be loaded in to a output file
-
-        :param outFile: name of the output file
-
-        :type outFile: file
+        :param oFile: name of the output file
+        :type oFile: file
         """
-        self.oFile = outFile
+        self.oFile = oFile
         writer = open(self.oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s1 = x + ":" + str(y)
+            s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
-
         :return: returning frequent patterns
-
         :rtype: dict
         """
         return self._finalPatterns
 
+    def printResults(self):
+        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
+        print("Total Memory in USS:", self.getMemoryUSS())
+        print("Total Memory in RSS", self.getMemoryRSS())
+        print("Total ExecutionTime in ms:",  self.getRuntime())
+
 
 if __name__ == "__main__":
     _ap = str()
     if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
         if len(_ab._sys.argv) == 5:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
         if len(_ab._sys.argv) == 4:
-            _ap = TUFP(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
         _ap.startMine()
-        _Patterns = _ap.getPatterns()
-        print("Total number of Patterns:", len(_Patterns))
+        print("Total number of Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
-        _memUSS = _ap.getMemoryUSS()
-        print("Total Memory in USS:", _memUSS)
-        _memRSS = _ap.getMemoryRSS()
-        print("Total Memory in RSS", _memRSS)
-        _run = _ap.getRuntime()
-        print("Total ExecutionTime in ms:", _run)
+        print("Total Memory in USS:", _ap.getMemoryUSS())
+        print("Total Memory in RSS", _ap.getMemoryRSS())
+        print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        '''ap = TUFP("/home/apiiit-rkv/Desktop/uncertain/tubeSample", 10, ' ')
-        ap.startMine()
-        Patterns = ap.getPatterns()
-        print("Total number of Patterns:", len(Patterns))
-        ap.save("patterns.txt")
-        memUSS = ap.getMemoryUSS()
-        print("Total Memory in USS:", memUSS)
-        memRSS = ap.getMemoryRSS()
-        print("Total Memory in RSS", memRSS)
-        run = ap.getRuntime()
-        print("Total ExecutionTime in ms:", run)'''
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.uncertainFrequentPattern.basic import UFGrowth as alg
+#     from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 #
-#     obj = alg.UFGrowth(iFile, minSup)
+#     obj = alg.WFRIMiner(iFile, WS, regularity)
 #
 #     obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#     weightedFrequentRegularPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 #
 #     obj.savePatterns(oFile)
 #
-#     Df = obj.getPatternsAsDataFrame()
+#     Df = obj.getPatternInDataFrame()
 #
-#     memUSS = obj.getmemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
+
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -43,629 +44,722 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.uncertainFrequentPattern.basic import abstract as _ab
+from PAMI.weightedFrequentRegularPattern.basic import abstract as _fp
 
-_minSup = str()
-_ab._sys.setrecursionlimit(20000)
-_finalPatterns = {}
+_WS = str()
+_regularity = str()
+_lno = int()
+_weights = {}
+_wf = {}
+_fp._sys.setrecursionlimit(20000)
 
 
-class _Item:
-    """
-    A class used to represent the item with probability in transaction of dataset
-    ...
-    Attributes:
-    __________
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
+class _Node:
     """
+        A class used to represent the node of frequentPatternTree
 
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
-
-
-class _Node(object):
-    """
-    A class used to represent the node of frequentPatternTree
-        ...
     Attributes:
     ----------
-        item : int
+        itemId: int
             storing item of a node
-        probability : int
-            To maintain the expected support of node
-        parent : node
-            To maintain the parent of every node
-        children : list
+        counter: int
+            To maintain the support of node
+        parent: node
+            To maintain the parent of node
+        children: list
             To maintain the children of node
+
     Methods:
     -------
-        addChild(itemName)
-            storing the children to their respective parent nodes
+
+        addChild(node)
+            Updates the nodes children list and parent for the given node
+
     """
 
-    def __init__(self):
-        self.itemId = -1
-        self.counter = 0
-        self.probability = 0
-        self.child = []
+    def __init__(self, item, children):
+        """ Initializing the Node class
+
+        :param item: Storing the item of a node
+        :type item: int or None
+        :param children: To maintain the children of a node
+        :type children: dict
+        """
+
+        self.item = item
+        self.children = children
         self.parent = None
-        self.nodeLink = None
-        self.expSup = 0
+        self.timeStamps = []
+
+    def addChild(self, node):
+        """ To add the children to a node
+
+            :param node: parent node in the tree
+        """
 
-    def getChild(self, id1):
-        for i in self.child:
-            if i.itemid == id1:
-                return i
-        return None
+        self.children[node.item] = node
+        node.parent = self
 
 
-class _Tree(object):
+class _Tree:
     """
     A class used to represent the frequentPatternGrowth tree structure
-    ...
+
     Attributes:
     ----------
         root : Node
-            Represents the root node of the tree
+            The first node of the tree set to Null.
         summaries : dictionary
-            storing the nodes with same item name
+            Stores the nodes itemId which shares same itemId
         info : dictionary
-            stores the support of items
+            frequency of items in the transactions
+
     Methods:
     -------
-        addTransaction(transaction)
-            creating transaction as a branch in frequentPatternTree
-        addConditionalPattern(prefixPaths, supportOfItems)
-            construct the conditional tree for prefix paths
-        conditionalPatterns(Node)
-            generates the conditional patterns from tree for specific node
-        conditionalTransactions(prefixPaths,Support)
-            takes the prefixPath of a node and support at child of the path and extract the frequent items from
-            prefixPaths and generates prefixPaths with items which are frequent
-        remove(Node)
-            removes the node from tree once after generating all the patterns respective to the node
-        generatePatterns(Node)
-            starts from the root node of the tree and mines the frequent patterns
+        addTransaction(transaction, freq)
+            adding items of  transactions into the tree as nodes and freq is the count of nodes
+        getFinalConditionalPatterns(node)
+            getting the conditional patterns from fp-tree for a node
+        getConditionalPatterns(patterns, frequencies)
+            sort the patterns by removing the items with lower minSup
+        generatePatterns(prefix)
+            generating the patterns from fp-tree
     """
 
     def __init__(self):
-        self.headerList = []
-        self.mapItemNodes = {}
-        self.mapItemLastNodes = {}
-        self.root = _Node()
-
-    def fixNodeLinks(self, item, newNode):
-        if item in self.mapItemLastNodes.keys():
-            lastNode = self.mapItemLastNodes[item]
-            lastNode.nodeLink = newNode
-        self.mapItemLastNodes[item] = newNode
-        if item not in self.mapItemNodes.keys():
-            self.mapItemNodes[item] = newNode
-
-    def addTransaction(self, transaction):
-        y = 0
-        current = self.root
-        for i in transaction:
-            child = current.getChild(i.item)
-            if child is None:
-                newNode = _Node()
-                newNode.counter = 1
-                newNode.probability = i.probability
-                newNode.itemId = i.item
-                newNode.expSup = i.probability
-                newNode.parent = current
-                current.child.append(newNode)
-                self.fixNodeLinks(i.item, newNode)
-                current = newNode
-            else:
-                if child.probability == i.probability:
-                    child.counter += 1
-                    current = child
+        self.root = _Node(None, {})
+        self.summaries = {}
+        self.info = {}
+
+    def addTransaction(self, transaction, tid):
+        """     Adding a transaction into tree
+
+                :param transaction: To represent the complete database
+                :type transaction: list
+                :param tid: To represent the timestamp of a database
+                :type tid: list
+                :return: pfp-growth tree
+        """
+
+        currentNode = self.root
+        for i in range(len(transaction)):
+            if transaction[i] not in currentNode.children:
+                newNode = _Node(transaction[i], {})
+                currentNode.addChild(newNode)
+                if transaction[i] in self.summaries:
+                    self.summaries[transaction[i]].append(newNode)
                 else:
-                    newNode = _Node()
-                    newNode.counter = 1
-                    newNode.itemId = i.item
-                    newNode.probability = i.probability
-                    newNode.expSup = i.probability
-                    newNode.parent = current
-                    current.child.append(newNode)
-                    self.fixNodeLinks(i.item, newNode)
-                    current = newNode
-        return y
-
-    def printTree(self, root):
-        if root.child is []:
-            return
-        else:
-            for i in root.child:
-                print(i.itemid, i.counter)
-                self.printTree(i)
-
-    def update(self, mapSup, u1):
-        t1 = []
-        for i in mapSup:
-            if i in u1:
-                t1.append(i)
-        return t1
-
-    def createHeaderList(self, mapSupport, min_sup):
-        t1 = []
-        for x, y in mapSupport.items():
-            if y >= min_sup:
-                t1.append(x)
-        mapSup = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.headerList = self.update(mapSup, t1)
-
-    def addPrefixPath(self, prefix, mapSupportBeta, min_sup):
-        q = 0
-        pathCount = prefix[0].counter
-        current = self.root
-        prefix.reverse()
-        for i in range(0, len(prefix) - 1):
-            pathItem = prefix[i]
-            # pathCount=mapSupportBeta.get(pathItem.itemId)
-            if mapSupportBeta.get(pathItem.itemId) >= min_sup:
-                child = current.getChild(pathItem.itemId)
-                if child is None:
-                    newNode = _Node()
-                    q += 1
-                    newNode.itemid = pathItem.itemId
-                    if newNode.expSup == 0:
-                        newNode.expSup = pathItem.expSup
-                    newNode.probability = pathItem.probability
-                    newNode.parent = current
-                    newNode.counter = pathCount
-                    current.child.append(newNode)
-                    current = newNode
-                    self.fixNodeLinks(pathItem.itemid, newNode)
+                    self.summaries[transaction[i]] = [newNode]
+                currentNode = newNode
+            else:
+                currentNode = currentNode.children[transaction[i]]
+        currentNode.timeStamps = currentNode.timeStamps + tid
+
+    def getConditionalPatterns(self, alpha, pattern):
+        """Generates all the conditional patterns of a respective node
+
+            :param alpha: To represent a Node in the tree
+            :type alpha: Node
+            :param pattern: prefix of the pattern
+            :type alpha: list
+            :return: A tuple consisting of finalPatterns, conditional pattern base and information
+        """
+        finalPatterns = []
+        finalSets = []
+        for i in self.summaries[alpha]:
+            set1 = i.timeStamps
+            set2 = []
+            while i.parent.item is not None:
+                set2.append(i.parent.item)
+                i = i.parent
+            if len(set2) > 0:
+                set2.reverse()
+                finalPatterns.append(set2)
+                finalSets.append(set1)
+        finalPatterns, finalSets, info = self.conditionalDatabases(finalPatterns, finalSets, pattern)
+        return finalPatterns, finalSets, info
+
+    @staticmethod
+    def generateTimeStamps(node):
+        """To get the timestamps of a node
+
+        :param node: A node in the tree
+        :return: Timestamps of a node
+        """
+
+        finalTimeStamps = node.timeStamps
+        return finalTimeStamps
+
+    def removeNode(self, nodeValue):
+        """ Removing the node from tree
+
+            :param nodeValue: To represent a node in the tree
+            :type nodeValue: node
+            :return: Tree with their nodes updated with timestamps
+        """
+
+        for i in self.summaries[nodeValue]:
+            i.parent.timeStamps = i.parent.timeStamps + i.timeStamps
+            del i.parent.children[nodeValue]
+
+    def getTimeStamps(self, alpha):
+        """ To get all the timestamps of the nodes which share same item name
+
+            :param alpha: Node in a tree
+            :return: Timestamps of a  node
+        """
+        temporary = []
+        for i in self.summaries[alpha]:
+            temporary += i.timeStamps
+        return temporary
+
+    @staticmethod
+    def getSupportAndPeriod(timeStamps, pattern):
+        """To calculate the periodicity and support
+
+        :param timeStamps: Timestamps of an item set
+        :type timeStamps: list
+        :param pattern: pattern to evaluate the weighted frequent regular or not
+        :type pattern: list
+        :return: support, periodicity
+        """
+
+        global _WS, _regularity, _lno, _weights
+        timeStamps.sort()
+        cur = 0
+        per = list()
+        sup = 0
+        for j in range(len(timeStamps)):
+            per.append(timeStamps[j] - cur)
+            cur = timeStamps[j]
+            sup += 1
+        per.append(_lno - cur)
+        l = int()
+        for i in pattern:
+            l = l + _weights[i]
+        wf = (l / (len(pattern))) * sup
+        if len(per) == 0:
+            return [0, 0]
+        return [sup, max(per), wf]
+
+    def conditionalDatabases(self, conditionalPatterns, conditionalTimeStamps, pattern):
+        """ It generates the conditional patterns with periodic-frequent items
+
+            :param conditionalPatterns: conditionalPatterns generated from conditionPattern method of a respective node
+            :type conditionalPatterns: list
+            :param conditionalTimeStamps: Represents the timestamps of a conditional patterns of a node
+            :type conditionalTimeStamps: list
+            :param pattern: prefix of the pattern
+            :type pattern: list
+            :returns: Returns conditional transactions by removing non-periodic and non-frequent items
+        """
+
+        global _WS, _regularity
+        pat = []
+        timeStamps = []
+        data1 = {}
+        for i in range(len(conditionalPatterns)):
+            for j in conditionalPatterns[i]:
+                if j in data1:
+                    data1[j] = data1[j] + conditionalTimeStamps[i]
                 else:
-                    if child.probability == prefix[i].probability:
-                        child.counter += pathCount
-                        child.expSup = child.expSup * pathItem.expSup
-                        current = child
-                    else:
-                        newNode = _Node()
-                        q += 1
-                        newNode.itemId = pathItem.itemId
-                        newNode.probability = pathItem.probability
-                        if newNode.expSup == 0:
-                            newNode.expSup = pathItem.expSup
-                        newNode.parent = current
-                        newNode.counter = pathCount
-                        current.child.append(newNode)
-                        current = newNode
-                        self.fixNodeLinks(pathItem.itemid, newNode)
-        return q
+                    data1[j] = conditionalTimeStamps[i]
+        updatedDictionary = {}
+        for m in data1:
+            updatedDictionary[m] = self.getSupportAndPeriod(data1[m], pattern + [m])
+        updatedDictionary = {k: v for k, v in updatedDictionary.items() if v[0] >= _WS and v[1] <= _regularity}
+        count = 0
+        for p in conditionalPatterns:
+            p1 = [v for v in p if v in updatedDictionary]
+            trans = sorted(p1, key=lambda x: (updatedDictionary.get(x)[0], -x), reverse=True)
+            if len(trans) > 0:
+                pat.append(trans)
+                timeStamps.append(conditionalTimeStamps[count])
+            count += 1
+        return pat, timeStamps, updatedDictionary
+
+    def generatePatterns(self, prefix):
+        """ Generates the patterns
+
+            :param prefix: Forms the combination of items
+            :type prefix: list
+            :returns: yields patterns with their support and periodicity
+        """
+        global _WS
+        for i in sorted(self.summaries, key=lambda x: (self.info.get(x)[0], -x)):
+            pattern = prefix[:]
+            pattern.append(i)
+            if self.info[i][2] >= _WS:
+                yield pattern, self.info[i]
+                patterns, timeStamps, info = self.getConditionalPatterns(i, pattern)
+                conditionalTree = _Tree()
+                conditionalTree.info = info.copy()
+                for pat in range(len(patterns)):
+                    conditionalTree.addTransaction(patterns[pat], timeStamps[pat])
+                if len(patterns) > 0:
+                    for q in conditionalTree.generatePatterns(pattern):
+                        yield q
+            self.removeNode(i)
 
 
-class UFGrowth(_ab._frequentPatterns):
+class WFRIMiner(_fp._weightedFrequentRegularPatterns):
     """
-    Description:
-    -------------
-        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
-        using PUF-Tree.
-    Reference:
-    -----------
-        Carson Kai-Sang Leung, Syed Khairuzzaman Tanbeer, "PUF-Tree: A Compact Tree Structure for Frequent Pattern Mining of Uncertain Data",
-        Pacific-Asia Conference on Knowledge Discovery and Data Mining(PAKDD 2013), https://link.springer.com/chapter/10.1007/978-3-642-37453-1_2
-    Attributes:
-    -----------
+       WFRIMiner is one of the fundamental algorithm to discover weighted frequent regular patterns in a transactional database.
+       It stores the database in compressed WFRI-tree decreasing the memory usage and extracts the
+       patterns from tree.It employs employs downward closure property to  reduce the search space effectively.
+
+    Reference :
+    ---------
+           K. Klangwisan and K. Amphawan, "Mining weighted-frequent-regular itemsets from transactional database,"
+           2017 9th International Conference on Knowledge and Smart Technology (KST), 2017, pp. 66-71,
+           doi: 10.1109/KST.2017.7886090.
+
+    Attributes :
+    ----------
         iFile : file
-            Name of the Input file or path of the input file
-        oFile : file
-            Name of the output file or path of the output file
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+            Input file name or path of the input file
+        WS: float or int or str
+            The user can specify WS either in count or proportion of database size.
+            If the program detects the data type of WS is integer, then it treats WS is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: WS=10 will be treated as integer, while WS=10.0 will be treated as float
+        regularity: float or int or str
+            The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
         sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+            This variable is used to distinguish items from one another in a transaction. The default separator is tab space or \t.
             However, the users can override their default separator.
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
+        oFile : file
+            Name of the output file or the path of the output file
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
+        memoryUSS : float
+            To store the total amount of USS memory consumed by the program
+        memoryRSS : float
+            To store the total amount of RSS memory consumed by the program
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            To represent the total no of transaction
+            it represents the total no of transactions
         tree : class
-            To represents the Tree class
-        itemSetCount : int
-            To represents the total no of patterns
+            it represents the Tree class
         finalPatterns : dict
-            To store the complete patterns
-    Methods:
-    --------
+            it represents to store the patterns
+
+    Methods :
+    -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
         save(oFile)
             Complete set of frequent patterns will be loaded in to a output file
         getPatternsAsDataFrame()
             Complete set of frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
+        creatingItemSets()
+            Scans the dataset or dataframes and stores in list format
         frequentOneItem()
-            Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
+            Extracts the one-frequent patterns from transactions
+
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>>  python3 PUFGrowth.py <inputFile> <outputFile> <minSup>
+                      >>> python3 WFRIMiner.py <inputFile> <outputFile> <weightSupport> <regularity>
             Example:
-                      >>>  python3 PUFGrowth.py sampleTDB.txt patterns.txt 3
+                      >>>  python3 WFRIMiner.py sampleDB.txt patterns.txt 10 5
 
-            .. note:: minSup  will be considered in support count or frequency
+                     .. note:: WS & regularity will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import UFGrowth as alg
+            from PAMI.weightedFrequentRegularpattern.basic import WFRIMiner as alg
 
-            obj = alg.UFGrowth(iFile, minSup)
+            obj = alg.WFRIMiner(iFile, WS, regularity)
 
             obj.startMine()
 
-            frequentPatterns = obj.getPatterns()
+            weightedFrequentRegularPatterns = obj.getPatterns()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+            print("Total number of Frequent Patterns:", len(weightedFrequentRegularPatterns))
 
             obj.savePatterns(oFile)
 
-            Df = obj.getPatternsAsDataFrame()
+            Df = obj.getPatternInDataFrame()
 
-            memUSS = obj.getmemoryUSS()
+            memUSS = obj.getMemoryUSS()
 
             print("Total Memory in USS:", memUSS)
 
             memRSS = obj.getMemoryRSS()
 
             print("Total Memory in RSS", memRSS)
 
             run = obj.getRuntime()
 
             print("Total ExecutionTime in seconds:", run)
 
     **Credits:**
 
-             The complete program was written by P.Likhitha under the supervision of Professor Rage Uday Kiran.
+             The complete program was written by P.Likhitha  under the supervision of Professor Rage Uday Kiran.
+
+        """
 
-    """
     _startTime = float()
     _endTime = float()
-    _minSup = str()
+    _WS = str()
+    _regularity = str()
+    _weight = {}
     _finalPatterns = {}
+    _wFile = " "
     _iFile = " "
     _oFile = " "
     _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
     _Database = []
-    _rank = {}
     _mapSupport = {}
     _lno = 0
     _tree = _Tree()
-    _itemsetBuffer = None
-    _fpNodeTempBuffer = []
-    _maxPatternLength = 1000
-    _itemsetCount = 0
-    _frequentitems = {}
-    _fpnode = 0
-    _conditionalnodes = 0
+    _rank = {}
+    _rankDup = {}
 
-    def __init__(self, iFile, minSup, sep='\t'):
-        super().__init__(iFile, minSup, sep)
+    def __init__(self, iFile, _wFile, WS, regularity, sep='\t'):
+        super().__init__(iFile, _wFile, WS, regularity, sep)
 
     def _creatingItemSets(self):
         """
-            Scans the uncertain transactional dataset
+            Storing the complete transactions of the database/input file in a database variable
+
+
         """
         self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
+        self._weight = {}
+        if isinstance(self._iFile, _fp._pd.DataFrame):
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
+
+        if isinstance(self._wFile, _fp._pd.DataFrame):
+            _items, _weights = [], []
+            if self._wFile.empty:
+                print("its empty..")
+            i = self._wFile.columns.values.tolist()
+            if 'items' in i:
+                _items = self._wFile['items'].tolist()
+            if 'weight' in i:
+                _weights = self._wFile['weight'].tolist()
+            for i in range(len(_items)):
+                self._weight[_items[i]] = _weights[i]
 
             # print(self.Database)
         if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
+            if _fp._validators.url(self._iFile):
+                data = _fp._urlopen(self._iFile)
                 for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    tr = []
-                    for i in temp:
-                        i1 = i.index('(')
-                        i2 = i.index(')')
-                        item = i[0:i1]
-                        probability = float(i[i1 + 1:i2])
-                        product = _Item(item, probability)
-                        tr.append(product)
                     self._Database.append(temp)
             else:
                 try:
-                    with open(self._iFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            tr = []
-                            for i in temp:
-                                i1 = i.index('(')
-                                i2 = i.index(')')
-                                item = i[0:i1]
-                                probability = float(i[i1 + 1:i2])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
-        """takes the self.Database and calculates the support of each item in the dataset and assign the
-            ranks to the items by decreasing support and returns the frequent items list
-                :param self.Database : it represents the one self.Database in database
-                :type self.Database : list
-        """
-
-        mapSupport = {}
-        for i in self._Database:
-            for j in i:
-                if j.item not in mapSupport:
-                    mapSupport[j.item] = j.probability
-                else:
-                    mapSupport[j.item] += j.probability
-        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
-        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
-        return mapSupport, plist
-
-    def _ufgrowth(self, tree, prefix, prefixLength, prefixSupport, mapSupport):
-        if prefixLength == self._maxPatternLength:
-            return
-        singlePath = True
-        position = 0
-        s = 0
-        if len(tree.root.child) > 1:
-            singlePath = False
-        else:
-            currentNode = tree.root.child[0]
-            while True:
-                if len(currentNode.child) > 1:
-                    singlePath = False
-                    break
-                self._fpNodeTempBuffer.insert(position, currentNode)
-                s = currentNode.counter
-                position += 1
-                if len(currentNode.child) == 0:
-                    break
-                currentNode = currentNode.child[0]
-        if singlePath is True:
-            self._saveAllcombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
-        else:
-            for i in reversed(tree.headerList):
-                item = i
-                betaSupport = mapSupport[item]
-                prefix.insert(prefixLength, item)
-                # print prefix,betaSupport
-                self._saveItemset(prefix, prefixLength + 1, betaSupport)
-                if prefixLength + 1 < self._maxPatternLength:
-                    prefixPaths = []
-                    path = tree.mapItemNodes.get(item)
-                    mapSupportBeta = {}
-                    while path is not None:
-                        if path.parent.itemid != -1:
-                            prefixPath = []
-                            prefixPath.append(path)
-                            pathCount = path.counter
-                            parent1 = path.parent
-                            while parent1.itemid != -1:
-                                prefixPath.append(parent1)
-                                s = (pathCount * path.expSup) * parent1.probability
-                                if mapSupportBeta.get(parent1.itemid) == None:
-                                    mapSupportBeta[parent1.itemid] = s
-                                else:
-                                    mapSupportBeta[parent1.itemid] = mapSupportBeta[parent1.itemid] + s
-                                parent1 = parent1.parent
-                            prefixPaths.append(prefixPath)
-                        path = path.nodeLink
-                    treeBeta = _Tree()
-                    for i in prefixPaths:
-                        q = treeBeta.addPrefixPath(i, mapSupportBeta, self._minSup)
-                        self._conditionalnodes += q
-                    if len(treeBeta.root.child) > 0:
-                        treeBeta.createHeaderList(mapSupportBeta, self._minSup)
-                        # print(treeBeta.headerList)
-                        self._ufgrowth(treeBeta, prefix, prefixLength + 1, betaSupport, mapSupportBeta)
-
-    def _saveItemset(self, prefix, prefixLength, support):
-        l = []
-        for i in range(prefixLength):
-            l.append(prefix[i])
-        self._itemsetCount += 1
-        l.sort()
-        s = '\t'.join(l)
-        self._finalPatterns[s] = support
-
-    def _saveAllcombinations(self, TempBuffer, s, position, prefix, prefixLength):
-        # support=0
-        max1 = 1 << position
-        for i in range(1, max1):
-            newprefixLength = prefixLength
-            for j in range(position):
-                isset = i & (1 << j)
-                if isset > 0:
-                    prefix.insert(newprefixLength, TempBuffer[j].itemid)
-                    newprefixLength += 1
-                    support = TempBuffer[j].counter
-            self._saveItemset(prefix, newprefixLength, s)
+        if isinstance(self._wFile, str):
+            if _fp._validators.url(self._wFile):
+                data = _fp._urlopen(self._wFile)
+                for line in data:
+                    line.strip()
+                    line = line.decode("utf-8")
+                    temp = [i.rstrip() for i in line.split(self._sep)]
+                    temp = [x for x in temp if x]
+                    self._weight[temp[0]] = float(temp[1])
+            else:
+                try:
+                    with open(self._wFile, 'r', encoding='utf-8') as f:
+                        for line in f:
+                            line.strip()
+                            temp = [i.rstrip() for i in line.split(self._sep)]
+                            temp = [x for x in temp if x]
+                            self._weight[temp[0]] = float(temp[1])
+                except IOError:
+                    print("File Not Found")
+                    quit()
 
     def _convert(self, value):
         """
-        To convert the type of user specified minSup value
-            :param value: user specified minSup value
-            :return: converted type minSup value
+        to convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
+                value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
+    def _frequentOneItem(self):
+        """
+        Generating One frequent items sets
+
+        """
+        global _lno, _wf, _weights
+        self._mapSupport = {}
+        _owf = {}
+        for tr in self._Database:
+            for i in range(1, len(tr)):
+                if tr[i] not in self._mapSupport:
+                    self._mapSupport[tr[i]] = [int(tr[0]), int(tr[0]), 1]
+                else:
+                    self._mapSupport[tr[i]][0] = max(self._mapSupport[tr[i]][0], (int(tr[0]) - self._mapSupport[tr[i]][1]))
+                    self._mapSupport[tr[i]][1] = int(tr[0])
+                    self._mapSupport[tr[i]][2] += 1
+        for key in self._mapSupport:
+            self._mapSupport[key][0] = max(self._mapSupport[key][0], abs(len(self._Database) - self._mapSupport[key][1]))
+        _lno = len(self._Database)
+        self._mapSupport = {k: [v[2], v[0]] for k, v in self._mapSupport.items() if v[0] <= self._regularity}
+        for x, y in self._mapSupport.items():
+            if self._weight.get(x) is None:
+                self._weight[x] = 0
+        gmax = max([self._weight[values] for values in self._mapSupport.keys()])
+        for x, y in self._mapSupport.items():
+            _owf[x] = y[0] * gmax
+        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v[0] * _owf[k] >= self._WS}
+        for x, y in self._mapSupport.items():
+            temp = self._weight[x] * y[0]
+            _wf[x] = temp
+            self._mapSupport[x].append(temp)
+        genList = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse= True)]
+        self._rank = dict([(index, item) for (item, index) in enumerate(genList)])
+        for x, y in self._rank.items():
+            _weights[y] = self._weight[x]
+        return genList
+
+    def _updateTransactions(self, itemSet):
+        """
+        Updates the items in transactions with rank of items according to their support
+
+        :Example: oneLength = {'a':7, 'b': 5, 'c':'4', 'd':3}
+                    rank = {'a':0, 'b':1, 'c':2, 'd':3}
+
+        Parameters
+        ----------
+        itemSet: list of one-frequent items
+
+        -------
+
+        """
+        list1 = []
+        for tr in self._Database:
+            list2 = [int(tr[0])]
+            for i in range(1, len(tr)):
+                if tr[i] in itemSet:
+                    list2.append(self._rank[tr[i]])
+            if len(list2) >= 2:
+                basket = list2[1:]
+                basket.sort()
+                list2[1:] = basket[0:]
+                list1.append(list2)
+        return list1
+
+    @staticmethod
+    def _buildTree(transactions, info):
+        """
+        Builds the tree with updated transactions
+        Parameters:
+        ----------
+            transactions: updated transactions
+            info: support details of each item in transactions
+
+        Returns:
+        -------
+            transactions compressed in fp-tree
+
+        """
+        rootNode = _Tree()
+        rootNode.info = info.copy()
+        for i in range(len(transactions)):
+            set1 = [transactions[i][0]]
+            rootNode.addTransaction(transactions[i][1:], set1)
+        return rootNode
+
+    def _savePeriodic(self, itemSet):
+        """
+        The duplication items and their ranks
+        Parameters:
+        ----------
+            itemSet: frequent itemSet that generated
+
+        Returns:
+        -------
+            patterns with original item names.
+
+        """
+        temp = str()
+        for i in itemSet:
+            temp = temp + self._rankDup[i] + "\t"
+        return temp
+
     def startMine(self):
-        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
-            by counting the original support of a patterns
         """
-        global minSup
-        self._startTime = _ab._time.time()
+            main program to start the operation
+
+        """
+        global _WS, _regularity, _weights
+        self._startTime = _fp._time.time()
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
+        if self._WS is None:
+            raise Exception("Please enter the Minimum Support")
         self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
-        minSup = self._minSup
+        self._WS = self._convert(self._WS)
+        self._regularity = self._convert(self._regularity)
+        _WS, _regularity, _weights = self._WS, self._regularity, self._weight
+        itemSet = self._frequentOneItem()
+        updatedTransactions = self._updateTransactions(itemSet)
+        for x, y in self._rank.items():
+            self._rankDup[y] = x
+        info = {self._rank[k]: v for k, v in self._mapSupport.items()}
+        _Tree = self._buildTree(updatedTransactions, info)
+        patterns = _Tree.generatePatterns([])
         self._finalPatterns = {}
-        _mapSupport, plist = self._frequentOneItem()
-        for i in self._Database:
-            transaction = []
-            for j in i:
-                if _mapSupport.get(j.item) >= self._minSup:
-                    transaction.append(j)
-            transaction.sort(key=lambda val: _mapSupport[val.item], reverse=True)
-            o = self._tree.addTransaction(transaction)
-        self._tree.createHeaderList(_mapSupport, self._minSup)
-        if len(self._tree.headerList) > 0:
-            self._itemsetBuffer = []
-            # self.fpNodeTempBuffer=[]
-            self._ufgrowth(self._tree, self._itemsetBuffer, 0, self._lno, _mapSupport)
-        print("Frequent patterns were generated from uncertain databases successfully using UF algorithm")
-        self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
+        for k in patterns:
+            s = self._savePeriodic(k[0])
+            self._finalPatterns[str(s)] = k[1]
+        print("Weighted Frequent Regular patterns were generated successfully using WFRIM algorithm")
+        self._endTime = _fp._time.time()
+        self._memoryUSS = float()
+        self._memoryRSS = float()
+        process = _fp._psutil.Process(_fp._os.getpid())
+        self._memoryRSS = float()
         self._memoryUSS = float()
-        self.memoryRSS = float()
         self._memoryUSS = process.memory_full_info().uss
-        self.memoryRSS = process.memory_info().rss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
-        return self.memoryRSS
+        return self._memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
             data.append([a.replace('\t', ' '), b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+            dataframe = _fp._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
     def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
+
         :param outFile: name of the output file
+
         :type outFile: file
         """
-        self.oFile = outFile
-        writer = open(self.oFile, 'w+')
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of  Weighted Frequent Regular Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = UFGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
-        if len(_ab._sys.argv) == 4:
-            _ap = UFGrowth(_ab._sys.argv[1], _ab._sys.argv[3])
+    if len(_fp._sys.argv) == 6 or len(_fp._sys.argv) == 7:
+        if len(_fp._sys.argv) == 7:
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5], _fp._sys.argv[6])
+        if len(_fp._sys.argv) == 5:
+            _ap = WFRIMiner(_fp._sys.argv[1], _fp._sys.argv[3], _fp._sys.argv[4], _fp._sys.argv[5])
         _ap.startMine()
-        print("Total number of Uncertain Frequent Patterns:", len(_ap.getPatterns()))
-        _ap.save(_ab._sys.argv[2])
+        print("Total number of Weighted Frequent Regular Patterns:", len(_ap.getPatterns()))
+        _ap.save(_fp._sys.argv[2])
         print("Total Memory in USS:",  _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
-        print("Error! The number of input parameters do not match the total number of parameters provided")
+        print("Error! The number of input parameters do not match the total number of parameters provided")
```

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
+#     from PAMI.periodicFrequentPattern.basic import parallelPFPGrowth as alg
 #
-#     obj = alg.UVEclat(iFile, minSup)
+#     obj = alg.parallelPFPGrowth(iFile, minSup, maxPer, noWorkers)
 #
 #     obj.startMine()
 #
-#     frequentPatterns = obj.getPatterns()
+#     periodicFrequentPatterns = obj.getPatterns()
 #
-#     print("Total number of Frequent Patterns:", len(frequentPatterns))
+#     print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
 #     obj.savePatterns(oFile)
 #
 #     Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getmemoryUSS()
+#     memUSS = obj.getMemoryUSS()
 #
 #     print("Total Memory in USS:", memUSS)
 #
 #     memRSS = obj.getMemoryRSS()
 #
 #     print("Total Memory in RSS", memRSS)
 #
 #     run = obj.getRuntime()
 #
 #     print("Total ExecutionTime in seconds:", run)
 
-
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.
@@ -44,62 +43,309 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-import operator as _operator
-from PAMI.uncertainFrequentPattern.basic import abstract as _ab
-
+from PAMI.periodicFrequentPattern.pyspark import abstract as _ab
+from pyspark import SparkContext, SparkConf
 
+_maxPer = float()
 _minSup = float()
-_finalPatterns = {}
+_lno = int()
 
 
-class _Item:
+class Node(object):
     """
-    A class used to represent the item with probability in transaction of dataset
-    ...
-    Attributes:
-    __________
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
+        A class used to represent the node of frequentPatternTree
+
+        Attributes:
+        ----------
+            item : int or None
+                Storing item of a node
+            timeStamps : list
+                To maintain the timestamps of a database at the end of the branch
+            parent : node
+                To maintain the parent of every node
+            children : list
+                To maintain the children of a node
+            count : int
+                To maintain the count of every node
+
+        Methods:
+        -------
+            addChild(itemName)
+                Storing the children to their respective parent nodes
+            toString()
+                To print the node
     """
 
-    def __init__(self, item, probability):
+    def __init__(self, item, count, children):
+        """ Initializing the Node class
+
+        :param item: item of a node
+        :param count: count of a node
+        :param children: children of a node
+
+        """
         self.item = item
-        self.probability = probability
+        self.count = count
+        self.children = children  # dictionary of children
+        self.parent = None
+        self.tids = set()
+
+    def __repr__(self):
+        return self.toString(0)
+
+    def toString(self, level=0):
+        """ To print the node
+
+        :param level: level of a node
+
+        """
+        if self.item == None:
+            s = "Root("
+        else:
+            s = "(item=" + str(self.item)
+            s += ", count=" + str(self.count)
+            for i in self.tids:
+                s += " " + str(i)
+        tabs = "\t".join(['' for i in range(0, level + 2)])
+        for v in self.children.values():
+            s += tabs + "\n"
+            s += tabs + v.toString(level=level + 1)
+        s += ")"
+        return s
+
+    def addChild(self, node):
+        """ To add the children to a node
+
+        :param node: children of a node
+
+        """
+        self.children[node.item] = node
+        node.parent = self
+
+    def _getTransactions(self):
+        count = self.count
+        tids = self.tids
+        for child in self.children.values():
+            for t in child._getTransactions():
+                count -= t[2]
+                t[0].insert(0, child.item)
+                yield t
+        if (count > 0):
+            yield ([], tids, count)
+
+
+class PFPTree(object):
+    """
+
+    A class used to represent the periodic frequent pattern tree
+
+    Attributes:
+    ----------
+        root : node
+            To maintain the root of the tree
+        summaries : dict
+            To maintain the summary of the tree
+
+    Methods:
+    -------
+        add(basket, tid, count)
+            To add the basket to the tree
+        getTransactions()
+            To get the transactions of the tree
+        merge(tree)
+            To merge the tree
+        project(itemId)
+            To project the tree
+        satisfyPer(tids, maxPer, numTrans)
+            To satisfy the periodicity constraint
+        extract(minCount, maxPer, numTrans, isResponsible = lambda x:True)
+            To extract the periodic frequent patterns
+
+
+    """
+
+    def __init__(self):
+        self.root = Node(None, 0, {})
+        self.summaries = {}
+
+    def __repr__(self):
+        return repr(self.root)
+
+    def add(self, basket, tid, count):
+        """
+        To add the basket to the tree
+
+        :param basket: basket of a database
+        :param tid: timestamp of a database
+        :param count: count of a node
+
+        """
+        curr = self.root
+        curr.count += count
+        for i in tid:
+            curr.tids.add(i)
+
+        for i in range(0, len(basket)):
+            item = basket[i]
+            if item in self.summaries.keys():
+                summary = self.summaries.get(item)
+            else:
+                summary = Summary(0, set())
+                self.summaries[item] = summary
+            summary.count += count
+
+            if item in curr.children.keys():
+                child = curr.children.get(item)
+            else:
+                child = Node(item, 0, {})
+                curr.addChild(child)
+            summary.nodes.add(child)
+            child.count += count
+            for j in tid:
+                summary.tids.add(j)
+                if (i == len(basket) - 1):
+                    child.tids.add(j)
+            curr = child
+        return self
+
+    def getTransactions(self):
+        """
+        To get the transactions of the tree
+
+        :return: returning the transactions of the tree
 
+        """
+        return [x for x in self.root._getTransactions()]
+
+    def merge(self, tree):
+        """
+        To merge the tree
+
+        :param tree: tree of a database
+
+        """
+        for t in tree.getTransactions():
+            self.add(t[0], t[1], t[2])
+        return self
+
+    def project(self, itemId):
+        """
+        To project the tree
+
+        :param itemId: item of a node
+
+        """
+        newTree = PFPTree()
+        summaryItem = self.summaries.get(itemId)
+        if summaryItem:
+            for element in summaryItem.nodes:
+                t = []
+                curr = element.parent
+                while curr.parent:
+                    t.insert(0, curr.item)
+                    curr = curr.parent
+                newTree.add(t, element.tids, element.count)
+        return newTree
+
+    def satisfyPer(self, tids, maxPer, numTrans):
+        """
+        To satisfy the periodicity constraint
+
+        :param tids: timestamps of a database
+        :param maxPer: maximum periodicity
+        :param numTrans: number of transactions
+
+        """
+
+        tids = list(tids)
+        tids.sort()
+        if tids[0] > maxPer:
+            return 0
+        tids.append(numTrans)
+        for i in range(1, len(tids)):
+            if (tids[i] - tids[i - 1]) > maxPer:
+                return 0
+        return 1
+
+    def extract(self, minCount, maxPer, numTrans, isResponsible=lambda x: True):
+        """
+        To extract the periodic frequent patterns
+
+        :param minCount: minimum count of a node
+        :param maxPer: maximum periodicity
+        :param numTrans: number of transactions
+        :param isResponsible: responsible node of a tree
+
+        """
+        for item in sorted(self.summaries, reverse=True):
+            summary = self.summaries[item]
+            if (isResponsible(item)):
+                if (summary.count >= minCount and self.satisfyPer(summary.tids, maxPer, numTrans)):
+                    yield ([item], summary.count)
+                    for element in self.project(item).extract(minCount, maxPer, numTrans):
+                        yield ([item] + element[0], element[1])
+            for element in summary.nodes:
+                parent = element.parent
+                parent.tids |= element.tids
+
+
+class Summary(object):
+    """
+    A class used to represent the summary of the tree
+
+    Attributes:
+    ----------
+        count : int
+            To maintain the count of a node
+        nodes : list
+            To maintain the nodes of a tree
+        tids : set
+            To maintain the timestamps of a database
 
-class UVEclat(_ab._frequentPatterns):
+    """
+
+    def __init__(self, count, nodes):
+        self.count = count
+        self.nodes = nodes
+        self.tids = set()
+
+
+class parallelPFPGrowth(_ab._periodicFrequentPatterns):
     """
     Description:
     -------------
-        It is one of the fundamental algorithm to discover frequent patterns in a uncertain transactional database
-        using PUF-Tree.
+        ParallelPFPGrowth is one of the fundamental distributed algorithm to discover periodic-frequent patterns in a transactional database. It is based PySpark framework.
+
     Reference:
-    ----------
-    Carson Kai-Sang Leung, Lijing Sun: "Equivalence class transformation based mining of frequent itemsets from uncertain data",
-    SAC '11: Proceedings of the 2011 ACM Symposium on Applied ComputingMarch, 2011, Pages 983–984,
-    https://doi.org/10.1145/1982185.1982399
+    -----------
+        C. Saideep, R. Uday Kiran, Koji Zettsu, Cheng-Wei Wu, P. Krishna Reddy, Masashi Toyoda, Masaru Kitsuregawa: Parallel Mining of Partial Periodic Itemsets in Big Data. IEA/AIE 2020: 807-819
 
     Attributes:
-    ------------
+    ----------
         iFile : file
             Name of the Input file or path of the input file
         oFile : file
             Name of the output file or path of the output file
-        minSup: float or int or str
+        minSup: int or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        maxPer: int or float or str
+            The user can specify maxPer either in count or proportion of database size.
+            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
+        numWorker: int
+            The user can specify the number of worker machines to be employed for finding periodic-frequent patterns.
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator.
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
@@ -115,409 +361,392 @@
             To represent the total no of transaction
         tree : class
             To represents the Tree class
         itemSetCount : int
             To represents the total no of patterns
         finalPatterns : dict
             To store the complete patterns
+
     Methods:
-    ---------
+    -------
         startMine()
             Mining process will start from here
         getPatterns()
             Complete set of patterns will be retrieved with this function
-        storePatternsInFile(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
-        getPatternsInDataFrame()
-            Complete set of frequent patterns will be loaded in to a dataframe
+        save(oFile)
+            Complete set of periodic-frequent patterns will be loaded in to a output file
+        getPatternsAsDataFrame()
+            Complete set of periodic-frequent patterns will be loaded in to a dataframe
         getMemoryUSS()
             Total amount of USS memory consumed by the mining process will be retrieved from this function
         getMemoryRSS()
             Total amount of RSS memory consumed by the mining process will be retrieved from this function
         getRuntime()
             Total amount of runtime taken by the mining process will be retrieved from this function
         creatingItemSets(fileName)
             Scans the dataset and stores in a list format
-        frequentOneItem()
-            Extracts the one-length frequent patterns from database
+        PeriodicFrequentOneItem()
+            Extracts the one-periodic-frequent patterns from database
+        updateDatabases()
+            Update the database by removing aperiodic items and sort the Database by item decreased support
+        buildTree()
+            After updating the Database, remaining items will be added into the tree by setting root node as null
+        convert()
+            to convert the user specified value
 
 
     **Methods to execute code on terminal**
 
             Format:
-                      >>> python3 uveclat.py <inputFile> <outputFile> <minSup>
+                      >>>  python3 parallelPFPGrowth.py <inputFile> <outputFile> <minSup> <maxPer> <noWorker>
             Example:
-                      >>>  python3 uveclat.py sampleTDB.txt patterns.txt 3
+                      >>>  python3 parallelPFPGrowth.py sampleTDB.txt patterns.txt 0.3 0.4 5
+
+            .. note:: minSup will be considered in percentage of database transactions
 
-            .. note:: minSup  will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
 
     .. code-block:: python
 
-            from PAMI.uncertainFrequentPattern.basic import UVECLAT as alg
-
-            obj = alg.UVEclat(iFile, minSup)
-
+                from PAMI.periodicFrequentPattern.basic import parallelPFPGrowth as alg
 
-            obj.startMine()
+                obj = alg.parallelPFPGrowth(iFile, minSup, maxPer)
 
-            frequentPatterns = obj.getPatterns()
+                obj.startMine()
 
-            print("Total number of Frequent Patterns:", len(frequentPatterns))
+                periodicFrequentPatterns = obj.getPatterns()
 
-            obj.savePatterns(oFile)
+                print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 
-            Df = obj.getPatternsAsDataFrame()
+                obj.savePatterns(oFile)
 
-            memUSS = obj.getmemoryUSS()
+                Df = obj.getPatternsAsDataFrame()
 
-            print("Total Memory in USS:", memUSS)
+                memUSS = obj.getMemoryUSS()
 
-            memRSS = obj.getMemoryRSS()
+                print("Total Memory in USS:", memUSS)
 
-            print("Total Memory in RSS", memRSS)
+                memRSS = obj.getMemoryRSS()
 
-            run = obj.getRuntime()
+                print("Total Memory in RSS", memRSS)
 
-            print("Total ExecutionTime in seconds:", run)
+                run = obj.getRuntime()
 
-    **Credits:**
-
-         The complete program was written by   P.Likhitha    under the supervision of Professor Rage Uday Kiran.
+                print("Total ExecutionTime in seconds:", run)
 
     """
-    _startTime = float()
-    _endTime = float()
+    __startTime = float()
+    __endTime = float()
     _minSup = str()
-    _finalPatterns = {}
+    _maxPer = str()
+    _numWorkers = str()
+    __finalPatterns = {}
     _iFile = " "
     _oFile = " "
     _sep = " "
-    _memoryUSS = float()
-    _memoryRSS = float()
-    _Database = []
-    _tidList = {}
-    _rank = {}
-
-    def _creatingItemSets(self):
-        """
-            Scans the dataset
-        """
-        self._Database = []
-        if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
-            if self._iFile.empty:
-                print("its empty..")
-            i = self._iFile.columns.values.tolist()
-            if 'Transactions' in i:
-                self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
-
-            # print(self.Database)
-        if isinstance(self._iFile, str):
-            if _ab._validators.url(self._iFile):
-                data = _ab._urlopen(self._iFile)
-                for line in data:
-                    line.strip()
-                    line = line.decode("utf-8")
-                    temp = [i.rstrip() for i in line.split(self._sep)]
-                    temp = [x for x in temp if x]
-                    tr = []
-                    for i in temp:
-                        i1 = i.index('(')
-                        i2 = i.index(')')
-                        item = i[0:i1]
-                        probability = float(i[i1 + 1:i2])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(temp)
-            else:
-                try:
-                    with open(self._iFile, 'r') as f:
-                        for line in f:
-                            temp = [i.rstrip() for i in line.split(self._sep)]
-                            temp = [x for x in temp if x]
-                            tr = []
-                            for i in temp:
-                                i1 = i.index('(')
-                                i2 = i.index(')')
-                                item = i[0:i1]
-                                probability = float(i[i1 + 1:i2])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
-                except IOError:
-                    print("File Not Found")
-
-    def _frequentOneItem(self):
-        """takes the self.Database and calculates the support of each item in the dataset and assign the
-            ranks to the items by decreasing support and returns the frequent items list
-        """
-
-        mapSupport = {}
-        k = 0
-        for i in self._Database:
-            k += 1
-            for j in i:
-                if j.item not in mapSupport:
-                    mapSupport[str(j.item)] = j.probability
-                    self._tidList[str(j.item)] = {k: j.probability}
-                else:
-                    mapSupport[str(j.item)] += j.probability
-                    self._tidList[str(j.item)].update({k: j.probability})
-        mapSupport = {k: v for k, v in mapSupport.items() if v >= self._minSup}
-        plist = dict( sorted(mapSupport.items(), key=_operator.itemgetter(1),reverse=True))
-        return list(plist.keys())
-
-    @staticmethod
-    def _check(i, x):
-        """To check the presence of item or pattern in transaction
-                :param x: it represents the pattern
-                :type x : list
-                :param i : represents the uncertain self.Database
-                :type i : list
-        """
-
-        # This method taken a transaction as input and returns the tree
-        for m in x:
-            k = 0
-            for n in i:
-                if m == n.item:
-                    k += 1
-            if k == 0:
-                return 0
-        return 1
+    __memoryUSS = float()
+    __memoryRSS = float()
+    __Database = []
+    __mapSupport = {}
+    __lno = 0
+    # __tree = _Tree()
+    __rank = {}
+    __rankDup = {}
+    _numTrans = str()
+    __tarunpat = {}
+
+    def __init__(self, iFile, minSup, maxPer, numWorker, sep='\t'):
+        super().__init__(iFile, minSup, maxPer, numWorker, sep)
+
+    def func1(self, ps1, tid):
+        """
+        Add the tid to the set
+
+        :param ps1: set
+        :param tid: timestamp of a database
+
+        return: set
 
-    @staticmethod
-    def _convert(value):
         """
-        To convert the type of user specified minSup value
-            :param value: user specified minSup value
-            :return: converted type minSup value
+        ps1.add(tid)
+        return ps1
+
+    def func2(self, ps1, ps2):
+        """
+
+        Union of two sets
+
+        :param ps1: set
+        :param ps2: set
+
+        return: set
+
+        """
+
+        ps1 |= ps2
+        return ps1
+
+    def func3(self, tids, endts):
+        """
+
+        Calculate the periodicity of a transaction
+
+        :param tids: timestamps of a database
+
+        return: periodicity
+
+
+        """
+        # print(tids)
+        z = sorted(tids)
+        # print(maxPer)
+        cur = 0
+        for i in z:
+            if i - cur > self._maxPer:
+                return -1
+            cur = i
+        if endts - cur > self._maxPer:
+            return -1
+        else:
+            return len(z)
+
+    def getFrequentItems(self, data):
+        """
+        Get the frequent items from the database
+
+        :param data: database
+
+        return: frequent items
+
+        """
+        singleItems = data.flatMap(lambda x: [(x[i], x[0]) for i in range(1, len(x))])
+        ps = set()
+        freqItems = singleItems.aggregateByKey(ps, lambda ps1, tid: self.func1(ps1, tid),
+                                               lambda tuple1, tuple2: self.func2(tuple1, tuple2))
+        # print(freqItems.take(10))
+        freqItems = freqItems.map(lambda x: (x[0], self.func3(x[1], self._numTrans.value)))
+        # print(freqItems.take(10))
+        perFreqItems = [x for (x, y) in
+                        sorted(freqItems.filter(lambda c: c[1] >= self._minSup).collect(), key=lambda x: -x[1])]
+        # print(perFreqItems)
+        return perFreqItems
+
+    def getFrequentItemsets(self, data, freqItems):
+        """
+        Get the frequent itemsets from the database
+
+        :param data: database
+        :param freqItems: frequent items
+
+        return: frequent itemsets
+
+        """
+        rank = dict([(index, item) for (item, index) in enumerate(self._perFreqItems)])
+        numPartitions = data.getNumPartitions()
+        workByPartition = data.flatMap(
+            lambda basket: self.genCondTransactions(basket[0], basket[1:], rank, numPartitions))
+        emptyTree = PFPTree()
+        forest = workByPartition.aggregateByKey(emptyTree,
+                                                lambda tree, transaction: tree.add(transaction[0], [transaction[1]], 1),
+                                                lambda tree1, tree2: tree1.merge(tree2))
+        itemsets = forest.flatMap(
+            lambda partId_bonsai: partId_bonsai[1].extract(self._minSup, self._maxPer, self._numTrans.value,
+                                                           lambda x: self.getPartitionId(x, numPartitions) ==
+                                                                     partId_bonsai[0]))
+        frequentItemsets = itemsets.map(
+            lambda ranks_count: ([self._perFreqItems[z] for z in ranks_count[0]], ranks_count[1]))
+
+        ### TARUN MODIFICATION ###
+        frequentItemsets_list = frequentItemsets.collect()
+
+        for itemset, count in frequentItemsets_list:
+            string = "\t".join([str(x) for x in itemset])
+            self.__tarunpat[string] = count
+        ##########################
+
+        return frequentItemsets
+
+    def genCondTransactions(self, tid, basket, rank, nPartitions):
+        """
+        Get the conditional transactions from the database
+
+        :param tid: timestamp of a database
+        :param basket: basket of a database
+        :param rank: rank of a database
+        :param nPartitions: number of partitions
+
+        """
+        filtered = [rank[int(x)] for x in basket if int(x) in rank.keys()]
+        filtered = sorted(filtered)
+        output = {}
+        for i in range(len(filtered) - 1, -1, -1):
+            item = filtered[i]
+            partition = self.getPartitionId(item, nPartitions)
+            if partition not in output.keys():
+                output[partition] = [filtered[:i + 1], tid]
+        return [x for x in output.items()]
+
+    def getPartitionId(self, key, nPartitions):
+        """
+        Get the partition id
+
+        :param key: key of a database
+        :param nPartitions: number of partitions
+
+        return: partition id
+
+        """
+        return key % nPartitions
+
+    def __convert(self, value):
+        """
+        to convert the type of user specified minSup value
+
+        :param value: user specified minSup value
+
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
-            value = float(value)
+            value = (len(self.__Database) * value)
         if type(value) is str:
             if '.' in value:
                 value = float(value)
+                value = (len(self.__Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _removeFalsePositives(self):
-        """
-            To remove the false positive patterns generated in frequent patterns
-            :return: patterns with accurate probability
+    def startMine(self):
         """
-        global _finalPatterns
-        periods = {}
-        for i in self._Database:
-            for x, y in _finalPatterns.items():
-                if len(x) == 1:
-                    periods[x] = y
-                else:
-                    s = 1
-                    check = self._check(i, x)
-                    if check == 1:
-                        for j in i:
-                            if j.item in x:
-                                s *= j.probability
-                        if x in periods:
-                            periods[x] += s
-                        else:
-                            periods[x] = s
-        for x, y in periods.items():
-            if y >= self._minSup:
-                sample = str()
-                for i in x:
-                    sample = sample + i + "\t"
-                self._finalPatterns[sample] = y
-
-    @staticmethod
-    def _Intersection(tidSetx, tidSetY):
-        tids = []
-        support = []
-        tidDict = {}
-        for x, y in tidSetx.items():
-            for x1, y1 in tidSetY.items():
-                if x == x1:
-                    tids.append(x)
-                    support.append(y * y1)
-                    tidDict.update({x: y * y1})
-        return tidDict
-
-    def _calculateExpSup(self, tidList):
-        return sum(tidList.values())
-
-    def _save(self, prefix, suffix, tidSetI):
-        """Saves the patterns that satisfy the periodic frequent property.
-            :param prefix: the prefix of a pattern
-            :type prefix: list
-            :param suffix: the suffix of a patterns
-            :type suffix: list
-            :param tidSetI: the timestamp of a patterns
-            :type tidSetI: dict
-        """
-
-        global _finalPatterns
-        if prefix is None:
-            prefix = suffix
-        else:
-            prefix = prefix + suffix
-        val = self._calculateExpSup(tidSetI)
-        _finalPatterns[tuple(prefix)] = val
-
-    def _Generation(self, prefix, itemSets, tidSets):
-        """Equivalence class is followed  and checks for the patterns generated for periodic-frequent patterns.
-            :param prefix:  main equivalence prefix
-            :type prefix: periodic-frequent item or pattern
-            :param itemSets: patterns which are items combined with prefix and satisfying the periodicity
-                            and frequent with their timestamps
-            :type itemSets: list
-            :param tidSets: timestamps of the items in the argument itemSets
-            :type tidSets: list
-                    """
-        if len(itemSets) == 1:
-            i = itemSets[0]
-            tidI = tidSets[0]
-            self._save(prefix, [i], tidI)
-            return
-        for i in range(len(itemSets)):
-            itemI = itemSets[i]
-            if itemI is None:
-                continue
-            tidSetI = tidSets[i]
-            classItemSets = []
-            classTidSets = []
-            itemSetX = [itemI]
-            for j in range(i + 1, len(itemSets)):
-                itemJ = itemSets[j]
-                tidSetJ = tidSets[j]
-                y = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y) >= self._minSup:
-                    classItemSets.append(itemJ)
-                    classTidSets.append(y)
-            newPrefix = list(set(itemSetX)) + prefix
-            self._Generation(newPrefix, classItemSets, classTidSets)
-            self._save(prefix, list(set(itemSetX)), tidSetI)
+        Start the mining process
 
-    def startMine(self):
-        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
-            by counting the original support of a patterns
         """
-        global _minSup
-        self._startTime = _ab._time.time()
-        self._creatingItemSets()
-        self._minSup = self._convert(self._minSup)
-        _minSup = self._minSup
-        plist = self._frequentOneItem()
-        for i in range(len(plist)):
-            itemI = plist[i]
-            tidSetI = self._tidList[itemI]
-            itemSetX = [itemI]
-            itemSets = []
-            tidSets = []
-            for j in range(i+1, len(plist)):
-                itemJ = plist[j]
-                tidSetJ = self._tidList[itemJ]
-                y1 = self._Intersection(tidSetI, tidSetJ)
-                if self._calculateExpSup(y1) >= self._minSup:
-                    itemSets.append(itemJ)
-                    tidSets.append(y1)
-            self._Generation(itemSetX, itemSets, tidSets)
-            self._save(None, itemSetX, tidSetI)
-        self._removeFalsePositives()
-        print("Frequent patterns were generated from uncertain databases successfully using PUF algorithm")
-        self._endTime = _ab._time.time()
+        self.__startTime = _ab._time.time()
+        APP_NAME = "parallelPFPGrowth"
+        conf = _ab.SparkConf().setAppName(APP_NAME)
+        # conf = conf.setMaster("local[*]")
+        sc = _ab.SparkContext(conf=conf).getOrCreate()
+        # sc = SparkContext.getOrCreate();
+        data = sc.textFile(self._iFile, minPartitions=self._numWorkers).map(
+            lambda x: [int(y) for y in x.strip().split(self._sep)])
+        # data = sc.textFile(finput).map(lambda x: [int(y) for y in x.strip().split(' ')])
+        data.cache()
+        # minSupport = data.count() * threshold/100
+        # maxPer = data.count() * periodicity_threshold/100
+        self._minSup = self.__convert(self._minSup)
+        self._maxPer = self.__convert(self._maxPer)
+        self._numTrans = sc.broadcast(data.count())
+        self._perFreqItems = self.getFrequentItems(data)
+        freqItemsets = self.getFrequentItemsets(data, self._perFreqItems)
+        self.__finalPatterns = self.__tarunpat
+        sc.stop()
+        self.__endTime = _ab._time.time()
+        self.__memoryUSS = float()
+        self.__memoryRSS = float()
         process = _ab._psutil.Process(_ab._os.getpid())
-        self._memoryRSS = float()
-        self._memoryUSS = float()
-        self._memoryUSS = process.memory_full_info().uss
-        self._memoryRSS = process.memory_info().rss
+        self.__memoryUSS = process.memory_full_info().uss
+        self.__memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
+
         :rtype: float
         """
 
-        return self._memoryUSS
+        return self.__memoryUSS
 
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
+
         :rtype: float
         """
 
-        return self._memoryRSS
+        return self.__memoryRSS
 
     def getRuntime(self):
         """Calculating the total amount of runtime taken by the mining process
+
+
         :return: returning total amount of runtime taken by the mining process
+
         :rtype: float
         """
 
-        return self._endTime - self._startTime
+        return self.__endTime - self.__startTime
 
     def getPatternsAsDataFrame(self):
         """Storing final frequent patterns in a dataframe
+
         :return: returning frequent patterns in a dataframe
+
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
-        for a, b in self._finalPatterns.items():
+        for a, b in self.__tarunpat.items():
             data.append([a.replace('\t', ' '), b])
             dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
         return dataframe
 
-    def save(self, oFile):
+    def save(self, outFile):
         """Complete set of frequent patterns will be loaded in to a output file
-        :param oFile: name of the output file
-        :type oFile: file
+
+        :param outFile: name of the output file
+
+        :type outFile: file
         """
-        self.oFile = oFile
-        writer = open(self.oFile, 'w+')
-        for x, y in self._finalPatterns.items():
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
+        # print(self.getFrequentItems())
+        for x, y in self.__tarunpat.items():
+            # print(x,y)
             s1 = x.strip() + ":" + str(y)
             writer.write("%s \n" % s1)
 
     def getPatterns(self):
         """ Function to send the set of frequent patterns after completion of the mining process
+
         :return: returning frequent patterns
+
         :rtype: dict
         """
-        return self._finalPatterns
+        return self.__tarunpat
 
     def printResults(self):
-        print("Total number of  Uncertain Frequent Patterns:", len(self.getPatterns()))
+        print("Total number of Frequent Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
-        print("Total ExecutionTime in ms:",  self.getRuntime())
+        print("Total ExecutionTime in ms:", self.getRuntime())
 
 
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 4 or len(_ab._sys.argv) == 5:
-        if len(_ab._sys.argv) == 5:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4])
+    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
+        if len(_ab._sys.argv) == 7:
+            _ap = parallelPFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5],
+                                    _ab._sys.argv[6])
         if len(_ab._sys.argv) == 4:
-            _ap = UVEclat(_ab._sys.argv[1], _ab._sys.argv[3])
+            _ap = parallelPFPGrowth(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
         _ap.startMine()
-        print("Total number of Patterns:", len(_ap.getPatterns()))
+        print("Total number of Frequent Patterns:", _ab.getPatterns())
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
         print("Total ExecutionTime in ms:", _ap.getRuntime())
     else:
+        _ap = parallelPFPGrowth('Temporal_T10I4D100K.csv', 500, 5000, 5, '\t')
+        _ap.startMine()
+        # print("Total number of Frequent Patterns:", len( _ab.getPatterns()))
+        # _ap.save(_ab._sys.argv[2])
+        _ap.printResults()
+        # print("Total Memory in USS:", _ap.getMemoryUSS())
+        # print("Total Memory in RSS", _ap.getMemoryRSS())
+        # print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.uncertainPeriodicFrequentPattern import UPFPGrowth as alg
+#     from PAMI.uncertainPeriodicFrequentPattern import basic as alg
 #
-#     obj = alg.UPFPGrowth(iFile, minSup, maxPer)
+#     obj = alg.basic(iFile, minSup, maxPer)
 #
 #     obj.startMine()
 #
 #     periodicFrequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
 #
@@ -372,15 +372,15 @@
 
 
 class UPFPGrowth(_ab._periodicFrequentPatterns):
     """
     Description:
     -------------
 
-        UPFPGrowth is  to discover periodic-frequent patterns in a uncertain temporal database.
+        basic is  to discover periodic-frequent patterns in a uncertain temporal database.
 
     Reference:
     ---------------
             Uday Kiran, R., Likhitha, P., Dao, MS., Zettsu, K., Zhang, J. (2021).
             Discovering Periodic-Frequent Patterns in Uncertain Temporal Databases. In:
             Mantoro, T., Lee, M., Ayu, M.A., Wong, K.W., Hidayanto, A.N. (eds) Neural Information Processing.
             ICONIP 2021. Communications in Computer and Information Science, vol 1516. Springer, Cham.
@@ -454,28 +454,28 @@
                 to remove the false positives in generated patterns
 
     Executing the code on terminal:
     --------------------------------------------
         Format:
         -------
 
-           >>> python3 UPFPGrowth.py <inputFile> <outputFile> <minSup> <maxPer>
+           >>> python3 basic.py <inputFile> <outputFile> <minSup> <maxPer>
 
         Examples:
         ------------------------
-           >>> python3 UPFPGrowth.py sampleTDB.txt patterns.txt 0.3 4     (minSup and maxPer will be considered in support count or frequency)
+           >>> python3 basic.py sampleTDB.txt patterns.txt 0.3 4     (minSup and maxPer will be considered in support count or frequency)
 
     **Importing this algorithm into a python program**
     -----------------------------------------------------------------
 
     .. code-block:: python
 
-        from PAMI.uncertainPeriodicFrequentPattern import UPFPGrowth as alg
+        from PAMI.uncertainPeriodicFrequentPattern import basic as alg
 
-        obj = alg.UPFPGrowth(iFile, minSup, maxPer)
+        obj = alg.basic(iFile, minSup, maxPer)
 
         obj.startMine()
 
         periodicFrequentPatterns = obj.getPatterns()
 
         print("Total number of Periodic Frequent Patterns:", len(periodicFrequentPatterns))
```

### Comparing `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.8.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files 0% similar despite different names*

```diff
@@ -400,15 +400,15 @@
             self.removeNode(i)
 
 class UPFPGrowthPlus(_ab._periodicFrequentPatterns):
     """
     Description:
     -------------
 
-        UPFPGrowth Plus is  to discover periodic-frequent patterns in a uncertain temporal database.
+        basic Plus is  to discover periodic-frequent patterns in a uncertain temporal database.
 
     Reference:
     ------------
 
 
 
     Attributes:
```

### Comparing `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,151 +8,165 @@
 #      This program is distributed in the hope that it will be useful,
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU General Public License for more details.
 #
 #      You should have received a copy of the GNU General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
+#
+#      This program is free software: you can redistribute it and/or modify
+#      it under the terms of the GNU General Public License as published by
+#      the Free Software Foundation, either version 3 of the License, or
+#      (at your option) any later version.
+#
+#      This program is distributed in the hope that it will be useful,
+#      but WITHOUT ANY WARRANTY; without even the implied warranty of
+#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#      GNU General Public License for more details.
+#
+#      You should have received a copy of the GNU General Public License
+#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
+# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
-import math as _math
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
+import functools as _functools
 
 
-class _periodicFrequentPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every periodic-frequent pattern mining algorithm must
+class _weightedFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
-       Attributes
-        ----------
+
+
+       Attributes:
+       ----------
         iFile : str
             Input file name or path of the input file
-        minSup: int or float or str
+        minSup: integer or float or str
             The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        maxPer: int or float or str
-            The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator.
+            However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
         finalPatterns: dict
             Storing the complete set of patterns in a dictionary variable
         oFile : str
-            Name of the output file to store complete set of periodic-frequent patterns
+            Name of the output file to store complete set of frequent patterns
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
-        Methods
-        -------
+
+       Methods:
+       -------
         startMine()
-            Mining process will start from here
+            Calling this function will start the actual mining process
         getPatterns()
-            Complete set of patterns will be retrieved with this function
+            This function will output all interesting patterns discovered by an algorithm
         save(oFile)
-            Complete set of periodic-frequent patterns will be loaded in to a output file
+            This function will store the discovered patterns in an output file specified by the user
         getPatternsAsDataFrame()
-            Complete set of periodic-frequent patterns will be loaded in to data frame
+            The function outputs the patterns generated by an algorithm as a data frame
         getMemoryUSS()
-            Total amount of USS memory consumed by the program will be retrieved from this function
+            This function outputs the total amount of USS memory consumed by a mining algorithm
         getMemoryRSS()
-            Total amount of RSS memory consumed by the program will be retrieved from this function
+            This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
-            Total amount of runtime taken by the program will be retrieved from this function
+            This function outputs the total runtime of a mining algorithm
+
     """
 
-    def __init__(self, iFile, minSup, maxPer, sep = '\t'):
+    def __init__(self, iFile, wFile, minSup, minWeight, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
-        :type iFile: str
+        :type iFile: str or DataFrame
+        :param wFile: Input file name or path of the input file
+        :type wFile: str or DataFrame
         :param minSup: The user can specify minSup either in count or proportion of database size.
             If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
             Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
         :type minSup: int or float or str
-        :param maxPer: The user can specify maxPer either in count or proportion of database size.
-            If the program detects the data type of maxPer is integer, then it treats maxPer is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: maxPer=10 will be treated as integer, while maxPer=10.0 will be treated as float
-        :type maxPer: int or float or str
-        :param sep: The user specified seperator used in the input file
-        :type maxPer: str
+        :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
+        :type sep: str
         """
 
         self._iFile = iFile
-        self._minSup = minSup
-        self._maxPer = maxPer
+        self._wFile = wFile
         self._sep = sep
-        self._oFile = str()
+        self._minSup = minSup
+        self._minWeight = minWeight
         self._finalPatterns = {}
+        self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
     @_abstractmethod
     def startMine(self):
         """Code for the mining process will start from this function"""
 
         pass
 
     @_abstractmethod
     def getPatterns(self):
-        """Complete set of periodic-frequent patterns generated will be retrieved from this function"""
+        """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
-        """Complete set of periodic-frequent patterns will be saved in to an output file from this function
+        """Complete set of frequent patterns will be saved in to an output file from this function
+
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
     @_abstractmethod
     def getPatternsAsDataFrame(self):
-        """Complete set of periodic-frequent patterns will be loaded in to data frame from this function"""
+        """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def getMemoryRSS(self):
         """Total amount of RSS memory consumed by the program will be retrieved from this function"""
+
         pass
 
     @_abstractmethod
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
         """ To print all the results of execution"""
 
-        pass
+
+        pass
```

### Comparing `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.8.1/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.weightFrequentPattern.basic import WFIM as alg
+#     from PAMI.weightFrequentPattern.basic import basic as alg
 #
-#     obj = alg.WFIM(iFile, wFile, minSup, minWeight)
+#     obj = alg.basic(iFile, wFile, minSup, minWeight)
 #
 #     obj.startMine()
 #
 #     frequentPatterns = obj.getPatterns()
 #
 #     print("Total number of Frequent Patterns:", len(frequentPatterns))
 #
@@ -296,27 +296,27 @@
         creatingItemSets()
             Scans the dataset or dataframes and stores in list format
         frequentOneItem()
             Extracts the one-frequent patterns from transactions
     Methods to execute code on terminal
     ------------------------------------
         Format:
-                  >>>  python3 WFIM.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
+                  >>>  python3 basic.py <inputFile> <weightFile> <outputFile> <minSup> <minWeight>
         Example:
-                  >>>  python3 WFIM.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
+                  >>>  python3 basic.py sampleDB.txt weightSample.txt patterns.txt 10.0 3.4
 
                  .. note:: minSup and maxPer will be considered in support count or frequency
 
     **Importing this algorithm into a python program**
     --------------------------------------------------
     .. code-block:: python
 
-            from PAMI.weightFrequentPattern.basic import WFIM as alg
+            from PAMI.weightFrequentPattern.basic import basic as alg
 
-            obj = alg.WFIM(iFile, wFile, minSup, minWeight)
+            obj = alg.basic(iFile, wFile, minSup, minWeight)
 
             obj.startMine()
 
             frequentPatterns = obj.getPatterns()
 
             print("Total number of Frequent Patterns:", len(frequentPatterns))
 
@@ -550,15 +550,15 @@
         info = {self.__rank[k]: v for k, v in self.__mapSupport.items()}
         __Tree = self.__buildTree(updatedTransactions, info)
         patterns = __Tree.generatePatterns([])
         self.__finalPatterns = {}
         for k in patterns:
             s = self.__savePeriodic(k[0])
             self.__finalPatterns[str(s)] = k[1]
-        print("Weighted Frequent patterns were generated successfully using WFIM algorithm")
+        print("Weighted Frequent patterns were generated successfully using basic algorithm")
         self.__endTime = _fp._time.time()
         self.__memoryUSS = float()
         self.__memoryRSS = float()
         process = _fp._psutil.Process(_fp._os.getpid())
         self.__memoryUSS = process.memory_full_info().uss
         self.__memoryRSS = process.memory_info().rss
```

### Comparing `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,28 +38,31 @@
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
 
 
-class _weightedFrequentPatterns(_ABC):
+class _weightedFrequentRegularPatterns(_ABC):
     """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
         employ in PAMI
 
 
        Attributes:
        ----------
         iFile : str
             Input file name or path of the input file
-        minSup: integer or float or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
+            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
+        :param regularity: The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
         sep : str
             This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
             However, the users can override their default separator
         startTime:float
             To record the start time of the algorithm
         endTime:float
             To record the completion time of the algorithm
@@ -87,34 +90,39 @@
         getMemoryRSS()
             This function outputs the total amount of RSS memory consumed by a mining algorithm
         getRuntime()
             This function outputs the total runtime of a mining algorithm
 
     """
 
-    def __init__(self, iFile, wFile, minSup, minWeight, sep="\t"):
+    def __init__(self, iFile, wFile, weightSupport, regularity, sep="\t"):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
-        :param wFile: Input file name or path of the input file
+        :param wFile: Input weight file name or path of the input file
         :type wFile: str or DataFrame
-        :param minSup: The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
+            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
+            Otherwise, it will be treated as float.
+            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
+        :type weightSupport: int or float or str
+        :param regularity: The user can specify regularity either in count or proportion of database size.
+            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
             Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        :type minSup: int or float or str
+            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
+        :type regularity: int or float or str
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
         self._wFile = wFile
         self._sep = sep
-        self._minSup = minSup
-        self._minWeight = minWeight
+        self._regularity = regularity
+        self._WS = weightSupport
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
@@ -164,9 +172,8 @@
 
         pass
 
     @_abstractmethod
     def printResults(self):
         """ To print all the results of execution"""
 
-
         pass
```

### Comparing `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/periodicFrequentPattern/pyspark/abstract.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,87 @@
-#  Copyright (C)  2021 Rage Uday Kiran
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-#
-#      This program is free software: you can redistribute it and/or modify
-#      it under the terms of the GNU General Public License as published by
-#      the Free Software Foundation, either version 3 of the License, or
-#      (at your option) any later version.
-#
-#      This program is distributed in the hope that it will be useful,
-#      but WITHOUT ANY WARRANTY; without even the implied warranty of
-#      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#      GNU General Public License for more details.
-#
-#      You should have received a copy of the GNU General Public License
-#      along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-# from abc import ABC as _ABC, abstractmethod as _abstractmethod
 from abc import ABC as _ABC, abstractmethod as _abstractmethod
 import time as _time
 import csv as _csv
 import pandas as _pd
 from collections import defaultdict as _defaultdict
 from itertools import combinations as _c
 import os as _os
 import os.path as _ospath
 import psutil as _psutil
 import sys as _sys
 import validators as _validators
 from urllib.request import urlopen as _urlopen
 import functools as _functools
+from pyspark import SparkContext, SparkConf
 
-
-class _weightedFrequentRegularPatterns(_ABC):
-    """ This abstract base class defines the variables and methods that every frequent pattern mining algorithm must
-        employ in PAMI
+class _periodicFrequentPatterns(_ABC):
+    """ This abstract base class defines the variables and methods that every periodic frequent pattern mining algorithm must
+            employ in PAMI
+           Attributes:
+           ----------
+            iFile : str
+                Input file name or path of the input file
+            minSup: integer or float or str
+                The user can specify minSup either in count or proportion of database size.
+                If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+                Otherwise, it will be treated as float.
+                Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+            sep : str
+                This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
+                However, the users can override their default separator
+            startTime:float
+                To record the start time of the algorithm
+            endTime:float
+                To record the completion time of the algorithm
+            finalPatterns: dict
+                Storing the complete set of patterns in a dictionary variable
+            oFile : str
+                Name of the output file to store complete set of frequent patterns
+            memoryUSS : float
+                To store the total amount of USS memory consumed by the program
+            memoryRSS : float
+                To store the total amount of RSS memory consumed by the program
+           Methods:
+           -------
+            startMine()
+                Calling this function will start the actual mining process
+            getPatterns()
+                This function will output all interesting patterns discovered by an algorithm
+            save(oFile)
+                This function will store the discovered patterns in an output file specified by the user
+            getMemoryUSS()
+                This function outputs the total amount of USS memory consumed by a mining algorithm
+            getMemoryRSS()
+                This function outputs the total amount of RSS memory consumed by a mining algorithm
+            getRuntime()
+                This function outputs the total runtime of a mining algorithm
+    """
 
 
-       Attributes:
-       ----------
-        iFile : str
-            Input file name or path of the input file
-        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
-            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
-        :param regularity: The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
-        sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator
-        startTime:float
-            To record the start time of the algorithm
-        endTime:float
-            To record the completion time of the algorithm
-        finalPatterns: dict
-            Storing the complete set of patterns in a dictionary variable
-        oFile : str
-            Name of the output file to store complete set of frequent patterns
-        memoryUSS : float
-            To store the total amount of USS memory consumed by the program
-        memoryRSS : float
-            To store the total amount of RSS memory consumed by the program
-
-       Methods:
-       -------
-        startMine()
-            Calling this function will start the actual mining process
-        getPatterns()
-            This function will output all interesting patterns discovered by an algorithm
-        save(oFile)
-            This function will store the discovered patterns in an output file specified by the user
-        getPatternsAsDataFrame()
-            The function outputs the patterns generated by an algorithm as a data frame
-        getMemoryUSS()
-            This function outputs the total amount of USS memory consumed by a mining algorithm
-        getMemoryRSS()
-            This function outputs the total amount of RSS memory consumed by a mining algorithm
-        getRuntime()
-            This function outputs the total runtime of a mining algorithm
 
-    """
-
-    def __init__(self, iFile, wFile, weightSupport, regularity, sep="\t"):
+    def __init__(self, iFile, minSup, maxPer, numWorkers, sep='\t'):
         """
         :param iFile: Input file name or path of the input file
         :type iFile: str or DataFrame
-        :param wFile: Input weight file name or path of the input file
-        :type wFile: str or DataFrame
-        :param weightSupport(ws): The user can specify ws either in count or proportion of database size.
-            If the program detects the data type of ws is integer, then it treats ws is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: ws=10 will be treated as integer, while ws=10.0 will be treated as float
-        :type weightSupport: int or float or str
-        :param regularity: The user can specify regularity either in count or proportion of database size.
-            If the program detects the data type of regularity is integer, then it treats regularity is expressed in count.
+        :param minSup: The user can specify minSup either in count or proportion of database size.
+            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
             Otherwise, it will be treated as float.
-            Example: regularity=10 will be treated as integer, while regularity=10.0 will be treated as float
-        :type regularity: int or float or str
+            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
+        :type minSup: int or float or str
+        :param numWorkers: The user can specify numWorkers as the number of cores which are used.
+        :type numWorkers: int
         :param sep: separator used to distinguish items from each other. The default separator is tab space. However, users can override the default separator
         :type sep: str
         """
 
         self._iFile = iFile
-        self._wFile = wFile
+        self._minSup = minSup
+        self._maxPer = maxPer
+        self._numWorkers = numWorkers
         self._sep = sep
-        self._regularity = regularity
-        self._WS = weightSupport
         self._finalPatterns = {}
         self._oFile = str()
         self._memoryUSS = float()
         self._memoryRSS = float()
         self._startTime = float()
         self._endTime = float()
 
@@ -137,26 +96,25 @@
         """Complete set of frequent patterns generated will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def save(self, oFile):
         """Complete set of frequent patterns will be saved in to an output file from this function
-
         :param oFile: Name of the output file
         :type oFile: file
         """
 
         pass
 
-    @_abstractmethod
-    def getPatternsAsDataFrame(self):
-        """Complete set of frequent patterns will be loaded in to data frame from this function"""
+#     @_abstractmethod
+#     def getPatternsAsDataFrame(self):
+#         """Complete set of frequent patterns will be loaded in to data frame from this function"""
 
-        pass
+#         pass
 
     @_abstractmethod
     def getMemoryUSS(self):
         """Total amount of USS memory consumed by the program will be retrieved from this function"""
 
         pass
 
@@ -170,10 +128,10 @@
     def getRuntime(self):
         """Total amount of runtime taken by the program will be retrieved from this function"""
 
         pass
 
     @_abstractmethod
     def printResults(self):
-        """ To print all the results of execution"""
+        """ To print the results of execution."""
 
         pass
```

### Comparing `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.8.1/PAMI/correlatedPattern/basic/CoMine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
+# CoMine is one of the fundamental algorithm to discover correlated patterns in a transactional database.
+#
 # **Importing this algorithm into a python program**
 # --------------------------------------------------------
 #
 #
-#     from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
+#             from PAMI.correlatedPattern.basic import CoMine as alg
 #
-#     obj = alg.WFIM(iFile, wFile, expSup, expWSup)
+#             obj = alg.CoMine(iFile, minSup, minAllConf, sep)
 #
-#     obj.startMine()
+#             obj.startMine()
 #
-#     Patterns = obj.getPatterns()
+#             Rules = obj.getPatterns()
 #
-#     print("Total number of  Patterns:", len(Patterns))
+#             print("Total number of  Patterns:", len(Patterns))
 #
-#     obj.savePatterns(oFile)
+#             obj.save(oFile)
 #
-#     Df = obj.getPatternsAsDataFrame()
+#             Df = obj.getPatternsAsDataFrame()
 #
-#     memUSS = obj.getMemoryUSS()
+#             memUSS = obj.getMemoryUSS()
 #
-#     print("Total Memory in USS:", memUSS)
+#             print("Total Memory in USS:", memUSS)
 #
-#     memRSS = obj.getMemoryRSS()
+#             memRSS = obj.getMemoryRSS()
 #
-#     print("Total Memory in RSS", memRSS)
+#             print("Total Memory in RSS", memRSS)
 #
-#     run = obj.getRuntime()
+#             run = obj.getRuntime()
 #
-#     print("Total ExecutionTime in seconds:", run)
+#             print("Total ExecutionTime in seconds:", run)
+
+
+
 
 
 __copyright__ = """
  Copyright (C)  2021 Rage Uday Kiran
 
      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
@@ -44,722 +49,649 @@
 
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <https://www.gnu.org/licenses/>.
      Copyright (C)  2021 Rage Uday Kiran
 
 """
 
-from PAMI.weightedUncertainFrequentPattern.basic import abstract as _ab
-
-_expSup = str()
-_expWSup = str()
-_weights = {}
-_finalPatterns = {}
-_ab._sys.setrecursionlimit(20000)
-
+from PAMI.correlatedPattern.basic import abstract as _ab
 
-class _Item:
+class _Node:
     """
-    A class used to represent the item with probability in transaction of dataset
-    ...
-    Attributes:
-    __________
-        item : int or word
-            Represents the name of the item
-        probability : float
-            Represent the existential probability(likelihood presence) of an item
-    """
-
-    def __init__(self, item, probability):
-        self.item = item
-        self.probability = probability
+    A class used to represent the node of correlatedPatternTree
 
 
-class _Node(object):
-    """
-    A class used to represent the node of frequentPatternTree
-        ...
-    Attributes:
+    Attributes :
     ----------
-        item : int
+        itemId : int
             storing item of a node
-        probability : int
-            To maintain the expected support of node
+        counter : int
+            To maintain the support of node
         parent : node
             To maintain the parent of every node
-        children : list
+        child : list
             To maintain the children of node
-    Methods:
+        nodeLink : node
+            Points to the node with same itemId
+
+    Methods :
     -------
-        addChild(itemName)
-            storing the children to their respective parent nodes
+
+        getChild(itemName)
+            returns the node with same itemName from correlatedPatternTree
     """
 
-    def __init__(self, item, children):
-        self.item = item
-        self.probability = 1
-        self.children = children
+    def __init__(self):
+        self.itemId = -1
+        self.counter = 1
         self.parent = None
+        self.child = []
+        self.nodeLink = None
 
-    def addChild(self, node):
-        self.children[node.item] = node
-        node.parent = self
+    def getChild(self, id1):
+        """
+
+        Param id1: give item id as input
+        type id1:
+
+        """
+        for i in self.child:
+            if i.itemId == id1:
+                return i
+        return None
 
 
-class _Tree(object):
+class _Tree:
     """
-    A class used to represent the frequentPatternGrowth tree structure
-    ...
-    Attributes:
+        A class used to represent the correlatedPatternGrowth tree structure
+
+    Attributes :
     ----------
-        root : Node
-            Represents the root node of the tree
-        summaries : dictionary
+        headerList : list
+            storing the list of items in tree sorted in ascending of their supports
+        mapItemNodes : dictionary
             storing the nodes with same item name
-        info : dictionary
-            stores the support of items
-    Methods:
+        mapItemLastNodes : dictionary
+            representing the map that indicates the last node for each item
+        root : Node
+            representing the root Node in a tree
+
+
+    Methods :
     -------
+        createHeaderList(items,minSup)
+            takes items only which are greater than minSup and sort the items in ascending order
         addTransaction(transaction)
-            creating transaction as a branch in frequentPatternTree
-        addConditionalPattern(prefixPaths, supportOfItems)
-            construct the conditional tree for prefix paths
-        conditionalPatterns(Node)
-            generates the conditional patterns from tree for specific node
-        conditionalTransactions(prefixPaths,Support)
-            takes the prefixPath of a node and support at child of the path and extract the frequent items from
-            prefixPaths and generates prefixPaths with items which are frequent
-        remove(Node)
-            removes the node from tree once after generating all the patterns respective to the node
-        generatePatterns(Node)
-            starts from the root node of the tree and mines the frequent patterns
+            creating transaction as a branch in correlatedPatternTree
+        fixNodeLinks(item,newNode)
+            To create the link for nodes with same item
+        printTree(Node)
+            gives the details of node in correlatedPatternGrowth tree
+        addPrefixPath(prefix,port,minSup)
+           It takes the items in prefix pattern whose support is >=minSup and construct a subtree
     """
 
     def __init__(self):
-        self.root = _Node(None, {})
-        self.summaries = {}
-        self.info = {}
+        self.headerList = []
+        self.mapItemNodes = {}
+        self.mapItemLastNodes = {}
+        self.root = _Node()
 
     def addTransaction(self, transaction):
-        """adding transaction into tree
-            :param transaction : it represents the one self.Database in database
-            :type transaction : list
-        """
-
-        currentNode = self.root
-        for i in range(len(transaction)):
-            if transaction[i].item not in currentNode.children:
-                newNode = _Node(transaction[i].item, {})
-                l1 = i - 1
-                lp = []
-                while l1 >= 0:
-                    lp.append(transaction[l1].probability)
-                    l1 -= 1
-                if len(lp) == 0:
-                    newNode.probability = transaction[i].probability
-                else:
-                    newNode.probability = max(lp) * transaction[i].probability
-                currentNode.addChild(newNode)
-                if transaction[i].item in self.summaries:
-                    self.summaries[transaction[i].item].append(newNode)
-                else:
-                    self.summaries[transaction[i].item] = [newNode]
-                currentNode = newNode
-            else:
-                currentNode = currentNode.children[transaction[i].item]
-                l1 = i - 1
-                lp = []
-                while l1 >= 0:
-                    lp.append(transaction[l1].probability)
-                    l1 -= 1
-                if len(lp) == 0:
-                    currentNode.probability += transaction[i].probability
-                else:
-                    currentNode.probability += max(lp) * transaction[i].probability
+        """
+        adding transaction into tree
 
-    def addConditionalPattern(self, transaction, sup):
-        """constructing conditional tree from prefixPaths
-            :param transaction : it represents the one self.Database in database
-            :type transaction : list
-            :param sup : support of prefixPath taken at last child of the path
-            :type sup : int
-        """
-
-        # This method takes transaction, support and constructs the conditional tree
-        currentNode = self.root
-        for i in range(len(transaction)):
-            if transaction[i] not in currentNode.children:
-                newNode = _Node(transaction[i], {})
-                newNode.probability = sup
-                currentNode.addChild(newNode)
-                if transaction[i] in self.summaries:
-                    self.summaries[transaction[i]].append(newNode)
-                else:
-                    self.summaries[transaction[i]] = [newNode]
-                currentNode = newNode
+        :param transaction : it represents a single transaction in a database
+        :type transaction : list
+        """
+
+        current = self.root
+        for i in transaction:
+            child = current.getChild(i)
+            if child is None:
+                newNode = _Node()
+                newNode.itemId = i
+                newNode.parent = current
+                current.child.append(newNode)
+                self.fixNodeLinks(i, newNode)
+                current = newNode
             else:
-                currentNode = currentNode.children[transaction[i]]
-                currentNode.probability += sup
+                child.counter += 1
+                current = child
 
-    def conditionalPatterns(self, alpha):
-        """generates all the conditional patterns of respective node
-            :param alpha : it represents the Node in tree
-            :type alpha : _Node
-        """
-
-        # This method generates conditional patterns of node by traversing the tree
-        finalPatterns = []
-        sup = []
-        for i in self.summaries[alpha]:
-            s = i.probability
-            set2 = []
-            while i.parent.item is not None:
-                set2.append(i.parent.item)
-                i = i.parent
-            if len(set2) > 0:
-                set2.reverse()
-                finalPatterns.append(set2)
-                sup.append(s)
-        finalPatterns, support, info = self.conditionalTransactions(finalPatterns, sup)
-        return finalPatterns, support, info
-
-    def removeNode(self, nodeValue):
-        """removing the node from tree
-            :param nodeValue : it represents the node in tree
-            :type nodeValue : node
-        """
-
-        for i in self.summaries[nodeValue]:
-            del i.parent.children[nodeValue]
-
-    def conditionalTransactions(self, condPatterns, support):
-        """ It generates the conditional patterns with frequent items
-                :param condPatterns : conditionalPatterns generated from conditionalPattern method for respective node
-                :type condPatterns : list
-                :support : the support of conditional pattern in tree
-                :support : int
-        """
-
-        global _expSup, _expWSup
-        pat = []
-        sup = []
-        count = {}
-        for i in range(len(condPatterns)):
-            for j in condPatterns[i]:
-                if j in count:
-                    count[j] += support[i]
+    def fixNodeLinks(self, item, newNode):
+        """
+        Fixing node link for the newNode that inserted into correlatedPatternTree
+
+        :param item: it represents the item of newNode
+        :type item : int
+        :param newNode : it represents the newNode that inserted in correlatedPatternTree
+        :type newNode : Node
+
+        """
+        if item in self.mapItemLastNodes.keys():
+            lastNode = self.mapItemLastNodes[item]
+            lastNode.nodeLink = newNode
+        self.mapItemLastNodes[item] = newNode
+        if item not in self.mapItemNodes.keys():
+            self.mapItemNodes[item] = newNode
+
+    def printTree(self, root):
+        """
+        This method is to find the details of parent, children, and support of a Node
+
+        :param root: it represents the Node in correlatedPatternTree
+        :type root: Node
+
+        """
+
+        if root.child is None:
+            return
+        else:
+            for i in root.child:
+                print(i.itemId, i.counter, i.parent.itemId)
+                self.printTree(i)
+
+    def createHeaderList(self, mapSupport, minSup):
+        """
+        To create the headerList
+
+        :param mapSupport : it represents the items with their supports
+        :type mapSupport : dictionary
+        :param minSup : it represents the minSup
+        :param minSup : float
+        """
+        
+        t1 = []
+        for x, y in mapSupport.items():
+            if y >= minSup:
+                t1.append(x)
+        itemSetBuffer = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        self.headerList = [i for i in t1 if i in itemSetBuffer]
+
+    def addPrefixPath(self, prefix, mapSupportBeta, minSup):
+        """
+        To construct the conditional tree with prefix paths of a node in correlatedPatternTree
+
+        :param prefix : it represents the prefix items of a Node
+        :type prefix : list
+        :param mapSupportBeta : it represents the items with their supports
+        :param mapSupportBeta : dictionary
+        :param minSup : to check the item meets with minSup
+        :param minSup : float
+        """
+        pathCount = prefix[0].counter
+        current = self.root
+        prefix.reverse()
+        for i in range(0, len(prefix) - 1):
+            pathItem = prefix[i]
+            if mapSupportBeta.get(pathItem.itemId) >= minSup:
+                child = current.getChild(pathItem.itemId)
+                if child is None:
+                    newNode = _Node()
+                    newNode.itemId = pathItem.itemId
+                    newNode.parent = current
+                    newNode.counter = pathCount
+                    current.child.append(newNode)
+                    current = newNode
+                    self.fixNodeLinks(pathItem.itemId, newNode)
                 else:
-                    count[j] = support[i]
-        updatedDict = {}
-        updatedDict = {k: v for k, v in count.items() if v >= _expSup}
-        count = 0
-        for p in condPatterns:
-            p1 = [v for v in p if v in updatedDict]
-            trans = sorted(p1, key=lambda x: updatedDict[x], reverse=True)
-            if len(trans) > 0:
-                pat.append(trans)
-                sup.append(support[count])
-                count += 1
-        return pat, sup, updatedDict
-
-    def generatePatterns(self, prefix):
-        """generates the patterns
-            :param prefix : forms the combination of items
-            :type prefix : list
-        """
-
-        global _finalPatterns, _expSup, _expWSup, _weights
-        for i in sorted(self.summaries, key=lambda x: (self.info.get(x))):
-            pattern = prefix[:]
-            pattern.append(i)
-            weight = 0
-            for k in pattern:
-                weight = weight + _weights[k]
-            weight = weight/len(pattern)
-            if self.info.get(i) >= _expSup and self.info.get(i) * weight >= _expWSup:
-                _finalPatterns[tuple(pattern)] = self.info.get(i)
-                patterns, support, info = self.conditionalPatterns(i)
-                conditionalTree = _Tree()
-                conditionalTree.info = info.copy()
-                for pat in range(len(patterns)):
-                    conditionalTree.addConditionalPattern(patterns[pat], support[pat])
-                if len(patterns) > 0:
-                    conditionalTree.generatePatterns(pattern)
-            self.removeNode(i)
+                    child.counter += pathCount
+                    current = child
 
 
-class WUFIM(_ab._weightedFrequentPatterns):
+class CoMine(_ab._correlatedPatterns):
     """
-    Description:
-    -------------
-        It is one of the algorithm to discover weighted frequent patterns in a uncertain transactional database
-        using PUF-Tree.
-
-    Reference:
-    ------------
-        Efficient Mining of Weighted Frequent Itemsets in Uncertain Databases, In book: Machine Learning and Data Mining in Pattern Recognition
-        Chun-Wei Jerry Lin, Wensheng Gan, Philippe Fournier Viger, Tzung-Pei Hong
-
-    Attributes:
-    ------------
-        iFile : file
-            Name of the Input file or path of the input file
-        wFile : file
-            Name of the Input file or path of the input file
-        oFile : file
-            Name of the output file or path of the output file
-        minSup: float or int or str
-            The user can specify minSup either in count or proportion of database size.
-            If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
-            Otherwise, it will be treated as float.
-            Example: minSup=10 will be treated as integer, while minSup=10.0 will be treated as float
-        sep : str
-            This variable is used to distinguish items from one another in a transaction. The default seperator is tab space or \t.
-            However, the users can override their default separator.
+    :Description: CoMine is one of the fundamental algorithm to discover correlated  patterns in a transactional database. It is based on the traditional FP-Growth algorithm. This algorithm uses depth-first search technique to find all correlated patterns in a transactional database.
+
+    :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
+
+    :param  iFile: str :
+                   Name of the Input file to mine complete set of correlated patterns
+    :param  oFile: str :
+                   Name of the output file to store complete set of correlated patterns
+    :param  minSup: int or float or str :
+                   The user can specify minSup either in count or proportion of database size. If the program detects the data type of minSup is integer, then it treats minSup is expressed in count.
+    :param minAllConf: float :
+                    The user can specify minAllConf values within the range (0, 1).
+    :param  sep: str :
+                   This variable is used to distinguish items from one another in a transaction. The default seperator is tab space. However, the users can override their default separator.
+
+
+    :Attributes:
+
         memoryUSS : float
             To store the total amount of USS memory consumed by the program
         memoryRSS : float
             To store the total amount of RSS memory consumed by the program
         startTime:float
             To record the start time of the mining process
         endTime:float
             To record the completion time of the mining process
+        minSup : int
+            The user given minSup
+        minAllConf: float
+            The user given minimum all confidence Ratio(should be in range of 0 to 1)
         Database : list
             To store the transactions of a database in list
         mapSupport : Dictionary
             To maintain the information of item and their frequency
         lno : int
-            To represent the total no of transaction
+            it represents the total no of transactions
         tree : class
-            To represents the Tree class
+            it represents the Tree class
         itemSetCount : int
-            To represents the total no of patterns
+            it represents the total no of patterns
         finalPatterns : dict
-            To store the complete patterns
-    Methods:
-    ---------
-        startMine()
-            Mining process will start from here
-        getPatterns()
-            Complete set of patterns will be retrieved with this function
-        save(oFile)
-            Complete set of frequent patterns will be loaded in to a output file
-        getPatternsAsDataFrame()
-            Complete set of frequent patterns will be loaded in to a dataframe
-        getMemoryUSS()
-            Total amount of USS memory consumed by the mining process will be retrieved from this function
-        getMemoryRSS()
-            Total amount of RSS memory consumed by the mining process will be retrieved from this function
-        getRuntime()
-            Total amount of runtime taken by the mining process will be retrieved from this function
-        creatingItemSets(fileName)
-            Scans the dataset and stores in a list format
-        frequentOneItem()
-            Extracts the one-length frequent patterns from database
-        updateTransactions()
-            Update the transactions by removing non-frequent items and sort the Database by item decreased support
-        buildTree()
-            After updating the Database, remaining items will be added into the tree by setting root node as null
-        convert()
-            to convert the user specified value
-        startMine()
-            Mining process will start from this function
+            it represents to store the patterns
+        itemSetBuffer : list
+            it represents the store the items in mining
+        maxPatternLength : int
+           it represents the constraint for pattern length
+
 
     **Methods to execute code on terminal**
+    ----------------------------------------
 
-        Format:
-                  >>>  python3 WUFIM.py <inputFile> <outputFile> <minSup>
-        Example:
-                  >>>  python3 WUFIM.py sampleTDB.txt patterns.txt 3
+            Format:
+                      >>> python3 CoMine.py <inputFile> <outputFile> <minSup> <minAllConf> <sep>
+            Example:
+                      >>>  python3 CoMine.py sampleTDB.txt output.txt 0.25 0.2
 
-                 .. note:: minSup  will be considered in support count or frequency
+                     .. note:: minSup will be considered in percentage of database transactions
 
     **Importing this algorithm into a python program**
+    --------------------------------------------------------------------------------
+    .. code-block:: python
 
-.. code-block:: python
+            from PAMI.correlatedPattern.basic import CoMine as alg
 
-        from PAMI.weightedUncertainFrequentPattern.basic import WFIM as alg
+            obj = alg.CoMine(iFile, minSup, minAllConf,sep)
 
-        obj = alg.WFIM(iFile, wFile, expSup, expWSup)
+            obj.startMine()
 
-        obj.startMine()
+            patterns = obj.getPatterns()
 
-        Patterns = obj.getPatterns()
+            print("Total number of  Patterns:", len(patterns))
 
-        print("Total number of  Patterns:", len(Patterns))
+            obj.savePatterns(oFile)
 
-        obj.savePatterns(oFile)
+            df = obj.getPatternsAsDataFrame()
 
-        Df = obj.getPatternsAsDataFrame()
+            memUSS = obj.getMemoryUSS()
 
-        memUSS = obj.getMemoryUSS()
+            print("Total Memory in USS:", memUSS)
 
-        print("Total Memory in USS:", memUSS)
+            memRSS = obj.getMemoryRSS()
 
-        memRSS = obj.getMemoryRSS()
+            print("Total Memory in RSS", memRSS)
 
-        print("Total Memory in RSS", memRSS)
+            run = obj.getRuntime()
 
-        run = obj.getRuntime()
+            print("Total ExecutionTime in seconds:", run)
+
+    **Credits:**
+    ----------------------------------------
+             The complete program was written by B.Sai Chitra under the supervision of Professor Rage Uday Kiran.
+
+        """
 
-        print("Total ExecutionTime in seconds:", run)
-   """
     _startTime = float()
     _endTime = float()
-    _minSup = str()
+    _minSup = float()
     _finalPatterns = {}
     _iFile = " "
-    _wFile = " "
     _oFile = " "
-    _sep = " "
     _memoryUSS = float()
     _memoryRSS = float()
+    _minAllConf = 0.0
     _Database = []
-    _rank = {}
-    _expSup = float()
-    _expWSup = float()
+    _mapSupport = {}
+    _lno = 0
+    _tree = str()
+    _itemSetBuffer = None
+    _fpNodeTempBuffer = []
+    _itemSetCount = 0
+    _maxPatternLength = 1000
+    _sep = "\t"
+
+    def __init__(self, iFile, minSup, minAllConf, sep="\t"):
+        """param iFile: give the input file
+           type iFile: str or DataFrame or url
+           param minSup: minimum support
+           type minSup:   int or float
+           param sep: Delimiter of input file
+           type sep: str
+        """
 
-    def __init__(self, iFile, wFile, expSup, expWSup, sep='\t'):
-        super().__init__(iFile, wFile, expSup, expWSup, sep)
+        super().__init__(iFile, minSup, minAllConf, sep)
 
     def _creatingItemSets(self):
         """
-            Scans the uncertain transactional dataset
-        """
+            Storing the complete transactions of the database/input file in a database variable
+
+            """
         self._Database = []
         if isinstance(self._iFile, _ab._pd.DataFrame):
-            uncertain, data = [], []
             if self._iFile.empty:
                 print("its empty..")
             i = self._iFile.columns.values.tolist()
             if 'Transactions' in i:
                 self._Database = self._iFile['Transactions'].tolist()
-            if 'uncertain' in i:
-                uncertain = self._iFile['uncertain'].tolist()
-            for k in range(len(data)):
-                tr = []
-                for j in range(len(data[k])):
-                    product = _Item(data[k][j], uncertain[k][j])
-                    tr.append(product)
-                self._Database.append(tr)
-
-            # print(self.Database)
         if isinstance(self._iFile, str):
             if _ab._validators.url(self._iFile):
                 data = _ab._urlopen(self._iFile)
                 for line in data:
-                    line = line.decode("utf-8")
-                    line = line.strip()
-                    line = [i for i in line.split(':')]
-                    temp1 = [i.rstrip() for i in line[0].split(self._sep)]
-                    temp2 = [i.rstrip() for i in line[1].split(self._sep)]
-                    temp1 = [x for x in temp1 if x]
-                    temp2 = [x for x in temp2 if x]
-                    tr = []
-                    for i in range(len(temp1)):
-                        item = temp1[i]
-                        probability = float(temp2[i])
-                        product = _Item(item, probability)
-                        tr.append(product)
-                    self._Database.append(tr)
-            else:
-                try:
-                    with open(self._iFile, 'r') as f:
-                        for line in f:
-                            line = line.strip()
-                            line = [i for i in line.split(':')]
-                            temp1 = [i.rstrip() for i in line[0].split(self._sep)]
-                            temp2 = [i.rstrip() for i in line[1].split(self._sep)]
-                            temp1 = [x for x in temp1 if x]
-                            temp2 = [x for x in temp2 if x]
-                            tr = []
-                            for i in range(len(temp1)):
-                                item = temp1[i]
-                                probability = float(temp2[i])
-                                product = _Item(item, probability)
-                                tr.append(product)
-                            self._Database.append(tr)
-                except IOError:
-                    print("File Not Found")
-
-    def _scanningWeights(self):
-        """
-            Scans the uncertain transactional dataset
-        """
-        self._weights = {}
-        if isinstance(self._wFile, _ab._pd.DataFrame):
-            weights, data = [], []
-            if self._wFile.empty:
-                print("its empty..")
-            i = self._wFile.columns.values.tolist()
-            if 'items' in i:
-                data = self._wFile['items'].tolist()
-            if 'weights' in i:
-                weights = self._wFile['weights'].tolist()
-            for k in range(len(data)):
-                self._weights[data[k]] = int(float(weights[k]))
-
-            # print(self.Database)
-        if isinstance(self._wFile, str):
-            if _ab._validators.url(self._wFile):
-                data = _ab._urlopen(self._wFile)
-                for line in data:
                     line.strip()
                     line = line.decode("utf-8")
                     temp = [i.rstrip() for i in line.split(self._sep)]
                     temp = [x for x in temp if x]
-                    self._weights[temp[0]] = int(float(temp[1]))
+                    self._Database.append(temp)
             else:
                 try:
-                    with open(self._wFile, 'r') as f:
+                    with open(self._iFile, 'r', encoding='utf-8') as f:
                         for line in f:
+                            line.strip()
                             temp = [i.rstrip() for i in line.split(self._sep)]
                             temp = [x for x in temp if x]
-                            self._weights[temp[0]] = float(temp[1])
+                            self._Database.append(temp)
                 except IOError:
                     print("File Not Found")
+                    quit()
 
-    def _frequentOneItem(self):
-        """takes the self.Database and calculates the support of each item in the dataset and assign the
-            ranks to the items by decreasing support and returns the frequent items list
-                :param self.Database : it represents the one self.Database in database
-                :type self.Database : list
+    def _getRatio(self, prefix, prefixLength, s):
         """
+            A Function to get itemSet Ratio
+            :param prefix:the path
+            :type prefix: list
+            :param prefixLength: length
+            :type prefixLength:int
+            :s :current ratio
+            :type s:float
+            :return: minAllConf of prefix
+            :rtype:float
+        """
+        maximums = 0
+        for ele in range(prefixLength):
+            i = prefix[ele]
+            if maximums < self._mapSupport.get(i):
+                maximums = self._mapSupport.get(i)
+        return s / maximums
 
-        mapSupport = {}
+    def _correlatedOneItem(self):
+        """
+            Generating One correlated item
+        """
+        self._mapSupport = {}
         for i in self._Database:
             for j in i:
-                if j.item not in mapSupport:
-                    if self._weights.get(j.item) is not None:
-                        mapSupport[j.item] = [j.probability, self._weights[j.item]]
+                if j not in self._mapSupport:
+                    self._mapSupport[j] = 1
                 else:
-                    mapSupport[j.item][0] += j.probability
-        mapSupport = {k: v[0] for k, v in mapSupport.items() if v[0] >= self._expSup and v[0] * v[1] >= self._expWSup}
-        plist = [k for k, v in sorted(mapSupport.items(), key=lambda x: x[1], reverse=True)]
-        self.rank = dict([(index, item) for (item, index) in enumerate(plist)])
-        return mapSupport, plist
-
-    @staticmethod
-    def _buildTree(data, info):
-        """it takes the self.Database and support of each item and construct the main tree with setting root
-            node as null
-                :param data : it represents the one self.Database in database
-                :type data : list
-                :param info : it represents the support of each item
-                :type info : dictionary
-        """
-
-        rootNode = _Tree()
-        rootNode.info = info.copy()
-        for i in range(len(data)):
-            rootNode.addTransaction(data[i])
-        return rootNode
-
-    def _updateTransactions(self, dict1):
-        """remove the items which are not frequent from self.Database and updates the self.Database with rank of items
-            :param dict1 : frequent items with support
-            :type dict1 : dictionary
-        """
-
-        list1 = []
-        for tr in self._Database:
-            list2 = []
-            for i in range(0, len(tr)):
-                if tr[i].item in dict1:
-                    list2.append(tr[i])
-            if len(list2) >= 2:
-                basket = list2
-                basket.sort(key=lambda val: self.rank[val.item])
-                list2 = basket
-                list1.append(list2)
-        return list1
-
-    @staticmethod
-    def _check(i, x):
-        """To check the presence of item or pattern in transaction
-                :param x: it represents the pattern
-                :type x : list
-                :param i : represents the uncertain self.Database
-                :type i : list
-        """
-
-        # This method taken a transaction as input and returns the tree
-        for m in x:
-            k = 0
-            for n in i:
-                if m == n.item:
-                    k += 1
-            if k == 0:
-                return 0
-        return 1
+                    self._mapSupport[j] += 1
+
+    def _saveItemSet(self, prefix, prefixLength, support):
+        """
+        To save the correlated patterns mined form correlatedPatternTree
 
+        :param prefix: the correlated pattern
+        :type prefix: list
+        :param prefixLength : the length of a correlated pattern
+        :type prefixLength : int
+        :param support: the support of a pattern
+        :type support :  int
+        :The correlated patterns were stored in a global variable finalPatterns
+        """
+        all_conf = self._getRatio(prefix, prefixLength, support)
+        if all_conf < self._minAllConf:
+            return
+        l = []
+        for i in range(prefixLength):
+            l.append(prefix[i])
+        self._itemSetCount += 1
+        self._finalPatterns[tuple(l)] = [support, all_conf]
+    
     def _convert(self, value):
         """
-        To convert the type of user specified minSup value
-            :param value: user specified minSup value
-            :return: converted type minSup value
+        to convert the type of user specified minSup value
+        :param value: user specified minSup value
+        :return: converted type
         """
         if type(value) is int:
             value = int(value)
         if type(value) is float:
             value = (len(self._Database) * value)
         if type(value) is str:
             if '.' in value:
+                value = float(value)
                 value = (len(self._Database) * value)
             else:
                 value = int(value)
         return value
 
-    def _removeFalsePositives(self):
-        """
-            To remove the false positive patterns generated in frequent patterns
-            :return: patterns with accurate probability
-        """
-        global _finalPatterns
-        periods = {}
-        for i in self._Database:
-            for x, y in _finalPatterns.items():
-                if len(x) == 1:
-                    periods[x] = y
-                else:
-                    s = 1
-                    check = self._check(i, x)
-                    if check == 1:
-                        for j in i:
-                            if j.item in x:
-                                s *= j.probability
-                        if x in periods:
-                            periods[x] += s
-                        else:
-                            periods[x] = s
-        for x, y in periods.items():
-            weight = 0
-            for i in x:
-                weight += self._weights[i]
-            weight = weight / len(x)
-            if weight * y >= self._expWSup:
-                sample = str()
-                for i in x:
-                    sample = sample + i + "\t"
-                self._finalPatterns[sample] = y
+    def _saveAllCombinations(self, tempBuffer, s, position, prefix, prefixLength):
+        """Generating all the combinations for items in single branch in correlatedPatternTree
 
+        :param tempBuffer: items in a single branch
+        :type tempBuffer: list
+        :param s : support at leaf node of a branch
+        :param position : the length of a tempBuffer
+        :type position : int
+        :param prefix : it represents the list of leaf node
+        :type prefix : list
+        :param prefixLength : the length of prefix
+        :type prefixLength :int
+        
+        """
+        max1 = 1 << position
+        for i in range(1, max1):
+            newPrefixLength = prefixLength
+            for j in range(position):
+                isSet = i & (1 << j)
+                if isSet > 0:
+                    prefix.insert(newPrefixLength, tempBuffer[j].itemId)
+                    newPrefixLength += 1
+            self._saveItemSet(prefix, newPrefixLength, s)
+
+    def _correlatedPatternGrowthGenerate(self, correlatedPatternTree, prefix, prefixLength, mapSupport):
+        """
+
+        Mining the fp tree
+
+        :param correlatedPatternTree: it represents the correlatedPatternTree
+        :type correlatedPatternTree: class Tree
+        :param prefix : it represents an empty list and store the patterns that are mined
+        :type prefix : list
+        :param prefixLength : the length of prefix
+        :type prefixLength :int
+        :param mapSupport : it represents the support of item
+        :type mapSupport : dictionary
+
+        """
+
+        singlePath = True
+        position = 0
+        s = 0
+        if len(correlatedPatternTree.root.child) > 1:
+            singlePath = False
+        else:
+            currentNode = correlatedPatternTree.root.child[0]
+            while True:
+                if len(currentNode.child) > 1:
+                    singlePath = False
+                    break
+                self._fpNodeTempBuffer.insert(position, currentNode)
+                s = currentNode.counter
+                position += 1
+                if len(currentNode.child) == 0:
+                    break
+                currentNode = currentNode.child[0]
+        if singlePath is True:
+            self._saveAllCombinations(self._fpNodeTempBuffer, s, position, prefix, prefixLength)
+        else:
+            for i in reversed(correlatedPatternTree.headerList):
+                item = i
+                support = mapSupport[i]
+                betaSupport = support
+                prefix.insert(prefixLength, item)
+                self._saveItemSet(prefix, prefixLength + 1, betaSupport)
+                if prefixLength + 1 < self._maxPatternLength:
+                    prefixPaths = []
+                    path = correlatedPatternTree.mapItemNodes.get(item)
+                    mapSupportBeta = {}
+                    while path is not None:
+                        if path.parent.itemId != -1:
+                            prefixPath = []
+                            prefixPath.append(path)
+                            pathCount = path.counter
+                            parent1 = path.parent
+                            while parent1.itemId != -1:
+                                prefixPath.append(parent1)
+                                if mapSupportBeta.get(parent1.itemId) is None:
+                                    mapSupportBeta[parent1.itemId] = pathCount
+                                else:
+                                    mapSupportBeta[parent1.itemId] = mapSupportBeta[parent1.itemId] + pathCount
+                                parent1 = parent1.parent
+                            prefixPaths.append(prefixPath)
+                        path = path.nodeLink
+                    treeBeta = _Tree()
+                    for k in prefixPaths:
+                        treeBeta.addPrefixPath(k, mapSupportBeta, self._minSup)
+                    if len(treeBeta.root.child) > 0:
+                        treeBeta.createHeaderList(mapSupportBeta, self._minSup)
+                        self._correlatedPatternGrowthGenerate(treeBeta, prefix, prefixLength + 1, mapSupportBeta)
+    
     def startMine(self):
-        """Main method where the patterns are mined by constructing tree and remove the remove the false patterns
-            by counting the original support of a patterns
         """
-        global _expSup, _expWSup, _weights, _finalPatterns
+        main method to start
+
+        """
         self._startTime = _ab._time.time()
-        self._Database, self._weights = [], {}
+        if self._iFile is None:
+            raise Exception("Please enter the file path or file name:")
         self._creatingItemSets()
-        self._scanningWeights()
-        _weights = self._weights
-        self._expSup = float(self._expSup)
-        self._expWSup = float(self._expWSup)
-        _expSup = self._expSup
-        _expWSup = self._expWSup
+        self._minSup = self._convert(self._minSup)
+        self._tree = _Tree()
         self._finalPatterns = {}
-        mapSupport, plist = self._frequentOneItem()
-        self.Database1 = self._updateTransactions(mapSupport)
-        info = {k: v for k, v in mapSupport.items()}
-        Tree1 = self._buildTree(self.Database1, info)
-        Tree1.generatePatterns([])
-        self._removeFalsePositives()
-        print("Weighted Frequent patterns were generated  successfully using WUFIM algorithm")
+        self._correlatedOneItem()
+        self._mapSupport = {k: v for k, v in self._mapSupport.items() if v >= self._minSup}
+        _itemSetBuffer = [k for k, v in sorted(self._mapSupport.items(), key=lambda x: x[1], reverse=True)]
+        for i in self._Database:
+            _transaction = []
+            for j in i:
+                if j in _itemSetBuffer:
+                    _transaction.append(j)
+            _transaction.sort(key=lambda val: self._mapSupport[val], reverse=True)
+            self._tree.addTransaction(_transaction)
+        self._tree.createHeaderList(self._mapSupport, self._minSup)
+        if len(self._tree.headerList) > 0:
+            self._itemSetBuffer = []
+            self._correlatedPatternGrowthGenerate(self._tree, self._itemSetBuffer, 0, self._mapSupport)
+        print("Correlated patterns were generated successfully using CoMine algorithm")
         self._endTime = _ab._time.time()
-        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = float()
-        self.memoryRSS = float()
+        self._memoryRSS = float()
+        process = _ab._psutil.Process(_ab._os.getpid())
         self._memoryUSS = process.memory_full_info().uss
-        self.memoryRSS = process.memory_info().rss
+        self._memoryRSS = process.memory_info().rss
 
     def getMemoryUSS(self):
-        """Total amount of USS memory consumed by the mining process will be retrieved from this function
+        """
+        Total amount of USS memory consumed by the mining process will be retrieved from this function
+
         :return: returning USS memory consumed by the mining process
         :rtype: float
         """
 
         return self._memoryUSS
 
     def getMemoryRSS(self):
-        """Total amount of RSS memory consumed by the mining process will be retrieved from this function
+        """
+        Total amount of RSS memory consumed by the mining process will be retrieved from this function
+
         :return: returning RSS memory consumed by the mining process
         :rtype: float
         """
 
-        return self.memoryRSS
+        return self._memoryRSS
 
     def getRuntime(self):
-        """Calculating the total amount of runtime taken by the mining process
+        """
+        Calculating the total amount of runtime taken by the mining process
+
+
         :return: returning total amount of runtime taken by the mining process
         :rtype: float
         """
 
         return self._endTime - self._startTime
 
     def getPatternsAsDataFrame(self):
-        """Storing final frequent patterns in a dataframe
-        :return: returning frequent patterns in a dataframe
+        """
+
+        Storing final correlated patterns in a dataframe
+
+        :return: returning correlated patterns in a dataframe
         :rtype: pd.DataFrame
         """
 
         dataframe = {}
         data = []
         for a, b in self._finalPatterns.items():
-            s = str()
+            pat = " "
             for i in a:
-                s = s + i + " "
-            data.append([s, b])
-            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support'])
+                pat += str(i) + " "
+            data.append([pat, b[0], b[1]])
+            dataframe = _ab._pd.DataFrame(data, columns=['Patterns', 'Support', 'Confidence'])
         return dataframe
 
     def save(self, outFile):
-        """Complete set of frequent patterns will be loaded in to a output file
-        :param outFile: name of the output file
+        """
+        Complete set of correlated patterns will be saved into an output file
+
+        :param outFile: name of the outputfile
         :type outFile: file
         """
-        self.oFile = outFile
-        writer = open(self.oFile, 'w+')
+        self._oFile = outFile
+        writer = open(self._oFile, 'w+')
         for x, y in self._finalPatterns.items():
-            s = str()
+            pat = ""
             for i in x:
-                s = s + i + "\t"
-            s1 = s.strip() + ":" + str(y)
-            writer.write("%s \n" % s1)
+                pat += str(i) + "\t"
+            patternsAndSupport = pat.strip() + ":" + str(y[0]) + ":" + str(y[1])
+            writer.write("%s \n" % patternsAndSupport)
 
     def getPatterns(self):
-        """ Function to send the set of frequent patterns after completion of the mining process
-        :return: returning frequent patterns
+        """
+        Function to send the set of correlated patterns after completion of the mining process
+
+        :return: returning correlated patterns
         :rtype: dict
         """
         return self._finalPatterns
 
     def printResults(self):
-        print("Total number of  Weighted Uncertain Frequent Patterns:", len(self.getPatterns()))
+        """
+
+        function to print the result after completing the process
+
+        """
+        print("Total number of Correlated Patterns:", len(self.getPatterns()))
         print("Total Memory in USS:", self.getMemoryUSS())
         print("Total Memory in RSS", self.getMemoryRSS())
         print("Total ExecutionTime in ms:",  self.getRuntime())
 
-
 if __name__ == "__main__":
     _ap = str()
-    if len(_ab._sys.argv) == 6 or len(_ab._sys.argv) == 7:
-        if len(_ab._sys.argv) == 7:
-            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5], _ab._sys.argv[6])
+    if len(_ab._sys.argv) == 5 or len(_ab._sys.argv) == 6:
         if len(_ab._sys.argv) == 6:
-            _ap = WUFIM(_ab._sys.argv[1], _ab._sys.argv[3], _ab._sys.argv[4], _ab._sys.argv[5])
+            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]), _ab._sys.argv[5])
+        if len(_ab._sys.argv) == 5:
+            _ap = CoMine(_ab._sys.argv[1], _ab._sys.argv[3], float(_ab._sys.argv[4]))
         _ap.startMine()
-        print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
+        print("Total number of Correlated-Frequent Patterns:", len(_ap.getPatterns()))
         _ap.save(_ab._sys.argv[2])
         print("Total Memory in USS:", _ap.getMemoryUSS())
         print("Total Memory in RSS", _ap.getMemoryRSS())
-        print("Total ExecutionTime in ms:", _ap.getRuntime())
+        print("Total ExecutionTime in seconds:", _ap.getRuntime())
     else:
-        for k in [120, 140, 160, 180, 200]:
-            _ap = WUFIM('/Users/likhitha/Downloads/uncertainTransaction_T10I4D200K.csv', '/Users/likhitha/Downloads/T10_weights.txt',
-                        k, 500, '\t')
-            _ap.startMine()
-            print("Total number of Weighted Uncertain Frequent Patterns:", len(_ap.getPatterns()))
-            _ap.save('/Users/likhitha/Downloads/WUFIM_output.txt')
-            print("Total Memory in USS:", _ap.getMemoryUSS())
-            print("Total Memory in RSS", _ap.getMemoryRSS())
-            print("Total ExecutionTime in ms:", _ap.getRuntime())
         print("Error! The number of input parameters do not match the total number of parameters provided")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.8.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.7/pami.egg-info/SOURCES.txt` & `pami-2023.8.1/pami.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 PAMI/AssociationRules/basic/ARWithConfidence.py
 PAMI/AssociationRules/basic/ARWithLeverage.py
 PAMI/AssociationRules/basic/ARWithLift.py
 PAMI/AssociationRules/basic/RuleMiner.py
 PAMI/AssociationRules/basic/__init__.py
 PAMI/AssociationRules/basic/abstract.py
 PAMI/correlatedPattern/__init__.py
-PAMI/correlatedPattern/basic/CPGrowth.py
-PAMI/correlatedPattern/basic/CPGrowthPlus.py
+PAMI/correlatedPattern/basic/CoMine.py
+PAMI/correlatedPattern/basic/CoMinePlus.py
 PAMI/correlatedPattern/basic/__init__.py
 PAMI/correlatedPattern/basic/abstract.py
-PAMI/coveragePatterns/__init__.py
-PAMI/coveragePatterns/basic/CMine.py
-PAMI/coveragePatterns/basic/CPPG.py
-PAMI/coveragePatterns/basic/__init__.py
-PAMI/coveragePatterns/basic/abstract.py
+PAMI/coveragePattern/__init__.py
+PAMI/coveragePattern/basic/CMine.py
+PAMI/coveragePattern/basic/CPPG.py
+PAMI/coveragePattern/basic/__init__.py
+PAMI/coveragePattern/basic/abstract.py
 PAMI/extras/__init__.py
 PAMI/extras/generateLatexGraphFile.py
 PAMI/extras/plotPointOnMap.py
 PAMI/extras/plotPointOnMap_dump.py
 PAMI/extras/scatterPlotSpatialPoints.py
 PAMI/extras/topKPatterns.py
 PAMI/extras/uncertaindb_convert.py
@@ -36,14 +36,15 @@
 PAMI/extras/DF2DB/sparseDF2DB.py
 PAMI/extras/DF2DB/sparseDF2DBPlus.py
 PAMI/extras/calculateMISValues/__init__.py
 PAMI/extras/calculateMISValues/usingBeta.py
 PAMI/extras/calculateMISValues/usingSD.py
 PAMI/extras/dbStats/__init__.py
 PAMI/extras/dbStats/fuzzyDatabaseStats.py
+PAMI/extras/dbStats/sequencialDatabaseStats.py
 PAMI/extras/dbStats/temporalDatabaseStats.py
 PAMI/extras/dbStats/transactionalDatabaseStats.py
 PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
 PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
 PAMI/extras/dbStats/utilityDatabaseStats.py
 PAMI/extras/fuzzyTransformation/__init__.py
 PAMI/extras/fuzzyTransformation/abstract.py
@@ -61,27 +62,27 @@
 PAMI/extras/graph/plotLineGraphsFromDataFrame.py
 PAMI/extras/graph/visualizePatterns.py
 PAMI/extras/image2Database/__init__.py
 PAMI/extras/imageProcessing/__init__.py
 PAMI/extras/imageProcessing/imagery2Databases.py
 PAMI/extras/neighbours/__init__.py
 PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+PAMI/extras/neighbours/findNeighboursUsingGeodesic.py
 PAMI/extras/syntheticDatabaseGenerator/__init__.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
 PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
 PAMI/faultTolerantFrequentPattern/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
 PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
-PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
 PAMI/faultTolerantFrequentPattern/basic/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/abstract.py
 PAMI/frequentPattern/__init__.py
 PAMI/frequentPattern/basic/Apriori.py
 PAMI/frequentPattern/basic/ECLAT.py
 PAMI/frequentPattern/basic/ECLATDiffset.py
 PAMI/frequentPattern/basic/ECLATbitset.py
@@ -107,73 +108,75 @@
 PAMI/frequentPattern/pyspark/abstract.py
 PAMI/frequentPattern/pyspark/parallelApriori.py
 PAMI/frequentPattern/pyspark/parallelECLAT.py
 PAMI/frequentPattern/pyspark/parallelFPGrowth.py
 PAMI/frequentPattern/topk/FAE.py
 PAMI/frequentPattern/topk/__init__.py
 PAMI/frequentPattern/topk/abstract.py
-PAMI/frequentSpatialPattern/__init__.py
-PAMI/frequentSpatialPattern/basic/FSPGrowth.py
-PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
-PAMI/frequentSpatialPattern/basic/__init__.py
-PAMI/frequentSpatialPattern/basic/abstract.py
 PAMI/fuzzyCorrelatedPattern/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
 PAMI/fuzzyCorrelatedPattern/basic/__init__.py
 PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-PAMI/fuzzyFrequentPatterns/__init__.py
-PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
-PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
-PAMI/fuzzyFrequentPatterns/basic/__init__.py
-PAMI/fuzzyFrequentPatterns/basic/abstract.py
-PAMI/fuzzyFrequentSpatialPattern/__init__.py
-PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
-PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
-PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
-PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
-PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+PAMI/fuzzyFrequentPattern/__init__.py
+PAMI/fuzzyFrequentPattern/basic/FFIMiner.py
+PAMI/fuzzyFrequentPattern/basic/FFIMiner_old.py
+PAMI/fuzzyFrequentPattern/basic/__init__.py
+PAMI/fuzzyFrequentPattern/basic/abstract.py
+PAMI/fuzzyGeoreferencedFrequentPattern/__init__.py
+PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner.py
+PAMI/fuzzyGeoreferencedFrequentPattern/basic/FFSPMiner_old.py
+PAMI/fuzzyGeoreferencedFrequentPattern/basic/__init__.py
+PAMI/fuzzyGeoreferencedFrequentPattern/basic/abstract.py
+PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/__init__.py
+PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner.py
+PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/__init__.py
+PAMI/fuzzyGeoreferencedPeriodicFrequentPattern/basic/abstract.py
 PAMI/fuzzyPeriodicFrequentPattern/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
 PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
-PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
-PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
-PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-PAMI/geoReferencedFrequentPattern/GFPGrowth.py
-PAMI/geoReferencedFrequentPattern/__init__.py
-PAMI/geoReferencedFrequentPattern/abstract.py
 PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+PAMI/georeferencedFrequentPattern/__init__.py
+PAMI/georeferencedFrequentPattern/basic/FSPGrowth.py
+PAMI/georeferencedFrequentPattern/basic/SpatialECLAT.py
+PAMI/georeferencedFrequentPattern/basic/__init__.py
+PAMI/georeferencedFrequentPattern/basic/abstract.py
 PAMI/georeferencedFrequentSequencePattern/__init__.py
 PAMI/georeferencedFrequentSequencePattern/abstract.py
-PAMI/highUtilityFrequentPatterns/__init__.py
-PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
-PAMI/highUtilityFrequentPatterns/basic/__init__.py
-PAMI/highUtilityFrequentPatterns/basic/abstract.py
-PAMI/highUtilityFrequentSpatialPattern/__init__.py
-PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
-PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
-PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-PAMI/highUtilityPatterns/__init__.py
-PAMI/highUtilityPatterns/basic/EFIM.py
-PAMI/highUtilityPatterns/basic/HMiner.py
-PAMI/highUtilityPatterns/basic/UPGrowth.py
-PAMI/highUtilityPatterns/basic/__init__.py
-PAMI/highUtilityPatterns/basic/abstract.py
-PAMI/highUtilityPatterns/basic/efimParallel.py
-PAMI/highUtilityPatterns/parallel/__init__.py
-PAMI/highUtilityPatterns/parallel/abstract.py
-PAMI/highUtilityPatterns/parallel/efimparallel.py
+PAMI/georeferencedPartialPeriodicPattern/__init__.py
+PAMI/georeferencedPartialPeriodicPattern/basic/STEclat.py
+PAMI/georeferencedPartialPeriodicPattern/basic/__init__.py
+PAMI/georeferencedPartialPeriodicPattern/basic/abstract.py
+PAMI/highUtilityFrequentPattern/__init__.py
+PAMI/highUtilityFrequentPattern/basic/HUFIM.py
+PAMI/highUtilityFrequentPattern/basic/__init__.py
+PAMI/highUtilityFrequentPattern/basic/abstract.py
+PAMI/highUtilityGeoreferencedFrequentPattern/__init__.py
+PAMI/highUtilityGeoreferencedFrequentPattern/basic/SHUFIM.py
+PAMI/highUtilityGeoreferencedFrequentPattern/basic/__init__.py
+PAMI/highUtilityGeoreferencedFrequentPattern/basic/abstract.py
+PAMI/highUtilityPattern/__init__.py
+PAMI/highUtilityPattern/basic/EFIM.py
+PAMI/highUtilityPattern/basic/HMiner.py
+PAMI/highUtilityPattern/basic/UPGrowth.py
+PAMI/highUtilityPattern/basic/__init__.py
+PAMI/highUtilityPattern/basic/abstract.py
+PAMI/highUtilityPattern/basic/efimParallel.py
+PAMI/highUtilityPattern/parallel/__init__.py
+PAMI/highUtilityPattern/parallel/abstract.py
+PAMI/highUtilityPattern/parallel/efimparallel.py
+PAMI/highUtilityPatternsInStreams/HUPMS.py
+PAMI/highUtilityPatternsInStreams/SHUGrowth.py
+PAMI/highUtilityPatternsInStreams/__init__.py
+PAMI/highUtilityPatternsInStreams/abstract.py
 PAMI/highUtilitySpatialPattern/__init__.py
 PAMI/highUtilitySpatialPattern/abstract.py
 PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
 PAMI/highUtilitySpatialPattern/basic/SHUIM.py
 PAMI/highUtilitySpatialPattern/basic/__init__.py
 PAMI/highUtilitySpatialPattern/basic/abstract.py
 PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
@@ -204,24 +207,20 @@
 PAMI/partialPeriodicPattern/basic/abstract.py
 PAMI/partialPeriodicPattern/closed/PPPClose.py
 PAMI/partialPeriodicPattern/closed/__init__.py
 PAMI/partialPeriodicPattern/closed/abstract.py
 PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
 PAMI/partialPeriodicPattern/maximal/__init__.py
 PAMI/partialPeriodicPattern/maximal/abstract.py
-PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
-PAMI/partialPeriodicPattern/timeSeries/__init__.py
-PAMI/partialPeriodicPattern/timeSeries/abstract.py
 PAMI/partialPeriodicPattern/topk/__init__.py
 PAMI/partialPeriodicPattern/topk/abstract.py
 PAMI/partialPeriodicPattern/topk/k3PMiner.py
-PAMI/partialPeriodicSpatialPattern/__init__.py
-PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
-PAMI/partialPeriodicSpatialPattern/basic/__init__.py
-PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+PAMI/partialPeriodicPatternInMultipleTimeSeries/PPGrowth.py
+PAMI/partialPeriodicPatternInMultipleTimeSeries/__init__.py
+PAMI/partialPeriodicPatternInMultipleTimeSeries/abstract.py
 PAMI/periodicCorrelatedPattern/__init__.py
 PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
 PAMI/periodicCorrelatedPattern/basic/__init__.py
 PAMI/periodicCorrelatedPattern/basic/abstract.py
 PAMI/periodicFrequentPattern/__init__.py
 PAMI/periodicFrequentPattern/basic/PFECLAT.py
 PAMI/periodicFrequentPattern/basic/PFPGrowth.py
@@ -236,33 +235,37 @@
 PAMI/periodicFrequentPattern/cuda/__init__.py
 PAMI/periodicFrequentPattern/cuda/abstract.py
 PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
 PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
 PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
 PAMI/periodicFrequentPattern/maximal/__init__.py
 PAMI/periodicFrequentPattern/maximal/abstract.py
+PAMI/periodicFrequentPattern/pyspark/__init__.py
+PAMI/periodicFrequentPattern/pyspark/abstract.py
+PAMI/periodicFrequentPattern/pyspark/parallelPFPGrowth.py
 PAMI/periodicFrequentPattern/topk/__init__.py
 PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
 PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
 PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
 PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
 PAMI/recurringPattern/__init__.py
 PAMI/recurringPattern/basic/RPGrowth.py
 PAMI/recurringPattern/basic/__init__.py
 PAMI/recurringPattern/basic/abstract.py
-PAMI/relativeFrequentPatterns/__init__.py
-PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
-PAMI/relativeFrequentPatterns/basic/__init__.py
-PAMI/relativeFrequentPatterns/basic/abstract.py
-PAMI/relativeHighUtilityPatterns/__init__.py
-PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
-PAMI/relativeHighUtilityPatterns/basic/__init__.py
-PAMI/relativeHighUtilityPatterns/basic/abstract.py
+PAMI/relativeFrequentPattern/__init__.py
+PAMI/relativeFrequentPattern/basic/RSFPGrowth.py
+PAMI/relativeFrequentPattern/basic/__init__.py
+PAMI/relativeFrequentPattern/basic/abstract.py
+PAMI/relativeHighUtilityPattern/__init__.py
+PAMI/relativeHighUtilityPattern/basic/RHUIM.py
+PAMI/relativeHighUtilityPattern/basic/__init__.py
+PAMI/relativeHighUtilityPattern/basic/abstract.py
+PAMI/sequence/__init__.py
 PAMI/sequentialPatternMining/__init__.py
 PAMI/sequentialPatternMining/basic/SPADE.py
 PAMI/sequentialPatternMining/basic/__init__.py
 PAMI/sequentialPatternMining/basic/abstract.py
 PAMI/sequentialPatternMining/basic/prefixSpan.py
 PAMI/sequentialPatternMining/closed/__init__.py
 PAMI/sequentialPatternMining/closed/abstract.py
@@ -272,33 +275,31 @@
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
 PAMI/stablePeriodicFrequentPattern/basic/__init__.py
 PAMI/stablePeriodicFrequentPattern/basic/abstract.py
 PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
 PAMI/stablePeriodicFrequentPattern/topK/__init__.py
 PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-PAMI/streams/__init__.py
-PAMI/streams/frequentPatterns/__init__.py
-PAMI/streams/frequentPatterns/basic/FPStream.py
-PAMI/streams/frequentPatterns/basic/__init__.py
-PAMI/streams/frequentPatterns/basic/abstract.py
-PAMI/streams/highUtility/HUPMS.py
-PAMI/streams/highUtility/SHUGrowth.py
-PAMI/streams/highUtility/__init__.py
-PAMI/streams/highUtility/abstract.py
+PAMI/uncertainFaultTolerantFrequentPattern/VBFTMine.py
+PAMI/uncertainFaultTolerantFrequentPattern/__init__.py
+PAMI/uncertainFaultTolerantFrequentPattern/abstract.py
 PAMI/uncertainFrequentPattern/__init__.py
 PAMI/uncertainFrequentPattern/basic/CUFPTree.py
 PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
 PAMI/uncertainFrequentPattern/basic/TUFP.py
 PAMI/uncertainFrequentPattern/basic/TubeP.py
 PAMI/uncertainFrequentPattern/basic/TubeS.py
 PAMI/uncertainFrequentPattern/basic/UFGrowth.py
 PAMI/uncertainFrequentPattern/basic/UVECLAT.py
 PAMI/uncertainFrequentPattern/basic/__init__.py
 PAMI/uncertainFrequentPattern/basic/abstract.py
+PAMI/uncertainGeoreferencedFrequentPattern/__init__.py
+PAMI/uncertainGeoreferencedFrequentPattern/basic/GFPGrowth.py
+PAMI/uncertainGeoreferencedFrequentPattern/basic/__init__.py
+PAMI/uncertainGeoreferencedFrequentPattern/basic/abstract.py
 PAMI/uncertainPeriodicFrequentPattern/__init__.py
 PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
 PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
 PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
 PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
 PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
 PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
```

### Comparing `pami-2023.7.7/setup.py` & `pami-2023.8.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name = 'pami',
-    version = '2023.07.07',
-    author = 'Rage Uday Kiran',
-    author_email = 'uday.rage@gmail.com',
-    description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
-    long_description = long_description,
-    long_description_content_type = 'text/markdown',
+    name='pami',
+    version='2023.08.1',
+    author='Rage Uday Kiran',
+    author_email='uday.rage@gmail.com',
+    description='This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=setuptools.find_packages(),
-    url = 'https://github.com/udayRage/PAMI',
+    url='https://github.com/udayLab/PAMI',
     license='GPLv3',
     install_requires=[            # All necessary packages utilized by our PAMI software
         'psutil',
         'pandas',
         'plotly',
         'matplotlib',
         'resource',
         'validators',
         'urllib3',
         'Pillow',
         'numpy',
     ],
-    extras_require = {
-        'gpu':  ['cupy'],
+    extras_require={
+        'gpu':  ['cupy', 'pycuda'],
         'spark': ['pyspark'],
+        'dev': ['twine', 'setuptools', 'build'],
+        'all': ['cupy', 'pycuda', 'pyspark', 'twine', 'setuptools', 'build']
     },
-    classifiers = [
+    classifiers=[
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
-    python_requires = '>=3.5',
+    python_requires='>=3.5',
 )
```

