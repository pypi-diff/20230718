# Comparing `tmp/pami-2023.7.1.tar.gz` & `tmp/pami-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pami-2023.7.1.tar", last modified: Wed Jul  5 02:40:46 2023, max compression
+gzip compressed data, was "pami-2023.7.7.tar", last modified: Tue Jul 18 12:23:34 2023, max compression
```

## Comparing `pami-2023.7.1.tar` & `pami-2023.7.7.tar`

### file list

```diff
@@ -1,396 +1,434 @@
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.068497 pami-2023.7.1/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.1/LICENSE
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.991639 pami-2023.7.1/PAMI/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.991938 pami-2023.7.1/PAMI/AssociationRules/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.993820 pami-2023.7.1/PAMI/AssociationRules/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithConfidence.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLeverage.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLift.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/RuleMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/AssociationRules/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.993985 pami-2023.7.1/PAMI/correlatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.995945 pami-2023.7.1/PAMI/correlatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24412 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/correlatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.996140 pami-2023.7.1/PAMI/coveragePatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.997686 pami-2023.7.1/PAMI/coveragePatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/CMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/CPPG.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/coveragePatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:45.998948 pami-2023.7.1/PAMI/extras/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.000584 pami-2023.7.1/PAMI/extras/DF2DB/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/DF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/DF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/DF2DB/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/createTDB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DB.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.001023 pami-2023.7.1/PAMI/extras/calculateMISValues/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/usingBeta.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/calculateMISValues/usingSD.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.002310 pami-2023.7.1/PAMI/extras/dbStats/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/dbStats/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/temporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/transactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/dbStats/utilityDatabaseStats.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.004048 pami-2023.7.1/PAMI/extras/fuzzyTransformation/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.004853 pami-2023.7.1/PAMI/extras/generateDatabase/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateDatabase/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/generateLatexGraphFile.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006183 pami-2023.7.1/PAMI/extras/graph/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/dataFrameInToFigures.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/graph/visualizePatterns.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006385 pami-2023.7.1/PAMI/extras/image2Database/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/image2Database/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.006747 pami-2023.7.1/PAMI/extras/imageProcessing/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/imageProcessing/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/imageProcessing/imagery2Databases.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.007040 pami-2023.7.1/PAMI/extras/neighbours/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/neighbours/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/plotPointOnMap.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/plotPointOnMap_dump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/scatterPlotSpatialPoints.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/topKPatterns.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/extras/uncertaindb_convert.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.007240 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.008384 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.008684 pami-2023.7.1/PAMI/frequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.010529 pami-2023.7.1/PAMI/frequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/Apriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/ECLATbitset.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/basic/FPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.011225 pami-2023.7.1/PAMI/frequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/closed/CHARM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.012556 pami-2023.7.1/PAMI/frequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.013238 pami-2023.7.1/PAMI/frequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.014293 pami-2023.7.1/PAMI/frequentPattern/pyspark/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.015471 pami-2023.7.1/PAMI/frequentPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentPattern/topk/FAE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.015605 pami-2023.7.1/PAMI/frequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.016591 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/frequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.016800 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.017635 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.017845 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.018942 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.019167 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020130 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020436 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.020865 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.021086 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.022205 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.022436 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.023591 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.024431 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedFrequentPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.024667 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.025401 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.025636 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.026469 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.027147 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.027990 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.028221 pami-2023.7.1/PAMI/highUtilityPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.029468 pami-2023.7.1/PAMI/highUtilityPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/EFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/HMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/UPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.029912 pami-2023.7.1/PAMI/highUtilitySpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.031160 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.031948 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.032177 pami-2023.7.1/PAMI/localPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.033366 pami-2023.7.1/PAMI/localPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/localPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.033599 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.034638 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.034855 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.035794 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.036013 pami-2023.7.1/PAMI/partialPeriodicPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.039089 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.039939 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.040890 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.041687 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.042431 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.042854 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.043456 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.043732 pami-2023.7.1/PAMI/periodicCorrelatedPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.044298 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.044501 pami-2023.7.1/PAMI/periodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.046568 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.047372 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/closed/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.047787 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.048739 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.048955 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.049755 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.050428 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.050746 pami-2023.7.1/PAMI/recurringPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.051482 pami-2023.7.1/PAMI/recurringPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/recurringPattern/basic/RPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/recurringPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.051699 pami-2023.7.1/PAMI/relativeFrequentPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.052434 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.052647 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.053284 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.053503 pami-2023.7.1/PAMI/sequentialPatternMining/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.054576 pami-2023.7.1/PAMI/sequentialPatternMining/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/SPADE.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.055173 pami-2023.7.1/PAMI/sequentialPatternMining/closed/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/sequentialPatternMining/closed/bide.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.055260 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.056453 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.057421 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.057658 pami-2023.7.1/PAMI/uncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.062262 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.062509 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.063689 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.063931 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.064605 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.064843 pami-2023.7.1/PAMI/weightedFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.065590 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.065846 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.066475 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.066736 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/__init__.py
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.067463 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34817 2023-07-05 02:40:46.068347 pami-2023.7.1/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34213 2023-06-21 07:17:51.000000 pami-2023.7.1/README.md
-drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-05 02:40:46.068132 pami-2023.7.1/pami.egg-info/
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    34817 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/PKG-INFO
--rw-r--r--   0 udaykiranrage   (501) staff       (20)    13493 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/SOURCES.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/dependency_links.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       75 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/requires.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-05 02:40:45.000000 pami-2023.7.1/pami.egg-info/top_level.txt
--rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-05 02:40:46.068543 pami-2023.7.1/setup.cfg
--rw-r--r--   0 udaykiranrage   (501) staff       (20)     1205 2023-07-05 02:36:58.000000 pami-2023.7.1/setup.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.306139 pami-2023.7.7/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35149 2023-06-03 08:26:58.000000 pami-2023.7.7/LICENSE
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213420 pami-2023.7.7/PAMI/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.213780 pami-2023.7.7/PAMI/AssociationRules/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215229 pami-2023.7.7/PAMI/AssociationRules/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8001 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8038 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8085 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12384 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6547 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      139 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.215381 pami-2023.7.7/PAMI/correlatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.216924 pami-2023.7.7/PAMI/correlatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24417 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25824 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6055 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.217089 pami-2023.7.7/PAMI/coveragePatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.218352 pami-2023.7.7/PAMI/coveragePatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13995 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16075 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6938 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.219319 pami-2023.7.7/PAMI/extras/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221044 pami-2023.7.7/PAMI/extras/DF2DB/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2243 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/DF2DB/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4185 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4917 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9942 2023-07-05 02:36:31.000000 pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3607 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3359 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.221516 pami-2023.7.7/PAMI/extras/calculateMISValues/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3741 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3794 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.223716 pami-2023.7.7/PAMI/extras/dbStats/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/dbStats/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13043 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14661 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     9364 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13229 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    10040 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11775 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.225281 pami-2023.7.7/PAMI/extras/fuzzyTransformation/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5925 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5919 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5803 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.227961 pami-2023.7.7/PAMI/extras/generateDatabase/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2877 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7092 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3444 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3593 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231441 pami-2023.7.7/PAMI/extras/graph/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1656 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2954 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1167 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1753 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2203 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231576 pami-2023.7.7/PAMI/extras/image2Database/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/image2Database/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.231920 pami-2023.7.7/PAMI/extras/imageProcessing/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4582 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.232234 pami-2023.7.7/PAMI/extras/neighbours/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2834 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3031 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     3214 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2178 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233791 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2280 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2257 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2509 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1887 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1860 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2124 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2075 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     2265 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1827 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/topKPatterns.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      473 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/extras/uncertaindb_convert.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.233937 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235273 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14656 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21114 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6691 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.235589 pami-2023.7.7/PAMI/frequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.237534 pami-2023.7.7/PAMI/frequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13124 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    12531 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13188 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13480 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20324 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7733 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.238433 pami-2023.7.7/PAMI/frequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19874 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6445 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.240335 pami-2023.7.7/PAMI/frequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13459 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14203 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuAprioriBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13085 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13942 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cuEclatBit.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5738 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8648 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5576 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.241160 pami-2023.7.7/PAMI/frequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25097 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6436 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.242453 pami-2023.7.7/PAMI/frequentPattern/pyspark/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5603 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    13209 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    11487 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16147 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243543 pami-2023.7.7/PAMI/frequentPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    14674 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4575 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.243784 pami-2023.7.7/PAMI/frequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.244809 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20041 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19099 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6680 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245067 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.245890 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25239 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6635 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.246160 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247438 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    20740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24624 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6450 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.247699 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.248928 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23992 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26791 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6580 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249301 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.249802 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6449 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.250466 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251507 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23521 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25345 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6668 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.251792 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.252874 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26817 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32216 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6618 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.254340 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5007 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255007 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.255910 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19950 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6774 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256357 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6676 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/georeferencedFrequentSequencePattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.256630 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257531 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35401 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6081 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.257812 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261273 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    39910 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6181 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.261803 pami-2023.7.7/PAMI/highUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.264098 pami-2023.7.7/PAMI/highUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32747 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24847 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26567 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16479 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/basic/efimParallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265044 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5053 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16481 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/highUtilityPatterns/parallel/efimparallel.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.265480 pami-2023.7.7/PAMI/highUtilitySpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6718 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.266895 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27632 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34623 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5955 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267687 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35216 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6625 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.267930 pami-2023.7.7/PAMI/localPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269128 pami-2023.7.7/PAMI/localPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    32664 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21999 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21120 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     8378 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.269369 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270382 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23034 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22318 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5913 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.270633 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271619 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27316 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21102 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5392 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.271849 pami-2023.7.7/PAMI/partialPeriodicPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.273903 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    50844 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4195 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24330 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17878 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5572 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.274936 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21069 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5595 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.275960 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28482 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.276849 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26058 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5550 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277438 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7837 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17705 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.277755 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278324 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19876 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6165 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.278541 pami-2023.7.7/PAMI/periodicCorrelatedPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279293 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27518 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6652 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.279512 pami-2023.7.7/PAMI/periodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.281487 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15591 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25146 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    24942 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16311 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33244 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      726 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6525 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.282417 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    21540 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6538 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.283856 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6564 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19727 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17474 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.284826 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    28740 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7873 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285069 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.285761 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18066 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6898 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286394 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4583 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17235 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.286673 pami-2023.7.7/PAMI/recurringPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287396 pami-2023.7.7/PAMI/recurringPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26300 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6632 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.287636 pami-2023.7.7/PAMI/relativeFrequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288407 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26260 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4261 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.288643 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289267 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33573 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7391 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.289510 pami-2023.7.7/PAMI/sequentialPatternMining/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.290707 pami-2023.7.7/PAMI/sequentialPatternMining/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    41062 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6554 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    22592 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291328 pami-2023.7.7/PAMI/sequentialPatternMining/closed/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6279 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/sequentialPatternMining/closed/bide.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.291420 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.292688 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    16341 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25169 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    17918 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7258 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293628 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26386 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7177 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.293913 pami-2023.7.7/PAMI/streams/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294014 pami-2023.7.7/PAMI/streams/frequentPatterns/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.294626 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31851 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/FPStream.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7792 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/frequentPatterns/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295292 pami-2023.7.7/PAMI/streams/highUtility/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29434 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/HUPMS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    33678 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/SHUGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     5195 2023-07-07 08:23:47.000000 pami-2023.7.7/PAMI/streams/highUtility/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.295424 pami-2023.7.7/PAMI/uncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298349 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25974 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    26009 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    18710 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27060 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27823 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    25507 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    19046 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4962 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.298597 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      727 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.299797 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31127 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    31329 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6551 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300033 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300646 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27481 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6693 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.300913 pami-2023.7.7/PAMI/weightedFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.301700 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    23852 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     6737 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302005 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.302627 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    27228 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     7555 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.303017 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/__init__.py
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.304367 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    29070 2023-06-21 07:17:51.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        0 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/__init__.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     4782 2023-06-03 08:26:58.000000 pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.305978 pami-2023.7.7/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    34480 2023-07-07 08:24:43.000000 pami-2023.7.7/README.md
+drwxr-xr-x   0 udaykiranrage   (501) staff       (20)        0 2023-07-18 12:23:34.305715 pami-2023.7.7/pami.egg-info/
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    35126 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/PKG-INFO
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)    15099 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/SOURCES.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        1 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/dependency_links.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)      102 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/requires.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)        5 2023-07-18 12:23:34.000000 pami-2023.7.7/pami.egg-info/top_level.txt
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)       38 2023-07-18 12:23:34.306190 pami-2023.7.7/setup.cfg
+-rw-r--r--   0 udaykiranrage   (501) staff       (20)     1289 2023-07-18 12:22:32.000000 pami-2023.7.7/setup.py
```

### Comparing `pami-2023.7.1/LICENSE` & `pami-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithConfidence.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithConfidence.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLeverage.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLeverage.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/AssociationRules/basic/ARWithLift.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/ARWithLift.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/AssociationRules/basic/RuleMiner.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/RuleMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/AssociationRules/basic/abstract.py` & `pami-2023.7.7/PAMI/AssociationRules/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/correlatedPattern/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowth.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowth.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
                 else:
                     child.counter += pathCount
                     current = child
 
 
 class CPGrowth(_ab._correlatedPatterns):
     """
-    :Description: CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database. It is based on traditional Fpgrowth Algorithm,This algorithm uses breadth-first search technique to find the correlated Frequent patterns in transactional database.
+    :Description: CPGrowth is one of the fundamental algorithm to discover correlated frequent patterns in a transactional database. It is based on the traditional Fpgrowth Algorithm, this algorithm uses breadth-first search technique to find the correlated Frequent patterns in transactional database.
 
     :Reference: Lee, Y.K., Kim, W.Y., Cao, D., Han, J. (2003). CoMine: efficient mining of correlated patterns. In ICDM (pp. 581–584).
     :param  iFile: str :
                    Name of the Input file to mine complete set of frequent patterns
     :param  oFile: str :
                    Name of the output file to store complete set of frequent patterns
     :param  minSup: int or float or str :
```

### Comparing `pami-2023.7.1/PAMI/correlatedPattern/basic/CPGrowthPlus.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/CPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/correlatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/correlatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/correlatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/coveragePatterns/basic/CMine.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/coveragePatterns/basic/CPPG.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/CPPG.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/coveragePatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/coveragePatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/DF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/DF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/DF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/createTDB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/createTDB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/denseDF2DB_dump.py` & `pami-2023.7.7/PAMI/extras/DF2DB/denseDF2DB_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DB.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DB.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/DF2DB/sparseDF2DBPlus.py` & `pami-2023.7.7/PAMI/extras/DF2DB/sparseDF2DBPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/calculateMISValues/usingBeta.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingBeta.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/calculateMISValues/usingSD.py` & `pami-2023.7.7/PAMI/extras/calculateMISValues/usingSD.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/fuzzyDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/fuzzyDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/temporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/temporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/transactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/transactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTemporalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/uncertainTransactionalDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/dbStats/utilityDatabaseStats.py` & `pami-2023.7.7/PAMI/extras/dbStats/utilityDatabaseStats.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/fuzzyTransformation/abstract.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/temporalToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/transactionalToFuzzyTimeSeries.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py` & `pami-2023.7.7/PAMI/extras/fuzzyTransformation/utilityToFuzzy.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateSpatioTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/generateDatabase/generateTemporalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTemporalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/generateDatabase/generateTransactionalDatabase.py` & `pami-2023.7.7/PAMI/extras/generateDatabase/generateTransactionalDatabase.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/generateLatexGraphFile.py` & `pami-2023.7.7/PAMI/extras/generateLatexGraphFile.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/graph/dataFrameInToFigures.py` & `pami-2023.7.7/PAMI/extras/graph/dataFrameInToFigures.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/graph/generateLatexFileFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/generateLatexFileFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/graph/plotLineGraphFromDictionary.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphFromDictionary.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/graph/plotLineGraphsFromDataFrame.py` & `pami-2023.7.7/PAMI/extras/graph/plotLineGraphsFromDataFrame.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/graph/visualizePatterns.py` & `pami-2023.7.7/PAMI/extras/graph/visualizePatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/imageProcessing/imagery2Databases.py` & `pami-2023.7.7/PAMI/extras/imageProcessing/imagery2Databases.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py` & `pami-2023.7.7/PAMI/extras/neighbours/findNeighboursUsingEuclidean.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/plotPointOnMap.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/plotPointOnMap_dump.py` & `pami-2023.7.7/PAMI/extras/plotPointOnMap_dump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/scatterPlotSpatialPoints.py` & `pami-2023.7.7/PAMI/extras/scatterPlotSpatialPoints.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/extras/topKPatterns.py` & `pami-2023.7.7/PAMI/extras/topKPatterns.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/faultTolerantFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/faultTolerantFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/Apriori.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/Apriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/ECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/ECLATDiffset.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATDiffset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/ECLATbitset.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/ECLATbitset.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/FPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/FPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/closed/CHARM.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/CHARM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaAprioriTID.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaAprioriTID.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/cuda/cudaEclatGCT.py` & `pami-2023.7.7/PAMI/frequentPattern/cuda/cudaEclatGCT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/maximal/MaxFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/MaxFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/pyspark/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelApriori.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelApriori.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelECLAT.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/pyspark/parallelFPGrowth.py` & `pami-2023.7.7/PAMI/frequentPattern/pyspark/parallelFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/topk/FAE.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/FAE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/frequentPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/FSPGrowth.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/FSPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/SpatialECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/frequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/frequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/FCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/FFIMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentPatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/FFSPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPartialPeriodicPatterns/irregularTimeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/FPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzyPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/FGPFPMiner_old.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/fuzzySpatialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/geoReferencedFrequentPattern/GFPGrowth.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/GFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/geoReferencedFrequentPattern/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedFrequentPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/HUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityFrequentPatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityPatterns/basic/EFIM.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/EFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityPatterns/basic/HMiner.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/HMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityPatterns/basic/UPGrowth.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/UPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilityPatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/__init__.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/SHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/SHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/highUtilitySpatialPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/highUtilitySpatialPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPGrowth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMBreadth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMBreadth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/localPeriodicPattern/basic/LPPMDepth.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/LPPMDepth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/localPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/localPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/CFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/multipleMinimumSupportBasedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/GPFgrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/PPF_DFS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/GThreePGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/Gabstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/Gabstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/PPP_ECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/closed/PPPClose.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/PPPClose.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/Max3PGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/PPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/timeSeries/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/timeSeries/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/topk/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicPattern/topk/k3PMiner.py` & `pami-2023.7.7/PAMI/partialPeriodicPattern/topk/k3PMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/STEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/partialPeriodicSpatialPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/partialPeriodicSpatialPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/EPCPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicCorrelatedPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicCorrelatedPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFECLAT.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PFPMC.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PFPMC.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/PSGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/PSGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/CPFPMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/CPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/closed/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/__init__.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/maximal/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/maximal/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/TopkPFP/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py` & `pami-2023.7.7/PAMI/periodicFrequentPattern/topk/kPFPMiner/kPFPMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/recurringPattern/basic/RPGrowth.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/RPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/recurringPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/recurringPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/RSFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/relativeFrequentPatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeFrequentPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/RHUIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/relativeHighUtilityPatterns/basic/abstract.py` & `pami-2023.7.7/PAMI/relativeHighUtilityPatterns/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/sequentialPatternMining/basic/SPADE.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/SPADE.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/sequentialPatternMining/basic/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/sequentialPatternMining/basic/prefixSpan.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/basic/prefixSpan.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/sequentialPatternMining/closed/abstract.py` & `pami-2023.7.7/PAMI/sequentialPatternMining/closed/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPEclat.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/stablePeriodicFrequentPattern/topK/abstract.py` & `pami-2023.7.7/PAMI/stablePeriodicFrequentPattern/topK/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/CUFPTree.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/CUFPTree.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/PUFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TUFP.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TUFP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeP.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeP.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/TubeS.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/TubeS.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UFGrowth.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UFGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/UVECLAT.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/UVECLAT.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/__init__.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/__init__.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/UPFPGrowthPlus.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/uncertainPeriodicFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/SWFPGrowth.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentNeighbourhoodPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentPattern/basic/WFIM.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/WFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/WFRIMiner.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedFrequentRegularPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedFrequentRegularPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/WUFIM.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PAMI/weightedUncertainFrequentPattern/basic/abstract.py` & `pami-2023.7.7/PAMI/weightedUncertainFrequentPattern/basic/abstract.py`

 * *Files identical despite different names*

### Comparing `pami-2023.7.1/PKG-INFO` & `pami-2023.7.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,42 @@
-Metadata-Version: 2.1
-Name: pami
-Version: 2023.7.1
-Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
-Home-page: https://github.com/udayRage/PAMI
-Author: Rage Uday Kiran
-Author-email: uday.rage@gmail.com
-License: GPLv3
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
-![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
-![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
-[![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
-[![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
-[![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
-[![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
+[![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
+[![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
+[![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
+[![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
+
+[Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
-1. User manual https://udayrage.github.io/PAMI/manuals/index.html
+1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
-2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
+2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-5. Report issues https://github.com/udayRage/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
+- Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
@@ -69,25 +56,25 @@
 
 ## 1. Mining Databases
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
@@ -95,229 +82,229 @@
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
-| CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
 | Basic                                                                                                                                                                                                                                      |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+| GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
 |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+| EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
 | Basic      | TopK |
 |------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
-| FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
+| spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
+| FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
 | Basic     |
 |-----------|
-| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
+| RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
 
 ### Utility databases
 
 1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
-| EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
-| HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
+| EFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
+| HMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
 2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
+| HUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
 
 
 3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
-| SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
+| SHUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
 
 4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
-| HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
-| SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
+| HDSHIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
+| SHUIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
 
-5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
 
 | Basic |
 |-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+| RHUIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
 
 6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
 
 | Basic |
 |-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+| WFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
 
 
 7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
+| WFRIMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
 
 
-8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
 | SSWFPGrowth |
 
 ### Fuzzy databases
-1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
+| FFI-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
 
 
 
 2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+| FCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
 
 
-3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+| FFSP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
 
-4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
 
-5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 ### Uncertain databases
 
 
 1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
 | Basic   | top-k |
 |---------|-------|
-| PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
-| TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
-| TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
+| PUF [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
+| TubeP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
+| TubeS  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
 
 2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
-| UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
-| UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
+| UPFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
+| UPFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
 
 
 3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
 
 | Basic |
 |-------|
-| WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
+| WUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
 
 ### Sequence databases
 
-1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+1. Sequence frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
-| SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
-| prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+| SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
+| prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+
 
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
    __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__   
      
      
-
-
```

### Comparing `pami-2023.7.1/README.md` & `pami-2023.7.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,61 @@
+Metadata-Version: 2.1
+Name: pami
+Version: 2023.7.7
+Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
+Home-page: https://github.com/udayRage/PAMI
+Author: Rage Uday Kiran
+Author-email: uday.rage@gmail.com
+License: GPLv3
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+Provides-Extra: gpu
+Provides-Extra: spark
+License-File: LICENSE
+
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
-![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
-![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
-[![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
-[![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
-[![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
-[![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
+[![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
+[![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
+[![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
+[![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
+
+[Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
-1. User manual https://udayrage.github.io/PAMI/manuals/index.html
+1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
-2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
+2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-5. Report issues https://github.com/udayRage/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
+- Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
@@ -52,25 +75,25 @@
 
 ## 1. Mining Databases
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
@@ -78,227 +101,231 @@
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
-| CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
 | Basic                                                                                                                                                                                                                                      |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+| GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
 |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+| EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
 | Basic      | TopK |
 |------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
-| FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
+| spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
+| FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
 | Basic     |
 |-----------|
-| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
+| RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
 
 ### Utility databases
 
 1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
-| EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
-| HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
+| EFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
+| HMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
 2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
+| HUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
 
 
 3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
-| SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
+| SHUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
 
 4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
-| HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
-| SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
+| HDSHIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
+| SHUIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
 
-5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
 
 | Basic |
 |-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+| RHUIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
 
 6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
 
 | Basic |
 |-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+| WFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
 
 
 7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
+| WFRIMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
 
 
-8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
 | SSWFPGrowth |
 
 ### Fuzzy databases
-1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
+| FFI-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
 
 
 
 2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+| FCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
 
 
-3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+| FFSP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
 
-4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
 
-5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 ### Uncertain databases
 
 
 1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
 | Basic   | top-k |
 |---------|-------|
-| PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
-| TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
-| TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
+| PUF [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
+| TubeP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
+| TubeS  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
 
 2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
-| UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
-| UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
+| UPFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
+| UPFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
 
 
 3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
 
 | Basic |
 |-------|
-| WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
+| WUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
 
 ### Sequence databases
 
-1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+1. Sequence frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
-| SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
-| prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+| SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
+| prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+
 
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
    __coming soon__    
 
 ## 3. Mining Graphs
 __coming soon__   
      
      
+
+
```

### Comparing `pami-2023.7.1/pami.egg-info/PKG-INFO` & `pami-2023.7.7/pami.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 Metadata-Version: 2.1
 Name: pami
-Version: 2023.7.1
+Version: 2023.7.7
 Summary: This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan
 Home-page: https://github.com/udayRage/PAMI
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
+Provides-Extra: gpu
+Provides-Extra: spark
 License-File: LICENSE
 
 ![PyPI](https://img.shields.io/pypi/v/PAMI)
-![AppVeyor](https://img.shields.io/appveyor/build/udayRage/PAMI)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/PAMI)
-![GitHub all releases](https://img.shields.io/github/downloads/udayRage/PAMI/total)
-[![GitHub license](https://img.shields.io/github/license/udayRage/PAMI)](https://github.com/udayRage/PAMI/blob/main/LICENSE)
+[![GitHub license](https://img.shields.io/github/license/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/blob/main/LICENSE)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/PAMI)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/PAMI)
 ![PyPI - Status](https://img.shields.io/pypi/status/PAMI)
-[![GitHub issues](https://img.shields.io/github/issues/udayRage/PAMI)](https://github.com/udayRage/PAMI/issues)
-[![GitHub forks](https://img.shields.io/github/forks/udayRage/PAMI)](https://github.com/udayRage/PAMI/network)
-[![GitHub stars](https://img.shields.io/github/stars/udayRage/PAMI)](https://github.com/udayRage/PAMI/stargazers)
+[![GitHub issues](https://img.shields.io/github/issues/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/issues)
+[![GitHub forks](https://img.shields.io/github/forks/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/network)
+[![GitHub stars](https://img.shields.io/github/stars/UdayLab/PAMI)](https://github.com/UdayLab/PAMI/stargazers)
+[![Downloads](https://static.pepy.tech/badge/pami)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/month)](https://pepy.tech/project/pami)
+[![Downloads](https://static.pepy.tech/badge/pami/week)](https://pepy.tech/project/pami)
+
+[Click here for more information](https://pepy.tech/project/pami)
 
 
 # Introduction
 PAttern MIning (PAMI) is a Python library containing several algorithms to discover user interest-based patterns in transactional/temporal/geo-referential/sequence databases across multiple computing platforms.
 
 
-1. User manual https://udayrage.github.io/PAMI/manuals/index.html
+1. User manual https://udaylab.github.io/PAMI/manuals/index.html
 
-2. Coders manual https://udayrage.github.io/PAMI/codersManual/index.html
+2. Coders manual https://udaylab.github.io/PAMI/codersManual/index.html
 
-3. Code documentation [PAMI documentation](https://raw.githack.com/udayRage/PAMI/main/htmlDocs/_build/html/index.html)
+3. Code documentation [PAMI documentation](https://raw.githack.com/UdayLab/PAMI/main/htmlDocs/_build/html/index.html)
 
 3. Datasets   https://u-aizu.ac.jp/~udayrage/datasets.html
 
-4. Discussions on PAMI usage https://github.com/udayRage/PAMI/discussions
+4. Discussions on PAMI usage https://github.com/UdayLab/PAMI/discussions
 
-5. Report issues https://github.com/udayRage/PAMI/issues
+5. Report issues https://github.com/UdayLab/PAMI/issues
   
  # Recent versions  
 
+- Version 2023.07.07: New algorithms: cuApriroi, cuAprioriBit, cuEclat, cuEclatBit, gPPMiner, cuGPFMiner, FPStream, HUPMS, SHUPGrowth New codes to generate synthetic databases
 - Version 2023.06.20: Fuzzy Partial Periodic, Periodic Patterns in High Utility, Code Documentation, help() function Update 
 - Version 2023.03.01: prefixSpan and SPADE   
 
 Total number of algorithms: 83
 
 # Maintenance
 
@@ -69,25 +75,25 @@
 
 ## 1. Mining Databases
 ### Transactional databases
 1. Frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                            | Closed                                                                                                                                                                                                           | Maximal                                                                                                                   | Top-k                                                                                                                                                                                                  | CUDA           | pyspark                                                                                                                                                                                                                                               |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| Apriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
-| FP-growth  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
-| ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
-| ECLAT-bitSet [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
-| ECLAT-diffset [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
+| Apriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/APRIORI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/Apriori/Apriori-ad.md)              | Closed [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/closed/CHARM/CHARM-ad.md) | maxFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/maximal/MaxFPGrowth/MaxFPGrowth-st.md) | topK [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/topk/FAE-ad.pdf) | cudaAprioriGCT | parallelApriori [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/parallelApriori-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelApriori/ParallelApriori-ad%20(1).md) |
+| FP-growth  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_basic.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/FPGrowth/fpGrowth_adv.md)         |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaAprioriTID | parallelFPGrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/parallelFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelFPGrowth/ParallelFPGrowth-ad%20.md) |
+| ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLAT/Eclat-ad.md)                   |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        | cudaEclatGCT   | parallelECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/parallelECLAT/parallelECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/pyspark/ParallelECLAT-ad.pdf)             |
+| ECLAT-bitSet [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/ECLATbitset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATbitset/Eclatbitset-ad.md) |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |                                                                                                                                                                                                                                                       |
+| ECLAT-diffset [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/ECLATDiffset-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentPattern/basic/ECLATDiffset/EclatDiffset-ad.md)                                                                                                                                                                                                                    |                                                                                                                                                                                                                  |                                                                                                                           |                                                                                                                                                                                                        |                |
 
 2. Relative frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/relativeFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| RSFP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
+| RSFP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/relativeFrequentPatterns/RSFPGrowth/RSFPGrowt-ad.md)|
 
 
 3. Frequent pattern with multiple minimum support: [Sample](https://udayrage.github.io/PAMI/multipleMinSupFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
 | CFPGrowth   |
@@ -95,224 +101,226 @@
 
 
 
 4. Correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/correlatePatternMining.html)
 
 | Basic                                                                                                                                                                                                            |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
-| CP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
+| CP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-st.md) -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowth/CPGrowth-ad.md) |
+| CP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPuls-st.md)                                                                                              -[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/correlatedPattern/CPGrowthPlus/CPGrowthPlus-ad.md)|
 
 
 ### Temporal databases
 
 
 1. Periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                                | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                           | Top-K |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------| -----------------------------------------------------------------------------------------------------------------------------------|
-| PFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
-| PFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PS-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
-| PFP-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowth/PFPGrowth-ad.md)       | CPFP [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/closed/CPFPMiner/CPFPMiner-ad.md) | maxPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/maximal/MaxPFGrowth-ad.md) |  kPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/topk/kPFPMiner/kPFPMiner-ad%20.md) |
+| PFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFPGrowthPlus/PFPGrowthPlus-ad%20.md) |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PS-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PSGrowth/PSGrowth-ad.md)              |                                                                                                                                                                                                                                        |                                                                                                                                   |
+| PFP-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/basic/PFECLAT/PFECLAT-ad%20.md)                |                                                                                                                                                                                                                                        |                                                                                                                                   |
 
 
 2. Local periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/localPeriodicPatternMining.html)
 
 | Basic       |
 |-------------|
-| LPPGrowth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
-| LPPMBreadth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
-| LPPMDepth   [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
+| LPPGrowth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPGrowth/LPPGrowth-st.md)|
+| LPPMBreadth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMBreadth/LPPMBreadth-st.md)|
+| LPPMDepth   [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/localPeriodicPatterns/basic/LPPMDepth/LPPMDepth-st.md)|
 
 3. Partial periodic-frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicFrequentPattern.html)
 
 | Basic                                                                                                                                                                                                                                      |
 |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| GPF-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
-| PPF-DFS [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
+| GPF-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/GPFGrowth/GPFgrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf) |
+| PPF-DFS [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPatterns/PPF_DFS/PPF_DFS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicFrequentPattern/PPF_DFS-ad.pdf)    |
 
 4. Partial periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/partialPeriodicPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                         | Closed                                                                                                                                                                                                                                 | Maximal                                                                                                                          |
 |-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------|
-| 3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
-| 3P-ECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
-| G3P-Growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
+| 3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPGrowth/PPPGrowth-ad.md) | 3P-close [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/closed/PPPClose-ad.pdf) | max3P-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPattern/maximal/Max3PGrowth-st.pdf) |                                                                                                                                                                                                                                         |                                                                                                                                  |               | |
+| 3P-ECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/PPPECLAT/PPP_ECLAT-ad.md)|  |  |
+| G3P-Growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/basic/G3PGrowth/GThreePGrowth-ad.md) | | |
 
 
 5. Periodic correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| EPCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
+| EPCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/correlated/EPCPGrowth/EPCPGrowth-ad.md) |
 
 6. Stable periodic pattern mining: [Sample](https://udayrage.github.io/PAMI/stablePeriodicPatterns.html)
 
 | Basic      | TopK |
 |------------|------|
-| SPP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
-| SPP-ECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
+| SPP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPGrowth/SPPGrowth-ad%20.md)| TSPIN  |
+| SPP-ECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/stablePeriodicFrequentPatterns/SPPEclat/SPPECLAT-ad%20.md) |  |
 
 ### Geo-referenced (or spatiotemporal) databases
 
 1. Frequent spatial pattern mining: [Sample](https://udayrage.github.io/PAMI/frequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                 |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| spatialECLAT  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
-| FSP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
+| spatialECLAT  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/SpatialECLAT-ad.pdf) |
+| FSP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/frequentSpatialPattern/FSPGrowth-ad.pdf)          |
 
 2. Geo referenced Periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/periodicFrequentSpatial.html)
 
 | Basic     |
 |-----------|
-| GPFPMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
+| GPFPMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/spatial/GPFPMiner/GPFPMiner-ad.md)  |
 
 3. Partial periodic spatial pattern mining:[Sample](https://udayrage.github.io/PAMI/partialPeriodicSpatialPatternMining.html)
 
 | Basic   |
 |---------|
-| STECLAT [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
+| STECLAT [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/partialPeriodicPatterns/spatial/STECLAT/STECLAT-ad.md)|
 
 4. Recurring pattern mining: [Sample](https://udayrage.github.io/PAMI/RecurringPatterns.html)
 
 | Basic    |
 |----------|
-| RPgrowth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
+| RPgrowth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/periodicFrequentPatterns/recurring/RPGrowth-ad.md)|
 
 
 ### Utility databases
 
 1. High utility pattern mining:   [Sample](https://udayrage.github.io/PAMI/highUtilityPatternMining.html)
 
 | Basic    |
 |----------|
-| EFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
-| HMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
+| EFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-ad.md)   |
+| HMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/EFIM/EFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/basic/HMiner/HMiner-st.md)  |
 | UPGrowth |
 
 2. High utility frequent pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtiltiyFrequentPatternMining.html)
 
 | Basic |
 |-------|
-| HUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
+| HUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/basic/HUFIM/HUFIM-ad.md)|
 
 
 3. High utility frequent spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  |
 |--------|
-| SHUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
+| SHUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/hitghUtilityFrequent/spatial/SHUFIM-ad.md)|
 
 4. High utility spatial pattern mining:  [Sample](https://udayrage.github.io/PAMI/highUtilitySpatialPatternMining.html)
 
 | Basic  | topk    |
 |--------|---------|
-| HDSHIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
-| SHUIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
+| HDSHIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-st%20-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/HDSHUIM/HDSHUIM-ad.md)| TKSHUIM |
+| SHUIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/spatial/SHUM/SHUIM-st.md)|
 
 
-5. Relative High utility pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
+5. Relative High utility pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/mainManuals/relativeUtility.html)
 
 | Basic |
 |-------|
-| RHUIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
+| RHUIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/highUtilityPatterns/relative/RHUIM-ad.md)| 
 
 
 6. Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentPattern.html)
 
 | Basic |
 |-------|
-| WFIM  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
+| WFIM  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFIM/WFIM-ad.md)|
 
 
 7. Weighted frequent regular pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedFrequentRegularPatterns.html)
 
 | Basic     |
 |-----------|
-| WFRIMiner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
+| WFRIMiner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/WFRIM/WFRI.md)|
 
 
-8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+8. Weighted frequent neighbourhood pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
 
 | Basic       |
 |-------------|
 | SSWFPGrowth |
 
 ### Fuzzy databases
-1. Fuzzy Frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentPatternMining.html)
+1. Fuzzy Frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                   |
 |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFI-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
+| FFI-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/basic/FFIMiner/FFIMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/FFIMiner-ad.pdf) |
 
 
 
 
 2. Fuzzy correlated pattern mining: [Sample](https://udayrage.github.io/PAMI/fuzzyCorrelatedPatternMining.html)
 
 | Basic                                                                                                                                                                                                                        |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FCP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
+| FCP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-st%20.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyCorrelatedPatterns/basic/FCPGrowth/FCPGrowth-ad.md) |
 
 
-3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyFrequentSpatialPatternMining.html)
+3. Fuzzy frequent spatial pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyFrequentSpatialPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FFSP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
+| FFSP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-ad.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyFrequentPatterns/fuzzySpatial/FFSPMiner/FFSPMiner-st.md) |
 
-4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzyPeriodicFrequentPatternMining.html)
+4. Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzyPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPatterns/basic/FPFPMiner/FPFPMiner-ad.md) |
 
-5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
+5. Geo referenced Fuzzy periodic frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/fuzzySpatialPeriodicFrequentPatternMining.html)
 
 | Basic                                                                                                                                                                                                                                    |
 |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| FPFP-Miner [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
+| FPFP-Miner [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-st.pdf)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/fuzzyPeriodicFrequentPattern/FPFPMiner-ad.pdf) |
 
 ### Uncertain databases
 
 
 1. Uncertain frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainFrequentPatternMining.html)
 
 | Basic   | top-k |
 |---------|-------|
-| PUF [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
-| TubeP  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
-| TubeS  [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
+| PUF [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/PUFGrowth/PUFGrowth-ad.md)    | TUFP  |
+| TubeP  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeP/TubeP-ad.md)  |       |
+| TubeS  [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainFrequentPatterns/basic/TubeS/TubeS-ad.md)  |       | 
 | UVEclat |       |
 
 2. Uncertain periodic frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/uncertainPeriodicFrequentPatternMining.html)
 
 | Basic       |
 |-------------|
-| UPFP-growth [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
-| UPFP-growth++ [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
+| UPFP-growth [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowth/UPFPGrowth-ad.md) |
+| UPFP-growth++ [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-st-2.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/uncertainPeriodicFrequent/basic/UPFPGrowthPlus/UPFPGrowthPlus-ad.md)|
 
 
 3. Uncertain Weighted frequent pattern mining: [Sample](https://udayrage.github.io/PAMI/weightedUncertainFrequentPatterns.html)
 
 | Basic |
 |-------|
-| WUFIM [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
+| WUFIM [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/weightedFrequentPatterns/weightedUncertain/WUFIM-st.md)|
 
 ### Sequence databases
 
-1. Sequence frequent pattern mining: [Sample](https://github.com/udayRage/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
+1. Sequence frequent pattern mining: [Sample](https://github.com/UdayLab/PAMI/blob/main/docs/weightedSpatialFrequentPattern.html)
     
 | Basic       |
 |-------------|
-| SPADE [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
-| prefixSpan [Basic](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/udayRage/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+| SPADE [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/SPADE/Spade-ad.md)|
+| prefixSpan [Basic](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-st.md)-[Adv](https://github.com/UdayLab/PAMI/blob/main/sampleManuals/sequencePatternMining/basic/prefixSpan/PrifixSpan-ad.md)|
+
 
+2, Geo-referenced Frequent Sequence Pattern
 ### Timeseries databases
 
 
 ## 2. Mining Streams
    __coming soon__    
 
 ## 3. Mining Graphs
```

### Comparing `pami-2023.7.1/pami.egg-info/SOURCES.txt` & `pami-2023.7.7/pami.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -61,14 +61,23 @@
 PAMI/extras/graph/plotLineGraphsFromDataFrame.py
 PAMI/extras/graph/visualizePatterns.py
 PAMI/extras/image2Database/__init__.py
 PAMI/extras/imageProcessing/__init__.py
 PAMI/extras/imageProcessing/imagery2Databases.py
 PAMI/extras/neighbours/__init__.py
 PAMI/extras/neighbours/findNeighboursUsingEuclidean.py
+PAMI/extras/syntheticDatabaseGenerator/__init__.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTemporal.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialTransactions.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticGeoreferentialUncertainTransaction.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticTemporal.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticTransactions.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTemporal.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticUncertainTransactions.py
+PAMI/extras/syntheticDatabaseGenerator/createSyntheticUtility.py
 PAMI/faultTolerantFrequentPattern/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/FTApriori.py
 PAMI/faultTolerantFrequentPattern/basic/FTFPGrowth.py
 PAMI/faultTolerantFrequentPattern/basic/VBFTMine.py
 PAMI/faultTolerantFrequentPattern/basic/__init__.py
 PAMI/faultTolerantFrequentPattern/basic/abstract.py
 PAMI/frequentPattern/__init__.py
@@ -79,14 +88,19 @@
 PAMI/frequentPattern/basic/FPGrowth.py
 PAMI/frequentPattern/basic/__init__.py
 PAMI/frequentPattern/basic/abstract.py
 PAMI/frequentPattern/closed/CHARM.py
 PAMI/frequentPattern/closed/__init__.py
 PAMI/frequentPattern/closed/abstract.py
 PAMI/frequentPattern/cuda/__init__.py
+PAMI/frequentPattern/cuda/abstract.py
+PAMI/frequentPattern/cuda/cuApriori.py
+PAMI/frequentPattern/cuda/cuAprioriBit.py
+PAMI/frequentPattern/cuda/cuEclat.py
+PAMI/frequentPattern/cuda/cuEclatBit.py
 PAMI/frequentPattern/cuda/cudaAprioriGCT.py
 PAMI/frequentPattern/cuda/cudaAprioriTID.py
 PAMI/frequentPattern/cuda/cudaEclatGCT.py
 PAMI/frequentPattern/maximal/MaxFPGrowth.py
 PAMI/frequentPattern/maximal/__init__.py
 PAMI/frequentPattern/maximal/abstract.py
 PAMI/frequentPattern/pyspark/__init__.py
@@ -132,28 +146,34 @@
 PAMI/geoReferencedFrequentPattern/GFPGrowth.py
 PAMI/geoReferencedFrequentPattern/__init__.py
 PAMI/geoReferencedFrequentPattern/abstract.py
 PAMI/geoReferencedPeriodicFrequentPattern/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/GPFPMiner.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/__init__.py
 PAMI/geoReferencedPeriodicFrequentPattern/basic/abstract.py
+PAMI/georeferencedFrequentSequencePattern/__init__.py
+PAMI/georeferencedFrequentSequencePattern/abstract.py
 PAMI/highUtilityFrequentPatterns/__init__.py
 PAMI/highUtilityFrequentPatterns/basic/HUFIM.py
 PAMI/highUtilityFrequentPatterns/basic/__init__.py
 PAMI/highUtilityFrequentPatterns/basic/abstract.py
 PAMI/highUtilityFrequentSpatialPattern/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/SHUFIM.py
 PAMI/highUtilityFrequentSpatialPattern/basic/__init__.py
 PAMI/highUtilityFrequentSpatialPattern/basic/abstract.py
 PAMI/highUtilityPatterns/__init__.py
 PAMI/highUtilityPatterns/basic/EFIM.py
 PAMI/highUtilityPatterns/basic/HMiner.py
 PAMI/highUtilityPatterns/basic/UPGrowth.py
 PAMI/highUtilityPatterns/basic/__init__.py
 PAMI/highUtilityPatterns/basic/abstract.py
+PAMI/highUtilityPatterns/basic/efimParallel.py
+PAMI/highUtilityPatterns/parallel/__init__.py
+PAMI/highUtilityPatterns/parallel/abstract.py
+PAMI/highUtilityPatterns/parallel/efimparallel.py
 PAMI/highUtilitySpatialPattern/__init__.py
 PAMI/highUtilitySpatialPattern/abstract.py
 PAMI/highUtilitySpatialPattern/basic/HDSHUIM.py
 PAMI/highUtilitySpatialPattern/basic/SHUIM.py
 PAMI/highUtilitySpatialPattern/basic/__init__.py
 PAMI/highUtilitySpatialPattern/basic/abstract.py
 PAMI/highUtilitySpatialPattern/topk/TKSHUIM.py
@@ -210,14 +230,16 @@
 PAMI/periodicFrequentPattern/basic/PSGrowth.py
 PAMI/periodicFrequentPattern/basic/__init__.py
 PAMI/periodicFrequentPattern/basic/abstract.py
 PAMI/periodicFrequentPattern/closed/CPFPMiner.py
 PAMI/periodicFrequentPattern/closed/__init__.py
 PAMI/periodicFrequentPattern/closed/abstract.py
 PAMI/periodicFrequentPattern/cuda/__init__.py
+PAMI/periodicFrequentPattern/cuda/abstract.py
+PAMI/periodicFrequentPattern/cuda/cuGPFMiner.py
 PAMI/periodicFrequentPattern/cuda/gPFMinerBit.py
 PAMI/periodicFrequentPattern/maximal/MaxPFGrowth.py
 PAMI/periodicFrequentPattern/maximal/__init__.py
 PAMI/periodicFrequentPattern/maximal/abstract.py
 PAMI/periodicFrequentPattern/topk/__init__.py
 PAMI/periodicFrequentPattern/topk/TopkPFP/TopkPFP.py
 PAMI/periodicFrequentPattern/topk/TopkPFP/__init__.py
@@ -250,14 +272,23 @@
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowth.py
 PAMI/stablePeriodicFrequentPattern/basic/SPPGrowthDump.py
 PAMI/stablePeriodicFrequentPattern/basic/__init__.py
 PAMI/stablePeriodicFrequentPattern/basic/abstract.py
 PAMI/stablePeriodicFrequentPattern/topK/TSPIN.py
 PAMI/stablePeriodicFrequentPattern/topK/__init__.py
 PAMI/stablePeriodicFrequentPattern/topK/abstract.py
+PAMI/streams/__init__.py
+PAMI/streams/frequentPatterns/__init__.py
+PAMI/streams/frequentPatterns/basic/FPStream.py
+PAMI/streams/frequentPatterns/basic/__init__.py
+PAMI/streams/frequentPatterns/basic/abstract.py
+PAMI/streams/highUtility/HUPMS.py
+PAMI/streams/highUtility/SHUGrowth.py
+PAMI/streams/highUtility/__init__.py
+PAMI/streams/highUtility/abstract.py
 PAMI/uncertainFrequentPattern/__init__.py
 PAMI/uncertainFrequentPattern/basic/CUFPTree.py
 PAMI/uncertainFrequentPattern/basic/PUFGrowth.py
 PAMI/uncertainFrequentPattern/basic/TUFP.py
 PAMI/uncertainFrequentPattern/basic/TubeP.py
 PAMI/uncertainFrequentPattern/basic/TubeS.py
 PAMI/uncertainFrequentPattern/basic/UFGrowth.py
```

### Comparing `pami-2023.7.1/setup.py` & `pami-2023.7.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'pami',
-    version = '2023.07.01',
+    version = '2023.07.07',
     author = 'Rage Uday Kiran',
     author_email = 'uday.rage@gmail.com',
     description = 'This software is being developed at the University of Aizu, Aizu-Wakamatsu, Fukushima, Japan',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages=setuptools.find_packages(),
     url = 'https://github.com/udayRage/PAMI',
@@ -18,17 +18,21 @@
         'psutil',
         'pandas',
         'plotly',
         'matplotlib',
         'resource',
         'validators',
         'urllib3',
-        'pyspark',
         'Pillow',
+        'numpy',
     ],
+    extras_require = {
+        'gpu':  ['cupy'],
+        'spark': ['pyspark'],
+    },
     classifiers = [
         'Development Status :: 5 - Production/Stable',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires = '>=3.5',
```

