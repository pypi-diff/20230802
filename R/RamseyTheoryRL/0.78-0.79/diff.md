# Comparing `tmp/RamseyTheoryRL-0.78.tar.gz` & `tmp/RamseyTheoryRL-0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RamseyTheoryRL-0.78.tar", last modified: Mon Jul 31 23:40:58 2023, max compression
+gzip compressed data, was "RamseyTheoryRL-0.79.tar", last modified: Wed Aug  2 21:32:02 2023, max compression
```

## Comparing `RamseyTheoryRL-0.78.tar` & `RamseyTheoryRL-0.79.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.943600 RamseyTheoryRL-0.78/
--rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.78/LICENSE.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 03:58:20.000000 RamseyTheoryRL-0.78/MANIFEST.in
--rw-r--r--   0 stevevott   (501) staff       (20)     5138 2023-07-31 23:40:58.943672 RamseyTheoryRL-0.78/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     4672 2023-07-24 16:38:37.000000 RamseyTheoryRL-0.78/README.md
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.889077 RamseyTheoryRL-0.78/RamseyTheoryRL/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.887269 RamseyTheoryRL-0.78/RamseyTheoryRL/data/
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.886139 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.895754 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/
--rw-r--r--   0 stevevott   (501) staff       (20)   172832 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/all_leq6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)     4100 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_4.csv
--rw-r--r--   0 stevevott   (501) staff       (20)   163072 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_5.csv
--rw-r--r--   0 stevevott   (501) staff       (20)  1420327 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)    32697 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_7.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      240 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_9.csv
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.899076 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/
--rw-r--r--   0 stevevott   (501) staff       (20)    62803 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/all_leq6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)     1811 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_4.csv
--rw-r--r--   0 stevevott   (501) staff       (20)    42779 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_5.csv
--rw-r--r--   0 stevevott   (501) staff       (20)   376715 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)    10322 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_7.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      129 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_9.csv
--rw-r--r--   0 stevevott   (501) staff       (20)   776505 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_4_4.csv
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.902462 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/
--rw-r--r--   0 stevevott   (501) staff       (20)      112 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v35.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      117 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v36.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      123 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v37.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      130 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v38.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      136 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v39.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      142 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/empty_graphs/v40.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.911667 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/
--rw-r--r--   0 stevevott   (501) staff       (20)      161 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r34_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        7 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r34_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)   401300 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r34_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       87 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r35_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      304 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r35_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r39_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_10_35_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      727 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_6_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       69 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_6_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      756 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_7_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_7_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     3648 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_7_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)      196 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_8_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       77 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_8_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)   399016 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_8_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       65 2023-07-24 16:10:44.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_12_2_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       26 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_12_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_3_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       14 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_3_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       96 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_3_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)     1294 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_6_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    42316 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_6_path.txt
--rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-24 16:11:31.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_9_35_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-27 00:29:49.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r4_6_35_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    47888 2023-07-15 16:54:40.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r5_5_42_isograph.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.914420 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/
--rw-r--r--   0 stevevott   (501) staff       (20)        4 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_3_5_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_6_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       42 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_7_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       28 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       10 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_10_graph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     1140 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_8_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2053 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_9_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     1969 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_6_8_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_10_4_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_15_4_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    11973 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_4_12_isograph.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       20 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_8_3_isograph.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.916588 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       12 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       33 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      136 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      780 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     6264 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    86422 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph8.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.887041 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.919403 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       18 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       36 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       75 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_8.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.922107 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     3130 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_10.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     1260 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_11.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      156 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_12.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_13.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       52 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      160 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      426 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     1253 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_8.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2320 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_9.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.924984 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    66570 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_10.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      175 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_17.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       56 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      185 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      600 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2492 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_8.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    11256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_9.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.925151 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_7/
--rw-r--r--   0 stevevott   (501) staff       (20)     7831 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_7/r37_22.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.925314 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_9/
--rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_9/r39_35.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.927957 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    12800 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_15.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       44 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_16.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       25 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_17.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       12 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       27 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       96 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      420 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2172 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    14553 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_8.g6
--rw-r--r--   0 stevevott   (501) staff       (20)   117608 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_9.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.928450 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_6/
--rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_6/r46_35some.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.928731 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/5_5/
--rw-r--r--   0 stevevott   (501) staff       (20)    47888 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/5_5/r55_42some.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.930734 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/
--rw-r--r--   0 stevevott   (501) staff       (20)      124 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_all_leq6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      186 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_igraph_all_leq9.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      192 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_3_4.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      304 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_3_5.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_3_6.csv
--rw-r--r--   0 stevevott   (501) staff       (20)       32 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_3_7.csv
--rw-r--r--   0 stevevott   (501) staff       (20)       32 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_3_9.csv
--rw-r--r--   0 stevevott   (501) staff       (20)      261 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_4_4.csv
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/time/time_ramsey_4_5.csv
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.930855 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r(4,6,36)_graph.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.932557 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       18 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       36 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       75 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r34/r34_8.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.935942 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     3130 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_10.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      156 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_12.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_13.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       52 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      160 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      426 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     1253 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_8.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2320 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_9.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.939159 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/
--rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_1.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      175 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_17.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_2.g6
--rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_3.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_4.g6
--rw-r--r--   0 stevevott   (501) staff       (20)       56 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_5.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      185 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_6.g6
--rw-r--r--   0 stevevott   (501) staff       (20)      600 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_7.g6
--rw-r--r--   0 stevevott   (501) staff       (20)     2492 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_8.g6
--rw-r--r--   0 stevevott   (501) staff       (20)    11256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_9.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.939540 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r46/
--rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r46/r46_35some.g6
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.939824 RamseyTheoryRL-0.78/RamseyTheoryRL/src/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/__init__.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.941018 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:39.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)    12523 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/gbfs.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3539 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1070 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/igraph_train_gen.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1157 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/isofile_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3365 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/train_gen.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.942044 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-07-13 02:08:34.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
--rw-r--r--   0 stevevott   (501) staff       (20)    11323 2023-07-13 02:08:21.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-07-27 17:34:43.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
--rw-r--r--   0 stevevott   (501) staff       (20)    14806 2023-07-27 17:34:10.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/test.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.942627 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/gfeatures.py
--rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/guseful.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.943460 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/
--rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/__init__.py
--rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
--rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
--rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
-drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-07-31 23:40:58.889559 RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/
--rw-r--r--   0 stevevott   (501) staff       (20)     5138 2023-07-31 23:40:58.000000 RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/PKG-INFO
--rw-r--r--   0 stevevott   (501) staff       (20)     8781 2023-07-31 23:40:58.000000 RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/SOURCES.txt
--rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-07-31 23:40:58.000000 RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/dependency_links.txt
--rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-31 23:40:58.000000 RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/top_level.txt
--rw-r--r--   0 stevevott   (501) staff       (20)      563 2023-07-31 23:40:32.000000 RamseyTheoryRL-0.78/pyproject.toml
--rw-r--r--   0 stevevott   (501) staff       (20)      154 2023-07-31 23:40:58.943912 RamseyTheoryRL-0.78/setup.cfg
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.330336 RamseyTheoryRL-0.79/
+-rw-r--r--   0 stevevott   (501) staff       (20)     1071 2023-07-03 02:47:52.000000 RamseyTheoryRL-0.79/LICENSE.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 03:58:20.000000 RamseyTheoryRL-0.79/MANIFEST.in
+-rw-r--r--   0 stevevott   (501) staff       (20)     5134 2023-08-02 21:32:02.330429 RamseyTheoryRL-0.79/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     4672 2023-07-24 16:38:37.000000 RamseyTheoryRL-0.79/README.md
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.273904 RamseyTheoryRL-0.79/RamseyTheoryRL/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:08:07.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.271869 RamseyTheoryRL-0.79/RamseyTheoryRL/data/
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.270808 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.280156 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/
+-rw-r--r--   0 stevevott   (501) staff       (20)   172832 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/all_leq6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)     4100 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_4.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)   163072 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_5.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)  1420327 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)    32697 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_7.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      240 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_9.csv
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.283880 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/
+-rw-r--r--   0 stevevott   (501) staff       (20)    62803 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/all_leq6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)     1811 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_4.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)    42779 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_5.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)   376715 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)    10322 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_7.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      129 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_9.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)   776505 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_4_4.csv
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.287171 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/
+-rw-r--r--   0 stevevott   (501) staff       (20)      112 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v35.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      117 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v36.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      123 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v37.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      130 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v38.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      136 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v39.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      142 2023-07-13 02:19:59.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/empty_graphs/v40.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.295118 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/
+-rw-r--r--   0 stevevott   (501) staff       (20)      161 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r34_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        7 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r34_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)   401300 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r34_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       87 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r35_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      304 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r35_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r39_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_10_35_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      727 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_6_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       69 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_6_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      756 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_7_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_7_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     3648 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_7_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)      196 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_8_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       77 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)   399016 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_8_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       65 2023-07-24 16:10:44.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_12_2_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       26 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_12_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       38 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_3_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       14 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_3_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       96 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_3_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)     1294 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_6_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    42316 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_6_path.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-24 16:11:31.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_9_35_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-27 00:29:49.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r4_6_35_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    47888 2023-07-15 16:54:40.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r5_5_42_isograph.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.304227 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/
+-rw-r--r--   0 stevevott   (501) staff       (20)        4 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_3_5_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_6_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       42 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_7_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       28 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_4_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       10 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_10_graph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1140 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2053 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_9_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1969 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_6_8_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_10_4_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       30 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_15_4_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    11973 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_4_12_isograph.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       20 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_8_3_isograph.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.306068 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       12 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       33 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      136 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      780 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     6264 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    86422 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph8.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.271717 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.307941 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       18 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       36 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       75 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_4/r34_8.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.310249 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     3130 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_10.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1260 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_11.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      156 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_12.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_13.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       52 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      160 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      426 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1253 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_8.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2320 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_9.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.312990 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    66570 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_10.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      175 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_17.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       56 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      185 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      600 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2492 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_8.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    11256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_9.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.313139 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_7/
+-rw-r--r--   0 stevevott   (501) staff       (20)     7831 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_7/r37_22.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.313294 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_9/
+-rw-r--r--   0 stevevott   (501) staff       (20)      102 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_9/r39_35.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.315827 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    12800 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_15.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       44 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_16.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       25 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_17.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       12 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       27 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       96 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      420 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2172 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    14553 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_8.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)   117608 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_9.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.316106 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_6/
+-rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_6/r46_35some.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.316347 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/5_5/
+-rw-r--r--   0 stevevott   (501) staff       (20)    47888 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/5_5/r55_42some.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.317984 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/
+-rw-r--r--   0 stevevott   (501) staff       (20)      124 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_all_leq6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      186 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_igraph_all_leq9.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      192 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_3_4.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      304 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_3_5.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_3_6.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)       32 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_3_7.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)       32 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_3_9.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)      261 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_4_4.csv
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/time/time_ramsey_4_5.csv
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.318084 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r(4,6,36)_graph.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.319518 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       18 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       36 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       75 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       54 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r34/r34_8.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.322747 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     3130 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_10.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      156 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_12.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_13.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       52 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      160 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      426 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     1253 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_8.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2320 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_9.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.325778 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/
+-rw-r--r--   0 stevevott   (501) staff       (20)        2 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_1.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      175 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_17.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        6 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_2.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)        9 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_3.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       21 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_4.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)       56 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_5.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      185 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_6.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)      600 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_7.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)     2492 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_8.g6
+-rw-r--r--   0 stevevott   (501) staff       (20)    11256 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_9.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.326143 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r46/
+-rw-r--r--   0 stevevott   (501) staff       (20)     3774 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r46/r46_35some.g6
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.326407 RamseyTheoryRL-0.79/RamseyTheoryRL/src/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:40.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/__init__.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.327621 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:29:39.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    12523 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/gbfs.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3539 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1070 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/igraph_train_gen.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1157 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/isofile_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3365 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/train_gen.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.328644 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 03:03:49.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     5761 2023-08-01 23:28:57.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    11323 2023-07-13 02:08:21.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     8240 2023-08-01 23:28:55.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py
+-rw-r--r--   0 stevevott   (501) staff       (20)    14806 2023-08-01 21:59:15.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/test.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.329252 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     3529 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/gfeatures.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     4581 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/guseful.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.330169 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/
+-rw-r--r--   0 stevevott   (501) staff       (20)        0 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/__init__.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      398 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/create_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     1686 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py
+-rw-r--r--   0 stevevott   (501) staff       (20)      383 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/test_heuristic.py
+-rw-r--r--   0 stevevott   (501) staff       (20)     2168 2023-07-03 02:41:12.000000 RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py
+drwxr-xr-x   0 stevevott   (501) staff       (20)        0 2023-08-02 21:32:02.274430 RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/
+-rw-r--r--   0 stevevott   (501) staff       (20)     5134 2023-08-02 21:32:02.000000 RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/PKG-INFO
+-rw-r--r--   0 stevevott   (501) staff       (20)     8781 2023-08-02 21:32:02.000000 RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/SOURCES.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)        1 2023-08-02 21:32:02.000000 RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/dependency_links.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)       15 2023-08-02 21:32:02.000000 RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/top_level.txt
+-rw-r--r--   0 stevevott   (501) staff       (20)      559 2023-08-02 21:31:22.000000 RamseyTheoryRL-0.79/pyproject.toml
+-rw-r--r--   0 stevevott   (501) staff       (20)      154 2023-08-02 21:32:02.330703 RamseyTheoryRL-0.79/setup.cfg
```

### Comparing `RamseyTheoryRL-0.78/LICENSE.txt` & `RamseyTheoryRL-0.79/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/PKG-INFO` & `RamseyTheoryRL-0.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.78
+Version: 0.79
 Summary: Ramsey Number Explorer
