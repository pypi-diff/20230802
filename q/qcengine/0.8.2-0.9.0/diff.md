# Comparing `tmp/qcengine-0.8.2.tar.gz` & `tmp/qcengine-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qcengine-0.8.2.tar", last modified: Thu Jul 25 19:30:35 2019, max compression
+gzip compressed data, was "dist/qcengine-0.9.0.tar", last modified: Thu Aug 15 00:02:02 2019, max compression
```

## Comparing `qcengine-0.8.2.tar` & `qcengine-0.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/
--rw-r--r--   0 levinaden   (501) staff       (20)     3218 2019-07-25 19:30:35.000000 qcengine-0.8.2/PKG-INFO
--rw-r--r--   0 levinaden   (501) staff       (20)     1546 2019-03-18 17:13:40.000000 qcengine-0.8.2/LICENSE
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine.egg-info/
--rw-r--r--   0 levinaden   (501) staff       (20)     3218 2019-07-25 19:30:34.000000 qcengine-0.8.2/qcengine.egg-info/PKG-INFO
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-01-28 16:29:42.000000 qcengine-0.8.2/qcengine.egg-info/not-zip-safe
--rw-r--r--   0 levinaden   (501) staff       (20)     1879 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine.egg-info/SOURCES.txt
--rw-r--r--   0 levinaden   (501) staff       (20)       48 2019-07-25 19:30:34.000000 qcengine-0.8.2/qcengine.egg-info/entry_points.txt
--rw-r--r--   0 levinaden   (501) staff       (20)      159 2019-07-25 19:30:34.000000 qcengine-0.8.2/qcengine.egg-info/requires.txt
--rw-r--r--   0 levinaden   (501) staff       (20)        9 2019-07-25 19:30:34.000000 qcengine-0.8.2/qcengine.egg-info/top_level.txt
--rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-07-25 19:30:34.000000 qcengine-0.8.2/qcengine.egg-info/dependency_links.txt
--rw-r--r--   0 levinaden   (501) staff       (20)      156 2018-08-29 12:25:19.000000 qcengine-0.8.2/MANIFEST.in
--rw-r--r--   0 levinaden   (501) staff       (20)     2096 2019-07-18 20:06:02.000000 qcengine-0.8.2/README.md
--rw-r--r--   0 levinaden   (501) staff       (20)     2177 2019-07-18 20:06:16.000000 qcengine-0.8.2/setup.py
--rw-r--r--   0 levinaden   (501) staff       (20)      474 2019-07-25 19:30:35.000000 qcengine-0.8.2/setup.cfg
--rw-r--r--   0 levinaden   (501) staff       (20)    68611 2018-08-29 12:25:19.000000 qcengine-0.8.2/versioneer.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/procedures/
--rw-r--r--   0 levinaden   (501) staff       (20)     2072 2019-07-22 12:23:14.000000 qcengine-0.8.2/qcengine/procedures/geometric.py
--rw-r--r--   0 levinaden   (501) staff       (20)      100 2019-03-07 19:16:16.000000 qcengine-0.8.2/qcengine/procedures/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1573 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/procedures/model.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1448 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/procedures/base.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1341 2019-03-18 17:13:40.000000 qcengine-0.8.2/qcengine/extras.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6967 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/config.py
--rw-r--r--   0 levinaden   (501) staff       (20)      137 2019-03-07 19:16:16.000000 qcengine-0.8.2/qcengine/units.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1725 2019-03-07 19:16:16.000000 qcengine-0.8.2/qcengine/stock_mols.py
--rw-r--r--   0 levinaden   (501) staff       (20)      498 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/_version.py
--rw-r--r--   0 levinaden   (501) staff       (20)    17061 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/util.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)     5946 2019-07-22 12:23:14.000000 qcengine-0.8.2/qcengine/tests/test_procedures.py
--rw-r--r--   0 levinaden   (501) staff       (20)       63 2018-08-29 12:25:19.000000 qcengine-0.8.2/qcengine/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1920 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/tests/test_standard_suite.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1247 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/tests/test_program_utils.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4875 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/tests/test_config.py
--rw-r--r--   0 levinaden   (501) staff       (20)      567 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/
--rw-r--r--   0 levinaden   (501) staff       (20)    14754 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/molpro.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/gamess/
--rw-r--r--   0 levinaden   (501) staff       (20)     6409 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/gamess/runner.py
--rw-r--r--   0 levinaden   (501) staff       (20)      105 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/programs/gamess/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     9969 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/programs/gamess/harvester.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5774 2019-07-22 12:23:14.000000 qcengine-0.8.2/qcengine/programs/psi4.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/util/
--rw-r--r--   0 levinaden   (501) staff       (20)       70 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/programs/util/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1203 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/programs/util/hessparse.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4811 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/programs/util/pdict.py
--rw-r--r--   0 levinaden   (501) staff       (20)     8303 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/entos.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/nwchem/
--rw-r--r--   0 levinaden   (501) staff       (20)     4980 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/nwchem/runner.py
--rw-r--r--   0 levinaden   (501) staff       (20)       34 2019-07-15 18:42:58.000000 qcengine-0.8.2/qcengine/programs/nwchem/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    32855 2019-07-15 18:42:58.000000 qcengine-0.8.2/qcengine/programs/nwchem/harvester.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/tests/
--rw-r--r--   0 levinaden   (501) staff       (20)        0 2019-06-18 13:15:03.000000 qcengine-0.8.2/qcengine/programs/tests/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    45023 2019-07-15 18:42:58.000000 qcengine-0.8.2/qcengine/programs/tests/test_dftd3_mp2d.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2008 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/tests/test_molpro.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2360 2019-06-07 14:27:34.000000 qcengine-0.8.2/qcengine/programs/tests/test_entos.py
--rw-r--r--   0 levinaden   (501) staff       (20)     6423 2019-07-22 12:23:14.000000 qcengine-0.8.2/qcengine/programs/tests/test_programs.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2050 2019-06-04 00:00:20.000000 qcengine-0.8.2/qcengine/programs/tests/test_terachem.py
--rw-r--r--   0 levinaden   (501) staff       (20)      146 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/__init__.py
-drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-07-25 19:30:35.000000 qcengine-0.8.2/qcengine/programs/cfour/
--rw-r--r--   0 levinaden   (501) staff       (20)     4627 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/cfour/runner.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1825 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/programs/cfour/keywords.py
--rw-r--r--   0 levinaden   (501) staff       (20)       33 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/programs/cfour/__init__.py
--rw-r--r--   0 levinaden   (501) staff       (20)    33722 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/programs/cfour/harvester.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4005 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/torchani.py
--rw-r--r--   0 levinaden   (501) staff       (20)    57935 2019-06-17 16:16:13.000000 qcengine-0.8.2/qcengine/programs/empirical_dispersion_resources.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2034 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/model.py
--rw-r--r--   0 levinaden   (501) staff       (20)     8189 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/terachem.py
--rw-r--r--   0 levinaden   (501) staff       (20)    14357 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/dftd3.py
--rw-r--r--   0 levinaden   (501) staff       (20)     3913 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/rdkit.py
--rw-r--r--   0 levinaden   (501) staff       (20)     8625 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/mopac.py
--rw-r--r--   0 levinaden   (501) staff       (20)     2627 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/base.py
--rw-r--r--   0 levinaden   (501) staff       (20)     8961 2019-07-18 20:06:16.000000 qcengine-0.8.2/qcengine/programs/mp2d.py
--rw-r--r--   0 levinaden   (501) staff       (20)      668 2019-01-28 16:29:34.000000 qcengine-0.8.2/qcengine/cli.py
--rw-r--r--   0 levinaden   (501) staff       (20)     1678 2019-06-04 00:00:19.000000 qcengine-0.8.2/qcengine/exceptions.py
--rw-r--r--   0 levinaden   (501) staff       (20)     5673 2019-07-22 12:23:14.000000 qcengine-0.8.2/qcengine/testing.py
--rw-r--r--   0 levinaden   (501) staff       (20)     4747 2019-07-25 19:30:03.000000 qcengine-0.8.2/qcengine/compute.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/
+-rw-r--r--   0 levinaden   (501) staff       (20)     3218 2019-08-15 00:02:02.000000 qcengine-0.9.0/PKG-INFO
+-rw-r--r--   0 levinaden   (501) staff       (20)     1546 2019-03-18 17:13:40.000000 qcengine-0.9.0/LICENSE
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine.egg-info/
+-rw-r--r--   0 levinaden   (501) staff       (20)     3218 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/PKG-INFO
+-rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-01-28 16:29:42.000000 qcengine-0.9.0/qcengine.egg-info/not-zip-safe
+-rw-r--r--   0 levinaden   (501) staff       (20)     1879 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/SOURCES.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)       48 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/entry_points.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)      159 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/requires.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)        9 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/top_level.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)        1 2019-08-15 00:02:01.000000 qcengine-0.9.0/qcengine.egg-info/dependency_links.txt
+-rw-r--r--   0 levinaden   (501) staff       (20)      156 2018-08-29 12:25:19.000000 qcengine-0.9.0/MANIFEST.in
+-rw-r--r--   0 levinaden   (501) staff       (20)     2096 2019-07-18 20:06:02.000000 qcengine-0.9.0/README.md
+-rw-r--r--   0 levinaden   (501) staff       (20)     2177 2019-08-14 23:02:21.000000 qcengine-0.9.0/setup.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      474 2019-08-15 00:02:02.000000 qcengine-0.9.0/setup.cfg
+-rw-r--r--   0 levinaden   (501) staff       (20)    68611 2018-08-29 12:25:19.000000 qcengine-0.9.0/versioneer.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/procedures/
+-rw-r--r--   0 levinaden   (501) staff       (20)     2030 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/procedures/geometric.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      100 2019-03-07 19:16:16.000000 qcengine-0.9.0/qcengine/procedures/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1573 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/procedures/model.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1448 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/procedures/base.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1341 2019-03-18 17:13:40.000000 qcengine-0.9.0/qcengine/extras.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6967 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/config.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      137 2019-03-07 19:16:16.000000 qcengine-0.9.0/qcengine/units.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1725 2019-03-07 19:16:16.000000 qcengine-0.9.0/qcengine/stock_mols.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      498 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/_version.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    18201 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/util.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/tests/
+-rw-r--r--   0 levinaden   (501) staff       (20)     6166 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/tests/test_procedures.py
+-rw-r--r--   0 levinaden   (501) staff       (20)       63 2018-08-29 12:25:19.000000 qcengine-0.9.0/qcengine/tests/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2345 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/tests/test_standard_suite.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1248 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/tests/test_program_utils.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4880 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/tests/test_config.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      567 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/__init__.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/
+-rw-r--r--   0 levinaden   (501) staff       (20)    17819 2019-08-14 16:18:14.000000 qcengine-0.9.0/qcengine/programs/molpro.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/gamess/
+-rw-r--r--   0 levinaden   (501) staff       (20)     6285 2019-08-14 16:18:14.000000 qcengine-0.9.0/qcengine/programs/gamess/runner.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      105 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/programs/gamess/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    11537 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/programs/gamess/harvester.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5784 2019-08-14 23:02:21.000000 qcengine-0.9.0/qcengine/programs/psi4.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/util/
+-rw-r--r--   0 levinaden   (501) staff       (20)       70 2019-06-04 00:00:20.000000 qcengine-0.9.0/qcengine/programs/util/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1203 2019-06-04 00:00:20.000000 qcengine-0.9.0/qcengine/programs/util/hessparse.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4811 2019-06-04 00:00:20.000000 qcengine-0.9.0/qcengine/programs/util/pdict.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8303 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/entos.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/nwchem/
+-rw-r--r--   0 levinaden   (501) staff       (20)     4980 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/nwchem/runner.py
+-rw-r--r--   0 levinaden   (501) staff       (20)       34 2019-07-15 18:42:58.000000 qcengine-0.9.0/qcengine/programs/nwchem/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    32825 2019-08-14 16:18:14.000000 qcengine-0.9.0/qcengine/programs/nwchem/harvester.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/tests/
+-rw-r--r--   0 levinaden   (501) staff       (20)        0 2019-06-18 13:15:03.000000 qcengine-0.9.0/qcengine/programs/tests/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    45023 2019-07-15 18:42:58.000000 qcengine-0.9.0/qcengine/programs/tests/test_dftd3_mp2d.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2008 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/tests/test_molpro.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2360 2019-06-07 14:27:34.000000 qcengine-0.9.0/qcengine/programs/tests/test_entos.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     6423 2019-07-22 12:23:14.000000 qcengine-0.9.0/qcengine/programs/tests/test_programs.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2050 2019-06-04 00:00:20.000000 qcengine-0.9.0/qcengine/programs/tests/test_terachem.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      146 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/__init__.py
+drwxr-xr-x   0 levinaden   (501) staff       (20)        0 2019-08-15 00:02:02.000000 qcengine-0.9.0/qcengine/programs/cfour/
+-rw-r--r--   0 levinaden   (501) staff       (20)     4627 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/cfour/runner.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1825 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/programs/cfour/keywords.py
+-rw-r--r--   0 levinaden   (501) staff       (20)       33 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/programs/cfour/__init__.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    33722 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/programs/cfour/harvester.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     4005 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/torchani.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    57922 2019-08-14 16:18:14.000000 qcengine-0.9.0/qcengine/programs/empirical_dispersion_resources.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2034 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/model.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8189 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/terachem.py
+-rw-r--r--   0 levinaden   (501) staff       (20)    14390 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/programs/dftd3.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     3913 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/rdkit.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8631 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/programs/mopac.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     2627 2019-07-18 20:06:16.000000 qcengine-0.9.0/qcengine/programs/base.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     8994 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/programs/mp2d.py
+-rw-r--r--   0 levinaden   (501) staff       (20)      668 2019-01-28 16:29:34.000000 qcengine-0.9.0/qcengine/cli.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     1678 2019-06-04 00:00:19.000000 qcengine-0.9.0/qcengine/exceptions.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5204 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/testing.py
+-rw-r--r--   0 levinaden   (501) staff       (20)     5040 2019-08-07 13:30:27.000000 qcengine-0.9.0/qcengine/compute.py
```

### Comparing `qcengine-0.8.2/PKG-INFO` & `qcengine-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcengine
-Version: 0.8.2
+Version: 0.9.0
 Summary: A compute wrapper for Quantum Chemistry.
 Home-page: https://github.com/MolSSI/QCEngine
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: QCEngine
         ========
