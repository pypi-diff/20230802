# Comparing `tmp/noether-1.0.1.tar.gz` & `tmp/noether-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noether-1.0.1.tar", last modified: Thu Jul 27 10:52:32 2023, max compression
+gzip compressed data, was "noether-1.1.tar", last modified: Wed Aug  2 16:48:28 2023, max compression
```

## Comparing `noether-1.0.1.tar` & `noether-1.1.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.878870 noether-1.0.1/
--rw-r--r--   0 yunruse    (501) staff       (20)     1064 2023-07-23 17:43:49.000000 noether-1.0.1/LICENSE.txt
--rw-r--r--   0 yunruse    (501) staff       (20)     3635 2023-07-27 10:52:32.878051 noether-1.0.1/PKG-INFO
--rw-r--r--   0 yunruse    (501) staff       (20)     3061 2023-07-23 18:03:30.000000 noether-1.0.1/README.md
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.811092 noether-1.0.1/noether/
--rw-r--r--   0 yunruse    (501) staff       (20)     3958 2023-07-27 10:51:03.000000 noether-1.0.1/noether/Multiplication.py
--rw-r--r--   0 yunruse    (501) staff       (20)      119 2023-07-23 17:43:49.000000 noether-1.0.1/noether/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2164 2023-07-23 17:43:49.000000 noether-1.0.1/noether/__main__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1430 2023-07-27 10:21:44.000000 noether-1.0.1/noether/_tokenizers.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.820063 noether-1.0.1/noether/catalogue/
--rw-r--r--   0 yunruse    (501) staff       (20)     1140 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/__init__.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.825851 noether-1.0.1/noether/catalogue/conventional/
--rw-r--r--   0 yunruse    (501) staff       (20)      145 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/conventional/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     3138 2023-07-27 10:21:27.000000 noether-1.0.1/noether/catalogue/conventional/conventional.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2524 2023-07-26 11:03:04.000000 noether-1.0.1/noether/catalogue/conventional/imperial.py
--rw-r--r--   0 yunruse    (501) staff       (20)      634 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/conventional/typographic.py
--rw-r--r--   0 yunruse    (501) staff       (20)     5950 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/dimensions.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1048 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/fundamental.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.833232 noether-1.0.1/noether/catalogue/historic/
--rw-r--r--   0 yunruse    (501) staff       (20)      110 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2485 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/ancient_greek.units.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4233 2023-07-27 10:49:00.000000 noether-1.0.1/noether/catalogue/historic/ancient_greek_.py
--rw-r--r--   0 yunruse    (501) staff       (20)      567 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/mts.units.py
--rw-r--r--   0 yunruse    (501) staff       (20)      792 2023-07-27 10:49:00.000000 noether-1.0.1/noether/catalogue/historic/mts_.py
--rw-r--r--   0 yunruse    (501) staff       (20)      456 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/historic/scientific.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.837338 noether-1.0.1/noether/catalogue/humorous/
--rw-r--r--   0 yunruse    (501) staff       (20)       73 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2377 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/fictional.py
--rw-r--r--   0 yunruse    (501) staff       (20)      820 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/potrzebie.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1080 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/humorous/unusual.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.844539 noether-1.0.1/noether/catalogue/info/
--rw-r--r--   0 yunruse    (501) staff       (20)       97 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2610 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/comparison.py
--rw-r--r--   0 yunruse    (501) staff       (20)      282 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/dimension.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2152 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/spectrum.py
--rw-r--r--   0 yunruse    (501) staff       (20)      355 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/info/unit_context.py
--rw-r--r--   0 yunruse    (501) staff       (20)      476 2023-07-26 10:15:46.000000 noether-1.0.1/noether/catalogue/info/unit_value.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2304 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/prefixes.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.858234 noether-1.0.1/noether/catalogue/scientific/
--rw-r--r--   0 yunruse    (501) staff       (20)     2804 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/CODATA.py
--rw-r--r--   0 yunruse    (501) staff       (20)      216 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1354 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/astronomy.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1640 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/cgs.py
--rw-r--r--   0 yunruse    (501) staff       (20)      290 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/climate.py
--rw-r--r--   0 yunruse    (501) staff       (20)      752 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/constants.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1803 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/data.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2411 2023-07-23 17:43:49.000000 noether-1.0.1/noether/catalogue/scientific/essential.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2796 2023-07-26 10:54:35.000000 noether-1.0.1/noether/catalogue/scientific/si.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4883 2023-07-24 12:28:18.000000 noether-1.0.1/noether/config.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.871126 noether-1.0.1/noether/core/
--rw-r--r--   0 yunruse    (501) staff       (20)     4088 2023-07-27 10:51:03.000000 noether-1.0.1/noether/core/Catalogue.py
--rw-r--r--   0 yunruse    (501) staff       (20)     4395 2023-07-26 12:23:58.000000 noether-1.0.1/noether/core/Dimension.py
--rw-r--r--   0 yunruse    (501) staff       (20)    10693 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/Measure.py
--rw-r--r--   0 yunruse    (501) staff       (20)      471 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/MeasureInfo.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1293 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/MeasureRelative.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1652 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/Prefix.py
--rw-r--r--   0 yunruse    (501) staff       (20)     5098 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/Unit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1179 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/UnitSet.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2462 2023-07-26 10:13:13.000000 noether-1.0.1/noether/core/_DisplayHandler.py
--rw-r--r--   0 yunruse    (501) staff       (20)      271 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/__init__.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.877009 noether-1.0.1/noether/core/units/
--rw-r--r--   0 yunruse    (501) staff       (20)     1257 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/AffineUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1813 2023-07-26 12:27:47.000000 noether-1.0.1/noether/core/units/GeometricUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2345 2023-07-24 12:28:18.000000 noether-1.0.1/noether/core/units/LinearUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)      516 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/PrefixedUnit.py
--rw-r--r--   0 yunruse    (501) staff       (20)      180 2023-07-23 17:43:49.000000 noether-1.0.1/noether/core/units/__init__.py
--rw-r--r--   0 yunruse    (501) staff       (20)     3296 2023-07-26 13:08:12.000000 noether-1.0.1/noether/display.py
--rw-r--r--   0 yunruse    (501) staff       (20)      974 2023-07-23 17:43:49.000000 noether-1.0.1/noether/errors.py
--rw-r--r--   0 yunruse    (501) staff       (20)     2076 2023-07-27 10:51:03.000000 noether-1.0.1/noether/gnu.py
--rw-r--r--   0 yunruse    (501) staff       (20)     1576 2023-07-23 17:43:49.000000 noether-1.0.1/noether/helpers.py
-drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-07-27 10:52:32.814603 noether-1.0.1/noether.egg-info/
--rw-r--r--   0 yunruse    (501) staff       (20)     3635 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/PKG-INFO
--rw-r--r--   0 yunruse    (501) staff       (20)     2060 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/SOURCES.txt
--rw-r--r--   0 yunruse    (501) staff       (20)        1 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/dependency_links.txt
--rw-r--r--   0 yunruse    (501) staff       (20)        8 2023-07-27 10:52:32.000000 noether-1.0.1/noether.egg-info/top_level.txt
--rw-r--r--   0 yunruse    (501) staff       (20)      301 2023-07-23 17:43:49.000000 noether-1.0.1/pyproject.toml
--rw-r--r--   0 yunruse    (501) staff       (20)       38 2023-07-27 10:52:32.879052 noether-1.0.1/setup.cfg
--rw-r--r--   0 yunruse    (501) staff       (20)      807 2023-07-23 18:03:30.000000 noether-1.0.1/setup.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.328417 noether-1.1/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1064 2023-08-01 11:04:18.000000 noether-1.1/LICENSE.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)     3706 2023-08-02 16:48:28.327285 noether-1.1/PKG-INFO
+-rw-r--r--   0 yunruse    (501) staff       (20)     3134 2023-08-02 16:47:17.000000 noether-1.1/README.md
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.264132 noether-1.1/noether/
+-rw-r--r--   0 yunruse    (501) staff       (20)     3958 2023-08-01 11:04:18.000000 noether-1.1/noether/Multiplication.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      119 2023-08-01 11:04:18.000000 noether-1.1/noether/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2736 2023-08-01 11:04:18.000000 noether-1.1/noether/__main__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1732 2023-08-01 11:04:18.000000 noether-1.1/noether/_tokenizers.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.272937 noether-1.1/noether/catalogue/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1102 2023-08-01 11:34:28.000000 noether-1.1/noether/catalogue/__init__.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.276235 noether-1.1/noether/catalogue/conventional/
+-rw-r--r--   0 yunruse    (501) staff       (20)      148 2023-08-01 19:32:00.000000 noether-1.1/noether/catalogue/conventional/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4253 2023-08-01 20:14:18.000000 noether-1.1/noether/catalogue/conventional/avourdupois.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     3894 2023-08-02 12:00:12.000000 noether-1.1/noether/catalogue/conventional/conventional.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      637 2023-08-01 19:32:00.000000 noether-1.1/noether/catalogue/conventional/typographic.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1811 2023-08-01 11:34:28.000000 noether-1.1/noether/catalogue/data.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     6074 2023-08-01 12:17:05.000000 noether-1.1/noether/catalogue/dimensions.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1125 2023-08-01 20:09:04.000000 noether-1.1/noether/catalogue/fundamental.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.282523 noether-1.1/noether/catalogue/historic/
+-rw-r--r--   0 yunruse    (501) staff       (20)      110 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/historic/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2485 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/historic/ancient_greek.units.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4233 2023-08-02 16:48:18.000000 noether-1.1/noether/catalogue/historic/ancient_greek_.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      567 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/historic/mts.units.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      792 2023-08-02 16:48:18.000000 noether-1.1/noether/catalogue/historic/mts_.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1981 2023-08-01 20:08:18.000000 noether-1.1/noether/catalogue/historic/scientific.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.287122 noether-1.1/noether/catalogue/humorous/
+-rw-r--r--   0 yunruse    (501) staff       (20)       73 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/humorous/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2377 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/humorous/fictional.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      820 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/humorous/potrzebie.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1364 2023-08-01 15:41:02.000000 noether-1.1/noether/catalogue/humorous/unusual.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.294618 noether-1.1/noether/catalogue/info/
+-rw-r--r--   0 yunruse    (501) staff       (20)       97 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/info/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2679 2023-08-01 11:41:01.000000 noether-1.1/noether/catalogue/info/comparison.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      282 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/info/dimension.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2152 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/info/spectrum.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      355 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/info/unit_context.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      781 2023-08-02 08:56:15.000000 noether-1.1/noether/catalogue/info/unit_value.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2304 2023-08-01 11:04:18.000000 noether-1.1/noether/catalogue/prefixes.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.305475 noether-1.1/noether/catalogue/scientific/
+-rw-r--r--   0 yunruse    (501) staff       (20)     3116 2023-08-01 15:14:40.000000 noether-1.1/noether/catalogue/scientific/CODATA.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      210 2023-08-01 14:50:27.000000 noether-1.1/noether/catalogue/scientific/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     3011 2023-08-01 17:01:10.000000 noether-1.1/noether/catalogue/scientific/astronomy.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1660 2023-08-01 19:51:46.000000 noether-1.1/noether/catalogue/scientific/cgs.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      742 2023-08-01 15:15:02.000000 noether-1.1/noether/catalogue/scientific/constants.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      565 2023-08-02 11:58:29.000000 noether-1.1/noether/catalogue/scientific/earth.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      969 2023-08-01 15:10:11.000000 noether-1.1/noether/catalogue/scientific/micro.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2236 2023-08-01 20:05:24.000000 noether-1.1/noether/catalogue/scientific/misc.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2782 2023-08-01 19:34:35.000000 noether-1.1/noether/catalogue/scientific/si.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4883 2023-08-01 11:04:18.000000 noether-1.1/noether/config.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.318013 noether-1.1/noether/core/
+-rw-r--r--   0 yunruse    (501) staff       (20)     4272 2023-08-02 16:43:40.000000 noether-1.1/noether/core/Catalogue.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     4395 2023-08-01 11:04:18.000000 noether-1.1/noether/core/Dimension.py
+-rw-r--r--   0 yunruse    (501) staff       (20)    12404 2023-08-02 11:49:59.000000 noether-1.1/noether/core/Measure.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      471 2023-08-01 11:04:18.000000 noether-1.1/noether/core/MeasureInfo.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1407 2023-08-02 08:27:34.000000 noether-1.1/noether/core/MeasureRelative.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1652 2023-08-01 11:04:18.000000 noether-1.1/noether/core/Prefix.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     5072 2023-08-02 13:30:52.000000 noether-1.1/noether/core/Unit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1179 2023-08-01 11:04:18.000000 noether-1.1/noether/core/UnitSet.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2462 2023-08-01 11:04:18.000000 noether-1.1/noether/core/_DisplayHandler.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      316 2023-08-02 08:40:39.000000 noether-1.1/noether/core/__init__.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.326115 noether-1.1/noether/core/units/
+-rw-r--r--   0 yunruse    (501) staff       (20)     1257 2023-08-02 11:56:04.000000 noether-1.1/noether/core/units/AffineUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1813 2023-08-01 11:04:18.000000 noether-1.1/noether/core/units/GeometricUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2345 2023-08-01 11:55:36.000000 noether-1.1/noether/core/units/LinearUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1883 2023-08-02 16:45:09.000000 noether-1.1/noether/core/units/LogarithmicUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      516 2023-08-01 11:04:18.000000 noether-1.1/noether/core/units/PrefixedUnit.py
+-rw-r--r--   0 yunruse    (501) staff       (20)      248 2023-08-01 23:08:55.000000 noether-1.1/noether/core/units/__init__.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     3541 2023-08-01 11:04:18.000000 noether-1.1/noether/display.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1209 2023-08-02 08:28:59.000000 noether-1.1/noether/errors.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     2076 2023-08-01 11:04:18.000000 noether-1.1/noether/gnu.py
+-rw-r--r--   0 yunruse    (501) staff       (20)     1576 2023-08-01 11:04:18.000000 noether-1.1/noether/helpers.py
+drwxr-xr-x   0 yunruse    (501) staff       (20)        0 2023-08-02 16:48:28.268105 noether-1.1/noether.egg-info/
+-rw-r--r--   0 yunruse    (501) staff       (20)     3706 2023-08-02 16:48:28.000000 noether-1.1/noether.egg-info/PKG-INFO
+-rw-r--r--   0 yunruse    (501) staff       (20)     2121 2023-08-02 16:48:28.000000 noether-1.1/noether.egg-info/SOURCES.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)        1 2023-08-02 16:48:28.000000 noether-1.1/noether.egg-info/dependency_links.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)        8 2023-08-02 16:48:28.000000 noether-1.1/noether.egg-info/top_level.txt
+-rw-r--r--   0 yunruse    (501) staff       (20)      301 2023-08-01 11:04:18.000000 noether-1.1/pyproject.toml
+-rw-r--r--   0 yunruse    (501) staff       (20)       38 2023-08-02 16:48:28.328739 noether-1.1/setup.cfg
+-rw-r--r--   0 yunruse    (501) staff       (20)      805 2023-08-01 11:04:18.000000 noether-1.1/setup.py
```

### Comparing `noether-1.0.1/LICENSE.txt` & `noether-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/PKG-INFO` & `noether-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: noether
-Version: 1.0.1
+Version: 1.1
 Summary: Work with physical measurements and constants
 Home-page: https://github.com/yunruse/noether
 Author: Mia yun Ruse
 Author-email: mia@yunru.se
 Keywords: physics unit measure constant measurement uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Noether 1.0.1 (in development)
