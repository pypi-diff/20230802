# Comparing `tmp/codebot-0.0.7.tar.gz` & `tmp/codebot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.7.tar", last modified: Wed Aug  2 06:51:18 2023, max compression
+gzip compressed data, was "codebot-0.0.8.tar", last modified: Wed Aug  2 06:55:08 2023, max compression
```

## Comparing `codebot-0.0.7.tar` & `codebot-0.0.8.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.706212 codebot-0.0.7/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.7/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:51:18.705844 codebot-0.0.7/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.586570 codebot-0.0.7/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2487 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 06:51:18.000000 codebot-0.0.7/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 06:51:18.706377 codebot-0.0.7/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      571 2023-08-02 06:51:07.000000 codebot-0.0.7/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.595148 codebot-0.0.7/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.597534 codebot-0.0.7/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.0.7/src/.chainlit/.langchain.db
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.0.7/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5835 2023-08-02 06:50:58.000000 codebot-0.0.7/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.618147 codebot-0.0.7/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7921 2023-08-02 06:36:52.000000 codebot-0.0.7/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.7/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.7/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.0.7/src/__pycache__/app.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.7/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.7/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.0.7/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    15650 2023-08-02 06:40:06.000000 codebot-0.0.7/src/__pycache__/app_terminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.7/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.7/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.7/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.7/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.0.7/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    11401 2023-08-02 06:39:48.000000 codebot-0.0.7/src/app_terminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.0.7/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.621986 codebot-0.0.7/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.7/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.7/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.629632 codebot-0.0.7/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.7/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.7/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.7/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.7/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.7/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.635790 codebot-0.0.7/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.7/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.7/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.7/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.636931 codebot-0.0.7/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.7/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.637499 codebot-0.0.7/src/plugins/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.0.7/src/plugins/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.640070 codebot-0.0.7/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.649732 codebot-0.0.7/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.652762 codebot-0.0.7/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.659034 codebot-0.0.7/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.671098 codebot-0.0.7/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.0.7/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.677682 codebot-0.0.7/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.686936 codebot-0.0.7/src/plugins/terminal/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.688590 codebot-0.0.7/src/plugins/terminal/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2410 2023-08-02 06:02:16.000000 codebot-0.0.7/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.0.7/src/plugins/terminal/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1812 2023-08-02 06:00:40.000000 codebot-0.0.7/src/plugins/terminal/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.690450 codebot-0.0.7/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.7/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:51:18.703158 codebot-0.0.7/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.7/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.7/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.7/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.7/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.972961 codebot-0.0.8/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.8/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:55:08.972395 codebot-0.0.8/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.762044 codebot-0.0.8/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2487 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 06:55:08.973885 codebot-0.0.8/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      571 2023-08-02 06:55:05.000000 codebot-0.0.8/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.807150 codebot-0.0.8/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.811267 codebot-0.0.8/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.0.8/src/.chainlit/.langchain.db
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.0.8/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5836 2023-08-02 06:54:59.000000 codebot-0.0.8/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.844973 codebot-0.0.8/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 06:54:52.000000 codebot-0.0.8/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.8/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.8/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.0.8/src/__pycache__/app.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.8/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.8/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.0.8/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    15650 2023-08-02 06:40:06.000000 codebot-0.0.8/src/__pycache__/app_terminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.8/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.0.8/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    11401 2023-08-02 06:39:48.000000 codebot-0.0.8/src/app_terminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.0.8/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.851072 codebot-0.0.8/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.8/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.8/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.862867 codebot-0.0.8/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.8/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.8/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.870865 codebot-0.0.8/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.8/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.8/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.8/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.872888 codebot-0.0.8/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.8/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.875912 codebot-0.0.8/src/plugins/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.0.8/src/plugins/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.878300 codebot-0.0.8/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.886340 codebot-0.0.8/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.893616 codebot-0.0.8/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.898936 codebot-0.0.8/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.917359 codebot-0.0.8/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.0.8/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.927939 codebot-0.0.8/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.938479 codebot-0.0.8/src/plugins/terminal/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.940967 codebot-0.0.8/src/plugins/terminal/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2410 2023-08-02 06:02:16.000000 codebot-0.0.8/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.0.8/src/plugins/terminal/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1812 2023-08-02 06:00:40.000000 codebot-0.0.8/src/plugins/terminal/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.945130 codebot-0.0.8/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.970449 codebot-0.0.8/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.8/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.8/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.8/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.8/src/tmp/sin_function.png
```

### Comparing `codebot-0.0.7/codebot.egg-info/SOURCES.txt` & `codebot-0.0.8/codebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/setup.py` & `codebot-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="codebot",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "codebot = src:main",
             "terminalbot = src:main_terminal",  # 添加这一行
         ],
     },
