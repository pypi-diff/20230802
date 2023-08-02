# Comparing `tmp/codebot-0.1.1.tar.gz` & `tmp/codebot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.1.1.tar", last modified: Wed Aug  2 08:23:46 2023, max compression
+gzip compressed data, was "codebot-0.1.2.tar", last modified: Wed Aug  2 08:39:20 2023, max compression
```

## Comparing `codebot-0.1.1.tar` & `codebot-0.1.2.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.660256 codebot-0.1.1/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.1.1/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:23:46.659853 codebot-0.1.1/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.591244 codebot-0.1.1/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2576 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      124 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 08:23:46.660432 codebot-0.1.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      591 2023-08-02 08:23:42.000000 codebot-0.1.1/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.596797 codebot-0.1.1/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.598302 codebot-0.1.1/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.1.1/src/.chainlit/.langchain.db
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.1.1/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5921 2023-08-02 08:23:31.000000 codebot-0.1.1/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.610270 codebot-0.1.1/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 07:29:57.000000 codebot-0.1.1/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.1.1/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.1.1/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.1.1/src/__pycache__/app.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.1.1/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.1.1/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.1.1/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    18128 2023-08-02 08:06:54.000000 codebot-0.1.1/src/__pycache__/app_terminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.1.1/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.1.1/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13482 2023-08-02 08:11:50.000000 codebot-0.1.1/src/app_terminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.1.1/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.613352 codebot-0.1.1/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7172 2023-08-02 07:32:10.000000 codebot-0.1.1/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1140 2023-08-02 07:45:08.000000 codebot-0.1.1/src/functions/RemoteTerminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1.1/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.619651 codebot-0.1.1/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7715 2023-08-02 07:32:13.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2756 2023-08-02 07:45:43.000000 codebot-0.1.1/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.1.1/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.1.1/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.621628 codebot-0.1.1/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.1.1/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.1.1/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.1.1/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.622607 codebot-0.1.1/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.1.1/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.623173 codebot-0.1.1/src/plugins/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.1.1/src/plugins/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.624583 codebot-0.1.1/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.627684 codebot-0.1.1/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.629403 codebot-0.1.1/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.631982 codebot-0.1.1/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.637992 codebot-0.1.1/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.1.1/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.640289 codebot-0.1.1/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.646092 codebot-0.1.1/src/plugins/terminal/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.646820 codebot-0.1.1/src/plugins/terminal/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3845 2023-08-02 07:30:01.000000 codebot-0.1.1/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.1.1/src/plugins/terminal/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2895 2023-08-02 07:27:13.000000 codebot-0.1.1/src/plugins/terminal/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.648398 codebot-0.1.1/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.658837 codebot-0.1.1/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.1.1/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.1.1/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.1.1/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.1.1/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.858218 codebot-0.1.2/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.1.2/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:39:20.857867 codebot-0.1.2/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.753034 codebot-0.1.2/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2647 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      124 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 08:39:20.000000 codebot-0.1.2/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 08:39:20.858371 codebot-0.1.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      591 2023-08-02 08:39:15.000000 codebot-0.1.2/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.757078 codebot-0.1.2/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.758509 codebot-0.1.2/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.1.2/src/.chainlit/.langchain.db
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.1.2/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6117 2023-08-02 08:37:38.000000 codebot-0.1.2/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.809172 codebot-0.1.2/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8394 2023-08-02 08:38:41.000000 codebot-0.1.2/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.1.2/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.1.2/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.1.2/src/__pycache__/app.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.1.2/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.1.2/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.1.2/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    18347 2023-08-02 08:38:52.000000 codebot-0.1.2/src/__pycache__/app_terminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    18244 2023-08-02 08:38:43.000000 codebot-0.1.2/src/__pycache__/app_terminal_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.1.2/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.1.2/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.1.2/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.1.2/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.1.2/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13495 2023-08-02 08:38:10.000000 codebot-0.1.2/src/app_terminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13482 2023-08-02 08:37:55.000000 codebot-0.1.2/src/app_terminal_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.1.2/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.813022 codebot-0.1.2/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7172 2023-08-02 07:32:10.000000 codebot-0.1.2/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1140 2023-08-02 07:45:08.000000 codebot-0.1.2/src/functions/RemoteTerminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1.2/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.822347 codebot-0.1.2/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7715 2023-08-02 07:32:13.000000 codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2756 2023-08-02 07:45:43.000000 codebot-0.1.2/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.1.2/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.1.2/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.1.2/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.1.2/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.1.2/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.825383 codebot-0.1.2/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.1.2/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.1.2/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.1.2/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.826616 codebot-0.1.2/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.1.2/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.827157 codebot-0.1.2/src/plugins/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.1.2/src/plugins/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.828762 codebot-0.1.2/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.831272 codebot-0.1.2/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.832765 codebot-0.1.2/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.835055 codebot-0.1.2/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.839963 codebot-0.1.2/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.1.2/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.841708 codebot-0.1.2/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.846865 codebot-0.1.2/src/plugins/terminal/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.848245 codebot-0.1.2/src/plugins/terminal/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3845 2023-08-02 07:30:01.000000 codebot-0.1.2/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.1.2/src/plugins/terminal/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2895 2023-08-02 07:27:13.000000 codebot-0.1.2/src/plugins/terminal/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.849610 codebot-0.1.2/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.1.2/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:39:20.856322 codebot-0.1.2/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.1.2/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.1.2/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.1.2/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.1.2/src/tmp/sin_function.png
```

### Comparing `codebot-0.1.1/codebot.egg-info/SOURCES.txt` & `codebot-0.1.2/codebot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 codebot.egg-info/entry_points.txt
 codebot.egg-info/requires.txt
 codebot.egg-info/top_level.txt
 src/__init__.py
 src/app.py
 src/app_cn.py
 src/app_terminal.py
+src/app_terminal_cn.py
 src/chainlit.md
 src/get_env.py
 src/get_text.py
 src/.chainlit/.langchain.db
 src/.chainlit/config.toml
 src/__pycache__/__init__.cpython-311.pyc
 src/__pycache__/__init__.cpython-38.pyc
 src/__pycache__/app.cpython-310.pyc
 src/__pycache__/app.cpython-311.pyc
 src/__pycache__/app.cpython-38.pyc
 src/__pycache__/app_cn.cpython-310.pyc
 src/__pycache__/app_cn.cpython-311.pyc
 src/__pycache__/app_terminal.cpython-311.pyc