+# Noether
+`523 units, 60 prefixes`
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -31,14 +32,16 @@
 
 ```sh
 $ alias noe='python -im noether'
 $ noe marathon
 marathon  # length, 42195 m, Race length based on Greek legend, set by convention from 1908 Summer Olympics
 $ noether 23degC @ degF
 73.4 °F  # temperature
+$ noether 'horsepower @ dB(kW)'
+-1.33418061 dB(kW)  # power, 0.73549875 kW
 ```
 
 The CLI allows a few niceties such as slightly terser syntax, but otherwise behaves identically to Python:
 
 ```sh
 $ noether 5cm @ in --value
 1.9685039370078738
@@ -53,15 +56,15 @@
 ```py
 >>> display(inch)
 >>> 5 * cm
 >>> mile
 mile  # length, 63360 in
 ```
 
-Units can propagate uncertainty automatically under most operations:
+Units propagate uncertainty automatically under most operations:
 
 ```py
 >>> m(5, 0.1)**3
 125 ± 7.5 m**3  # volume
 ```
 
 You can define your own units and dimensions:
```

### Comparing `noether-1.0.1/README.md` & `noether-1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# Noether 1.0.1 (in development)
+# Noether
+`523 units, 60 prefixes`
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -14,14 +15,16 @@
 
 ```sh
 $ alias noe='python -im noether'
 $ noe marathon
 marathon  # length, 42195 m, Race length based on Greek legend, set by convention from 1908 Summer Olympics
 $ noether 23degC @ degF
 73.4 °F  # temperature
+$ noether 'horsepower @ dB(kW)'
+-1.33418061 dB(kW)  # power, 0.73549875 kW
 ```
 
 The CLI allows a few niceties such as slightly terser syntax, but otherwise behaves identically to Python:
 
 ```sh
 $ noether 5cm @ in --value
 1.9685039370078738
@@ -36,15 +39,15 @@
 ```py
 >>> display(inch)
 >>> 5 * cm
 >>> mile
 mile  # length, 63360 in
 ```
 
-Units can propagate uncertainty automatically under most operations:
+Units propagate uncertainty automatically under most operations:
 
 ```py
 >>> m(5, 0.1)**3
 125 ± 7.5 m**3  # volume
 ```
 
 You can define your own units and dimensions:
```

### Comparing `noether-1.0.1/noether/Multiplication.py` & `noether-1.1/noether/Multiplication.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/__main__.py` & `noether-1.1/noether/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,99 @@
 """
-TODO: write a description here...
-"""
+Command-line interface to Noether.
+
+Provide terms (eg `-10degC @ degF` or `30dalton`) to see their value.
 
