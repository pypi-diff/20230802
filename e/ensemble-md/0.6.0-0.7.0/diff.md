# Comparing `tmp/ensemble_md-0.6.0.tar.gz` & `tmp/ensemble_md-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensemble_md-0.6.0.tar", last modified: Mon May  1 20:24:45 2023, max compression
+gzip compressed data, was "ensemble_md-0.7.0.tar", last modified: Wed Aug  2 21:50:06 2023, max compression
```

## Comparing `ensemble_md-0.6.0.tar` & `ensemble_md-0.7.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.058627 ensemble_md-0.6.0/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3557 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1069 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/LICENSE
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      145 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/MANIFEST.in
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3017 2023-05-01 20:24:45.058929 ensemble_md-0.6.0/PKG-INFO
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1605 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/README.md
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.060784 ensemble_md-0.6.0/ensemble_md/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      339 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/__init__.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      497 2023-05-01 20:24:45.061053 ensemble_md-0.6.0/ensemble_md/_version.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.021900 ensemble_md-0.6.0/ensemble_md/analysis/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14013 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_free_energy.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     9937 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_matrix.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    20028 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/analyze_traj.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5451 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/analysis/msm_analysis.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.024212 ensemble_md-0.6.0/ensemble_md/cli/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    21672 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/analyze_EEXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5516 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/explore_EEXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    13152 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/cli/run_EEXE.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.025432 ensemble_md-0.6.0/ensemble_md/data/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1139 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/data/README.md
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      333 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/data/look_and_say.dat
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    62953 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/ensemble_EXE.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.031463 ensemble_md-0.6.0/ensemble_md/tests/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      113 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/__init__.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.035949 ensemble_md-0.6.0/ensemble_md/tests/data/
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.040769 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6769 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6739 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6731 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6749 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2200 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/expanded.mdp
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.053746 ensemble_md-0.6.0/ensemble_md/tests/data/log/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    38509 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32761 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_0.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_1.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32763 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_2.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_3.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7992 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/HREX.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    71966 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_1.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    65113 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_2.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    44910 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/log/case3.log
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)   113593 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/sys.gro
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2067 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/data/sys.top
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7426 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_analyze_matrix.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1424 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_analyze_traj.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32028 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_ensemble_EXE.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4495 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_gmx_parser.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3796 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/tests/test_utils.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.057897 ensemble_md-0.6.0/ensemble_md/utils/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      858 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/exceptions.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    16515 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/gmx_parser.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7954 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/ensemble_md/utils/utils.py
-drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-05-01 20:24:45.019121 ensemble_md-0.6.0/ensemble_md.egg-info/
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3017 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/PKG-INFO
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1576 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/SOURCES.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)        1 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/dependency_links.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      157 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/entry_points.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       94 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/requires.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       12 2023-05-01 20:24:44.000000 ensemble_md-0.6.0/ensemble_md.egg-info/top_level.txt
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      360 2023-05-01 20:24:45.060192 ensemble_md-0.6.0/setup.cfg
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4646 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/setup.py
--rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    68611 2023-05-01 19:22:32.000000 ensemble_md-0.6.0/versioneer.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.398903 ensemble_md-0.7.0/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3557 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1069 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/LICENSE
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      145 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/MANIFEST.in
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3251 2023-08-02 21:50:06.399083 ensemble_md-0.7.0/PKG-INFO
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1839 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/README.md
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.400217 ensemble_md-0.7.0/ensemble_md/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      339 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/__init__.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      497 2023-08-02 21:50:06.400324 ensemble_md-0.7.0/ensemble_md/_version.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.386523 ensemble_md-0.7.0/ensemble_md/analysis/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14013 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/analysis/analyze_free_energy.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    10036 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/analysis/analyze_matrix.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    34637 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/analysis/analyze_traj.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     5459 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/analysis/msm_analysis.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.387621 ensemble_md-0.7.0/ensemble_md/cli/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    22038 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/cli/analyze_EEXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7023 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/cli/explore_EEXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    14132 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/cli/run_EEXE.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.388267 ensemble_md-0.7.0/ensemble_md/data/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1139 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/data/README.md
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      333 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/data/look_and_say.dat
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    71385 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/ensemble_EXE.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.390559 ensemble_md-0.7.0/ensemble_md/tests/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      113 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/__init__.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.391782 ensemble_md-0.7.0/ensemble_md/tests/data/
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.393330 ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6769 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6739 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6731 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     6749 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2199 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/expanded.mdp
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.397171 ensemble_md-0.7.0/ensemble_md/tests/data/log/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    38509 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32761 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_0.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_1.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32763 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_2.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    32765 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_3.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7992 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/HREX.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    71966 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/case2_1.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    65113 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/case2_2.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    44910 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/log/case3.log
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)   113593 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/sys.gro
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     2067 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/data/sys.top
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     7426 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/test_analyze_matrix.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1424 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/test_analyze_traj.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    30067 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/test_ensemble_EXE.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4495 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/test_gmx_parser.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3751 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/tests/test_utils.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.398562 ensemble_md-0.7.0/ensemble_md/utils/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      858 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/utils/exceptions.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    16747 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/utils/gmx_parser.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     9902 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/ensemble_md/utils/utils.py
+drwxr-xr-x   0 Wei-TseHsu   (501) staff       (20)        0 2023-08-02 21:50:06.385056 ensemble_md-0.7.0/ensemble_md.egg-info/
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     3251 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/PKG-INFO
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     1576 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/SOURCES.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)        1 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/dependency_links.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      157 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/entry_points.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       94 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/requires.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)       12 2023-08-02 21:50:06.000000 ensemble_md-0.7.0/ensemble_md.egg-info/top_level.txt
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)      360 2023-08-02 21:50:06.399797 ensemble_md-0.7.0/setup.cfg
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)     4646 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/setup.py
+-rw-r--r--   0 Wei-TseHsu   (501) staff       (20)    68611 2023-08-02 21:49:52.000000 ensemble_md-0.7.0/versioneer.py
```

### Comparing `ensemble_md-0.6.0/CODE_OF_CONDUCT.md` & `ensemble_md-0.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/LICENSE` & `ensemble_md-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/PKG-INFO` & `ensemble_md-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemble_md
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package for setting up, performing, and analyzing molecular dynamics ensembles using GROMACS
 Author: Wei-Tse Hsu
 Author-email: wehs7661@colorado.edu
 License: MIT
 Project-URL: Documentation, https://ensemble-md.readthedocs.io/
 Project-URL: Source Code, https://github.com/wehs7661/ensemble_md
 Keywords: molecular mechanics,free energy calculations,advanced sampling