+src/__pycache__/app_terminal_cn.cpython-311.pyc
 src/__pycache__/get_text.cpython-310.pyc
 src/__pycache__/get_text.cpython-311.pyc
 src/__pycache__/get_text.cpython-38.pyc
 src/functions/FunctionManager.py
 src/functions/RemoteTerminal.py
 src/functions/__init__.py
 src/functions/__pycache__/FunctionManager.cpython-310.pyc
```

### Comparing `codebot-0.1.1/setup.py` & `codebot-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="codebot",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "codebot = src:main",
             "terminalbot = src:main_terminal",  # 添加这一行
         ],
     },
```

### Comparing `codebot-0.1.1/src/.chainlit/.langchain.db` & `codebot-0.1.2/src/.chainlit/.langchain.db`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/.chainlit/config.toml` & `codebot-0.1.2/src/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__init__.py` & `codebot-0.1.2/src/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -122,14 +122,15 @@
         subprocess.run(["chainlit", "run", "app.py"])  # Run your application
         
         
 def main_terminal():
     parser = argparse.ArgumentParser()
     parser.add_argument("--config", action="store_true", help="Reset configuration")
     parser.add_argument("--port", type=int, help="Port")
+    parser.add_argument("--fix", action="store_true")
     args = parser.parse_args()
     os.chdir(os.path.dirname(os.path.abspath(__file__)))  # Change the current working directory to your application's directory
     if args.config:
         # If the --config option is given, delete the existing configuration file and create a new one
         config_path = os.path.join(os.path.expanduser('~'), '.codebot', 'config.json')
         if os.path.exists(config_path):
             os.remove(config_path)
@@ -137,13 +138,16 @@
     else:
         print("Checking configuration...")
         check_config()  # Check and create the configuration file if not exists
     
    
             
     port = args.port if args.port else 10086
-    subprocess.run(["chainlit", "run", "app_terminal.py", "--port", str(port)])  # Run your application
+    if args.fix:
+        subprocess.run(["chainlit", "run", "app_terminal_cn.py", "--port", str(port)])  # Run your application
+    else:
+        subprocess.run(["chainlit", "run", "app_terminal.py", "--port", str(port)])  # Run your application
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `codebot-0.1.1/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.1.2/src/__pycache__/__init__.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc3fdc964 (Wed Aug  2 06:54:59 2023 UTC)
-files sz: 5836
+moddate:  0xd215ca64 (Wed Aug  2 08:37:38 2023 UTC)
+files sz: 6117
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -54,28 +54,28 @@
                 64 MAKE_FUNCTION            0
                 66 STORE_NAME               8 (main)
    
    125          68 LOAD_CONST               7 (<code object main_terminal, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 125>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME               9 (main_terminal)
    
-   147          74 LOAD_NAME               10 (__name__)
+   152          74 LOAD_NAME               10 (__name__)
                 76 LOAD_CONST               8 ('__main__')
                 78 COMPARE_OP               2 (==)
                 84 POP_JUMP_FORWARD_IF_FALSE    12 (to 110)
    
-   148          86 PUSH_NULL
+   153          86 PUSH_NULL
                 88 LOAD_NAME                8 (main)
                 90 PRECALL                  0
                 94 CALL                     0
                104 POP_TOP
                106 LOAD_CONST               1 (None)
                108 RETURN_VALUE
    
-   147     >>  110 LOAD_CONST               1 (None)
+   152     >>  110 LOAD_CONST               1 (None)
                112 RETURN_VALUE
    consts
       0
       None
       ('ngrok',)
       False
       code
@@ -969,41 +969,50 @@
          name       'main'
          firstlineno 89
          lnotab
             0x020126012e013a0130012802a6020e027c013e01280122021e011c020e
             0102012602320228013201120136ff08030e013002
       code
          argcount  : 0
-         nlocals   : 3
-         stacksize : 7
+         nlocals   : 4
+         stacksize : 9
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d007c00a002000000000000000000000000000000
             0000000000640164026403ac04a6030000ab03000000000000000001007c
-            00a0030000000000000000000000000000000000000000a6000000ab0000
-            000000000000007d017409000000000000000000006a0500000000000000
-            007408000000000000000000006a060000000000000000a0070000000000
-            0000000000000000000000000000007408000000000000000000006a0600
+            00a002000000000000000000000000000000000000000064057406000000
+            000000000000006406ac07a6030000ab03000000000000000001007c00a0
+            02000000000000000000000000000000000000000064086402ac09a60200
+            00ab02000000000000000001007c00a00400000000000000000000000000
+            00000000000000a6000000ab0000000000000000007d01740b0000000000
+            00000000006a060000000000000000740a000000000000000000006a0700
             00000000000000a008000000000000000000000000000000000000000074
-            1200000000000000000000a6010000ab010000000000000000a6010000ab
-            010000000000000000a6010000ab01000000000000000001007c016a0a00
-            0000000000000072827408000000000000000000006a0600000000000000
-            00a00b000000000000000000000000000000000000000074080000000000
-            00000000006a060000000000000000a00c00000000000000000000000000
-            000000000000006405a6010000ab01000000000000000064066407a60300
-            00ab0300000000000000007d027408000000000000000000006a06000000
-            0000000000a00d00000000000000000000000000000000000000007c02a6
-            010000ab01000000000000000072147409000000000000000000006a0e00
-            000000000000007c02a6010000ab0100000000000000000100741f000000
-            000000000000006408ac09a6010000ab01000000000000000001006e1d74
-            2100000000000000000000640aa6010000ab010000000000000000010074
-            1f00000000000000000000a6000000ab0000000000000000000100742300
-            0000000000000000006a1200000000000000006700640ba201a6010000ab
-            010000000000000000010064005300
+            0a000000000000000000006a070000000000000000a00900000000000000
+            00000000000000000000000000741400000000000000000000a6010000ab
+            010000000000000000a6010000ab010000000000000000a6010000ab0100
+            0000000000000001007c016a0b00000000000000007282740a0000000000
+            00000000006a070000000000000000a00c00000000000000000000000000
+            00000000000000740a000000000000000000006a070000000000000000a0
+            0d0000000000000000000000000000000000000000640aa6010000ab0100
+            00000000000000640b640ca6030000ab0300000000000000007d02740a00
+            0000000000000000006a070000000000000000a00e000000000000000000
+            00000000000000000000007c02a6010000ab010000000000000000721474
+            0b000000000000000000006a0f00000000000000007c02a6010000ab0100
+            000000000000000100742100000000000000000000640dac0ea6010000ab
+            01000000000000000001006e1d742300000000000000000000640fa60100
+            00ab0100000000000000000100742100000000000000000000a6000000ab
+            00000000000000000001007c016a12000000000000000072077c016a1200
+            000000000000006e0164107d037c016a1300000000000000007228742900
+            0000000000000000006a1500000000000000006411641264136405742d00
+            0000000000000000007c03a6010000ab0100000000000000006705a60100
+            00ab0100000000000000000100640053007429000000000000000000006a
+            1500000000000000006411641264146405742d000000000000000000007c
+            03a6010000ab0100000000000000006705a6010000ab0100000000000000
+            00010064005300
          125           0 RESUME                   0
          
          126           2 LOAD_GLOBAL              1 (NULL + argparse)
                       14 LOAD_ATTR                1 (ArgumentParser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (parser)
@@ -1015,123 +1024,189 @@
                       68 LOAD_CONST               3 ('Reset configuration')
                       70 KW_NAMES                 4
                       72 PRECALL                  3
                       76 CALL                     3
                       86 POP_TOP
          
          128          88 LOAD_FAST                0 (parser)
-                      90 LOAD_METHOD              3 (parse_args)
-                     112 PRECALL                  0
-                     116 CALL                     0
-                     126 STORE_FAST               1 (args)
-         
-         129         128 LOAD_GLOBAL              9 (NULL + os)
-                     140 LOAD_ATTR                5 (chdir)
-                     150 LOAD_GLOBAL              8 (os)
-                     162 LOAD_ATTR                6 (path)
-                     172 LOAD_METHOD              7 (dirname)
-                     194 LOAD_GLOBAL              8 (os)
-                     206 LOAD_ATTR                6 (path)
-                     216 LOAD_METHOD              8 (abspath)
-                     238 LOAD_GLOBAL             18 (__file__)
-                     250 PRECALL                  1
-                     254 CALL                     1
-                     264 PRECALL                  1
-                     268 CALL                     1
-                     278 PRECALL                  1
-                     282 CALL                     1
-                     292 POP_TOP
+                      90 LOAD_METHOD              2 (add_argument)
+                     112 LOAD_CONST               5 ('--port')
+                     114 LOAD_GLOBAL              6 (int)
+                     126 LOAD_CONST               6 ('Port')
+                     128 KW_NAMES                 7
+                     130 PRECALL                  3
+                     134 CALL                     3
+                     144 POP_TOP
+         
+         129         146 LOAD_FAST                0 (parser)
+                     148 LOAD_METHOD              2 (add_argument)
+                     170 LOAD_CONST               8 ('--fix')
+                     172 LOAD_CONST               2 ('store_true')
+                     174 KW_NAMES                 9
+                     176 PRECALL                  2
+                     180 CALL                     2
+                     190 POP_TOP
          
-         130         294 LOAD_FAST                1 (args)
-                     296 LOAD_ATTR               10 (config)
-                     306 POP_JUMP_FORWARD_IF_FALSE   130 (to 568)
-         
-         132         308 LOAD_GLOBAL              8 (os)
-                     320 LOAD_ATTR                6 (path)
-                     330 LOAD_METHOD             11 (join)
-                     352 LOAD_GLOBAL              8 (os)
-                     364 LOAD_ATTR                6 (path)
-                     374 LOAD_METHOD             12 (expanduser)
-                     396 LOAD_CONST               5 ('~')
-                     398 PRECALL                  1
-                     402 CALL                     1
-                     412 LOAD_CONST               6 ('.codebot')
-                     414 LOAD_CONST               7 ('config.json')
-                     416 PRECALL                  3
-                     420 CALL                     3
-                     430 STORE_FAST               2 (config_path)
-         
-         133         432 LOAD_GLOBAL              8 (os)
-                     444 LOAD_ATTR                6 (path)
-                     454 LOAD_METHOD             13 (exists)
-                     476 LOAD_FAST                2 (config_path)
-                     478 PRECALL                  1
-                     482 CALL                     1
-                     492 POP_JUMP_FORWARD_IF_FALSE    20 (to 534)
-         
-         134         494 LOAD_GLOBAL              9 (NULL + os)
-                     506 LOAD_ATTR               14 (remove)
-                     516 LOAD_FAST                2 (config_path)
-                     518 PRECALL                  1
-                     522 CALL                     1
-                     532 POP_TOP
-         
-         135     >>  534 LOAD_GLOBAL             31 (NULL + check_config_terminal)
-                     546 LOAD_CONST               8 (True)
-                     548 KW_NAMES                 9
-                     550 PRECALL                  1
-                     554 CALL                     1
-                     564 POP_TOP
-                     566 JUMP_FORWARD            29 (to 626)
+         130         192 LOAD_FAST                0 (parser)
+                     194 LOAD_METHOD              4 (parse_args)
+                     216 PRECALL                  0
+                     220 CALL                     0
+                     230 STORE_FAST               1 (args)
          
-         137     >>  568 LOAD_GLOBAL             33 (NULL + print)
-                     580 LOAD_CONST              10 ('Checking configuration...')
+         131         232 LOAD_GLOBAL             11 (NULL + os)
+                     244 LOAD_ATTR                6 (chdir)
+                     254 LOAD_GLOBAL             10 (os)
+                     266 LOAD_ATTR                7 (path)
+                     276 LOAD_METHOD              8 (dirname)
+                     298 LOAD_GLOBAL             10 (os)
+                     310 LOAD_ATTR                7 (path)
+                     320 LOAD_METHOD              9 (abspath)
+                     342 LOAD_GLOBAL             20 (__file__)
+                     354 PRECALL                  1
+                     358 CALL                     1
+                     368 PRECALL                  1
+                     372 CALL                     1
+                     382 PRECALL                  1
+                     386 CALL                     1
+                     396 POP_TOP
+         
+         132         398 LOAD_FAST                1 (args)
+                     400 LOAD_ATTR               11 (config)
+                     410 POP_JUMP_FORWARD_IF_FALSE   130 (to 672)
+         
+         134         412 LOAD_GLOBAL             10 (os)
+                     424 LOAD_ATTR                7 (path)
+                     434 LOAD_METHOD             12 (join)
+                     456 LOAD_GLOBAL             10 (os)
+                     468 LOAD_ATTR                7 (path)
+                     478 LOAD_METHOD             13 (expanduser)
+                     500 LOAD_CONST              10 ('~')
+                     502 PRECALL                  1
+                     506 CALL                     1
+                     516 LOAD_CONST              11 ('.codebot')
+                     518 LOAD_CONST              12 ('config.json')
+                     520 PRECALL                  3
+                     524 CALL                     3
+                     534 STORE_FAST               2 (config_path)
+         
+         135         536 LOAD_GLOBAL             10 (os)
+                     548 LOAD_ATTR                7 (path)
+                     558 LOAD_METHOD             14 (exists)
+                     580 LOAD_FAST                2 (config_path)
                      582 PRECALL                  1
                      586 CALL                     1
-                     596 POP_TOP
+                     596 POP_JUMP_FORWARD_IF_FALSE    20 (to 638)
+         
+         136         598 LOAD_GLOBAL             11 (NULL + os)
+                     610 LOAD_ATTR               15 (remove)
+                     620 LOAD_FAST                2 (config_path)
+                     622 PRECALL                  1
+                     626 CALL                     1
+                     636 POP_TOP
          
-         138         598 LOAD_GLOBAL             31 (NULL + check_config_terminal)
-                     610 PRECALL                  0
-                     614 CALL                     0
-                     624 POP_TOP
-         
-         143     >>  626 LOAD_GLOBAL             35 (NULL + subprocess)
-                     638 LOAD_ATTR               18 (run)
-                     648 BUILD_LIST               0
-                     650 LOAD_CONST              11 (('chainlit', 'run', 'app_terminal.py', '--port', '10086'))
-                     652 LIST_EXTEND              1
+         137     >>  638 LOAD_GLOBAL             33 (NULL + check_config)
+                     650 LOAD_CONST              13 (True)
+                     652 KW_NAMES                14
                      654 PRECALL                  1
                      658 CALL                     1
                      668 POP_TOP
-                     670 LOAD_CONST               0 (None)
-                     672 RETURN_VALUE
+                     670 JUMP_FORWARD            29 (to 730)
+         
+         139     >>  672 LOAD_GLOBAL             35 (NULL + print)
+                     684 LOAD_CONST              15 ('Checking configuration...')
+                     686 PRECALL                  1
+                     690 CALL                     1
+                     700 POP_TOP
+         
+         140         702 LOAD_GLOBAL             33 (NULL + check_config)
+                     714 PRECALL                  0
+                     718 CALL                     0
+                     728 POP_TOP
+         
+         144     >>  730 LOAD_FAST                1 (args)
+                     732 LOAD_ATTR               18 (port)
+                     742 POP_JUMP_FORWARD_IF_FALSE     7 (to 758)
+                     744 LOAD_FAST                1 (args)
+                     746 LOAD_ATTR               18 (port)
+                     756 JUMP_FORWARD             1 (to 760)
+                 >>  758 LOAD_CONST              16 (10086)
+                 >>  760 STORE_FAST               3 (port)
+         
+         145         762 LOAD_FAST                1 (args)
+                     764 LOAD_ATTR               19 (fix)
+                     774 POP_JUMP_FORWARD_IF_FALSE    40 (to 856)
+         
+         146         776 LOAD_GLOBAL             41 (NULL + subprocess)
+                     788 LOAD_ATTR               21 (run)
+                     798 LOAD_CONST              17 ('chainlit')
+                     800 LOAD_CONST              18 ('run')
+                     802 LOAD_CONST              19 ('app_terminal_cn.py')
+                     804 LOAD_CONST               5 ('--port')
+                     806 LOAD_GLOBAL             45 (NULL + str)
+                     818 LOAD_FAST                3 (port)
+                     820 PRECALL                  1
+                     824 CALL                     1
+                     834 BUILD_LIST               5
+                     836 PRECALL                  1
+                     840 CALL                     1
+                     850 POP_TOP
+                     852 LOAD_CONST               0 (None)
+                     854 RETURN_VALUE
+         
+         148     >>  856 LOAD_GLOBAL             41 (NULL + subprocess)
+                     868 LOAD_ATTR               21 (run)
+                     878 LOAD_CONST              17 ('chainlit')
+                     880 LOAD_CONST              18 ('run')
+                     882 LOAD_CONST              20 ('app_terminal.py')
+                     884 LOAD_CONST               5 ('--port')
+                     886 LOAD_GLOBAL             45 (NULL + str)
+                     898 LOAD_FAST                3 (port)
+                     900 PRECALL                  1
+                     904 CALL                     1
+                     914 BUILD_LIST               5
+                     916 PRECALL                  1
+                     920 CALL                     1
+                     930 POP_TOP
+                     932 LOAD_CONST               0 (None)
+                     934 RETURN_VALUE
          consts
             None
             '--config'
             'store_true'
             'Reset configuration'
             ('action', 'help')
+            '--port'
+            'Port'
+            ('type', 'help')
+            '--fix'
+            ('action',)
             '~'
             '.codebot'
             'config.json'
             True
             ('force_config',)
             'Checking configuration...'
-            ('chainlit', 'run', 'app_terminal.py', '--port', '10086')
-         names      ('argparse', 'ArgumentParser', 'add_argument', 'parse_args', 'os', 'chdir', 'path', 'dirname', 'abspath', '__file__', 'config', 'join', 'expanduser', 'exists', 'remove', 'check_config_terminal', 'print', 'subprocess', 'run')
-         varnames   ('parser', 'args', 'config_path')
+            10086
+            'chainlit'
+            'run'
+            'app_terminal_cn.py'
+            'app_terminal.py'
+         names      ('argparse', 'ArgumentParser', 'add_argument', 'int', 'parse_args', 'os', 'chdir', 'path', 'dirname', 'abspath', '__file__', 'config', 'join', 'expanduser', 'exists', 'remove', 'check_config', 'print', 'port', 'fix', 'subprocess', 'run', 'str')
+         varnames   ('parser', 'args', 'config_path', 'port')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
          name       'main_terminal'
          firstlineno 125
-         lnotab 0x0201260130012801a6010e027c013e01280122021e011c05
+         lnotab
+            0x0201260130013a012e012801a6010e027c013e01280122021e011c0420
+            010e015002
       '__main__'
       (False,)
    names      ('os', 'subprocess', 'json', 'argparse', 'pyngrok', 'ngrok', 'check_config', 'check_config_terminal', 'main', 'main_terminal', '__name__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010801080108010c020827082b062406160c0118ff
+   lnotab 0x00ff020108010801080108010c020827082b0624061b0c0118ff
```

### Comparing `codebot-0.1.1/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.1.2/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app.cpython-310.pyc` & `codebot-0.1.2/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app.cpython-311.pyc` & `codebot-0.1.2/src/__pycache__/app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app.cpython-38.pyc` & `codebot-0.1.2/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.1.2/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.1.2/src/__pycache__/app_cn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/app_terminal.cpython-311.pyc` & `codebot-0.1.2/src/__pycache__/app_terminal_cn.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x990eca64 (Wed Aug  2 08:06:49 2023 UTC)
-files sz: 13369
+moddate:  0xe315ca64 (Wed Aug  2 08:37:55 2023 UTC)
+files sz: 13482
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -204,15 +204,15 @@
                510 LOAD_METHOD             16 (join)
                532 LOAD_NAME               28 (current_dir)
                534 LOAD_CONST              11 ('plugins')
                536 PRECALL                  2
                540 CALL                     2
                550 STORE_NAME              29 (plugins_dir)
    
-    29         552 LOAD_CONST              12 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 29>)
+    29         552 LOAD_CONST              12 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 29>)
                554 MAKE_FUNCTION            0
    
     30         556 PUSH_NULL
                558 LOAD_NAME                4 (os)
                560 LOAD_ATTR               30 (listdir)
                570 LOAD_NAME               29 (plugins_dir)
                572 PRECALL                  1
@@ -313,15 +313,15 @@
                830 BUILD_STRING             3
                832 PRECALL                  1
                836 CALL                     1
                846 STORE_NAME              40 (module)
    
     47         848 LOAD_NAME               32 (functions)
                850 LOAD_METHOD             41 (extend)
-               872 LOAD_CONST              19 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 47>)
+               872 LOAD_CONST              19 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 47>)
                874 MAKE_FUNCTION            0
    
     48         876 PUSH_NULL
                878 LOAD_NAME                9 (inspect)
                880 LOAD_ATTR               42 (getmembers)
                890 LOAD_NAME               40 (module)
                892 PRECALL                  1
