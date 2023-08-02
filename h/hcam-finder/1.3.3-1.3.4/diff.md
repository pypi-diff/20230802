# Comparing `tmp/hcam_finder-1.3.3.tar.gz` & `tmp/hcam_finder-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcam_finder-1.3.3.tar", last modified: Thu Jul 27 22:12:18 2023, max compression
+gzip compressed data, was "hcam_finder-1.3.4.tar", last modified: Wed Aug  2 08:28:17 2023, max compression
```

## Comparing `hcam_finder-1.3.3.tar` & `hcam_finder-1.3.4.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607489 hcam_finder-1.3.3/
--rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/AUTHORS.rst
--rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/CONTRIBUTING.rst
--rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/HISTORY.rst
--rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/LICENSE
--rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.3/MANIFEST.in
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-27 22:12:18.607561 hcam_finder-1.3.3/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.3/README.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.597465 hcam_finder-1.3.3/docs/
--rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/docs/Makefile
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.594638 hcam_finder-1.3.3/docs/_build/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.594742 hcam_finder-1.3.3/docs/_build/html/
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.599620 hcam_finder-1.3.3/docs/_build/html/_images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.3/docs/_build/html/_images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/_build/html/_images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/_build/html/_images/main.png
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.600475 hcam_finder-1.3.3/docs/_build/html/_static/
--rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/file.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/minus.png
--rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.3/docs/_build/html/_static/plus.png
--rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.3/docs/conf.py
--rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.3/docs/hcam_finder.rst
--rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/hipercam.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.602696 hcam_finder-1.3.3/docs/images/
--rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/images/compo.png
--rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/images/inst.png
--rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.3/docs/images/main.png
--rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/index.rst
--rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/docs/make.bat
--rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.3/docs/modules.rst
--rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/ultracam.rst
--rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/docs/ultraspec.rst
--rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/docs/usage.rst
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.604174 hcam_finder-1.3.3/hcam_finder/
--rw-r--r--   0 sl         (501) staff       (20)      150 2023-07-27 22:12:08.000000 hcam_finder-1.3.3/hcam_finder/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)     2379 2023-07-24 10:46:18.000000 hcam_finder-1.3.3/hcam_finder/config.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.606811 hcam_finder-1.3.3/hcam_finder/data/
--rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.3/hcam_finder/data/Lato-Black.ttf
--rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.3/hcam_finder/data/Lato-Regular.ttf
--rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.3/hcam_finder/data/README.rst
--rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/data/config
--rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/data/configspec.ini
--rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.3/hcam_finder/data/guider_hole_arcseconds.txt
--rw-r--r--   0 sl         (501) staff       (20)    21032 2023-07-24 10:01:37.000000 hcam_finder-1.3.3/hcam_finder/finders.py
--rw-r--r--   0 sl         (501) staff       (20)     2804 2023-07-24 10:43:37.000000 hcam_finder-1.3.3/hcam_finder/finding_chart.py
--rw-r--r--   0 sl         (501) staff       (20)    10394 2023-07-27 22:08:20.000000 hcam_finder-1.3.3/hcam_finder/hcam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.3/hcam_finder/panstarrs.py
--rw-r--r--   0 sl         (501) staff       (20)     2358 2023-07-24 10:46:20.000000 hcam_finder-1.3.3/hcam_finder/shapes.py
--rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.3/hcam_finder/skyview.py
--rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.3/hcam_finder/ucam_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.3/hcam_finder/uspec_finder.py
--rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.3/hcam_finder/ztf.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.604843 hcam_finder-1.3.3/hcam_finder.egg-info/
--rw-r--r--   0 sl         (501) staff       (20)     3683 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/PKG-INFO
--rw-r--r--   0 sl         (501) staff       (20)     1288 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/SOURCES.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/dependency_links.txt
--rw-r--r--   0 sl         (501) staff       (20)        1 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/not-zip-safe
--rw-r--r--   0 sl         (501) staff       (20)       55 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/requires.txt
--rw-r--r--   0 sl         (501) staff       (20)       12 2023-07-27 22:12:18.000000 hcam_finder-1.3.3/hcam_finder.egg-info/top_level.txt
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607163 hcam_finder-1.3.3/scripts/
--rw-r--r--   0 sl         (501) staff       (20)    12541 2023-07-24 14:23:43.000000 hcam_finder-1.3.3/scripts/hfinder
--rw-r--r--   0 sl         (501) staff       (20)    10843 2023-07-24 14:23:41.000000 hcam_finder-1.3.3/scripts/ufinder
--rw-r--r--   0 sl         (501) staff       (20)    11348 2023-07-24 14:23:57.000000 hcam_finder-1.3.3/scripts/usfinder
--rw-r--r--   0 sl         (501) staff       (20)      312 2023-07-27 22:12:18.607791 hcam_finder-1.3.3/setup.cfg
--rw-r--r--   0 sl         (501) staff       (20)     1858 2023-07-27 22:12:08.000000 hcam_finder-1.3.3/setup.py
-drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-07-27 22:12:18.607387 hcam_finder-1.3.3/tests/
--rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/tests/__init__.py
--rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.3/tests/test_hcam_finder.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.786743 hcam_finder-1.3.4/
+-rw-r--r--   0 sl         (501) staff       (20)      166 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/AUTHORS.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3291 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 sl         (501) staff       (20)       89 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/HISTORY.rst
+-rw-r--r--   0 sl         (501) staff       (20)     1077 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/LICENSE
+-rw-r--r--   0 sl         (501) staff       (20)      302 2017-11-14 10:44:10.000000 hcam_finder-1.3.4/MANIFEST.in
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-08-02 08:28:17.786816 hcam_finder-1.3.4/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     2663 2021-08-05 13:35:16.000000 hcam_finder-1.3.4/README.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.777300 hcam_finder-1.3.4/docs/
+-rw-r--r--   0 sl         (501) staff       (20)     6782 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/docs/Makefile
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.774277 hcam_finder-1.3.4/docs/_build/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.774382 hcam_finder-1.3.4/docs/_build/html/
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.778785 hcam_finder-1.3.4/docs/_build/html/_images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-05-17 08:38:05.000000 hcam_finder-1.3.4/docs/_build/html/_images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.4/docs/_build/html/_images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.4/docs/_build/html/_images/main.png
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.779700 hcam_finder-1.3.4/docs/_build/html/_static/
+-rw-r--r--   0 sl         (501) staff       (20)      286 2022-07-14 07:38:21.000000 hcam_finder-1.3.4/docs/_build/html/_static/file.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sl         (501) staff       (20)       90 2022-07-14 07:38:21.000000 hcam_finder-1.3.4/docs/_build/html/_static/plus.png
+-rwxr-xr-x   0 sl         (501) staff       (20)     8468 2021-01-18 16:26:27.000000 hcam_finder-1.3.4/docs/conf.py
+-rw-r--r--   0 sl         (501) staff       (20)     1714 2023-05-19 12:39:10.000000 hcam_finder-1.3.4/docs/hcam_finder.rst
+-rw-r--r--   0 sl         (501) staff       (20)    27352 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/docs/hipercam.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.782314 hcam_finder-1.3.4/docs/images/
+-rw-r--r--   0 sl         (501) staff       (20)   438400 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/docs/images/compo.png
+-rw-r--r--   0 sl         (501) staff       (20)    30314 2017-12-18 14:51:55.000000 hcam_finder-1.3.4/docs/images/inst.png
+-rw-r--r--   0 sl         (501) staff       (20)    91154 2017-12-18 14:51:55.000000 hcam_finder-1.3.4/docs/images/main.png
+-rw-r--r--   0 sl         (501) staff       (20)      468 2021-01-18 16:44:46.000000 hcam_finder-1.3.4/docs/index.rst
+-rw-r--r--   0 sl         (501) staff       (20)     6469 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/docs/make.bat
+-rw-r--r--   0 sl         (501) staff       (20)       70 2023-05-19 12:39:10.000000 hcam_finder-1.3.4/docs/modules.rst
+-rw-r--r--   0 sl         (501) staff       (20)     5650 2021-01-18 16:44:46.000000 hcam_finder-1.3.4/docs/ultracam.rst
+-rw-r--r--   0 sl         (501) staff       (20)       46 2021-01-18 16:44:46.000000 hcam_finder-1.3.4/docs/ultraspec.rst
+-rw-r--r--   0 sl         (501) staff       (20)     4055 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/docs/usage.rst
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.783842 hcam_finder-1.3.4/hcam_finder/
+-rw-r--r--   0 sl         (501) staff       (20)      150 2023-08-02 08:28:06.000000 hcam_finder-1.3.4/hcam_finder/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)     2506 2023-08-02 08:26:44.000000 hcam_finder-1.3.4/hcam_finder/config.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.786108 hcam_finder-1.3.4/hcam_finder/data/
+-rwxr-xr-x   0 sl         (501) staff       (20)   114588 2017-05-05 16:12:30.000000 hcam_finder-1.3.4/hcam_finder/data/Lato-Black.ttf
+-rwxr-xr-x   0 sl         (501) staff       (20)   120196 2017-05-05 16:12:30.000000 hcam_finder-1.3.4/hcam_finder/data/Lato-Regular.ttf
+-rw-r--r--   0 sl         (501) staff       (20)      257 2017-02-12 22:30:12.000000 hcam_finder-1.3.4/hcam_finder/data/README.rst
+-rw-r--r--   0 sl         (501) staff       (20)     3387 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/hcam_finder/data/config
+-rw-r--r--   0 sl         (501) staff       (20)     4062 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/hcam_finder/data/configspec.ini
+-rw-r--r--   0 sl         (501) staff       (20)     2966 2020-12-04 18:50:57.000000 hcam_finder-1.3.4/hcam_finder/data/guider_hole_arcseconds.txt
+-rw-r--r--   0 sl         (501) staff       (20)    21032 2023-07-24 10:01:37.000000 hcam_finder-1.3.4/hcam_finder/finders.py
+-rw-r--r--   0 sl         (501) staff       (20)     2931 2023-08-02 08:27:03.000000 hcam_finder-1.3.4/hcam_finder/finding_chart.py
+-rw-r--r--   0 sl         (501) staff       (20)    10394 2023-07-28 00:17:57.000000 hcam_finder-1.3.4/hcam_finder/hcam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     5618 2021-02-22 09:06:04.000000 hcam_finder-1.3.4/hcam_finder/panstarrs.py
+-rw-r--r--   0 sl         (501) staff       (20)     2358 2023-07-24 10:46:20.000000 hcam_finder-1.3.4/hcam_finder/shapes.py
+-rw-r--r--   0 sl         (501) staff       (20)     4186 2020-12-04 18:50:57.000000 hcam_finder-1.3.4/hcam_finder/skyview.py
+-rw-r--r--   0 sl         (501) staff       (20)     3050 2021-01-21 12:23:25.000000 hcam_finder-1.3.4/hcam_finder/ucam_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     2394 2021-01-18 16:44:46.000000 hcam_finder-1.3.4/hcam_finder/uspec_finder.py
+-rw-r--r--   0 sl         (501) staff       (20)     4764 2021-02-12 09:10:54.000000 hcam_finder-1.3.4/hcam_finder/ztf.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.784494 hcam_finder-1.3.4/hcam_finder.egg-info/
+-rw-r--r--   0 sl         (501) staff       (20)     3683 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/PKG-INFO
+-rw-r--r--   0 sl         (501) staff       (20)     1288 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 sl         (501) staff       (20)        1 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/not-zip-safe
+-rw-r--r--   0 sl         (501) staff       (20)       55 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/requires.txt
+-rw-r--r--   0 sl         (501) staff       (20)       12 2023-08-02 08:28:17.000000 hcam_finder-1.3.4/hcam_finder.egg-info/top_level.txt
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.786426 hcam_finder-1.3.4/scripts/
+-rw-r--r--   0 sl         (501) staff       (20)    12541 2023-07-24 14:23:43.000000 hcam_finder-1.3.4/scripts/hfinder
+-rw-r--r--   0 sl         (501) staff       (20)    10843 2023-07-24 14:23:41.000000 hcam_finder-1.3.4/scripts/ufinder
+-rw-r--r--   0 sl         (501) staff       (20)    11348 2023-07-24 14:23:57.000000 hcam_finder-1.3.4/scripts/usfinder
+-rw-r--r--   0 sl         (501) staff       (20)      312 2023-08-02 08:28:17.787047 hcam_finder-1.3.4/setup.cfg
+-rw-r--r--   0 sl         (501) staff       (20)     1858 2023-08-02 08:28:06.000000 hcam_finder-1.3.4/setup.py
+drwxr-xr-x   0 sl         (501) staff       (20)        0 2023-08-02 08:28:17.786643 hcam_finder-1.3.4/tests/
+-rw-r--r--   0 sl         (501) staff       (20)       24 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/tests/__init__.py
+-rw-r--r--   0 sl         (501) staff       (20)      647 2017-02-11 14:24:09.000000 hcam_finder-1.3.4/tests/test_hcam_finder.py
```

### Comparing `hcam_finder-1.3.3/CONTRIBUTING.rst` & `hcam_finder-1.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/LICENSE` & `hcam_finder-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/PKG-INFO` & `hcam_finder-1.3.4/hcam_finder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: hcam_finder
-Version: 1.3.3
+Name: hcam-finder
+Version: 1.3.4
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.4.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.3/README.rst` & `hcam_finder-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/Makefile` & `hcam_finder-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/_build/html/_images/compo.png` & `hcam_finder-1.3.4/docs/_build/html/_images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/_build/html/_images/inst.png` & `hcam_finder-1.3.4/docs/_build/html/_images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/_build/html/_images/main.png` & `hcam_finder-1.3.4/docs/_build/html/_images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/conf.py` & `hcam_finder-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/hcam_finder.rst` & `hcam_finder-1.3.4/docs/hcam_finder.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/hipercam.rst` & `hcam_finder-1.3.4/docs/hipercam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/images/compo.png` & `hcam_finder-1.3.4/docs/images/compo.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/images/inst.png` & `hcam_finder-1.3.4/docs/images/inst.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/images/main.png` & `hcam_finder-1.3.4/docs/images/main.png`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/make.bat` & `hcam_finder-1.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/ultracam.rst` & `hcam_finder-1.3.4/docs/ultracam.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/docs/usage.rst` & `hcam_finder-1.3.4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/config.py` & `hcam_finder-1.3.4/hcam_finder/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # read in config
 from __future__ import absolute_import, print_function, division
 import configobj
-import importlib
 import os
 import validate
 
+try:
+    from importlib import resources as importlib_resources
+except Exception:
+    # backport for python 3.6
+    import importlib_resources
+
 
 def check_user_dir(g, app_name="hfinder"):
     """
     Check directories exist for saving apps/configs etc. Create if not.
     """
     direc = os.path.expanduser("~/." + app_name)
     if not os.path.exists(direc):
@@ -19,26 +24,26 @@
 
 
 def load_config(g, app_name="hfinder", env_var="HCAM_FINDER_CONF"):
     """
     Populate application level globals from config file
     """
     configspec_file = str(
-        importlib.resources.files("hcam_finder") / "data/configspec.ini"
+        importlib_resources.files("hcam_finder") / "data/configspec.ini"
     )
     # try and load config file.
     # look in the following locations in order
     # - HCAM_FINDER_CONF environment variable
     # - ~/.hfinder directory
     # - package resources
     paths = []
     if env_var in os.environ:
         paths.append(os.environ[env_var])
     paths.append(os.path.expanduser("~/." + app_name))
-    resource_dir = str(importlib.resources.files("hcam_finder") / "data")
+    resource_dir = str(importlib_resources.files("hcam_finder") / "data")
     paths.append(resource_dir)
 
     # now load config file
     config = configobj.ConfigObj({}, configspec=configspec_file)
     for loc in paths:
         try:
             with open(os.path.join(loc, "config")) as source:
@@ -58,15 +63,15 @@
 
 
 def write_config(g, app_name="hfinder"):
     """
     Dump application level globals to config file
     """
     configspec_file = str(
-        importlib.resources.files("hcam_finder") / "data/configspec.ini"
+        importlib_resources.files("hcam_finder") / "data/configspec.ini"
     )
 
     config = configobj.ConfigObj({}, configspec=configspec_file)
     config.update(g.cpars)
     config.filename = os.path.expanduser("~/.{}/config".format(app_name))
     if not os.path.exists(config.filename):
         try:
```