-Author-email: Steve Vott <svott03@gmail.com>, Adam Lehavi <alehavi@usc.edu>
+Author-email: Steve Vott <svott@usc.edu>, Adam Lehavi <alehavi@usc.edu>
 Project-URL: Homepage, https://github.com/aLehav/RamseyTheoryRL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `RamseyTheoryRL-0.78/README.md` & `RamseyTheoryRL-0.79/README.md`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/all_leq6.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/all_leq6.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_4.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_4.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_5.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_5.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_6.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_6.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/scaled/ramsey_3_7.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/scaled/ramsey_3_7.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/all_leq6.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/all_leq6.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_4.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_4.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_5.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_5.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_6.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_6.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_3_7.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_3_7.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/csv/unscaled/ramsey_4_4.csv` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/csv/unscaled/ramsey_4_4.csv`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r34_path.txt` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r34_path.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_6_graph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_6_graph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_7_graph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_7_graph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_7_path.txt` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_7_path.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_4_8_path.txt` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_4_8_path.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_6_graph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_6_graph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r3_5_6_path.txt` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r3_5_6_path.txt`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r4_6_35_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r4_6_35_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/r5_5_42_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/r5_5_42_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_8_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_8_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_9_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_5_9_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_6_8_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r3_6_8_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_4_12_isograph.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/found_counters/scaled_dnn/r4_4_12_isograph.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph6.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph6.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph7.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph7.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/isomorphic_by_n/graph8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/isomorphic_by_n/graph8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_10.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_10.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_11.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_11.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_9.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_5/r35_9.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_10.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_10.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_7.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_7.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_9.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_6/r36_9.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/3_7/r37_22.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/3_7/r37_22.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_15.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_15.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_7.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_7.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_9.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_4/r44_9.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/4_6/r46_35some.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/4_6/r46_35some.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/ramsey_s_t_n/5_5/r55_42some.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/ramsey_s_t_n/5_5/r55_42some.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_10.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_10.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r35/r35_9.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r35/r35_9.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_7.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_7.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_8.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_8.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r36/r36_9.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r36/r36_9.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/data/visualization_work/r46/r46_35some.g6` & `RamseyTheoryRL-0.79/RamseyTheoryRL/data/visualization_work/r46/r46_35some.g6`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/gbfs.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/gbfs.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/heuristic.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/igraph_train_gen.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/igraph_train_gen.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/isofile_checker.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/isofile_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/models/train_gen.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/models/train_gen.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_multi_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/ramsey_checker_single_thread.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/ramsey_checker/test.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/ramsey_checker/test.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/gfeatures.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/gfeatures.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/guseful.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/guseful.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/handle_neptune.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py` & `RamseyTheoryRL-0.79/RamseyTheoryRL/src/utils/heuristic/train_heuristic.py`

 * *Files identical despite different names*

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/PKG-INFO` & `RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RamseyTheoryRL
-Version: 0.78
+Version: 0.79
 Summary: Ramsey Number Explorer
-Author-email: Steve Vott <svott03@gmail.com>, Adam Lehavi <alehavi@usc.edu>
+Author-email: Steve Vott <svott@usc.edu>, Adam Lehavi <alehavi@usc.edu>
 Project-URL: Homepage, https://github.com/aLehav/RamseyTheoryRL
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `RamseyTheoryRL-0.78/RamseyTheoryRL.egg-info/SOURCES.txt` & `RamseyTheoryRL-0.79/RamseyTheoryRL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