@@ -374,71 +374,71 @@
    
     57     >> 1080 LOAD_CONST              23 (5000)
               1082 STORE_NAME              48 (max_tokens)
    
     58     >> 1084 LOAD_CONST              24 (False)
               1086 STORE_GLOBAL            49 (is_stop)
    
-    61        1088 LOAD_CONST              25 (<code object __truncate_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 61>)
+    61        1088 LOAD_CONST              25 (<code object __truncate_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 61>)
               1090 MAKE_FUNCTION            0
               1092 STORE_NAME              50 (__truncate_conversation)
    
-    73        1094 LOAD_CONST              26 (<code object get_token_count, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 73>)
+    73        1094 LOAD_CONST              26 (<code object get_token_count, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 73>)
               1096 MAKE_FUNCTION            0
               1098 STORE_NAME              51 (get_token_count)
    
     87        1100 LOAD_CONST              27 (100)
               1102 STORE_NAME              52 (MAX_ITER)
    
     90        1104 LOAD_CONST              28 ('user_message')
               1106 LOAD_NAME               53 (object)
               1108 BUILD_TUPLE              2
-              1110 LOAD_CONST              29 (<code object on_message, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 90>)
+              1110 LOAD_CONST              29 (<code object on_message, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 90>)
               1112 MAKE_FUNCTION            4 (annotations)
               1114 STORE_NAME              54 (on_message)
    