### Comparing `hcam_finder-1.3.3/hcam_finder/data/Lato-Black.ttf` & `hcam_finder-1.3.4/hcam_finder/data/Lato-Black.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/data/Lato-Regular.ttf` & `hcam_finder-1.3.4/hcam_finder/data/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/data/config` & `hcam_finder-1.3.4/hcam_finder/data/config`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/data/configspec.ini` & `hcam_finder-1.3.4/hcam_finder/data/configspec.ini`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/data/guider_hole_arcseconds.txt` & `hcam_finder-1.3.4/hcam_finder/data/guider_hole_arcseconds.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/finders.py` & `hcam_finder-1.3.4/hcam_finder/finders.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/finding_chart.py` & `hcam_finder-1.3.4/hcam_finder/finding_chart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, absolute_import, unicode_literals, division
-import importlib
 import six
 from os.path import expanduser
 
+try:
+    from importlib import resources as importlib_resources
+except Exception:
+    # backport for python 3.6
+    import importlib_resources
+
 if not six.PY3:
     import tkFileDialog as filedialog
 else:
     from tkinter import filedialog
 
 from . import __version__ as version
 
@@ -72,15 +77,15 @@
             dec=dec,
             pa=pa,
             wins=wins,
             version=version,
         )
     )
     font_size = 5
