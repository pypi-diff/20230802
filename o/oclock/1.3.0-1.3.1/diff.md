# Comparing `tmp/oclock-1.3.0.tar.gz` & `tmp/oclock-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\oclock-1.3.0.tar", last modified: Mon Jan 25 16:59:47 2021, max compression
+gzip compressed data, was "oclock-1.3.1.tar", last modified: Wed Aug  2 08:50:28 2023, max compression
```

## Comparing `oclock-1.3.0.tar` & `oclock-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.684283 oclock-1.3.0/
--rw-rw-rw-   0        0        0       75 2021-01-05 21:35:23.000000 oclock-1.3.0/.gitignore
--rw-rw-rw-   0        0        0     4093 2021-01-25 16:42:42.000000 oclock-1.3.0/AccuracyTests.md
--rw-rw-rw-   0        0        0     7290 2021-01-12 14:47:33.000000 oclock-1.3.0/Examples.ipynb
--rw-rw-rw-   0        0        0    35823 2021-01-25 16:42:42.000000 oclock-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      102 2021-01-25 16:42:42.000000 oclock-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    19602 2021-01-25 16:59:47.685280 oclock-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    15708 2021-01-25 16:42:42.000000 oclock-1.3.0/README.md
--rw-rw-rw-   0        0        0      470 2021-01-25 16:19:55.000000 oclock-1.3.0/example.py
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.592531 oclock-1.3.0/media/
--rw-rw-rw-   0        0        0    53154 2021-01-03 11:16:14.000000 oclock-1.3.0/media/countdown.gif
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.646391 oclock-1.3.0/media/img/
--rw-rw-rw-   0        0        0    34866 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_macos_1000ms.png
--rw-rw-rw-   0        0        0    34131 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_macos_100ms.png
--rw-rw-rw-   0        0        0    35454 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_macos_10ms.png
--rw-rw-rw-   0        0        0    38781 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_macos_1ms.png
--rw-rw-rw-   0        0        0    36275 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_macos_40ms.png
--rw-rw-rw-   0        0        0    23765 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_windows_1000ms.png
--rw-rw-rw-   0        0        0    30214 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_windows_100ms.png
--rw-rw-rw-   0        0        0    30779 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_windows_10ms.png
--rw-rw-rw-   0        0        0    26842 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_windows_1ms.png
--rw-rw-rw-   0        0        0    32829 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/precisetimer_windows_40ms.png
--rw-rw-rw-   0        0        0    69846 2021-01-25 16:42:42.000000 oclock-1.3.0/media/img/ribosome.png
--rw-rw-rw-   0        0        0    37413 2021-01-03 13:46:58.000000 oclock-1.3.0/media/img/timer_interval_exceeded.png
--rw-rw-rw-   0        0        0    36134 2021-01-03 13:50:23.000000 oclock-1.3.0/media/img/timer_macos_1000ms.png
--rw-rw-rw-   0        0        0    36719 2021-01-03 13:49:53.000000 oclock-1.3.0/media/img/timer_macos_100ms.png
--rw-rw-rw-   0        0        0    39398 2021-01-03 13:48:18.000000 oclock-1.3.0/media/img/timer_macos_10ms.png
--rw-rw-rw-   0        0        0    57825 2021-01-03 13:47:38.000000 oclock-1.3.0/media/img/timer_macos_1ms.png
--rw-rw-rw-   0        0        0    40345 2021-01-03 13:48:59.000000 oclock-1.3.0/media/img/timer_macos_40ms.png
--rw-rw-rw-   0        0        0    33693 2021-01-03 09:47:09.000000 oclock-1.3.0/media/img/timer_windows_1000ms.png
--rw-rw-rw-   0        0        0    51059 2021-01-03 09:55:41.000000 oclock-1.3.0/media/img/timer_windows_100ms.png
--rw-rw-rw-   0        0        0    55678 2021-01-03 09:57:38.000000 oclock-1.3.0/media/img/timer_windows_10ms.png
--rw-rw-rw-   0        0        0    33242 2021-01-03 10:02:54.000000 oclock-1.3.0/media/img/timer_windows_1ms.png
--rw-rw-rw-   0        0        0    55281 2021-01-03 10:06:29.000000 oclock-1.3.0/media/img/timer_windows_40ms.png
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.667328 oclock-1.3.0/oclock/
--rw-rw-rw-   0        0        0     1325 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/__init__.py
--rw-rw-rw-   0        0        0     1433 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/__main__.py
--rw-rw-rw-   0        0        0     4260 2021-01-25 16:54:52.000000 oclock-1.3.0/oclock/countdown.py
--rw-rw-rw-   0        0        0     5169 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/event.py
--rw-rw-rw-   0        0        0     3577 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/general.py
--rw-rw-rw-   0        0        0     4609 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/loop.py
--rw-rw-rw-   0        0        0     4114 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/performance.py
--rw-rw-rw-   0        0        0     7302 2021-01-25 16:42:42.000000 oclock-1.3.0/oclock/timer.py
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.681291 oclock-1.3.0/oclock.egg-info/
--rw-rw-rw-   0        0        0    19602 2021-01-25 16:59:47.000000 oclock-1.3.0/oclock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2021-01-25 16:59:47.000000 oclock-1.3.0/oclock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-25 16:59:47.000000 oclock-1.3.0/oclock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2021-01-25 16:59:47.000000 oclock-1.3.0/oclock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-01-25 16:59:47.000000 oclock-1.3.0/oclock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1074 2021-01-25 16:59:47.688272 oclock-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       93 2021-01-01 10:57:17.000000 oclock-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-01-25 16:59:47.683286 oclock-1.3.0/tests/
--rw-rw-rw-   0        0        0     2598 2021-01-25 16:42:42.000000 oclock-1.3.0/tests/test_oclock.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867336 oclock-1.3.1/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       69 2023-08-02 07:21:25.000000 oclock-1.3.1/.gitignore
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4004 2023-08-02 07:21:25.000000 oclock-1.3.1/AccuracyTests.md
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    90676 2023-08-02 08:37:25.000000 oclock-1.3.1/Examples.ipynb
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    35149 2023-08-02 07:21:25.000000 oclock-1.3.1/LICENSE
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       97 2023-08-02 07:21:25.000000 oclock-1.3.1/MANIFEST.in
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 08:50:28.867416 oclock-1.3.1/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    15691 2023-08-02 08:46:47.000000 oclock-1.3.1/README.md
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)      450 2023-08-02 07:21:25.000000 oclock-1.3.1/example.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.861307 oclock-1.3.1/media/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    53154 2023-08-02 07:21:25.000000 oclock-1.3.1/media/countdown.gif
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.865136 oclock-1.3.1/media/img/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    34866 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    34131 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    35454 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    38781 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36275 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_macos_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    23765 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    30214 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    30779 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    26842 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    32829 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/precisetimer_windows_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    69846 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/ribosome.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    37413 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_interval_exceeded.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36134 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    36719 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    39398 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    57825 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    40345 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_macos_40ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    33693 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_1000ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    51059 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_100ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    55678 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_10ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    33242 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_1ms.png
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    55281 2023-08-02 07:21:25.000000 oclock-1.3.1/media/img/timer_windows_40ms.png
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.866356 oclock-1.3.1/oclock/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1291 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/__init__.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1394 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/__main__.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4260 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/countdown.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4974 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/event.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     3443 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/general.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     4480 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/loop.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     3992 2023-08-02 07:21:25.000000 oclock-1.3.1/oclock/performance.py
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     7288 2023-08-02 08:21:04.000000 oclock-1.3.1/oclock/timer.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867106 oclock-1.3.1/oclock.egg-info/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)    16603 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/PKG-INFO
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1216 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/SOURCES.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        1 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/dependency_links.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       19 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/requires.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)        7 2023-08-02 08:50:28.000000 oclock-1.3.1/oclock.egg-info/top_level.txt
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     1039 2023-08-02 08:50:28.867722 oclock-1.3.1/setup.cfg
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)       89 2023-08-02 07:21:25.000000 oclock-1.3.1/setup.py
+drwxr-xr-x   0 olivier.vincent   (502) staff       (20)        0 2023-08-02 08:50:28.867241 oclock-1.3.1/tests/
+-rw-r--r--   0 olivier.vincent   (502) staff       (20)     2512 2023-08-02 07:21:25.000000 oclock-1.3.1/tests/test_oclock.py
```

### Comparing `oclock-1.3.0/AccuracyTests.md` & `oclock-1.3.1/AccuracyTests.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-
-# Accuracy test
-
-This file summarizes accuracy test for loops of constant duration using the `oclock.Timer` class. Tests are done using the performance_test function (see *Readme.md*), e.g.
-```python
-from oclock.performance import performance_test
-performance_test(dt=0.1, nloops=1000, fmax=0.5, plot=True, precise=True)
-```
-
-Below are some results on timing accuracy in an Unix Environment (MacOS) and Windows, using `nloops=1000`, `fmax=0.5` for various values of `dt`. *Regular Timer* means with `precise=False` while *Precise Timer* means with `precise=True`.
-
-## Unix
-
-### Regular Timer
-
-|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
-|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
-| average `dt` - requested `dt` (ms) | 0.0012 | 0.00012 | 0.00016 | 0.00005 | 0.00023 |
-| standard deviation in `dt` (ms)    | 0.48   | 0.36    |   0.31  |  0.23   | 0.08    |
-
-Corresponding graphs:
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_1000ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_100ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_400ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_10ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_1ms.png)
-
-
-### Precise Timer
-
-|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
-|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
-| average `dt` - requested `dt` (ms) | 3.6E-5 | 3.4E-5  | 2.8E-5  | 3.0E-5  | 1.2E-5  |
-| standard deviation in `dt` (ms)    | 0.0118 | 0.0104  | 0.0117  | 0.0105  | 0.0073  |
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_1000ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_100ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_400ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_10ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_1ms.png)
-
-
-## Windows
-
-### Regular Timer
-
-|         Requested `dt` (ms)        | 1000  |   100   |   40    |   10    |  1  |
-|:----------------------------------:|:-----:|:-------:|:-------:|:-------:|:---:|
-| average `dt` - requested `dt` (ms) | 0.014 | 0.0015  | 0.0013  |  1.2    | 1.1 |
-| standard deviation in `dt` (ms)    | 7.0   | 7.1     |  7.0    |  5.6    | 1.9 |
-
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_1000ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_100ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_400ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_10ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_1ms.png)
-
-
-### Precise Timer
-
-
-|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
-|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
-| average `dt` - requested `dt` (ms) | 1.3E-5 | 1.5E-5  | 1.6E-5  | 6.7E-6  | 1.5E-6  |
-| standard deviation in `dt` (ms)    | 0.0066 | 0.0100  | 0.0088  | 0.0068  | 0.0036  |
-
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_1000ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_100ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_400ms.png)
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_10ms.png)
-
+
+# Accuracy test
+
+This file summarizes accuracy test for loops of constant duration using the `oclock.Timer` class. Tests are done using the performance_test function (see *Readme.md*), e.g.
+```python
+from oclock.performance import performance_test
+performance_test(dt=0.1, nloops=1000, fmax=0.5, plot=True, precise=True)
+```
+
+Below are some results on timing accuracy in an Unix Environment (MacOS) and Windows, using `nloops=1000`, `fmax=0.5` for various values of `dt`. *Regular Timer* means with `precise=False` while *Precise Timer* means with `precise=True`.
+
+## Unix
+
+### Regular Timer
+
+|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
+|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
+| average `dt` - requested `dt` (ms) | 0.0012 | 0.00012 | 0.00016 | 0.00005 | 0.00023 |
+| standard deviation in `dt` (ms)    | 0.48   | 0.36    |   0.31  |  0.23   | 0.08    |
+
+Corresponding graphs:
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_1000ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_100ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_400ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_10ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_macos_1ms.png)
+
+
+### Precise Timer
+
+|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
+|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
+| average `dt` - requested `dt` (ms) | 3.6E-5 | 3.4E-5  | 2.8E-5  | 3.0E-5  | 1.2E-5  |
+| standard deviation in `dt` (ms)    | 0.0118 | 0.0104  | 0.0117  | 0.0105  | 0.0073  |
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_1000ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_100ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_400ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_10ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_macos_1ms.png)
+
+
+## Windows
+
+### Regular Timer
+
+|         Requested `dt` (ms)        | 1000  |   100   |   40    |   10    |  1  |
+|:----------------------------------:|:-----:|:-------:|:-------:|:-------:|:---:|
+| average `dt` - requested `dt` (ms) | 0.014 | 0.0015  | 0.0013  |  1.2    | 1.1 |
+| standard deviation in `dt` (ms)    | 7.0   | 7.1     |  7.0    |  5.6    | 1.9 |
+
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_1000ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_100ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_400ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_10ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_windows_1ms.png)
+
+
+### Precise Timer
+
+
+|         Requested `dt` (ms)        |  1000  |   100   |   40    |   10    |    1    |
+|:----------------------------------:|:------:|:-------:|:-------:|:-------:|:-------:|
+| average `dt` - requested `dt` (ms) | 1.3E-5 | 1.5E-5  | 1.6E-5  | 6.7E-6  | 1.5E-6  |
+| standard deviation in `dt` (ms)    | 0.0066 | 0.0100  | 0.0088  | 0.0068  | 0.0036  |
+
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_1000ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_100ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_400ms.png)
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_10ms.png)
+
 ![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/precisetimer_windows_1ms.png)