-   235        1116 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 235>)
+   235        1116 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 235>)
               1118 MAKE_FUNCTION            0
               1120 STORE_NAME              55 (process_new_delta)
    
    270        1122 LOAD_NAME                6 (cl)
               1124 LOAD_ATTR               56 (on_chat_start)
    
-   271        1134 LOAD_CONST              31 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 270>)
+   271        1134 LOAD_CONST              31 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 270>)
               1136 MAKE_FUNCTION            0
    
    270        1138 PRECALL                  0
               1142 CALL                     0
    
    271        1152 STORE_NAME              57 (start_chat)
    
-   324        1154 LOAD_NAME                6 (cl)
+   326        1154 LOAD_NAME                6 (cl)
               1156 LOAD_ATTR               54 (on_message)
    
-   325        1166 LOAD_CONST              28 ('user_message')
+   327        1166 LOAD_CONST              28 ('user_message')
               1168 LOAD_NAME               53 (object)
               1170 BUILD_TUPLE              2
-              1172 LOAD_CONST              32 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 324>)
+              1172 LOAD_CONST              32 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 326>)
               1174 MAKE_FUNCTION            4 (annotations)
    
-   324        1176 PRECALL                  0
+   326        1176 PRECALL                  0
               1180 CALL                     0
    
-   325        1190 STORE_NAME              58 (run_conversation)
+   327        1190 STORE_NAME              58 (run_conversation)
    