-    font_file = importlib.resources.files("hcam_finder") / "data/Lato-Regular.ttf"
+    font_file = importlib_resources.files("hcam_finder") / "data/Lato-Regular.ttf"
     text_x = 0.0
     while text_x / width < 0.4:
         font_size += 1
         font = ImageFont.truetype(str(font_file), font_size)
         _, _, text_x, text_y = max((font.getbbox(txt) for txt in info_msg.splitlines()))
 
     nlines = len(info_msg.splitlines()) + 1
```

### Comparing `hcam_finder-1.3.3/hcam_finder/hcam_finder.py` & `hcam_finder-1.3.4/hcam_finder/hcam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/panstarrs.py` & `hcam_finder-1.3.4/hcam_finder/panstarrs.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/shapes.py` & `hcam_finder-1.3.4/hcam_finder/shapes.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/skyview.py` & `hcam_finder-1.3.4/hcam_finder/skyview.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/ucam_finder.py` & `hcam_finder-1.3.4/hcam_finder/ucam_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/uspec_finder.py` & `hcam_finder-1.3.4/hcam_finder/uspec_finder.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder/ztf.py` & `hcam_finder-1.3.4/hcam_finder/ztf.py`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/hcam_finder.egg-info/PKG-INFO` & `hcam_finder-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: hcam-finder
-Version: 1.3.3
+Name: hcam_finder
+Version: 1.3.4
 Summary: Observation planning and finding charts for HiPerCAM
 Home-page: https://github.com/HiPERCAM/hcam_finder
-Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz
+Download-URL: https://github.com/HiPERCAM/hcam_finder/archive/v1.3.4.tar.gz
 Author: Stuart Littlefair
 Author-email: s.littlefair@shef.ac.uk
 License: MIT license
 Keywords: hcam_finder
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcam_finder-1.3.3/hcam_finder.egg-info/SOURCES.txt` & `hcam_finder-1.3.4/hcam_finder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/scripts/hfinder` & `hcam_finder-1.3.4/scripts/hfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/scripts/ufinder` & `hcam_finder-1.3.4/scripts/ufinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/scripts/usfinder` & `hcam_finder-1.3.4/scripts/usfinder`

 * *Files identical despite different names*