```

### Comparing `codebot-0.0.7/src/.chainlit/.langchain.db` & `codebot-0.0.8/src/.chainlit/.langchain.db`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/.chainlit/config.toml` & `codebot-0.0.8/src/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__init__.py` & `codebot-0.0.8/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,13 +136,13 @@
     else:
         print("Checking configuration...")
         check_config_terminal()  # Check and create the configuration file if not exists
     
    
             
 
-    subprocess.run(["chainlit", "run", "app_terminal.py" "--port", "10086"])  # Run your application
+    subprocess.run(["chainlit", "run", "app_terminal.py", "--port", "10086"])  # Run your application
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `codebot-0.0.7/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.0.8/src/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x80f9c964 (Wed Aug  2 06:36:48 2023 UTC)
-files sz: 5817
+moddate:  0xbafdc964 (Wed Aug  2 06:54:50 2023 UTC)
+files sz: 5836
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -1093,15 +1093,15 @@
                      610 PRECALL                  0
                      614 CALL                     0
                      624 POP_TOP
          
          143     >>  626 LOAD_GLOBAL             35 (NULL + subprocess)
                      638 LOAD_ATTR               18 (run)
                      648 BUILD_LIST               0
-                     650 LOAD_CONST              11 (('chainlit', 'run', 'app_terminal.py'))
+                     650 LOAD_CONST              11 (('chainlit', 'run', 'app_terminal.py', '--port', '10086'))
                      652 LIST_EXTEND              1
                      654 PRECALL                  1
                      658 CALL                     1
                      668 POP_TOP
                      670 LOAD_CONST               0 (None)
                      672 RETURN_VALUE
          consts
@@ -1112,15 +1112,15 @@
             ('action', 'help')
             '~'
             '.codebot'
             'config.json'
             True
             ('force_config',)
             'Checking configuration...'
-            ('chainlit', 'run', 'app_terminal.py')
+            ('chainlit', 'run', 'app_terminal.py', '--port', '10086')
          names      ('argparse', 'ArgumentParser', 'add_argument', 'parse_args', 'os', 'chdir', 'path', 'dirname', 'abspath', '__file__', 'config', 'join', 'expanduser', 'exists', 'remove', 'check_config_terminal', 'print', 'subprocess', 'run')
          varnames   ('parser', 'args', 'config_path')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
          name       'main_terminal'
          firstlineno 125
```

### Comparing `codebot-0.0.7/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.0.8/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app.cpython-310.pyc` & `codebot-0.0.8/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app.cpython-311.pyc` & `codebot-0.0.8/src/__pycache__/app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app.cpython-38.pyc` & `codebot-0.0.8/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.0.8/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.0.8/src/__pycache__/app_cn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/app_terminal.cpython-311.pyc` & `codebot-0.0.8/src/__pycache__/app_terminal.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.0.8/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.0.8/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.0.8/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/app.py` & `codebot-0.0.8/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/app_cn.py` & `codebot-0.0.8/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/app_terminal.py` & `codebot-0.0.8/src/app_terminal.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/chainlit.md` & `codebot-0.0.8/src/chainlit.md`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/functions/FunctionManager.py` & `codebot-0.0.8/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/get_text.py` & `codebot-0.0.8/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/language/en.json` & `codebot-0.0.8/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/language/zh_CN.json` & `codebot-0.0.8/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/common/functions.py` & `codebot-0.0.8/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/mysql/functions.py` & `codebot-0.0.8/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/executor.py` & `codebot-0.0.8/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/python/functions.py` & `codebot-0.0.8/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.0.8/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.0.8/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/terminal/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.8/src/plugins/terminal/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/terminal/functions.py` & `codebot-0.0.8/src/plugins/terminal/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/plugins/vue/functions.py` & `codebot-0.0.8/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/tmp/1690769899.3643498.png` & `codebot-0.0.8/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/tmp/1690769912.7088609.png` & `codebot-0.0.8/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/tmp/sin_function.gif` & `codebot-0.0.8/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.0.7/src/tmp/sin_function.png` & `codebot-0.0.8/src/tmp/sin_function.png`

 * *Files identical despite different names*