```

### Comparing `oclock-1.3.0/LICENSE` & `oclock-1.3.1/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `oclock-1.3.0/PKG-INFO` & `oclock-1.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,390 +1,394 @@
-Metadata-Version: 2.1
-Name: oclock
-Version: 1.3.0
-Summary: Tools for timed, no-drift loops of constant duration, and other misc. timing tools (GUI countdown, context managers etc.)
-Home-page: https://github.com/ovinc/oclock
-Author: Olivier Vincent
-Author-email: ovinc.py@gmail.com
-License: GNU GPLv3
-Description: # About
-        
-        **oclock** is a Python 3 package. Its main goal is to provide a simple way to create timed loops with constant time intervals and no drift. It also provides various other timing tools and a GUI time.
-        
-        ### Timed loops
-        
-        No drift, timed loops are based on the `Timer` class,
-        - either using the `checkpt()` method at a location in a for/while loop acting as a reference point to maintain constant duration from one loop to the next,
-        - or using the `@loop` or `@interactiveloop` decorators that use `Timer` and `checkpt()` in the background.
-        
-        The timing (interval) and execution (pause/stop etc.) can be modified in real time thanks to cancellable sleeping times.
-        
-        ### Other tools
-        
-        - `Event`: class mimicking `threading.Event()` but with much better sleeping time accuracy.
-        - `Countdown`: a class that starts a GUI countdown timer.
-        - `parse_time()` function: returns a `datetime.timedelta` from a time string (e.g. `':2:25'`).
-        - `measure_time()` and `measure_duration()` functions: are context managers for measuring time and execution times / time uncertainty of encapsulated commands.
-        - Note that the `Timer` class can also be used as a regular chronometer with its methods `pause()`, `resume()`, `stop()` etc.
-        
-        # Quick start
-        
-        ## Install
-        
-        ```bash
-        pip install oclock
-        ```
-        
-        ## Timed Loops
-        
-        The `Timer` class is mostly designed to create loops of constant duration without drift, while allowing immediate modification/cancellation (sleep time interruption) in threaded environments. It can also be used as a regular chronometer.
-        
-        Below are some peudo-code quick-start examples. For complete, working examples, see:
-        - *Examples.ipynb* notebook (https://github.com/ovinc/oclock/blob/master/Example.ipynb)
-        - *example.py* script (https://github.com/ovinc/oclock/blob/master/example.py)
-        
-        
-        ### Constant-duration loops
-        
-        The most basic use of the `Timer()` class in Python code to create a loop of constant duration is:
-        ```python
-        from oclock import Timer
-        timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
-        while condition:
-            my_function()  # can be of any duration between 0 and 2 seconds
-            timer.checkpt()
-        ```
-        The `checkpt()` method waits the adequate amount of time to make the loop of constant duration, without drift (using a target regularly spaced in time); `condition` can include timer methods and attributes, e.g. `timer.elapsed_time < max_time`.
-        
-        Note that if *my_function()* takes longer to execute than the required time interval, the Timer class does not try to compensate the extra time by making the next loop shorter. It just aims at making the total duration of the next loop be the requested interval again (see *Behavior when interval is exceeded* section below).
-        
-        The same behavior can be achieved using the `@loop` decorator:
-        ```python
-        from oclock import loop
-        timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
-        @loop(timer)
-        def my_function():
-            ...
-        ```
-        Then, calling `my_function()` will execute the contents of the function in a repeated manner.
-        
-        The `@loop` execution exits automatically if the timer is stopped.
-        Thus, It is useful to include a condition in `my_function` to exit the loop when needed, e.g.
-        ```python
-        if timer.elapsed_time > t_max:
-            timer.stop()
-        ```
-        
-        ### Interactive modification/cancellation
-        
-        The timer is also modifiable (change time interval) and cancellable in real time (i.e. even when the timer is in a `checkpt()` waiting phase). To do so, it must be accessed by another thread that runs concurrently. For example:
-        
-        ```python
-        from oclock import Timer
-        from threading import Thread
-        
-        def user_input(timer):
-            """Threaded command line input to change time interval or exit timer."""
-            while not timer.is_stopped:
-                a = input()
-                try:
-                    dt = float(a)
-                except ValueError:  # immediately cancel timer & exit all loops/threads
-                    timer.stop()
-                else:               # immediately change interval to input value
-                    timer.interval = dt
-        
-        timer = Timer(interval=2)
-        Thread(target=user_input, args=(exit_event, timer)).start()
-        
-        while not timer.is_stopped:
-            my_function()
-            timer.checkpt()
-        ```
-        During operation, the `Timer` object can be paused, resumed, stopped and reset using the corresponding `Timer` methods (see *Regular Timer* paragraph below). The *oclock* module also provides a simple command line interface to create a timed loop for a function and interact with it dynamically using the `@interactiveloop` decorator:
-        ```python
-        from oclock import interactiveloop
-        @interactiveloop(interval=2)
-        def my_function():
-            ...
-        ```
-        Now when `my_function()` is called, an interactive CLI thread starts at the same time where the user can pause/resume/reset/stop the timer in real time, change its interval, and print timing information.
-        
-        ### Regular Timer
-        
-        Although not its main purpose, the `Timer` class can be used as a regular chronometer with the following methods (no need to be in a threaded environment, although the methods below whould work and be cancellable in a threaded environment):
-        
-        ```python
-        from oclock import Timer
-        
-        # The timer starts counting time immediately upon instantiation.
-        timer = Timer()
-        
-        # Temporarily pause, then resume timer
-        timer.pause()
-        timer.resume()
-        
-        # Stop and restart timer completely
-        timer.stop()
-        timer.reset()  # note: can be called without calling stop() first
-        
-        # At any time, the elapsed time and total pause duration can be accessed with
-        timer.elapsed_time
-        timer.pause_time
-        timer.total_time  # sum of the two other times
-        ```
-        
-        **Important Note**: Do not use the `checkpt()` method after a `pause()` call if not in a threaded environment, this will cause the program to be in a perpetual waiting state. In a threaded environment, call `resume()` to unpause.
-        
-        ### Details
-        
-        See *Timer Class details* section below for all methods, properties and attributes and the *Development* section below for accuracy information.
-        
-        
-        ## Event class
-        
-        The `oclock.Event` class mimicks `threading.Event` (https://docs.python.org/3/library/threading.html#event-objects) but provides much better sleep time accuracy.
-        
-        Available methods are the same as for `threading.Event`:
-        - `set()`
-        - `clear()`
-        - `is_set()`
-        - `wait()`
-        
-        
-        Below are comments from Chris D. who originally posted the code for this class on StackOverflow (see *Contributors* at the end of this file):
-        
-        > Internally, it uses a combination of a time.sleep() loop and a busy loop for greatly increased precision. The sleep loop runs in a separate thread so that the blocking wait() call in the main thread can still be immediately interrupted. When the set() method is called, the sleep thread should terminate shortly afterwards. Also, in order to minimize CPU utilization, I made sure that the busy loop will never run for more than 3 milliseconds.
-        
-        
-        ## Countdown GUI
-        
-        A simple graphical countdown timer based on the `Timer` class. It can be used either as a python main program from a shell, or as a function in Python code or console.
-        
-        ![](https://raw.githubusercontent.com/ovinc/oclock/master/media/countdown.gif)
-        
-        From a terminal:
-        ```bash
-        python -m oclock 1:45:00   # start timer of duration 1 hour 45 minutes
-        python -m oclock 1:45:     # exactly the same as above
-        python -m oclock 00:02:00  # start 2-minute timer
-        python -m oclock :2:       # exactly the same as above
-        python -m oclock 00:00:05  # start 5-second timer
-        python -m oclock ::5       # exactly the same as above
-        ```
-        
-        In python:
-        ```python
-        from oclock import Countdown
-        Countdown('1:45:')         # start timer of duration 1 hour 45 minutes
-        ```
-        (the inputs are of the same format as from the terminal, see above).
-        
-        When countdown is finished, 'Done' is displayed for 5 seconds in the GUI while the console displays *Countdown finished* and emits a sound. Then the time passed since the end of countdown is displayed as a negative value in red. The program stops when the GUI window is closed.
-        
-        ## Parse time function
-        
-        The `parse_time()` function is used in the argument parsing of the countdown GUI from a terminal (see above). It transforms a string in the form `'h:m:s'` into a `datetime.timedelta` object. Inputs of the form e.g. `'::5'` or `:2:`, `'3:30:'` are acceptable for 5 seconds, 2 minutes, and 3.5 hours, respectively.
-        ```python
-        >>> parse_time(':2:30')
-        datetime.timedelta(seconds=150)
-        ```
-        
-        ## Context managers to record timing of commands
-        
-        The `measure_time()` function is a context manager that saves the timing info of the encapsulated commands. This can be e.g. used in scientific experiments to get the time and time uncertainty associated with a measurement.
-        ```python
-        from oclock import measure_time, measure_duration
-        
-        # ----------------------------------------------------------------------------
-        # Examples where one just wants to get timing info ---------------------------
-        # ----------------------------------------------------------------------------
-        
-        with measure_time() as timing:
-            my_function()
-        print(timing)
-        
-        # Out: {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
-        
-        # (dt (s) is half the total duration. To get the total duration instead, do:)
-        
-        with measure_duration() as duration:
-            my_function()
-        print(duration)
-        
-        # Out: {'duration (s)': 1.1689763555421325}
-        
-        # ----------------------------------------------------------------------------
-        # Example where the timing info is directly added to a data dictionary -------
-        # ----------------------------------------------------------------------------
-        
-        with measure_time() as data:
-            measurement = my_function()  # returns e.g. 3.618
-            data['measurement'] = measurement
-        print(data)
-        
-        # Out: {'measurement': 3.618,
-        #       'time (unix)': 1604780958.0705943,
-        #       'dt (s)': 0.6218999624252319}
-        ```
-        
-        
-        # Timer Class details
-        
-        ## Instantiation
-        
-        ```python
-        from oclock import Timer
-        timer = Timer(interval=1, name='Timer', warnings=False, precise=False)
-        ```
-        
-        Parameters:
-        - `interval` (float): timer interval in seconds
-        - `name` (str): optional name for description purposes (repr and warnings)
-        - `warnings` (bool): If True, prints warning when time interval exceeded
-        - `precise` (bool) if True, increase time precision (useful for Windows)
-        
-        *Note:* The `precise=True` option uses a custom `Event` class to replace `threading.Event`, originally written by Chris D. (see below).
-        
-        ## Methods
-        
-        ```python
-        timer.checkpt()  # Reference point for constant-duration loops, see above
-        
-        timer.pause()    # Immediately pause timer and put checkpt() in waiting phase
-        timer.resume()   # Restart the elapsed time counter and unlock checkpt()
-        
-        timer.stop()     # Stop counting time and exit checkpt()
-        timer.reset()    # Stop and restart timer immediately
-        ```
-        
-        ## Properties (settable)
-        
-        ```python
-        timer.interval       # get interval (in s)
-        timer.interval += 1  # increase interval by 1 second
-        timer.interval = 10  # set interval to 10 seconds.
-        
-        timer.warnings          # get current status of warnings
-        timer.warnings = True   # activate warnings if time between checkpts too short
-        
-        timer.name                      # optional name (for repr and warnings)
-        timer.name = 'Countdown timer'  # (can also be set during instantiation)
-        ```
-        
-        ## Attributes (read-only)
-        
-        ```python
-        # Most useful attributes
-        timer.elapsed_time  # Time in seconds since init or last reset
-        timer.pause_time    # total time (in s) the timer has been paused.
-        timer.total_time    # Sum of the last two
-        ```
-        
-        ## Background attributes and methods
-        (mostly for development)
-        ```python
-        timer.now()                 # Reference time used by all methods
-        timer.start_time            # Ref. time corresponding to start/reset of timer
-        timer.next_checkpt_release  # Ref. time at which next checkpt waittime is over
-        timer.interval_exceeded     # (bool) True if loop contents take longer to execute than requested interval
-        ```
-        
-        ## Notes
-        
-        - As mentioned previously, methods (and interval setting) take effect immediately, even if the timer is in a waiting phase.
-        
-        - After calling `pause()`, the `checkpt()` command blocks until `resume()` is called, however in the current version after `stop()` the `checkpt()` becomes non-blocking (equivalent to a `pass`), so that all following lines will be executed immediately and without any waiting time (i.e. as fast as possible if within a loop), until `timer.reset()` is called again. This means that it is useful to pin the condition of the loop to the stopping of the timer (see examples).
-        
-        
-        ## Timer accuracy
-        
-        See *performance.py* file of the module for functions to test the behavior and accuracy of the timer. In particular:
-        ```python
-        from oclock.performance import performance_test
-        performance_test(dt=0.01, nloops=1000, fmax=0.99, plot=True, warnings=False, precise=True)
-        ```
-        tests the timing on 1000 loops of requested duration 0.01 second (10ms), using within the loop a function sleeping for a random amount of time between 0 and 0.99 dt (with `plot=True` option to see the results on a *matplotlib* graph, and `warnings=False` to not have a printed warning when the execution time of the nested commands exceed the target duration of the loop); `precise=True` uses the timer in precise mode.
-        
-        The *AccuracyTests.md* file gathers some accuracy results in Unix and Windows environments. In summary:
-        
-        - with **Unix**, time fluctuations are < 0.5 ms with the regular timer, and on the order of 0.01 ms (standard deviation) with the precise timer
-        
-        - with **Windows**, the regular timer fails quickly as frame rate is increased, due to fluctuations in the ~ 10 ms range. However the precise timer performs even better than in Unix, with fluctuations of less than 0.01 ms (standard deviation).
-        
-        
-        ## Behavior when interval is exceeded
-        
-        As explained above, it the contents of the loop take longer to execute than the requested time interval, the Timer simply moves on to the next loop but does not try to compensate for the extra time by making the next loop shorter:
-        
-        ![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_interval_exceeded.png)
-        
-        
-        
-        # Development
-        
-        Install the package by cloning the GitHub repo (https://github.com/ovinc/oclock.git) and install in editable mode from the root of the repo:
-        ```
-        pip install -e .
-        ```
-        
-        ## Testing
-        
-        Package requirements to run the tests:
-        - pytest
-        - numpy
-        
-        General testing is done with *pytest* (from the root of the repository):
-        ```bash
-        pytest
-        ```
-        (**Note**: close the interactive countdown window at the end of the pytest run to finish the test.)
-        
-        Additional testing of interactive command line for real-time timer control can be done by running the example file from the root of the repository.
-        ```bash
-        python -m example
-        ```
-        
-        See also *Accuracy Test* paragraph above to run performance tests for constant-duration loops with the `Timer` class.
-        
-        ## Contributing
-        
-        Issues and Pull requests must be submitted on GitHub (https://github.com/ovinc/oclock) with commits (preferably squashed into a single commit) in branch *authors*.
-        
-        Version number is automatically extracted from git tag using *setuptools_scm*. Git tags are added by the repo's maintainer.
-        
-        # Requirements
-        
-        Python 3.x
-        
-        (Tests only made from python 3.5 to python 3.9 included)
-        
-        
-        # Author
-        
-        Olivier Vincent
-        
-        (ovinc.py@gmail.com)
-        
-        # Contributors
-        
-        The `oclock.Event` class was originally written by Chris D.
-        
-        (https://stackoverflow.com/questions/48984512/making-a-timer-timeout-inaccuracy-of-threading-event-wait-python-3-6)
-        
-        
-        # License
-        
-        GNU GPLv3, see *LICENSE* file
-        
-Keywords: timing,loops,constant duration,cancellable,modifiable,countdown,context manager,gui
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: oclock
+Version: 1.3.1
+Summary: Tools for timed, no-drift loops of constant duration, and other misc. timing tools (GUI countdown, context managers etc.)
+Home-page: https://github.com/ovinc/oclock
+Author: Olivier Vincent
+Author-email: ovinc.py@gmail.com
+License: GNU GPLv3
+Keywords: timing,loops,constant duration,cancellable,modifiable,countdown,context manager,gui
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# About
+
+**oclock** is a Python 3 package. Its main goal is to provide a simple way to create timed loops with constant time intervals and no drift. It also provides various other timing tools and a GUI time.
+
+### Timed loops
+
+No drift, timed loops are based on the `Timer` class,
+- either using the `checkpt()` method at a location in a for/while loop acting as a reference point to maintain constant duration from one loop to the next,
+- or using the `@loop` or `@interactiveloop` decorators that use `Timer` and `checkpt()` in the background.
+
+The timing (interval) and execution (pause/stop etc.) can be modified in real time thanks to cancellable sleeping times.
+
+### Other tools
+
+- `Event`: class mimicking `threading.Event()` but with much better sleeping time accuracy.
+- `Countdown`: a class that starts a GUI countdown timer.
+- `parse_time()` function: returns a `datetime.timedelta` from a time string (e.g. `':2:25'`).
+- `measure_time()` and `measure_duration()` functions: are context managers for measuring time and execution times / time uncertainty of encapsulated commands.
+- Note that the `Timer` class can also be used as a regular chronometer with its methods `pause()`, `resume()`, `stop()` etc.
+
+# Quick start
+
+## Install
+
+```bash
+pip install oclock
+```
+
+## Timed Loops
+
+The `Timer` class is mostly designed to create loops of constant duration without drift, while allowing immediate modification/cancellation (sleep time interruption) in threaded environments. It can also be used as a regular chronometer.
+
+Below are some peudo-code quick-start examples. For complete, working examples, see:
+- *Examples.ipynb* notebook (https://github.com/ovinc/oclock/blob/master/Example.ipynb)
+- *example.py* script (https://github.com/ovinc/oclock/blob/master/example.py)
+
+
+### Constant-duration loops
+
+The most basic use of the `Timer()` class in Python code to create a loop of constant duration is:
+```python
+from oclock import Timer
+timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
+while condition:
+    my_function()  # can be of any duration between 0 and 2 seconds
+    timer.checkpt()
+```
+The `checkpt()` method waits the adequate amount of time to make the loop of constant duration, without drift (using a target regularly spaced in time); `condition` can include timer methods and attributes, e.g. `timer.elapsed_time < max_time`.
+
+Note that if *my_function()* takes longer to execute than the required time interval, the Timer class does not try to compensate the extra time by making the next loop shorter. It just aims at making the total duration of the next loop be the requested interval again (see *Behavior when interval is exceeded* section below).
+
+The same behavior can be achieved using the `@loop` decorator:
+```python
+from oclock import loop
+timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
+@loop(timer)
+def my_function():
+    ...
+```
+Then, calling `my_function()` will execute the contents of the function in a repeated manner.
+
+The `@loop` execution exits automatically if the timer is stopped.
+Thus, It is useful to include a condition in `my_function` to exit the loop when needed, e.g.
+```python
+if timer.elapsed_time > t_max:
+    timer.stop()
+```
+
+### Interactive modification/cancellation
+
+The timer is also modifiable (change time interval) and cancellable in real time (i.e. even when the timer is in a `checkpt()` waiting phase). To do so, it must be accessed by another thread that runs concurrently. For example:
+
+```python
+from oclock import Timer
+from threading import Thread
+
+def user_input(timer):
+    """Threaded command line input to change time interval or exit timer."""
+    while not timer.is_stopped:
+        a = input()
+        try:
+            dt = float(a)
+        except ValueError:  # immediately cancel timer & exit all loops/threads
+            timer.stop()
+        else:               # immediately change interval to input value
+            timer.interval = dt
+
+timer = Timer(interval=2)
+Thread(target=user_input, args=(exit_event, timer)).start()
+
+while not timer.is_stopped:
+    my_function()
+    timer.checkpt()
+```
+During operation, the `Timer` object can be paused, resumed, stopped and reset using the corresponding `Timer` methods (see *Regular Timer* paragraph below). The *oclock* module also provides a simple command line interface to create a timed loop for a function and interact with it dynamically using the `@interactiveloop` decorator:
+```python
+from oclock import interactiveloop
+@interactiveloop(interval=2)
+def my_function():
+    ...
+```
+Now when `my_function()` is called, an interactive CLI thread starts at the same time where the user can pause/resume/reset/stop the timer in real time, change its interval, and print timing information.
+
+### Regular Timer
+
+Although not its main purpose, the `Timer` class can be used as a regular chronometer with the following methods (no need to be in a threaded environment, although the methods below whould work and be cancellable in a threaded environment):
+
+```python
+from oclock import Timer
+
+# The timer starts counting time immediately upon instantiation.
+timer = Timer()
+
+# Temporarily pause, then resume timer
+timer.pause()
+timer.resume()
+
+# Stop and restart timer completely
+timer.stop()
+timer.reset()  # note: can be called without calling stop() first
+
+# At any time, the elapsed time and total pause duration can be accessed with
+timer.elapsed_time
+timer.pause_time
+timer.total_time  # sum of the two other times
+```
+
+**Important Note**: Do not use the `checkpt()` method after a `pause()` call if not in a threaded environment, this will cause the program to be in a perpetual waiting state. In a threaded environment, call `resume()` to unpause.
+
+### Details
+
+See *Timer Class details* section below for all methods, properties and attributes and the *Development* section below for accuracy information.
+
+
+## Event class
+
+The `oclock.Event` class mimicks `threading.Event` (https://docs.python.org/3/library/threading.html#event-objects) but provides much better sleep time accuracy.
+
+Available methods are the same as for `threading.Event`:
+- `set()`
+- `clear()`
+- `is_set()`
+- `wait()`
+
+
+Below are comments from Chris D. who originally posted the code for this class on StackOverflow (see *Contributors* at the end of this file):
+
+> Internally, it uses a combination of a time.sleep() loop and a busy loop for greatly increased precision. The sleep loop runs in a separate thread so that the blocking wait() call in the main thread can still be immediately interrupted. When the set() method is called, the sleep thread should terminate shortly afterwards. Also, in order to minimize CPU utilization, I made sure that the busy loop will never run for more than 3 milliseconds.
+
+
+## Countdown GUI
+
+A simple graphical countdown timer based on the `Timer` class. It can be used either as a python main program from a shell, or as a function in Python code or console.
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/countdown.gif)
+
+From a terminal:
+```bash
+python -m oclock 1:45:00   # start timer of duration 1 hour 45 minutes
+python -m oclock 1:45:     # exactly the same as above
+python -m oclock 00:02:00  # start 2-minute timer
+python -m oclock :2:       # exactly the same as above
+python -m oclock 00:00:05  # start 5-second timer
+python -m oclock ::5       # exactly the same as above
+```
+
+In python:
+```python
+from oclock import Countdown
+Countdown('1:45:')         # start timer of duration 1 hour 45 minutes
+```
+(the inputs are of the same format as from the terminal, see above).
+
+When countdown is finished, 'Done' is displayed for 5 seconds in the GUI while the console displays *Countdown finished* and emits a sound. Then the time passed since the end of countdown is displayed as a negative value in red. The program stops when the GUI window is closed.
+
+## Parse time function
+
+The `parse_time()` function is used in the argument parsing of the countdown GUI from a terminal (see above). It transforms a string in the form `'h:m:s'` into a `datetime.timedelta` object. Inputs of the form e.g. `'::5'` or `:2:`, `'3:30:'` are acceptable for 5 seconds, 2 minutes, and 3.5 hours, respectively.
+```python
+>>> parse_time(':2:30')
+datetime.timedelta(seconds=150)
+```
+
+## Context managers to record timing of commands
+
+The `measure_time()` function is a context manager that saves the timing info of the encapsulated commands. This can be e.g. used in scientific experiments to get the time and time uncertainty associated with a measurement.
+```python
+from oclock import measure_time, measure_duration
+
+# ----------------------------------------------------------------------------
+# Examples where one just wants to get timing info ---------------------------
+# ----------------------------------------------------------------------------
+
+with measure_time() as timing:
+    my_function()
+print(timing)
+
+# Out: {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
+
+# (dt (s) is half the total duration. To get the total duration instead, do:)
+
+with measure_duration() as duration:
+    my_function()
+print(duration)
+
+# Out: {'duration (s)': 1.1689763555421325}
+
+# ----------------------------------------------------------------------------
+# Example where the timing info is directly added to a data dictionary -------
+# ----------------------------------------------------------------------------
+
+with measure_time() as data:
+    measurement = my_function()  # returns e.g. 3.618
+    data['measurement'] = measurement
+print(data)
+
+# Out: {'measurement': 3.618,
+#       'time (unix)': 1604780958.0705943,
+#       'dt (s)': 0.6218999624252319}
+```
+
+
+# Timer Class details
+
+## Instantiation
+
+```python
+from oclock import Timer
+timer = Timer(interval=1, name='Timer', warnings=False, precise=False)
+```
+
+Parameters:
+- `interval` (float): timer interval in seconds
+- `name` (str): optional name for description purposes (repr and warnings)
+- `warnings` (bool): If True, prints warning when time interval exceeded
+- `precise` (bool) if True, increase time precision (useful for Windows)
+
+*Note:* The `precise=True` option uses a custom `Event` class to replace `threading.Event`, originally written by Chris D. (see below).
+
+## Methods
+
+```python
+timer.checkpt()  # Reference point for constant-duration loops, see above
+
+timer.pause()    # Immediately pause timer and put checkpt() in waiting phase
+timer.resume()   # Restart the elapsed time counter and unlock checkpt()
+
+timer.stop()     # Stop counting time and exit checkpt()
+timer.reset()    # Stop and restart timer immediately
+
+# Change timer interval
+timer.set_interval(...)  # immediately, equivalent to timer.interval = ...
+timer.set_interval(..., immediate=False)   # wait next checkpt
+```
+
+## Properties (settable)
+
+```python
+timer.interval       # get interval (in s)
+timer.interval += 1  # increase interval by 1 second
+timer.interval = 10  # set interval to 10 seconds.
+
+timer.warnings          # get current status of warnings
+timer.warnings = True   # activate warnings if time between checkpts too short
+
+timer.name                      # optional name (for repr and warnings)
+timer.name = 'Countdown timer'  # (can also be set during instantiation)
+```
+
+## Attributes (read-only)
+
+```python
+# Most useful attributes
+timer.elapsed_time  # Time in seconds since init or last reset
+timer.pause_time    # total time (in s) the timer has been paused.
+timer.total_time    # Sum of the last two
+```
+
+## Background attributes and methods
+(mostly for development)
+```python
+timer.now()                 # Reference time used by all methods
+timer.start_time            # Ref. time corresponding to start/reset of timer
+timer.next_checkpt_release  # Ref. time at which next checkpt waittime is over
+timer.interval_exceeded     # (bool) True if loop contents take longer to execute than requested interval
+```
+
+## Notes
+
+- As mentioned previously, methods (and interval setting) take effect immediately, even if the timer is in a waiting phase. It is however possible to wait for the next checkpt to apply a new timer interval, by using the `immediate=False` option in `set_interval()` (see example in the *Examples.ipynb* notebook).
+
+- After calling `pause()`, the `checkpt()` command blocks until `resume()` is called, however in the current version after `stop()` the `checkpt()` becomes non-blocking (equivalent to a `pass`), so that all following lines will be executed immediately and without any waiting time (i.e. as fast as possible if within a loop), until `timer.reset()` is called again. This means that it is useful to pin the condition of the loop to the stopping of the timer (see examples).
+
+
+## Timer accuracy
+
+See *performance.py* file of the module for functions to test the behavior and accuracy of the timer. In particular:
+```python
+from oclock.performance import performance_test
+performance_test(dt=0.01, nloops=1000, fmax=0.99, plot=True, warnings=False, precise=True)
+```
+tests the timing on 1000 loops of requested duration 0.01 second (10ms), using within the loop a function sleeping for a random amount of time between 0 and 0.99 dt (with `plot=True` option to see the results on a *matplotlib* graph, and `warnings=False` to not have a printed warning when the execution time of the nested commands exceed the target duration of the loop); `precise=True` uses the timer in precise mode.
+
+The *AccuracyTests.md* file gathers some accuracy results in Unix and Windows environments. In summary:
+
+- with **Unix**, time fluctuations are < 0.5 ms with the regular timer, and on the order of 0.01 ms (standard deviation) with the precise timer
+
+- with **Windows**, the regular timer fails quickly as frame rate is increased, due to fluctuations in the ~ 10 ms range. However the precise timer performs even better than in Unix, with fluctuations of less than 0.01 ms (standard deviation).
+
+
+## Behavior when interval is exceeded
+
+As explained above, it the contents of the loop take longer to execute than the requested time interval, the Timer simply moves on to the next loop but does not try to compensate for the extra time by making the next loop shorter:
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_interval_exceeded.png)
+
+
+
+# Development
+
+Install the package by cloning the GitHub repo (https://github.com/ovinc/oclock.git) and install in editable mode from the root of the repo:
+```
+pip install -e .
+```
+
+## Testing
+
+Package requirements to run the tests:
+- pytest
+- numpy
+
+General testing is done with *pytest* (from the root of the repository):
+```bash
+pytest
+```
+(**Note**: close the interactive countdown window at the end of the pytest run to finish the test.)
+
+Additional testing of interactive command line for real-time timer control can be done by running the example file from the root of the repository.
+```bash
+python -m example
+```
+
+See also *Accuracy Test* paragraph above to run performance tests for constant-duration loops with the `Timer` class.
+
+## Contributing
+
+Issues and Pull requests must be submitted on GitHub (https://github.com/ovinc/oclock) with commits (preferably squashed into a single commit) in branch *authors*.
+
+Version number is automatically extracted from git tag using *setuptools_scm*. Git tags are added by the repo's maintainer.
+
+# Requirements
+
+Python 3.x
+
+(Tests only made from python 3.5 to python 3.9 included)
+
+
+# Author
+
+Olivier Vincent
+
+(ovinc.py@gmail.com)
+
+# Contributors
+
+The `oclock.Event` class was originally written by Chris D.
+
+(https://stackoverflow.com/questions/48984512/making-a-timer-timeout-inaccuracy-of-threading-event-wait-python-3-6)
+
+
+# License
+
+GNU GPLv3, see *LICENSE* file
```