-# TODO: utilise lexer for the rules
-#    `1m` -> `1 * m`
-#    `in` -> `inch`
-# TODO: add --si
+Best ran as `python -im noether`, as if no terms are provided,
+a convenient interactive prompt is summoned.
+"""
 
+from os import environ
 import noether
 from noether import *
 
 
 from argparse import ArgumentParser
-parser = ArgumentParser()
+parser = ArgumentParser(
+    description=__doc__,
+    usage='python -[i]m noether [-h] [--no-color] [--value] [terms ...]'
+)
 parser.add_argument(
-    '--no-color',  # TODO: what is the gnu standard here?
+    '--no-color',
     action='store_false',
-    help='Suppress colour output',
+    help='Suppress colour output (NO_COLOR=1 is also supported)',
     dest='color')
 parser.add_argument(
-    '--value', '-V',  # TODO: what is the gnu standard here?
+    '--value', '-V',
     action='store_true',
-    help='Display the value only (equivalent to str(statement))')
+    help='If terms are present, display only their numeric value')
 
-parser.add_argument('terms', nargs='*')
+# weird args like `-10degC` are thrown to `unknown`,
+# but if we get args with a nargs='*', they may be in the wrong order
+# therefore, we'll just fetch every unknown argument
+args, unknown = parser.parse_known_args()
+args.terms = unknown
 
-args = parser.parse_args()
+# % Color
+
+if environ.get('NO_COLOR', ''):
+    args.color = False
 
 pretty = None
 if args.color and not args.value:
     try:
-        from rich import pretty, print
+        from rich import pretty
     except ImportError:
         pass
     else:
         pretty.install()
 
+# % Eval and print terms
+
 if args.terms:
-    # this is very basic at the moment!
     from ._tokenizers import cli_dialect, transform
     src = transform(" ".join(args.terms), cli_dialect)
     try:
         del cli_dialect, transform
         value = eval(src)
         if args.value:
             if isinstance(value, Measure):
                 print(value.value)
             else:
                 print(value)
         else:
-            print(repr(value))
+            if isinstance(value, Measure) and pretty:
+                from rich import print as _print
+                _print(value)
+            else:
+                print(repr(value))
     except Exception as e:
         import traceback
-        traceback.print_exception(e, limit=0)
         import os
+        traceback.print_exception(e, limit=0)
         os._exit(2)
     else:
         import os
         os._exit(0)
     # regular exit(0) does not work with `python -im noether` - it displays an exception and continues.
     # _exit, meanwhile, forces an exit.
     # Note that this will NOT process any __del__ cleanups,
     # but this is considered not a major problem – bare evals automatically self-delete this way,
     # and we can't assign variables in eval(), so we shouldn't feasibly be able to, for example,
     # have `open()` leave a file handle open or something.
 
+# % REPL
+
+# TODO: allow cli dialect?
+
 print(f'{len(catalogue.units())} units, {len(list(catalogue.prefixes()))} prefixes')
 print('''
 >>> import noether
 >>> from noether import *''')
 
 if pretty is not None:
     print('''\
->>> from rich import pretty, print
+>>> from rich import pretty
 >>> pretty.install()''')
 print()
 
-del args, parser, ArgumentParser
+del ArgumentParser, parser, args, unknown
```

### Comparing `noether-1.0.1/noether/catalogue/__init__.py` & `noether-1.1/noether/catalogue/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from noether.config import Config, conf
 
 # Essentials
 from .prefixes import *
 from .dimensions import *
 
 # Units are imported in this exact order
+from .data import *
 from .scientific import *
 from .conventional import *
 
 Config.register('CATALOGUE_historical', True, help='''\
 Provide historical units.''')
 if conf.get('CATALOGUE_historical'):
     from .historic import *
@@ -29,10 +30,7 @@
 vars().update({p.prefix: p for p in catalogue.prefixes()})
 
 Config.register('CATALOGUE_all_prefixes_in_namespace', True, help='''\
 Put every prefixed unit (microohm, kibibyte &c) as measures in the Noether namespace.
 This may cause annoyance if you `from noether import *`!''')
 if conf.get('CATALOGUE_all_prefixes_in_namespace'):
     vars().update(catalogue.all_prefixed_units())
-
-# HACK: some name collisions are not the best
-K = kelvin
```

### Comparing `noether-1.0.1/noether/catalogue/conventional/conventional.py` & `noether-1.1/noether/catalogue/conventional/conventional.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 '''
 Conventional SI-compatible units.
 '''
 
-from noether.core import Unit, AffineUnit
+from noether.core import Unit, AffineUnit, LogarithmicUnit
 from noether.core import display
 from noether.config import Config, conf
 
-from math import pi
+from math import pi, log as _log, e as _e
 
 from ..prefixes import SI_all, SI_large, SI_small
 from ..scientific import meter, second, kilogram, kelvin
 from ..scientific import radian, turn
 from ..scientific import turn
 from ..scientific import day, hour, minute
-from ..scientific import gram
+from ..scientific import gram, bar
 from ..scientific import standard_gravity
 
 # % Ratio
 percent = Unit(1/100, 'percent', '%')
 permille = Unit(1/1000, 'permille', '‰')
 ppm = parts_per_million = Unit(1/1_000_000, 'parts_per_million', 'ppm')
 proof = Unit(0.5, 'proof', '°', info='alcohol purity')
 karat = Unit(
     1 / 24, 'karat', 'Kt',
     info="Used in gold purity; 24Kt is pure or near-pure."
     " Increasingly deprecated for millesimal fineness."
     " Not to be confused with the carat.")
 
+# % Logarithmic ratio
+
+bel = LogarithmicUnit(1, 1, "bel", "B")
+decibel = dB = LogarithmicUnit(1, 10, "decibel", "dB")
+neper = Np = LogarithmicUnit(1/_e, _log(10), "neper", "Np")
+
 # % Temperature
 celsius = degC = AffineUnit(kelvin*1, kelvin*273.15, "celsius", "°C")
 
 # % Time
 week = Unit(day * 7, "week", "w")
 fortnight = week * 2
 year_gregorian = Unit(
@@ -49,20 +55,28 @@
 )
 
 # % Area
 are = Unit(100 * meter**2, "are", "a")
 hectare = Unit(100 * are, "hectare", "ha")
 
 # % Volume
-litre = liter = L = Unit((meter/10) ** 3, ["liter", "litre"], "l", SI_all)
-milliliter = milliliter = ml = mL = Unit(
-    liter / 1000, ['milliliter', 'millilitre'], 'mL')
+litre = liter = L = Unit((meter/10) ** 3, ["liter", "litre"], "L", SI_all)
+_ml = L / 1000
+
+# % cooking
+tablespoon = tbsp = Unit(
+    15 * _ml, 'tablespoon', 'tbsp',
+    info="A cooking volume used in the UK and Canada. Not to be confused with the AU or US tablespoon.")
+teaspoon = tsp = Unit(
+    tbsp / 3, 'teaspoon', 'tsp', info='A cooking volume.')
+dessertspoon = dstspn = Unit(
+    10 * _ml, 'dessertspoon', 'dstspn', info='A cooking volume.')
 
 # % Mass & density
-ton = tonne = Unit(
+ton = tonne = metricton = Unit(
     kilogram*1000, ["ton", "tonne"], "t", SI_large, info="metric")
 gsm = Unit(
     gram / meter**2, "gram per square meter", "gsm",
     info="Used especially in paper-making as a proxy for thickness and pliability. "
     " A standard sheet of printer paper is usually 100gsm.")
 carat = Unit(
     gram * 0.2, "carat", "ct",
@@ -74,21 +88,28 @@
 
 deg = degree = Unit(radian * pi / 180, "degree", ["°", "deg"])
 arcminute = arcmin = Unit(degree / 60, "arcminute", ["′", "arcmin"])
 arcsecond = arcsec = Unit(
     degree / 3600, "arcsecond", ["″", "arcsec"], SI_small)
 
 # % Mechanical
-
 horsepower = Unit(
     standard_gravity * kilogram*75 * meter / second,
     'horsepower', 'hp',
     info="Metric horsepower, not to be confused with the"
     " imperial horsepower which is slightly larger")
 
+mach = Unit(
+    331.46 * meter/second, "mach", "Ma",
+    info="Conventional measure for air at 0°C; a mach number is defined locally relative to the air.")
+
+msw = Unit(bar/10, "meter_sea_water", "msw")
+
+mired = Unit(1 / kelvin(1e6), "mired")
+
 
 # % Display
 Config.register('UNITS_conventional_time', True, '''\
 Display time in year & day & hour & minute & second.''')
 if conf.get('UNITS_conventional_time'):
     display(year & day & hour & minute & second)
```

### Comparing `noether-1.0.1/noether/catalogue/conventional/imperial.py` & `noether-1.1/noether/catalogue/historic/scientific.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,71 @@
 '''
-Imperial units.
+Obscure scientific units.
 '''
 
-# TODO: #1 all of this nonsense
+from math import pi
+from noether.core import Unit
 
-from fractions import Fraction
+from noether.core.units import AffineUnit
 
-from noether.core import Unit, AffineUnit
-from noether.config import Config, conf
+from noether.catalogue.prefixes import SI_all
 
-from ..scientific import meter, kelvin, mercury
-from ..scientific import cm, gram, hour, second
-from .conventional import liter
+from ..scientific import kilogram, hertz, kelvin, meter, coulomb
+from ..scientific import becquerel, nit, candela
+from ..scientific import dalton, electron_charge
+from ..scientific import cm, gram, au
+from ..conventional import liter, foot
 
-Config.register('UNITS_country', 'us', '''\
-The country to define imperial units (and other niceties) from. (Use the ISO 3166 code.)
-''')
-_USE_US_UNITS = conf.get('UNITS_country').lower() == 'us'
 
-rankine = Unit(kelvin * 5/9, "rankine", "°R")
-fahrenheit = degF = AffineUnit(rankine, rankine(459.67), "fahrenheit", "°F")
+# % Photometry
+fresnel = Unit(hertz(1e12), "fresnel")
 
-# % Length
-inch = Unit(cm * Fraction(127, 50), "inch", ["in", '"'])
+apostilb = blondel = Unit(nit / pi, "apostilb", "asb")
+skot = Unit(apostilb(1e-3), "skot", "sk")
+bril = Unit(apostilb(1e-7), "bril")
+lambert = Unit(apostilb(1e4), "lambert", ["Lb", "L"], SI_all)
+foot_lambert = Unit(candela / pi / foot**2, "foot_lambert", "fL")
 
-barleycorn = Unit(inch / 3, "barleycorn")
-thou = Unit(inch / 1000, "barleycorn")
-twip = Unit(inch / 1440, "twip")  # twentieth of a point
+# TODO: foot-lambert
 
-# twip =
-hand = Unit(inch * 4, "hand", "hh")
-foot = Unit(inch * 12, "foot", ["ft", "'"])
-yard = Unit(foot * 3, "yard", "yd")
-chain = Unit(yard * 22, "chain", "ch")
-furlong = Unit(chain * 10, "furlong", "fur")
-mile = Unit(furlong * 8, "mile", "mi")
-league = Unit(mile * 3, "league", "lea")
-# TODO: maritime units, Gunter's survey units
+# % Temperature
 
-# % Speed
-nautical_mile = Unit(meter * 1852, "nautical_mile", "nmi")
+degN = degNewton = AffineUnit(
+    kelvin * 100/33, kelvin*273.15, "degNewton", "°N")
+degRe = Reamur = AffineUnit(
+    kelvin*0.8, kelvin*273.15, "Réamur", "°Ré")
+degDe = Delisle = AffineUnit(
+    kelvin*-2/3, kelvin*373.15, "Delisle", "°De")
+degRo = Romer = AffineUnit(
+    kelvin * 40/21, kelvin * (273.15-7.5 * 40/21), "Rømer", "°Rø")
 
-mph = miles_per_hour = Unit(mile / hour, "miles_per_hour", "mph")
-knot = Unit(nautical_mile / hour, "knot", ["kn", "kt"])
+# % Radiation
 
+curie = Unit(
+    3.7e10 * becquerel, "curie", "Ci",
+    info="Introduced in 1910. Discouraged for the becquerel")
+rutherford = Unit(
+    1e6 * becquerel, "rutherford", "Rd",
+    info="Introduced in 1946. Discouraged for the becquerel since 1975")
+roentgen = Unit(
+    2.58 * coulomb / kilogram, ["roentgen", "röntgen"], "R",
+    info="Adopted as international standard in 1928. Deprecated since roughly 1998")
+mache = Unit(
+    3.64e-10 * curie / liter, "Mache", "ME",
+    info="Deprecated")
 
-# % Area
+# % Atomic
 
-acre = Unit(chain * furlong, "acre", "ac")
+thomson = Unit(
+    dalton / electron_charge, "thomson", "Th",
+    info="Deprecated since 2013")
 
-# TODO: all of this nonsense
+# % Astronomy
 
-# % Volume
-gallon_uk = Unit(liter(4.546_09), "gallon_uk", "gal")
-gallon_us = Unit(inch**3 * 231, "gallon_us", "gal")
-# gallon_us_dry = usdrygal = Unit(bushel_us / 8, "gallon_us_dry", "usdrygal"))
+siriometer = Unit(au * 1e6, "siriometer", "sir")
+spat_length = Unit(meter * 1e12, "spat_length", "S")
 
-pint_uk = Unit(gallon_uk / 8, "pint_uk", "pt")
-pint_us = Unit(gallon_us / 8, "pint_us", "pt")
-pint = pint_us if _USE_US_UNITS else pint_uk
+# % Earth
 
-fluid_ounce_uk = floz_uk = Unit(pint_uk / 12, "fluid_ounce_uk", "fl oz")
-fluid_ounce_us = floz_us = Unit(pint_us / 16, "fluid_ounce_us", "fl oz")
-fluid_ounce = floz = floz_us if _USE_US_UNITS else floz_uk
-
-
-dram = Unit(fluid_ounce / 8, "dram", "dr")
-
-
-hogshead = Unit(0, "hogshead", "hhd")  # TODO
-butt = Unit(hogshead * 2, "butt")  # y'all nerds
-
-
-# % Mass
-pound = lb = Unit(453.59237 * gram, "pound", "lb")
-poundal = Unit(lb * foot / second**2, "poundal", "pdl")
-
-oz = ounce = Unit(pound / 16, "ounce", "oz")
-grain = Unit(pound / 7000, "grain", "gr")
-
-stone = st = Unit(pound * 14, "stone", "st")
-imperial_ton = Unit(pound * 2240, "ton", "t")
-
-
-# % Derived
-
-inch_mercury = Unit(mercury * inch,
-                    "inch_mercury", "inHg")
+technical_atmosphere = Unit(
+    kilogram * gram / cm**2, "technical_atmosphere", "at",
+    info="Deprecated")
```

### Comparing `noether-1.0.1/noether/catalogue/conventional/typographic.py` & `noether-1.1/noether/catalogue/conventional/typographic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Typographic (imperial) units.
 '''
 
 from noether.core import Unit
 
-from .imperial import inch
+from .avourdupois import inch
 
 pica = Unit(inch / 6, "pica")  # as defined by PostScript
 cicero = Unit(inch / 6, "cicero")
 
 pica_american = Unit(inch * 400/2409, "pica_american")  # as used in TeX
 pica_french = Unit(inch * 0.1776, "pica_french")
 point = Unit(inch / 72, "point", "pt")  # DTP point - this one varies a lot!
```

### Comparing `noether-1.0.1/noether/catalogue/dimensions.py` & `noether-1.1/noether/catalogue/dimensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 if conf.get('DIMENSION_angle'):
     angle = Dimension.new("angle", "φ", 200)
 else:
     angle = dimensionless
 solid_angle = D(angle**2, 'solid_angle')
 
-frequency = D(time**-1, 'frequency')
+frequency = radioactivity = D(time**-1, 'frequency', 'radioactivity')
 
 # % Dynamics
 
 force = weight = D(mass * acceleration, 'force', 'weight')
 pressure = D(force / area, 'pressure')
 energy = D(force * length, 'energy')
 power = D(energy / time, 'power')
@@ -99,15 +99,15 @@
 luminance = D(luminosity / area, 'luminance')
 illuminance = luminous_exitance = luminous_emittance = D(
     luminous_flux / area, 'illuminance', 'luminous_exitance', 'luminous_emittance')
 
 luminous_exposure = D(illuminance * time, 'luminous_exposure')
 luminous_energy_density = D(
     luminous_energy / volume, 'luminous_energy_density')
-luminous_efficiacy = D(luminosity / power, 'luminous_efficiacy')
+luminous_efficacy = D(luminous_energy / power, 'luminous_efficiacy')
 
 irradiance = intensity = heat_flux = D(
     power / area, 'irradiance', 'intensity', 'heat_flux')
 
 emission_coefficient = D(
     length / time**3 * solid_angle, 'emission_coefficient')
 
@@ -121,14 +121,17 @@
 density = D(mass / volume, 'density')
 specific_volume = D(volume / mass, 'specific_volume')
 
 number_density = D(1 / volume, 'number_density')
 probability_density = D(1 / volume, 'probability_density')
 reaction_rate = D(substance / (volume * time), 'reaction_rate')
 
+volumetric_radioactivity = D(
+    radioactivity / volume, 'volumetric_radioactivity')
+
 specific_energy = dose = D(energy / mass, 'specific_energy', 'dose')
 energy_density = D(energy / volume, 'energy_density')
 molar_energy = D(energy / substance, 'molar_energy')
 
 heat_capacity = entropy = D(energy / temperature, 'entropy')
 specific_heat_capacity = D(heat_capacity / mass, 'specific_heat_capacity')
 molar_heat_capacity = D(heat_capacity / substance, 'molar_heat_capacity')
```

### Comparing `noether-1.0.1/noether/catalogue/fundamental.py` & `noether-1.1/noether/catalogue/fundamental.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 substance = Dimension.new('substance', 'N', -3)
 length = Dimension.new('length', 'L', -2)
 time = Dimension.new('time', 'T', -1)
 
 candela = cd = Unit(luminosity, 'candela', 'cd', SI_all)
 ampere = A = Unit(current, 'ampere', 'A', SI_all)
 kelvin = K = Unit(temperature, 'kelvin', 'K', SI_all)
-kilogram = kg = Unit(mass, 'kilogram', 'kg')
+kilogram = kg = Unit(mass, ['kilogram', 'key'], 'kg')
+# prefixes are assigned to gram in scientific/cgs.py
 mole = mol = Unit(substance, 'mole', 'mol', SI_all)
 meter = metre = m = Unit(length, ['meter', 'metre'], 'm', SI_all)
-second = s = Unit(time, 'second', 's', SI_all)
+second = s = sec = Unit(time, ['second', 'sec'], 's', SI_all)
 
 __all__ = [
     'luminosity', 'candela', 'cd',
     'current', 'ampere', 'A',
     'temperature', 'kelvin', 'K',
     'mass', 'kilogram', 'kg',
     'substance', 'mole', 'mol',
```

### Comparing `noether-1.0.1/noether/catalogue/historic/ancient_greek.units.py` & `noether-1.1/noether/catalogue/historic/ancient_greek.units.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/historic/ancient_greek_.py` & `noether-1.1/noether/catalogue/historic/ancient_greek_.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/historic/mts.units.py` & `noether-1.1/noether/catalogue/historic/mts.units.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/historic/mts_.py` & `noether-1.1/noether/catalogue/historic/mts_.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/humorous/fictional.py` & `noether-1.1/noether/catalogue/humorous/fictional.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/humorous/potrzebie.py` & `noether-1.1/noether/catalogue/humorous/potrzebie.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/humorous/unusual.py` & `noether-1.1/noether/catalogue/humorous/unusual.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 '''
 
 from noether.core import Unit, UnitSet
 
 from ..prefixes import SI_all
 from ..fundamental import second
 from ..scientific import minute, watt_hour, sievert, angstrom, sol
-from ..conventional import inch
-
-U = UNUSUAL = UnitSet()
+from ..conventional import inch, hour, year
 
 # % Length
 beard_second = Unit(
     angstrom * 100, "beard_second",
     info="According to popular convention, although the average figure is close to half of this.")
 
 # % Time
 warhol = Unit(minute * 15, "warhol", prefixes=SI_all,
               info="Warhol's \"fifteen minutes of fame\"")
 beard_inch = Unit(inch / (beard_second/second), "beard_inch")
 
+dog_year = Unit(
+    year / 7, "dog_year",
+    info="This is a very approximate measure and dependent on breed and size")
 
 # % Energy and radiation
+# https://blog.xkcd.com/2011/03/19/radiation-chart/
 BED = banana_equivalent_dose = Unit(
     sievert * 1e-7, "banana_equivalent_dose", "BED",
     info="c.f. xkcd radiation chart for other useful radiation units")
-# https://blog.xkcd.com/2011/03/19/radiation-chart/
+flight_dose_rate = Unit(
+    sievert * 4e-9 / hour, "flight_dose_rate", "FED",
+    info="Standardised ionizing radiation at 10km cruising altitude")
 
 pirate_ninja = Unit(
     watt_hour * 1000 / sol, "pirate_ninja", "pn",
-    info="from the book The Martian")
+    info="1 kWh per Martian day, from Andy Weir's The Martian")
```

### Comparing `noether-1.0.1/noether/catalogue/info/comparison.py` & `noether-1.1/noether/catalogue/info/comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from math import log
 
 from noether import Dimension, Measure, MeasureInfo
 
 from .. import angstrom, km, cm, meter, foot
 from .. import year, day, hour, minute, second
-from .. import c
+from .. import c, liter
 
 # TODO: incorporate all catalogue units to save effort
 # and then you can move some unusual units to a new `unusual.py`
 
 kmq = km**2
 COMPARISON_MEASURES: dict[str, Measure] = {
     'average human height': cm(170),
@@ -44,14 +44,17 @@
 
     'Sergipe': kmq(91_910.4),
     'São Paulo': kmq(1_521.11),
 
     # % Speed
     'the speed of sound in air': meter(343) / second,
     'average human walk speed': meter(1.42) / second,
+
+    # % volume
+    'olympic swimming pool': liter(2_500_000)
 }
 
 
 @Measure.Info
 class info_comparison(MeasureInfo):
     "Compare measures to everyday or well-known items."
     style = 'underline red'
```

### Comparing `noether-1.0.1/noether/catalogue/info/spectrum.py` & `noether-1.1/noether/catalogue/info/spectrum.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/prefixes.py` & `noether-1.1/noether/catalogue/prefixes.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/catalogue/scientific/CODATA.py` & `noether-1.1/noether/catalogue/scientific/CODATA.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,17 +9,21 @@
 
 from . import si
 catalogue = Catalogue(vars(si), 'CODATA data-fetching catalogue')
 
 
 COLUMN_LENGTHS = [60, 25, 25]
 NAMED_CODATA_UNITS = {
-    'atomic mass constant': 'u',
-    'electron mass': 'm_e',
-    'Newtonian constant of gravitation': 'G'
+    'atomic_mass_constant': 'u',
+    'electron_mass': 'm_e',
+    'Newtonian_constant_of_gravitation': 'G',
+    'Loschmidt_constant_at_101_325_Pa': 'n_0',
+    'Avogadro_constant': 'N_a',
+    'Boltzmann_constant': 'k_B',
+    'fine_structure_constant': 'α',
 }
 
 one = Unit(1)
 
 
 def _fmt_name(string: str):
     return (string
@@ -27,14 +31,16 @@
             .replace('-', '_')
             .replace('._', '_')
             .replace('.', '_')
             .replace('_(', '_with_')
             .replace(')', '')
             .replace(',', '')
             .replace('/', '_over_')
+            .replace('_with_273_15_K_', '_at_')
+            .replace('101_325_kPa', '101_325_Pa')
             )
 
 
 def _fmt_value(string: str):
     if string == '(exact)':
         return 0
     return float(string
@@ -50,39 +56,40 @@
     scanning = False
     with open(path) as f:
         for line in f.readlines():
             if not scanning:
                 scanning = line.startswith('----')
                 continue
 
-            name, value, uncertainty, unit = scanline(line, COLUMN_LENGTHS)
+            full_name, value, uncertainty, unit = scanline(
+                line, COLUMN_LENGTHS)
 
-            if name == 'Avogadro constant':
-                # TODO: #42 ComposedUnit
-                # HACK
-                unit = ''
+            # if full_name == 'Avogadro constant':
+            #     # TODO: #42 ComposedUnit
+            #     # HACK
+            #     unit = ''
 
-            chunks = name.split()
-            if 'in' in chunks and not name.startswith('shielding'):
+            chunks = full_name.split()
+            if 'in' in chunks and not full_name.startswith('shielding'):
                 continue  # already defined in another unit
             if chunks[-1] == 'relationship':
                 continue  # unit does not need extra definition
 
             value = _fmt_value(value)
-            name = _fmt_name(name)
+            name = _fmt_name(full_name)
             uncertainty = _fmt_value(uncertainty) or None
             unit = unit.replace('^', '**').replace(' ', '*')
             unit = eval(unit, {}, catalogue) if unit else one
 
             symbol = NAMED_CODATA_UNITS.get(name)
             units[name] = Unit(
                 unit(value, uncertainty),
                 name,
                 symbol,
-                info='CODATA 2018',
+                info=f'{full_name}, CODATA 2018',
             )
 
     return units
 
 
 _CODATA_PATH = __file__.removesuffix('.py') + '.txt'
 CODATA = _codata(_CODATA_PATH)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noether-1.0.1/noether/catalogue/scientific/cgs.py` & `noether-1.1/noether/catalogue/scientific/cgs.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from noether.core import Unit, UnitSet
 
 from math import pi
 
 from ..prefixes import SI_all, centi
 from .si import SI_all, meter, kilogram, second as s
 from .si import ampere, lux, coulomb, henry, ohm, volt, tesla
-from .essential import turn, nit
+from .misc import turn, nit
 
 
 # CGS units
-gram = g = Unit(kilogram / 1000, 'gram', 'g', SI_all)
+gram = g = Unit(
+    kilogram / 1000, ['gram', 'gramme'], ['g', 'gm'], SI_all)
 cm = centi * meter
 
 CGS = UnitSet({cm, g, s})
 
 
 # Dynamics
 gal = CGS(Unit(cm/s**2, "gal", "Gal"))
@@ -25,15 +26,15 @@
 erg = CGS(Unit(dyne * cm, "erg"))
 barye = CGS(Unit(g / (cm * s**2), "barye", "Ba"))
 poise = CGS(Unit(g / (cm*s), "poise", "P"))
 stokes = CGS(Unit(cm**2/s, "stokes", "St"))
 kayser = CGS(Unit(1/cm, "kayser", "K"))
 
 # Luminance
-phot = CGS(Unit(lux / 10_000, 'phot', 'ph'))
+phot = CGS(Unit(10_000 * lux, 'phot', 'ph'))
 stilb = CGS(Unit(nit * 1e4, 'stilb', 'sb'))
 
 # EMU
 abampere = abA = biot = Unit(
     ampere * 10, ["abampere", "biot"], ["abA", "Bi"])
 abcoulomb = abC = Unit(coulomb * 10, "abcoulomb", "abC")
 abhenry = abH = Unit(henry * 1e-9, "abhenry", "abH")
```

### Comparing `noether-1.0.1/noether/catalogue/scientific/constants.py` & `noether-1.1/noether/catalogue/scientific/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 
 from ..fundamental import ampere, kelvin, kilogram, meter
 from .si import joule, newton, e, hbar, c
 from .CODATA import CODATA
 
 from math import pi
 
-mu_0 = Unit(4 * pi * 1e-7 * newton / ampere ** 2, "mu_0", "μ₀")
-e_0 = Unit(1 / (mu_0 * c ** 2), "e_0", "e₀")
+vacuum_permeability = mu_0 = Unit(
+    4 * pi * 1e-7 * newton / ampere ** 2, "vacuum_permeability", ["mu_0", "μ₀"])
+vacuum_permittivity = e_0 = Unit(
+    1 / (mu_0 * c ** 2), "vacuum_permittivity", ["e_0", "ε₀"])
 z_0 = Unit(mu_0 * c, "z_0", "z₀")
 
 k_e = Unit(1 / (4*pi*e_0), "k_e", "kₑ")
 
-fine_structure_constant = alpha = Unit(
-    k_e * e**2 / (hbar*c),
-    ["fine_structure_constant", "alpha"], "α")
 rydberg = Ry = Unit(
     joule(2.179_872_361_1035, 4.2e-15),
     "rydberg", "Ry", info="CODATA 2018")
 
 # % Miscelleneous
 t = kelvin(273.15)
 water_density = (kilogram/meter**2)(0.9998395)
```

### Comparing `noether-1.0.1/noether/catalogue/scientific/data.py` & `noether-1.1/noether/catalogue/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Data units, including the byte, shannon and pixel.
 '''
 
 from noether.core import Unit, Dimension
 from noether.core import display
 
-from ..prefixes import IEC, SI_all, SI_large
-from ..fundamental import length, second, time
-from .cgs import cm
-from ..conventional import inch
+from .prefixes import IEC, SI_all, SI_large
+from .fundamental import length, second, time
+from .scientific.cgs import cm
+from .conventional import inch
 
 from math import log
 
 
 def D(d: Dimension, *n: str):
     return display(Dimension(d, *n))
```

### Comparing `noether-1.0.1/noether/catalogue/scientific/essential.py` & `noether-1.1/noether/catalogue/scientific/misc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 '''
-Essential scientific units.
+Miscelaneous or human scientific units.
 '''
 
 from noether.core import Unit
 
 from math import pi
 
-from ..prefixes import SI_all, micro
+from ..prefixes import SI_all
 from ..fundamental import candela, kilogram, meter, kelvin, ampere
 from .si import radian, steradian
 from .si import joule, watt, pascal, cumec
-from .si import hour
+from .si import hour, minute, second
 
 # % Angle
-gradian = Unit(radian * pi / 200, "gradian", "grad")
-circle = turn = Unit(radian * 2*pi, "turn", "turn")
+gradian = grade = Unit(radian * pi / 200, "gradian", "grad")
+turn = Unit(
+    radian * 2*pi,
+    ["circle", "turn", "revolution", "rev"], "turn")
 sphere = spat = Unit(steradian * 4*pi, "spat", "sp")
 
+rpm = Unit(turn / minute, "revolutions_per_minute", "rpm")
+rps = Unit(turn / second, "revolutions_per_second", "rps")
+
 # % Electricity
 watt_hour = Wh = Unit(watt * hour, 'watt_hour', 'Wh', SI_all)
 amp_hour = ampere_hour = Ah = Unit(ampere * hour, 'amp_hour', 'Ah', SI_all)
 ampere_turn = At = Unit(ampere * turn, "ampere_turn", "At", SI_all)
 
 # % Human
 small_calorie = cal = Unit(
-    4.814 * joule, ["calorie", "large_calorie"], "cal",
+    4.814 * joule, ["calorie", "small_calorie"], "cal",
     info="Energy to heat 1g of water by 1°C."
     " Defined by convention; now regarded as obsolete."
-    " Not to be confused with the large calorie (heats 1kg)."
-)
+    " Not to be confused with the large calorie (heats 1kg).")
 large_calorie = kilocalorie = kcal = Unit(
-    cal * 1000, ["kilocalorie", "small_calorie"], "kcal",
+    cal * 1000, ["kilocalorie", "large_calorie"], "kcal",
     info="Energy to heat 1kg of water by 1°C."
     " Defined by convention; now regarded as obsolete."
     " Not to be confused with the small calorie (heats 1g)."
-    " Often used in food as an alternative to the kilojoule."
-)
+    " Often used in food as an alternative to the kilojoule.")
 bmi = Unit(kilogram / meter**2, "BMI", "BMI")
 
 # A unit of solar irradiation
 met = Unit(
     38.2 * watt / meter**2, "met", "met",
     info='energy per surface area of average person at rest')
 
@@ -48,32 +51,17 @@
 tog = Unit(RSI * 0.1, "tog")
 clo = Unit(tog * 1.55, "clo")
 
 # % Pressure
 
 bar = Unit(1e5 * pascal, "bar", "bar", SI_all)
 atmosphere = atm = Unit(101_325 * pascal, "atmosphere", ["atm", "ata"])
+torr = Unit(atm / 760, "torr", "Torr")
 metre_mercury = meter_mercury = Unit(
     pascal(133_322.387_415),
     "meter_mercury", "mHg", SI_all,
     info="defined by convention")
-mercury = meter_mercury / meter
+mercury = hg = meter_mercury / meter
 sverdrup = Unit(cumec * 1e6, "sverdrup", "Sv")
 
-# % Hartree atomic units
-# where hbar = a_0 = m_e = e = 1
-
-hartree = Unit(
-    joule(4.359_744_722_2071e-18, 8.5e-30),  # CODATA 2018
-    "hartree", "Eₕ")
-bohr_radius = a_0 = Unit(
-    meter(5.291_772_109_03e-11, 8e-21),  # CODATA 2018
-    "bohr_radius", "a_0")
-
-# % Small-scale
-
-micron = micro * meter
-angstrom = Unit(meter(1e-10), "angstrom", "Å")
-barn = Unit(1e-28 * meter**2, "barn", "b", SI_all)
-
 # % Photometric
-nit = Unit(candela / meter**2, 'nit', 'nit')
+nit = Unit(candela / meter**2, 'nit', 'nt', SI_all)
```

### Comparing `noether-1.0.1/noether/catalogue/scientific/si.py` & `noether-1.1/noether/catalogue/scientific/si.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 
 
 def SI_d(unit: Unit):
     return display(SI(unit))
 
 
 # Time
-minute = Unit(second*60, 'minute', ['min'])
-hour = Unit(minute * 60, 'hour', ['hr', 'h'])
-day = Unit(hour * 24, "day", "d")
+minute = min = Unit(second*60, 'minute', ['min'])
+hour = hr = Unit(minute * 60, 'hour', ['hr', 'h'])
+day = da = Unit(hour * 24, "day", "d")
 year_julian = Unit(
     day * 365.25,
     "year", ["yr", "ya"], SI_large,
     info="Julian calendar - assuming leap year every 400 years."
     " Superseded by Gregorian year.")
+julian_month = month = Unit(
+    year_julian / 12, "month", "mo",
+    info="1/12 of a Julian year")
 
 # Rotation
 becquerel = Bq = SI(Unit(frequency, 'becquerel', "Bq", SI_all))
 hertz = Hz = SI_d(Unit(frequency, 'hertz', "Hz", SI_all))
 radian = rad = SI_d(Unit(angle, 'radian', "rad", SI_small))
 steradian = sr = SI_d(Unit(solid_angle, 'steradian', "sr", SI_all))
 
@@ -69,17 +72,13 @@
 
 # GCWM 17
 speed_of_light = c = Unit(299_792_458 * meter / second, "c", "c")
 
 # GCWM 26 (2019 redefinition of the SI base units)
 electron_charge = e = Unit(
     coulomb(1.602_176_634e-19), "electron_charge", "e")
-N_a = 6.022_140_76e23 / mole
-boltzmann_constant = k_B = Unit(
-    1.380649e-23 * joule / kelvin,
-    "boltzmann_constant", 'k_b')
 h = Unit(6.626_070_15e-34 * joule * second, "h", "h")
 hbar = Unit(h / (pi*2), "hbar", "ħ")
 
 
 eV = electronvolt = Unit(electron_charge * volt, "electronvolt", "eV", SI_all)
 gee = standard_gravity * kilogram
```

### Comparing `noether-1.0.1/noether/config.py` & `noether-1.1/noether/config.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/Catalogue.py` & `noether-1.1/noether/core/Catalogue.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         for k, v in catalogue.items():
             self.register(k, v)
 
     def register(self, name: str, value: Unit | Dimension | PrefixSet):
         if isinstance(value, Unit):
             ud = self.units_by_dimension
             ud.setdefault(value.dim, [])
-            if value not in ud[value.dim]:
+            # celsius == kelvin, therefore we check via `is` #71
+            if any(value is v for v in ud[value.dim]):
                 ud[value.dim].append(value)
 
             self.units_by_name[name] = value
             for n in value.names:
                 self.units_by_name[n] = value
             for n in value.symbols:
                 self.units_by_name[n] = value
@@ -87,22 +88,24 @@
     def units(self):
         return set(self.units_by_name.values())
 
     def prefixes(self):
         for prefix_set in self.prefix_sets.values():
             yield from prefix_set
 
-    def all_prefixed_units(self):
-        units: dict[str, Unit] = {}
-
+    def _all_prefixed_units(self):
         for unit in self.units_by_name.values():
-            units.update(unit._namespace())
-            for u in unit.prefixed_units():
-                units.update(u._namespace())
+            yield unit
+            yield from unit.prefixed_units()
 
+    def all_prefixed_units(self):
+        units: dict[str, Unit] = {}
+        for unit in self._all_prefixed_units():
+            for n, u in unit._namespace().items():
+                units.setdefault(n, u)
         return units
 
     def __repr__(self):
         U = len(self.units())
         D = len(self.dimensions.values())
         P = len(list(self.prefixes()))
         return (
```

### Comparing `noether-1.0.1/noether/core/Dimension.py` & `noether-1.1/noether/core/Dimension.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/Measure.py` & `noether-1.1/noether/core/Measure.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 __all__ = ('Measure', )
 
+from typing import Callable, Optional, TypeVar, ClassVar, Generic, TYPE_CHECKING
 from dataclasses import dataclass
 from functools import total_ordering
 import operator
 from sys import version_info
-from typing import Callable, Optional, TypeVar, ClassVar, Generic, TYPE_CHECKING
-from noether.helpers import MeasureValue
+from datetime import date, datetime, timedelta
 
+from ..helpers import MeasureValue
 from ..errors import NoetherError, DimensionError
 from ..config import Config, conf
 from ..display import DISPLAY_REPR_CODE
+
 from .Prefix import Prefix
 from .Dimension import Dimension, dimensionless
 from .MeasureInfo import MeasureInfo
 
 if TYPE_CHECKING:
     from .Unit import Unit
     from .UnitSet import UnitSet
     from .MeasureRelative import MeasureRelative
 
+Time = date | datetime | timedelta
+T = TypeVar('T', int, MeasureValue)
+
 
 OPENLINEAR = Config.register("measure_ignore_dimension", False, """\
 Allow any addition, even between incompatible units
 (eg metre and second)""")
 
 BARENUMBER = Config.register("measure_barenumber", False, """\
 Allow addition and subtraction of bare numbers to units""")
 
 UNCERTAINTY_SHORTHAND = Config.register("uncertainty_display_shorthand", False, """\
 Display e.g. 0.15(2) instead of 0.15 ± 0.02.""")
 
-T = TypeVar('T', int, MeasureValue)
-
 
 @dataclass(
     frozen=True,
     init=False,
     **(dict(slots=True) if version_info.minor >= 10 else dict()),
 )
 @total_ordering
@@ -49,18 +52,21 @@
 
     @property
     def value(self):
         return self._value
 
     def __init__(
         self,
-        value: "Measure[T] | T" = 1,
+        value: "Measure[T] | T | timedelta" = 1,
         stddev: Optional[T] = None,
         dim: Optional[Dimension] = None,
     ):
+        if isinstance(value, timedelta):
+            value = self.from_timedelta(value)
+
         def set(x, v):
             # bypass Frozen
             object.__setattr__(self, x, v)
 
         if isinstance(value, Measure):
             set('_value', value._value)
             set('stddev', value.stddev)
@@ -135,14 +141,28 @@
 
         Config.register(handler.__name__,
                         handler.enabled_by_default,
                         handler.__doc__)
 
         return handler
 
+    @classmethod
+    def from_timedelta(cls, dt: timedelta):
+        from ..catalogue.fundamental import second  # type: ignore
+        return second * dt.total_seconds()
+
+    def to_timedelta(self):
+        from ..catalogue.fundamental import second  # type: ignore
+        if not conf.get(OPENLINEAR):
+            DimensionError.check(
+                self.dim, second.dim,
+                f"Cannot convert to a timedelta."
+                f" Enable conf.{OPENLINEAR} to bypass this.")
+        return timedelta(seconds=float(self/second))
+
     # |~~\ '      |
     # |   ||(~|~~\|/~~|\  /
     # |__/ |_)|__/|\__| \/
     #         |        _/
 
     def _info(self):
         for handler in self.info_handlers:
@@ -185,17 +205,20 @@
 
     #  /~~\                   |     '
     # |  __/~//~\|/~\ /~\ /~/~|~|/~\|/~~
     #  \__/\/_\_/|   |   |\/_ | |   |\__
 
     def __geo(
         self,
-        other: 'Measure[T] | MeasureValue',
+        other: 'Measure[T] | MeasureValue | timedelta',
         op=operator.mul
     ) -> 'Measure':
+        if isinstance(other, timedelta):
+            return op(self, self.from_timedelta(other))
+
         value = self._value
         stddev = None
         dim = self.dim
 
         if isinstance(other, Prefix):
             other = other.value
 
@@ -243,30 +266,36 @@
         if conf.get(OPENLINEAR):
             return
 
         match op:
             case operator.add: oper = "Addition"
             case operator.sub: oper = "Subtraction"
             case operator.mod: oper = "Modulo"
+            case operator.eq: oper = "Comparison"
             case operator.lt: oper = "Comparison"
             case _: oper = "A linear operation"
 
         if isinstance(other, Measure):
-            if self.dim != other.dim:
-                raise DimensionError(
-                    self.dim, other.dim,
-                    f"{oper} only works on units of the same dimension."
-                    f" Enable conf.{OPENLINEAR} to bypass this.")
+            DimensionError.check(
+                self.dim, other.dim,
+                f"{oper} only works on units of the same dimension."
+                f" Enable conf.{OPENLINEAR} to bypass this.")
 
-        elif not conf.get(BARENUMBER):
+        elif self.dim and not conf.get(BARENUMBER):
             raise NoetherError(
                 f"{oper} only works on Measures and Units."
                 f" Enable conf.{BARENUMBER} to bypass this.")
 
-    def __lin(self, other: 'Measure[T] | Dimension | MeasureValue', op: Callable):
+    def __lin(self, other: 'Measure[T] | Dimension | MeasureValue | Time', op: Callable, reverse=False):
+        if isinstance(other, Time):
+            if reverse:
+                return op(other, self.to_timedelta())
+            else:
+                return op(self.to_timedelta(), other)
+
         self.__lin_cmp(other, op)
 
         value = self._value
         stddev = self.stddev
         dim = self.dim
 
         if isinstance(other, Dimension):
@@ -276,60 +305,78 @@
             if self.stddev is None and other.stddev is None:
                 stddev = None
             else:
                 ss = 0 if stddev is None else stddev
                 so = 0 if other.stddev is None else other.stddev
                 stddev = (ss**2 + so**2) ** 0.5
         else:
-            value = op(self._value, other)
+            if reverse:
+                value = op(other, self._value)
+            else:
+                value = op(self._value, other)
 
         return Measure(value, stddev, dim)
 
     def __add__(self, other): return self.__lin(other, operator.add)
     def __radd__(self, other): return self.__lin(other, operator.add)
     def __sub__(self, other): return self.__lin(other, operator.sub)
+
+    def __rsub__(self, other):
+        return self.__lin(other, operator.sub, reverse=True)
+
     def __mod__(self, other): return self.__lin(other, operator.mod)
 
     # Equality and ordering
 
+    @staticmethod
+    def _extract_dim(v: 'Measure | MeasureValue') -> Dimension:
+        return v.dim if isinstance(v, Measure) else Dimension()  # type: ignore
+
+    @staticmethod
+    def _extract_value(v: 'Measure | MeasureValue') -> MeasureValue:
+        return v._value if isinstance(v, Measure) else v  # type: ignore
+
     def __eq__(self, other):
-        if isinstance(other, Measure):
-            if other.dim != self.dim and not conf.get(OPENLINEAR):
-                return False
-            return self._value == other._value
+        if self._extract_dim(other) != self.dim and not conf.get(OPENLINEAR):
+            return False
+        return self._value == self._extract_value(other)
 
     def __lt__(self, other):
         self.__lin_cmp(other, operator.lt)
-        if isinstance(other, Measure):
-            return self._value < other._value
+        return self._value < self._extract_value(other)
 
     #  /~~       |               |~~\ '      |
     # |  |   |(~~|~/~\|/~\ /~\   |   ||(~|~~\|/~~|\  /
     #  \__\_/|_) | \_/|   |   |  |__/ |_)|__/|\__| \/
     #                                    |        _/
 
-    def __matmul__(self, unit_or_unitset: 'Unit | UnitSet'):
+    def __matmul__(self, display_with: 'Unit | UnitSet'):
         from .Unit import Unit
         from .UnitSet import UnitSet
 
-        if isinstance(unit_or_unitset, UnitSet):
-            unit = unit_or_unitset.unit_for_dimension(self.dim)
+        if isinstance(display_with, UnitSet):
+            unit = display_with.unit_for_dimension(self.dim)
             if unit is None:
                 return self
             return self @ unit
 
-        if not isinstance(unit_or_unitset, Unit):
+        if not isinstance(display_with, Unit):
             raise TypeError('Can only use @ (display relative to) on a Unit.')
 
         # HACK
         # We are intentionally deferring dimension checks.
         # This is because @ binds more tightly than &, * and /,
         # and so therefore until displayed we will
         # override these such that eg     a  @  b  /  c
         #               which binds as   (a  @  b) /  c
         # effortlessly becomes equiv to   a  @ (b  /  c)
 
-        return MeasureRelative(self, unit_or_unitset)
+        return MeasureRelative(self, display_with)
+
+    def __rmatmul__(self, display_this: 'Measure | timedelta'):
+        if isinstance(display_this, timedelta):
+            display_this = self.from_timedelta(display_this)
+        return Measure(display_this) @ self
 
 
 # Avoid import loops
 from .MeasureRelative import MeasureRelative  # noqa
```

### Comparing `noether-1.0.1/noether/core/MeasureRelative.py` & `noether-1.1/noether/core/MeasureRelative.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from typing import TYPE_CHECKING
 
-from noether.errors import DimensionError
-from noether.config import conf
+from ..errors import DimensionError
+from ..config import conf
 from .Measure import OPENLINEAR, Measure
 
 if TYPE_CHECKING:
     from .Unit import Unit
 
 
 class MeasureRelative(Measure):
@@ -17,23 +17,28 @@
     '''
 
     __slots__ = ('_value', 'stddev', 'dim', 'unit')
     unit: 'Unit'
 
     @property
     def value(self):
-        return self._value / self.unit._value
+        from .units import AffineUnit
+        value = self._value
+        if isinstance(self.unit, AffineUnit):
+            value -= self.unit.zero_point._value
+
+        return value / self.unit._value
 
     def __init__(self, measure: Measure, unit: 'Unit'):
         Measure.__init__(self, measure)
         object.__setattr__(self, 'unit', unit)
 
     def display_unit(self):
-        if self.dim != self.unit.dim and not conf.get(OPENLINEAR):
-            raise DimensionError(
+        if not conf.get(OPENLINEAR):
+            DimensionError.check(
                 self.dim, self.unit.dim,
                 f"To use @ on units with different dimensions, enable conf.{OPENLINEAR}.")
 
         return self.unit
 
     # HACK: syntactic sugar such that @ "binds looser"
```

### Comparing `noether-1.0.1/noether/core/Prefix.py` & `noether-1.1/noether/core/Prefix.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/Unit.py` & `noether-1.1/noether/core/Unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import timedelta
 from itertools import chain
 from noether.helpers import Rational, Real, removeprefix
 
 from ..errors import NoetherError
 from ..config import conf
 from ..display import DISPLAY_REPR_CODE, canonical_number
-from .Prefix import Prefix, PrefixSet
+from .Prefix import PrefixSet
 from .Dimension import Dimension
 from .Measure import Measure, UNCERTAINTY_SHORTHAND
 
 
 class Unit(Measure):
     __slots__ = '_value stddiv dim symbols names prefixes info'.split()
 
@@ -28,19 +28,14 @@
         self,
         measure: Real | Measure | Dimension | timedelta,
         names: str | list[str] | None = None,
         symbols: str | list[str] | None = None,
         prefixes: PrefixSet | None = None,
         info: str | None = None,
     ):
-        # TODO: this should be far more thoroughly supported
-        if isinstance(measure, timedelta):
-            from ..catalogue.fundamental import second  # noqa
-            measure = second * measure.total_seconds()
-
         if isinstance(measure, Dimension):
             measure = Measure(dim=measure)
         super().__init__(measure)
 
         def setattr(x, v):
             # bypass Frozen
             object.__setattr__(self, x, v)
@@ -150,22 +145,28 @@
             del json['stddev']
         if self.prefixes:
             json['prefixes'] = self.prefixes.name.split(' + ')
         if self.info:
             json['info'] = self.info
         return json
 
-    def _repr_measure(self, measure: Measure):
-        val = measure._value / self._value
-        stddev = None
-        if measure.stddev is not None:
-            stddev = measure.stddev / self._value
+    def _repr_measure(self, measure: Real | Measure):
+        if isinstance(measure, Measure):
+            val = measure._value / self._value
+            stddev = None
+            if measure.stddev is not None:
+                stddev = measure.stddev / self._value
+        else:
+            val: Real = measure  # type: ignore
+            stddev = None
 
         v = canonical_number(val, stddev, conf.get(UNCERTAINTY_SHORTHAND))
-        return f'{v} {self.symbol}'
+        if self.dim or self.symbols:
+            v += ' ' + self.symbol
+        return v
 
     def __and__(self, unit: 'Unit'):
         from .units.LinearUnit import LinearUnit
         return LinearUnit([self, unit])
 
 
 # Avoid import loops
```

### Comparing `noether-1.0.1/noether/core/UnitSet.py` & `noether-1.1/noether/core/UnitSet.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/_DisplayHandler.py` & `noether-1.1/noether/core/_DisplayHandler.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/units/AffineUnit.py` & `noether-1.1/noether/core/units/AffineUnit.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 
     def __init__(
         self,
         unit: Measure,
         zero_point: Measure,
         names: list[str] | str | None = None,
         symbols: list[str] | str | None = None,
+        info: str | None = None,
     ):
-        if unit.dim != zero_point.dim:
-            raise DimensionError(zero_point.dim, unit.dim,
-                                 '(AffineUnit creation)')
+        DimensionError.check(zero_point.dim, unit.dim, '(AffineUnit creation)')
         object.__setattr__(self, 'zero_point', zero_point)
-        Unit.__init__(self, unit, names, symbols)
+        Unit.__init__(
+            self, unit,
+            names=names, symbols=symbols, info=info)
 
     def __call__(self, value: Real, stddev: Real | None = None):
         return Measure.__call__(self, value, stddev) + self.zero_point
 
     def __and__(self, _: Unit):
         raise IncompatibleUnitError(
             'An affine unit {self} cannot be composed with other units!')
@@ -33,8 +34,8 @@
 
     __rand__ = __and__
 
     def _repr_measure(self, measure: Measure):
         return Unit._repr_measure(self, measure - self.zero_point)
 
     def _json_extras(self):
-        return {'zero_point': self.zero_point / self._value}
+        return {'zero_point': self.zero_point._value}
```

### Comparing `noether-1.0.1/noether/core/units/GeometricUnit.py` & `noether-1.1/noether/core/units/GeometricUnit.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/units/LinearUnit.py` & `noether-1.1/noether/core/units/LinearUnit.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/core/units/PrefixedUnit.py` & `noether-1.1/noether/core/units/PrefixedUnit.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/display.py` & `noether-1.1/noether/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Functions for transforming various numbers into strings.
 
 Handles Unicode.
 '''
 
 from decimal import Decimal
 from fractions import Fraction
-from noether.helpers import Real, removeprefix
+from math import ceil, log10
+from noether.helpers import Real, removeprefix, removesuffix
 
 from .config import Config, conf
 
 DISPLAY_UNICODE_SYMBOLS = Config.register("display_unicode_symbols", True, '''\
 Use Unicode symbols eg ± instead of +-.
 ''')
 
@@ -81,23 +82,31 @@
 
     return f'{ai}.{af}({bf})'
 
 
 def scinot(number: Real, digits: int | None = None):
     notation = format(number, f'.{digits}e' if digits is not None else 'e')
     num, exp = notation.split('e')
+
+    while num.endswith('0'):
+        num = num[:-1]
+    num = removesuffix(num, '.')
+
     sign = '' if exp.startswith('+') else '-'
     exp = int(exp[1:])
     return f'{num}e{sign}{exp}'
 
 
 def _fmt(number: Real):
+    if number == 0:
+        return '0'
+    mag = log10(abs(number))
     DIGITS: int = conf.get(DISPLAY_DIGITS)
-    n = str(round(number, DIGITS))
-    if len(n) > DIGITS:
+    n = str(round(number, DIGITS - ceil(mag)))
+    if 'e' in n or (len(n) > DIGITS and not -3 < mag < 4):
         return scinot(number)
 
     m = ''
     if '.' in n:
         n, m = n.split('.')
         m = '' if m == '0' else '.'+m
     UNDERSCORE_DIGITS = conf.get(DISPLAY_UNDERSCORE_AFTER)
```

### Comparing `noether-1.0.1/noether/errors.py` & `noether-1.1/noether/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,29 @@
 class NoetherError(Exception):
     'Common error used in Noether.'
 
 
 class DimensionError(NoetherError):
     'Dimensions do not match.'
 
-    args: 'tuple[Dimension, Dimension, str]'
+    args: 'tuple[Dimension, Dimension, str | None]'
 
     def __init__(self, dim1: 'Dimension', dim2: 'Dimension', message: str | None = None):
         super().__init__(dim1, dim2, message)
 
+    @classmethod
+    def check(cls, dim1: 'Dimension', dim2: 'Dimension', message: str | None = None):
+        # ensure not dimensionless - those are usually okay
+        if dim1 != dim2:
+            raise cls(dim1, dim2, message)
+
     def __str__(self):
         dim1, dim2, msg = self.args
         message = f'Dimensions {dim1} and {dim2} do not match.'
-        if message is not None:
+        if msg is not None:
             message += ' ' + msg
         return message
 
 
 class UnitError(NoetherError):
     'Problem with creating a unit.'
```

### Comparing `noether-1.0.1/noether/gnu.py` & `noether-1.1/noether/gnu.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether/helpers.py` & `noether-1.1/noether/helpers.py`

 * *Files identical despite different names*

### Comparing `noether-1.0.1/noether.egg-info/PKG-INFO` & `noether-1.1/noether.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: noether
-Version: 1.0.1
+Version: 1.1
 Summary: Work with physical measurements and constants
 Home-page: https://github.com/yunruse/noether
 Author: Mia yun Ruse
 Author-email: mia@yunru.se
 Keywords: physics unit measure constant measurement uncertainty
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved
 Classifier: Topic :: Scientific/Engineering
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Noether 1.0.1 (in development)
+# Noether
+`523 units, 60 prefixes`
 
 [![PyPI](https://img.shields.io/pypi/v/noether?color=blue)](https://pypi.org/packages/noether)
 
 **Noether** is a unit-enriched Python package, akin to Wolfram Alpha or gnu `units`. It has a large (and expanding) catalogue of up-to-date units and constants, allowing code to be written directly in the units they are concerned with while also ensuring e.g. you don't mistakenly add an energy to a length.
 
 Just grab Python 3.10 or later and `pip install noether` to run!
 
@@ -31,14 +32,16 @@
 
 ```sh
 $ alias noe='python -im noether'
 $ noe marathon
 marathon  # length, 42195 m, Race length based on Greek legend, set by convention from 1908 Summer Olympics
 $ noether 23degC @ degF
 73.4 °F  # temperature
+$ noether 'horsepower @ dB(kW)'
+-1.33418061 dB(kW)  # power, 0.73549875 kW
 ```
 
 The CLI allows a few niceties such as slightly terser syntax, but otherwise behaves identically to Python:
 
 ```sh
 $ noether 5cm @ in --value
 1.9685039370078738
@@ -53,15 +56,15 @@
 ```py
 >>> display(inch)
 >>> 5 * cm
 >>> mile
 mile  # length, 63360 in
 ```
 
-Units can propagate uncertainty automatically under most operations:
+Units propagate uncertainty automatically under most operations:
 
 ```py
 >>> m(5, 0.1)**3
 125 ± 7.5 m**3  # volume
 ```
 
 You can define your own units and dimensions:
```

### Comparing `noether-1.0.1/noether.egg-info/SOURCES.txt` & `noether-1.1/noether.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 noether/gnu.py
 noether/helpers.py
 noether.egg-info/PKG-INFO
 noether.egg-info/SOURCES.txt
 noether.egg-info/dependency_links.txt
 noether.egg-info/top_level.txt
 noether/catalogue/__init__.py
+noether/catalogue/data.py
 noether/catalogue/dimensions.py
 noether/catalogue/fundamental.py
 noether/catalogue/prefixes.py
 noether/catalogue/conventional/__init__.py
+noether/catalogue/conventional/avourdupois.py
 noether/catalogue/conventional/conventional.py
-noether/catalogue/conventional/imperial.py
 noether/catalogue/conventional/typographic.py
 noether/catalogue/historic/__init__.py
 noether/catalogue/historic/ancient_greek.units.py
 noether/catalogue/historic/ancient_greek_.py
 noether/catalogue/historic/mts.units.py
 noether/catalogue/historic/mts_.py
 noether/catalogue/historic/scientific.py
@@ -39,27 +40,28 @@
 noether/catalogue/info/spectrum.py
 noether/catalogue/info/unit_context.py
 noether/catalogue/info/unit_value.py
 noether/catalogue/scientific/CODATA.py
 noether/catalogue/scientific/__init__.py
 noether/catalogue/scientific/astronomy.py
 noether/catalogue/scientific/cgs.py
-noether/catalogue/scientific/climate.py
 noether/catalogue/scientific/constants.py
-noether/catalogue/scientific/data.py
-noether/catalogue/scientific/essential.py
+noether/catalogue/scientific/earth.py
+noether/catalogue/scientific/micro.py
+noether/catalogue/scientific/misc.py
 noether/catalogue/scientific/si.py
 noether/core/Catalogue.py
 noether/core/Dimension.py
 noether/core/Measure.py
 noether/core/MeasureInfo.py
 noether/core/MeasureRelative.py
 noether/core/Prefix.py
 noether/core/Unit.py
 noether/core/UnitSet.py
 noether/core/_DisplayHandler.py
 noether/core/__init__.py
 noether/core/units/AffineUnit.py
 noether/core/units/GeometricUnit.py
 noether/core/units/LinearUnit.py
+noether/core/units/LogarithmicUnit.py
 noether/core/units/PrefixedUnit.py
 noether/core/units/__init__.py
```

### Comparing `noether-1.0.1/setup.py` & `noether-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 packages = setuptools.find_packages()
 
 setuptools.setup(
     name="noether",
-    version="1.0.1",
+    version="1.1",
     author="Mia yun Ruse",
     author_email="mia@yunru.se",
     description="Work with physical measurements and constants",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yunruse/noether",
     packages=packages,
```