@@ -37,16 +37,18 @@
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Downloads](https://static.pepy.tech/badge/ensemble-md)](https://pepy.tech/project/ensemble-md)
+[![Twitter Follow](https://img.shields.io/twitter/follow/WeiTseHsu?style=social)](https://twitter.com/WeiTseHsu)
 
-**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
+**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble-md.readthedocs.io/en/latest/?badge=latest).
 
 ### Copyright
 
 Copyright (c) 2022, Wei-Tse Hsu
 
 
 #### Acknowledgements
```

### Comparing `ensemble_md-0.6.0/README.md` & `ensemble_md-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Downloads](https://static.pepy.tech/badge/ensemble-md)](https://pepy.tech/project/ensemble-md)
+[![Twitter Follow](https://img.shields.io/twitter/follow/WeiTseHsu?style=social)](https://twitter.com/WeiTseHsu)
 
-**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
+**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble-md.readthedocs.io/en/latest/?badge=latest).
 
 ### Copyright
 
 Copyright (c) 2022, Wei-Tse Hsu
 
 
 #### Acknowledgements
```

### Comparing `ensemble_md-0.6.0/ensemble_md/analysis/analyze_free_energy.py` & `ensemble_md-0.7.0/ensemble_md/analysis/analyze_free_energy.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/analysis/analyze_matrix.py` & `ensemble_md-0.7.0/ensemble_md/analysis/analyze_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
     log_file : str
         The log file to be parsed.
     expanded_ensemble : bool
         Whether the simulation is expanded ensemble or replica exchange
 
     Returns
     -------
-    empirical : numpy.ndarray
+    empirical : np.ndarray
         The final empirical state transition matrix.
-    theoretical : None or numpy.ndarray
+    theoretical : None or np.ndarray
         The final theoretical state transition matrix.
-    diff_matrix : None or numpy.ndarray
+    diff_matrix : None or np.ndarray
         The difference between the theortial and empirical state transition matrix (empirical - theoretical).
     """
     f = open(log_file, "r")
     lines = f.readlines()
     f.close()
 
     lines.reverse()
@@ -88,20 +88,20 @@
     doubly stochastic (replica exchange), or right stochastic (expanded ensemble). For the latter case,
     the staionary distribution vector is the left eigenvector corresponding to the eigenvalue 1
     of the transition matrix. (For the former case, it's either left or right eigenvector corresponding
     to the eigenvalue 1 - as the left and right eigenvectors are the same for a doubly stochasti matrix.)
 
     Parameters
     ----------
-    trans_mtx : numpy.ndarray
+    trans_mtx : np.ndarray
         The input state transition matrix
 
     Returns
     -------
-    equil_prob : numpy.ndarray
+    equil_prob : np.ndarray
     """
     check_row = sum([np.isclose(np.sum(trans_mtx[i]), 1) for i in range(len(trans_mtx))])
     check_col = sum([np.isclose(np.sum(trans_mtx[:, i]), 1) for i in range(len(trans_mtx))])
 
     if check_row == len(trans_mtx):  # note that this also include doubly stochastic matrices
         # Right or doubly stachstic matrices - calculate the left eigenvector
         eig_vals, eig_vecs = np.linalg.eig(trans_mtx.T)
@@ -118,32 +118,34 @@
     close_to_1_idx = np.isclose(eig_vals, 1, atol=1e-4)
     equil_prob = eig_vecs[:, close_to_1_idx]  # note that this is normalized
     equil_prob /= np.sum(equil_prob)   # So the sum of all components is 1
 
     return equil_prob
 
 
-def calc_spectral_gap(trans_mtx):
+def calc_spectral_gap(trans_mtx, atol=1e-8):
     """
     Calculates the spectral gap of the input transition matrix.
 
     Parameters
     ----------
-    trans_mtx : numpy.ndarray
+    trans_mtx : np.ndarray
         The input state transition matrix
+    atol: float
+        The absolute tolerance for checking the sum of columns and rows.
 
     Returns
     -------
     spectral_gap : float
-        The spectral gap of the input transition matrix
+        The spectral gap of the input transitio n matrix
     eig_vals : list
         The list of eigenvalues
     """
-    check_row = sum([np.isclose(np.sum(trans_mtx[i]), 1) for i in range(len(trans_mtx))])
-    check_col = sum([np.isclose(np.sum(trans_mtx[:, i]), 1) for i in range(len(trans_mtx))])
+    check_row = sum([np.isclose(np.sum(trans_mtx[i]), 1, atol=atol) for i in range(len(trans_mtx))])
+    check_col = sum([np.isclose(np.sum(trans_mtx[:, i]), 1, atol=atol) for i in range(len(trans_mtx))])
 
     if check_row == len(trans_mtx):
         eig_vals, eig_vecs = np.linalg.eig(trans_mtx.T)
     elif check_col == len(trans_mtx):
         eig_vals, eig_vecs = np.linalg.eig(trans_mtx)
     else:
         result_str = "The input transition matrix is neither right nor left stochastic, so the spectral gap cannot be calculated."  # noqa: E501
@@ -166,15 +168,15 @@
     difrerent alchemical ranges of different replicas. Notably, the function assumes
     homogeneous shifts and number of states across replicas. Also, the blocks of the
     transition matrix is generally not doubly stochastic but right stochastic even if
     the input is doubly stochastic.
 
     Parameters
     ----------
-    trans_mtx : numpy.ndarray
+    trans_mtx : np.ndarray
         The input state transition matrix to split
     n_sim : int
         The number of replicas in EEXE.
     n_sub : int
         The number of states for each replica.
 
     Returns
@@ -196,15 +198,15 @@
 
 def plot_matrix(matrix, png_name, title=None, start_idx=0):
     """
     Visualizes a matrix a in heatmap.
 
     Parameters
     ----------
-    matrix : numpy.ndarray
+    matrix : np.ndarray
         The matrix to be visualized
     png_name : str
         The file name of the output PNG file (including the extension).
     title : str
         The title of the plot
     start_idx : int
         The starting value of the state index
```

### Comparing `ensemble_md-0.6.0/ensemble_md/analysis/analyze_traj.py` & `ensemble_md-0.7.0/ensemble_md/cli/analyze_EEXE.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,497 +3,392 @@
 #    ensemble_md,                                                  #
 #    a python package for running GROMACS simulation ensembles     #
 #                                                                  #
 #    Written by Wei-Tse Hsu <wehs7661@colorado.edu>                #
 #    Copyright (c) 2022 University of Colorado Boulder             #
 #                                                                  #
 ####################################################################
-"""
-The :obj:`.analyze_traj` module provides methods for analyzing trajectories in EEXE.
-"""
+import os
+import sys
+import time
+import glob
+import pyemma
+import pymbar
+import pickle
+import natsort
+import argparse
+import warnings
 import numpy as np
 import matplotlib.pyplot as plt
-from matplotlib.ticker import MaxNLocator
-
-from alchemlyb.parsing.gmx import _get_headers as get_headers
-from alchemlyb.parsing.gmx import _extract_dataframe as extract_dataframe
-from ensemble_md.utils import utils
-
-
-def extract_state_traj(dhdl):
-    """
-    Extracts the state-space trajectory from a GROMACS DHDL file.
-    Note that the state indices here are local indices.
-
-    Parameters
-    ----------
-    dhdl : str
-        The filename of the GROMACS DHDL file to be parsed.
-
-    Returns
-    -------
-    traj : list
-        A list that represents that state-space trajectory
-    """
-    traj = list(extract_dataframe(dhdl, headers=get_headers(dhdl))['Thermodynamic state'])
-
-    return traj
-
-
-def stitch_trajs(files, rep_trajs, shifts=None, dhdl=True, col_idx=-1):
-    """
-    Stitches the state-space/CV-space trajectories for each configuration from DHDL files
-    or PLUMED output files generated at different iterations.
-
-    Parameters
-    ----------
-    files : list
-        A list of lists of file names of GROMACS DHDL files or general GROMACS XVG files or PLUMED ouptput files.
-        Specifically, :code:`files[i]` should be a list containing the files of interest from all iterations in
-        replica :code:`i`.
-    rep_trajs : list
-        A list of lists that represents the replica space trajectories for each configuration. For example,
-        :code:`rep_trajs[0] = [0, 2, 3, 0, 1, ...]` means that configuration 0 transitioned to replica 2, then
-        3, 0, 1, in iterations 1, 2, 3, 4, ..., respectively.
-    shifts : list
-        A list of values for shifting the state indices for each replica. The length of the list
-        should be equal to the number of replicas. This is only needed when :code:`dhdl=True`.
-    dhdl : bool
-        Whether the input files are GROMACS dhdl files, in which case trajectories of global alchemical indices
-        will be generated. If :code:`dhdl=False`, the input files must be readable by `numpy.loadtxt` assuming that
-        the start of a comment is indicated by either the :code:`#` or :code:`@` characters.
-        Such files include any GROMACS XVG files or PLUMED output files (output by plumed driver, for instance).
-        In this case, trajectories of the configurational collective variable of interest are generated.
-        The default is :code:`True`.
-    col_idx : int
-        The index of the column to be extracted from the input files. This is only needed when :code:`dhdl=False`,
-        By default, we extract the last column.
-
-    Returns
-    -------
-    trajs : list
-        A list that contains lists of state-space/CV-space trajectory (in global indices) for each configuration.
-        For example, :code:`trajs[i]` is the state-space/CV-space trajectory of configuration :code:`i`.
-    """
-    n_configs = len(files)  # number of starting configurations
-    n_iter = len(files[0])  # number of iterations per replica
-
-    # First figure out which dhdl/plumed output files each configuration corresponds to
-    # files_sorted[i] contains the dhdl/plumed output files for configuration i sorted based on iteration indices
-    files_sorted = [[] for i in range(n_configs)]
-    for i in range(n_configs):
-        for j in range(n_iter):
-            files_sorted[i].append(files[rep_trajs[i][j]][j])
-
-    # Then, stitch the trajectories for each configuration
-    trajs = [[] for i in range(n_configs)]  # for each configuration
-    for i in range(n_configs):
-        for j in range(n_iter):
-            if j == 0:
-                if dhdl:
-                    traj = extract_state_traj(files_sorted[i][j])
-                else:
-                    traj = np.loadtxt(files_sorted[i][j], comments=['#', '@'])[:, -1]
-            else:
-                # Starting from the 2nd iteration, we get rid of the first time frame the first
-                # frame of iteration n+1 the is the same as the last frame of iteration n
-                if dhdl:
-                    traj = extract_state_traj(files_sorted[i][j])[1:]
-                else:
-                    traj = np.loadtxt(files_sorted[i][j], comments=['#', '@'])[:, -1][1:]
-
-            if dhdl:  # Trajectories of global alchemical indices will be generated.
-                shift_idx = rep_trajs[i][j]
-                traj = list(np.array(traj) + shifts[shift_idx])
-            trajs[i].extend(traj)
-
-    return trajs
-
-
-def traj2transmtx(traj, N, normalize=True):
-    """
-    Computes the transition matrix given a trajectory. For example, if a state-space
-    trajectory from a EXE or HREX simulation given, a state transition matrix is returned.
-    If a trajectory showing transitions between replicas in a EEXE simulation is given,
-    a replica transition matrix is returned.
-
-    Parameters
-    ---------
-    traj : list
-        A list of state indices showing the trajectory in the state space.
-    N : int
-        The size (N) of the expcted transition matrix (N by N).
-    normalize : bool
-        Whether to normalize the matrix so that each row sum to 1. If False, then
-        the entries will be the counts of transitions.
-
-    Returns
-    -------
-    transmtx : numpy.ndarray
-        The transition matrix computed from the trajectory
-    """
-    transmtx = np.zeros([N, N])
-    for i in range(1, len(traj)):
-        transmtx[traj[i - 1], traj[i]] += 1   # counts of transitions
-    if normalize is True:
-        transmtx /= np.sum(transmtx, axis=1)[:, None]   # normalize the transition matrix
-        transmtx[np.isnan(transmtx)] = 0   # for non-sampled state, there could be nan due to 0/0
-
-    return transmtx
-
-
-def plot_rep_trajs(trajs, fig_name, dt=None, stride=None):
-    """
-    Plots the time series of replicas visited by each configuration in a single plot.
-
-    Parameters
-    ----------
-    trajs : list
-        A list of arrays that represent the replica space trajectories of all configurations.
-    fig_name : str
-        The file name of the png file to be saved (with the extension).
-    dt : float or None, optional
-        One trajectory timestep in ps. If None, it assumes there are no timeframes but MC steps.
-    stride : int, optional
-        The stride for plotting the time series. The default is 100 if the length of
-        any trajectory has more than one million frames. Otherwise, it will be 1. Typically
-        plotting more than 10 million frames can take a lot of memory.
-    """
-    n_sim = len(trajs)
-    cmap = plt.cm.ocean  # other good options are CMRmap, gnuplot, terrain, turbo, brg, etc.
-    colors = [cmap(i) for i in np.arange(n_sim) / n_sim]
-
-    if dt is None:
-        x = np.arange(len(trajs[0]))
+from matplotlib import rc
+from datetime import datetime
+from deeptime.markov.tools.analysis import is_transition_matrix
+warnings.simplefilter(action='ignore', category=UserWarning)
+
+from ensemble_md.utils import utils  # noqa: E402
+from ensemble_md.analysis import analyze_traj  # noqa: E402
+from ensemble_md.analysis import analyze_matrix  # noqa: E402
+from ensemble_md.analysis import msm_analysis  # noqa: E402
+from ensemble_md.analysis import analyze_free_energy  # noqa: E402
+from ensemble_md.ensemble_EXE import EnsembleEXE  # noqa: E402
+from ensemble_md.utils.exceptions import ParameterError  # noqa: E402
+
+
+def initialize(args):
+    parser = argparse.ArgumentParser(
+        description='This code analyzes an ensemble of expanded ensemble. Note that the template MDP\
+                file specified in the YAML file needs to be available in the working directory.')
+    parser.add_argument('-y',
+                        '--yaml',
+                        type=str,
+                        default='params.yaml',
+                        help='The input YAML file used to run the EEXE simulation. (Default: params.yaml)')
+    parser.add_argument('-o',
+                        '--output',
+                        type=str,
+                        default='analyze_EEXE_log.txt',
+                        help='The output log file that contains the analysis results of EEXE. \
+                            (Default: analyze_EEXE_log.txt)')
+    parser.add_argument('-rt',
+                        '--rep_trajs',
+                        type=str,
+                        default='rep_trajs.npy',
+                        help='The NPY file containing the replica-space trajectory. (Default: rep_trajs.npy)')
+    parser.add_argument('-st',
+                        '--state_trajs',
+                        type=str,
+                        default='state_trajs.npy',
+                        help='The NPY file containing the stitched state-space trajectory. \
+                            If the specified file is not found, the code will try to find all the trajectories and \
+                            stitch them. (Default: state_trajs.npy)')
+    parser.add_argument('-d',
+                        '--dir',
+                        default='analysis',
+                        help='The name of the folder for storing the analysis results.')
+    parser.add_argument('-m',
+                        '--maxwarn',
+                        type=int,
+                        default=0,
+                        help='The maximum number of warnings in parameter specification to be ignored.')
+    args_parse = parser.parse_args(args)
+
+    return args_parse
+
+
+def main():
+    t0 = time.time()
+    args = initialize(sys.argv[1:])
+    warnings.simplefilter(action='ignore', category=RuntimeWarning)
+    sys.stdout = utils.Logger(logfile=args.output)
+    sys.stderr = utils.Logger(logfile=args.output)
+    section_idx = 0
+    poor_sampling = None
+
+    rc('font', **{
+        'family': 'sans-serif',
+        'sans-serif': ['DejaVu Sans'],
+    })
+    # Set the font used for MathJax - more on this later
+    rc('mathtext', **{'default': 'regular'})
+    plt.rc('font', family='serif')
+
+    print(f'Current time: {datetime.now().strftime("%d/%m/%Y %H:%M:%S")}')
+    print(f'Command line: {" ".join(sys.argv)}')
+
+    EEXE = EnsembleEXE(args.yaml)
+    EEXE.print_params(params_analysis=True)
+
+    for i in EEXE.warnings:
+        print()
+        print(f'{i}')
+        print()
+
+    if len(EEXE.warnings) > args.maxwarn:
+        raise ParameterError(
+            f"The execution failed due to warning(s) about parameter spcificaiton. Consider setting maxwarn in the input YAML file if you want to ignore them.")  # noqa: E501, F541
+
+    # Check if the folder for saving the outputs exist. If not, create the folder.
+    if os.path.exists(args.dir) is False:
+        os.mkdir(args.dir)
+
+    print('\nData analysis of the simulation ensemble')
+    print('========================================')
+
+    # Section 1. Analysis based on transitions between alchemical ranges
+    print('[ Section 1. Analysis based on transitions between alchemical ranges ]')
+    section_idx += 1
+
+    # 1-0. Read in replica-space trajectories
+    print('1-0. Reading in the replica-space trajectory ...')
+    rep_trajs = np.load(args.rep_trajs)  # Shape: (n_sim, n_iter)
+
+    # 1-1. Plot the replica-sapce trajectory
+    print('1-1. Plotting transitions between alchemical ranges ...')
+    dt_swap = EEXE.nst_sim * EEXE.dt    # dt for swapping replicas
+    analyze_traj.plot_rep_trajs(rep_trajs, f'{args.dir}/rep_trajs.png', dt_swap)
+
+    # 1-2. Plot the replica-space transition matrix
+    print('1-2. Plotting the replica-space transition matrix (considering all continuous trajectories) ...')
+    counts = [analyze_traj.traj2transmtx(rep_trajs[i], EEXE.n_sim, normalize=False) for i in range(len(rep_trajs))]
+    reps_mtx = np.sum(counts, axis=0)  # First sum up the counts. This should be symmetric if n_ex=1. Otherwise it might not be. # noqa: E501
+    reps_mtx /= np.sum(reps_mtx, axis=1)[:, None]   # and then normalize each row
+    analyze_matrix.plot_matrix(reps_mtx, f'{args.dir}/rep_transmtx_allconfigs.png')
+
+    # 1-3. Calculate the spectral gap for the replica-space transition amtrix
+    spectral_gap, eig_vals = analyze_matrix.calc_spectral_gap(reps_mtx)
+    print(f'1-3. The spectral gap of the replica-space transition matrix: {spectral_gap:.3f}')
+
+    # Section 2. Analysis based on transitions between states
+    print('\n[ Section 2. Analysis based on transitions between states ]')
+    section_idx += 1
+
+    # 2-0. Recover all continuous trajectories
+    if os.path.isfile(args.state_trajs) is True:
+        print('2-0. Reading in the stitched state-space trajectory ...')
+        state_trajs = np.load(args.state_trajs)
     else:
-        x = np.arange(len(trajs[0])) * dt
-        if max(x) >= 10000:
-            x = x / 1000   # convert to ns
-            units = 'ns'
-        else:
-            units = 'ps'
-
-    if stride is None:
-        if len(trajs[0]) > 1000000:
-            stride = 100
-        else:
-            stride = 1
-
-    fig = plt.figure()
-    ax = fig.add_subplot(111)
-    for i in range(n_sim):
-        if len(trajs[0]) >= 100:  # don't show the markers
-            plt.plot(x[::stride], trajs[i][::stride], color=colors[i], label=f'Configuration {i}')
-        else:
-            plt.plot(x[::stride], trajs[i][::stride], color=colors[i], label=f'Configuration {i}', marker='o')
-
-    if dt is None:
-        plt.xlabel('MC moves')
-    else:
-        plt.xlabel(f'Time ({units})')
-
-    plt.ylabel('Replica')
-    plt.grid()
-    plt.legend()
-    ax.yaxis.set_major_locator(MaxNLocator(integer=True))
-    plt.savefig(f'{fig_name}', dpi=600)
-
-
-def plot_state_trajs(trajs, state_ranges, fig_name, dt=None, stride=1):
-    """
-    Plots the time series of states visited by each configuration in a subplot.
-
-    Parameters
-    ----------
-    trajs : list
-        A list of arrays that represent the state space trajectories of all configurations.
-    state_ranges : list
-        A list of lists of state indices. (Like the attribute :code:`state_ranges` in :code:`EnsemblEXE`.)
-    fig_name : str
-        The file name of the png file to be saved (with the extension).
-    dt : float or None, optional
-        The time interval between consecutive frames of the trajectories. If None, it is assumed
-        that the trajectories are in terms of Monte Carlo (MC) moves instead of timeframes, and
-        the x-axis label is set to 'MC moves'. Default is None.
-    stride : int, optional
-        The stride for plotting the time series. The default is 10 if the length of
-        any trajectory has more than 100,000 frames. Otherwise, it will be 1. Typically
-        plotting more than 10 million frames can take a lot of memory.
-    """
-    n_sim = len(trajs)
-    cmap = plt.cm.ocean  # other good options are CMRmap, gnuplot, terrain, turbo, brg, etc.
-    colors = [cmap(i) for i in np.arange(n_sim) / n_sim]
-
-    if dt is None:
-        x = np.arange(len(trajs[0]))
-    else:
-        x = np.arange(len(trajs[0])) * dt
-        if max(x) >= 10000:
-            x = x / 1000   # convert to ns
-            units = 'ns'
-        else:
-            units = 'ps'
-
-    if stride is None:
-        if len(trajs[0]) > 100000:
-            stride = 10
-        else:
-            stride = 1
-
-    # x_range = [-5, len(trajs[0]) - 1 + 5]
-    x_range = [np.min(x), np.max(x)]
-    y_range = [-0.2, np.max(trajs) + 0.2]
-    n_configs = len(trajs)
-    n_rows, n_cols = utils.get_subplot_dimension(n_configs)
-    _, ax = plt.subplots(nrows=n_rows, ncols=n_cols, figsize=(2.5 * n_cols, 2.5 * n_rows))
-    for i in range(n_configs):
-        plt.subplot(n_rows, n_cols, i + 1)
-
-        # First color different regions showing alchemical ranges
-        for j in range(n_configs):
-            bounds = [list(state_ranges[j])[0], list(state_ranges[j])[-1]]
-            if j == 0:
-                bounds[0] -= 0.5
-            if j == n_configs - 1:
-                bounds[1] += 0.5
-            plt.fill_between(x_range, y1=bounds[1], y2=bounds[0], color=colors[j], alpha=0.1)
-
-        if len(trajs[0]) > 100000:
-            linewidth = 0.01
-        else:
-            linewidth = 1  # this is the default
-
-        # Finally, plot the trajectories
-        linewidth = 1  # this is the default
-        plt.plot(x[::stride], trajs[i][::stride], color=colors[i], linewidth=linewidth)
-        if dt is None:
-            plt.xlabel('MC moves')
-        else:
-            plt.xlabel(f'Time ({units})')
-
-        plt.ylabel('State')
-        plt.title(f'Configuration {i}', fontweight='bold')
-        if len(trajs[0]) >= 10000:
-            plt.ticklabel_format(style='sci', axis='x', scilimits=(0, 0))
-        plt.xlim(x_range)
-        plt.ylim(y_range)
-        plt.grid()
-
-    # Remove redundant subplots
-    n_rm = n_cols * n_rows - n_configs
-    for i in range(n_rm):
-        ax.flat[-1 * (i + 1)].set_visible(False)
-
-    plt.tight_layout()
-    plt.savefig(f'{fig_name}', dpi=600)
-
-
-def plot_state_hist(trajs, state_ranges, fig_name):
-    """
-    Plots the histograms of the state index for each configuration.
-
-    Parameters
-    ----------
-    trajs : list
-         A list of arrays that represent the state space trajectories of all configurations.
-    state_ranges : list
-        A list of lists of state indices. (Like the attribute :code:`state_ranges` in :obj:`.EnsembleEXE`.)
-    fig_name : str
-        The file name of the png file to be saved (with the extension).
-    """
-    n_configs = len(trajs)
-    cmap = plt.cm.ocean  # other good options are CMRmap, gnuplot, terrain, turbo, brg, etc.
-    colors = [cmap(i) for i in np.arange(n_configs) / n_configs]
-
-    fig = plt.figure()
-    ax = fig.add_subplot(111)
-    lower_bound = min(trajs[0]) - 0.5
-    upper_bound = max(trajs[-1]) + 0.5
-    for i in range(len(trajs)):
-        plt.hist(trajs[i], np.arange(lower_bound, upper_bound + 1, 1), label=f'Configuration {i}', alpha=0.5, edgecolor='black', color=colors[i])  # noqa: E501
-    plt.xticks(range(max(state_ranges[-1]) + 1))
-
-    # Here we color the different regions to show alchemical ranges
-    y_min, y_max = ax.get_ylim()
-    for i in range(n_configs):
-        bounds = [list(state_ranges[i])[0], list(state_ranges[i])[-1]]
-        if i == 0:
-            bounds[0] -= 0.5
-        if i == n_configs - 1:
-            bounds[1] += 0.5
-        plt.fill_betweenx([y_min, y_max], x1=bounds[1] + 0.5, x2=bounds[0] - 0.5, color=colors[i], alpha=0.1, zorder=0)
-    plt.xlim([lower_bound, upper_bound])
-    plt.ylim([y_min, y_max])
-    plt.xlabel('State index')
-    plt.ylabel('Count')
-    plt.grid()
-    plt.legend()
-    plt.savefig(f'{fig_name}', dpi=600)
-
-
-def plot_transit_time(trajs, N, fig_prefix=None, dt=None, folder='.'):
-    """
-    Caclulcates and plots the average transit times for each configuration, including the time
-    it takes from states 0 to k, from k to 0 and from 0 to k back to 0 (i.e. round-trip time).
-    If there are more than 100 round-trips, 3 histograms corresponding to t_0k, t_k0 and t_roundtrip
-    will be generated.
-
-    Parameters
-    ----------
-    trajs : list
-        A list of arrays that represent the state space trajectories of all configurations.
-    N : int
-        The total number of states in the whole alchemical range.
-    fig_prefix : str
-        A prefix to use for all generated figures.
-    dt : float or None, optional
-        One trajectory timestep in ps. If None, it assumes there are no timeframes but MC steps.
-    folder : str, optional
-        The directory for saving the figures
-
-    Returns
-    -------
-    t_0k_list : list
-        A list of transit time from states 0 to k for each configuration.
-    t_k0_list : list
-        A list of transit time from states k to 0 for each configuration.
-    t_roundtrip_list : list
-        A list of round-trip times for each configuration.
-    units : str
-        The units of the times.
-    """
-    if dt is None:
-        x = np.arange(len(trajs[0]))
-        units = 'step'
+        # This may take a while.
+        print('2-0. Stitching trajectories for each starting configuration from dhdl files ...')
+        dhdl_files = [natsort.natsorted(glob.glob(f'sim_{i}/iteration_*/*dhdl*xvg')) for i in range(EEXE.n_sim)]
+        shifts = np.arange(EEXE.n_sim) * EEXE.s
+        state_trajs = analyze_traj.stitch_trajs(dhdl_files, rep_trajs, shifts=shifts, save=True)  # length: the number of replicas  # noqa: E501
+
+    # 2-1. Plot the state-space trajectory
+    print('\n2-1. Plotting transitions between different alchemical states ...')
+    dt_traj = EEXE.dt * EEXE.template['nstdhdl']  # in ps
+    analyze_traj.plot_state_trajs(state_trajs, EEXE.state_ranges, f'{args.dir}/state_trajs.png', dt_traj)
+
+    # 2-2. Plot the histograms for the states
+    print('\n2-2. Plotting the histograms of the state index ...')
+    analyze_traj.plot_state_hist(state_trajs, EEXE.state_ranges, f'{args.dir}/state_hist.png')
+
+    # 2-3. Plot the overall state transition matrices calculated from the state-space trajectories
+    print('\n2-3. Plotting the overall state transition matrices ...')
+    mtx_list = []
+    for i in range(EEXE.n_sim):
+        mtx = analyze_traj.traj2transmtx(state_trajs[i], EEXE.n_tot)
+        mtx_list.append(mtx)
+        analyze_matrix.plot_matrix(mtx, f'{args.dir}/traj_{i}_state_transmtx.png')
+
+    # 2-4. For each configurration, calculate the spectral gap of the overall transition matrix obtained in step 2-2.
+    print('\n2-4. Calculating the spectral gap of the state transition matrices ...')
+    results = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]  # a list of tuples
+    spectral_gaps = [results[i][0] if None not in results else None for i in range(len(results))]
+    eig_vals = [results[i][1] if None not in results else None for i in range(len(results))]
+    if None not in spectral_gaps:
+        for i in range(EEXE.n_sim):
+            print(f'   - Trajectory {i}: {spectral_gaps[i]:.3f} (λ_1: {eig_vals[i][0]:.5f}, λ_2: {eig_vals[i][1]:.5f})')  # noqa: E501
+        print(f'   - Average of the above: {np.mean(spectral_gaps):.3f} (std: {np.std(spectral_gaps, ddof=1):.3f})')
+
+    # 2-5. For each trajectory, calculate the stationary distribution from the overall transition matrix obtained in step 2-2.  # noqa: E501
+    print('\n2-5. Calculating the stationary distributions ...')
+    pi_list = [analyze_matrix.calc_equil_prob(mtx) for mtx in mtx_list]
+    if any([x is None for x in pi_list]):
+        pass  # None is in the list
     else:
-        x = np.arange(len(trajs[0])) * dt
-        if max(x) >= 10000:
-            x = x / 1000   # convert to ns
-            units = 'ns'
-        else:
-            units = 'ps'
-
-    # The lists below are for storing data corresponding to different configurations.
-    t_0k_list, t_k0_list, t_roundtrip_list = [], [], []
-    t_0k_avg, t_k0_avg, t_roundtrip_avg = [], [], []
-
-    sci = False  # whether to use scientific notation in the y-axis in the plot
-    for i in range(len(trajs)):
-        traj = trajs[i]
-        last_visited = None   # last visited end
-        k = N - 1
-        t_0, t_k = [], []   # time frames visting states 0 and k (k is the other end)
-
-        # time spent from statkes 0 to k, k to 0 and the round-trip time (from 0 to k to 0)
-        t_0k, t_k0, t_roundtrip = [], [], []
-
-        end_0_found, end_k_found = None, None
-        for t in range(len(traj)):
-            if traj[t] == 0:
-                end_0_found = True
-                if last_visited != 0:
-                    t_0.append(t)
-                    if last_visited == k:
-                        t_k0.append(t - t_k[-1])
-                last_visited = 0
-            if traj[t] == k:
-                end_k_found = True
-                if last_visited != k:
-                    t_k.append(t)
-                    if last_visited == 0:
-                        t_0k.append(t - t_0[-1])
-                last_visited = k
-
-        # Here we figure out the round-trip time from t_0k and t_k0.
-        if len(t_0k) != len(t_k0):   # then it must be len(t_0k) = len(t_k0) + 1 or len(t_k0) = len(t_0k) + 1, so we drop the last element of the larger list  # noqa: E501
-            if len(t_0k) > len(t_k0):
-                t_0k.pop()
+        for i in range(EEXE.n_sim):
+            print(f'   - Trajectory {i}: {", ".join([f"{j:.3f}" for j in pi_list[i].reshape(-1)])}')
+        if len({len(i) for i in pi_list}) == 1:  # all lists in pi_list have the same length
+            print(f'   - Average of the above: {", ".join([f"{i:.3f}" for i in np.mean(pi_list, axis=0).reshape(-1)])}')  # noqa: E501
+
+    # 2-6. Calculate the state index correlation time for each trajectory (this step is more time-consuming one)
+    print('\n2-6. Calculating the state index correlation time ...')
+    tau_list = [(pymbar.timeseries.statistical_inefficiency(state_trajs[i], fast=True) - 1) / 2 * dt_traj for i in range(EEXE.n_sim)]  # noqa: E501
+    for i in range(EEXE.n_sim):
+        print(f'   - Trajectory {i}: {tau_list[i]:.1f} ps')
+    print(f'   - Average of the above: {np.mean(tau_list):.1f} ps (std: {np.std(tau_list, ddof=1):.1f} ps)')
+
+    # 2-7. Calculate transit times for each trajectory
+    print('\n2-7. Plotting the average transit times ...')
+    t_0k_list, t_k0_list, t_roundtrip_list, units = analyze_traj.plot_transit_time(state_trajs, EEXE.n_tot, dt=dt_traj, folder=args.dir)  # noqa: E501
+    meta_list = [t_0k_list, t_k0_list, t_roundtrip_list]
+    t_names = [
+        '\n   - Average transit time from states 0 to k',
+        '\n   - Average transit time from states k to 0',
+        '\n   - Average round-trip time',
+    ]
+    for i in range(len(meta_list)):
+        t_list = meta_list[i]
+        print(t_names[i])
+        for j in range(len(t_list)):
+            if t_list[j] is None:
+                print(f'     - Trajectory {j}: Skipped')
             else:
-                t_k0.pop()
-        t_roundtrip = list(np.array(t_0k) + np.array(t_k0))
+                print(f'     - Trajectory {j} ({len(t_list[j])} events): {np.mean(t_list[j]):.2f} {units}')
+        print(f'     - Average of the above: {np.mean([np.mean(i) for i in t_list]):.2f} {units} (std: {np.std([np.mean(i) for i in t_list], ddof=1):.2f} {units})')  # noqa: E501
 
-        if end_0_found is True and end_k_found is True:
-            if dt is not None:
-                units = 'ps'
-                t_0k = list(np.array(t_0k) * dt)  # units: ps
-                t_k0 = list(np.array(t_k0) * dt)  # units: ps
-                t_roundtrip = list(np.array(t_roundtrip) * dt)  # units: ps
-                if np.max([t_0k, t_k0, t_roundtrip]) >= 10000:
-                    units = 'ns'
-                    t_0k = list(np.array(t_0k) / 1000)   # units: ns
-                    t_k0 = list(np.array(t_k0) / 1000)   # units: ns
-                    t_roundtrip = list(np.array(t_roundtrip) / 1000)   # units: ns
-
-            t_0k_list.append(t_0k)
-            t_0k_avg.append(np.mean(t_0k))
+    if np.sum(np.isnan([np.mean(i) for i in t_list])) != 0:
+        poor_sampling = True
 
-            t_k0_list.append(t_k0)
-            t_k0_avg.append(np.mean(t_k0))
+    if EEXE.msm is True:
+        section_idx += 1
 
-            t_roundtrip_list.append(t_roundtrip)
-            t_roundtrip_avg.append(np.mean(t_roundtrip))
-
-            if sci is False and np.max([t_0k, t_k0, t_roundtrip]) >= 10000:
-                sci = True
-        else:
-            t_0k_list.append([])
-            t_k0_list.append([])
-            t_roundtrip_list.append([])
-
-    # Now we plot! (If there are no events, the figures will just be blank)
-    meta_list = [t_0k_list, t_k0_list, t_roundtrip_list]
-    y_labels = [
-        f'Average transit time from states 0 to k ({units})',
-        f'Average transit time from states k to 0 ({units})',
-        f'Average round-trip time ({units})',
-    ]
-    fig_names = ['t_0k.png', 't_k0.png', 't_roundtrip.png']
-    for t in range(len(meta_list)):
-        t_list = meta_list[t]
-        if all(not x for x in t_list):
-            # If the nested list is empty, no plots will be generated.
-            pass
-        else:
-            len_list = [len(i) for i in t_list]
-            if np.max(len_list) <= 10:
-                marker = 'o'
+        # Section 3. Analysis based on Markov state models
+        print('\n[ Section 3. Analysis based on Markov state models ]')
+
+        # 3-1. Plot the implied timescale as a function of lag time
+        print('\n3-1. Plotting the implied timescale as a function of lag time for all trajectories ...')
+        lags = np.arange(EEXE.lag_spacing, EEXE.lag_max + EEXE.lag_spacing, EEXE.lag_spacing)
+        # lags could also be None and decided automatically. Could consider using that.
+        ts_list = msm_analysis.plot_its(state_trajs, lags, fig_name=f'{args.dir}/implied_timescales.png', dt=dt_traj, units='ps')  # noqa: E501
+
+        # 3-2. Decide a lag time for building MSM
+        print('\n3-2. Calculating recommended lag times for building MSMs ...')
+        chosen_lags = msm_analysis.decide_lagtimes(ts_list)
+        print('     \nSuggested lag times for each trajectory:')
+        for i in range(len(chosen_lags)):
+            print(f'       - Trajectory {i}: {chosen_lags[i] * dt_traj:.1f} ps')
+
+        # 3-3. Build a Bayesian MSM and perform a CK test for each trajectory to validate the models
+        print('\n3-3. Building Bayesian MSMs for the state-space trajectory for each trajectory ...')
+        print('     Performing a Chapman-Kolmogorov test on each trajectory ...')
+        models = [pyemma.msm.bayesian_markov_model(state_trajs[i], chosen_lags[i], dt_traj=f'{dt_traj} ps', show_progress=False) for i in range(EEXE.n_sim)]  # noqa: E501
+
+        for i in range(len(models)):
+            print(f'     Plotting the CK-test results for trajectory {i} ...')
+            mlags = 5  # this maps to 5 (mlags: multiples of lag times for testing the model)
+            nsets = models[i].nstates  # number of metastable states.
+            # Note that nstates is the number of unique states in the input trajectores counted with the effective mode
+            # (see the documentation) Therefore, if a system barely sampled some of the states, those states will
+            # not be counted as involved in the transition matrix (i.e. not in the active set). To check the
+            # active states, use models[i].active_set. If the system sampled all states frequently,
+            # models[i].active_set should be equal to np.unique(state_trajs[i]) and both lengths should be
+            # EEXE.n_tot. I'm not sure why the attribute nstates_full is not always EEXE.n_tot but is less
+            # relevant here.
+            cktest = models[i].cktest(nsets=nsets, mlags=mlags, show_progress=False)
+            pyemma.plots.plot_cktest(cktest, dt=dt_traj, units='ps')
+            plt.tight_layout(rect=[0, 0.03, 1, 0.98])
+            plt.savefig(f'{args.dir}/traj_{i}_CKtest.png', dpi=600)
+
+        # Additionally, check if the sampling is poor for each trajectory
+        for i in range(len(models)):
+            if models[i].nstates != EEXE.n_tot:
+                print(f'     Note: The sampling of trajectory {i} was poor.')
+
+        # 3-4. Plot the state transition matrices estimated with the specified lag times in MSMs
+        print('\n3-4. Plotting the overall transition matrices for all trajectories and their average ...')
+        mtx_list = [m.transition_matrix for m in models]
+        mtx_list_modified = []  # just for plotting (if all trajs sampled the fulle range frequently, this will be the same as mtx_list)  # noqa: E501
+        for i in range(len(mtx_list)):
+            # check if each mtx in mtx_list spans the full alchemical range. (If the system did not visit
+            # certain states, the dimension will be less than EEXE.n_tot * EEXE.n_tot. In this case, we
+            # add rows and columns of 0. Note that the modified matrix will not be a transition matrix,
+            # so this is only for plotting. For later analysis such as spectral gap calculation, we
+            # will just use the unmodified matrices.
+            if mtx_list[i].shape != (EEXE.n_tot, EEXE.n_tot):  # add rows and columns of 0
+                sampled = models[i].active_set
+                missing = list(set(range(EEXE.n_tot)) - set(sampled))  # states not visited
+
+                # figure out which end we should stack rows/columns to
+                n_1 = sum(missing > max(sampled))   # add rows/columns to the end of large state indices
+                n_2 = sum(missing < min(sampled))   # add rows/columns to the end of small state indices
+
+                # Below we first add a column and a row and so on
+                mtx = mtx_list[i]
+                for j in range(n_1):
+                    d = mtx.shape[0]  # size of the square matrix
+                    mtx = np.hstack((mtx, np.zeros([d, 1])))
+                    mtx = np.vstack((mtx, np.zeros([1, d + 1])))
+                for j in range(n_2):
+                    d = mtx.shape[0]  # size of the square matrix
+                    mtx = np.hstack((np.zeros([d, 1]), mtx))
+                    mtx = np.vstack((np.zeros([1, d + 1]), mtx))
+                mtx_list_modified.append(mtx)
             else:
-                marker = ''
+                mtx_list_modified.append(mtx_list[i])
 
-            plt.figure()
-            for i in range(len(t_list)):    # t_list[i] is the list for configuration i
-                plt.plot(np.arange(len(t_list[i])) + 1, t_list[i], label=f'Configuration {i}', marker=marker)
-            if np.array(t_list).shape != (1, 0):  # at least one configuration has at least one event
-                if np.max(np.max((t_list))) >= 10000:
-                    plt.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
-            plt.xlabel('Event index')
-            plt.ylabel(f'{y_labels[t]}')
-            plt.grid()
-            plt.legend()
-            if fig_prefix is None:
-                plt.savefig(f'{folder}/{fig_names[t]}')
-            else:
-                plt.savefig(f'{folder}/{fig_prefix}_{fig_names[t]}', dpi=600)
+        avg_mtx = np.mean(mtx_list_modified, axis=0)
+        print('     Saving transmtx.npy (plotted transition matrices)...')
+        np.save(f'{args.dir}/transmtx.npy', mtx_list_modified)
+
+        for i in range(EEXE.n_sim):
+            analyze_matrix.plot_matrix(mtx_list[i], f'{args.dir}/traj_{i}_state_transmtx_msm.png')
+        analyze_matrix.plot_matrix(avg_mtx, f'{args.dir}/state_transmtx_avg_msm.png')
+
+        # Note that if a trajectory never visited a certain replica, the rows in the alchemical range of that
+        # replica will only have 0 entries. Below we check if this is the case.
+        print('     Checking the sum of each row of each transition matrix is 1 ...')
+        is_transmtx = [is_transition_matrix(i) for i in mtx_list]
+        for i in range(len(is_transmtx)):
+            if is_transmtx[i] is False:
+                print(f'     The sums of the rows are not 1 (but {np.sum(mtx_list[i], axis=1)}) for the transition matrix of trajectory {i}.')  # noqa: E501
+
+        # 3-5. Calculate the spectral gap from the transition matrix of each trajectory
+        print('\n3-5. Calculating the spectral gap of the state transition matrices obtained from MSMs ...')
+        spectral_gaps, eig_vals = [analyze_matrix.calc_spectral_gap(mtx) for mtx in mtx_list]
+        for i in range(EEXE.n_sim):
+            print(f'       - Trajectory {i}: {spectral_gaps[i]:.3f}')
+
+        # 3-6. Calculate the stationary distribution for each trajectory
+        print('\n3-6. Calculating the stationary distributions from the transition matrices obtained from MSMs ...')
+        pi_list = [m.pi for m in models]
+        for i in range(EEXE.n_sim):
+            print(f'       - Trajectory {i}: {", ".join([f"{j:.3f}" for j in pi_list[i]])}')
+        if len({len(i) for i in pi_list}) == 1:  # all lists in pi_list have the same length
+            print(f'       - Average of the above: {", ".join([f"{i:.3f}" for i in np.mean(pi_list, axis=0)])}')
+
+        # 3-7. Calculate the mean first-passage time (MFPT) from each MSM
+        print('\n3-7. Calculating the mean first-passage times (MFPTs) ...')
+        # note that it's not m.mfpt(min(m.active_set), max(m.active_set)) as the input to mfpt should be indices
+        # though sometimes these two could be same.
+        mfpt_list = [m.mfpt(0, m.nstates - 1) for m in models]
+        for i in range(EEXE.n_sim):
+            print(f'       - Trajectory {i}: {mfpt_list[i]:.1f} ps')
+        print(f'       - Average of the above: {np.mean(mfpt_list):.1f} ps (std: {np.std(mfpt_list, ddof=1):.1f} ps)')
+
+        # 3-8. Calculate the state index correlation time for each trajectory
+        print('\n3-8. Plotting the state index correlation times for all trajectories ...')
+        msm_analysis.plot_acf(models, EEXE.n_tot, f'{args.dir}/state_ACF.png')
+
+    # Section 4 (or Section 3). Free energy calculations
+    if EEXE.free_energy is True:
+        if poor_sampling is True:
+            print('\nFree energy calculation is not performed since the sampling appears poor.')
+            sys.exit()
+        section_idx += 1
+        print(f'\n[ Section {section_idx}. Free energy calculations ]')
+
+        u_nk_list, dHdl_list = [], []
+
+        if os.path.isfile(f'{args.dir}/u_nk_data.pickle') is True:
+            print('Loading the preprocessed data u_nk ...')
+            with open(f'{args.dir}/u_nk_data.pickle', 'rb') as handle:
+                u_nk_list = pickle.load(handle)
+
+        if os.path.isfile(f'{args.dir}/dHdl_data.pickle') is True:
+            print('Loading the preprocessed data dHdl ...')
+            with open(f'{args.dir}/dHdl_data.pickle', 'rb') as handle:
+                dHdl_list = pickle.load(handle)
+
+        if u_nk_list == [] and dHdl_list == []:
+            for i in range(EEXE.n_sim):
+                print(f'Reading dhdl files of alchemical range {i} ...')
+                files = natsort.natsorted(glob.glob(f'sim_{i}/iteration_*/*dhdl*xvg'))
+                u_nk, dHdl = analyze_free_energy.preprocess_data(files, EEXE.temp, EEXE.df_spacing, EEXE.get_u_nk, EEXE.get_dHdl)  # noqa: E501
+                u_nk_list.append(u_nk)
+                dHdl_list.append(dHdl)
+
+            with open(f'{args.dir}/u_nk_data.pickle', 'wb') as handle:
+                pickle.dump(u_nk_list, handle, protocol=pickle.HIGHEST_PROTOCOL)
+
+            with open(f'{args.dir}/dHdl_data.pickle', 'wb') as handle:
+                pickle.dump(dHdl_list, handle, protocol=pickle.HIGHEST_PROTOCOL)
+
+        state_ranges = [list(i) for i in EEXE.state_ranges]
+        if EEXE.get_u_nk is True:
+            f, f_err = analyze_free_energy.calculate_free_energy(u_nk_list, state_ranges, EEXE.df_method, EEXE.err_method, EEXE.n_bootstrap, EEXE.seed)  # noqa: E501
+        else:
+            f, f_err = analyze_free_energy.calculate_free_energy(dHdl_list, state_ranges, EEXE.df_method, EEXE.err_method, EEXE.n_bootstrap, EEXE.seed)  # noqa: E501
 
-            lens = [len(t_list[i]) for i in range(len(t_list))]
-            if np.min(lens) >= 100:  # plot a histogram
-                counts, bins = np.histogram(t_list[i])
-
-                plt.figure()
-                for i in range(len(t_list)):
-                    plt.hist(t_list[i], bins=int(len(t_list[i]) / 20), label=f'Configuration {i}')
-                    if max(counts) >= 10000:
-                        plt.ticklabel_format(style='sci', axis='y', scilimits=(0, 0))
-                plt.xlabel(f'{y_labels[t]}')
-                plt.ylabel('Event count')
-                plt.grid()
-                plt.legend()
-                if fig_prefix is None:
-                    plt.savefig(f'{folder}/hist_{fig_names[t]}', dpi=600)
-                else:
-                    plt.savefig(f'{folder}/{fig_prefix}_hist_{fig_names[t]}', dpi=600)
+        print('Plotting the full-range free energy profile ...')
+        analyze_free_energy.plot_free_energy(f, f_err, f'{args.dir}/free_energy_profile.png')
 
-    return t_0k_list, t_k0_list, t_roundtrip_list, units
+        print('The full-range free energy profile averaged over all replicas:')
+        print(f"  {', '.join(f'{f[i]: .3f} +/- {f_err[i]: .3f} kT' for i in range(EEXE.n_tot))}")
+        print(f'The free energy difference between the coupled and decoupled states: {f[-1]: .3f} +/- {f_err[-1]: .3f} kT')  # noqa: E501
 
+    # Section 4. Calculate the time spent in GROMACS (This could take a while.)
+    t_wall_tot, t_sync, _ = utils.analyze_EEXE_time()
+    print(f'\nTotal wall time GROMACS spent to finish all iterations: {utils.format_time(t_wall_tot)}')
+    print(f'Total time spent in syncrhonizing all replicas: {utils.format_time(t_sync)}')
 
-def plot_g_vecs(f_g_vecs):
-    pass
+    print(f'\nTime elpased: {utils.format_time(time.time() - t0)}')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ensemble_md-0.6.0/ensemble_md/analysis/msm_analysis.py` & `ensemble_md-0.7.0/ensemble_md/analysis/msm_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         Physical time between frames. The default is 1.
     units : str
         The units of dt. The default is 'ps'.
 
     Returns
     -------
     ts_list : list
-        An list of instances of the ImpliedTimescales class in PyEMMA.
+        An list of instances of the :code:`ImpliedTimescales` class in PyEMMA.
     """
     ts_list = []
     n_rows, n_cols = utils.get_subplot_dimension(len(trajs))
     fig = plt.figure(figsize=(3 * n_cols, 2.5 * n_rows))
     for i in range(len(trajs)):
         # We convert trajs[i] to list to avoid BufferError: memoryview: underlying buffer is not C-contiguous
         ts = pyemma.msm.its(list(trajs[i]), lags=lags, show_progress=False)
```

### Comparing `ensemble_md-0.6.0/ensemble_md/cli/explore_EEXE.py` & `ensemble_md-0.7.0/ensemble_md/cli/explore_EEXE.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 #    a python package for running GROMACS simulation ensembles     #
 #                                                                  #
 #    Written by Wei-Tse Hsu <wehs7661@colorado.edu>                #
 #    Copyright (c) 2022 University of Colorado Boulder             #
 #                                                                  #
 ####################################################################
 import sys
+import random
 import argparse
 import numpy as np
 import pandas as pd
+from ensemble_md.ensemble_EXE import EnsembleEXE
 
 
 def initialize(args):
     parser = argparse.ArgumentParser(
         description='This code explores the parameter space of homogenous EEXE to help you figure \
                 out all possible combinations of the number of replicas, the number of \
                 states in each replica, and the number of overlapping states, and the total number states.')
@@ -36,15 +38,21 @@
                         type=int,
                         help='The state shift between adjacent replicas.')
     parser.add_argument('-c',
                         '--cnst',
                         default=False,
                         action='store_true',
                         help='Whether the apply the constraint such that the number of overlapping states \
-                            does notexceed 50%% of the number of states in both overlapping replicas.')
+                            does not exceed 50%% of the number of states in both overlapping replicas.')
+    parser.add_argument('-e',
+                        '--estimate',
+                        default=False,
+                        action='store_true',
+                        help='Whether to provide estimates of the chance of not having any swappable \
+                            pairs for each solution.')
     args_parse = parser.parse_args(args)
 
     return args_parse
 
 
 def solv_EEXE_diophantine(N, constraint=False):
     """
@@ -84,14 +92,42 @@
         s = 1 - t
         soln_all.extend([{'N': N, 'r': r, 'n': n[i], 's': s[i]} for i in range(len(t))])  # [N, r, n, s]
     soln_all = pd.DataFrame.from_dict(soln_all)  # turn the dict to pandas df, which is more convenient
 
     return soln_all
 
 
+def estimate_swapless_rate(state_ranges, N=1000000):
+    """
+    Estimates the chance of not having any swappable pair in an iteration.
+
+    Parameters
+    ----------
+    state_ranges : list
+        A list of lists of state indices. (Like the attribute :code:`state_ranges` in :code:`EnsemblEXE`.)
+    N : n
+        The number of Monte Carlo iterations for the estimation.
+
+    Returns
+    -------
+    p : float
+        The probability of not having any swappable pair in an iteration.
+    """
+    n = 0  # number of times of not having any swappable pairs
+    for i in range(N):
+        rands = [random.choice(state_ranges[i]) for i in range(len(state_ranges))]
+        swappables = EnsembleEXE.identify_swappable_pairs(rands, state_ranges, False)
+        if swappables == []:
+            n += 1
+
+    p = n / N * 100   # in percentage
+
+    return p
+
+
 def main():
     # For now, we only consider homogenous EEXE simulations
     args = initialize(sys.argv[1:])
     print('Exploration of the EEXE parameter space')
     print('=======================================')
     print('[ EEXE parameters of interest ]')
     print('- N: The total number of states')
@@ -112,11 +148,16 @@
 
     # Print out the solutions
     print('\n[ Solutions ]')
     for row_idx in range(len(soln_all)):
         soln = soln_all.iloc[row_idx]
         start_idx = [i * soln['s'] for i in range(soln['r'])]
         state_ranges = [list(np.arange(i, i + soln['n'])) for i in start_idx]
-        print(f"- Solution {row_idx + 1}: (N, r, n, s) = ({args.N}, {soln['r']}, {soln['n']}, {soln['s']})")
+
+        if args.estimate is True:
+            p = estimate_swapless_rate(state_ranges)
+            print(f"- Solution {row_idx + 1}: (N, r, n, s) = ({args.N}, {soln['r']}, {soln['n']}, {soln['s']}), {p:.1f}% chance to not have any swappable pair")  # noqa: E501
+        else:
+            print(f"- Solution {row_idx + 1}: (N, r, n, s) = ({args.N}, {soln['r']}, {soln['n']}, {soln['s']})")
         for i in range(soln['r']):
             print(f'  - Replica {i}: {state_ranges[i]}')
         print()
```

### Comparing `ensemble_md-0.6.0/ensemble_md/cli/run_EEXE.py` & `ensemble_md-0.7.0/ensemble_md/cli/run_EEXE.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import argparse
 import numpy as np
 from mpi4py import MPI
 from datetime import datetime
 
 from ensemble_md.utils import utils
 from ensemble_md.ensemble_EXE import EnsembleEXE
-from ensemble_md.utils.exceptions import ParameterError
 
 
 def initialize(args):
     parser = argparse.ArgumentParser(
         description='This code runs an ensemble of expanded ensemble given necessary inputs.')
     parser.add_argument('-y',
                         '--yaml',
@@ -80,42 +79,42 @@
         EEXE.print_params()
 
         # Print out warnings and fail if needed
         for i in EEXE.warnings:
             print(f'\n{i}\n')
 
         if len(EEXE.warnings) > args.maxwarn:
-            raise ParameterError(
-                f"The execution failed due to warning(s) about parameter spcificaiton. Check the warnings, or consider setting maxwarn in the input YAML file if you find them harmless.")  # noqa: E501, F541
+            print(f"The execution failed due to warning(s) about parameter spcificaiton. Check the warnings, or consider setting maxwarn in the input YAML file if you find them harmless.")  # noqa: E501, F541
+            comm.Abort(101)
 
     # Step 2: If there is no checkpoint file found/provided, perform the 1st iteration (index 0)
     if os.path.isfile(args.ckpt) is False:
         start_idx = 1
 
-        # 2-1. Set up input files for all simulations with 1 rank
+        # 2-1. Set up input files for all simulations
         if rank == 0:
             for i in range(EEXE.n_sim):
                 os.mkdir(f'sim_{i}')
                 os.mkdir(f'sim_{i}/iteration_0')
                 MDP = EEXE.initialize_MDP(i)
-                MDP.write(f"sim_{i}/iteration_0/{EEXE.mdp.split('/')[-1]}", skipempty=True)
+                MDP.write(f"sim_{i}/iteration_0/expanded.mdp", skipempty=True)
 
         # 2-2. Run the first ensemble of simulations
         EEXE.run_EEXE(0)
 
     else:
         if rank == 0:
             # If there is a checkpoint file, we see the execution as an extension of an EEXE simulation
             ckpt_data = np.load(args.ckpt)
             start_idx = len(ckpt_data[0])  # The length should be the same for the same axis
             print(f'\nGetting prepared to extend the EEXE simulation from iteration {start_idx} ...')
 
             if start_idx == EEXE.n_iter:
                 print('Extension aborted: The expected number of iterations have been completed!')
-                sys.exit()
+                MPI.COMM_WORLD.Abort(1)
             else:
                 print('Deleting data generated after the checkpoint ...')
                 for i in range(EEXE.n_sim):
                     n_finished = len(next(os.walk(f'sim_{i}'))[1])  # number of finished iterations
                     for j in range(start_idx, n_finished):
                         print(f'  Deleting the folder sim_{i}/iteration_{j}')
                         shutil.rmtree(f'sim_{i}/iteration_{j}')
@@ -127,14 +126,17 @@
             if os.path.isfile(args.g_vecs) is True:
                 EEXE.g_vecs = [list(i) for i in np.load(args.g_vecs)]
         else:
             start_idx = None
 
         start_idx = comm.bcast(start_idx, root=0)  # so that all the ranks are aware of start_idx
 
+    # 2-3. Get the reference distance for the distance restraint specified in the pull code, if any.
+    EEXE.get_ref_dist()
+
     for i in range(start_idx, EEXE.n_iter):
         if rank == 0:
             # Step 3: Swap the coordinates
             # 3-1. For all the replica simulations,
             #   (1) Find the last sampled state and the corresponding lambda values from the DHDL files.
             #   (2) Find the final Wang-Landau incrementors and weights from the LOG files.
             dhdl_files = [f'sim_{j}/iteration_{i - 1}/dhdl.xvg' for j in range(EEXE.n_sim)]
@@ -148,15 +150,15 @@
             # since they are updated by `get_swapping_pattern`. (Even if the function does not explicitly
             # returns `states_` and `weights_`, `states_` and `weights_` can still be different after
             # the use of the function.) Therefore, here we create copyes for `states_` and `weights_`
             # before the use of `get_swapping_pattern`, so we can use them in `histogram_correction`,
             # `combine_weights` and `update_MDP`.
             states = copy.deepcopy(states_)
             weights = copy.deepcopy(weights_)
-            swap_pattern = EEXE.get_swapping_pattern(dhdl_files, states_, weights_)
+            swap_pattern, swap_list = EEXE.get_swapping_pattern(dhdl_files, states_, weights_)  # swap_list will only be used for modify_coords  # noqa: E501
 
             # 3-3. Calculate the weights averaged since the last update of the Wang-Landau incrementor.
             # Note that the averaged weights are used for histogram correction/weight combination.
             # For the calculation of the acceptance ratio (inside get_swapping_pattern), final weights should be used.
             if EEXE.N_cutoff != -1 or EEXE.w_combine is True:
                 # Only when histogram correction/weight combination is needed.
                 weights_avg, weights_err = EEXE.get_averaged_weights(log_files)
@@ -165,56 +167,71 @@
             # Note that we never use final weights but averaged weights here.
             # The product of this step should always be named as "weights" to be used in update_MDP
             if wl_delta != [None for i in range(EEXE.n_sim)]:  # weight-updating
                 print(f'\nCurrent Wang-Landau incrementors: {wl_delta}')
             if EEXE.N_cutoff != -1 and EEXE.w_combine is True:
                 # perform both
                 weights_avg = EEXE.histogram_correction(weights_avg, counts)
-                weights, g_vec = EEXE.combine_weights(weights_avg)
+                weights, g_vec = EEXE.combine_weights(weights_avg)  # inverse-variance weighting seems worse
                 EEXE.g_vecs.append(g_vec)
             elif EEXE.N_cutoff == -1 and EEXE.w_combine is True:
                 # only perform weight combination
                 print('\nNote: No histogram correction will be performed.')
-                weights, g_vec = EEXE.combine_weights(weights_avg)
+                weights, g_vec = EEXE.combine_weights(weights_avg)  # inverse-variance weighting seems worse
                 EEXE.g_vecs.append(g_vec)
             elif EEXE.N_cutoff != -1 and EEXE.w_combine is False:
                 # only perform histogram correction
                 print('\nNote: No weight combination will be performed.')
                 weights = EEXE.histogram_correction(weights_avg, counts)
             else:
                 print('\nNote: No histogram correction will be performed.')
                 print('Note: No weight combination will be performed.')
 
             # 3-5. Modify the MDP files and swap out the GRO files (if needed)
             # Here we keep the lambda range set in mdp the same across different iterations in the same folder but swap out the gro file  # noqa: E501
             # Note we use states (copy of states_) instead of states_ in update_MDP.
             for j in list(range(EEXE.n_sim)):
                 os.mkdir(f'sim_{j}/iteration_{i}')
-                MDP = EEXE.update_MDP(f"sim_{j}/iteration_{i - 1}/{EEXE.mdp.split('/')[-1]}", j, i, states, wl_delta, weights, counts)   # modify with a new template  # noqa: E501
-                MDP.write(f"sim_{j}/iteration_{i}/{EEXE.mdp.split('/')[-1]}", skipempty=True)
+                MDP = EEXE.update_MDP(f"sim_{j}/iteration_{i - 1}/expanded.mdp", j, i, states, wl_delta, weights, counts)   # modify with a new template  # noqa: E501
+                MDP.write(f"sim_{j}/iteration_{i}/expanded.mdp", skipempty=True)
                 # In run_EEXE(i, swap_pattern), where the tpr files will be generated, we use the top file at the
                 # level of the simulation (the file that will be shared by all simulations). For the gro file, we pass
                 # swap_pattern to the function to figure it out internally.
         else:
-            swap_pattern = None
+            swap_pattern, swap_list = None, None
 
         if -1 not in EEXE.equil and 0 not in EEXE.equil:
             # This is the case where the weights are equilibrated in a weight-updating simulation.
             # As a remidner, EEXE.equil should be a list of 0 after extract_final_log_info in a
             # fixed-weight simulation, and a list of -1 for a weight-updating simulation with unequilibrated weights.
             print('\nSimulation terminated: The weights have been equilibrated for all replicas.')
             break
 
         # Step 4: Perform another iteration
-        # 4-1. Run another ensemble of simulations
+        # 4-1. Modify the coordinates of the output gro files if needed.
         swap_pattern = comm.bcast(swap_pattern, root=0)
+        swap_list = comm.bcast(swap_list, root=0)
+
+        if len(swap_list) == 0:
+            pass
+        else:
+            if EEXE.modify_coords_fn is not None:
+                if rank == 0:
+                    for j in range(len(swap_list)):
+                        print('\nModifying the coordinates of the following output GRO files ...')
+                        gro_1 = f'sim_{swap_list[j][0]}/iteration_{i-1}/confout.gro'
+                        gro_2 = f'sim_{swap_list[j][1]}/iteration_{i-1}/confout.gro'
+                        print(f'  - {gro_1}\n  - {gro_2}')
+                        EEXE.modify_coords_fn(gro_1, gro_2)  # the order should not matter
+
+        # 4-2. Run another ensemble of simulations
         EEXE.run_EEXE(i, swap_pattern)
 
+        # 4-3. Save data
         if rank == 0:
-            # 4-2. Save data
             if (i + 1) % EEXE.n_ckpt == 0:
                 if len(EEXE.g_vecs) != 0:
                     # Save g_vec as a function of time if weight combination was used.
                     np.save('g_vecs.npy', EEXE.g_vecs)
 
                 print('\n----- Saving .npy files to checkpoint the simulation ---')
                 np.save('rep_trajs.npy', EEXE.rep_trajs)
@@ -241,12 +258,13 @@
                     units = 'ns'
                     EEXE.equil[i] /= 1000
                 else:
                     units = 'ps'
                 print(f'  - Rep {i}: The weights have been equilibrated at {EEXE.equil[i]:.2f} {units} (iteration {idx}).')  # noqa: E501
 
         print(f'\n{EEXE.n_empty_swappable} out of {EEXE.n_iter}, or {EEXE.n_empty_swappable / EEXE.n_iter * 100:.1f}% iterations had an empty list of swappable pairs.')  # noqa: E501
-        print(f'{EEXE.n_rejected} out of {EEXE.n_swap_attempts}, or {EEXE.n_rejected / EEXE.n_swap_attempts * 100:.1f}% of attempted exchanges were rejected.')  # noqa: E501
+        if EEXE.n_swap_attempts != 0:
+            print(f'{EEXE.n_rejected} out of {EEXE.n_swap_attempts}, or {EEXE.n_rejected / EEXE.n_swap_attempts * 100:.1f}% of attempted exchanges were rejected.')  # noqa: E501
 
         print(f'\nTime elapsed: {utils.format_time(time.time() - t1)}')
 
     sys.exit()
```

### Comparing `ensemble_md-0.6.0/ensemble_md/data/README.md` & `ensemble_md-0.7.0/ensemble_md/data/README.md`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/ensemble_EXE.py` & `ensemble_md-0.7.0/ensemble_md/ensemble_EXE.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,47 +10,48 @@
 """
 The :obj:`.ensemble_EXE` module provides functions for setting up and ensemble of expanded ensemble.
 """
 import os
 import sys
 import copy
 import yaml
-import shutil
 import random
+import importlib
 import subprocess
 import numpy as np
 from mpi4py import MPI
 from itertools import combinations
 from collections import OrderedDict
-from alchemlyb.parsing.gmx import extract_dHdl
 from alchemlyb.parsing.gmx import _get_headers as get_headers
 from alchemlyb.parsing.gmx import _extract_dataframe as extract_dataframe
 
 import ensemble_md
+from ensemble_md.utils import utils
 from ensemble_md.utils import gmx_parser
 from ensemble_md.utils.exceptions import ParameterError
 
 comm = MPI.COMM_WORLD
-rank = comm.Get_rank()  # Note that this is a GLOBAL variable
+rank = comm.Get_rank()
 
 
 class EnsembleEXE:
     """
     This class provides a variety of functions useful for setting up and running
     an ensemble of expanded ensemble. Upon instantiation, all parameters in the YAML
     file will be assigned to an attribute in the class. In addition to these variables,
     below is a list of attributes of the class. (All the the attributes are assigned by
     :obj:`set_params` unless otherwise noted.)
 
+    :ivar gmx_path: The absolute path of the GROMACS exectuable.
+    :ivar gmx_version: The version of the GROMACS executable.
     :ivar yaml: The input YAML file used to instantiate the class. Assigned by the :code:`__init__` function.
     :ivar warnings: Warnings about parameter specification in either YAML or MDP files.
     :ivar reformatted_mdp: Whether the templated MDP file has been reformatted by replacing hyphens
         with underscores or not.
     :ivar template: The instance of the :obj:`MDP` class based on the template MDP file.
-    :ivar nsteps: The number of steps per iteration.
     :ivar dt: The simulation timestep in ps.
     :ivar temp: The simulation temperature in Kelvin.
     :ivar fixed_weights: Whether the weights will be fixed during the simulation (according to the template MDP file).
     :ivar updating_weights: The list of weights as a function of time (since the last update of the Wang-Landau
         incrementor) for different replicas. The length is equal to the number of replicas. This is only relevant for
         weight-updating simulations.
     :ivar equilibrated_weights: The equilibrated weights of different replicas. For weight-equilibrating simulations,
@@ -63,36 +64,35 @@
         :code:`fep_lambdas`, :code:`mass_lambdas`, :code:`coul_lambdas`, etc.
     :ivar n_tot: The total number of states for all replicas.
     :ivar n_sub: The numbmer of states for each replica. The current implementation assumes homogenous replicas.
     :ivar state_ranges: A list of list of state indices for each replica.
     :ivar equil: A list of times it took to equilibrated the weights for different replicas. This
         list is initialized with a list of -1, where -1 means that the weights haven't been equilibrated. Also,
         a value of 0 means that the simulation is a fixed-weight simulation.
-    :ivar lambda_dict: A dictionary with keys being the tuples of coupling parameters used in each replicas and
-        values being the corresponding global index (starting from 0). Assigned by :obj:`map_lambda2state`.
-    :ivar lambda_ranges: A list of lambda vectors of state range of each replica. Assigned by :obj:`map_lambda2state`.
-    :ivar n_rejected: The number of proposed exchanges that have been rejected. Updated by :obj:`accept_or_reject`.
+    :ivar n_rejected: The number of proposed exchanges that have been rejected. Updated by :obj:`.accept_or_reject`.
     :ivar n_swap_attempts: The number of swaps attempted so far. This does not include the cases
-        where there is no swappable pair. Updated by :obj:`get_swapping_pattern`.
+        where there is no swappable pair. Updated by :obj:`.get_swapping_pattern`.
     :ivar n_emtpy_swappable: The number of times when there was no swappable pair.
-    :ivar rep_trajs: The replica-space trajectories of all replicas.
+    :ivar rep_trajs: The replica-space trajectories of all configurations.
     :ivar configs: A list that thows the current configuration index that each replica is sampling.
     :ivar g_vecs: The time series of the (processed) whole-range alchemical weights. If no weight combination is
         applied, this list will just be a list of :code:`None`'s.
     :ivar get_u_nk: Whether to get the :math:`u_{nk}` dataset from the DHDL files. Only meaningful during
         data analysis and if :code:`df_method` is specified.
     :ivar get_dHdl: Whether to get the :math:`dH/dλ` dataset from the DHDL files. Only meaningful
         during data analysis and if :code:`df_method` is specified.
+    :ivar modify_coords_fn: The function (callable) in the external module (specified as :code:`modify_coords` in
+        the input YAML file) for modifying coordinates at exchanges.
     """
 
-    def __init__(self, yaml_file):
+    def __init__(self, yaml_file, analysis=False):
         self.yaml = yaml_file
-        self.set_params()
+        self.set_params(analysis)
 
-    def set_params(self):
+    def set_params(self, analysis):
         """
         Sets up or reads in the user-defined parameters from a yaml file and an MDP template.
         This function is called to instantiate the class in the :code:`__init__` function of
         class. Specifically, it does the following:
 
           1. Sets up constants.
           2. Reads in parameters from a YAML file.
@@ -103,14 +103,17 @@
 
         After instantiation, the class instance will have attributes corresponding to
         each of the parameters specified in the YAML file. For a full list of the parameters that
         can be specified in the YAML file, please refer to :ref:`doc_parameters`.
 
         :param yaml_file: The file name of the YAML file for specifying the parameters for EEXE.
         :type yaml_file: str
+        :param analysis: Whether the instantiation of the class is for data analysis of EEXE simulations.
+            The default is :code:`False`
+        :type analysis: bool
 
         :raises ParameterError:
 
               - If a required parameter is not specified in the YAML file.
               - If a specified parameter is not recognizable.
               - If a specified weight combining scheme is not available.
               - If a specified acceptance scheme is not available.
@@ -146,27 +149,27 @@
         ]
         for i in required_args:
             if hasattr(self, i) is False or getattr(self, i) is None:
                 raise ParameterError(
                     f"Required parameter '{i}' not specified in {self.yaml}."
                 )  # noqa: F405
 
-        # Check the GROMACS executable
-        self.check_gmx_executable()
-
         # Step 3: Handle the optional YAML parameters
         # Key: Optional argument; Value: Default value
         optional_args = {
+            "add_swappables": None,
+            "modify_coords": None,
             "nst_sim": None,
             "proposal": 'exhaustive',
             "acceptance": "metropolis",
             "w_combine": False,
             "N_cutoff": 1000,
             "n_ex": 'N^3',   # only active for multiple swaps.
             "verbose": True,
+            "mdp_args": None,
             "grompp_args": None,
             "runtime_args": None,
             "n_ckpt": 100,
             "msm": False,
             "free_energy": False,
             "df_spacing": 1,
             "df_method": "MBAR",
@@ -204,52 +207,82 @@
             params_int.append('n_ex')
         if self.seed is not None:
             params_int.append('seed')
         for i in params_int:
             if type(getattr(self, i)) != int:
                 raise ParameterError(f"The parameter '{i}' should be an integer.")
 
-        params_pos = ['n_sim', 'n_iter', 's', 'n_ckpt', 'df_spacing', 'n_bootstrap']  # positive parameters
+        params_pos = ['n_sim', 'n_iter', 'n_ckpt', 'df_spacing', 'n_bootstrap']  # positive parameters
         if self.nst_sim is not None:
             params_pos.append('nst_sim')
         for i in params_pos:
             if getattr(self, i) <= 0:
                 raise ParameterError(f"The parameter '{i}' should be positive.")
 
         if self.n_ex != 'N^3' and self.n_ex < 0:
             raise ParameterError("The parameter 'n_ex' should be non-negative.")
 
+        if self.s < 0:
+            raise ParameterError("The parameter 's' should be non-negative.")
+
         if self.N_cutoff < 0 and self.N_cutoff != -1:
             raise ParameterError("The parameter 'N_cutoff' should be non-negative unless no histogram correction is needed, i.e. N_cutoff = -1.")  # noqa: E501
 
         params_str = ['gro', 'top', 'mdp']
+        # First check if self.gro and self.top are lists and check their lengths
+        check_files = ['gro', 'top']  # just for checking file types that can take multiple inputs
+        for i in check_files:
+            if isinstance(getattr(self, i), list):
+                params_str.remove(i)
+                if len(getattr(self, i)) != self.n_sim:
+                    raise ParameterError(f"The number of the input {i.upper()} files must be the same as the number of replicas, if multiple are specified.")  # noqa: E501
         for i in params_str:
             if type(getattr(self, i)) != str:
                 raise ParameterError(f"The parameter '{i}' should be a string.")
 
         params_bool = ['verbose', 'msm']
         for i in params_bool:
             if type(getattr(self, i)) != bool:
                 raise ParameterError(f"The parameter '{i}' should be a boolean variable.")
 
+        if self.add_swappables is not None:
+            if not isinstance(self.add_swappables, list):
+                raise ParameterError("The parameter 'add_swappables' should be a nested list.")
+            for sublist in self.add_swappables:
+                if not isinstance(sublist, list):
+                    raise ParameterError("The parameter 'add_swappables' should be a nested list.")
+                for item in sublist:
+                    if not isinstance(item, int) or item < 0:
+                        raise ParameterError("Each number specified in 'add_swappables' should be a non-negative integer.")  # noqa: E501
+
+        if self.mdp_args is not None:
+            for key in self.mdp_args.keys():
+                if not isinstance(key, str):
+                    raise ParameterError("All keys specified in 'mdp_args' should be strings.")
+                else:
+                    if '-' in key:
+                        raise ParameterError("Parameters specified in 'mdp_args' must use underscores in place of hyphens.")  # noqa: E501
+            for val_list in self.mdp_args.values():
+                if len(val_list) != self.n_sim:
+                    raise ParameterError("The number of values specified for each key in 'mdp_args' should be the same as the number of replicas.")  # noqa: E501
+
         # Step 5: Reformat the input MDP file to replace all hypens with underscores.
-        self.reformat_MDP()
+        self.reformat_MDP(self.mdp)
 
         # Step 6: Read in parameters from the MDP template
         self.template = gmx_parser.MDP(self.mdp)
-        self.nsteps = self.template["nsteps"]  # will be overwritten by self.nst_sim if nst_sim is specified.
         self.dt = self.template["dt"]  # ps
         self.temp = self.template["ref_t"]
 
         if self.nst_sim is None:
-            self.nst_sim = self.nsteps
+            self.nst_sim = self.template["nsteps"]
 
         if 'wl_scale' in self.template.keys():
-            if isinstance(self.template['wl_scale'], np.ndarray):
-                # If wl_scale in the MDP file is a blank (i.e. fixed weights), mdp['wl_scale'] will be an empty array.
+            if self.template['wl_scale'] == []:
+                # If wl_scale in the MDP file is a blank (i.e. fixed weights), mdp['wl_scale'] will be an empty list.
                 # This is the only case where mdp['wl_scale'] is a numpy array.
                 self.fixed_weights = True
                 self.equilibrated_weights = [None for i in range(self.n_sim)]
             else:
                 self.fixed_weights = False
                 self.equilibrated_weights = [[] for i in range(self.n_sim)]
                 self.updating_weights = [[] for i in range(self.n_sim)]
@@ -267,20 +300,66 @@
 
         if 'lmc_seed' in self.template and self.template['lmc_seed'] != -1:
             self.warnings.append('Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
 
         if 'gen_seed' in self.template and self.template['gen_seed'] != -1:
             self.warnings.append('Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
 
-        if 'symmetrized_transition_matrix' in self.template and self.template['symmetrized_transition_matrix'] == 'yes':  # noqa: E501
-            self.warnings.append('Warning: We recommend setting symmetrized-transition-matrix to no instead of yes.')
+        if 'gen_vel' not in self.template or ('gen_vel' in self.template and self.template['gen_vel'] == 'no'):
+            self.warnings.append('Warning: We recommend generating new velocities for each iteration to avoid potential issues with detailed balance.')  # noqa: E501
+
+        if self.nst_sim % self.template['nstlog'] != 0:
+            raise ParameterError(
+                'The parameter "nstlog" must be a factor of the parameter "nst_sim" specified in the YAML file.')
+
+        if self.nst_sim % self.template['nstdhdl'] != 0:
+            raise ParameterError(
+                'The parameter "nstdhdl" must be a factor of the parameter "nst_sim" specified in the YAML file.')
 
-        if self.template['nstlog'] > self.nst_sim:
+        if self.template['nstexpanded'] % self.template['nstdhdl'] != 0:
             raise ParameterError(
-                'The parameter "nstlog" should be equal to or smaller than "nst_sim" specified in the YAML file so that the sampling information can be parsed.')  # noqa: E501
+                'In EEXE, the parameter "nstdhdl" must be a factor of the parameter "nstexpanded", or the calculation of acceptance ratios might be wrong.')  # noqa: E501
+
+        if self.mdp_args is not None:
+            if 'lmc_seed' in self.mdp_args and -1 not in self.mdp_args['lmc_seed']:
+                self.warnings.append('Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
+
+            if 'gen_seed' in self.mdp_args and -1 not in self.mdp_args['gen_seed']:
+                self.warnings.append('Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.')  # noqa: E501
+
+            if 'gen_vel' in self.mdp_args and 'no' in self.mdp_args['gen_vel']:
+                self.warnings.append('Warning: We recommend generating new velocities for each iteration to avoid potential issues with the detailed balance.')  # noqa: E501
+
+            if 'nstlog' in self.mdp_args and sum(self.nst_sim % np.array(self.mdp_args['nstlog'])) != 0:
+                raise ParameterError(
+                    'The parameter "nstlog" must be a factor of the parameter "nst_sim" specified in the YAML file.')
+
+            if 'nstdhdl' in self.mdp_args and sum(self.nst_sim % np.array(self.mdp_args['nstdhdl'])) != 0:
+                raise ParameterError(
+                    'The parameter "nstdhdl" must be a factor of the parameter "nst_sim" specified in the YAML file.')
+
+            if 'nstexpanded' in self.mdp_args and 'nstdhdl' in self.mdp_args and sum(np.array(self.mdp_args['nstexpanded']) % np.array(self.mdp_args['nstdhdl'])) != 0:  # noqa: E501
+                raise ParameterError(
+                    'In EEXE, the parameter "nstdhdl" must be a factor of the parameter "nstexpanded", or the calculation of acceptance ratios might be wrong.')  # noqa: E501
+
+        if 'pull' in self.template and self.template['pull'] == 'yes':
+            pull_ncoords = self.template['pull_ncoords']
+            self.set_ref_dist = []
+            for i in range(pull_ncoords):
+                if self.template[f'pull_coord{i+1}_geometry'] == 'distance':
+                    if self.template[f'pull_coord{i+1}_start'] == 'yes':
+                        self.set_ref_dist.append(True)  # starting from the second iteration, set pull_coord*_init.
+                        if 'pull_nstxout' not in self.template:
+                            self.warnings.append('A non-zero value should be specified for pull_nstxout if pull_coord*_start is set to yes.')  # noqa: E501
+                        if self.template['pull_nstxout'] == 0:
+                            self.warnings.append('A non-zero value should be specified for pull_nstxout if pull_coord*_start is set to yes.')  # noqa: E501
+                    else:
+                        self.set_ref_dist.append(False)  # Here we assume that the user know what reference distance to use.  # noqa: E501
+                else:
+                    self.set_ref_dist.append(False)  # we only deal with distance restraints for now.
 
         # Step 7: Set up derived parameters
         # 7-1. kT in kJ/mol
         self.kT = k * NA * self.temp / 1000  # 1 kT in kJ/mol
 
         # 7-2. Figure out what types of lambda variables are involved
         # Here is we possible lambda types in the order read by GROMACS, which is likely also the order when being printed to the log file.  # noqa: E501
@@ -303,47 +382,56 @@
         # 7-5. A list of sets of state indices
         start_idx = [i * self.s for i in range(self.n_sim)]
         self.state_ranges = [list(np.arange(i, i + self.n_sub)) for i in start_idx]
 
         # 7-6. A list of time it took to get the weights equilibrated
         self.equil = [-1 for i in range(self.n_sim)]   # -1 means unequilibrated
 
-        # 7-7. Map the lamda vectors to state indices
-        self.map_lambda2state()
-
-        # 7-8. Some variables for counting
+        # 7-7. Some variables for counting
         self.n_rejected = 0
         self.n_swap_attempts = 0
         self.n_empty_swappable = 0
 
-        # 7-9. Replica space trajectories. For example, rep_trajs[0] = [0, 2, 3, 0, 1, ...] means
+        # 7-8. Replica space trajectories. For example, rep_trajs[0] = [0, 2, 3, 0, 1, ...] means
         # that configuration 0 transitioned to replica 2, then 3, 0, 1, in iterations 1, 2, 3, 4, ...,
         # respectively. The first element of rep_traj[i] should always be i.
         self.rep_trajs = [[i] for i in range(self.n_sim)]
 
-        # 7-10. configs shows the current configuration that each replica is sampling.
+        # 7-9. configs shows the current configuration that each replica is sampling.
         # For example, self.configs = [0, 2, 1, 3] means that configurations 0, 2, 1, and 3 are
         # in replicas, 0, 1, 2, 3, respectively. This list will be constantly updated during the simulation.
         self.configs = list(range(self.n_sim))
 
-        # 7-11. The time series of the (processed) whole-range alchemical weights
+        # 7-10. The time series of the (processed) whole-range alchemical weights
         # If no weight combination is applied, self.g_vecs will just be a list of None's.
         self.g_vecs = []
 
-        # 7-12. Data analysis
+        # 7-11. Data analysis
         if self.df_method == 'MBAR':
             self.get_u_nk = True
             self.get_dHdl = False
         else:
             self.get_u_nk = False
             self.get_dHdl = True
 
+        # 7-12. External module for coordinate modification
+        if self.modify_coords is not None:
+            sys.path.append(os.getcwd())
+            module = importlib.import_module(self.modify_coords)
+            self.modify_coords_fn = getattr(module, self.modify_coords)
+        else:
+            self.modify_coords_fn = None
+
+        # Step 8. Check the executables
+        if analysis is False:
+            self.check_gmx_executable()
+
     def check_gmx_executable(self):
         """
-        Checks if the GROMACS executable can be used and  gets its absolute path and version.
+        Checks if the GROMACS executable can be used and gets its absolute path and version.
         """
         try:
             result = subprocess.run(['which', self.gmx_executable], capture_output=True, text=True, check=True)
             self.gmx_path = result.stdout.strip()  # this can be exactly the same as self.gmx_executable
 
             version_output = subprocess.run([self.gmx_path, "-version"], capture_output=True, text=True, check=True)
             for line in version_output.stdout.splitlines():
@@ -360,34 +448,51 @@
         Prints important parameters related to the EXEE simulation.
 
         Parameters
         ----------
         params_analysis : bool, optional
             If True, additional parameters related to data analysis will be printed. Default is False.
         """
+        if isinstance(self.gro, list):
+            gro_str = ', '.join(self.gro)
+        else:
+            gro_str = self.gro
+
+        if isinstance(self.top, list):
+            top_str = ', '.join(self.top)
+        else:
+            top_str = self.top
+
         print("Important parameters of EXEE")
         print("============================")
         print(f"Python version: {sys.version}")
         print(f"GROMACS executable: {self.gmx_path}")  # we print the full path here
         print(f"GROMACS version: {self.gmx_version}")
         print(f"ensemble_md version: {ensemble_md.__version__}")
-        print(f'Simulation inputs: {self.gro}, {self.top}, {self.mdp}')
+        print(f'Simulation inputs: {gro_str}, {top_str}, {self.mdp}')
         print(f"Verbose log file: {self.verbose}")
         print(f"Proposal scheme: {self.proposal}")
         print(f"Acceptance scheme for swapping simulations: {self.acceptance}")
         print(f"Whether to perform weight combination: {self.w_combine}")
         print(f"Histogram cutoff: {self.N_cutoff}")
         print(f"Number of replicas: {self.n_sim}")
         print(f"Number of iterations: {self.n_iter}")
         print(f"Number of attempted swaps in one exchange interval: {self.n_ex}")
         print(f"Length of each replica: {self.dt * self.nst_sim} ps")
         print(f"Frequency for checkpointing: {self.n_ckpt} iterations")
         print(f"Total number of states: {self.n_tot}")
+        print(f"Additionally defined swappable states: {self.add_swappables}")
         print(f"Additional grompp arguments: {self.grompp_args}")
         print(f"Additional runtime arguments: {self.runtime_args}")
+        if self.mdp_args is not None and len(self.mdp_args.keys()) > 1:
+            print("MDP parameters differing across replicas:")
+            for i in self.mdp_args.keys():
+                print(f"  - {i}: {self.mdp_args[i]}")
+        else:
+            print(f"MDP parameters differing across replicas: {self.mdp_args}")
         print("Alchemical ranges of each replica in EEXE:")
         for i in range(self.n_sim):
             print(f"  - Replica {i}: States {self.state_ranges[i]}")
 
         if params_analysis is True:
             print()
             print(f"Whether to build Markov state models and perform relevant analysis: {self.msm}")
@@ -397,53 +502,36 @@
             print(f"The method for estimating the uncertainty of free energies in free energy calculations, if any: {self.err_method}")  # noqa: E501
             print(f"The number of bootstrap iterations in the boostrapping method, if used: {self.n_bootstrap}")
             print(f"The random seed to use in bootstrapping, if used: {self.seed}")
 
         if self.reformatted_mdp is True:
             print("Note that the input MDP file has been reformatted by replacing hypens with underscores. The original mdp file has been renamed as *backup.mdp.")  # noqa: E501
 
-    def reformat_MDP(self):
+    def reformat_MDP(self, mdp_file):
         """
-        Reformats an MDP file so that all hyphens in the parameter names are replaced by underscores.
+        Reformats the input MDP file so that all hyphens in the parameter names are replaced by underscores.
         If the input MDP file contains hyphens in its parameter names, the class attribue :code:`self.reformatted`
         will be set to :code:`True`. In this case, the new MDP object with reformatted parameter names will be
-        written to the original file paththe file, while the original file will be renamed with a
-        :code:`_backup` suffix. If the input MDP file contains underscores in its parameter names, the function sets
+        written to the original file path of the file, while the original file will be renamed with a
+        :code:`_backup` suffix. If the input MDP file is not reformatted, the function sets
         the class attribute :code:`self.reformatted_mdp` to :code:`False`.
         """
-        params = gmx_parser.MDP(self.mdp)
+        params = gmx_parser.MDP(mdp_file)
 
         odict = OrderedDict([(k.replace('-', '_'), v) for k, v in params.items()])
         params_new = gmx_parser.MDP(None, **odict)
 
-        if params_new.keys() == params.keys():
-            self.reformatted_mdp = False  # no need to reformat the file
-        else:
-            self.reformatted_mdp = True
-            new_name = self.mdp.split('.mdp')[0] + '_backup.mdp'
-            shutil.move(self.mdp, new_name)
-            params_new.write(self.mdp)
-
-    def map_lambda2state(self):
-        """
-        Define attrbitues that map vectors of coupling parameters to state indices.
-
-        Attributes
-        ----------
-        lambda_dict : dict
-            A dictionary whose keys are tuples of coupling parameters and
-            values are the corresponding GLOBAL state indices (starting from 0).
-        lambda_ranges : list
-            A list of lambda vectors of the state range of each replica.
-        """
-        self.lambda_dict = {}  # key: vector of coupling parameters, value: state index
-        for i in range(self.n_tot):
-            key = tuple([self.template[j][i] for j in self.lambda_types])
-            self.lambda_dict[key] = i
-        self.lambda_ranges = [[list(self.lambda_dict.keys())[j] for j in self.state_ranges[i]]for i in range(len(self.state_ranges))]  # noqa: E501
+        if rank == 0:
+            if params_new.keys() == params.keys():
+                self.reformatted_mdp = False  # no need to reformat the file
+            else:
+                self.reformatted_mdp = True
+                new_name = mdp_file.split('.mdp')[0] + '_backup.mdp'
+                os.rename(mdp_file, new_name)
+                params_new.write(mdp_file)
 
     def initialize_MDP(self, idx):
         """
         Initializes the MDP object for generating MDP files for a replica based on the MDP template.
         This function should be called only for generating MDP files for the FIRST iteration
         and it has nothing to do with whether the weights are fixed or equilibrating.
         It is assumed that the MDP template has all the common parameters of all replicas.
@@ -457,23 +545,42 @@
         -------
         MDP : :obj:`.gmx_parser.MDP` obj
             An updated object of :obj:`.gmx_parser.MDP` that can be used to write MDP files.
         """
         MDP = copy.deepcopy(self.template)
         MDP["nsteps"] = self.nst_sim
 
+        if self.mdp_args is not None:
+            for param in self.mdp_args.keys():
+                MDP[param] = self.mdp_args[param][idx]
+
         start_idx = idx * self.s
         for i in self.lambda_types:
             MDP[i] = self.template[i][start_idx:start_idx + self.n_sub]
 
         if "init_lambda_weights" in self.template:
             MDP["init_lambda_weights"] = self.template["init_lambda_weights"][start_idx:start_idx + self.n_sub]
 
         return MDP
 
+    def get_ref_dist(self):
+        """
+        Gets the reference distance(s) to use starting from the second iteration if distance restraint(s) are used.
+        Specifically, a reference distance determined here is the initial COM distance between the pull groups
+        in the input GRO file. This function initializes the attribute :code:`ref_dist`.
+        """
+        if hasattr(self, 'set_ref_dist'):
+            self.ref_dist = []
+            pullx_file = 'sim_0/iteration_0/pullx.xvg'
+            headers = get_headers(pullx_file)
+            for i in range(len(self.set_ref_dist)):
+                if self.set_ref_dist[i] is True:
+                    dist = list(extract_dataframe(pullx_file, headers=headers)[f'{i+1}'])[0]
+                    self.ref_dist.append(dist)
+
     def update_MDP(self, new_template, sim_idx, iter_idx, states, wl_delta, weights, counts=None):
         """
         Updates the MDP file for a new iteration based on the new MDP template coming from the previous iteration.
         Note that if the weights got equilibrated in the previous iteration, then the weights will be fixed
         at these equilibrated values for all the following iterations.
 
         Parameters
@@ -518,41 +625,45 @@
             MDP["lmc_stats"] = "no"
             MDP["wl_scale"] = ""
             MDP["wl_ratio"] = ""
             MDP["init_wl_delta"] = ""
             MDP["lmc_weights_equil"] = ""
             MDP["weight_equil_wl_delta"] = ""
 
+        # Here we deal with the distance restraint in the pull code, if any.
+        if hasattr(self, 'ref_dist'):
+            for i in range(len(self.ref_dist)):
+                MDP[f'pull_coord{i+1}_start'] = "no"
+                MDP[f'pull_coord{i+1}_init'] = self.ref_dist[i]
+
         return MDP
 
     def extract_final_dhdl_info(self, dhdl_files):
         """
         For all the replica simulations, finds the last sampled state
-        and the corresponding lambda values from a dhdl file.
+        and print the corresponding lambda values from a dhdl file.
 
         Parameters
         ----------
         dhdl_files : list
             A list of file paths to GROMACS DHDL files of different replicas.
 
         Returns
         -------
         states : list
             A list of the global indices of the last sampled states of all simulaitons.
         """
-        states, lambda_vecs = [], []
+        states = []
         print("\nBelow are the final states being visited:")
-        for i in range(self.n_sim):
-            dhdl = extract_dHdl(dhdl_files[i], T=self.temp)
-            lambda_vecs.append(dhdl.index[-1][1:])
-            states.append(self.lambda_dict[lambda_vecs[-1]])  # absolute order
-            print(
-                f"  Simulation {i}: Global state {states[i]}, (coul, vdw) = \
-                {list(self.lambda_dict.keys())[list(self.lambda_dict.values()).index(states[i])]}"
-            )
+        for i in range(len(dhdl_files)):
+            headers = get_headers(dhdl_files[i])
+            state_local = list(extract_dataframe(dhdl_files[i], headers=headers)['Thermodynamic state'])[-1]  # local index of the last state  # noqa: E501
+            state_global = state_local + i * self.s  # global index of the last state
+            states.append(state_global)  # append the global index
+            print(f"  Simulation {i}: Global state {states[i]}")
         print('\n', end='')
 
         return states
 
     def extract_final_log_info(self, log_files):
         """
         Extracts the following information for each replica simulation from a given list of GROMACS LOG files:
@@ -575,15 +686,15 @@
             A list of lists of final weights of all simulations.
         counts : list
             A list of lists of final counts of all simulations.
         """
         wl_delta, weights, counts = [], [], []
 
         # Find the final Wang-Landau incrementors and weights
-        for i in range(self.n_sim):
+        for i in range(len(log_files)):
             if self.verbose:
                 print(f'Parsing {log_files[i]} ...')
             result = gmx_parser.parse_log(log_files[i])  # weights, counts, wl_delta, equil_time
             weights.append(result[0][-1])
             counts.append(result[1])
             wl_delta.append(result[2])
 
@@ -631,58 +742,82 @@
             else:
                 self.current_wl_delta[i] = wl_delta
                 self.updating_weights[i] = weights
 
         # shape of self.updating_weights is (n_sim, n_points, n_states), but n_points can be different
         # for different replicas, which will error out np.mean(self.updating_weights, axis=1)
         weight_avg = [np.mean(self.updating_weights[i], axis=0).tolist() for i in range(self.n_sim)]
-        weight_err = [np.std(self.updating_weights[i], axis=0, ddof=1).tolist() for i in range(self.n_sim)]
+        weight_err = []
+        for i in range(self.n_sim):
+            if len(self.updating_weights[i]) == 1:  # this would lead to a RunTime Warning and nan
+                weight_err.append([0] * self.n_sub)  # in `weighted_mean``, a simple average will be returned.
+            else:
+                weight_err.append(np.std(self.updating_weights[i], axis=0, ddof=1).tolist())
 
         return weight_avg, weight_err
 
-    def identify_swappable_pairs(self, states, state_ranges):
+    @staticmethod
+    def identify_swappable_pairs(states, state_ranges, neighbor_exchange, add_swappables=None):
         """
         Identify swappable pairs. By definition, a pair of simulation is considered swappable only if
         their last sampled states are in the alchemical ranges of both simulations. This is required
         to ensure that the values of involved ΔH and Δg can always be looked up from the DHDL and LOG files.
         This also automatically guarantee that the simulations to be swapped have overlapping alchemical ranges.
 
         Parameters
         ----------
         states : list
             A list of the global indices of the last sampled states of all simulations. This list can be
             generated by the :obj:`.extract_final_dhdl_info` method. Notably, the input list should not be
             a list that has been updated/modified by :obj:`get_swapping_pattern`, or the result will be incorrect.
         state_ranges : list of lists
             A list of state indies for all replicas. The input list can be a list updated by
-            :code:`get_swapping_pattern`, especially in the case where there is a need to re-identify the
+            :obj:`.get_swapping_pattern`, especially in the case where there is a need to re-identify the
             swappable pairs after an attempted swap is accepted.
+        neighbor_exchange : bool
+            Whether to exchange only between neighboring replicas.
+        add_swappables: list
+            A list of lists that additionally consider states (in global indices) that can be swapped.
+            For example, :code:`add_swappables=[[4, 5], [14, 15]]` means that if a replica samples state 4,
+            it can be swapped with another replica that samples state 5 and vice versa. The same logic applies
+            to states 14 and 15.
 
         Returns
         -------
         swappables : list
             A list of tuples representing the simulations that can be swapped.
         """
-        sim_idx = list(range(self.n_sim))
+        n_sim = len(states)
+        sim_idx = list(range(n_sim))
         all_pairs = list(combinations(sim_idx, 2))
 
         # First, we identify pairs of replicas with overlapping ranges
         swappables = [i for i in all_pairs if set(state_ranges[i[0]]).intersection(set(state_ranges[i[1]])) != set()]  # noqa: E501
 
         # Then, from these pairs, we exclude the ones whose the last sampled states are not present in both alchemical ranges  # noqa: E501
         # In this case, U^i_n, U_^j_m, g^i_n, and g_^j_m are unknown and the acceptance cannot be calculated.
         swappables = [i for i in swappables if states[i[0]] in state_ranges[i[1]] and states[i[1]] in state_ranges[i[0]]]  # noqa: E501
 
-        if self.proposal == 'neighboring':
+        # Expand the definition of swappable pairs when add_swappables is specified
+        if add_swappables is not None:
+            all_paired_states = [[states[p[0]], states[p[1]]] for p in all_pairs]
+            for i in all_paired_states:
+                if i in add_swappables:
+                    pair = all_pairs[all_paired_states.index(i)]
+                    if pair not in swappables:
+                        swappables.append(pair)
+
+        if neighbor_exchange is True:
             print('Note: One neighboring swap will be proposed.')
             swappables = [i for i in swappables if np.abs(i[0] - i[1]) == 1]
 
         return swappables
 
-    def propose_swap(self, swappables):
+    @staticmethod
+    def propose_swap(swappables):
         """
         Proposes a swap of coordinates between replicas by drawing samples from the swappable pairs.
 
         Parameters
         ----------
         swappables : list
             A list of tuples representing the simulations that can be swapped.
@@ -727,16 +862,19 @@
         weights : list
             A list of lists of final weights of ALL simulations. :code:`weights[i]` corresponds to the list of weights
             used in replica :code:`i`. The list can be generated by :obj:`.extract_final_log_info`.
 
         Returns
         -------
         swap_pattern : list
-            A list that represents how the replicas should be swapped.
+            A list showing the configuration of replicas after swapping.
+        swap_list : list
+            A list of tuples showing the accepted swaps.
         """
+        swap_list = []
         if self.proposal != 'multiple':
             if self.proposal == 'exhaustive':
                 n_ex = int(np.floor(self.n_sim / 2))  # This is the maximum, not necessarily the number that will always be reached.  # noqa
                 n_ex_exhaustive = 0    # The actual number of swaps atttempted.
             else:
                 n_ex = 1  # single swap or neighboring swap
         else:
@@ -746,80 +884,83 @@
             else:
                 n_ex = self.n_ex
 
         shifts = list(self.s * np.arange(self.n_sim))
         swap_pattern = list(range(self.n_sim))   # Can be regarded as the indices of DHDL files/configurations
         state_ranges = copy.deepcopy(self.state_ranges)
         states_copy = copy.deepcopy(states)  # only for re-identifying swappable pairs given updated state_ranges
-        swappables = self.identify_swappable_pairs(states, state_ranges)
+        swappables = EnsembleEXE.identify_swappable_pairs(states, state_ranges, self.proposal == 'neighboring', self.add_swappables)  # noqa: E501
 
         # Note that if there is only 1 swappable pair, then it will still be the only swappable pair
         # after an attempted swap is accepted. Therefore, there is no need to perform multiple swaps or re-identify
         # the new set of swappable pairs. In this case, we set n_ex back to 1.
         if len(swappables) == 1:
             if n_ex > 1:
-                print('n_ex is set back to 1 since there is only 1 swappable pair.')
-                n_ex = 1
+                n_ex = 1  # n_ex is set back to 1 since there is only 1 swappable pair.
 
         print(f"Swappable pairs: {swappables}")
         for i in range(n_ex):
             # Update the list of swappable pairs starting from the 2nd attempted swap for the exhaustive swap method.
             if self.proposal == 'exhaustive' and i >= 1:
                 # Note that this should be done regardless of the acceptance/rejection of the previously drawn pairs.
                 # Also note that at this point, swap is still the last attempted swap.
                 swappables = [i for i in swappables if set(i).intersection(set(swap)) == set()]  # noqa: F821
                 print(f'\nRemaining swappable pairs: {swappables}')
 
             if len(swappables) == 0 and self.proposal == 'exhaustive':
                 # This should only happen when the method of exhaustive swaps is used.
-                print(f'{n_ex_exhaustive} swap(s) have been attempted to exhaustively explore all possible swaps.')
                 if i == 0:
                     self.n_empty_swappable += 1
                 break
             else:
                 self.n_swap_attempts += 1
                 if self.proposal == 'exhaustive':
                     n_ex_exhaustive += 1
 
-                swap = self.propose_swap(swappables)
+                swap = EnsembleEXE.propose_swap(swappables)
                 print(f'\nProposed swap: {swap}')
                 if swap == []:
+                    self.n_empty_swappable += 1
                     print('No swap is proposed because there is no swappable pair at all.')
                     break  # no need to re-identify swappable pairs and draw new samples
                 else:
                     if self.verbose is True and self.proposal != 'exhaustive':
                         print(f'A swap ({i + 1}/{n_ex}) is proposed between the configurations of Simulation {swap[0]} (state {states[swap[0]]}) and Simulation {swap[1]} (state {states[swap[1]]}) ...')  # noqa: E501
 
-                    # Calculate the acceptance ratio and decide whether to accept the swap.
-                    prob_acc = self.calc_prob_acc(swap, dhdl_files, states, shifts, weights)
-                    swap_bool = self.accept_or_reject(prob_acc)
+                    if self.modify_coords_fn is not None:
+                        swap_bool = True  # always accept the move
+                    else:
+                        # Calculate the acceptance ratio and decide whether to accept the swap.
+                        prob_acc = self.calc_prob_acc(swap, dhdl_files, states, shifts, weights)
+                        swap_bool = self.accept_or_reject(prob_acc)
 
                     # Theoretically, in an EEXE simulation, we could either choose to swap configurations (via
                     # swapping GRO files) or replicas (via swapping MDP files). In ensemble_md package, we chose the
                     # former when implementing the EEXE algorithm. Specifically, in the CLI `run_EEXE`, `swap_pattern`
                     # is used to swap the GRO files. Therefore, when an attempted swap is accetped and `swap_pattern`
                     # is updated, we also need to update the variables `shifts`, `weights`, `dhdl_files`,
                     # `state_ranges`, `self.configs` but not anything else. Otherwise, incorrect results will be
                     # produced. To better understand this, one can refer to our unit test for get_swapping_pattern
                     # and calc_prob_acc, set checkpoints and examine why the variables should/should not be updated.
 
                     if swap_bool is True:
+                        swap_list.append(swap)
                         # The assignments need to be done at the same time in just one line.
                         # states[swap[0]], states[swap[1]] = states[swap[1]], states[swap[0]]
                         shifts[swap[0]], shifts[swap[1]] = shifts[swap[1]], shifts[swap[0]]
                         weights[swap[0]], weights[swap[1]] = weights[swap[1]], weights[swap[0]]
                         dhdl_files[swap[0]], dhdl_files[swap[1]] = dhdl_files[swap[1]], dhdl_files[swap[0]]
                         swap_pattern[swap[0]], swap_pattern[swap[1]] = swap_pattern[swap[1]], swap_pattern[swap[0]]
                         state_ranges[swap[0]], state_ranges[swap[1]] = state_ranges[swap[1]], state_ranges[swap[0]]
                         self.configs[swap[0]], self.configs[swap[1]] = self.configs[swap[1]], self.configs[swap[0]]
 
                         if n_ex > 1 and self.proposal == 'multiple':  # must be multiple swaps
                             # After state_ranges have been updated, we re-identify the swappable pairs.
                             # Notably, states_copy (instead of states) should be used. (They could be different.)
-                            swappables = self.identify_swappable_pairs(states_copy, state_ranges)
+                            swappables = EnsembleEXE.identify_swappable_pairs(states_copy, state_ranges, self.proposal == 'neighboring', self.add_swappables)  # noqa: E501
                             print(f"  New swappable pairs: {swappables}")
                     else:
                         # In this case, there is no need to update the swappables
                         pass
 
                 print(f'  Current list of configurations: {self.configs}')
 
@@ -828,15 +969,15 @@
         print(f'\nThe finally adopted swap pattern: {swap_pattern}')
         print(f'The list of configurations sampled in each replica in the next iteration: {self.configs}')
 
         # Update the replica-space trajectories
         for i in range(self.n_sim):
             self.rep_trajs[i].append(self.configs.index(i))
 
-        return swap_pattern
+        return swap_pattern, swap_list
 
     def calc_prob_acc(self, swap, dhdl_files, states, shifts, weights):
         """
         Calculates the acceptance ratio given the Monte Carlo scheme for swapping the simulations.
 
         Parameters
         ----------
@@ -1003,28 +1144,31 @@
                 print(f'  Corrected weights of rep {i}:\t{[float(f"{k:.3f}") for k in weights[i]]}\n')
 
         if self.verbose is False:
             print(' Done')
 
         return weights
 
-    def combine_weights(self, weights):
+    def combine_weights(self, weights, weights_err=None):
         """
-        Combine alchemical weights across multiple replicas. (See :ref:`doc_w_schemes` for mor details.)
+        Combine alchemical weights across multiple replicas. Note that if
+        :code:`weights_err` is provided, inverse-variance weighting will be used.
+        Care must be taken since inverse-variance weighting can lead to slower
+        convergence if the provided errors are not accurate. (See :ref:`doc_w_schemes` for mor details.)
 
         Parameters
         ----------
         weights : list
             A list of Wang-Landau weights of ALL simulations
 
         Returns
         -------
         weights : list
             A list of modified Wang-Landau weights of ALL simulations.
-        g_vec : np.array
+        g_vec : np.ndarray
             An array of alchemical weights of the whole range of states.
         """
         if self.verbose is True:
             print('Performing weight combination ...')
         else:
             print('Performing weight combination ...', end='')
 
@@ -1033,61 +1177,32 @@
             print('  Original weights:')
             for i in range(len(w)):
                 print(f'    Rep {i}: {w[i]}')
 
         # Method based on weight differences (the original g-diff)
         dg_vec = []
         dg_adjacent = [list(np.diff(weights[i])) for i in range(len(weights))]
+        if weights_err is not None:
+            dg_adjacent_err = [[np.sqrt(weights_err[i][j] ** 2 + weights_err[i][j + 1] ** 2) for j in range(len(weights_err[i]) - 1)] for i in range(len(weights_err))]  # noqa: E501
+
         for i in range(self.n_tot - 1):
-            dg_list = []
+            dg_list, dg_err_list = [], []
             for j in range(len(self.state_ranges)):
                 if i in self.state_ranges[j] and i + 1 in self.state_ranges[j]:
                     idx = self.state_ranges[j].index(i)
                     dg_list.append(dg_adjacent[j][idx])
-            dg_vec.append(np.mean(dg_list))
+                    if weights_err is not None:
+                        dg_err_list.append(dg_adjacent_err[j][idx])
+            if weights_err is None:
+                dg_vec.append(np.mean(dg_list))
+            else:
+                dg_vec.append(utils.weighted_mean(dg_list, dg_err_list)[0])
         dg_vec.insert(0, 0)
         g_vec = np.array([sum(dg_vec[:(i + 1)]) for i in range(len(dg_vec))])
 
-        """  Deprecated methods: mean and geo-mean
-        # Method based on probability ratios
-        # Step 1: Convert the weights into probabilities
-        weights = np.array(weights)
-        prob = np.array([[np.exp(-i)/np.sum(np.exp(-weights[j])) for i in weights[j]] for j in range(len(weights))])  # noqa: E501
-
-        # Step 2: Caclulate the probability ratios (after figuring out overlapped states between adjacent replicas)  # noqa: E501
-        overlapped = [set(self.state_ranges[i]).intersection(set(self.state_ranges[i + 1])) for i in range(len(self.state_ranges) - 1)]  # noqa: E501
-        prob_ratio = [prob[i + 1][: len(overlapped[i])] / prob[i][-len(overlapped[i]):] for i in range(len(overlapped))]  # noqa: E501
-
-        # Step 3: Average the probability ratios
-        avg_ratio = [1]   # This allows easier scaling since the first prob vector stays the same.
-        if self.w_scheme == 'mean':
-            avg_ratio.extend([np.mean(prob_ratio[i]) for i in range(len(prob_ratio))])
-        elif self.w_scheme == 'geo-mean':
-            avg_ratio.extend([np.prod(prob_ratio[i])**(1/len(prob_ratio[i])) for i in range(len(prob_ratio))])
-
-        # Step 4: Scale the probabilities for each replica
-        scaled_prob = np.array([prob[i] / np.prod(avg_ratio[: i + 1]) for i in range(len(prob))])
-
-        # Step 5: Average and convert the probabilities
-        p_vec = []
-        for i in range(self.n_tot):   # global state index
-            p = []   # a list of probabilities to be averaged for each state
-            for j in range(len(self.state_ranges)):   # j can be regared as the replica index
-                if i in self.state_ranges[j]:
-                    local_idx = i - j * self.s
-                    p.append(scaled_prob[j][local_idx])
-            if self.w_scheme == 'mean':
-                p_vec.append(np.mean(p))
-            elif self.w_scheme == 'geo-mean' or self.w_scheme == 'geo_mean':
-                p_vec.append(np.prod(p) ** (1 / len(p)))
-
-        g_vec = -np.log(p_vec)
-        g_vec -= g_vec[0]
-        """
-
         # Determine the vector of alchemical weights for each replica
         for i in range(self.n_sim):
             if self.equil[i] == -1:  # unequilibrated
                 weights[i] = list(g_vec[i: i + self.n_sub] - g_vec[i: i + self.n_sub][0])
             else:
                 weights[i] = self.equilibrated_weights[i]
         weights = np.round(weights, decimals=5).tolist()
@@ -1139,29 +1254,34 @@
         Prepares TPR files for the simulation ensemble using the GROMACS :code:`grompp` command.
 
         Parameters
         ----------
         n : int
             The iteration index (starting from 0).
         swap_pattern : list
-            A list generated by :code:`get_swapping_pattern`. It represents how the replicas should be swapped.
+            A list generated by :obj:`.get_swapping_pattern`. It represents how the replicas should be swapped.
         """
         args_list = []
         for i in range(self.n_sim):
-            # mpirun -np 1 does not seem needed here.
-            # Actually, it made stderr and stdout both empty even if the return code is 1 ...
             arguments = [self.gmx_executable, 'grompp']
 
             # Input files
             mdp = f"sim_{i}/iteration_{n}/{self.mdp.split('/')[-1]}"
             if n == 0:
-                gro = f"{self.gro}"
+                if isinstance(self.gro, list):
+                    gro = f"{self.gro[i]}"
+                else:
+                    gro = f"{self.gro}"
             else:
                 gro = f"sim_{swap_pattern[i]}/iteration_{n-1}/confout.gro"  # This effectively swap out GRO files
-            top = f"{self.top}"
+
+            if isinstance(self.top, list):
+                top = f"{self.top[i]}"
+            else:
+                top = f"{self.top}"
 
             # Add input file arguments
             arguments.extend(["-f", mdp, "-c", gro, "-p", top])
 
             # Add output file arguments
             arguments.extend([
                 "-o", f"sim_{i}/iteration_{n}/sys_EE.tpr",
@@ -1173,19 +1293,30 @@
                 # Turn the dictionary into a list with the keys alternating with values
                 add_args = [elem for pair in self.grompp_args.items() for elem in pair]
                 arguments.extend(add_args)
 
             args_list.append(arguments)
 
         # Run the GROMACS grompp commands in parallel
+        returncode = None  # Initialize as None for all ranks (necessary for the case when -np > n_sim, which is rare)
+        if rank == 0:
+            print('Generating TPR files ...')
         if rank < self.n_sim:
-            print(f'Generating a TPR file on rank {rank} ...')
             returncode, stdout, stderr = self.run_gmx_cmd(args_list[rank])
             if returncode != 0:
-                print(f'Error on rank {rank}:\n{stderr}')
+                print(f'Error on rank {rank} (return code: {returncode}):\n{stderr}')
+
+        # gather return codes at rank 0
+        code_list = comm.gather(returncode, root=0)
+
+        if rank == 0:
+            # Filter out None values which represent ranks that did not execute the command
+            code_list = [code for code in code_list if code is not None]
+            if code_list != [0] * self.n_sim:
+                MPI.COMM_WORLD.Abort(1)   # Doesn't matter what non-zero returncode we put here as the code from GROMACS will be printed before this point anyway.  # noqa: E501
 
     def run_mdrun(self, n):
         """
         Executes GROMACS mdrun commands in parallel.
 
         Parameters
         ----------
@@ -1200,36 +1331,46 @@
 
         if self.runtime_args is not None:
             # Turn the dictionary into a list with the keys alternating with values
             add_args = [elem for pair in self.runtime_args.items() for elem in pair]
             arguments.extend(add_args)
 
         # Run the GROMACS mdrun commands in parallel
+        returncode = None  # Initialize as None for all ranks (necessary for the case when -np > n_sim, which is rare)
+        if rank == 0:
+            print('Running EXE simulations ...')
         if rank < self.n_sim:
-            print(f'Running an EXE simulation on rank {rank} ...')
             os.chdir(f'sim_{rank}/iteration_{n}')
             returncode, stdout, stderr = self.run_gmx_cmd(arguments)
             if returncode != 0:
-                print(f'Error on rank {rank}:\n{stderr}')
-                sys.exit(returncode)
+                print(f'Error on rank {rank} (return code: {returncode}):\n{stderr}')
             os.chdir('../../')
 
+        # gather return codes at rank 0
+        code_list = comm.gather(returncode, root=0)
+
+        if rank == 0:
+            # Filter out None values which represent ranks that did not execute the command
+            code_list = [code for code in code_list if code is not None]
+            if code_list != [0] * self.n_sim:
+                MPI.COMM_WORLD.Abort(1)   # Doesn't matter what non-zero returncode we put here as the code from GROMACS will be printed before this point anyway.  # noqa: E501
+
     def run_EEXE(self, n, swap_pattern=None):
         """
         Perform one iteration in the EEXE simulation, which includes generating the
         TPR files using the GROMACS grompp :code:`command` and running the expanded ensemble simulations
         in parallel using GROMACS :code:`mdrun` command. The GROMACS commands are launched by as subprocesses.
         The function assumes that the GROMACS executable is available.
 
         Parameters
         ----------
         n : int
             The iteration index (starting from 0).
         swap_pattern : list
-            A list generated by :code:`get_swapping_pattern`. It represents how the replicas should be swapped.
+            A list generated by :obj:`.get_swapping_pattern`. It represents how the replicas should be swapped.
             This parameter is not needed only if :code:`n` is 0.
         """
         if rank == 0:
             iter_str = f'\nIteration {n}: {self.dt * self.nst_sim * n: .1f} - {self.dt * self.nst_sim * (n + 1): .1f} ps'  # noqa: E501
             print(iter_str + '\n' + '=' * (len(iter_str) - 1))
 
         # 1st synchronizing point for all MPI processes: To make sure ranks other than 0 will not start executing
```

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg` & `ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_0.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg` & `ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_1.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg` & `ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_2.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg` & `ensemble_md-0.7.0/ensemble_md/tests/data/dhdl/dhdl_3.xvg`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/expanded.mdp` & `ensemble_md-0.7.0/ensemble_md/tests/data/expanded.mdp`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 nstcomm = 1
 nstfout = 0
 
 ; Output control
 nstlog = 100
 nstcalcenergy = 1
 nstenergy = 1000
-nstxout_compressed = 1000
+nstxout_compressed = 100
 
 ; Neighborsearching and short-range nonbonded interactions
 nstlist = 10
 ns_type = grid
 pbc = xyz
 rlist = 1.0
```

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_0.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_0.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_1.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_1.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_2.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_2.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/EXE_3.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/EXE_3.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/HREX.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/HREX.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_1.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/case2_1.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/case2_2.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/case2_2.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/log/case3.log` & `ensemble_md-0.7.0/ensemble_md/tests/data/log/case3.log`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/sys.gro` & `ensemble_md-0.7.0/ensemble_md/tests/data/sys.gro`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/data/sys.top` & `ensemble_md-0.7.0/ensemble_md/tests/data/sys.top`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/test_analyze_matrix.py` & `ensemble_md-0.7.0/ensemble_md/tests/test_analyze_matrix.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/test_analyze_traj.py` & `ensemble_md-0.7.0/ensemble_md/tests/test_analyze_traj.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/test_ensemble_EXE.py` & `ensemble_md-0.7.0/ensemble_md/tests/test_ensemble_EXE.py`

 * *Files 10% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
         # 8. nstlog > nst_sim
         mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))  # A perfect mdp file
         mdp['nstlog'] = 200
         mdp.write(os.path.join(input_path, "expanded_test.mdp"))
         params_dict['mdp'] = 'ensemble_md/tests/data/expanded_test.mdp'
         params_dict['nst_sim'] = 100
-        with pytest.raises(ParameterError, match='The parameter "nstlog" should be equal to or smaller than "nst_sim" specified in the YAML file so that the sampling information can be parsed.'):  # noqa: E501
+        with pytest.raises(ParameterError, match='The parameter "nstlog" must be a factor of the parameter "nst_sim" specified in the YAML file.'):  # noqa: E501
             get_EEXE_instance(params_dict)
         params_dict['nst_sim'] = 500
         os.remove(os.path.join(input_path, "expanded_test.mdp"))
 
         # 9. n_sub < 1
         params_dict['s'] = 5
         params_dict['mdp'] = 'ensemble_md/tests/data/expanded.mdp'
@@ -133,30 +133,27 @@
         warning = 'Warning: Parameter "cool" specified in the input YAML file is not recognizable.'
         assert warning in EEXE.warnings
 
         # 2. Warnings related to the mdp file
         mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))  # A perfect mdp file
         mdp['lmc_seed'] = 1000
         mdp['gen_seed'] = 1000
-        mdp['symmetrized_transition_matrix'] = 'yes'
         mdp['wl_scale'] = ''
         mdp.write(os.path.join(input_path, "expanded_test.mdp"))
 
         params_dict['mdp'] = 'ensemble_md/tests/data/expanded_test.mdp'
         params_dict['N_cutoff'] = 1000
         EEXE = get_EEXE_instance(params_dict)
 
         warning_1 = 'Warning: The histogram correction/weight combination method is specified but will not be used since the weights are fixed.'  # noqa: E501
         warning_2 = 'Warning: We recommend setting lmc_seed as -1 so the random seed is different for each iteration.'
         warning_3 = 'Warning: We recommend setting gen_seed as -1 so the random seed is different for each iteration.'
-        warning_4 = 'Warning: We recommend setting symmetrized-transition-matrix to no instead of yes.'
         assert warning_1 in EEXE.warnings
         assert warning_2 in EEXE.warnings
         assert warning_3 in EEXE.warnings
-        assert warning_4 in EEXE.warnings
 
         os.remove(os.path.join(input_path, "expanded_test.mdp"))
 
     def test_set_params(self, params_dict):
         # 0. Get an EEXE instance to test
         EEXE = get_EEXE_instance(params_dict)
 
@@ -183,22 +180,21 @@
         assert EEXE.df_spacing == 1
         assert EEXE.df_method == 'MBAR'
         assert EEXE.err_method == 'propagate'
         assert EEXE.n_bootstrap == 50
         assert EEXE.seed is None
 
         # 3. Check the MDP parameters
-        assert EEXE.nsteps == 500
         assert EEXE.dt == 0.002
         assert EEXE.temp == 298
         assert EEXE.nst_sim == 500
         assert EEXE.fixed_weights is False
 
         # 4. Checked the derived parameters
-        # Note that lambda_dict and lambda_ranges will also be tested in test_map_lambda2state.
+        # Note that lambda_dict will also be tested in test_map_lambda2state.
         k = 1.380649e-23
         NA = 6.0221408e23
         assert EEXE.kT == k * NA * 298 / 1000
         assert EEXE.lambda_types == ['coul_lambdas', 'vdw_lambdas']
         assert EEXE.n_tot == 9
         assert EEXE.n_sub == 6
         assert EEXE.state_ranges == [
@@ -257,70 +253,14 @@
         assert EEXE.reformatted_mdp is True
         assert EEXE.template['cool_stuff'] == 10
         assert os.path.isfile(os.path.join(input_path, "expanded_test_backup.mdp"))
 
         os.remove(os.path.join(input_path, "expanded_test.mdp"))
         os.remove(os.path.join(input_path, "expanded_test_backup.mdp"))
 
-    def test_map_lambda2state(self, params_dict):
-        # Note that the function map_lambda2state is called in set_params
-        EEXE = get_EEXE_instance(params_dict)
-        assert EEXE.lambda_dict == {
-            (0, 0): 0,
-            (0.25, 0): 1,
-            (0.5, 0): 2,
-            (0.75, 0): 3,
-            (1, 0): 4,
-            (1, 0.25): 5,
-            (1, 0.5): 6,
-            (1, 0.75): 7,
-            (1, 1): 8}
-        assert EEXE.lambda_ranges == [
-            [(0.0, 0.0), (0.25, 0.0), (0.5, 0.0), (0.75, 0.0), (1.0, 0.0), (1.0, 0.25)],
-            [(0.25, 0.0), (0.5, 0.0), (0.75, 0.0), (1.0, 0.0), (1.0, 0.25), (1.0, 0.5)],
-            [(0.5, 0.0), (0.75, 0.0), (1.0, 0.0), (1.0, 0.25), (1.0, 0.5), (1.0, 0.75)],
-            [(0.75, 0.0), (1.0, 0.0), (1.0, 0.25), (1.0, 0.5), (1.0, 0.75), (1.0, 1.0)], ]
-
-        # Here we test another combinations: only 'fep_lambdas'
-        mdp = gmx_parser.MDP(os.path.join(input_path, "expanded.mdp"))
-        del mdp['coul_lambdas']
-        del mdp['vdw_lambdas']
-        mdp['fep_lambdas'] = '0.0 0.2 0.4 0.6 0.8 1.0'
-        mdp.write(os.path.join(input_path, "expanded_test.mdp"))
-        params_dict['mdp'] = 'ensemble_md/tests/data/expanded_test.mdp'
-        params_dict['n_sim'] = 3
-        EEXE = get_EEXE_instance(params_dict)
-        assert EEXE.lambda_types == ['fep_lambdas']
-        assert EEXE.lambda_dict == {
-            (0.0,): 0, (0.2,): 1, (0.4,): 2, (0.6,): 3, (0.8,): 4, (1.0,): 5}
-        assert EEXE.lambda_ranges == [
-            [(0.0, ), (0.2,), (0.4,), (0.6,)], [(0.2,), (0.4,), (0.6,), (0.8,)], [(0.4,), (0.6,), (0.8,), (1.0,)]]
-
-        # Still another combination: fep_lambdas, coul_lambdas, vdw_lambdas, restraint_lambdas
-        mdp['coul_lambdas'] = '0.0 0.5 0.8 1.0 1.0 1.0'
-        mdp['vdw_lambdas'] = '0.0 0.0 0.0 0.0 0.5 1.0'
-        mdp['restraint_lambdas'] = '0.0 0.2 0.4 0.6 0.8 1.0'
-        mdp.write(os.path.join(input_path, "expanded_test.mdp"))
-        EEXE = get_EEXE_instance(params_dict)
-        assert EEXE.lambda_types == ['fep_lambdas', 'coul_lambdas', 'vdw_lambdas', 'restraint_lambdas']
-        assert EEXE.lambda_dict == {
-            (0.0, 0.0, 0.0, 0.0): 0,
-            (0.2, 0.5, 0.0, 0.2): 1,
-            (0.4, 0.8, 0.0, 0.4): 2,
-            (0.6, 1.0, 0.0, 0.6): 3,
-            (0.8, 1.0, 0.5, 0.8): 4,
-            (1.0, 1.0, 1.0, 1.0): 5}
-
-        assert EEXE.lambda_ranges == [
-            [(0.0, 0.0, 0.0, 0.0), (0.2, 0.5, 0.0, 0.2), (0.4, 0.8, 0.0, 0.4), (0.6, 1.0, 0.0, 0.6)],
-            [(0.2, 0.5, 0.0, 0.2), (0.4, 0.8, 0.0, 0.4), (0.6, 1.0, 0.0, 0.6), (0.8, 1.0, 0.5, 0.8)],
-            [(0.4, 0.8, 0.0, 0.4), (0.6, 1.0, 0.0, 0.6), (0.8, 1.0, 0.5, 0.8), (1.0, 1.0, 1.0, 1.0)]]
-
-        os.remove(os.path.join(input_path, "expanded_test.mdp"))
-
     def test_print_params(self, capfd, params_dict):
         # capfd is a fixture in pytest for testing STDOUT
         EEXE = get_EEXE_instance(params_dict)
         EEXE.print_params()
         out_1, err = capfd.readouterr()
         L = ""
         L += "Important parameters of EXEE\n============================\n"
@@ -333,16 +273,18 @@
         L += "Proposal scheme: exhaustive\n"
         L += "Acceptance scheme for swapping simulations: metropolis\n"
         L += "Whether to perform weight combination: False\n"
         L += "Histogram cutoff: 1000\nNumber of replicas: 4\nNumber of iterations: 10\n"
         L += "Number of attempted swaps in one exchange interval: N^3\n"
         L += "Length of each replica: 1.0 ps\nFrequency for checkpointing: 100 iterations\n"
         L += "Total number of states: 9\n"
+        L += "Additionally defined swappable states: None\n"
         L += "Additional grompp arguments: None\n"
         L += "Additional runtime arguments: None\n"
+        L += "MDP parameters differing across replicas: None\n"
         L += "Alchemical ranges of each replica in EEXE:\n  - Replica 0: States [0, 1, 2, 3, 4, 5]\n"
         L += "  - Replica 1: States [1, 2, 3, 4, 5, 6]\n  - Replica 2: States [2, 3, 4, 5, 6, 7]\n"
         L += "  - Replica 3: States [3, 4, 5, 6, 7, 8]\n"
         assert out_1 == L
 
         EEXE.reformatted_mdp = True  # Just to test the case where EEXE.reformatted_mdp is True
         EEXE.print_params(params_analysis=True)
@@ -459,20 +401,20 @@
 
     def test_identify_swappable_pairs(self, params_dict):
         EEXE = get_EEXE_instance(params_dict)
         EEXE.state_ranges = [list(range(i, i + 5)) for i in range(EEXE.n_sim)]  # 5 states per replica
         states = [4, 2, 2, 7]   # This would lead to the swappables: [(0, 1), (0, 2), (1, 2)] in the standard case
 
         # Case 1: Any case that is not neighboring swap has the same definition for the swappable pairs
-        swappables_1 = EEXE.identify_swappable_pairs(states, EEXE.state_ranges)
+        swappables_1 = EEXE.identify_swappable_pairs(states, EEXE.state_ranges, EEXE.proposal == 'neighboring')
         assert swappables_1 == [(0, 1), (0, 2), (1, 2)]
 
         # Case 2: Neighboring exchange
         EEXE.proposal = 'neighboring'
-        swappables_2 = EEXE.identify_swappable_pairs(states, EEXE.state_ranges)
+        swappables_2 = EEXE.identify_swappable_pairs(states, EEXE.state_ranges, EEXE.proposal == 'neighboring')
         assert swappables_2 == [(0, 1), (1, 2)]
 
     def test_propose_swap(self, params_dict):
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         swap_1 = EEXE.propose_swap([])
         swap_2 = EEXE.propose_swap([(0, 1), (0, 2), (1, 2)])
@@ -490,88 +432,95 @@
         dhdl_files = [os.path.join(input_path, f"dhdl/dhdl_{i}.xvg") for i in range(4)]
 
         # Case 1: Empty swap list
         EEXE = get_EEXE_instance(params_dict)
         EEXE.verbose = False
         states = [0, 6, 7, 8]  # No swappable pairs
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_1 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_1, swap_list_1 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_empty_swappable == 1
         assert EEXE.n_swap_attempts == 0
         assert EEXE.n_rejected == 0
         assert pattern_1 == [0, 1, 2, 3]
+        assert swap_list_1 == []
 
         # Case 2: Single swap (proposal = 'single')
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.verbose = True
         EEXE.proposal = 'single'  # n_ex will be set to 1 automatically.
         states = [5, 2, 2, 8]  # swappable pairs: [(0, 1), (0, 2), (1, 2)], swap = (1, 2), accept
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_2 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_2, swap_list_2 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 1
         assert EEXE.n_rejected == 0
         assert pattern_2 == [0, 2, 1, 3]
+        assert swap_list_2 == [(1, 2)]
 
         # Case 3: Neighboring swap
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.proposal = 'neighboring'  # n_ex will be set to 1 automatically.
         states = [5, 2, 2, 8]  # swappable pairs: [(0, 1), (1, 2)], swap = (1, 2), accept
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_3 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_3, swap_list_3 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 1
         assert EEXE.n_rejected == 0
         assert pattern_3 == [0, 2, 1, 3]
+        assert swap_list_3 == [(1, 2)]
 
         # Case 4-1: Exhaustive swaps that end up in a single swap
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.proposal = 'exhaustive'
         states = [5, 2, 2, 8]  # swappable pairs: [(0, 1), (0, 2), (1, 2)], swap = (1, 2), accept
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_4_1 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_4_1, swap_list_4_1 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 1
         assert EEXE.n_rejected == 0
         assert pattern_4_1 == [0, 2, 1, 3]
+        assert swap_list_4_1 == [(1, 2)]
 
         # Case 4-2: Exhaustive swaps that involve multiple attempted swaps
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.proposal = 'exhaustive'
         states = [4, 2, 4, 3]  # swappable pairs: [(0, 1), (0, 2), (0, 3), (1, 2), (2, 3)]; swap 1: (2, 3), accepted; swap 2: (0, 1), accept  # noqa: E501
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_4_2 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_4_2, swap_list_4_2 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 2   # \Delta is negative for both swaps -> both accepted
         assert EEXE.n_rejected == 0
         assert pattern_4_2 == [1, 0, 3, 2]
+        assert swap_list_4_2 == [(2, 3), (0, 1)]
 
         # Case 5-1: Multiple swaps (proposal = 'multiple', n_ex = 5)
         print('test 5-1')
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         EEXE.n_ex = 5
         EEXE.proposal = 'multiple'
-        states = [3, 1, 4, 6]  # swappable pairs: [(0, 1), (0, 2), (1, 2)], first swap = (1, 2), accept
+        states = [3, 1, 4, 6]  # swappable pairs: [(0, 1), (0, 2), (1, 2)], first swap = (0, 2), accept
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_5_1 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_5_1, swap_list_5_1 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 5
         assert EEXE.n_rejected == 4
         assert pattern_5_1 == [2, 1, 0, 3]
+        assert swap_list_5_1 == [(0, 2)]
 
         # Case 5-2: Multiple swaps but with only one swappable pair (proposal = 'multiple')
         # This is specifically for testing n_swap_attempts in the case where n_ex reduces to 1.
         random.seed(0)
         EEXE = get_EEXE_instance(params_dict)
         states = [0, 2, 3, 8]  # The only swappable pair is [(1, 2)] --> accept
         w, f = copy.deepcopy(weights), copy.deepcopy(dhdl_files)
-        pattern_5_2 = EEXE.get_swapping_pattern(f, states, w)
+        pattern_5_2, swap_list_5_2 = EEXE.get_swapping_pattern(f, states, w)
         assert EEXE.n_swap_attempts == 1  # since there is only 1 swappable pair
         assert EEXE.n_rejected == 0
         assert pattern_5_2 == [0, 2, 1, 3]
+        assert swap_list_5_2 == [(1, 2)]
 
     def test_calc_prob_acc(self, capfd, params_dict):
         EEXE = get_EEXE_instance(params_dict)
         # EEXE.state_ranges = [[0, 1, 2, 3, 4, 5], [1, 2, 3, 4, 5, 6], ..., [3, 4, 5, 6, 7, 8]]
         states = [5, 2, 2, 8]
         shifts = [0, 1, 2, 3]
         weights = [
@@ -664,13 +613,22 @@
         EEXE.n_sub = 4
         EEXE.s = 1
         EEXE.n_sim = 3
         EEXE.state_ranges = [[0, 1, 2, 3], [1, 2, 3, 4], [2, 3, 4, 5]]
         weights = [[0, 2.1, 4.0, 3.7], [0, 1.7, 1.2, 2.6], [0, -0.4, 0.9, 1.9]]
 
         EEXE.w_combine = True
-        w, g_vec = EEXE.combine_weights(weights)
-        assert np.allclose(w, [
+        w_1, g_vec_1 = EEXE.combine_weights(weights)
+        assert np.allclose(w_1, [
             [0, 2.1, 3.9, 3.5],
             [0, 1.8, 1.4, 2.75],
             [0, -0.4, 0.95, 1.95]])
-        assert np.allclose(list(g_vec), [0, 2.1, 3.9, 3.5, 4.85, 5.85])
+        assert np.allclose(list(g_vec_1), [0, 2.1, 3.9, 3.5, 4.85, 5.85])
+
+        weights = [[0, 2.1, 4.0, 3.7], [0, 1.7, 1.2, 2.6], [0, -0.4, 0.9, 1.9]]
+        errors = [[0, 0.1, 0.15, 0.1], [0, 0.12, 0.1, 0.12], [0, 0.12, 0.15, 0.1]]
+        w_2, g_vec_2 = EEXE.combine_weights(weights, errors)
+        assert np.allclose(w_2, [
+            [0, 2.1, 3.86141, 3.45417],
+            [0, 1.76141, 1.35417, 2.71437],
+            [0, -0.40723, 0.95296, 1.95296]])
+        assert np.allclose(list(g_vec_2), [0, 2.1, 3.861407249466951, 3.4541731330165306, 4.814368891580968, 5.814368891580968])  # noqa: E501
```

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/test_gmx_parser.py` & `ensemble_md-0.7.0/ensemble_md/tests/test_gmx_parser.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/tests/test_utils.py` & `ensemble_md-0.7.0/ensemble_md/tests/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,18 +60,18 @@
     # Test string input that can be converted to int
     assert utils.autoconvert("42") == 42
 
     # Test string input that can be converted to float
     assert utils.autoconvert("3.14159") == 3.14159
 
     # Test string input that can be converted to a numpy array of ints
-    assert np.array_equal(utils.autoconvert("1 2 3"), np.array([1, 2, 3]))
+    assert utils.autoconvert("1 2 3") == [1, 2, 3]
 
     # Test string input that can be converted to a numpy array of floats
-    assert np.allclose(utils.autoconvert("1.0 2.0 3.0"), np.array([1.0, 2.0, 3.0]))
+    assert utils.autoconvert("1.0 2.0 3.0") == [1.0, 2.0, 3.0]
 
 
 def test_get_subplot_dimension():
     assert utils.get_subplot_dimension(1) == (1, 1)
     assert utils.get_subplot_dimension(2) == (1, 2)
     assert utils.get_subplot_dimension(3) == (2, 2)
     assert utils.get_subplot_dimension(4) == (2, 2)
```

### Comparing `ensemble_md-0.6.0/ensemble_md/utils/exceptions.py` & `ensemble_md-0.7.0/ensemble_md/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/ensemble_md/utils/gmx_parser.py` & `ensemble_md-0.7.0/ensemble_md/utils/gmx_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,18 @@
                         append_equil = True
 
             if "Weights have equilibrated" in l:
                 case = '2'  # we don't break the loop even if equil_time is found, as we need the final counts.
                 find_equil = True  # After this, we will append weights one last time, which are equilibrated weights.
                 equil_step = int(l.split(":")[0].split("Step")[1])
                 equil_time = equil_step * dt + tinit  # ps
-                if wl_delta < cutoff:
+                if wl_delta is not None and wl_delta < cutoff:
                     # Should only happen when equil_time % nstlog == 0, where the weights should have been appended
+                    # Note that we additionally have wl_delta is not None. Since wl_delta could be None if the
+                    # weights get equilibrated right after the simulation stop (before nstlog).
                     append_equil = True
 
             wl_delta = wl_delta_list[-1]
 
         if case == '2':
             wl_delta = None
```

### Comparing `ensemble_md-0.6.0/ensemble_md/utils/utils.py` & `ensemble_md-0.7.0/ensemble_md/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 """
 import sys
 import glob
 import natsort
 import datetime
 import collections
 import numpy as np
+from itertools import combinations
+from ensemble_md.utils import gmx_parser
 
 
 class Logger:
     """
     Redirects the STDOUT and STDERR to a specified output file while preserving them on screen.
 
     Parameters
@@ -64,26 +66,62 @@
         This method is needed for Python 3 compatibility. This handles the flush command by doing nothing.
         You might want to specify some extra behavior here.
         """
         # self.terminal.log()
         pass
 
 
+def compare_MDPs(mdp_list):
+    """
+    Given a list of MDP files, identify the parameters for which not all MDP
+    files have the same values. (Currently, this function is not used in the
+    workflow adopted in :code:`run_EEXE.py` but it might be useful in some places,
+    so we decided to keep it.)
+
+    Returns
+    -------
+    diff_params : list
+        The list of parameters differing between the input MDP files.
+    """
+    compare_list = list(combinations(mdp_list, r=2))
+    diff_params = []
+    for i in range(len(compare_list)):
+        mdp_1 = gmx_parser.MDP(compare_list[i][0])
+        mdp_2 = gmx_parser.MDP(compare_list[i][1])
+
+        # First figure out the union set of the parameters and exclude blanks and comments
+        all_params = set(list(mdp_1.keys()) + list(mdp_2.keys()))
+        all_params = [p for p in all_params if not p.startswith(('B', 'C'))]
+
+        for p in all_params:
+            if p in diff_params:
+                pass  # already in the list, no need to compare again
+            else:
+                if p not in mdp_1 or p not in mdp_2:
+                    diff_params.append(p)
+                else:
+                    # the parameter is in both MDP files
+                    if mdp_1[p] != mdp_2[p]:
+                        diff_params.append(p)
+
+    return diff_params
+
+
 def format_time(t):
     """
     Converts time in seconds to the "most readable" format.
 
     Parameters
     ----------
     t : float
         The time in seconds.
 
     Returns
     -------
-    t_str : sttr
+    t_str : str
         A string in the format of "XX day XX hour(s) XX minute(s) XX second(s)".
     """
     hh_mm_ss = str(datetime.timedelta(seconds=t)).split(":")
 
     if "day" in hh_mm_ss[0]:
         # hh_mm_ss[0] will contain "day" and cannot be converted to float
         hh, mm, ss = hh_mm_ss[0], float(hh_mm_ss[1]), float(hh_mm_ss[2])
@@ -130,19 +168,22 @@
         return s
     for converter in int, float, str:  # try them in increasing order of lenience
         try:
             s = [converter(i) for i in s.split()]
             if len(s) == 1:
                 return s[0]
             else:
+                return s
+                """
                 if len(s) != 0 and type(s[0]) == str:
-                    # For the case like pull_coord1_dim = Y Y Y, we don't want to us np.array
+                    # For the case like pull_coord1_dim = Y Y Y
                     return s
                 else:
                     return np.array(s)
+                """
         except (ValueError, AttributeError):
             pass
     raise ValueError("Failed to autoconvert {0!r}".format(s))
 
 
 def get_subplot_dimension(n_panels):
     """
@@ -166,15 +207,16 @@
         n_rows = int(np.floor(n_panels / n_cols)) + 1
 
     return n_rows, n_cols
 
 
 def weighted_mean(vals, errs):
     """
-    Calculates the inverse-variance-weighted mean.
+    Calculates the inverse-variance-weighted mean. Note that if
+    any error is 0, the simple mean will be returned.
 
     Parameters
     ----------
     vals : list
         A list of values to be averaged.
     errs : list
         A list of errors corresponding to the given values
@@ -182,14 +224,20 @@
     Returns
     -------
     mean : float
         The inverse-variance-weighted mean.
     err : float
         The propgated error of the mean.
     """
+    if 0 in errs:
+        # This could happen in the very beginning of a simulation, which could lead to an ZeroDivision warning/error.
+        # In this case, we just ignore the w vector and just calculate the simple average.
+        mean, err = np.mean(vals), None
+        return mean, err
+
     w = [1 / (i ** 2) for i in errs]
     wx = [w[i] * vals[i] for i in range(len(vals))]
     mean = np.sum(wx) / np.sum(w)
     err = np.sqrt(1 / np.sum(w))
 
     return mean, err
 
@@ -237,19 +285,23 @@
     Returns
     -------
     t_wall_tot : float
         The total wall time GROMACS spent to finish all iterations for the EEXE simulation.
     t_sync : float
         The total time spent in synchronizing all replicas, which is the sum of the differences
         between the longest and the shortest time elapsed to finish a iteration.
+    t_wall_list : list
+        The list of wall times of finishing each mdrun command.
     """
     n_iter = len(glob.glob('sim_0/iteration_*'))
     if log_files is None:
         log_files = [natsort.natsorted(glob.glob(f'sim_*/iteration_{i}/*log')) for i in range(n_iter)]
 
+    t_wall_list = []
     t_wall_tot, t_sync = 0, 0
     for i in range(n_iter):
         t_wall = [get_time_metrics(log_files[i][j])['t_wall'] for j in range(len(log_files[i]))]
+        t_wall_list.append(t_wall)
         t_wall_tot += max(t_wall)
         t_sync += (max(t_wall) - min(t_wall))
 
-    return t_wall_tot, t_sync
+    return t_wall_tot, t_sync, t_wall_list
```

### Comparing `ensemble_md-0.6.0/ensemble_md.egg-info/PKG-INFO` & `ensemble_md-0.7.0/ensemble_md.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensemble-md
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package for setting up, performing, and analyzing molecular dynamics ensembles using GROMACS
 Author: Wei-Tse Hsu
 Author-email: wehs7661@colorado.edu
 License: MIT
 Project-URL: Documentation, https://ensemble-md.readthedocs.io/
 Project-URL: Source Code, https://github.com/wehs7661/ensemble_md
 Keywords: molecular mechanics,free energy calculations,advanced sampling
@@ -37,16 +37,18 @@
 [//]: # (Badges)
 [![wehs7661](https://circleci.com/gh/wehs7661/ensemble_md.svg?style=shield)](https://app.circleci.com/pipelines/github/wehs7661/ensemble_md?branch=master)
 [![codecov](https://codecov.io/gh/wehs7661/ensemble_md/branch/master/graph/badge.svg)](https://app.codecov.io/gh/wehs7661/ensemble_md/tree/master)
 [![Documentation Status](https://readthedocs.org/projects/ensemble-md/badge/?version=latest)](https://ensemble-md.readthedocs.io/en/latest/?badge=latest)
 [![GitHub Actions Lint Status](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml/badge.svg)](https://github.com/wehs7661/ensemble_md/actions/workflows/lint.yaml)
 [![PyPI version](https://badge.fury.io/py/ensemble-md.svg)](https://badge.fury.io/py/ensemble-md)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+[![Downloads](https://static.pepy.tech/badge/ensemble-md)](https://pepy.tech/project/ensemble-md)
+[![Twitter Follow](https://img.shields.io/twitter/follow/WeiTseHsu?style=social)](https://twitter.com/WeiTseHsu)
 
-**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble_md.readthedocs.io/).
+**ensemble_md** is a Python package that provides methods for setting up, running, and analyzing molecular dynamics ensembles in GROMACS. The current implementation is mainly for synchronous ensemble of expanded ensemble (EXEE), but we will develop methods like asynchronous EEXE, or ensemble of alchemical metadynamics in the future. For installation instructions, theory overview, tutorials, and API references, please visit the [documentation](https://ensemble-md.readthedocs.io/en/latest/?badge=latest).
 
 ### Copyright
 
 Copyright (c) 2022, Wei-Tse Hsu
 
 
 #### Acknowledgements
```

### Comparing `ensemble_md-0.6.0/ensemble_md.egg-info/SOURCES.txt` & `ensemble_md-0.7.0/ensemble_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/setup.py` & `ensemble_md-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ensemble_md-0.6.0/versioneer.py` & `ensemble_md-0.7.0/versioneer.py`

 * *Files identical despite different names*