```

### Comparing `qcengine-0.8.2/LICENSE` & `qcengine-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine.egg-info/PKG-INFO` & `qcengine-0.9.0/qcengine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcengine
-Version: 0.8.2
+Version: 0.9.0
 Summary: A compute wrapper for Quantum Chemistry.
 Home-page: https://github.com/MolSSI/QCEngine
 Author: The QCArchive Development Team
 Author-email: qcarchive@molssi.org
 License: BSD-3C
 Description: QCEngine
         ========
```

### Comparing `qcengine-0.8.2/qcengine.egg-info/SOURCES.txt` & `qcengine-0.9.0/qcengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/README.md` & `qcengine-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/setup.py` & `qcengine-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         cmdclass=versioneer.get_cmdclass(),
         packages=setuptools.find_packages(),
         setup_requires=[] + pytest_runner,
         install_requires=[
             'pyyaml',
             'py-cpuinfo',
             'psutil',
-            'qcelemental>=0.4.2',
+            'qcelemental>=0.6.0',
             'pydantic>=0.30.1'
         ],
         entry_points={"console_scripts": [
             "qcengine=qcengine.cli:main",
         ]},
         extras_require={
             'docs': [
```

### Comparing `qcengine-0.8.2/versioneer.py` & `qcengine-0.9.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/procedures/geometric.py` & `qcengine-0.9.0/qcengine/procedures/geometric.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,16 @@
         try:
             import geometric
         except ModuleNotFoundError:
             raise ModuleNotFoundError("Could not find geomeTRIC in the Python path.")
 
         geometric_input = input_data.dict()
 
-        # Older QCElemental compat, can be removed in v0.6
-        if "extras" not in geometric_input["input_specification"]:
-            geometric_input["input_specification"]["extras"] = {}
+        # Temporary patch for geomeTRIC
+        geometric_input["initial_molecule"]["symbols"] = list(geometric_input["initial_molecule"]["symbols"])
 
         # Set retries to two if zero while respecting local_config
         local_config = config.dict()
         local_config["retries"] = local_config.get("retries", 2) or 2
         geometric_input["input_specification"]["extras"]["_qcengine_local_config"] = local_config
 
         # Run the program
```

### Comparing `qcengine-0.8.2/qcengine/procedures/model.py` & `qcengine-0.9.0/qcengine/procedures/model.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/procedures/base.py` & `qcengine-0.9.0/qcengine/procedures/base.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/extras.py` & `qcengine-0.9.0/qcengine/extras.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/config.py` & `qcengine-0.9.0/qcengine/config.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/stock_mols.py` & `qcengine-0.9.0/qcengine/stock_mols.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/util.py` & `qcengine-0.9.0/qcengine/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -262,14 +262,52 @@
             terminate_process(ret["proc"])
         finally:
             output, error = ret["proc"].communicate()
             ret["stdout"] = output.decode()
             ret["stderr"] = error.decode()
 
 
+@contextmanager
+def environ_context(config: Optional['JobConfig'] = None, env: Optional[Dict[str, str]] = None) -> Dict[str, str]:
+    """Temporarily set environment variables inside the context manager and
+    fully restore previous environment afterwards.
+
+    Parameters
+    ----------
+    config : Optional[JobConfig], optional
+        Automatically sets MKL/OMP num threads based off the input config.
+    env : Optional[Dict[str, str]], optional
+        A dictionary of environment variables to update.
+
+    Yields
+    ------
+    Dict[str, str]
+        The updated environment variables.
+    """
+
+    temporary_env = {}
+    if config:
+        temporary_env["OMP_NUM_THREADS"] = str(config.ncores)
+        temporary_env["MKL_NUM_THREADS"] = str(config.ncores)
+
+    if env:
+        temporary_env.update(env)
+
+    original_env = {key: os.getenv(key) for key in temporary_env}
+    os.environ.update(temporary_env)
+    try:
+        yield temporary_env
+    finally:
+        for key, value in original_env.items():
+            if value is None:
+                del os.environ[key]
+            else:
+                os.environ[key] = value
+
+
 def execute(command: List[str],
             infiles: Optional[Dict[str, str]] = None,
             outfiles: Optional[List[str]] = None,
             *,
             as_binary: Optional[List[str]] = None,
             scratch_name: Optional[str] = None,
             scratch_directory: Optional[str] = None,
```

### Comparing `qcengine-0.8.2/qcengine/tests/test_procedures.py` & `qcengine-0.9.0/qcengine/tests/test_procedures.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Tests the DQM compute dispatch module
 """
 
 import copy
 
 import numpy as np
 import pytest
-from qcelemental.models import OptimizationInput
 
 import qcengine as qcng
+from qcelemental.models import OptimizationInput
 from qcengine import testing
 from qcengine.testing import failure_engine
 
 _base_json = {
     "schema_name": "qcschema_optimization_input",
     "schema_version": 1,
     "keywords": {
@@ -158,18 +158,22 @@
 ]) # yapf: disable
 def test_geometric_generic(program, model, bench):
     inp = copy.deepcopy(_base_json)
 
     inp["initial_molecule"] = qcng.get_molecule("water")
     inp["input_specification"]["model"] = model
     inp["keywords"]["program"] = program
+    inp["input_specification"]["extras"] = {"_secret_tags": {"mysecret_tag": "data1"}}
 
     ret = qcng.compute_procedure(inp, "geometric", raise_error=True)
     assert ret.success is True
     assert "Converged!" in ret.stdout
 
     r01, r02, r12, a102 = ret.final_molecule.measure([[0, 1], [0, 2], [1, 2], [1, 0, 2]])
 
     assert pytest.approx(r01, 1.e-4) == bench[0]
     assert pytest.approx(r02, 1.e-4) == bench[0]
     assert pytest.approx(r12, 1.e-4) == bench[1]
     assert pytest.approx(a102, 1.e-4) == bench[2]
+
+    assert "_secret_tags" in ret.trajectory[0].extras
+    assert "data1" == ret.trajectory[0].extras["_secret_tags"]["mysecret_tag"]
```

### Comparing `qcengine-0.8.2/qcengine/tests/test_standard_suite.py` & `qcengine-0.9.0/qcengine/tests/test_standard_suite.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 """
 Tests the DQM compute dispatch module
 """
 
 import copy
 
+import numpy as np
 import pytest
-from qcelemental.models import Molecule, ResultInput
 
 import qcengine as qcng
+from qcelemental.models import Molecule, ResultInput
 from qcengine import testing
 
 _canonical_methods = [
     ("dftd3", {"method": "b3lyp-d3"}),
+    ("mopac", {"method": "PM6"}),
+    ("mp2d", {"method": "MP2-DMP2"}),
     ("psi4", {"method": "hf", "basis": "6-31G"}),
     ("rdkit", {"method": "UFF"}),
     ("torchani", {"method": "ANI1x"}),
-]
+] # yapf: disable
 
 @pytest.mark.parametrize("program, model", _canonical_methods)
 def test_compute_energy(program, model):
     if not testing.has_program(program):
         pytest.skip("Program '{}' not found.".format(program))
 
-
     inp = ResultInput(molecule=qcng.get_molecule("hydrogen"), driver="energy", model=model)
     ret = qcng.compute(inp, program, raise_error=True)
 
     assert ret.success is True
     assert isinstance(ret.return_result, float)
 
 
 @pytest.mark.parametrize("program, model", _canonical_methods)
 def test_compute_gradient(program, model):
     if not testing.has_program(program):
         pytest.skip("Program '{}' not found.".format(program))
 
-    inp = ResultInput(molecule=qcng.get_molecule("hydrogen"), driver="gradient", model=model)
+    inp = ResultInput(molecule=qcng.get_molecule("hydrogen"),
+                      driver="gradient",
+                      model=model,
+                      extras={"mytag": "something"})
     ret = qcng.compute(inp, program, raise_error=True)
 
     assert ret.success is True
-    assert isinstance(ret.return_result, list)
+    assert isinstance(ret.return_result, np.ndarray)
+    assert len(ret.return_result.shape) == 2
+    assert ret.return_result.shape[1] == 3
+    assert "mytag" in ret.extras, ret.extras
 
 
 @pytest.mark.parametrize("program, model", [
     ("dftd3", {"method": "bad"}),
+    ("dftd3", {"method": "b3lyp-d3", "driver": "hessian"}),
+    ("mopac", {"method": "bad"}),
+    ("mp2d", {"method": "bad"}),
     ("psi4", {"method": "bad"}),
     ("rdkit", {"method": "bad"}),
     ("torchani", {"method": "bad"}),
-    ("dftd3", {"method": "b3lyp-d3", "driver": "hessian"}),
-])
+]) # yapf: disable
 def test_compute_bad_models(program, model):
     if not testing.has_program(program):
         pytest.skip("Program '{}' not found.".format(program))
 
     adriver = model.pop("driver", "energy")
     amodel = model
     inp = ResultInput(molecule=qcng.get_molecule("hydrogen"), driver=adriver, model=amodel)
```

### Comparing `qcengine-0.8.2/qcengine/tests/test_program_utils.py` & `qcengine-0.9.0/qcengine/tests/test_program_utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,8 @@
 
 
 def test_procedure_avail_bounce():
 
     with pytest.raises(qcng.exceptions.InputError) as exc:
         qcng.compute_procedure({}, "bad_program", raise_error=True)
 
-    assert "not registered" in str(exc.value)
+    assert "not registered" in str(exc.value)
```

### Comparing `qcengine-0.8.2/qcengine/tests/test_config.py` & `qcengine-0.9.0/qcengine/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import copy
 import os
 
 import pydantic
 import pytest
 
 import qcengine as qcng
-from qcengine.testing import environ_context
+from qcengine.util import environ_context
 
 
 def test_node_blank():
     node = qcng.config.NodeDescriptor(name="something", hostname_pattern="*")
 
 
 def test_node_auto():
@@ -37,15 +37,15 @@
     assert job2.ncores == 2
     assert pytest.approx(job2.memory) == 5.0
 
 
 def test_node_environ():
 
     scratch_name = "myscratch1234"
-    with environ_context({"QCA_SCRATCH_DIR": scratch_name}):
+    with environ_context(env={"QCA_SCRATCH_DIR": scratch_name}):
         description = {
             "name": "something",
             "hostname_pattern": "*",
             "scratch_directory": "$QCA_SCRATCH_DIR",
         }
 
         node = qcng.config.NodeDescriptor(**description)
@@ -69,15 +69,15 @@
     Capture the options state and temporarily override.
     """
 
     # Snapshot env
     old_node = copy.deepcopy(qcng.config.NODE_DESCRIPTORS)
 
     scratch_name = "myscratch1234"
-    with environ_context({"QCA_SCRATCH_DIR": scratch_name}):
+    with environ_context(env={"QCA_SCRATCH_DIR": scratch_name}):
 
         configs = [{
             "name": "dragonstooth",
             "hostname_pattern": "dt*",
             "jobs_per_node": 2,
             "ncores": 12,
             "memory": 120,
```

### Comparing `qcengine-0.8.2/qcengine/__init__.py` & `qcengine-0.9.0/qcengine/__init__.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/molpro.py` & `qcengine-0.9.0/qcengine/programs/molpro.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Calls the Molpro executable.
 """
 
 import string
 import xml.etree.ElementTree as ET
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Set, Tuple, Optional
 
 from qcelemental.models import Result
 from qcelemental.util import parse_version, safe_version, which
 
 from ..exceptions import InputError, UnknownError
 from ..util import execute
 from .model import ProgramHarness
@@ -21,14 +21,42 @@
         "thread_safe": False,
         "thread_parallel": True,
         "node_parallel": False,
         "managed_memory": True,
     }
     version_cache: Dict[str, str] = {}
 
+    # Set of implemented dft functionals in Molpro according to dfunc.registry (version 2019.2)
+    _dft_functionals: Set[str] = {
+        "B86MGC", "B86R", "B86", "B88C", "B88", "B95", "B97DF", "B97RDF", "BR", "BRUEG", "BW", "CS1", "CS2",
+        "DIRAC", "ECERFPBE", "ECERF", "EXACT", "EXERFPBE", "EXERF", "G96", "HCTH120", "HCTH147",
+        "HCTH93", "HJSWPBEX", "LTA", "LYP", "M052XC", "M052XX", "M05C", "M05X", "M062XC",
+        "M062XX", "M06C", "M06HFC", "M06HFX", "M06LC", "M06LX", "M06X", "M12C", "MK00B", "MK00",
+        "P86", "PBEC", "PBESOLC", "PBESOLX", "PBEXREV", "PBEX", "PW86", "PW91C", "PW91X", "PW92C",
+        "STEST", "TFKE", "TH1", "TH2", "TH3", "TH4", "THGFCFO", "THGFCO", "THGFC", "THGFL",
+        "TPSSC", "TPSSX", "VSXC", "VW", "VWN3", "VWN5", "XC-M05-2X", "XC-M05", "XC-M06-2X",
+        "XC-M06-HF", "XC-M06-L", "XC-M06", "XC-M08-HX", "XC-M08-SO", "XC-M11-L", "XC-SOGGA11",
+        "XC-SOGGA11-X", "XC-SOGGA", "FRMTST", "LHF", "TLHF", "LXBECKE", "ELP", "NULL", "YTEST",
+        "TREF2", "TREF", "TTEST", "GLE", "GREEN", "SRB88", "SRLYP", "LB94", "EI", "SAOP", "USER",
+        "INE", "ECERF2", "ECERFINTER", "ECERFLOCAL2", "ECERFLOCAL", "EXERFLOCAL", "FC", "FCFO",
+        "FCO", "FL", "XC-M11", "PBEXANAL", "PBECANAL", "PBESOLCANAL", "PBESOLXANAL", "EXSRLDA",
+        "EXSRLPBE", "ECSRLPBE", "ECSRLLPBE", "ECSQRTLPBE", "ECMUDIVLPBE", "EXERFPHS", "ECLERFMUPBE",
+        "ECERFERFCPBE", "ECSQRTLDA", "REVPBEX", "B", "B-LYP", "BLYP", "B-P", "BP86", "B-VWN", "B3LYP",
+        "B3LYP3", "B3LYP5", "B88X", "B97", "B97R", "BECKE", "BH-LYP", "CS", "D", "HFB", "HFS", "LDA",
+        "LSDAC", "LSDC", "KYP88", "MM05", "MM05-2X", "MM06", "MM06-2X", "MM06-L", "MM06-HF", "PBE", "PBE0",
+        "PBE0MOL", "PBEREV", "PW91", "S", "S-VWN", "SLATER", "VS99", "VWN", "VWN80", 'M05',
+        "M05-2X", "M06", "M06-2X", "M06-L", "M06-HF", "M08-HX","M08-SO", "M11-L", "TPSS",
+        "TPSSH", "M12HFC", "HJSWPBE", "HJSWPBEH", "TCSWPBE", "PBESOL"
+    }
+
+    # Currently supported methods in QCEngine for Molpro
+    _scf_methods: Set[str] = {"HF", "RHF", "KS", "RKS"}
+    _post_hf_methods: Set[str] = {'MP2', 'CCSD', 'CCSD(T)'}
+    _supported_methods: Set[str] = {*_scf_methods, *_post_hf_methods}
+
     class Config(ProgramHarness.Config):
         pass
 
     def found(self, raise_error: bool = False) -> bool:
         return which('molpro',
                      return_bool=True,
                      raise_error=raise_error,
@@ -68,64 +96,70 @@
 
         # Setup the job
         job_inputs = self.build_input(input_data, config)
 
         # Run Molpro
         proc = self.execute(job_inputs)
 
+        # Return proc if it is type UnknownError for error propagation otherwise process the output
         if isinstance(proc, UnknownError):
             return proc
         else:
             # If execution succeeded, collect results
             result = self.parse_output(proc["outfiles"], input_data)
             return result
 
     def execute(self,
-                inputs,
-                extra_infiles=None,
-                extra_outfiles=None,
-                extra_commands=None,
-                scratch_name=None,
-                scratch_messy=False,
-                timeout=None):
+                inputs: Dict[str, Any],
+                extra_infiles: Optional[List[str]] = None,
+                extra_outfiles: Optional[List[str]] = None,
+                as_binary: Optional[List[str]] = None,
+                extra_commands: bool = None,
+                scratch_name: Optional[str] = None,
+                scratch_messy: bool = False,
+                timeout: Optional[int] = None) -> Tuple[bool, Dict[str, Any]]:
         """
         For option documentation go look at qcengine/util.execute
         """
 
+        # Collect all input files and update with extra_infiles
         infiles = inputs["infiles"]
         if extra_infiles is not None:
             infiles.update(extra_infiles)
 
+        # Collect all output files and update with extra_outfiles
         outfiles = ["dispatch.out", "dispatch.xml", "dispatch.wfu"]
         if extra_outfiles is not None:
             outfiles.extend(extra_outfiles)
 
+        # Replace commands with extra_commands if present
         commands = inputs["commands"]
         if extra_commands is not None:
             commands = extra_commands
 
+        # Run the Molpro program
         exe_success, proc = execute(commands,
                                     infiles=infiles,
                                     outfiles=outfiles,
-                                    scratch_directory=inputs["scratch_directory"],
+                                    as_binary=as_binary,
                                     scratch_name=scratch_name,
+                                    scratch_directory=inputs["scratch_directory"],
                                     scratch_messy=scratch_messy,
                                     timeout=timeout)
 
         # Determine whether the calculation succeeded
         if not exe_success:
             return UnknownError(proc["stderr"])
 
         return proc
 
     def build_input(self, input_model: 'ResultInput', config: 'JobConfig',
                     template: Optional[str] = None) -> Dict[str, Any]:
         if template is None:
             input_file = []
-            posthf_methods = {'mp2', 'ccsd', 'ccsd(t)'}
 
             # Memory is in megawords per core for Molpro
             memory_mw_core = int(config.memory * (1024**3) / 8e6 / config.ncores)
             input_file.append("memory,{},M".format(memory_mw_core))
             # TODO Decide how I want this keyword to look/work
             # if input_model.keywords.get('wfu') is not None:
             #     input_file.append('file,2,{}'.format(input_model.keywords.get('wfu')))
@@ -133,36 +167,38 @@
 
             # Write the geom
             xyz_block = input_model.molecule.to_string(dtype='molpro', units='Bohr')
             input_file.append(xyz_block)
 
             # Write the basis set
             input_file.append('basis={')
-            input_file.append('default,{}'.format(input_model.model.basis))
+            input_file.append(f'default,{input_model.model.basis}')
             input_file.append('}')
             input_file.append('')
 
-            # Start of Molpro Commands
             # Write energy call
             energy_call = []
-            write_hf = input_model.model.method.lower() in posthf_methods
-            if write_hf:
+            # If post-hf method is called then make sure to write a HF call first
+            if input_model.model.method.upper() in self._post_hf_methods:
                 energy_call.append('{HF}')
-            # TODO Support DFT calls, need to check if method is a DFT XC functional and then write {rks,XC}
-            energy_call.append('{{{:s}}}'.format(input_model.model.method))
+            # If DFT call make sure to write {rks,method}
+            if input_model.model.method.upper() in self._dft_functionals:
+                energy_call.append(f'{{rks,{input_model.model.method}}}')
+            else:
+                energy_call.append(f'{{{input_model.model.method}}}')
 
             # Write appropriate driver call
             if input_model.driver == 'energy':
                 input_file.extend(energy_call)
             elif input_model.driver == 'gradient':
                 input_file.extend(energy_call)
                 input_file.append('')
                 input_file.append('{force}')
             else:
-                raise InputError('Driver {} not implemented for Molpro.'.format(input_model.driver))
+                raise InputError(f'Driver {input_model.driver} not implemented for Molpro.')
 
             input_file = "\n".join(input_file)
         else:
             # Some of the potential different template options
             # (A) ordinary build_input (need to define a base template)
             # (B) user wants to add stuff after normal template (A)
             # (C) user knows their domain language (doesn't use any QCSchema quantities)
@@ -197,84 +233,95 @@
         #      - cml:molecule, cml:atomArray (?)
         #      - basisSet
         #      - orbitals
         output_data = {}
         properties = {}
         name_space = {'molpro_uri': 'http://www.molpro.net/schema/molpro-output'}
 
-        # SCF maps
-        scf_energy_map = {"Energy": "scf_total_energy"}
-        scf_dipole_map = {"Dipole moment": "scf_dipole_moment"}
-        scf_extras = {}
-
-        # MP2 maps
-        mp2_energy_map = {"total energy": "mp2_total_energy", "correlation energy": "mp2_correlation_energy"}
-        mp2_dipole_map = {"Dipole moment": "mp2_dipole_moment"}
-        mp2_extras = {
-            "singlet pair energy": "mp2_singlet_pair_energy",
-            "triplet pair energy": "mp2_triplet_pair_energy"
-        }
-
-        # CCSD maps
-        ccsd_energy_map = {"total energy": "ccsd_total_energy", "correlation energy": "ccsd_correlation_energy"}
-        ccsd_dipole_map = {"Dipole moment": "ccsd_dipole_moment"}
-        ccsd_extras = {
-            "singlet pair energy": "ccsd_singlet_pair_energy",
-            "triplet pair energy": "ccsd_triplet_pair_energy"
-        }
-
-        # CCSD(T) maps
-        # TODO There are two instances of "correlation energy" in the xml. One for CCSD and one for CCSD(T)
-        #      Will need a bit more logic to separate between the two
-        ccsd_prt_pr_energy_map = {
-            "total energy": "ccsd_prt_pr_total_energy",
-            "correlation energy": "ccsd_prt_pr_correlation_energy",
+        # Molpro commands map
+        molpro_map = {
+            "Energy": {
+                "HF": "scf_total_energy",
+                "RHF": "scf_total_energy",
+                "KS": "scf_total_energy",
+                "RKS": "scf_total_energy"
+            },
+            "total energy": {
+                "MP2": "mp2_total_energy",
+                "CCSD": "ccsd_total_energy",
+                "CCSD(T)": "ccsd_prt_pr_total_energy"
+            },
+            "correlation energy": {
+                "MP2": "mp2_correlation_energy",
+                "CCSD": "ccsd_correlation_energy",
+                "CCSD(T)": "ccsd_prt_pr_correlation_energy",  # Need both CCSD(T) and Total
+                "Total": "ccsd_prt_pr_correlation_energy"  # Total corresponds to CCSD(T) correlation energy
+            },
+            "singlet pair energy": {
+                "MP2": "mp2_singlet_pair_energy",
+                "CCSD": "ccsd_singlet_pair_energy"
+            },
+            "triplet pair energy": {
+                "MP2": "mp2_triplet_pair_energy",
+                "CCSD": "ccsd_triplet_pair_energy"
+            },
+            "Dipole moment": {
+                "HF": "scf_dipole_moment",
+                "RHF": "scf_dipole_moment",
+                "KS": "scf_dipole_moment",
+                "RKS": "scf_dipole_moment",
+                "MP2": "mp2_dipole_moment",
+                "CCSD": "ccsd_dipole_moment",
+                "CCSD(T)": "ccsd_prt_pr_dipole_moment"
+            }
         }
-        ccsd_prt_pr_dipole_map = {"Dipole moment": "ccsd_prt_pr_dipole_moment"}
-        ccsd_prt_pr_extras = {**ccsd_extras, "contribution": "prt_pr_contribution"}
 
-        # Compiling the method maps
-        scf_maps = {"energy": scf_energy_map, "dipole": scf_dipole_map, "extras": scf_extras}
-        mp2_maps = {"energy": mp2_energy_map, "dipole": mp2_dipole_map, "extras": mp2_extras}
-        ccsd_maps = {"energy": ccsd_energy_map, "dipole": ccsd_dipole_map, "extras": ccsd_extras}
-        ccsd_prt_pr_maps = {
-            "energy": ccsd_prt_pr_energy_map,
-            "dipole": ccsd_prt_pr_dipole_map,
-            "extras": ccsd_prt_pr_extras
+        # Molpro variables map used for quantities not found in the command map
+        molpro_var_map = {
+            "_ENUC": "nuclear_repulsion_energy",
+            "_DFTFUN": "scf_xc_energy"
+            # "_EMP2_SCS": "scs_mp2_total_energy"
         }
-        scf_methods = {"HF": scf_maps, "RHF": scf_maps}  # , "RKS": scf_maps}
-        post_hf_methods = {"MP2": mp2_maps, "CCSD": ccsd_maps}  # , "CCSD(T)": ccsd_prt_pr_maps}
-        supported_methods = {**scf_methods, **post_hf_methods}
 
+        # Loop through each jobstep
         # The jobstep tag in Molpro contains output from commands (e.g. {hf}, {force})
         for jobstep in root.findall('molpro_uri:job/molpro_uri:jobstep', name_space):
-
             # Remove the -SCF part of the command string when Molpro calls HF or KS
             command = jobstep.attrib['command']
             if '-SCF' in command:
                 command = command[:-4]
-
             # Grab energies and dipole moment
-            if command in supported_methods:
-                command_map = supported_methods[command]
+            if command in self._supported_methods:
                 for child in jobstep.findall('molpro_uri:property', name_space):
-                    if child.attrib['name'] in command_map['energy']:
-                        properties[command_map['energy'][child.attrib['name']]] = float(child.attrib['value'])
-                    elif child.attrib['name'] in command_map['extras']:
-                        properties[command_map['extras'][child.attrib['name']]] = float(child.attrib['value'])
-                    elif child.attrib['name'] in command_map['dipole']:
-                        properties[command_map['dipole'][child.attrib['name']]] = [
-                            float(x) for x in child.attrib['value'].split()
-                        ]
+                    prop_name = child.attrib['name']
+                    prop_method = child.attrib['method']
+                    value = child.attrib['value']
+                    if prop_name in molpro_map:
+                        if prop_method in molpro_map[prop_name]:
+                            if prop_name == "Dipole moment":
+                                properties[molpro_map[prop_name][prop_method]] = [float(x) for x in value.split()]
+                            else:
+                                properties[molpro_map[prop_name][prop_method]] = float(value)
             # Grab gradient
-            elif 'FORCE' in jobstep.attrib['command']:
+            elif 'FORCE' in command:
                 for child in jobstep.findall('molpro_uri:gradient', name_space):
                     # Stores gradient as a single list where the ordering is [1x, 1y, 1z, 2x, 2y, 2z, ...]
                     output_data['return_result'] = [float(x) for x in child.text.split()]
 
+        # Look for final energy in the molecule tag in case it's needed
+        # Note: For the DFT case mol_method is the name of the functional plus R or U in front
+        molecule = root.find('molpro_uri:job/molpro_uri:molecule', name_space)
+        mol_method = molecule.attrib['method']
+        mol_final_energy = float(molecule.attrib['energy'])
+        # Loop over each variable under the variables tag to grab additional info from molpro_var_map
+        for variable in molecule.findall('molpro_uri:variables/molpro_uri:variable', name_space):
+            var_name = variable.attrib['name']
+            if var_name in molpro_var_map:
+                properties[molpro_var_map[var_name]] = float(variable[0].text)
+
         # Convert triplet and singlet pair correlation energies to opposite-spin and same-spin correlation energies
         if 'mp2_singlet_pair_energy' in properties and 'mp2_triplet_pair_energy' in properties:
             properties["mp2_same_spin_correlation_energy"] = (2.0 / 3.0) * properties['mp2_triplet_pair_energy']
             properties["mp2_opposite_spin_correlation_energy"] = (1.0 / 3.0) \
                                                                  * properties['mp2_triplet_pair_energy'] \
                                                                  + properties['mp2_singlet_pair_energy']
             del properties['mp2_singlet_pair_energy']
@@ -284,44 +331,43 @@
             properties["ccsd_same_spin_correlation_energy"] = (2.0 / 3.0) * properties['ccsd_triplet_pair_energy']
             properties["ccsd_opposite_spin_correlation_energy"] = (1.0 / 3.0) \
                                                                   * properties['ccsd_triplet_pair_energy'] \
                                                                   + properties['ccsd_singlet_pair_energy']
             del properties['ccsd_singlet_pair_energy']
             del properties['ccsd_triplet_pair_energy']
 
-        # Look for final energy in the molecule tag in case it's needed
-        molecule = root.find('molpro_uri:job/molpro_uri:molecule', name_space)
-        mol_method = molecule.attrib['method']
-        mol_final_energy = float(molecule.attrib['energy'])
+        # Grab the method from input
+        method = input_model.model.method
+        if method.upper() in self._dft_functionals:  # Determine if method is a DFT functional
+            method = "RKS"
 
         # A slightly more robust way of determining the final energy.
         # Throws an error if the energy isn't found for the method specified from the input_model.
-        # TODO Will need to be modified to work for DFT. XC --> RKS
-        method = input_model.model.method
-        method_energy_map = supported_methods[method]['energy']
-        if method in post_hf_methods and method_energy_map['total energy'] in properties:
-            final_energy = properties[method_energy_map['total energy']]
-        elif method in scf_methods and method_energy_map['Energy'] in properties:
-            final_energy = properties[method_energy_map['Energy']]
+        if method in self._post_hf_methods and molpro_map['total energy'][method] in properties:
+            final_energy = properties[molpro_map['total energy'][method]]
+        elif method in self._scf_methods and molpro_map['Energy'][method] in properties:
+            final_energy = properties[molpro_map['Energy'][method]]
         else:
+            # Back up method for determining final energy if not already present in properties
             # Use the total energy from the molecule tag if it matches the input method
-            if mol_method == method:
+            if input_model.model.method in mol_method:
                 final_energy = mol_final_energy
-                if method in post_hf_methods:
-                    properties[method_energy_map['total energy']] = mol_final_energy
+                if method in self._post_hf_methods:
+                    properties[molpro_map['total energy'][method]] = mol_final_energy
                     properties[
-                        method_energy_map['correlation energy']] = mol_final_energy - properties['scf_total_energy']
-                elif method in scf_methods:
-                    properties[method_energy_map['Energy']] = mol_final_energy
+                        molpro_map['correlation energy'][method]] = mol_final_energy - properties['scf_total_energy']
+                elif method in self._scf_methods:
+                    properties[molpro_map['Energy'][method]] = mol_final_energy
             else:
-                raise KeyError("Could not find {:s} total energy".format(method))
+                raise KeyError(f"Could not find {method} total energy")
 
         # Replace return_result with final_energy if gradient wasn't called
         if "return_result" not in output_data:
             output_data["return_result"] = final_energy
 
+        # Final output_data assignments needed for the Result object
         output_data["properties"] = properties
         output_data['schema_name'] = 'qcschema_output'
         output_data['stdout'] = outfiles["dispatch.out"]
         output_data['success'] = True
 
         return Result(**{**input_model.dict(), **output_data})
```

### Comparing `qcengine-0.8.2/qcengine/programs/gamess/runner.py` & `qcengine-0.9.0/qcengine/programs/gamess/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     def build_input(self, input_model: 'ResultInput', config: 'JobConfig',
                     template: Optional[str] = None) -> Dict[str, Any]:
         pass
 
     def fake_input(self, input_model: 'ResultInput', config: 'JobConfig',
                     template: Optional[str] = None) -> Dict[str, Any]:
 
-# Note decr MEMORY=100000 to get
-# ***** ERROR: MEMORY REQUEST EXCEEDS AVAILABLE MEMORY
-# to test gms fail
+        # Note decr MEMORY=100000 to get
+        # ***** ERROR: MEMORY REQUEST EXCEEDS AVAILABLE MEMORY
+        # to test gms fail
         infile = \
 """ $CONTRL SCFTYP=ROHF MULT=3 RUNTYP=GRADIENT COORD=CART $END
  $SYSTEM TIMLIM=1 MEMORY=800000 $END
  $SCF    DIRSCF=.TRUE. $END
  $BASIS  GBASIS=STO NGAUSS=2 $END
  $GUESS  GUESS=HUCKEL $END
  $DATA
@@ -89,25 +89,23 @@
 Cnv  2
 
 Hydrogen   1.0    0.82884     0.7079   0.0
 Carbon     6.0
 Hydrogen   1.0   -0.82884     0.7079   0.0
  $END
 """
-
         # edits to rungms
         # set SCR=./
         # set USERSCR=./
         # set GMSPATH=/home/psilocaluser/gits/gamess
 
         return {
             "commands": [which("rungms"), "gamess"],  # rungms JOB VERNO NCPUS >& JOB.log &
             "infiles": {
-                #"gamess.inp": infile,
-                "gamess.inp": input_model.extras['gamess.inp'],
+                "gamess.inp": infile
             },
             "scratch_directory": config.scratch_directory,
             "input_result": input_model.copy(deep=True),
         }
 
 
     def execute(self, inputs, extra_outfiles=None, extra_commands=None, scratch_name=None, timeout=None):
@@ -165,14 +163,13 @@
 #            raise ValidationError("""gamess exited abnormally.""")
 #
 #        P4GAMESS_INFO.clear()
 #        P4GAMESS_INFO.update(internal_p4gamess_info)
 #
 #        optstash.restore()
 
-        # TODO Should only return True if Molpro calculation terminated properly
         output_data['success'] = True
 
         return Result(**{**input_model.dict(), **output_data})
 
 #            return Result(**output_data)
 #        return FailedOperation(success=output_data.pop("success", False), error=output_data.pop("error"), input_data=output_data)
```

### Comparing `qcengine-0.8.2/qcengine/programs/gamess/harvester.py` & `qcengine-0.9.0/qcengine/programs/gamess/harvester.py`

 * *Files 8% similar despite different names*

```diff
@@ -94,14 +94,42 @@
             r'^\s+' + r'E\(MP2\)' + r'=\s+' + NUMBER + r'\s*$'
             ,outtext, re.MULTILINE)
         if mobj:
             print('matched mp2')
             qcvar['MP2 CORRELATION ENERGY'] = mobj.group(3)
             qcvar['MP2 TOTAL ENERGY'] = mobj.group(4)
 
+        # Process CCSD
+        mobj = re.search(
+            r'^\s+' + r'SUMMARY OF RESULTS' +
+            r'\s+' + r'\n'+
+            r'^\s+' + r'REFERENCE ENERGY:' + r'\s+' + NUMBER + r'\s*' +
+            r'^\s+' + r'MBPT\(2\) ENERGY:' + r'\s+' + NUMBER + r'\s*' + r'CORR.E=\s+' + r'\s+' + NUMBER + r'\s*'+
+            r'^\s+' + r'CCSD    ENERGY:'   + r'\s+' + NUMBER + r'\s*' + r'CORR.E=\s+' + r'\s+' + NUMBER + r'\s*$',
+            outtext, re.MULTILINE)
+        if mobj:
+            print('matched rhf ccsd')
+            qcvar['SCF TOTAL ENERGY'] = mobj.group(1)
+            qcvar['MP2 CORRELATION ENERGY'] = mobj.group(3)
+            qcvar['MP2 TOTAL ENERGY'] = mobj.group(2)
+            qcvar['CCSD CORRELATION ENERGY'] = mobj.group(5)
+            qcvar['CCSD TOTAL ENERGY'] = mobj.group(4)
+
+        mobj = re.search(
+            r'^\s+' + r'SUMMARY OF CCSD RESULTS' +
+            r'\s+' + r'\n'+
+            r'^\s+' + r'REFERENCE ENERGY:' + r'\s+' + NUMBER + r'\s*' +
+            r'^\s+' + r'CCSD ENERGY:'   + r'\s+' + NUMBER + r'\s*' + r'CORR. E=\s+' + r'\s+' + NUMBER + r'\s*$',
+            outtext, re.MULTILINE)
+        if mobj:
+            print('matched rohf ccsd')
+            qcvar['SCF TOTAL ENERGY'] = mobj.group(1)
+            qcvar['CCSD CORRELATION ENERGY'] = mobj.group(3)
+            qcvar['CCSD TOTAL ENERGY'] = mobj.group(2)
+
         # Process CCSD(T)
         mobj = re.search(
             r'^\s+' + r'SUMMARY OF RESULTS' + 
             r'\s+' + r'\n'+
             r'^\s+' + r'REFERENCE ENERGY:' + r'\s+' + NUMBER + r'\s*' +
             r'^\s+' + r'MBPT\(2\) ENERGY:' + r'\s+' + NUMBER + r'\s*' + r'CORR.E=\s+' + r'\s+' + NUMBER + r'\s*'+
             r'^\s+' + r'CCSD    ENERGY:'   + r'\s+' + NUMBER + r'\s*' + r'CORR.E=\s+' + r'\s+' + NUMBER + r'\s*'+
@@ -204,14 +232,18 @@
         qcvar['CURRENT REFERENCE ENERGY'] = qcvar['HF TOTAL ENERGY']
         qcvar['CURRENT ENERGY'] = qcvar['HF TOTAL ENERGY']
 
     if 'MP2 TOTAL ENERGY' in qcvar and 'MP2 CORRELATION ENERGY' in qcvar:
             qcvar['CURRENT CORRELATION ENERGY'] = qcvar['MP2 CORRELATION ENERGY']
             qcvar['CURRENT ENERGY'] = qcvar['MP2 TOTAL ENERGY']
 
+    if 'CCSD TOTAL ENERGY' in qcvar and 'CCSD CORRELATION ENERGY' in qcvar:
+        qcvar['CURRENT CORRELATION ENERGY'] = qcvar['CCSD CORRELATION ENERGY']
+        qcvar['CURRENT ENERGY'] = qcvar['CCSD TOTAL ENERGY']
+
     if 'CCSD(T) TOTAL ENERGY' in qcvar and 'CCSD(T) CORRELATION ENERGY' in qcvar:
         qcvar['CURRENT CORRELATION ENERGY'] = qcvar['CCSD(T) CORRELATION ENERGY']
         qcvar['CURRENT ENERGY'] = qcvar['CCSD(T) TOTAL ENERGY']
 
     if 'DFT TOTAL ENERGY' in qcvar:
         qcvar['CURRENT REFERENCE ENERGY'] = qcvar['DFT TOTAL ENERGY']
         qcvar['CURRENT ENERGY'] = qcvar['DFT TOTAL ENERGY']
```

### Comparing `qcengine-0.8.2/qcengine/programs/psi4.py` & `qcengine-0.9.0/qcengine/programs/psi4.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         """
         self.found(raise_error=True)
 
         if parse_version(self.get_version()) < parse_version("1.2"):
             raise ResourceError("Psi4 version '{}' not understood.".format(self.get_version()))
 
         # Setup the job
-        input_data = input_model.json_dict()
+        input_data = input_model.dict(encoding="json")
         input_data["nthreads"] = config.ncores
         input_data["memory"] = int(config.memory * 1024 * 1024 * 1024 * 0.95)  # Memory in bytes
         input_data["success"] = False
         input_data["return_output"] = True
 
         if input_data["schema_name"] == "qcschema_input":
             input_data["schema_name"] = "qc_schema_input"
```

### Comparing `qcengine-0.8.2/qcengine/programs/util/hessparse.py` & `qcengine-0.9.0/qcengine/programs/util/hessparse.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/util/pdict.py` & `qcengine-0.9.0/qcengine/programs/util/pdict.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/entos.py` & `qcengine-0.9.0/qcengine/programs/entos.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/nwchem/runner.py` & `qcengine-0.9.0/qcengine/programs/nwchem/runner.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/nwchem/harvester.py` & `qcengine-0.9.0/qcengine/programs/nwchem/harvester.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from decimal import Decimal
 
-import numpy as np
 import qcelemental as qcel
 from qcelemental.models import Molecule
 
-from ..util import load_hessian, PreservingDict
+from ..util import PreservingDict
 
 def harvest_output(outtext):
     """Function to separate portions of a NWChem output file *outtext*,
     divided by " Line search:".
 
     """
     pass_psivar = []
@@ -570,15 +569,15 @@
 
 
 def harvest_hessian(hess):
     """Parses the contents *hessian* of the NWChem hess file into a hessian array.
     Hess file name has to be "nwchem.hess". (default)
 
     """
-    hess = hess.splitlines()
+    raise NotImplementedError()
 
 
 def harvest(p4Mol, nwout, **largs):  #check orientation and scratch files
     """Parses all the pieces of output from NWChem: the stdout in
     *nwout* Scratch files are not yet considered at this moment. 
 
     """
```

### Comparing `qcengine-0.8.2/qcengine/programs/tests/test_dftd3_mp2d.py` & `qcengine-0.9.0/qcengine/programs/tests/test_dftd3_mp2d.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/tests/test_molpro.py` & `qcengine-0.9.0/qcengine/programs/tests/test_molpro.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/tests/test_entos.py` & `qcengine-0.9.0/qcengine/programs/tests/test_entos.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/tests/test_programs.py` & `qcengine-0.9.0/qcengine/programs/tests/test_programs.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/tests/test_terachem.py` & `qcengine-0.9.0/qcengine/programs/tests/test_terachem.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/cfour/runner.py` & `qcengine-0.9.0/qcengine/programs/cfour/runner.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/cfour/keywords.py` & `qcengine-0.9.0/qcengine/programs/cfour/keywords.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/cfour/harvester.py` & `qcengine-0.9.0/qcengine/programs/cfour/harvester.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/torchani.py` & `qcengine-0.9.0/qcengine/programs/torchani.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/empirical_dispersion_resources.py` & `qcengine-0.9.0/qcengine/programs/empirical_dispersion_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,16 +553,15 @@
 
     if dashlevel_candidate_1 is None and dashlevel_candidate_2 is None:
         raise InputError(
             f"""Can't guess -D correction level from name_hint ({name_hint}) and level_hint ({level_hint})""")
     elif dashlevel_candidate_1 is not None and dashlevel_candidate_2 is not None:
         if dashlevel_candidate_1 != dashlevel_candidate_2:
             raise InputError(
-                f"""Inconsistent -D correction level ({dashlevel_candidate_2} != {dashlevel_candidate_1}) from name_hint ({name_hint}) and level_hint ({level_hint})"""
-            )
+                f"""Inconsistent -D correction level ({dashlevel_candidate_2} != {dashlevel_candidate_1}) from name_hint ({name_hint}) and level_hint ({level_hint})""")
     dashleveleff = dashlevel_candidate_1 or dashlevel_candidate_2
 
     allowed_params = dashcoeff[dashleveleff]['default'].keys()
 
     # << 2 >> use name_hint and/or param_tweaks to determine intended dispersion parameters
     if name_hint is None and param_tweaks is None:
         raise InputError("""Can't guess -D parameters without name_hint ({}) or param_tweaks ({})""".format(
```

### Comparing `qcengine-0.8.2/qcengine/programs/model.py` & `qcengine-0.9.0/qcengine/programs/model.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/terachem.py` & `qcengine-0.9.0/qcengine/programs/terachem.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/dftd3.py` & `qcengine-0.9.0/qcengine/programs/dftd3.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,25 +259,24 @@
         retres = calcinfo[f'CURRENT {input_model.driver.upper()}']
         if isinstance(retres, Decimal):
             retres = float(retres)
         elif isinstance(retres, np.ndarray):
             retres = retres.ravel().tolist()
 
         output_data = {
-            'extras': {
-                'local_keywords': input_model.extras['info'],
-                'qcvars': calcinfo,
-            },
+            'extras': input_model.extras,
             'properties': {},
             'provenance': Provenance(creator="DFTD3",
                                      version=self.get_version(),
                                      routine=__name__ + '.' + sys._getframe().f_code.co_name),
             'return_result': retres,
             'stdout': stdout,
         }  # yapf: disable
+        output_data["extras"]['local_keywords'] = input_model.extras['info']
+        output_data["extras"]['qcvars'] = calcinfo
 
         output_data['success'] = True
         return Result(**{**input_model.dict(), **output_data})
 
 
 def dftd3_coeff_formatter(dashlvl: str, dashcoeff: Dict) -> str:
     """Return strings for DFTD3 program parameter file.
```

### Comparing `qcengine-0.8.2/qcengine/programs/rdkit.py` & `qcengine-0.9.0/qcengine/programs/rdkit.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/mopac.py` & `qcengine-0.9.0/qcengine/programs/mopac.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
         output = input_model.dict()
         output["provenance"] = {"creator": "mopac", "version": data.pop("mopac_version")}
 
         output["properties"] = {}
         output["properties"]["return_energy"] = data["heat_of_formation"]
 
-        output["extras"] = data
+        output["extras"].update(data)
 
         if input_model.driver == "energy":
             output["return_result"] = data["heat_of_formation"]
         else:
             output["return_result"] = gradient
 
         output['stdout'] = outfiles["dispatch.out"]
```

### Comparing `qcengine-0.8.2/qcengine/programs/base.py` & `qcengine-0.9.0/qcengine/programs/base.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/programs/mp2d.py` & `qcengine-0.9.0/qcengine/programs/mp2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -208,21 +208,20 @@
         retres = calcinfo[f'CURRENT {input_model.driver.upper()}']
         if isinstance(retres, Decimal):
             retres = float(retres)
         elif isinstance(retres, np.ndarray):
             retres = retres.ravel().tolist()
 
         output_data = {
-            'extras': {
-                'local_keywords': input_model.extras['info'],
-                'qcvars': calcinfo,
-            },
+            'extras': input_model.extras,
             'properties': {},
             'provenance': Provenance(creator="MP2D",
                                      version=self.get_version(),
                                      routine=__name__ + '.' + sys._getframe().f_code.co_name),
             'return_result': retres,
             'stdout': stdout,
         }  # yapf: disable
+        output_data["extras"]["local_keywords"] = input_model.extras['info']
+        output_data["extras"]["qcvars"] = calcinfo
 
         output_data['success'] = True
         return Result(**{**input_model.dict(), **output_data})
```

### Comparing `qcengine-0.8.2/qcengine/cli.py` & `qcengine-0.9.0/qcengine/cli.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/exceptions.py` & `qcengine-0.9.0/qcengine/exceptions.py`

 * *Files identical despite different names*

### Comparing `qcengine-0.8.2/qcengine/testing.py` & `qcengine-0.9.0/qcengine/testing.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,14 @@
 from pkg_resources import parse_version
 
 import qcengine as qcng
 import qcelemental as qcel
 from qcelemental.util import which, which_import
 
 
-@contextmanager
-def environ_context(env):
-    """Temporarily set environment variables inside the context manager and
-    fully restore previous environment afterwards
-    """
-    original_env = {key: os.getenv(key) for key in env}
-    os.environ.update(env)
-    try:
-        yield
-    finally:
-        for key, value in original_env.items():
-            if value is None:
-                del os.environ[key]
-            else:
-                os.environ[key] = value
-
-
 def is_program_new_enough(program, version_feature_introduced):
     """Returns True if `program` registered in QCEngine, locatable in
     environment, has parseable version, and that version in normalized
     form is equal to or later than `version_feature_introduced`.
 
     """
     if program not in qcng.list_available_programs():
```

### Comparing `qcengine-0.8.2/qcengine/compute.py` & `qcengine-0.9.0/qcengine/compute.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from qcelemental.models import FailedOperation, ResultInput
 
 from .config import get_config
 from .exceptions import InputError, RandomError
 from .procedures import get_procedure
 from .programs import get_program
-from .util import compute_wrapper, handle_output_metadata, model_wrapper
+from .util import compute_wrapper, environ_context, handle_output_metadata, model_wrapper
 
 __all__ = ["compute", "compute_procedure"]
 
 
 def _process_failure_and_return(model, return_dict, raise_error):
     if isinstance(model, FailedOperation):
         if raise_error:
@@ -71,26 +71,30 @@
             local_options = {}
 
         input_engine_options = input_data.extras.pop("_qcengine_local_config", {})
 
         local_options = {**local_options, **input_engine_options}
         config = get_config(local_options=local_options)
 
-        for x in range(config.retries + 1):
-            try:
-                output_data = executor.compute(input_data, config)
-                break
-            except RandomError as e:
-
-                if x == config.retries:
-                    raise e
-                else:
-                    metadata["retries"] += 1
-            except:
-                raise
+        # Set environment parameters and execute
+        with environ_context(config=config):
+
+            # Handle optional retries
+            for x in range(config.retries + 1):
+                try:
+                    output_data = executor.compute(input_data, config)
+                    break
+                except RandomError as e:
+
+                    if x == config.retries:
+                        raise e
+                    else:
+                        metadata["retries"] += 1
+                except:
+                    raise
 
 
     return handle_output_metadata(output_data, metadata, raise_error=raise_error, return_dict=return_dict)
 
 
 def compute_procedure(input_data: Union[Dict[str, Any], 'BaseModel'],
                       procedure: str,
@@ -125,10 +129,13 @@
         executor = get_procedure(procedure)
 
         config = get_config(local_options=local_options)
         input_data = executor.build_input_model(input_data)
 
         # Create a base output data in case of errors
         output_data = input_data.copy()  # lgtm [py/multiple-definition]
-        output_data = executor.compute(input_data, config)
+
+        # Set environment parameters and execute
+        with environ_context(config=config):
+            output_data = executor.compute(input_data, config)
 
     return handle_output_metadata(output_data, metadata, raise_error=raise_error, return_dict=return_dict)
```