-   363        1192 LOAD_NAME                6 (cl)
+   365        1192 LOAD_NAME                6 (cl)
               1194 LOAD_ATTR               59 (on_stop)
    
-   364        1204 LOAD_CONST              33 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 363>)
+   366        1204 LOAD_CONST              33 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py", line 365>)
               1206 MAKE_FUNCTION            0
    
-   363        1208 PRECALL                  0
+   365        1208 PRECALL                  0
               1212 CALL                     0
    
-   364        1222 STORE_NAME              60 (stop_chat)
+   366        1222 STORE_NAME              60 (stop_chat)
               1224 LOAD_CONST               1 (None)
               1226 RETURN_VALUE
    ExceptionTable:
      242 to 274 -> 300 [1] lasti
      300 to 306 -> 308 [3] lasti
      314 to 314 -> 308 [3] lasti
      618 to 648 -> 776 [1]
@@ -509,15 +509,15 @@
                  >>  160 RETURN_VALUE
          consts
             '__pycache__'
          names      ('os', 'path', 'isdir', 'join', 'plugins_dir')
          varnames   ('.0', 'd')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       '<listcomp>'
          firstlineno 29
          lnotab 0x0801020182fe02020cff0201
       'plugins/'
       '/config.json'
       'enabled'
       True
@@ -554,15 +554,15 @@
                       60 JUMP_BACKWARD           28 (to 6)
                  >>   62 RETURN_VALUE
          consts
          names      ('inspect', 'isfunction')
          varnames   ('.0', 'name', 'obj')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       '<listcomp>'
          firstlineno 47
          lnotab 0x08012eff020102ff
       ('functions',)
       'functions:'
       'max_tokens'
       5000