### Comparing `hcam_finder-1.3.3/setup.py` & `hcam_finder-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,36 +7,36 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["ginga", "astropy", "six", "pillow", "configobj", "hcam_widgets>=1.1.1"]
+requirements = ["ginga", "astropy", "six", "pillow", "configobj", "hcam_widgets>=1.1.2"]
 
 test_requirements = [
     # TODO: put package test requirements here
 ]
 
 # Treat everything in scripts except README.rst as a script to be installed
 scripts = [
     fname
     for fname in glob.glob(os.path.join("scripts", "*"))
     if os.path.basename(fname) != "README.rst"
 ]
 
 setup(
     name="hcam_finder",
-    version="1.3.3",
+    version="1.3.4",
     description="Observation planning and finding charts for HiPerCAM",
     long_description=readme + "\n\n" + history,
     author="Stuart Littlefair",
     author_email="s.littlefair@shef.ac.uk",
     url="https://github.com/HiPERCAM/hcam_finder",
-    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.3.tar.gz",
+    download_url="https://github.com/HiPERCAM/hcam_finder/archive/v1.3.4.tar.gz",
     packages=[
         "hcam_finder",
     ],
     package_dir={"hcam_finder": "hcam_finder"},
     include_package_data=True,
     scripts=scripts,
     install_requires=requirements,
```

### Comparing `hcam_finder-1.3.3/tests/test_hcam_finder.py` & `hcam_finder-1.3.4/tests/test_hcam_finder.py`

 * *Files identical despite different names*