### Comparing `oclock-1.3.0/README.md` & `oclock-1.3.1/oclock.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,369 +1,394 @@
-# About
-
-**oclock** is a Python 3 package. Its main goal is to provide a simple way to create timed loops with constant time intervals and no drift. It also provides various other timing tools and a GUI time.
-
-### Timed loops
-
-No drift, timed loops are based on the `Timer` class,
-- either using the `checkpt()` method at a location in a for/while loop acting as a reference point to maintain constant duration from one loop to the next,
-- or using the `@loop` or `@interactiveloop` decorators that use `Timer` and `checkpt()` in the background.
-
-The timing (interval) and execution (pause/stop etc.) can be modified in real time thanks to cancellable sleeping times.
-
-### Other tools
-
-- `Event`: class mimicking `threading.Event()` but with much better sleeping time accuracy.
-- `Countdown`: a class that starts a GUI countdown timer.
-- `parse_time()` function: returns a `datetime.timedelta` from a time string (e.g. `':2:25'`).
-- `measure_time()` and `measure_duration()` functions: are context managers for measuring time and execution times / time uncertainty of encapsulated commands.
-- Note that the `Timer` class can also be used as a regular chronometer with its methods `pause()`, `resume()`, `stop()` etc.
-
-# Quick start
-
-## Install
-
-```bash
-pip install oclock
-```
-
-## Timed Loops
-
-The `Timer` class is mostly designed to create loops of constant duration without drift, while allowing immediate modification/cancellation (sleep time interruption) in threaded environments. It can also be used as a regular chronometer.
-
-Below are some peudo-code quick-start examples. For complete, working examples, see:
-- *Examples.ipynb* notebook (https://github.com/ovinc/oclock/blob/master/Example.ipynb)
-- *example.py* script (https://github.com/ovinc/oclock/blob/master/example.py)
-
-
-### Constant-duration loops
-
-The most basic use of the `Timer()` class in Python code to create a loop of constant duration is:
-```python
-from oclock import Timer
-timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
-while condition:
-    my_function()  # can be of any duration between 0 and 2 seconds
-    timer.checkpt()
-```
-The `checkpt()` method waits the adequate amount of time to make the loop of constant duration, without drift (using a target regularly spaced in time); `condition` can include timer methods and attributes, e.g. `timer.elapsed_time < max_time`.
-
-Note that if *my_function()* takes longer to execute than the required time interval, the Timer class does not try to compensate the extra time by making the next loop shorter. It just aims at making the total duration of the next loop be the requested interval again (see *Behavior when interval is exceeded* section below).
-
-The same behavior can be achieved using the `@loop` decorator:
-```python
-from oclock import loop
-timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
-@loop(timer)
-def my_function():
-    ...
-```
-Then, calling `my_function()` will execute the contents of the function in a repeated manner.
-
-The `@loop` execution exits automatically if the timer is stopped.
-Thus, It is useful to include a condition in `my_function` to exit the loop when needed, e.g.
-```python
-if timer.elapsed_time > t_max:
-    timer.stop()
-```
-
-### Interactive modification/cancellation
-
-The timer is also modifiable (change time interval) and cancellable in real time (i.e. even when the timer is in a `checkpt()` waiting phase). To do so, it must be accessed by another thread that runs concurrently. For example:
-
-```python
-from oclock import Timer
-from threading import Thread
-
-def user_input(timer):
-    """Threaded command line input to change time interval or exit timer."""
-    while not timer.is_stopped:
-        a = input()
-        try:
-            dt = float(a)
-        except ValueError:  # immediately cancel timer & exit all loops/threads
-            timer.stop()
-        else:               # immediately change interval to input value
-            timer.interval = dt
-
-timer = Timer(interval=2)
-Thread(target=user_input, args=(exit_event, timer)).start()
-
-while not timer.is_stopped:
-    my_function()
-    timer.checkpt()
-```
-During operation, the `Timer` object can be paused, resumed, stopped and reset using the corresponding `Timer` methods (see *Regular Timer* paragraph below). The *oclock* module also provides a simple command line interface to create a timed loop for a function and interact with it dynamically using the `@interactiveloop` decorator:
-```python
-from oclock import interactiveloop
-@interactiveloop(interval=2)
-def my_function():
-    ...
-```
-Now when `my_function()` is called, an interactive CLI thread starts at the same time where the user can pause/resume/reset/stop the timer in real time, change its interval, and print timing information.
-
-### Regular Timer
-
-Although not its main purpose, the `Timer` class can be used as a regular chronometer with the following methods (no need to be in a threaded environment, although the methods below whould work and be cancellable in a threaded environment):
-
-```python
-from oclock import Timer
-
-# The timer starts counting time immediately upon instantiation.
-timer = Timer()
-
-# Temporarily pause, then resume timer
-timer.pause()
-timer.resume()
-
-# Stop and restart timer completely
-timer.stop()
-timer.reset()  # note: can be called without calling stop() first
-
-# At any time, the elapsed time and total pause duration can be accessed with
-timer.elapsed_time
-timer.pause_time
-timer.total_time  # sum of the two other times
-```
-
-**Important Note**: Do not use the `checkpt()` method after a `pause()` call if not in a threaded environment, this will cause the program to be in a perpetual waiting state. In a threaded environment, call `resume()` to unpause.
-
-### Details
-
-See *Timer Class details* section below for all methods, properties and attributes and the *Development* section below for accuracy information.
-
-
-## Event class
-
-The `oclock.Event` class mimicks `threading.Event` (https://docs.python.org/3/library/threading.html#event-objects) but provides much better sleep time accuracy.
-
-Available methods are the same as for `threading.Event`:
-- `set()`
-- `clear()`
-- `is_set()`
-- `wait()`
-
-
-Below are comments from Chris D. who originally posted the code for this class on StackOverflow (see *Contributors* at the end of this file):
-
-> Internally, it uses a combination of a time.sleep() loop and a busy loop for greatly increased precision. The sleep loop runs in a separate thread so that the blocking wait() call in the main thread can still be immediately interrupted. When the set() method is called, the sleep thread should terminate shortly afterwards. Also, in order to minimize CPU utilization, I made sure that the busy loop will never run for more than 3 milliseconds.
-
-
-## Countdown GUI
-
-A simple graphical countdown timer based on the `Timer` class. It can be used either as a python main program from a shell, or as a function in Python code or console.
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/countdown.gif)
-
-From a terminal:
-```bash
-python -m oclock 1:45:00   # start timer of duration 1 hour 45 minutes
-python -m oclock 1:45:     # exactly the same as above
-python -m oclock 00:02:00  # start 2-minute timer
-python -m oclock :2:       # exactly the same as above
-python -m oclock 00:00:05  # start 5-second timer
-python -m oclock ::5       # exactly the same as above
-```
-
-In python:
-```python
-from oclock import Countdown
-Countdown('1:45:')         # start timer of duration 1 hour 45 minutes
-```
-(the inputs are of the same format as from the terminal, see above).
-
-When countdown is finished, 'Done' is displayed for 5 seconds in the GUI while the console displays *Countdown finished* and emits a sound. Then the time passed since the end of countdown is displayed as a negative value in red. The program stops when the GUI window is closed.
-
-## Parse time function
-
-The `parse_time()` function is used in the argument parsing of the countdown GUI from a terminal (see above). It transforms a string in the form `'h:m:s'` into a `datetime.timedelta` object. Inputs of the form e.g. `'::5'` or `:2:`, `'3:30:'` are acceptable for 5 seconds, 2 minutes, and 3.5 hours, respectively.
-```python
->>> parse_time(':2:30')
-datetime.timedelta(seconds=150)
-```
-
-## Context managers to record timing of commands
-
-The `measure_time()` function is a context manager that saves the timing info of the encapsulated commands. This can be e.g. used in scientific experiments to get the time and time uncertainty associated with a measurement.
-```python
-from oclock import measure_time, measure_duration
-
-# ----------------------------------------------------------------------------
-# Examples where one just wants to get timing info ---------------------------
-# ----------------------------------------------------------------------------
-
-with measure_time() as timing:
-    my_function()
-print(timing)
-
-# Out: {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
-
-# (dt (s) is half the total duration. To get the total duration instead, do:)
-
-with measure_duration() as duration:
-    my_function()
-print(duration)
-
-# Out: {'duration (s)': 1.1689763555421325}
-
-# ----------------------------------------------------------------------------
-# Example where the timing info is directly added to a data dictionary -------
-# ----------------------------------------------------------------------------
-
-with measure_time() as data:
-    measurement = my_function()  # returns e.g. 3.618
-    data['measurement'] = measurement
-print(data)
-
-# Out: {'measurement': 3.618,
-#       'time (unix)': 1604780958.0705943,
-#       'dt (s)': 0.6218999624252319}
-```
-
-
-# Timer Class details
-
-## Instantiation
-
-```python
-from oclock import Timer
-timer = Timer(interval=1, name='Timer', warnings=False, precise=False)
-```
-
-Parameters:
-- `interval` (float): timer interval in seconds
-- `name` (str): optional name for description purposes (repr and warnings)
-- `warnings` (bool): If True, prints warning when time interval exceeded
-- `precise` (bool) if True, increase time precision (useful for Windows)
-
-*Note:* The `precise=True` option uses a custom `Event` class to replace `threading.Event`, originally written by Chris D. (see below).
-
-## Methods
-
-```python
-timer.checkpt()  # Reference point for constant-duration loops, see above
-
-timer.pause()    # Immediately pause timer and put checkpt() in waiting phase
-timer.resume()   # Restart the elapsed time counter and unlock checkpt()
-
-timer.stop()     # Stop counting time and exit checkpt()
-timer.reset()    # Stop and restart timer immediately
-```
-
-## Properties (settable)
-
-```python
-timer.interval       # get interval (in s)
-timer.interval += 1  # increase interval by 1 second
-timer.interval = 10  # set interval to 10 seconds.
-
-timer.warnings          # get current status of warnings
-timer.warnings = True   # activate warnings if time between checkpts too short
-
-timer.name                      # optional name (for repr and warnings)
-timer.name = 'Countdown timer'  # (can also be set during instantiation)
-```
-
-## Attributes (read-only)
-
-```python
-# Most useful attributes
-timer.elapsed_time  # Time in seconds since init or last reset
-timer.pause_time    # total time (in s) the timer has been paused.
-timer.total_time    # Sum of the last two
-```
-
-## Background attributes and methods
-(mostly for development)
-```python
-timer.now()                 # Reference time used by all methods
-timer.start_time            # Ref. time corresponding to start/reset of timer
-timer.next_checkpt_release  # Ref. time at which next checkpt waittime is over
-timer.interval_exceeded     # (bool) True if loop contents take longer to execute than requested interval
-```
-
-## Notes
-
-- As mentioned previously, methods (and interval setting) take effect immediately, even if the timer is in a waiting phase.
-
-- After calling `pause()`, the `checkpt()` command blocks until `resume()` is called, however in the current version after `stop()` the `checkpt()` becomes non-blocking (equivalent to a `pass`), so that all following lines will be executed immediately and without any waiting time (i.e. as fast as possible if within a loop), until `timer.reset()` is called again. This means that it is useful to pin the condition of the loop to the stopping of the timer (see examples).
-
-
-## Timer accuracy
-
-See *performance.py* file of the module for functions to test the behavior and accuracy of the timer. In particular:
-```python
-from oclock.performance import performance_test
-performance_test(dt=0.01, nloops=1000, fmax=0.99, plot=True, warnings=False, precise=True)
-```
-tests the timing on 1000 loops of requested duration 0.01 second (10ms), using within the loop a function sleeping for a random amount of time between 0 and 0.99 dt (with `plot=True` option to see the results on a *matplotlib* graph, and `warnings=False` to not have a printed warning when the execution time of the nested commands exceed the target duration of the loop); `precise=True` uses the timer in precise mode.
-
-The *AccuracyTests.md* file gathers some accuracy results in Unix and Windows environments. In summary:
-
-- with **Unix**, time fluctuations are < 0.5 ms with the regular timer, and on the order of 0.01 ms (standard deviation) with the precise timer
-
-- with **Windows**, the regular timer fails quickly as frame rate is increased, due to fluctuations in the ~ 10 ms range. However the precise timer performs even better than in Unix, with fluctuations of less than 0.01 ms (standard deviation).
-
-
-## Behavior when interval is exceeded
-
-As explained above, it the contents of the loop take longer to execute than the requested time interval, the Timer simply moves on to the next loop but does not try to compensate for the extra time by making the next loop shorter:
-
-![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_interval_exceeded.png)
-
-
-
-# Development
-
-Install the package by cloning the GitHub repo (https://github.com/ovinc/oclock.git) and install in editable mode from the root of the repo:
-```
-pip install -e .
-```
-
-## Testing
-
-Package requirements to run the tests:
-- pytest
-- numpy
-
-General testing is done with *pytest* (from the root of the repository):
-```bash
-pytest
-```
-(**Note**: close the interactive countdown window at the end of the pytest run to finish the test.)
-
-Additional testing of interactive command line for real-time timer control can be done by running the example file from the root of the repository.
-```bash
-python -m example
-```
-
-See also *Accuracy Test* paragraph above to run performance tests for constant-duration loops with the `Timer` class.
-
-## Contributing
-
-Issues and Pull requests must be submitted on GitHub (https://github.com/ovinc/oclock) with commits (preferably squashed into a single commit) in branch *authors*.
-
-Version number is automatically extracted from git tag using *setuptools_scm*. Git tags are added by the repo's maintainer.
-
-# Requirements
-
-Python 3.x
-
-(Tests only made from python 3.5 to python 3.9 included)
-
-
-# Author
-
-Olivier Vincent
-
-(ovinc.py@gmail.com)
-
-# Contributors
-
-The `oclock.Event` class was originally written by Chris D.
-
-(https://stackoverflow.com/questions/48984512/making-a-timer-timeout-inaccuracy-of-threading-event-wait-python-3-6)
-
-
-# License
-
-GNU GPLv3, see *LICENSE* file
+Metadata-Version: 2.1
+Name: oclock
+Version: 1.3.1
+Summary: Tools for timed, no-drift loops of constant duration, and other misc. timing tools (GUI countdown, context managers etc.)
+Home-page: https://github.com/ovinc/oclock
+Author: Olivier Vincent
+Author-email: ovinc.py@gmail.com
+License: GNU GPLv3
+Keywords: timing,loops,constant duration,cancellable,modifiable,countdown,context manager,gui
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# About
+
+**oclock** is a Python 3 package. Its main goal is to provide a simple way to create timed loops with constant time intervals and no drift. It also provides various other timing tools and a GUI time.
+
+### Timed loops
+
+No drift, timed loops are based on the `Timer` class,
+- either using the `checkpt()` method at a location in a for/while loop acting as a reference point to maintain constant duration from one loop to the next,
+- or using the `@loop` or `@interactiveloop` decorators that use `Timer` and `checkpt()` in the background.
+
+The timing (interval) and execution (pause/stop etc.) can be modified in real time thanks to cancellable sleeping times.
+
+### Other tools
+
+- `Event`: class mimicking `threading.Event()` but with much better sleeping time accuracy.
+- `Countdown`: a class that starts a GUI countdown timer.
+- `parse_time()` function: returns a `datetime.timedelta` from a time string (e.g. `':2:25'`).
+- `measure_time()` and `measure_duration()` functions: are context managers for measuring time and execution times / time uncertainty of encapsulated commands.
+- Note that the `Timer` class can also be used as a regular chronometer with its methods `pause()`, `resume()`, `stop()` etc.
+
+# Quick start
+
+## Install
+
+```bash
+pip install oclock
+```
+
+## Timed Loops
+
+The `Timer` class is mostly designed to create loops of constant duration without drift, while allowing immediate modification/cancellation (sleep time interruption) in threaded environments. It can also be used as a regular chronometer.
+
+Below are some peudo-code quick-start examples. For complete, working examples, see:
+- *Examples.ipynb* notebook (https://github.com/ovinc/oclock/blob/master/Example.ipynb)
+- *example.py* script (https://github.com/ovinc/oclock/blob/master/example.py)
+
+
+### Constant-duration loops
+
+The most basic use of the `Timer()` class in Python code to create a loop of constant duration is:
+```python
+from oclock import Timer
+timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
+while condition:
+    my_function()  # can be of any duration between 0 and 2 seconds
+    timer.checkpt()
+```
+The `checkpt()` method waits the adequate amount of time to make the loop of constant duration, without drift (using a target regularly spaced in time); `condition` can include timer methods and attributes, e.g. `timer.elapsed_time < max_time`.
+
+Note that if *my_function()* takes longer to execute than the required time interval, the Timer class does not try to compensate the extra time by making the next loop shorter. It just aims at making the total duration of the next loop be the requested interval again (see *Behavior when interval is exceeded* section below).
+
+The same behavior can be achieved using the `@loop` decorator:
+```python
+from oclock import loop
+timer = Timer(interval=2)  # Loops will be of total duration 2 seconds
+@loop(timer)
+def my_function():
+    ...
+```
+Then, calling `my_function()` will execute the contents of the function in a repeated manner.
+
+The `@loop` execution exits automatically if the timer is stopped.
+Thus, It is useful to include a condition in `my_function` to exit the loop when needed, e.g.
+```python
+if timer.elapsed_time > t_max:
+    timer.stop()
+```
+
+### Interactive modification/cancellation
+
+The timer is also modifiable (change time interval) and cancellable in real time (i.e. even when the timer is in a `checkpt()` waiting phase). To do so, it must be accessed by another thread that runs concurrently. For example:
+
+```python
+from oclock import Timer
+from threading import Thread
+
+def user_input(timer):
+    """Threaded command line input to change time interval or exit timer."""
+    while not timer.is_stopped:
+        a = input()
+        try:
+            dt = float(a)
+        except ValueError:  # immediately cancel timer & exit all loops/threads
+            timer.stop()
+        else:               # immediately change interval to input value
+            timer.interval = dt
+
+timer = Timer(interval=2)
+Thread(target=user_input, args=(exit_event, timer)).start()
+
+while not timer.is_stopped:
+    my_function()
+    timer.checkpt()
+```
+During operation, the `Timer` object can be paused, resumed, stopped and reset using the corresponding `Timer` methods (see *Regular Timer* paragraph below). The *oclock* module also provides a simple command line interface to create a timed loop for a function and interact with it dynamically using the `@interactiveloop` decorator:
+```python
+from oclock import interactiveloop
+@interactiveloop(interval=2)
+def my_function():
+    ...
+```
+Now when `my_function()` is called, an interactive CLI thread starts at the same time where the user can pause/resume/reset/stop the timer in real time, change its interval, and print timing information.
+
+### Regular Timer
+
+Although not its main purpose, the `Timer` class can be used as a regular chronometer with the following methods (no need to be in a threaded environment, although the methods below whould work and be cancellable in a threaded environment):
+
+```python
+from oclock import Timer
+
+# The timer starts counting time immediately upon instantiation.
+timer = Timer()
+
+# Temporarily pause, then resume timer
+timer.pause()
+timer.resume()
+
+# Stop and restart timer completely
+timer.stop()
+timer.reset()  # note: can be called without calling stop() first
+
+# At any time, the elapsed time and total pause duration can be accessed with
+timer.elapsed_time
+timer.pause_time
+timer.total_time  # sum of the two other times
+```
+
+**Important Note**: Do not use the `checkpt()` method after a `pause()` call if not in a threaded environment, this will cause the program to be in a perpetual waiting state. In a threaded environment, call `resume()` to unpause.
+
+### Details
+
+See *Timer Class details* section below for all methods, properties and attributes and the *Development* section below for accuracy information.
+
+
+## Event class
+
+The `oclock.Event` class mimicks `threading.Event` (https://docs.python.org/3/library/threading.html#event-objects) but provides much better sleep time accuracy.
+
+Available methods are the same as for `threading.Event`:
+- `set()`
+- `clear()`
+- `is_set()`
+- `wait()`
+
+
+Below are comments from Chris D. who originally posted the code for this class on StackOverflow (see *Contributors* at the end of this file):
+
+> Internally, it uses a combination of a time.sleep() loop and a busy loop for greatly increased precision. The sleep loop runs in a separate thread so that the blocking wait() call in the main thread can still be immediately interrupted. When the set() method is called, the sleep thread should terminate shortly afterwards. Also, in order to minimize CPU utilization, I made sure that the busy loop will never run for more than 3 milliseconds.
+
+
+## Countdown GUI
+
+A simple graphical countdown timer based on the `Timer` class. It can be used either as a python main program from a shell, or as a function in Python code or console.
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/countdown.gif)
+
+From a terminal:
+```bash
+python -m oclock 1:45:00   # start timer of duration 1 hour 45 minutes
+python -m oclock 1:45:     # exactly the same as above
+python -m oclock 00:02:00  # start 2-minute timer
+python -m oclock :2:       # exactly the same as above
+python -m oclock 00:00:05  # start 5-second timer
+python -m oclock ::5       # exactly the same as above
+```
+
+In python:
+```python
+from oclock import Countdown
+Countdown('1:45:')         # start timer of duration 1 hour 45 minutes
+```
+(the inputs are of the same format as from the terminal, see above).
+
+When countdown is finished, 'Done' is displayed for 5 seconds in the GUI while the console displays *Countdown finished* and emits a sound. Then the time passed since the end of countdown is displayed as a negative value in red. The program stops when the GUI window is closed.
+
+## Parse time function
+
+The `parse_time()` function is used in the argument parsing of the countdown GUI from a terminal (see above). It transforms a string in the form `'h:m:s'` into a `datetime.timedelta` object. Inputs of the form e.g. `'::5'` or `:2:`, `'3:30:'` are acceptable for 5 seconds, 2 minutes, and 3.5 hours, respectively.
+```python
+>>> parse_time(':2:30')
+datetime.timedelta(seconds=150)
+```
+
+## Context managers to record timing of commands
+
+The `measure_time()` function is a context manager that saves the timing info of the encapsulated commands. This can be e.g. used in scientific experiments to get the time and time uncertainty associated with a measurement.
+```python
+from oclock import measure_time, measure_duration
+
+# ----------------------------------------------------------------------------
+# Examples where one just wants to get timing info ---------------------------
+# ----------------------------------------------------------------------------
+
+with measure_time() as timing:
+    my_function()
+print(timing)
+
+# Out: {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
+
+# (dt (s) is half the total duration. To get the total duration instead, do:)
+
+with measure_duration() as duration:
+    my_function()
+print(duration)
+
+# Out: {'duration (s)': 1.1689763555421325}
+
+# ----------------------------------------------------------------------------
+# Example where the timing info is directly added to a data dictionary -------
+# ----------------------------------------------------------------------------
+
+with measure_time() as data:
+    measurement = my_function()  # returns e.g. 3.618
+    data['measurement'] = measurement
+print(data)
+
+# Out: {'measurement': 3.618,
+#       'time (unix)': 1604780958.0705943,
+#       'dt (s)': 0.6218999624252319}
+```
+
+
+# Timer Class details
+
+## Instantiation
+
+```python
+from oclock import Timer
+timer = Timer(interval=1, name='Timer', warnings=False, precise=False)
+```
+
+Parameters:
+- `interval` (float): timer interval in seconds
+- `name` (str): optional name for description purposes (repr and warnings)
+- `warnings` (bool): If True, prints warning when time interval exceeded
+- `precise` (bool) if True, increase time precision (useful for Windows)
+
+*Note:* The `precise=True` option uses a custom `Event` class to replace `threading.Event`, originally written by Chris D. (see below).
+
+## Methods
+
+```python
+timer.checkpt()  # Reference point for constant-duration loops, see above
+
+timer.pause()    # Immediately pause timer and put checkpt() in waiting phase
+timer.resume()   # Restart the elapsed time counter and unlock checkpt()
+
+timer.stop()     # Stop counting time and exit checkpt()
+timer.reset()    # Stop and restart timer immediately
+
+# Change timer interval
+timer.set_interval(...)  # immediately, equivalent to timer.interval = ...
+timer.set_interval(..., immediate=False)   # wait next checkpt
+```
+
+## Properties (settable)
+
+```python
+timer.interval       # get interval (in s)
+timer.interval += 1  # increase interval by 1 second
+timer.interval = 10  # set interval to 10 seconds.
+
+timer.warnings          # get current status of warnings
+timer.warnings = True   # activate warnings if time between checkpts too short
+
+timer.name                      # optional name (for repr and warnings)
+timer.name = 'Countdown timer'  # (can also be set during instantiation)
+```
+
+## Attributes (read-only)
+
+```python
+# Most useful attributes
+timer.elapsed_time  # Time in seconds since init or last reset
+timer.pause_time    # total time (in s) the timer has been paused.
+timer.total_time    # Sum of the last two
+```
+
+## Background attributes and methods
+(mostly for development)
+```python
+timer.now()                 # Reference time used by all methods
+timer.start_time            # Ref. time corresponding to start/reset of timer
+timer.next_checkpt_release  # Ref. time at which next checkpt waittime is over
+timer.interval_exceeded     # (bool) True if loop contents take longer to execute than requested interval
+```
+
+## Notes
+
+- As mentioned previously, methods (and interval setting) take effect immediately, even if the timer is in a waiting phase. It is however possible to wait for the next checkpt to apply a new timer interval, by using the `immediate=False` option in `set_interval()` (see example in the *Examples.ipynb* notebook).
+
+- After calling `pause()`, the `checkpt()` command blocks until `resume()` is called, however in the current version after `stop()` the `checkpt()` becomes non-blocking (equivalent to a `pass`), so that all following lines will be executed immediately and without any waiting time (i.e. as fast as possible if within a loop), until `timer.reset()` is called again. This means that it is useful to pin the condition of the loop to the stopping of the timer (see examples).
+
+
+## Timer accuracy
+
+See *performance.py* file of the module for functions to test the behavior and accuracy of the timer. In particular:
+```python
+from oclock.performance import performance_test
+performance_test(dt=0.01, nloops=1000, fmax=0.99, plot=True, warnings=False, precise=True)
+```
+tests the timing on 1000 loops of requested duration 0.01 second (10ms), using within the loop a function sleeping for a random amount of time between 0 and 0.99 dt (with `plot=True` option to see the results on a *matplotlib* graph, and `warnings=False` to not have a printed warning when the execution time of the nested commands exceed the target duration of the loop); `precise=True` uses the timer in precise mode.
+
+The *AccuracyTests.md* file gathers some accuracy results in Unix and Windows environments. In summary:
+
+- with **Unix**, time fluctuations are < 0.5 ms with the regular timer, and on the order of 0.01 ms (standard deviation) with the precise timer
+
+- with **Windows**, the regular timer fails quickly as frame rate is increased, due to fluctuations in the ~ 10 ms range. However the precise timer performs even better than in Unix, with fluctuations of less than 0.01 ms (standard deviation).
+
+
+## Behavior when interval is exceeded
+
+As explained above, it the contents of the loop take longer to execute than the requested time interval, the Timer simply moves on to the next loop but does not try to compensate for the extra time by making the next loop shorter:
+
+![](https://raw.githubusercontent.com/ovinc/oclock/master/media/img/timer_interval_exceeded.png)
+
+
+
+# Development
+
+Install the package by cloning the GitHub repo (https://github.com/ovinc/oclock.git) and install in editable mode from the root of the repo:
+```
+pip install -e .
+```
+
+## Testing
+
+Package requirements to run the tests:
+- pytest
+- numpy
+
+General testing is done with *pytest* (from the root of the repository):
+```bash
+pytest
+```
+(**Note**: close the interactive countdown window at the end of the pytest run to finish the test.)
+
+Additional testing of interactive command line for real-time timer control can be done by running the example file from the root of the repository.
+```bash
+python -m example
+```
+
+See also *Accuracy Test* paragraph above to run performance tests for constant-duration loops with the `Timer` class.
+
+## Contributing
+
+Issues and Pull requests must be submitted on GitHub (https://github.com/ovinc/oclock) with commits (preferably squashed into a single commit) in branch *authors*.
+
+Version number is automatically extracted from git tag using *setuptools_scm*. Git tags are added by the repo's maintainer.
+
+# Requirements
+
+Python 3.x
+
+(Tests only made from python 3.5 to python 3.9 included)
+
+
+# Author
+
+Olivier Vincent
+
+(ovinc.py@gmail.com)
+
+# Contributors
+
+The `oclock.Event` class was originally written by Chris D.
+
+(https://stackoverflow.com/questions/48984512/making-a-timer-timeout-inaccuracy-of-threading-event-wait-python-3-6)
+
+
+# License
+
+GNU GPLv3, see *LICENSE* file
```

### Comparing `oclock-1.3.0/media/countdown.gif` & `oclock-1.3.1/media/countdown.gif`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_macos_1000ms.png` & `oclock-1.3.1/media/img/precisetimer_macos_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_macos_100ms.png` & `oclock-1.3.1/media/img/precisetimer_macos_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_macos_10ms.png` & `oclock-1.3.1/media/img/precisetimer_macos_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_macos_1ms.png` & `oclock-1.3.1/media/img/precisetimer_macos_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_macos_40ms.png` & `oclock-1.3.1/media/img/precisetimer_macos_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_windows_1000ms.png` & `oclock-1.3.1/media/img/precisetimer_windows_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_windows_100ms.png` & `oclock-1.3.1/media/img/precisetimer_windows_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_windows_10ms.png` & `oclock-1.3.1/media/img/precisetimer_windows_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_windows_1ms.png` & `oclock-1.3.1/media/img/precisetimer_windows_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/precisetimer_windows_40ms.png` & `oclock-1.3.1/media/img/precisetimer_windows_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/ribosome.png` & `oclock-1.3.1/media/img/ribosome.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_interval_exceeded.png` & `oclock-1.3.1/media/img/timer_interval_exceeded.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_macos_1000ms.png` & `oclock-1.3.1/media/img/timer_macos_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_macos_100ms.png` & `oclock-1.3.1/media/img/timer_macos_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_macos_10ms.png` & `oclock-1.3.1/media/img/timer_macos_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_macos_1ms.png` & `oclock-1.3.1/media/img/timer_macos_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_macos_40ms.png` & `oclock-1.3.1/media/img/timer_macos_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_windows_1000ms.png` & `oclock-1.3.1/media/img/timer_windows_1000ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_windows_100ms.png` & `oclock-1.3.1/media/img/timer_windows_100ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_windows_10ms.png` & `oclock-1.3.1/media/img/timer_windows_10ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_windows_1ms.png` & `oclock-1.3.1/media/img/timer_windows_1ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/media/img/timer_windows_40ms.png` & `oclock-1.3.1/media/img/timer_windows_40ms.png`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/oclock/__init__.py` & `oclock-1.3.1/oclock/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-"""Timing tools, including cancellable timers for loops of constant duration."""
-
-# ----------------------------- License information --------------------------
-
-# This file is part of the oclock python package.
-# Copyright (C) 2021 Olivier Vincent
-
-# The oclock package is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# The oclock package is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with the oclock python package.
-# If not, see <https://www.gnu.org/licenses/>
-
-
-from .timer import Timer
-from .countdown import Countdown
-from .general import parse_time, measure_time, measure_duration
-from .loop import loop, interactiveloop
-from .event import Event
-
-# from importlib.metadata import version (only for python 3.8+)
-from importlib_metadata import version
-
-__version__ = version('oclock')
-__author__ = 'Olivier Vincent'
-__license__ = 'GNU GPLv3'
+"""Manage command line parsing for the oclock module."""
+
+# ----------------------------- License information --------------------------
+
+# This file is part of the oclock python package.
+# Copyright (C) 2021 Olivier Vincent
+
+# The oclock package is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# The oclock package is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with the oclock python package.
+# If not, see <https://www.gnu.org/licenses/>
+
+
+import argparse
+
+from .countdown import Countdown
+
+
+descr = "GUI countdown clock based on the oclock module."
+
+parser = argparse.ArgumentParser(description=descr,
+                                 formatter_class=argparse.RawTextHelpFormatter)
+
+msg = "Input time in hh:mm:ss format, e.g. 10:30:00, or ::5 (5 seconds)"
+
+# The nargs='?' is to have a positional argument with a default value
+parser.add_argument('time', type=str, nargs='?', help=msg)
+
+args = parser.parse_args()
+countdown = Countdown(args.time)
```

### Comparing `oclock-1.3.0/oclock/countdown.py` & `oclock-1.3.1/oclock/countdown.py`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/oclock/general.py` & `oclock-1.3.1/oclock/general.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-"""General functions and tools for the oclock package."""
-
-# ----------------------------- License information --------------------------
-
-# This file is part of the oclock python package.
-# Copyright (C) 2021 Olivier Vincent
-
-# The oclock package is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# The oclock package is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with the oclock python package.
-# If not, see <https://www.gnu.org/licenses/>
-
-
-import time
-from datetime import timedelta
-from contextlib import contextmanager
-
-
-def parse_time(time_str):
-    """Transforms inputs in the form h:m:s in a h, m, s tuple.
-
-    Input
-    -----
-    time_str: str (e.g. ::5 for 5 seconds or 1:30: for 1.5 hours)
-    (see examples below)
-
-    Output
-    ------
-    datetime.timedelta object
-
-    Examples
-    --------
-    '3:14:16'   --> 3 hours, 14 minutes, 16 seconds
-    '1:45:00'   --> 1 hour 45 minutes
-    '1:45:'     --> 1 hour 45 minutes
-    '00:02:00'  --> 2 minutes
-    ':2:'       --> 2 minutes
-    '00:00:05'  --> 5 seconds
-    '::5'       --> 5 seconds
-    """
-    timestr = time_str.split(':')
-    tint = []
-
-    for tstr in timestr:
-        try:
-            t = int(tstr)
-        except ValueError:
-            t = 0
-        tint.append(t)
-
-    h, m, s = tint
-    duration = timedelta(hours=h, minutes=m, seconds=s)
-    return duration
-
-
-@contextmanager
-def measure_time():
-    """Measure mean unix time (s) and time uncertainty (s) of encapsulated commands.
-
-    Output
-    ------
-    Dictionary with keys:
-        - 'time (unix)': (tmax + tmin) / 2
-        - 'dt (s)': (tmax - tmin) / 2
-
-    where tmin, tmax are the unix times before the instructions and after the
-    instructions, respectively.
-
-    Examples
-    --------
-    >>> with measure_time() as timing:
-            my_function()
-        print(timing)
-
-    Out:
-    {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
-
-    >>> with measure_time() as data:
-            measurement = my_function()  # returns e.g. 3.618
-            data['measurement'] = measurement
-        print(data)
-
-    Out:
-    {'measurement': 3.618,
-     'time (unix)': 1604780958.0705943,
-     'dt (s)': 0.6218999624252319}
-    """
-    timing = {}
-    t1 = time.time()
-    t1p = time.perf_counter()
-    try:
-        yield timing
-    finally:
-        t2 = time.time()
-        t2p = time.perf_counter()
-        dt = (t2p - t1p) / 2
-        t = (t1 + t2) / 2
-        timing['time (unix)'] = t
-        timing['dt (s)'] = dt
-
-
-@contextmanager
-def measure_duration():
-    """Measure duration (s) of encapsulated commands.
-
-    Output
-    ------
-    Dict with total duration in seconds (key 'duration (s)')
-
-    Example
-    -------
-    >>> with measure_duration() as duration:
-            my_function()
-        print(duration)
-
-    Out:
-    {'duration (s)': 0.9871297000004233}
-    """
-    duration = {}
-    t1 = time.perf_counter()
-    try:
-        yield duration
-    finally:
-        t2 = time.perf_counter()
-        duration['duration (s)'] = t2 - t1
+"""General functions and tools for the oclock package."""
+
+# ----------------------------- License information --------------------------
+
+# This file is part of the oclock python package.
+# Copyright (C) 2021 Olivier Vincent
+
+# The oclock package is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# The oclock package is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with the oclock python package.
+# If not, see <https://www.gnu.org/licenses/>
+
+
+import time
+from datetime import timedelta
+from contextlib import contextmanager
+
+
+def parse_time(time_str):
+    """Transforms inputs in the form h:m:s in a h, m, s tuple.
+
+    Input
+    -----
+    time_str: str (e.g. ::5 for 5 seconds or 1:30: for 1.5 hours)
+    (see examples below)
+
+    Output
+    ------
+    datetime.timedelta object
+
+    Examples
+    --------
+    '3:14:16'   --> 3 hours, 14 minutes, 16 seconds
+    '1:45:00'   --> 1 hour 45 minutes
+    '1:45:'     --> 1 hour 45 minutes
+    '00:02:00'  --> 2 minutes
+    ':2:'       --> 2 minutes
+    '00:00:05'  --> 5 seconds
+    '::5'       --> 5 seconds
+    """
+    timestr = time_str.split(':')
+    tint = []
+
+    for tstr in timestr:
+        try:
+            t = int(tstr)
+        except ValueError:
+            t = 0
+        tint.append(t)
+
+    h, m, s = tint
+    duration = timedelta(hours=h, minutes=m, seconds=s)
+    return duration
+
+
+@contextmanager
+def measure_time():
+    """Measure mean unix time (s) and time uncertainty (s) of encapsulated commands.
+
+    Output
+    ------
+    Dictionary with keys:
+        - 'time (unix)': (tmax + tmin) / 2
+        - 'dt (s)': (tmax - tmin) / 2
+
+    where tmin, tmax are the unix times before the instructions and after the
+    instructions, respectively.
+
+    Examples
+    --------
+    >>> with measure_time() as timing:
+            my_function()
+        print(timing)
+
+    Out:
+    {'time (unix)': 1604780958.0705943, 'dt (s)': 0.6218999624252319}
+
+    >>> with measure_time() as data:
+            measurement = my_function()  # returns e.g. 3.618
+            data['measurement'] = measurement
+        print(data)
+
+    Out:
+    {'measurement': 3.618,
+     'time (unix)': 1604780958.0705943,
+     'dt (s)': 0.6218999624252319}
+    """
+    timing = {}
+    t1 = time.time()
+    t1p = time.perf_counter()
+    try:
+        yield timing
+    finally:
+        t2 = time.time()
+        t2p = time.perf_counter()
+        dt = (t2p - t1p) / 2
+        t = (t1 + t2) / 2
+        timing['time (unix)'] = t
+        timing['dt (s)'] = dt
+
+
+@contextmanager
+def measure_duration():
+    """Measure duration (s) of encapsulated commands.
+
+    Output
+    ------
+    Dict with total duration in seconds (key 'duration (s)')
+
+    Example
+    -------
+    >>> with measure_duration() as duration:
+            my_function()
+        print(duration)
+
+    Out:
+    {'duration (s)': 0.9871297000004233}
+    """
+    duration = {}
+    t1 = time.perf_counter()
+    try:
+        yield duration
+    finally:
+        t2 = time.perf_counter()
+        duration['duration (s)'] = t2 - t1
```

### Comparing `oclock-1.3.0/oclock/loop.py` & `oclock-1.3.1/oclock/loop.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-"""Use the timer class for timed loops without drift."""
-
-# ----------------------------- License information --------------------------
-
-# This file is part of the oclock python package.
-# Copyright (C) 2021 Olivier Vincent
-
-# The oclock package is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# The oclock package is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with the oclock python package.
-# If not, see <https://www.gnu.org/licenses/>
-
-
-from threading import Thread
-from functools import wraps
-
-from . import Timer
-
-
-# ============== Command Line Interface to interact with Timer ===============
-
-
-def cli(timer):
-    """Command line input to interact with a timer object.
-
-    Possible Inputs
-    ---------------
-    - any number (int/float): change timer interval to that new value
-    - 'p' or 'pause': pause timer
-    - 'r' or 'resume': resume timer
-    - 'R' or 'reset': reset timer
-    - 't' or 'time': print timing (interval, elapsed time, etc.) info
-    - 'q', 'Q', 'quit' or 'stop': stop timer and exit
-    """
-    msg = '-----------------------------------------------------------------\n'\
-          'Timer Command-Line-Interface. Possible inputs:\n' \
-          '- any number (int/float): change timer interval to that new value\n' \
-          "- 'p' or 'pause': pause timer\n" \
-          "- 'r' or 'resume': resume timer\n" \
-          "- 'R' or 'reset': reset timer\n" \
-          "- 't' or 'time': print timing (interval, elapsed time, etc.) info\n"\
-          "- 'q', 'Q', 'quit' or 'stop': stop timer and exit\n" \
-          '-----------------------------------------------------------------\n'
-    print(msg)
-
-    while not timer.is_stopped:
-        a = input()
-        try:
-            dt = float(a)
-        except ValueError:
-            if a in ('p', 'pause'):
-                print('--- Timer Paused')
-                timer.pause()
-            elif a in ('r', 'resume'):
-                print('--- Timer Resumed')
-                timer.resume()
-            elif a in ('R', 'reset'):
-                print('--- Timer Restarted')
-                timer.reset()
-            elif a in ('t', 'time'):
-                elapsed = timer.elapsed_time
-                paused = timer.pause_time
-                dt = timer.interval
-                tnext = timer.next_checkpt_release - timer.now()
-                print("[Interval {:.3f}] [Elapsed: {:.3f}] [Paused {:.3f}] "
-                      "[Next {:.3f}]".format(dt, elapsed, paused, tnext))
-            elif a in ('q', 'Q', 'quit', 'stop'):
-                print('--- Timer Stopped')
-                timer.stop()
-            else:
-                pass
-        else:
-            try:
-                timer.interval = dt
-            except ValueError:
-                print('--- Invalid Interval')
-            else:
-                print('--- Interval (s) changed to {}'.format(dt))
-
-    print('--- Loop Exited')
-
-
-# ========== Decorators to repeat function periodically using Timer ==========
-
-
-def loop(timer):
-    """Decorator to start a timed loop repeating a function periodically.
-
-    Parameters
-    ----------
-    - timer: oclock.Timer object
-    """
-    def decorator(function):
-        @wraps(function)
-        def wrapper(*args, **kwargs):
-            while not timer.is_stopped:
-                timer.checkpt()
-                function(*args, **kwargs)
-        return wrapper
-    return decorator
-
-
-def interactiveloop(**timer_kwargs):
-    """Decorator to start an interactive CLI for timed execution of a function
-
-    Parameters
-    ----------
-    any argument or keyword-argument taken by oclock.Timer(), e.g. 'interval'
-    """
-    def decorator(function):
-        @wraps(function)
-        def wrapper(*args, **kwargs):
-            timer = Timer(**timer_kwargs)
-            Thread(target=cli, args=(timer,)).start()
-            timer.reset()  # removes any delay introduced by thread starting
-            while not timer.is_stopped:
-                function(*args, **kwargs)
-                timer.checkpt()
-        return wrapper
-    return decorator
+"""Use the timer class for timed loops without drift."""
+
+# ----------------------------- License information --------------------------
+
+# This file is part of the oclock python package.
+# Copyright (C) 2021 Olivier Vincent
+
+# The oclock package is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# The oclock package is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with the oclock python package.
+# If not, see <https://www.gnu.org/licenses/>
+
+
+from threading import Thread
+from functools import wraps
+
+from . import Timer
+
+
+# ============== Command Line Interface to interact with Timer ===============
+
+
+def cli(timer):
+    """Command line input to interact with a timer object.
+
+    Possible Inputs
+    ---------------
+    - any number (int/float): change timer interval to that new value
+    - 'p' or 'pause': pause timer
+    - 'r' or 'resume': resume timer
+    - 'R' or 'reset': reset timer
+    - 't' or 'time': print timing (interval, elapsed time, etc.) info
+    - 'q', 'Q', 'quit' or 'stop': stop timer and exit
+    """
+    msg = '-----------------------------------------------------------------\n'\
+          'Timer Command-Line-Interface. Possible inputs:\n' \
+          '- any number (int/float): change timer interval to that new value\n' \
+          "- 'p' or 'pause': pause timer\n" \
+          "- 'r' or 'resume': resume timer\n" \
+          "- 'R' or 'reset': reset timer\n" \
+          "- 't' or 'time': print timing (interval, elapsed time, etc.) info\n"\
+          "- 'q', 'Q', 'quit' or 'stop': stop timer and exit\n" \
+          '-----------------------------------------------------------------\n'
+    print(msg)
+
+    while not timer.is_stopped:
+        a = input()
+        try:
+            dt = float(a)
+        except ValueError:
+            if a in ('p', 'pause'):
+                print('--- Timer Paused')
+                timer.pause()
+            elif a in ('r', 'resume'):
+                print('--- Timer Resumed')
+                timer.resume()
+            elif a in ('R', 'reset'):
+                print('--- Timer Restarted')
+                timer.reset()
+            elif a in ('t', 'time'):
+                elapsed = timer.elapsed_time
+                paused = timer.pause_time
+                dt = timer.interval
+                tnext = timer.next_checkpt_release - timer.now()
+                print("[Interval {:.3f}] [Elapsed: {:.3f}] [Paused {:.3f}] "
+                      "[Next {:.3f}]".format(dt, elapsed, paused, tnext))
+            elif a in ('q', 'Q', 'quit', 'stop'):
+                print('--- Timer Stopped')
+                timer.stop()
+            else:
+                pass
+        else:
+            try:
+                timer.interval = dt
+            except ValueError:
+                print('--- Invalid Interval')
+            else:
+                print('--- Interval (s) changed to {}'.format(dt))
+
+    print('--- Loop Exited')
+
+
+# ========== Decorators to repeat function periodically using Timer ==========
+
+
+def loop(timer):
+    """Decorator to start a timed loop repeating a function periodically.
+
+    Parameters
+    ----------
+    - timer: oclock.Timer object
+    """
+    def decorator(function):
+        @wraps(function)
+        def wrapper(*args, **kwargs):
+            while not timer.is_stopped:
+                timer.checkpt()
+                function(*args, **kwargs)
+        return wrapper
+    return decorator
+
+
+def interactiveloop(**timer_kwargs):
+    """Decorator to start an interactive CLI for timed execution of a function
+
+    Parameters
+    ----------
+    any argument or keyword-argument taken by oclock.Timer(), e.g. 'interval'
+    """
+    def decorator(function):
+        @wraps(function)
+        def wrapper(*args, **kwargs):
+            timer = Timer(**timer_kwargs)
+            Thread(target=cli, args=(timer,)).start()
+            timer.reset()  # removes any delay introduced by thread starting
+            while not timer.is_stopped:
+                function(*args, **kwargs)
+                timer.checkpt()
+        return wrapper
+    return decorator
```

### Comparing `oclock-1.3.0/oclock/performance.py` & `oclock-1.3.1/oclock/performance.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""Test accuracy of timer for constant-duration loops."""
-
-# ----------------------------- License information --------------------------
-
-# This file is part of the oclock python package.
-# Copyright (C) 2021 Olivier Vincent
-
-# The oclock package is free software: you can redistribute it and/or modify
-# it under the terms of the GNU General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-
-# The oclock package is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU General Public License for more details.
-
-# You should have received a copy of the GNU General Public License
-# along with the oclock python package.
-# If not, see <https://www.gnu.org/licenses/>
-
-
-import time
-from random import random
-from queue import Queue
-
-import numpy as np
-
-from . import Timer, measure_duration
-
-
-def constant_duration_loop(timer, q, fracmax=0.5, n=10):
-    """Try maintain loop timing constant with a function of random timing.
-
-    - timer is a timer object from the oclock module
-    - q is a queue that sends the data away from the loop for plotting
-    - fracmax is the max fraction of the interval the random time can be
-    - n is the number of loops
-    """
-    ts = []  # stores the times of the loop after the checkpt() call
-    rs = []  # stores the random times generated
-
-    timer.reset()  # Not obligatory, but ensures timing is counted from here.
-
-    t0 = time.perf_counter()
-    ts.append(t0)
-
-    for i in range(n):
-
-        # wait for a random time between 0 and the total requested interval / 2
-        with measure_duration() as duration:
-            r = timer.interval * fracmax * random()
-            time.sleep(r)
-        sleeptime = duration['duration (s)']
-
-        # this is where the timer adapts the wait time to the execution time
-        # of the lines above.
-        timer.checkpt()
-
-        t = time.perf_counter()
-
-        ts.append(t)
-        rs.append(sleeptime)
-
-    return np.array(ts), np.array(rs)
-
-
-def performance_test(dt, nloops, fmax, plot=False, warnings=False, precise=False):
-    """Test accuracy of the constant-loop timing using random timing in loop.
-
-    - dt is the requested total duration of the loop
-    - nloops is the total number of loops
-    - fmax is the max fraction of dt that can be taken by the random time.
-    - plot: if True, show plot (matplotlib) of timing of all loops
-    - warnings: if True, prints a warning when time interval too short
-    - precise: if True, increase time precision (useful for Windows)
-    """
-    timer = Timer(interval=dt, warnings=warnings, precise=precise)
-    q = Queue()
-
-    print('Test Started')
-    ts, rs = constant_duration_loop(timer, q, fmax, nloops)
-    print('Test Finished')
-
-    dts = np.diff(ts)
-    avg = dts.mean()
-    dev = dts.std()
-
-    print("Mean dt (s): {}, std: {}".format(avg, dev))
-    print("Mean dt - Requested dt (ms): {}".format((avg - dt) * 1000))
-    print("Std dev (ms): {}".format(dev * 1000))
-
-    if plot:
-
-        import matplotlib.pyplot as plt
-        fig, ax = plt.subplots(figsize=(6, 4))
-
-        n = len(dts)
-        ii = range(1, n + 1)
-
-        ax.plot([1, n], [dt * 1000, dt * 1000], '-', c='antiquewhite',
-                linewidth=6, label='requested duration')
-
-        ax.fill_between(ii, rs * 1000, label='random time', color='0.9')
-
-        ax.plot(ii, dts * 1000, '.', c='steelblue',
-                label='individual loop duration')
-
-        ax.plot([1, n], [avg * 1000, avg * 1000], ':', c='sandybrown',
-                linewidth=4, label='average loop duration')
-
-        ax.set_xlim((1, n))
-        ax.set_ylim((0, dts.max() * 1050))
-
-        ax.set_xlabel('loop number')
-        ax.set_ylabel(r'$\Delta t$ (ms)')
-
-        ax.grid()
-        ax.legend()
-        plt.show()
-
-    return {'mean dt (s)': avg, 'std dev (s)': dev}
+"""Test accuracy of timer for constant-duration loops."""
+
+# ----------------------------- License information --------------------------
+
+# This file is part of the oclock python package.
+# Copyright (C) 2021 Olivier Vincent
+
+# The oclock package is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# The oclock package is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
+
+# You should have received a copy of the GNU General Public License
+# along with the oclock python package.
+# If not, see <https://www.gnu.org/licenses/>
+
+
+import time
+from random import random
+from queue import Queue
+
+import numpy as np
+
+from . import Timer, measure_duration
+
+
+def constant_duration_loop(timer, q, fracmax=0.5, n=10):
+    """Try maintain loop timing constant with a function of random timing.
+
+    - timer is a timer object from the oclock module
+    - q is a queue that sends the data away from the loop for plotting
+    - fracmax is the max fraction of the interval the random time can be
+    - n is the number of loops
+    """
+    ts = []  # stores the times of the loop after the checkpt() call
+    rs = []  # stores the random times generated
+
+    timer.reset()  # Not obligatory, but ensures timing is counted from here.
+
+    t0 = time.perf_counter()
+    ts.append(t0)
+
+    for i in range(n):
+
+        # wait for a random time between 0 and the total requested interval / 2
+        with measure_duration() as duration:
+            r = timer.interval * fracmax * random()
+            time.sleep(r)
+        sleeptime = duration['duration (s)']
+
+        # this is where the timer adapts the wait time to the execution time
+        # of the lines above.
+        timer.checkpt()
+
+        t = time.perf_counter()
+
+        ts.append(t)
+        rs.append(sleeptime)
+
+    return np.array(ts), np.array(rs)
+
+
+def performance_test(dt, nloops, fmax, plot=False, warnings=False, precise=False):
+    """Test accuracy of the constant-loop timing using random timing in loop.
+
+    - dt is the requested total duration of the loop
+    - nloops is the total number of loops
+    - fmax is the max fraction of dt that can be taken by the random time.
+    - plot: if True, show plot (matplotlib) of timing of all loops
+    - warnings: if True, prints a warning when time interval too short
+    - precise: if True, increase time precision (useful for Windows)
+    """
+    timer = Timer(interval=dt, warnings=warnings, precise=precise)
+    q = Queue()
+
+    print('Test Started')
+    ts, rs = constant_duration_loop(timer, q, fmax, nloops)
+    print('Test Finished')
+
+    dts = np.diff(ts)
+    avg = dts.mean()
+    dev = dts.std()
+
+    print("Mean dt (s): {}, std: {}".format(avg, dev))
+    print("Mean dt - Requested dt (ms): {}".format((avg - dt) * 1000))
+    print("Std dev (ms): {}".format(dev * 1000))
+
+    if plot:
+
+        import matplotlib.pyplot as plt
+        fig, ax = plt.subplots(figsize=(6, 4))
+
+        n = len(dts)
+        ii = range(1, n + 1)
+
+        ax.plot([1, n], [dt * 1000, dt * 1000], '-', c='antiquewhite',
+                linewidth=6, label='requested duration')
+
+        ax.fill_between(ii, rs * 1000, label='random time', color='0.9')
+
+        ax.plot(ii, dts * 1000, '.', c='steelblue',
+                label='individual loop duration')
+
+        ax.plot([1, n], [avg * 1000, avg * 1000], ':', c='sandybrown',
+                linewidth=4, label='average loop duration')
+
+        ax.set_xlim((1, n))
+        ax.set_ylim((0, dts.max() * 1050))
+
+        ax.set_xlabel('loop number')
+        ax.set_ylabel(r'$\Delta t$ (ms)')
+
+        ax.grid()
+        ax.legend()
+        plt.show()
+
+    return {'mean dt (s)': avg, 'std dev (s)': dev}
```

### Comparing `oclock-1.3.0/oclock.egg-info/SOURCES.txt` & `oclock-1.3.1/oclock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oclock-1.3.0/setup.cfg` & `oclock-1.3.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,65 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206f 636c 6f63 6b0d 0a61 7574 686f   = oclock..autho
-00000020: 7220 3d20 4f6c 6976 6965 7220 5669 6e63  r = Olivier Vinc
-00000030: 656e 740d 0a61 7574 686f 725f 656d 6169  ent..author_emai
-00000040: 6c20 3d20 6f76 696e 632e 7079 4067 6d61  l = ovinc.py@gma
-00000050: 696c 2e63 6f6d 0d0a 7572 6c20 3d20 6874  il.com..url = ht
-00000060: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000070: 2f6f 7669 6e63 2f6f 636c 6f63 6b0d 0a64  /ovinc/oclock..d
-00000080: 6573 6372 6970 7469 6f6e 203d 2054 6f6f  escription = Too
-00000090: 6c73 2066 6f72 2074 696d 6564 2c20 6e6f  ls for timed, no
-000000a0: 2d64 7269 6674 206c 6f6f 7073 206f 6620  -drift loops of 
-000000b0: 636f 6e73 7461 6e74 2064 7572 6174 696f  constant duratio
-000000c0: 6e2c 2061 6e64 206f 7468 6572 206d 6973  n, and other mis
-000000d0: 632e 2074 696d 696e 6720 746f 6f6c 7320  c. timing tools 
-000000e0: 2847 5549 2063 6f75 6e74 646f 776e 2c20  (GUI countdown, 
-000000f0: 636f 6e74 6578 7420 6d61 6e61 6765 7273  context managers
-00000100: 2065 7463 2e29 0d0a 6c6f 6e67 5f64 6573   etc.)..long_des
-00000110: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-00000120: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-00000130: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-00000140: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000150: 2f6d 6172 6b64 6f77 6e0d 0a6b 6579 776f  /markdown..keywo
-00000160: 7264 7320 3d20 7469 6d69 6e67 2c20 6c6f  rds = timing, lo
-00000170: 6f70 732c 2063 6f6e 7374 616e 7420 6475  ops, constant du
-00000180: 7261 7469 6f6e 2c20 6361 6e63 656c 6c61  ration, cancella
-00000190: 626c 652c 206d 6f64 6966 6961 626c 652c  ble, modifiable,
-000001a0: 2063 6f75 6e74 646f 776e 2c20 636f 6e74   countdown, cont
-000001b0: 6578 7420 6d61 6e61 6765 722c 2067 7569  ext manager, gui
-000001c0: 0d0a 6c69 6365 6e73 655f 6669 6c65 7320  ..license_files 
-000001d0: 3d20 4c49 4345 4e53 450d 0a6c 6963 656e  = LICENSE..licen
-000001e0: 7365 203d 2047 4e55 2047 504c 7633 0d0a  se = GNU GPLv3..
-000001f0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
-00000200: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000210: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000220: 3a3a 2033 0d0a 0950 726f 6772 616d 6d69  :: 3...Programmi
-00000230: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000240: 7974 686f 6e20 3a3a 2033 2e35 0d0a 0950  ython :: 3.5...P
-00000250: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000260: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000270: 2033 2e36 0d0a 0950 726f 6772 616d 6d69   3.6...Programmi
-00000280: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000290: 7974 686f 6e20 3a3a 2033 2e37 0d0a 0950  ython :: 3.7...P
-000002a0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002b0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002c0: 2033 2e38 0d0a 0950 726f 6772 616d 6d69   3.8...Programmi
-000002d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002e0: 7974 686f 6e20 3a3a 2033 2e39 0d0a 094c  ython :: 3.9...L
-000002f0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000300: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
-00000310: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
-00000320: 656e 7365 2076 3320 6f72 206c 6174 6572  ense v3 or later
-00000330: 2028 4750 4c76 332b 290d 0a09 4f70 6572   (GPLv3+)...Oper
-00000340: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000350: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-00000360: 0d0a 5b6f 7074 696f 6e73 5d0d 0a69 6e63  ..[options]..inc
-00000370: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000380: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-00000390: 6573 203d 2066 696e 643a 0d0a 696e 7374  es = find:..inst
-000003a0: 616c 6c5f 7265 7175 6972 6573 203d 200d  all_requires = .
-000003b0: 0a09 696d 706f 7274 6c69 622d 6d65 7461  ..importlib-meta
-000003c0: 6461 7461 0d0a 7365 7475 705f 7265 7175  data..setup_requ
-000003d0: 6972 6573 203d 200d 0a09 7365 7475 7074  ires = ...setupt
-000003e0: 6f6f 6c73 5f73 636d 0d0a 7079 7468 6f6e  ools_scm..python
-000003f0: 5f72 6571 7569 7265 7320 3d20 0d0a 093e  _requires = ...>
-00000400: 3d33 2e35 0d0a 0d0a 5b65 6767 5f69 6e66  =3.5....[egg_inf
-00000410: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000420: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000430: 0d0a                                     ..
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6f63 6c6f 636b 0a61 7574 686f 7220  = oclock.author 
+00000020: 3d20 4f6c 6976 6965 7220 5669 6e63 656e  = Olivier Vincen
+00000030: 740a 6175 7468 6f72 5f65 6d61 696c 203d  t.author_email =
+00000040: 206f 7669 6e63 2e70 7940 676d 6169 6c2e   ovinc.py@gmail.
+00000050: 636f 6d0a 7572 6c20 3d20 6874 7470 733a  com.url = https:
+00000060: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7669  //github.com/ovi
+00000070: 6e63 2f6f 636c 6f63 6b0a 6465 7363 7269  nc/oclock.descri
+00000080: 7074 696f 6e20 3d20 546f 6f6c 7320 666f  ption = Tools fo
+00000090: 7220 7469 6d65 642c 206e 6f2d 6472 6966  r timed, no-drif
+000000a0: 7420 6c6f 6f70 7320 6f66 2063 6f6e 7374  t loops of const
+000000b0: 616e 7420 6475 7261 7469 6f6e 2c20 616e  ant duration, an
+000000c0: 6420 6f74 6865 7220 6d69 7363 2e20 7469  d other misc. ti
+000000d0: 6d69 6e67 2074 6f6f 6c73 2028 4755 4920  ming tools (GUI 
+000000e0: 636f 756e 7464 6f77 6e2c 2063 6f6e 7465  countdown, conte
+000000f0: 7874 206d 616e 6167 6572 7320 6574 632e  xt managers etc.
+00000100: 290a 6c6f 6e67 5f64 6573 6372 6970 7469  ).long_descripti
+00000110: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+00000120: 452e 6d64 0a6c 6f6e 675f 6465 7363 7269  E.md.long_descri
+00000130: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+00000140: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+00000150: 776e 0a6b 6579 776f 7264 7320 3d20 7469  wn.keywords = ti
+00000160: 6d69 6e67 2c20 6c6f 6f70 732c 2063 6f6e  ming, loops, con
+00000170: 7374 616e 7420 6475 7261 7469 6f6e 2c20  stant duration, 
+00000180: 6361 6e63 656c 6c61 626c 652c 206d 6f64  cancellable, mod
+00000190: 6966 6961 626c 652c 2063 6f75 6e74 646f  ifiable, countdo
+000001a0: 776e 2c20 636f 6e74 6578 7420 6d61 6e61  wn, context mana
+000001b0: 6765 722c 2067 7569 0a6c 6963 656e 7365  ger, gui.license
+000001c0: 5f66 696c 6573 203d 204c 4943 454e 5345  _files = LICENSE
+000001d0: 0a6c 6963 656e 7365 203d 2047 4e55 2047  .license = GNU G
+000001e0: 504c 7633 0a63 6c61 7373 6966 6965 7273  PLv3.classifiers
+000001f0: 203d 200a 0950 726f 6772 616d 6d69 6e67   = ..Programming
+00000200: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000210: 686f 6e20 3a3a 2033 0a09 5072 6f67 7261  hon :: 3..Progra
+00000220: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000230: 3a20 5079 7468 6f6e 203a 3a20 332e 350a  : Python :: 3.5.
+00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000260: 3a3a 2033 2e36 0a09 5072 6f67 7261 6d6d  :: 3.6..Programm
+00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000280: 5079 7468 6f6e 203a 3a20 332e 370a 0950  Python :: 3.7..P
+00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002b0: 2033 2e38 0a09 5072 6f67 7261 6d6d 696e   3.8..Programmin
+000002c0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000002d0: 7468 6f6e 203a 3a20 332e 390a 094c 6963  thon :: 3.9..Lic
+000002e0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
+000002f0: 6f76 6564 203a 3a20 474e 5520 4765 6e65  oved :: GNU Gene
+00000300: 7261 6c20 5075 626c 6963 204c 6963 656e  ral Public Licen
+00000310: 7365 2076 3320 6f72 206c 6174 6572 2028  se v3 or later (
+00000320: 4750 4c76 332b 290a 094f 7065 7261 7469  GPLv3+)..Operati
+00000330: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000340: 496e 6465 7065 6e64 656e 740a 0a5b 6f70  Independent..[op
+00000350: 7469 6f6e 735d 0a69 6e63 6c75 6465 5f70  tions].include_p
+00000360: 6163 6b61 6765 5f64 6174 6120 3d20 5472  ackage_data = Tr
+00000370: 7565 0a70 6163 6b61 6765 7320 3d20 6669  ue.packages = fi
+00000380: 6e64 3a0a 696e 7374 616c 6c5f 7265 7175  nd:.install_requ
+00000390: 6972 6573 203d 200a 0969 6d70 6f72 746c  ires = ..importl
+000003a0: 6962 2d6d 6574 6164 6174 610a 7365 7475  ib-metadata.setu
+000003b0: 705f 7265 7175 6972 6573 203d 200a 0973  p_requires = ..s
+000003c0: 6574 7570 746f 6f6c 735f 7363 6d0a 7079  etuptools_scm.py
+000003d0: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+000003e0: 0a09 3e3d 332e 350a 0a5b 6567 675f 696e  ..>=3.5..[egg_in
+000003f0: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
+00000400: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
```

### Comparing `oclock-1.3.0/tests/test_oclock.py` & `oclock-1.3.1/tests/test_oclock.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-"""Test oclock module with pytest"""
-
-import time
-import threading
-import random
-
-from oclock.performance import performance_test
-from oclock import Timer, Countdown, loop
-from oclock import parse_time, measure_time, measure_duration
-
-
-def test_timer():
-    """Test Timer() class (checkpt() and interval)"""
-    data = performance_test(dt=0.05, nloops=40, fmax=0.9, plot=False)
-    assert round(data['mean dt (s)'], 2) == 0.05
-
-
-def test_timer_precise():
-    """Test Timer() class in precise mode (precision not tested here)"""
-    data = performance_test(dt=0.05, nloops=40, fmax=0.9, plot=False, precise=True)
-    assert round(data['mean dt (s)'], 2) == 0.05
-
-
-def test_decorator():
-    """Test the @loop decorator and various Timer methods"""
-
-    timer = Timer(interval=0.1)
-    dt = 0.6  # interval between commands
-
-    def timer_control(timer):
-        """define a succession of commands to apply to the timer."""
-        methods = timer.reset, timer.pause, timer.resume, timer.stop
-        print('timer interval: {}'.format(timer.interval))
-        print('interval between commands: {}'.format(dt))
-        for method in methods:
-            time.sleep(dt)
-            print(method)
-            print('elapsed/paused before method: {:.3f}/{:.3f}'
-                  .format(timer.elapsed_time, timer.pause_time))
-            method()
-            print('elapsed/paused after method: {:.3f}/{:.3f}'
-                  .format(timer.elapsed_time, timer.pause_time))
-
-    @loop(timer)
-    def my_function():
-        time.sleep(0.05 * random.random())
-
-    threading.Thread(target=timer_control, args=(timer,)).start()
-    my_function()
-
-    assert round(timer.elapsed_time, 1) == 2 * dt
-    assert round(timer.pause_time, 1) == dt
-
-
-def test_parse():
-    """Test parsing of time strings."""
-    t1 = parse_time('::5')
-    t2 = parse_time('1::')
-    t3 = parse_time('2:30:25')
-    t4 = parse_time('::')
-
-    ts = t1, t2, t3, t4
-    ss = 5, 3600, 9025, 0
-
-    for t, s in zip(ts, ss):
-        assert t.total_seconds() == s
-
-
-def test_measure_time():
-    """Test measure_time() context manager."""
-    with measure_time() as timing:
-        time.sleep(1)
-    assert round(timing['dt (s)'], 1) == 0.5
-
-
-def test_measure_duration():
-    """Test measure_time() context manager."""
-    with measure_duration() as duration:
-        time.sleep(1)
-    assert round(duration['duration (s)'], 1) == 1
-
-
-def test_countdown():
-    """Test interactive countdown."""
-    countdown = Countdown('::5')
-    assert countdown.done
+"""Test oclock module with pytest"""
+
+import time
+import threading
+import random
+
+from oclock.performance import performance_test
+from oclock import Timer, Countdown, loop
+from oclock import parse_time, measure_time, measure_duration
+
+
+def test_timer():
+    """Test Timer() class (checkpt() and interval)"""
+    data = performance_test(dt=0.05, nloops=40, fmax=0.9, plot=False)
+    assert round(data['mean dt (s)'], 2) == 0.05
+
+
+def test_timer_precise():
+    """Test Timer() class in precise mode (precision not tested here)"""
+    data = performance_test(dt=0.05, nloops=40, fmax=0.9, plot=False, precise=True)
+    assert round(data['mean dt (s)'], 2) == 0.05
+
+
+def test_decorator():
+    """Test the @loop decorator and various Timer methods"""
+
+    timer = Timer(interval=0.1)
+    dt = 0.6  # interval between commands
+
+    def timer_control(timer):
+        """define a succession of commands to apply to the timer."""
+        methods = timer.reset, timer.pause, timer.resume, timer.stop
+        print('timer interval: {}'.format(timer.interval))
+        print('interval between commands: {}'.format(dt))
+        for method in methods:
+            time.sleep(dt)
+            print(method)
+            print('elapsed/paused before method: {:.3f}/{:.3f}'
+                  .format(timer.elapsed_time, timer.pause_time))
+            method()
+            print('elapsed/paused after method: {:.3f}/{:.3f}'
+                  .format(timer.elapsed_time, timer.pause_time))
+
+    @loop(timer)
+    def my_function():
+        time.sleep(0.05 * random.random())
+
+    threading.Thread(target=timer_control, args=(timer,)).start()
+    my_function()
+
+    assert round(timer.elapsed_time, 1) == 2 * dt
+    assert round(timer.pause_time, 1) == dt
+
+
+def test_parse():
+    """Test parsing of time strings."""
+    t1 = parse_time('::5')
+    t2 = parse_time('1::')
+    t3 = parse_time('2:30:25')
+    t4 = parse_time('::')
+
+    ts = t1, t2, t3, t4
+    ss = 5, 3600, 9025, 0
+
+    for t, s in zip(ts, ss):
+        assert t.total_seconds() == s
+
+
+def test_measure_time():
+    """Test measure_time() context manager."""
+    with measure_time() as timing:
+        time.sleep(1)
+    assert round(timing['dt (s)'], 1) == 0.5
+
+
+def test_measure_duration():
+    """Test measure_time() context manager."""
+    with measure_duration() as duration:
+        time.sleep(1)
+    assert round(duration['duration (s)'], 1) == 1
+
+
+def test_countdown():
+    """Test interactive countdown."""
+    countdown = Countdown('::5')
+    assert countdown.done
```