@@ -638,15 +638,15 @@
             None
             0
             1
          names      ('get_token_count', 'max_tokens', 'len', 'pop', 'insert')
          varnames   ('conversation', 'system_con')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       '__truncate_conversation'
          firstlineno 61
          lnotab 0x020110011401020156012c0202fc02052c01
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 10
@@ -742,15 +742,15 @@
             'name'
             -1
             2
          names      ('tiktoken', 'encoding_for_model', 'config_env', 'items', 'len', 'encode', 'str')
          varnames   ('conversation', 'encoding', 'num_tokens', 'message', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'get_token_count'
          firstlineno 73
          lnotab 0x02014a02040108010a01320164010c010cfd02040a01
       100
       'user_message'
       code
          argcount  : 1
@@ -1742,15 +1742,15 @@
             'output'
             'markdown'
             ('author', 'content', 'language', 'indent')
          names      ('is_stop', 'print', 'str', 'cl', 'user_session', 'get', 'append', 'MAX_ITER', 'Message', '__truncate_conversation', 'function_manager', 'generate_functions_array', 'openai', 'ChatCompletion', 'create', 'config_env', 'choices', 'process_new_delta', 'Exception', 'asyncio', 'sleep', 'send', 'ValueError', 'json', 'loads', 'ast', 'literal_eval', 'dumps', 'call_function', 'type', 'isinstance', 'startswith', 'dict')
          varnames   ('user_message', 'message_history', 'cur_iter', 'openai_message', 'function_ui_message', 'content_ui_message', 'stream_resp', 'send_message', 'functions', 'user_plugin_api_info', 'item', 'i', 'new_delta', 'e', 'function_name', 'function_response', 'arguments', 'description', 'language', 'final_response', 'content')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'on_message'
          firstlineno 90
          lnotab
             0x060204011e011e011e011e013e013001040128020a0104012a0104011e
             01020132013e010401080114012cff020220012c01240102010201020102
             0102fa160726010e0104010e0104010c0108ff2a0212011e010a01340114
             fc0806040134010402040134022e0104012e014002500144010401020116
@@ -1997,15 +1997,15 @@
             'json'
             ('author', 'content', 'indent', 'language')
             'arguments'
          names      ('get', 'stream_token', 'send', 'cl', 'Message')
          varnames   ('new_delta', 'openai_message', 'content_ui_message', 'function_ui_message', 'new_content', 'function_name')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'process_new_delta'
          firstlineno 235
          lnotab
             0x06020801160108012e0120013601080114011c010c01040204ff0a0334
             01160102010201020102fc12053602140114011601200102ff0a0102ff16
             0218011aff1c02
       code
@@ -2210,86 +2210,86 @@
          
          292     >>  902 LOAD_GLOBAL             19 (NULL + platform)
                      914 LOAD_ATTR               10 (system)
                      924 PRECALL                  0
                      928 CALL                     0
                      938 STORE_FAST               5 (platform_name)
          
-         293         940 LOAD_CONST               9 ('You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n')
+         293         940 LOAD_CONST               9 ('You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n```\nif terminal function return a long string, No need to return completely, just summarize the general content.\n')
          
-         312         942 LOAD_METHOD             11 (format)
+         314         942 LOAD_METHOD             11 (format)
                      964 LOAD_FAST                5 (platform_name)
                      966 LOAD_FAST                2 (password)
                      968 KW_NAMES                10
                      970 PRECALL                  2
                      974 CALL                     2
          
          293         984 STORE_FAST               6 (content)
          
-         313         986 LOAD_GLOBAL             24 (config_env)
+         315         986 LOAD_GLOBAL             24 (config_env)
                      998 LOAD_CONST              11 ('openai')
                     1000 BINARY_SUBSCR
                     1010 LOAD_CONST              12 ('language')
                     1012 BINARY_SUBSCR
                     1022 STORE_FAST               7 (language)
          
-         314        1024 LOAD_GLOBAL              0 (cl)
+         316        1024 LOAD_GLOBAL              0 (cl)
                     1036 LOAD_ATTR                1 (user_session)
                     1046 LOAD_METHOD              6 (set)
          
-         315        1068 LOAD_CONST              13 ('message_history')
+         317        1068 LOAD_CONST              13 ('message_history')
          
-         318        1070 LOAD_CONST              14 ('system')
+         320        1070 LOAD_CONST              14 ('system')
          
-         319        1072 LOAD_FAST                6 (content)
+         321        1072 LOAD_FAST                6 (content)
                     1074 LOAD_CONST              15 ('\n\n')
                     1076 BINARY_OP                0 (+)
                     1080 LOAD_CONST              16 ('Please answer me in ')
                     1082 BINARY_OP                0 (+)
                     1086 LOAD_FAST                7 (language)
                     1088 BINARY_OP                0 (+)
          
-         316        1092 LOAD_CONST              17 (('role', 'content'))
+         318        1092 LOAD_CONST              17 (('role', 'content'))
                     1094 BUILD_CONST_KEY_MAP      2
                     1096 BUILD_LIST               1
          
-         314        1098 PRECALL                  2
+         316        1098 PRECALL                  2
                     1102 CALL                     2
                     1112 POP_TOP
                     1114 LOAD_CONST               0 (None)
                     1116 RETURN_VALUE
          consts
             None
             'user_id'
             'username'
             'password'
             'hostname'
             '请输入需要连接的终端的IP地址'
             'content'
             '请输入需要连接的终端的用户名'
             '输入需要连接的终端的密码'
-            'You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n'
+            'You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n```\nif terminal function return a long string, No need to return completely, just summarize the general content.\n'
             ('platform_name', 'password')
             'openai'
             'language'
             'message_history'
             'system'
             '\n\n'
             'Please answer me in '
             ('role', 'content')
          names      ('cl', 'user_session', 'get', 'str', 'uuid', 'uuid4', 'set', 'AskUserMessage', 'send', 'platform', 'system', 'format', 'config_env')
          varnames   ('user_id', 'username', 'password', 'hostname', 'res', 'platform_name', 'content', 'language')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'start_chat'
          firstlineno 270
          lnotab
             0x06033e010401400140013e013e013e0104015801100140010401580110
-            0140010401580110014001260102132aed021426012c010203020114fd06
+            0140010401580110014001260102152aeb021626012c010203020114fd06
             fe
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 7
          flags     : 131
          code
@@ -2315,112 +2315,112 @@
             0000000000000000006411190000000000000000007d08740b0000000000
             00000000006a10000000000000000064127423000000000000000000007c
             086413a6020000ab0200000000000000009b0064147c039b009d03ac15a6
             020000ab020000000000000000a007000000000000000000000000000000
             0000000000a6000000ab000000000000000000830064007b035600970386
             040100640053007425000000000000000000007c00a6010000ab01000000
             0000000000830064007b03560097038604010064005300
-         324           0 RETURN_GENERATOR
+         326           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         326           6 LOAD_CONST               1 ('/upload')
+         328           6 LOAD_CONST               1 ('/upload')
                        8 LOAD_GLOBAL              1 (NULL + str)
                       20 LOAD_FAST                0 (user_message)
                       22 PRECALL                  1
                       26 CALL                     1
                       36 COMPARE_OP               2 (==)
                       42 EXTENDED_ARG             1
                       44 POP_JUMP_FORWARD_IF_FALSE   340 (to 726)
          
-         327          46 LOAD_GLOBAL              2 (os)
+         329          46 LOAD_GLOBAL              2 (os)
                       58 LOAD_ATTR                2 (path)
                       68 LOAD_METHOD              3 (exists)
                       90 LOAD_CONST               2 ('./tmp')
                       92 PRECALL                  1
                       96 CALL                     1
                      106 POP_JUMP_FORWARD_IF_TRUE    20 (to 148)
          
-         328         108 LOAD_GLOBAL              3 (NULL + os)
+         330         108 LOAD_GLOBAL              3 (NULL + os)
                      120 LOAD_ATTR                4 (mkdir)
                      130 LOAD_CONST               2 ('./tmp')
                      132 PRECALL                  1
                      136 CALL                     1
                      146 POP_TOP
          
-         329     >>  148 LOAD_GLOBAL             11 (NULL + cl)
+         331     >>  148 LOAD_GLOBAL             11 (NULL + cl)
                      160 LOAD_ATTR                6 (AskFileMessage)
          
-         330         170 LOAD_CONST               3 ('Please upload a file.')
+         332         170 LOAD_CONST               3 ('Please upload a file.')
          
-         331         172 LOAD_CONST               4 (10)
+         333         172 LOAD_CONST               4 (10)
          
-         333         174 LOAD_CONST               5 ('*')
+         335         174 LOAD_CONST               5 ('*')
          
-         332         176 BUILD_LIST               1
+         334         176 BUILD_LIST               1
          
-         329         178 KW_NAMES                 6
+         331         178 KW_NAMES                 6
                      180 PRECALL                  3
                      184 CALL                     3
          
-         334         194 LOAD_METHOD              7 (send)
+         336         194 LOAD_METHOD              7 (send)
                      216 PRECALL                  0
                      220 CALL                     0
          
-         329         230 GET_AWAITABLE            0
+         331         230 GET_AWAITABLE            0
                      232 LOAD_CONST               0 (None)
                  >>  234 SEND                     3 (to 242)
                      236 YIELD_VALUE
                      238 RESUME                   3
                      240 JUMP_BACKWARD_NO_INTERRUPT     4 (to 234)
                  >>  242 STORE_FAST               1 (files)
          
-         335         244 LOAD_FAST                1 (files)
+         337         244 LOAD_FAST                1 (files)
                      246 LOAD_CONST               7 (0)
                      248 BINARY_SUBSCR
                      258 STORE_FAST               2 (file)
          
-         336         260 LOAD_CONST               8 ('')
+         338         260 LOAD_CONST               8 ('')
                      262 STORE_FAST               3 (save_path)
          
-         339         264 LOAD_FAST                3 (save_path)
+         341         264 LOAD_FAST                3 (save_path)
                      266 LOAD_CONST               8 ('')
                      268 COMPARE_OP               2 (==)
                      274 POP_JUMP_FORWARD_IF_FALSE     7 (to 290)
          
-         340         276 LOAD_FAST                2 (file)
+         342         276 LOAD_FAST                2 (file)
                      278 LOAD_ATTR                8 (name)
                      288 STORE_FAST               3 (save_path)
          
-         341     >>  290 LOAD_CONST               9 ('./tmp/')
+         343     >>  290 LOAD_CONST               9 ('./tmp/')
                      292 LOAD_FAST                3 (save_path)
                      294 FORMAT_VALUE             0
                      296 BUILD_STRING             2
                      298 STORE_FAST               4 (file_path)
          
-         343         300 LOAD_FAST                2 (file)
+         345         300 LOAD_FAST                2 (file)
                      302 LOAD_ATTR                9 (content)
                      312 STORE_FAST               5 (content)
          
-         346         314 LOAD_GLOBAL             21 (NULL + open)
+         348         314 LOAD_GLOBAL             21 (NULL + open)
                      326 LOAD_FAST                4 (file_path)
                      328 LOAD_CONST              10 ('wb')
                      330 PRECALL                  2
                      334 CALL                     2
                      344 BEFORE_WITH
                      346 STORE_FAST               6 (f)
          
-         347         348 LOAD_FAST                6 (f)
+         349         348 LOAD_FAST                6 (f)
                      350 LOAD_METHOD             11 (write)
                      372 LOAD_FAST                5 (content)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 POP_TOP
          
-         346         390 LOAD_CONST               0 (None)
+         348         390 LOAD_CONST               0 (None)
                      392 LOAD_CONST               0 (None)
                      394 LOAD_CONST               0 (None)
                      396 PRECALL                  2
                      400 CALL                     2
                      410 POP_TOP
                      412 JUMP_FORWARD            11 (to 436)
                  >>  414 PUSH_EXC_INFO
@@ -2431,82 +2431,82 @@
                      424 POP_EXCEPT
                      426 RERAISE                  1
                  >>  428 POP_TOP
                      430 POP_EXCEPT
                      432 POP_TOP
                      434 POP_TOP
          
-         348     >>  436 LOAD_GLOBAL             10 (cl)
+         350     >>  436 LOAD_GLOBAL             10 (cl)
                      448 LOAD_ATTR               12 (user_session)
                      458 LOAD_METHOD             13 (get)
                      480 LOAD_CONST              11 ('message_history')
                      482 PRECALL                  1
                      486 CALL                     1
                      496 STORE_FAST               7 (message_history)
          
-         349         498 LOAD_FAST                7 (message_history)
+         351         498 LOAD_FAST                7 (message_history)
                      500 LOAD_METHOD             14 (append)
          
-         350         522 LOAD_CONST              12 ('assistant')
+         352         522 LOAD_CONST              12 ('assistant')
          
-         351         524 LOAD_CONST              13 ('upload file ./tmp/')
+         353         524 LOAD_CONST              13 ('upload file ./tmp/')
                      526 LOAD_FAST                3 (save_path)
                      528 FORMAT_VALUE             0
                      530 LOAD_CONST              14 (' success')
                      532 BUILD_STRING             3
          
-         349         534 LOAD_CONST              15 (('role', 'content'))
+         351         534 LOAD_CONST              15 (('role', 'content'))
                      536 BUILD_CONST_KEY_MAP      2
                      538 PRECALL                  1
                      542 CALL                     1
                      552 POP_TOP
          
-         353         554 LOAD_GLOBAL             30 (config_env)
+         355         554 LOAD_GLOBAL             30 (config_env)
                      566 LOAD_CONST              16 ('openai')
                      568 BINARY_SUBSCR
                      578 LOAD_CONST              17 ('language')
                      580 BINARY_SUBSCR
                      590 STORE_FAST               8 (language)
          
-         354         592 LOAD_GLOBAL             11 (NULL + cl)
+         356         592 LOAD_GLOBAL             11 (NULL + cl)
                      604 LOAD_ATTR               16 (Message)
          
-         355         614 LOAD_CONST              18 ('Chatbot')
+         357         614 LOAD_CONST              18 ('Chatbot')
          
-         356         616 LOAD_GLOBAL             35 (NULL + get_text)
+         358         616 LOAD_GLOBAL             35 (NULL + get_text)
                      628 LOAD_FAST                8 (language)
                      630 LOAD_CONST              19 ('upload_notification')
                      632 PRECALL                  2
                      636 CALL                     2
                      646 FORMAT_VALUE             0
                      648 LOAD_CONST              20 (' ./tmp/')
                      650 LOAD_FAST                3 (save_path)
                      652 FORMAT_VALUE             0
                      654 BUILD_STRING             3
          
-         354         656 KW_NAMES                21
+         356         656 KW_NAMES                21
                      658 PRECALL                  2
                      662 CALL                     2
          
-         357         672 LOAD_METHOD              7 (send)
+         359         672 LOAD_METHOD              7 (send)
                      694 PRECALL                  0
                      698 CALL                     0
          
-         354         708 GET_AWAITABLE            0
+         356         708 GET_AWAITABLE            0
                      710 LOAD_CONST               0 (None)
                  >>  712 SEND                     3 (to 720)
                      714 YIELD_VALUE
                      716 RESUME                   3
                      718 JUMP_BACKWARD_NO_INTERRUPT     4 (to 712)
                  >>  720 POP_TOP
          
-         358         722 LOAD_CONST               0 (None)
+         360         722 LOAD_CONST               0 (None)
                      724 RETURN_VALUE
          
-         360     >>  726 LOAD_GLOBAL             37 (NULL + on_message)
+         362     >>  726 LOAD_GLOBAL             37 (NULL + on_message)
                      738 LOAD_FAST                0 (user_message)
                      740 PRECALL                  1
                      744 CALL                     1
                      754 GET_AWAITABLE            0
                      756 LOAD_CONST               0 (None)
                  >>  758 SEND                     3 (to 766)
                      760 YIELD_VALUE
@@ -2542,61 +2542,61 @@
             'upload_notification'
             ' ./tmp/'
             ('author', 'content')
          names      ('str', 'os', 'path', 'exists', 'mkdir', 'cl', 'AskFileMessage', 'send', 'name', 'content', 'open', 'write', 'user_session', 'get', 'append', 'config_env', 'Message', 'get_text', 'on_message')
          varnames   ('user_message', 'files', 'file', 'save_path', 'file_path', 'content', 'f', 'message_history', 'language')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'run_conversation'
-         firstlineno 324
+         firstlineno 326
          lnotab
             0x060228013e01280116010201020202ff02fd100524fb0e06100104030c
             010e010a020e0322012aff2e023e01180102010afe140426011601020128
             fe100324fd0e040402
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 131
          code
             0x4b00010097007401000000000000000000006401a6010000ab01000000
             000000000001006402610164005300
-         363           0 RETURN_GENERATOR
+         365           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         366           6 LOAD_GLOBAL              1 (NULL + print)
+         368           6 LOAD_GLOBAL              1 (NULL + print)
                       18 LOAD_CONST               1 ('stop chat')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 POP_TOP
          
-         367          36 LOAD_CONST               2 (True)
+         369          36 LOAD_CONST               2 (True)
                       38 STORE_GLOBAL             1 (is_stop)
                       40 LOAD_CONST               0 (None)
                       42 RETURN_VALUE
          consts
             None
             'stop chat'
             True
          names      ('print', 'is_stop')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
          name       'stop_chat'
-         firstlineno 363
+         firstlineno 365
          lnotab 0x06031e01
    names      ('uuid', 'openai', 'json', 'ast', 'os', 'chainlit', 'cl', 'functions.FunctionManager', 'FunctionManager', 'inspect', 'tiktoken', 'importlib', 'asyncio', 'get_text', 'platform', 'path', 'join', 'expanduser', 'config_path', 'open', 'config_file', 'load', 'config_env', 'api_key', 'api_base', 'dirname', 'abspath', '__file__', 'current_dir', 'plugins_dir', 'listdir', 'plugin_dirs', 'functions', 'dir', 'f', 'config', 'get', 'enabled', 'FileNotFoundError', 'import_module', 'module', 'extend', 'getmembers', 'function_manager', 'print', 'generate_functions_array', 'env_max_tokens', 'int', 'max_tokens', 'is_stop', '__truncate_conversation', 'get_token_count', 'MAX_ITER', 'object', 'on_message', 'process_new_delta', 'on_chat_start', 'start_chat', 'run_conversation', 'on_stop', 'stop_chat')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
+   filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal_cn.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c0108010801080108010c0108
       0468031a0120ff2e03260126026401360204011eff120504010801020122
       0120ff2e023001080108ff08030401020228011c011eff220418013c011c
-      010401180204010403060c060e04030c7f001206230c0104ff0e0102350c
+      010401180204010403060c060e04030c7f001206230c0104ff0e0102370c
       010aff0e0102260c0104ff0e01
```

### Comparing `codebot-0.1.1/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.1.2/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.1.2/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.1.2/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/app.py` & `codebot-0.1.2/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/app_cn.py` & `codebot-0.1.2/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/app_terminal.py` & `codebot-0.1.2/src/app_terminal_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/chainlit.md` & `codebot-0.1.2/src/chainlit.md`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/FunctionManager.py` & `codebot-0.1.2/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/RemoteTerminal.py` & `codebot-0.1.2/src/functions/RemoteTerminal.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.1.2/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc` & `codebot-0.1.2/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/get_text.py` & `codebot-0.1.2/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/language/en.json` & `codebot-0.1.2/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/language/zh_CN.json` & `codebot-0.1.2/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.2/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/common/functions.py` & `codebot-0.1.2/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/mysql/functions.py` & `codebot-0.1.2/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.2/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/executor.py` & `codebot-0.1.2/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/python/functions.py` & `codebot-0.1.2/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.1.2/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.1.2/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/terminal/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.2/src/plugins/terminal/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/terminal/functions.py` & `codebot-0.1.2/src/plugins/terminal/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/plugins/vue/functions.py` & `codebot-0.1.2/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/tmp/1690769899.3643498.png` & `codebot-0.1.2/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/tmp/1690769912.7088609.png` & `codebot-0.1.2/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/tmp/sin_function.gif` & `codebot-0.1.2/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.1.1/src/tmp/sin_function.png` & `codebot-0.1.2/src/tmp/sin_function.png`

 * *Files identical despite different names*

