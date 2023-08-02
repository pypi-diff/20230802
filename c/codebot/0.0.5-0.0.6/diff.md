# Comparing `tmp/codebot-0.0.5.tar.gz` & `tmp/codebot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.5.tar", last modified: Mon Jul 31 03:41:16 2023, max compression
+gzip compressed data, was "codebot-0.0.6.tar", last modified: Wed Aug  2 06:46:32 2023, max compression
```

## Comparing `codebot-0.0.5.tar` & `codebot-0.0.6.tar`

### file list

```diff
@@ -1,80 +1,91 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.397329 codebot-0.0.5/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.5/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:41:16.396884 codebot-0.0.5/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.338219 codebot-0.0.5/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2183 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:41:16.397502 codebot-0.0.5/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      505 2023-07-31 03:41:13.000000 codebot-0.0.5/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.342728 codebot-0.0.5/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.343668 codebot-0.0.5/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1204 2023-07-31 02:17:30.000000 codebot-0.0.5/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.5/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.352409 codebot-0.0.5/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4741 2023-07-31 03:17:06.000000 codebot-0.0.5/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.5/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.5/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.5/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.5/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17324 2023-07-31 03:01:37.000000 codebot-0.0.5/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.5/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12827 2023-07-31 03:25:24.000000 codebot-0.0.5/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      761 2023-07-31 01:29:27.000000 codebot-0.0.5/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.354840 codebot-0.0.5/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.5/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.5/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.361907 codebot-0.0.5/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.5/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.5/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.364034 codebot-0.0.5/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.5/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.5/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.5/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.364903 codebot-0.0.5/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.5/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.366392 codebot-0.0.5/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.369367 codebot-0.0.5/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.372013 codebot-0.0.5/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.374651 codebot-0.0.5/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.379726 codebot-0.0.5/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.382179 codebot-0.0.5/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.387552 codebot-0.0.5/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.395895 codebot-0.0.5/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.5/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.5/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.5/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.5/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.321654 codebot-0.0.6/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.6/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:46:32.320647 codebot-0.0.6/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.188887 codebot-0.0.6/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:46:31.000000 codebot-0.0.6/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2487 2023-08-02 06:46:32.000000 codebot-0.0.6/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 06:46:31.000000 codebot-0.0.6/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 06:46:31.000000 codebot-0.0.6/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-08-02 06:46:31.000000 codebot-0.0.6/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 06:46:31.000000 codebot-0.0.6/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 06:46:32.322564 codebot-0.0.6/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      571 2023-08-02 06:46:22.000000 codebot-0.0.6/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.209072 codebot-0.0.6/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.212475 codebot-0.0.6/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.0.6/src/.chainlit/.langchain.db
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.0.6/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5817 2023-08-02 06:36:48.000000 codebot-0.0.6/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.234702 codebot-0.0.6/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7921 2023-08-02 06:36:52.000000 codebot-0.0.6/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.6/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.6/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.0.6/src/__pycache__/app.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.6/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.6/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.0.6/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    15650 2023-08-02 06:40:06.000000 codebot-0.0.6/src/__pycache__/app_terminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.6/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.6/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.6/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.6/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.0.6/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    11401 2023-08-02 06:39:48.000000 codebot-0.0.6/src/app_terminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.0.6/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.240538 codebot-0.0.6/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.6/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.6/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.249126 codebot-0.0.6/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.6/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.6/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.6/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.6/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.6/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.253614 codebot-0.0.6/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.6/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.6/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.6/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.254902 codebot-0.0.6/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.6/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.255589 codebot-0.0.6/src/plugins/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.0.6/src/plugins/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.261954 codebot-0.0.6/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.266353 codebot-0.0.6/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.268926 codebot-0.0.6/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.272816 codebot-0.0.6/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.289206 codebot-0.0.6/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.0.6/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.295725 codebot-0.0.6/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.302489 codebot-0.0.6/src/plugins/terminal/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.303499 codebot-0.0.6/src/plugins/terminal/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2410 2023-08-02 06:02:16.000000 codebot-0.0.6/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.0.6/src/plugins/terminal/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1812 2023-08-02 06:00:40.000000 codebot-0.0.6/src/plugins/terminal/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.305938 codebot-0.0.6/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.6/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:46:32.316429 codebot-0.0.6/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.6/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.6/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.6/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.6/src/tmp/sin_function.png
```

### Comparing `codebot-0.0.5/codebot.egg-info/SOURCES.txt` & `codebot-0.0.6/codebot.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 codebot.egg-info/dependency_links.txt
 codebot.egg-info/entry_points.txt
 codebot.egg-info/requires.txt
 codebot.egg-info/top_level.txt
 src/__init__.py
 src/app.py
 src/app_cn.py
+src/app_terminal.py
 src/chainlit.md
 src/get_env.py
 src/get_text.py
+src/.chainlit/.langchain.db
 src/.chainlit/config.toml
 src/__pycache__/__init__.cpython-311.pyc
 src/__pycache__/__init__.cpython-38.pyc
 src/__pycache__/app.cpython-310.pyc
+src/__pycache__/app.cpython-311.pyc
 src/__pycache__/app.cpython-38.pyc
 src/__pycache__/app_cn.cpython-310.pyc
 src/__pycache__/app_cn.cpython-311.pyc
+src/__pycache__/app_terminal.cpython-311.pyc
 src/__pycache__/get_text.cpython-310.pyc
 src/__pycache__/get_text.cpython-311.pyc
 src/__pycache__/get_text.cpython-38.pyc
 src/functions/FunctionManager.py
 src/functions/__init__.py
 src/functions/__pycache__/FunctionManager.cpython-310.pyc
 src/functions/__pycache__/FunctionManager.cpython-311.pyc
@@ -30,14 +34,15 @@
 src/functions/__pycache__/__init__.cpython-310.pyc
 src/functions/__pycache__/__init__.cpython-311.pyc
 src/functions/__pycache__/__init__.cpython-38.pyc
 src/language/__init__.py
 src/language/en.json
 src/language/zh_CN.json
 src/plugins/__init__.py
+src/plugins/__pycache__/__init__.cpython-311.pyc
 src/plugins/common/config.json
 src/plugins/common/functions.py
 src/plugins/common/__pycache__/functions.cpython-310.pyc
 src/plugins/common/__pycache__/functions.cpython-311.pyc
 src/plugins/common/__pycache__/functions.cpython-38.pyc
 src/plugins/mysql/config.json
 src/plugins/mysql/functions.py
@@ -49,13 +54,16 @@
 src/plugins/python/__pycache__/executor.cpython-38.pyc
 src/plugins/python/__pycache__/functions.cpython-310.pyc
 src/plugins/python/__pycache__/functions.cpython-311.pyc
 src/plugins/python/__pycache__/functions.cpython-38.pyc
 src/plugins/serverplugin_unfinsh/config.json
 src/plugins/serverplugin_unfinsh/functions.py
 src/plugins/serverplugin_unfinsh/my_apis.json
+src/plugins/terminal/config.json
+src/plugins/terminal/functions.py
+src/plugins/terminal/__pycache__/functions.cpython-311.pyc
 src/plugins/vue/config.json
 src/plugins/vue/functions.py
 src/tmp/1690769899.3643498.png
 src/tmp/1690769912.7088609.png
 src/tmp/sin_function.gif
 src/tmp/sin_function.png
```

### Comparing `codebot-0.0.5/src/.chainlit/config.toml` & `codebot-0.0.6/src/.chainlit/config.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Name of the app and chatbot.
 name = "Chatbot"
 
 # Description of the app and chatbot. This is used for HTML tags.
 # description = ""
 
 # The default value for the expand messages settings.
-default_expand_messages = false
+default_expand_messages = true
 
 # Hide the chain of thought details from the user in the UI.
 hide_cot = false
 
 # Link to your github repo. This will add a github button in the UI's header.
 # github = ""
```

### Comparing `codebot-0.0.5/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.0.6/src/__pycache__/__init__.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xae27c764 (Mon Jul 31 03:17:02 2023 UTC)
-files sz: 3134
+moddate:  0x80f9c964 (Wed Aug  2 06:36:48 2023 UTC)
+files sz: 5817
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      016c035a03640064026c046d055a0501006407640484015a06640584005a
-      07650864066b0200000000720c02006507a6000000ab0000000000000000
-      0001006401530064015300
+      016c035a03640064026c046d055a0501006409640484015a066409640584
+      015a07640684005a08640784005a09650a64086b0200000000720c020065
+      08a6000000ab00000000000000000001006401530064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (os)
                  8 STORE_NAME               0 (os)
    
@@ -36,38 +36,47 @@
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               2 (('ngrok',))
                 38 IMPORT_NAME              4 (pyngrok)
                 40 IMPORT_FROM              5 (ngrok)
                 42 STORE_NAME               5 (ngrok)
                 44 POP_TOP
    
-     7          46 LOAD_CONST               7 ((False,))
+     7          46 LOAD_CONST               9 ((False,))
                 48 LOAD_CONST               4 (<code object check_config, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 7>)
                 50 MAKE_FUNCTION            1 (defaults)
                 52 STORE_NAME               6 (check_config)
    
-    46          54 LOAD_CONST               5 (<code object main, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 46>)
-                56 MAKE_FUNCTION            0
-                58 STORE_NAME               7 (main)
-   
-    83          60 LOAD_NAME                8 (__name__)
-                62 LOAD_CONST               6 ('__main__')
-                64 COMPARE_OP               2 (==)
-                70 POP_JUMP_FORWARD_IF_FALSE    12 (to 96)
-   
-    84          72 PUSH_NULL
-                74 LOAD_NAME                7 (main)
-                76 PRECALL                  0
-                80 CALL                     0
-                90 POP_TOP
-                92 LOAD_CONST               1 (None)
-                94 RETURN_VALUE
+    46          54 LOAD_CONST               9 ((False,))
+                56 LOAD_CONST               5 (<code object check_config_terminal, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 46>)
+                58 MAKE_FUNCTION            1 (defaults)
+                60 STORE_NAME               7 (check_config_terminal)
    
-    83     >>   96 LOAD_CONST               1 (None)
-                98 RETURN_VALUE
+    89          62 LOAD_CONST               6 (<code object main, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 89>)
+                64 MAKE_FUNCTION            0
+                66 STORE_NAME               8 (main)
+   
+   125          68 LOAD_CONST               7 (<code object main_terminal, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py", line 125>)
+                70 MAKE_FUNCTION            0
+                72 STORE_NAME               9 (main_terminal)
+   
+   147          74 LOAD_NAME               10 (__name__)
+                76 LOAD_CONST               8 ('__main__')
+                78 COMPARE_OP               2 (==)
+                84 POP_JUMP_FORWARD_IF_FALSE    12 (to 110)
+   
+   148          86 PUSH_NULL
+                88 LOAD_NAME                8 (main)
+                90 PRECALL                  0
+                94 CALL                     0
+               104 POP_TOP
+               106 LOAD_CONST               1 (None)
+               108 RETURN_VALUE
+   
+   147     >>  110 LOAD_CONST               1 (None)
+               112 RETURN_VALUE
    consts
       0
       None
       ('ngrok',)
       False
       code
          argcount  : 1
@@ -352,14 +361,335 @@
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
          name       'check_config'
          firstlineno 7
          lnotab
             0x02027c040201020102010201020102fb04ff040b3e02660122012aff2e
             04220128ff2e0420023e012c010401180322012aff34f8
       code
+         argcount  : 1
+         nlocals   : 8
+         stacksize : 8
+         flags     : 3
+         code
+            0x97007400000000000000000000006a010000000000000000a002000000
+            00000000000000000000000000000000007400000000000000000000006a
+            010000000000000000a00300000000000000000000000000000000000000
+            006401a6010000ab01000000000000000064026403a6030000ab03000000
+            00000000007d016404640564066407640864096406640a9c0669017d0274
+            00000000000000000000006a010000000000000000a00400000000000000
+            000000000000000000000000007c01a6010000ab01000000000000000073
+            707401000000000000000000006a05000000000000000074000000000000
+            00000000006a010000000000000000a00600000000000000000000000000
+            000000000000007c01a6010000ab010000000000000000640bac0ca60200
+            00ab0200000000000000000100740f000000000000000000007c01640da6
+            020000ab02000000000000000035007d037411000000000000000000006a
+            0900000000000000007c027c03a6020000ab020000000000000000010064
+            0064006400a6020000ab02000000000000000001006e0b23003100730477
+            027803590077010100590001000100740f000000000000000000007c0164
+            0ea6020000ab02000000000000000035007d037411000000000000000000
+            006a0a00000000000000007c03a6010000ab0100000000000000007d0464
+            0064006400a6020000ab02000000000000000001006e0b23003100730477
+            0278035900770101005900010001007c00730e7c04640419000000000000
+            000000640f1900000000000000000073ab7c026404190000000000000000
+            00a00b0000000000000000000000000000000000000000a6000000ab0000
+            0000000000000044005d505c0200007d057d067419000000000000000000
+            0064107c059b0064117c069b0064129d05a6010000ab0100000000000000
+            007d077c0564136b020000000072227c0764066b0200000000721c741900
+            00000000000000000064107c059b0064117c069b0064129d05a6010000ab
+            0100000000000000007d077c0764066b0200000000b01c7c07720b7c077c
+            046404190000000000000000007c053c0000008c51740f00000000000000
+            0000007c01640da6020000ab02000000000000000035007d037411000000
+            000000000000006a0900000000000000007c047c03a6020000ab02000000
+            00000000000100640064006400a6020000ab020000000000000000010064
+            005300230031007304770278035900770101005900010001006400530064
+            005300
+          46           0 RESUME                   0
+         
+          48           2 LOAD_GLOBAL              0 (os)
+                      14 LOAD_ATTR                1 (path)
+                      24 LOAD_METHOD              2 (join)
+                      46 LOAD_GLOBAL              0 (os)
+                      58 LOAD_ATTR                1 (path)
+                      68 LOAD_METHOD              3 (expanduser)
+                      90 LOAD_CONST               1 ('~')
+                      92 PRECALL                  1
+                      96 CALL                     1
+                     106 LOAD_CONST               2 ('.codebot')
+                     108 LOAD_CONST               3 ('config.json')
+                     110 PRECALL                  3
+                     114 CALL                     3
+                     124 STORE_FAST               1 (config_path)
+         
+          52         126 LOAD_CONST               4 ('openai')
+         
+          53         128 LOAD_CONST               5 ('https://api.openai.com/v1')
+         
+          54         130 LOAD_CONST               6 ('')
+         
+          55         132 LOAD_CONST               7 ('gpt-3.5-turbo-16k')
+         
+          56         134 LOAD_CONST               8 ('5000')
+         
+          57         136 LOAD_CONST               9 ('chinese')
+         
+          58         138 LOAD_CONST               6 ('')
+         
+          52         140 LOAD_CONST              10 (('api_base', 'api_key', 'model', 'max_tokens', 'language', 'password'))
+                     142 BUILD_CONST_KEY_MAP      6
+         
+          51         144 BUILD_MAP                1
+                     146 STORE_FAST               2 (default_config)
+         
+          63         148 LOAD_GLOBAL              0 (os)
+                     160 LOAD_ATTR                1 (path)
+                     170 LOAD_METHOD              4 (exists)
+                     192 LOAD_FAST                1 (config_path)
+                     194 PRECALL                  1
+                     198 CALL                     1
+                     208 POP_JUMP_FORWARD_IF_TRUE   112 (to 434)
+         
+          65         210 LOAD_GLOBAL              1 (NULL + os)
+                     222 LOAD_ATTR                5 (makedirs)
+                     232 LOAD_GLOBAL              0 (os)
+                     244 LOAD_ATTR                1 (path)
+                     254 LOAD_METHOD              6 (dirname)
+                     276 LOAD_FAST                1 (config_path)
+                     278 PRECALL                  1
+                     282 CALL                     1
+                     292 LOAD_CONST              11 (True)
+                     294 KW_NAMES                12
+                     296 PRECALL                  2
+                     300 CALL                     2
+                     310 POP_TOP
+         
+          66         312 LOAD_GLOBAL             15 (NULL + open)
+                     324 LOAD_FAST                1 (config_path)
+                     326 LOAD_CONST              13 ('w')
+                     328 PRECALL                  2
+                     332 CALL                     2
+                     342 BEFORE_WITH
+                     344 STORE_FAST               3 (config_file)
+         
+          67         346 LOAD_GLOBAL             17 (NULL + json)
+                     358 LOAD_ATTR                9 (dump)
+                     368 LOAD_FAST                2 (default_config)
+                     370 LOAD_FAST                3 (config_file)
+                     372 PRECALL                  2
+                     376 CALL                     2
+                     386 POP_TOP
+         
+          66         388 LOAD_CONST               0 (None)
+                     390 LOAD_CONST               0 (None)
+                     392 LOAD_CONST               0 (None)
+                     394 PRECALL                  2
+                     398 CALL                     2
+                     408 POP_TOP
+                     410 JUMP_FORWARD            11 (to 434)
+                 >>  412 PUSH_EXC_INFO
+                     414 WITH_EXCEPT_START
+                     416 POP_JUMP_FORWARD_IF_TRUE     4 (to 426)
+                     418 RERAISE                  2
+                 >>  420 COPY                     3
+                     422 POP_EXCEPT
+                     424 RERAISE                  1
+                 >>  426 POP_TOP
+                     428 POP_EXCEPT
+                     430 POP_TOP
+                     432 POP_TOP
+         
+          70     >>  434 LOAD_GLOBAL             15 (NULL + open)
+                     446 LOAD_FAST                1 (config_path)
+                     448 LOAD_CONST              14 ('r')
+                     450 PRECALL                  2
+                     454 CALL                     2
+                     464 BEFORE_WITH
+                     466 STORE_FAST               3 (config_file)
+         
+          71         468 LOAD_GLOBAL             17 (NULL + json)
+                     480 LOAD_ATTR               10 (load)
+                     490 LOAD_FAST                3 (config_file)
+                     492 PRECALL                  1
+                     496 CALL                     1
+                     506 STORE_FAST               4 (config)
+         
+          70         508 LOAD_CONST               0 (None)
+                     510 LOAD_CONST               0 (None)
+                     512 LOAD_CONST               0 (None)
+                     514 PRECALL                  2
+                     518 CALL                     2
+                     528 POP_TOP
+                     530 JUMP_FORWARD            11 (to 554)
+                 >>  532 PUSH_EXC_INFO
+                     534 WITH_EXCEPT_START
+                     536 POP_JUMP_FORWARD_IF_TRUE     4 (to 546)
+                     538 RERAISE                  2
+                 >>  540 COPY                     3
+                     542 POP_EXCEPT
+                     544 RERAISE                  1
+                 >>  546 POP_TOP
+                     548 POP_EXCEPT
+                     550 POP_TOP
+                     552 POP_TOP
+         
+          74     >>  554 LOAD_FAST                0 (force_config)
+                     556 POP_JUMP_FORWARD_IF_TRUE    14 (to 586)
+                     558 LOAD_FAST                4 (config)
+                     560 LOAD_CONST               4 ('openai')
+                     562 BINARY_SUBSCR
+                     572 LOAD_CONST              15 ('api_key')
+                     574 BINARY_SUBSCR
+                     584 POP_JUMP_FORWARD_IF_TRUE   171 (to 928)
+         
+          76     >>  586 LOAD_FAST                2 (default_config)
+                     588 LOAD_CONST               4 ('openai')
+                     590 BINARY_SUBSCR
+                     600 LOAD_METHOD             11 (items)
+                     622 PRECALL                  0
+                     626 CALL                     0
+                     636 GET_ITER
+                 >>  638 FOR_ITER                80 (to 800)
+                     640 UNPACK_SEQUENCE          2
+                     644 STORE_FAST               5 (key)
+                     646 STORE_FAST               6 (default_value)
+         
+          77         648 LOAD_GLOBAL             25 (NULL + input)
+                     660 LOAD_CONST              16 ('Please enter ')
+                     662 LOAD_FAST                5 (key)
+                     664 FORMAT_VALUE             0
+                     666 LOAD_CONST              17 (" (default is '")
+                     668 LOAD_FAST                6 (default_value)
+                     670 FORMAT_VALUE             0
+                     672 LOAD_CONST              18 ("'): ")
+                     674 BUILD_STRING             5
+                     676 PRECALL                  1
+                     680 CALL                     1
+                     690 STORE_FAST               7 (user_input)
+         
+          78         692 LOAD_FAST                5 (key)
+                     694 LOAD_CONST              19 ('password')
+                     696 COMPARE_OP               2 (==)
+                     702 POP_JUMP_FORWARD_IF_FALSE    34 (to 772)
+         
+          79         704 LOAD_FAST                7 (user_input)
+                     706 LOAD_CONST               6 ('')
+                     708 COMPARE_OP               2 (==)
+                     714 POP_JUMP_FORWARD_IF_FALSE    28 (to 772)
+         
+          80     >>  716 LOAD_GLOBAL             25 (NULL + input)
+                     728 LOAD_CONST              16 ('Please enter ')
+                     730 LOAD_FAST                5 (key)
+                     732 FORMAT_VALUE             0
+                     734 LOAD_CONST              17 (" (default is '")
+                     736 LOAD_FAST                6 (default_value)
+                     738 FORMAT_VALUE             0
+                     740 LOAD_CONST              18 ("'): ")
+                     742 BUILD_STRING             5
+                     744 PRECALL                  1
+                     748 CALL                     1
+                     758 STORE_FAST               7 (user_input)
+         
+          79         760 LOAD_FAST                7 (user_input)
+                     762 LOAD_CONST               6 ('')
+                     764 COMPARE_OP               2 (==)
+                     770 POP_JUMP_BACKWARD_IF_TRUE    28 (to 716)
+         
+          81     >>  772 LOAD_FAST                7 (user_input)
+                     774 POP_JUMP_FORWARD_IF_FALSE    11 (to 798)
+         
+          82         776 LOAD_FAST                7 (user_input)
+                     778 LOAD_FAST                4 (config)
+                     780 LOAD_CONST               4 ('openai')
+                     782 BINARY_SUBSCR
+                     792 LOAD_FAST                5 (key)
+                     794 STORE_SUBSCR
+                 >>  798 JUMP_BACKWARD           81 (to 638)
+         
+          85     >>  800 LOAD_GLOBAL             15 (NULL + open)
+                     812 LOAD_FAST                1 (config_path)
+                     814 LOAD_CONST              13 ('w')
+                     816 PRECALL                  2
+                     820 CALL                     2
+                     830 BEFORE_WITH
+                     832 STORE_FAST               3 (config_file)
+         
+          86         834 LOAD_GLOBAL             17 (NULL + json)
+                     846 LOAD_ATTR                9 (dump)
+                     856 LOAD_FAST                4 (config)
+                     858 LOAD_FAST                3 (config_file)
+                     860 PRECALL                  2
+                     864 CALL                     2
+                     874 POP_TOP
+         
+          85         876 LOAD_CONST               0 (None)
+                     878 LOAD_CONST               0 (None)
+                     880 LOAD_CONST               0 (None)
+                     882 PRECALL                  2
+                     886 CALL                     2
+                     896 POP_TOP
+                     898 LOAD_CONST               0 (None)
+                     900 RETURN_VALUE
+                 >>  902 PUSH_EXC_INFO
+                     904 WITH_EXCEPT_START
+                     906 POP_JUMP_FORWARD_IF_TRUE     4 (to 916)
+                     908 RERAISE                  2
+                 >>  910 COPY                     3
+                     912 POP_EXCEPT
+                     914 RERAISE                  1
+                 >>  916 POP_TOP
+                     918 POP_EXCEPT
+                     920 POP_TOP
+                     922 POP_TOP
+                     924 LOAD_CONST               0 (None)
+                     926 RETURN_VALUE
+         
+          74     >>  928 LOAD_CONST               0 (None)
+                     930 RETURN_VALUE
+         ExceptionTable:
+           344 to 386 -> 412 [1] lasti
+           412 to 418 -> 420 [3] lasti
+           426 to 426 -> 420 [3] lasti
+           466 to 506 -> 532 [1] lasti
+           532 to 538 -> 540 [3] lasti
+           546 to 546 -> 540 [3] lasti
+           832 to 874 -> 902 [1] lasti
+           902 to 908 -> 910 [3] lasti
+           916 to 916 -> 910 [3] lasti
+         consts
+            None
+            '~'
+            '.codebot'
+            'config.json'
+            'openai'
+            'https://api.openai.com/v1'
+            ''
+            'gpt-3.5-turbo-16k'
+            '5000'
+            'chinese'
+            ('api_base', 'api_key', 'model', 'max_tokens', 'language', 'password')
+            True
+            ('exist_ok',)
+            'w'
+            'r'
+            'api_key'
+            'Please enter '
+            " (default is '"
+            "'): "
+            'password'
+         names      ('os', 'path', 'join', 'expanduser', 'exists', 'makedirs', 'dirname', 'open', 'json', 'dump', 'load', 'items', 'input')
+         varnames   ('force_config', 'config_path', 'default_config', 'config_file', 'config', 'key', 'default_value', 'user_input')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
+         name       'check_config_terminal'
+         firstlineno 46
+         lnotab
+            0x02027c0402010201020102010201020102fa04ff040c3e02660122012a
+            ff2e04220128ff2e0420023e012c010c010c012cff0c020401180322012a
+            ff34f5
+      code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a010000000000000000a6000000ab
             0000000000000000007d007c00a002000000000000000000000000000000
@@ -395,58 +725,58 @@
             000000000000002400721c7d0474230000000000000000000064127c049b
             009d02a6010000ab0100000000000000000100590064007d047e046e0864
             007d047e04770177007803590077017c016a180000000000000000721874
             33000000000000000000006a1a000000000000000067006413a201a60100
             00ab0100000000000000000100640053007433000000000000000000006a
             1a000000000000000067006414a201a6010000ab01000000000000000001
             0064005300
-          46           0 RESUME                   0
+          89           0 RESUME                   0
          
-          47           2 LOAD_GLOBAL              1 (NULL + argparse)
+          90           2 LOAD_GLOBAL              1 (NULL + argparse)
                       14 LOAD_ATTR                1 (ArgumentParser)
                       24 PRECALL                  0
                       28 CALL                     0
                       38 STORE_FAST               0 (parser)
          
-          48          40 LOAD_FAST                0 (parser)
+          91          40 LOAD_FAST                0 (parser)
                       42 LOAD_METHOD              2 (add_argument)
                       64 LOAD_CONST               1 ('--fix')
                       66 LOAD_CONST               2 ('store_true')
                       68 KW_NAMES                 3
                       70 PRECALL                  2
                       74 CALL                     2
                       84 POP_TOP
          
-          49          86 LOAD_FAST                0 (parser)
+          92          86 LOAD_FAST                0 (parser)
                       88 LOAD_METHOD              2 (add_argument)
                      110 LOAD_CONST               4 ('--ngrok')
                      112 LOAD_GLOBAL              6 (str)
                      124 LOAD_CONST               5 ('Ngrok auth token')
                      126 KW_NAMES                 6
                      128 PRECALL                  3
                      132 CALL                     3
                      142 POP_TOP
          
-          50         144 LOAD_FAST                0 (parser)
+          93         144 LOAD_FAST                0 (parser)
                      146 LOAD_METHOD              2 (add_argument)
                      168 LOAD_CONST               7 ('--config')
                      170 LOAD_CONST               2 ('store_true')
                      172 LOAD_CONST               8 ('Reset configuration')
                      174 KW_NAMES                 9
                      176 PRECALL                  3
                      180 CALL                     3
                      190 POP_TOP
          
-          51         192 LOAD_FAST                0 (parser)
+          94         192 LOAD_FAST                0 (parser)
                      194 LOAD_METHOD              4 (parse_args)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 STORE_FAST               1 (args)
          
-          53         232 LOAD_GLOBAL             11 (NULL + os)
+          96         232 LOAD_GLOBAL             11 (NULL + os)
                      244 LOAD_ATTR                6 (chdir)
                      254 LOAD_GLOBAL             10 (os)
                      266 LOAD_ATTR                7 (path)
                      276 LOAD_METHOD              8 (dirname)
                      298 LOAD_GLOBAL             10 (os)
                      310 LOAD_ATTR                7 (path)
                      320 LOAD_METHOD              9 (abspath)
@@ -455,112 +785,112 @@
                      358 CALL                     1
                      368 PRECALL                  1
                      372 CALL                     1
                      382 PRECALL                  1
                      386 CALL                     1
                      396 POP_TOP
          
-          55         398 LOAD_FAST                1 (args)
+          98         398 LOAD_FAST                1 (args)
                      400 LOAD_ATTR               11 (config)
                      410 POP_JUMP_FORWARD_IF_FALSE   130 (to 672)
          
-          57         412 LOAD_GLOBAL             10 (os)
+         100         412 LOAD_GLOBAL             10 (os)
                      424 LOAD_ATTR                7 (path)
                      434 LOAD_METHOD             12 (join)
                      456 LOAD_GLOBAL             10 (os)
                      468 LOAD_ATTR                7 (path)
                      478 LOAD_METHOD             13 (expanduser)
                      500 LOAD_CONST              10 ('~')
                      502 PRECALL                  1
                      506 CALL                     1
                      516 LOAD_CONST              11 ('.codebot')
                      518 LOAD_CONST              12 ('config.json')
                      520 PRECALL                  3
                      524 CALL                     3
                      534 STORE_FAST               2 (config_path)
          
-          58         536 LOAD_GLOBAL             10 (os)
+         101         536 LOAD_GLOBAL             10 (os)
                      548 LOAD_ATTR                7 (path)
                      558 LOAD_METHOD             14 (exists)
                      580 LOAD_FAST                2 (config_path)
                      582 PRECALL                  1
                      586 CALL                     1
                      596 POP_JUMP_FORWARD_IF_FALSE    20 (to 638)
          
-          59         598 LOAD_GLOBAL             11 (NULL + os)
+         102         598 LOAD_GLOBAL             11 (NULL + os)
                      610 LOAD_ATTR               15 (remove)
                      620 LOAD_FAST                2 (config_path)
                      622 PRECALL                  1
                      626 CALL                     1
                      636 POP_TOP
          
-          60     >>  638 LOAD_GLOBAL             33 (NULL + check_config)
+         103     >>  638 LOAD_GLOBAL             33 (NULL + check_config)
                      650 LOAD_CONST              13 (True)
                      652 KW_NAMES                14
                      654 PRECALL                  1
                      658 CALL                     1
                      668 POP_TOP
                      670 JUMP_FORWARD            29 (to 730)
          
-          62     >>  672 LOAD_GLOBAL             35 (NULL + print)
+         105     >>  672 LOAD_GLOBAL             35 (NULL + print)
                      684 LOAD_CONST              15 ('Checking configuration...')
                      686 PRECALL                  1
                      690 CALL                     1
                      700 POP_TOP
          
-          63         702 LOAD_GLOBAL             33 (NULL + check_config)
+         106         702 LOAD_GLOBAL             33 (NULL + check_config)
                      714 PRECALL                  0
                      718 CALL                     0
                      728 POP_TOP
          
-          65     >>  730 LOAD_FAST                1 (args)
+         108     >>  730 LOAD_FAST                1 (args)
                      732 LOAD_ATTR               18 (ngrok)
                      742 POP_JUMP_FORWARD_IF_FALSE   130 (to 1004)
          
-          66         744 NOP
+         109         744 NOP
          
-          67         746 LOAD_GLOBAL             37 (NULL + ngrok)
+         110         746 LOAD_GLOBAL             37 (NULL + ngrok)
                      758 LOAD_ATTR               19 (kill)
                      768 PRECALL                  0
                      772 CALL                     0
                      782 POP_TOP
          
-          69         784 LOAD_GLOBAL             37 (NULL + ngrok)
+         112         784 LOAD_GLOBAL             37 (NULL + ngrok)
                      796 LOAD_ATTR               20 (set_auth_token)
                      806 LOAD_FAST                1 (args)
                      808 LOAD_ATTR               18 (ngrok)
                      818 PRECALL                  1
                      822 CALL                     1
                      832 POP_TOP
          
-          71         834 LOAD_GLOBAL             37 (NULL + ngrok)
+         114         834 LOAD_GLOBAL             37 (NULL + ngrok)
                      846 LOAD_ATTR               21 (connect)
                      856 LOAD_CONST              16 (8000)
                      858 PRECALL                  1
                      862 CALL                     1
                      872 STORE_FAST               3 (ngrok_tunnel)
          
-          72         874 LOAD_GLOBAL             35 (NULL + print)
+         115         874 LOAD_GLOBAL             35 (NULL + print)
                      886 LOAD_CONST              17 ('Ngrok Tunnel Opened: ')
                      888 LOAD_FAST                3 (ngrok_tunnel)
                      890 LOAD_ATTR               22 (public_url)
                      900 FORMAT_VALUE             0
                      902 BUILD_STRING             2
                      904 PRECALL                  1
                      908 CALL                     1
                      918 POP_TOP
                      920 JUMP_FORWARD            41 (to 1004)
                  >>  922 PUSH_EXC_INFO
          
-          73         924 LOAD_GLOBAL             46 (Exception)
+         116         924 LOAD_GLOBAL             46 (Exception)
                      936 CHECK_EXC_MATCH
                      938 POP_JUMP_FORWARD_IF_FALSE    28 (to 996)
                      940 STORE_FAST               4 (e)
          
-          74         942 LOAD_GLOBAL             35 (NULL + print)
+         117         942 LOAD_GLOBAL             35 (NULL + print)
                      954 LOAD_CONST              18 ('Failed to set up ngrok tunnel: ')
                      956 LOAD_FAST                4 (e)
                      958 FORMAT_VALUE             0
                      960 BUILD_STRING             2
                      962 PRECALL                  1
                      966 CALL                     1
                      976 POP_TOP
@@ -570,35 +900,35 @@
                      984 DELETE_FAST              4 (e)
                      986 JUMP_FORWARD             8 (to 1004)
                  >>  988 LOAD_CONST               0 (None)
                      990 STORE_FAST               4 (e)
                      992 DELETE_FAST              4 (e)
                      994 RERAISE                  1
          
-          73     >>  996 RERAISE                  0
+         116     >>  996 RERAISE                  0
                  >>  998 COPY                     3
                     1000 POP_EXCEPT
                     1002 RERAISE                  1
          
-          76     >> 1004 LOAD_FAST                1 (args)
+         119     >> 1004 LOAD_FAST                1 (args)
                     1006 LOAD_ATTR               24 (fix)
                     1016 POP_JUMP_FORWARD_IF_FALSE    24 (to 1066)
          
-          77        1018 LOAD_GLOBAL             51 (NULL + subprocess)
+         120        1018 LOAD_GLOBAL             51 (NULL + subprocess)
                     1030 LOAD_ATTR               26 (run)
                     1040 BUILD_LIST               0
                     1042 LOAD_CONST              19 (('chainlit', 'run', 'app_cn.py'))
                     1044 LIST_EXTEND              1
                     1046 PRECALL                  1
                     1050 CALL                     1
                     1060 POP_TOP
                     1062 LOAD_CONST               0 (None)
                     1064 RETURN_VALUE
          
-          79     >> 1066 LOAD_GLOBAL             51 (NULL + subprocess)
+         122     >> 1066 LOAD_GLOBAL             51 (NULL + subprocess)
                     1078 LOAD_ATTR               26 (run)
                     1088 BUILD_LIST               0
                     1090 LOAD_CONST              20 (('chainlit', 'run', 'app.py'))
                     1092 LIST_EXTEND              1
                     1094 PRECALL                  1
                     1098 CALL                     1
                     1108 POP_TOP
@@ -633,21 +963,175 @@
             ('chainlit', 'run', 'app.py')
          names      ('argparse', 'ArgumentParser', 'add_argument', 'str', 'parse_args', 'os', 'chdir', 'path', 'dirname', 'abspath', '__file__', 'config', 'join', 'expanduser', 'exists', 'remove', 'check_config', 'print', 'ngrok', 'kill', 'set_auth_token', 'connect', 'public_url', 'Exception', 'fix', 'subprocess', 'run')
          varnames   ('parser', 'args', 'config_path', 'ngrok_tunnel', 'e')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
          name       'main'
-         firstlineno 46
+         firstlineno 89
          lnotab
             0x020126012e013a0130012802a6020e027c013e01280122021e011c020e
             0102012602320228013201120136ff08030e013002
+      code
+         argcount  : 0
+         nlocals   : 3
+         stacksize : 7
+         flags     : 3
+         code
+            0x97007401000000000000000000006a010000000000000000a6000000ab
+            0000000000000000007d007c00a002000000000000000000000000000000
+            0000000000640164026403ac04a6030000ab03000000000000000001007c
+            00a0030000000000000000000000000000000000000000a6000000ab0000
+            000000000000007d017409000000000000000000006a0500000000000000
+            007408000000000000000000006a060000000000000000a0070000000000
+            0000000000000000000000000000007408000000000000000000006a0600
+            00000000000000a008000000000000000000000000000000000000000074
+            1200000000000000000000a6010000ab010000000000000000a6010000ab
+            010000000000000000a6010000ab01000000000000000001007c016a0a00
+            0000000000000072827408000000000000000000006a0600000000000000
+            00a00b000000000000000000000000000000000000000074080000000000
+            00000000006a060000000000000000a00c00000000000000000000000000
+            000000000000006405a6010000ab01000000000000000064066407a60300
+            00ab0300000000000000007d027408000000000000000000006a06000000
+            0000000000a00d00000000000000000000000000000000000000007c02a6
+            010000ab01000000000000000072147409000000000000000000006a0e00
+            000000000000007c02a6010000ab0100000000000000000100741f000000
+            000000000000006408ac09a6010000ab01000000000000000001006e1d74
+            2100000000000000000000640aa6010000ab010000000000000000010074
+            1f00000000000000000000a6000000ab0000000000000000000100742300
+            0000000000000000006a1200000000000000006700640ba201a6010000ab
+            010000000000000000010064005300
+         125           0 RESUME                   0
+         
+         126           2 LOAD_GLOBAL              1 (NULL + argparse)
+                      14 LOAD_ATTR                1 (ArgumentParser)
+                      24 PRECALL                  0
+                      28 CALL                     0
+                      38 STORE_FAST               0 (parser)
+         
+         127          40 LOAD_FAST                0 (parser)
+                      42 LOAD_METHOD              2 (add_argument)
+                      64 LOAD_CONST               1 ('--config')
+                      66 LOAD_CONST               2 ('store_true')
+                      68 LOAD_CONST               3 ('Reset configuration')
+                      70 KW_NAMES                 4
+                      72 PRECALL                  3
+                      76 CALL                     3
+                      86 POP_TOP
+         
+         128          88 LOAD_FAST                0 (parser)
+                      90 LOAD_METHOD              3 (parse_args)
+                     112 PRECALL                  0
+                     116 CALL                     0
+                     126 STORE_FAST               1 (args)
+         
+         129         128 LOAD_GLOBAL              9 (NULL + os)
+                     140 LOAD_ATTR                5 (chdir)
+                     150 LOAD_GLOBAL              8 (os)
+                     162 LOAD_ATTR                6 (path)
+                     172 LOAD_METHOD              7 (dirname)
+                     194 LOAD_GLOBAL              8 (os)
+                     206 LOAD_ATTR                6 (path)
+                     216 LOAD_METHOD              8 (abspath)
+                     238 LOAD_GLOBAL             18 (__file__)
+                     250 PRECALL                  1
+                     254 CALL                     1
+                     264 PRECALL                  1
+                     268 CALL                     1
+                     278 PRECALL                  1
+                     282 CALL                     1
+                     292 POP_TOP
+         
+         130         294 LOAD_FAST                1 (args)
+                     296 LOAD_ATTR               10 (config)
+                     306 POP_JUMP_FORWARD_IF_FALSE   130 (to 568)
+         
+         132         308 LOAD_GLOBAL              8 (os)
+                     320 LOAD_ATTR                6 (path)
+                     330 LOAD_METHOD             11 (join)
+                     352 LOAD_GLOBAL              8 (os)
+                     364 LOAD_ATTR                6 (path)
+                     374 LOAD_METHOD             12 (expanduser)
+                     396 LOAD_CONST               5 ('~')
+                     398 PRECALL                  1
+                     402 CALL                     1
+                     412 LOAD_CONST               6 ('.codebot')
+                     414 LOAD_CONST               7 ('config.json')
+                     416 PRECALL                  3
+                     420 CALL                     3
+                     430 STORE_FAST               2 (config_path)
+         
+         133         432 LOAD_GLOBAL              8 (os)
+                     444 LOAD_ATTR                6 (path)
+                     454 LOAD_METHOD             13 (exists)
+                     476 LOAD_FAST                2 (config_path)
+                     478 PRECALL                  1
+                     482 CALL                     1
+                     492 POP_JUMP_FORWARD_IF_FALSE    20 (to 534)
+         
+         134         494 LOAD_GLOBAL              9 (NULL + os)
+                     506 LOAD_ATTR               14 (remove)
+                     516 LOAD_FAST                2 (config_path)
+                     518 PRECALL                  1
+                     522 CALL                     1
+                     532 POP_TOP
+         
+         135     >>  534 LOAD_GLOBAL             31 (NULL + check_config_terminal)
+                     546 LOAD_CONST               8 (True)
+                     548 KW_NAMES                 9
+                     550 PRECALL                  1
+                     554 CALL                     1
+                     564 POP_TOP
+                     566 JUMP_FORWARD            29 (to 626)
+         
+         137     >>  568 LOAD_GLOBAL             33 (NULL + print)
+                     580 LOAD_CONST              10 ('Checking configuration...')
+                     582 PRECALL                  1
+                     586 CALL                     1
+                     596 POP_TOP
+         
+         138         598 LOAD_GLOBAL             31 (NULL + check_config_terminal)
+                     610 PRECALL                  0
+                     614 CALL                     0
+                     624 POP_TOP
+         
+         143     >>  626 LOAD_GLOBAL             35 (NULL + subprocess)
+                     638 LOAD_ATTR               18 (run)
+                     648 BUILD_LIST               0
+                     650 LOAD_CONST              11 (('chainlit', 'run', 'app_terminal.py'))
+                     652 LIST_EXTEND              1
+                     654 PRECALL                  1
+                     658 CALL                     1
+                     668 POP_TOP
+                     670 LOAD_CONST               0 (None)
+                     672 RETURN_VALUE
+         consts
+            None
+            '--config'
+            'store_true'
+            'Reset configuration'
+            ('action', 'help')
+            '~'
+            '.codebot'
+            'config.json'
+            True
+            ('force_config',)
+            'Checking configuration...'
+            ('chainlit', 'run', 'app_terminal.py')
+         names      ('argparse', 'ArgumentParser', 'add_argument', 'parse_args', 'os', 'chdir', 'path', 'dirname', 'abspath', '__file__', 'config', 'join', 'expanduser', 'exists', 'remove', 'check_config_terminal', 'print', 'subprocess', 'run')
+         varnames   ('parser', 'args', 'config_path')
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
+         name       'main_terminal'
+         firstlineno 125
+         lnotab 0x0201260130012801a6010e027c013e01280122021e011c05
       '__main__'
       (False,)
-   names      ('os', 'subprocess', 'json', 'argparse', 'pyngrok', 'ngrok', 'check_config', 'main', '__name__')
+   names      ('os', 'subprocess', 'json', 'argparse', 'pyngrok', 'ngrok', 'check_config', 'check_config_terminal', 'main', 'main_terminal', '__name__')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff020108010801080108010c02082706250c0118ff
+   lnotab 0x00ff020108010801080108010c020827082b062406160c0118ff
```

### Comparing `codebot-0.0.5/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.0.6/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/app.cpython-310.pyc` & `codebot-0.0.6/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/app.cpython-38.pyc` & `codebot-0.0.6/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.0.6/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.0.6/src/__pycache__/app.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x331ac764 (Mon Jul 31 02:19:31 2023 UTC)
-files sz: 12714
+moddate:  0xba17c764 (Mon Jul 31 02:08:58 2023 UTC)
+files sz: 12727
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -172,15 +172,15 @@
                354 LOAD_CONST               8 ('openai')
                356 BINARY_SUBSCR
                366 LOAD_CONST              10 ('api_base')
                368 BINARY_SUBSCR
                378 LOAD_NAME                1 (openai)
                380 STORE_ATTR              23 (api_base)
    
-    25         390 LOAD_CONST              11 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 25>)
+    25         390 LOAD_CONST              11 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 25>)
                392 MAKE_FUNCTION            0
    
     26         394 PUSH_NULL
                396 LOAD_NAME                4 (os)
                398 LOAD_ATTR               24 (listdir)
                408 LOAD_CONST              12 ('plugins')
                410 PRECALL                  1
@@ -281,15 +281,15 @@
                668 BUILD_STRING             3
                670 PRECALL                  1
                674 CALL                     1
                684 STORE_NAME              34 (module)
    
     43         686 LOAD_NAME               26 (functions)
                688 LOAD_METHOD             35 (extend)
-               710 LOAD_CONST              19 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 43>)
+               710 LOAD_CONST              19 (<code object <listcomp>, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 43>)
                712 MAKE_FUNCTION            0
    
     44         714 PUSH_NULL
                716 LOAD_NAME                9 (inspect)
                718 LOAD_ATTR               36 (getmembers)
                728 LOAD_NAME               34 (module)
                730 PRECALL                  1
@@ -342,72 +342,72 @@
    
     53     >>  918 LOAD_CONST              23 (5000)
                920 STORE_NAME              42 (max_tokens)
    
     54     >>  922 LOAD_CONST              24 (False)
                924 STORE_GLOBAL            43 (is_stop)
    
-    57         926 LOAD_CONST              25 (<code object __truncate_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 57>)
+    57         926 LOAD_CONST              25 (<code object __truncate_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 57>)
                928 MAKE_FUNCTION            0
                930 STORE_NAME              44 (__truncate_conversation)
    
-    69         932 LOAD_CONST              26 (<code object get_token_count, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 69>)
+    69         932 LOAD_CONST              26 (<code object get_token_count, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 69>)
                934 MAKE_FUNCTION            0
                936 STORE_NAME              45 (get_token_count)
    
     83         938 LOAD_CONST              27 (100)
                940 STORE_NAME              46 (MAX_ITER)
    
     86         942 LOAD_CONST              28 ('user_message')
                944 LOAD_NAME               47 (object)
                946 BUILD_TUPLE              2
-               948 LOAD_CONST              29 (<code object on_message, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 86>)
+               948 LOAD_CONST              29 (<code object on_message, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 86>)
                950 MAKE_FUNCTION            4 (annotations)
                952 STORE_NAME              48 (on_message)
    
-   209         954 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 209>)
+   209         954 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 209>)
                956 MAKE_FUNCTION            0
                958 STORE_NAME              49 (process_new_delta)
    
    243         960 LOAD_CONST              31 ('error_info')
                962 LOAD_NAME               50 (str)
                964 BUILD_TUPLE              2
-               966 LOAD_CONST              32 (<code object analyze_error, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 243>)
+               966 LOAD_CONST              32 (<code object analyze_error, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 243>)
                968 MAKE_FUNCTION            4 (annotations)
                970 STORE_NAME              51 (analyze_error)
    
    255         972 LOAD_NAME                6 (cl)
                974 LOAD_ATTR               52 (on_chat_start)
    
-   256         984 LOAD_CONST              33 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 255>)
+   256         984 LOAD_CONST              33 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 255>)
                986 MAKE_FUNCTION            0
    
    255         988 PRECALL                  0
                992 CALL                     0
    
    256        1002 STORE_NAME              53 (start_chat)
    
    293        1004 LOAD_NAME                6 (cl)
               1006 LOAD_ATTR               48 (on_message)
    
    294        1016 LOAD_CONST              28 ('user_message')
               1018 LOAD_NAME               47 (object)
               1020 BUILD_TUPLE              2
-              1022 LOAD_CONST              34 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 293>)
+              1022 LOAD_CONST              34 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 293>)
               1024 MAKE_FUNCTION            4 (annotations)
    
    293        1026 PRECALL                  0
               1030 CALL                     0
    
    294        1040 STORE_NAME              54 (run_conversation)
    
    332        1042 LOAD_NAME                6 (cl)
               1044 LOAD_ATTR               55 (on_stop)
    
-   333        1054 LOAD_CONST              35 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py", line 332>)
+   333        1054 LOAD_CONST              35 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py", line 332>)
               1056 MAKE_FUNCTION            0
    
    332        1058 PRECALL                  0
               1062 CALL                     0
    
    333        1072 STORE_NAME              56 (stop_chat)
               1074 LOAD_CONST               1 (None)
@@ -484,15 +484,15 @@
          consts
             'plugins'
             '__pycache__'
          names      ('os', 'path', 'isdir', 'join')
          varnames   ('.0', 'd')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       '<listcomp>'
          firstlineno 25
          lnotab 0x0801020178fe02020cff0201
       'plugins'
       'plugins/'
       '/config.json'
       'enabled'
@@ -530,15 +530,15 @@
                       60 JUMP_BACKWARD           28 (to 6)
                  >>   62 RETURN_VALUE
          consts
          names      ('inspect', 'isfunction')
          varnames   ('.0', 'name', 'obj')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       '<listcomp>'
          firstlineno 43
          lnotab 0x08012eff020102ff
       ('functions',)
       'functions:'
       'max_tokens'
       5000
@@ -614,15 +614,15 @@
             None
             0
             1
          names      ('get_token_count', 'max_tokens', 'len', 'pop', 'insert')
          varnames   ('conversation', 'system_con')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       '__truncate_conversation'
          firstlineno 57
          lnotab 0x020110011401020156012c0202fc02052c01
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 10
@@ -718,15 +718,15 @@
             'name'
             -1
             2
          names      ('tiktoken', 'encoding_for_model', 'config_env', 'items', 'len', 'encode', 'str')
          varnames   ('conversation', 'encoding', 'num_tokens', 'message', 'key', 'value')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'get_token_count'
          firstlineno 69
          lnotab 0x02014a02040108010a01320164010c010cfd02040a01
       100
       'user_message'
       code
          argcount  : 1
@@ -738,103 +738,103 @@
             01000000000000000001007403000000000000000000007c00a6010000ab
             01000000000000000001007403000000000000000000006402a6010000ab
             01000000000000000001007405000000000000000000007c00a6010000ab
             0100000000000000007d007406000000000000000000006a040000000000
             000000a00500000000000000000000000000000000000000006403a60100
             00ab0100000000000000007d017c01a00600000000000000000000000000
             0000000000000064047c0064059c02a6010000ab01000000000000000001
-            0064067d027c02740e000000000000000000006b00000000009005721674
-            0000000000000000000000900573106407640764059c027d0364007d0474
+            0064067d027c02740e000000000000000000006b00000000009005722274
+            00000000000000000000009005731c6407640764059c027d0364007d0474
             07000000000000000000006a0800000000000000006407ac08a6010000ab
             0100000000000000007d0564007d067413000000000000000000007c01a6
             010000ab0100000000000000007d070900741400000000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000007d087406000000000000000000006a040000000000000000a0
             0500000000000000000000000000000000000000006409a6010000ab0100
             000000000000007d097c0981257c0944005d227d0a7c0a640a1900000000
             000000000044005d177d0b7c08a006000000000000000000000000000000
             00000000007c0ba6010000ab01000000000000000001008c188c23740300
             000000000000000000640b7c08a6020000ab020000000000000000010074
             18000000000000000000006a0d0000000000000000a00e00000000000000
             00000000000000000000000000741e00000000000000000000640c190000
             00000000000000640d190000000000000000007c07640e640f7c086406ac
-            10a6060000ab06000000000000000044005d437d067c066a100000000000
-            0000006406190000000000000000006411190000000000000000007d0c74
-            0000000000000000000000720b640e6100740e000000000000000000007d
-            0201006e1d7423000000000000000000007c0c7c037c057c04a6040000ab
-            040000000000000000830064007b035600970386045c0300007d037d057d
-            048c446e462300742400000000000000000000240072397d0d7403000000
-            000000000000007c0da6010000ab01000000000000000001007c0264127a
-            0d00007d027427000000000000000000006a1400000000000000006412a6
-            010000ab010000000000000000830064007b035600970386040100590064
-            007d0d7e0d90018c6a64007d0d7e0d770177007803590077017c06801c74
-            27000000000000000000006a1400000000000000006413a6010000ab0100
-            00000000000000830064007b03560097038604010090018c907c04811a7c
-            04a0150000000000000000000000000000000000000000a6000000ab0000
-            00000000000000830064007b0356009703860401007c066a100000000000
-            00000064061900000000000000000064141900000000000000000064156b
-            02000000007202640053007c066a10000000000000000064061900000000
-            000000000064141900000000000000000064166b03000000007220742d00
-            0000000000000000007c066a100000000000000000640619000000000000
-            000000641419000000000000000000a6010000ab01000000000000000082
-            017c03a00500000000000000000000000000000000000000006416a60100
-            00ab010000000000000000a0050000000000000000000000000000000000
-            0000006417a6010000ab0100000000000000007d0e740300000000000000
-            0000007c03a00500000000000000000000000000000000000000006416a6
-            010000ab010000000000000000a6010000ab010000000000000000010064
-            077d0f0900742f000000000000000000006a1800000000000000007c03a0
+            10a6060000ab060000000000000000830064007b03560097038604320033
+            0064007b035600970386047d067c066a1000000000000000006406190000
+            000000000000006411190000000000000000007d0c740000000000000000
+            000000720b640e6100740e000000000000000000007d0201006e1e742300
+            0000000000000000007c0c7c037c057c04a6040000ab0400000000000000
+            00830064007b035600970386045c0300007d037d057d048c4936006e4623
+            00742400000000000000000000240072397d0d7403000000000000000000
+            007c0da6010000ab01000000000000000001007c0264127a0d00007d0274
+            27000000000000000000006a1400000000000000006412a6010000ab0100
+            00000000000000830064007b035600970386040100590064007d0d7e0d90
+            018c7664007d0d7e0d770177007803590077017c06801c74270000000000
+            00000000006a1400000000000000006413a6010000ab0100000000000000
+            00830064007b03560097038604010090018c9c7c04811a7c04a015000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            00830064007b0356009703860401007c066a100000000000000000640619
+            00000000000000000064141900000000000000000064156b020000000072
+            02640053007c066a10000000000000000064061900000000000000000064
+            141900000000000000000064166b03000000007220742d00000000000000
+            0000007c066a100000000000000000640619000000000000000000641419
+            000000000000000000a6010000ab01000000000000000082017c03a00500
+            000000000000000000000000000000000000006416a6010000ab01000000
+            0000000000a00500000000000000000000000000000000000000006417a6
+            010000ab0100000000000000007d0e7403000000000000000000007c03a0
             0500000000000000000000000000000000000000006416a6010000ab0100
-            00000000000000a005000000000000000000000000000000000000000064
-            18a6010000ab010000000000000000a6010000ab0100000000000000007d
-            106ea52300010009007433000000000000000000006a1a00000000000000
-            007c03a00500000000000000000000000000000000000000006416a60100
-            00ab010000000000000000a0050000000000000000000000000000000000
-            0000006418a6010000ab010000000000000000a6010000ab010000000000
-            0000007d106e62230001007c0e64196b020000000073067c0e641a6b0200
-            000000724f7c0e64196b02000000007202641a7d0e641b7c03a005000000
-            00000000000000000000000000000000006416a6010000ab010000000000
-            000000a00500000000000000000000000000000000000000006418a60100
-            00ab01000000000000000069017d10742f000000000000000000006a1b00
-            000000000000007c10a6010000ab0100000000000000007c036416190000
-            0000000000000064183c00000059006e0378035900770159006e03780359
-            0077010900741400000000000000000000a01c0000000000000000000000
-            0000000000000000007c0e7c10a6020000ab020000000000000000830064
-            007b035600970386047d0f6e232300742400000000000000000000240072
-            167d0d7403000000000000000000007c0da6010000ab0100000000000000
-            0001007c0d820164007d0d7e0d7701770078035900770174030000000000
+            00000000000000a6010000ab010000000000000000010064077d0f090074
+            2f000000000000000000006a1800000000000000007c03a0050000000000
+            0000000000000000000000000000006416a6010000ab0100000000000000
+            00a00500000000000000000000000000000000000000006418a6010000ab
+            010000000000000000a6010000ab0100000000000000007d106ea5230001
+            0009007433000000000000000000006a1a00000000000000007c03a00500
+            000000000000000000000000000000000000006416a6010000ab01000000
+            0000000000a00500000000000000000000000000000000000000006418a6
+            010000ab010000000000000000a6010000ab0100000000000000007d106e
+            62230001007c0e64196b020000000073067c0e641a6b0200000000724f7c
+            0e64196b02000000007202641a7d0e641b7c03a005000000000000000000
+            00000000000000000000006416a6010000ab010000000000000000a00500
+            000000000000000000000000000000000000006418a6010000ab01000000
+            000000000069017d10742f000000000000000000006a1b00000000000000
+            007c10a6010000ab0100000000000000007c036416190000000000000000
+            0064183c00000059006e0378035900770159006e03780359007701090074
+            1400000000000000000000a01c0000000000000000000000000000000000
+            0000007c0e7c10a6020000ab020000000000000000830064007b03560097
+            0386047d0f6e232300742400000000000000000000240072167d0d740300
+            0000000000000000007c0da6010000ab01000000000000000001007c0d82
+            0164007d0d7e0d7701770078035900770174030000000000000000000064
+            02a6010000ab01000000000000000001007403000000000000000000007c
+            0fa6010000ab0100000000000000000100743b000000000000000000007c
+            0fa6010000ab0100000000000000007404000000000000000000006b0300
+            000000720f7405000000000000000000007c0fa6010000ab010000000000
+            0000007d0f7c01a00600000000000000000000000000000000000000007c
+            03a6010000ab01000000000000000001007c0e641a6b020000000072b664
+            1c7c0f760072b2641d7c0f760072ae641e7c0f760072aa74030000000000
+            0000000000641fa6010000ab0100000000000000000100742f0000000000
+            00000000006a1800000000000000007c0fa6010000ab0100000000000000
+            007d0f7c0f6420190000000000000000007d117c0f64203d007c01a00600
+            0000000000000000000000000000000000000064217c0e742f0000000000
+            00000000006a1b00000000000000007c0fa6010000ab0100000000000000
+            0064229c03a6010000ab0100000000000000000100741e00000000000000
+            000000640c190000000000000000006423190000000000000000007d127c
+            01a006000000000000000000000000000000000000000064047405000000
+            000000000000007c11a6010000ab01000000000000000064247a00000064
+            257a0000007c127a00000064059c02a6010000ab01000000000000000001
+            00740300000000000000000000641fa6010000ab01000000000000000001
+            006e197c01a006000000000000000000000000000000000000000064217c
+            0e7c0f64229c03a6010000ab010000000000000000010074030000000000
             00000000006402a6010000ab010000000000000000010074030000000000
-            00000000007c0fa6010000ab0100000000000000000100743b0000000000
-            00000000007c0fa6010000ab010000000000000000740400000000000000
-            0000006b0300000000720f7405000000000000000000007c0fa6010000ab
-            0100000000000000007d0f7c01a006000000000000000000000000000000
-            00000000007c03a6010000ab01000000000000000001007c0e641a6b0200
-            00000072b6641c7c0f760072b2641d7c0f760072ae641e7c0f760072aa74
-            0300000000000000000000641fa6010000ab010000000000000000010074
-            2f000000000000000000006a1800000000000000007c0fa6010000ab0100
-            000000000000007d0f7c0f6420190000000000000000007d117c0f64203d
-            007c01a006000000000000000000000000000000000000000064217c0e74
-            2f000000000000000000006a1b00000000000000007c0fa6010000ab0100
-            0000000000000064229c03a6010000ab0100000000000000000100741e00
-            000000000000000000640c19000000000000000000642319000000000000
-            0000007d127c01a006000000000000000000000000000000000000000064
-            047405000000000000000000007c11a6010000ab01000000000000000064
-            247a00000064257a0000007c127a00000064059c02a6010000ab01000000
-            00000000000100740300000000000000000000641fa6010000ab01000000
-            000000000001006e197c01a0060000000000000000000000000000000000
-            00000064217c0e7c0f64229c03a6010000ab010000000000000000010074
-            03000000000000000000006402a6010000ab010000000000000000010074
-            03000000000000000000007c01a6010000ab010000000000000000010074
-            03000000000000000000006402a6010000ab010000000000000000010074
-            07000000000000000000006a0800000000000000007c0e74050000000000
-            00000000007c0fa6010000ab01000000000000000064266412ac27a60400
-            00ab040000000000000000a0150000000000000000000000000000000000
-            000000a6000000ab000000000000000000830064007b0356009703860401
-            007c0264127a0d00007d027c02740e000000000000000000006b00000000
-            00720e7400000000000000000000009005af0c6400530064005300640053
-            0064005300
+            00000000007c01a6010000ab010000000000000000010074030000000000
+            00000000006402a6010000ab010000000000000000010074070000000000
+            00000000006a0800000000000000007c0e7405000000000000000000007c
+            0fa6010000ab01000000000000000064266412ac27a6040000ab04000000
+            0000000000a0150000000000000000000000000000000000000000a60000
+            00ab000000000000000000830064007b0356009703860401007c0264127a
+            0d00007d027c02740e000000000000000000006b0000000000720e740000
+            0000000000000000009005af1864005300640053006400530064005300
           86           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
           88           6 LOAD_CONST               1 (False)
                        8 STORE_GLOBAL             0 (is_stop)
          
@@ -883,18 +883,18 @@
           95         240 LOAD_CONST               6 (0)
                      242 STORE_FAST               2 (cur_iter)
          
           96     >>  244 LOAD_FAST                2 (cur_iter)
                      246 LOAD_GLOBAL             14 (MAX_ITER)
                      258 COMPARE_OP               0 (<)
                      264 EXTENDED_ARG             5
-                     266 POP_JUMP_FORWARD_IF_FALSE  1302 (to 2872)
+                     266 POP_JUMP_FORWARD_IF_FALSE  1314 (to 2896)
                      268 LOAD_GLOBAL              0 (is_stop)
                      280 EXTENDED_ARG             5
-                     282 POP_JUMP_FORWARD_IF_TRUE  1296 (to 2876)
+                     282 POP_JUMP_FORWARD_IF_TRUE  1308 (to 2900)
          
           98     >>  284 LOAD_CONST               7 ('')
                      286 LOAD_CONST               7 ('')
                      288 LOAD_CONST               5 (('role', 'content'))
                      290 BUILD_CONST_KEY_MAP      2
                      292 STORE_FAST               3 (openai_message)
          
@@ -964,15 +964,15 @@
                      580 LOAD_FAST                8 (functions)
                      582 PRECALL                  2
                      586 CALL                     2
                      596 POP_TOP
          
          111         598 LOAD_GLOBAL             24 (openai)
                      610 LOAD_ATTR               13 (ChatCompletion)
-                     620 LOAD_METHOD             14 (create)
+                     620 LOAD_METHOD             14 (acreate)
          
          112         642 LOAD_GLOBAL             30 (config_env)
                      654 LOAD_CONST              12 ('openai')
                      656 BINARY_SUBSCR
                      666 LOAD_CONST              13 ('model')
                      668 BINARY_SUBSCR
          
@@ -985,563 +985,578 @@
          116         684 LOAD_FAST                8 (functions)
          
          117         686 LOAD_CONST               6 (0)
          
          111         688 KW_NAMES                16
                      690 PRECALL                  6
                      694 CALL                     6
-                     704 GET_ITER
-                 >>  706 FOR_ITER                67 (to 842)
-                     708 STORE_FAST               6 (stream_resp)
-         
-         118         710 LOAD_FAST                6 (stream_resp)
-                     712 LOAD_ATTR               16 (choices)
-                     722 LOAD_CONST               6 (0)
-                     724 BINARY_SUBSCR
-                     734 LOAD_CONST              17 ('delta')
-                     736 BINARY_SUBSCR
-                     746 STORE_FAST              12 (new_delta)
-         
-         119         748 LOAD_GLOBAL              0 (is_stop)
-                     760 POP_JUMP_FORWARD_IF_FALSE    11 (to 784)
-         
-         120         762 LOAD_CONST              14 (True)
-                     764 STORE_GLOBAL             0 (is_stop)
-         
-         121         766 LOAD_GLOBAL             14 (MAX_ITER)
-                     778 STORE_FAST               2 (cur_iter)
-         
-         122         780 POP_TOP
-                     782 JUMP_FORWARD            29 (to 842)
-         
-         123     >>  784 LOAD_GLOBAL             35 (NULL + process_new_delta)
-         
-         124         796 LOAD_FAST               12 (new_delta)
-                     798 LOAD_FAST                3 (openai_message)
-                     800 LOAD_FAST                5 (content_ui_message)
-                     802 LOAD_FAST                4 (function_ui_message)
-         
-         123         804 PRECALL                  4
-                     808 CALL                     4
-                     818 GET_AWAITABLE            0
-                     820 LOAD_CONST               0 (None)
-                 >>  822 SEND                     3 (to 830)
-                     824 YIELD_VALUE
-                     826 RESUME                   3
-                     828 JUMP_BACKWARD_NO_INTERRUPT     4 (to 822)
-                 >>  830 UNPACK_SEQUENCE          3
-                     834 STORE_FAST               3 (openai_message)
-                     836 STORE_FAST               5 (content_ui_message)
-                     838 STORE_FAST               4 (function_ui_message)
-                     840 JUMP_BACKWARD           68 (to 706)
-                 >>  842 JUMP_FORWARD            70 (to 984)
-                 >>  844 PUSH_EXC_INFO
-         
-         125         846 LOAD_GLOBAL             36 (Exception)
-                     858 CHECK_EXC_MATCH
-                     860 POP_JUMP_FORWARD_IF_FALSE    57 (to 976)
-                     862 STORE_FAST              13 (e)
-         
-         126         864 LOAD_GLOBAL              3 (NULL + print)
-                     876 LOAD_FAST               13 (e)
-                     878 PRECALL                  1
-                     882 CALL                     1
-                     892 POP_TOP
-         
-         127         894 LOAD_FAST                2 (cur_iter)
-                     896 LOAD_CONST              18 (1)
-                     898 BINARY_OP               13 (+=)
-                     902 STORE_FAST               2 (cur_iter)
-         
-         128         904 LOAD_GLOBAL             39 (NULL + asyncio)
-                     916 LOAD_ATTR               20 (sleep)
-                     926 LOAD_CONST              18 (1)
-                     928 PRECALL                  1
-                     932 CALL                     1
-                     942 GET_AWAITABLE            0
-                     944 LOAD_CONST               0 (None)
-                 >>  946 SEND                     3 (to 954)
-                     948 YIELD_VALUE
-                     950 RESUME                   3
-                     952 JUMP_BACKWARD_NO_INTERRUPT     4 (to 946)
-                 >>  954 POP_TOP
-         
-         129         956 POP_EXCEPT
-                     958 LOAD_CONST               0 (None)
-                     960 STORE_FAST              13 (e)
-                     962 DELETE_FAST             13 (e)
-                     964 EXTENDED_ARG             1
-                     966 JUMP_BACKWARD          362 (to 244)
-                 >>  968 LOAD_CONST               0 (None)
-                     970 STORE_FAST              13 (e)
-                     972 DELETE_FAST             13 (e)
-                     974 RERAISE                  1
-         
-         125     >>  976 RERAISE                  0
-                 >>  978 COPY                     3
-                     980 POP_EXCEPT
-                     982 RERAISE                  1
-         
-         131     >>  984 LOAD_FAST                6 (stream_resp)
-                     986 POP_JUMP_FORWARD_IF_NOT_NONE    28 (to 1044)
-         
-         132         988 LOAD_GLOBAL             39 (NULL + asyncio)
-                    1000 LOAD_ATTR               20 (sleep)
-                    1010 LOAD_CONST              19 (2)
-                    1012 PRECALL                  1
-                    1016 CALL                     1
-                    1026 GET_AWAITABLE            0
-                    1028 LOAD_CONST               0 (None)
-                 >> 1030 SEND                     3 (to 1038)
-                    1032 YIELD_VALUE
-                    1034 RESUME                   3
-                    1036 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1030)
-                 >> 1038 POP_TOP
-         
-         133        1040 EXTENDED_ARG             1
-                    1042 JUMP_BACKWARD          400 (to 244)
-         
-         135     >> 1044 LOAD_FAST                4 (function_ui_message)
-                    1046 POP_JUMP_FORWARD_IF_NONE    26 (to 1100)
-         
-         136        1048 LOAD_FAST                4 (function_ui_message)
-                    1050 LOAD_METHOD             21 (send)
-                    1072 PRECALL                  0
-                    1076 CALL                     0
-                    1086 GET_AWAITABLE            0
-                    1088 LOAD_CONST               0 (None)
-                 >> 1090 SEND                     3 (to 1098)
-                    1092 YIELD_VALUE
-                    1094 RESUME                   3
-                    1096 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1090)
-                 >> 1098 POP_TOP
-         
-         138     >> 1100 LOAD_FAST                6 (stream_resp)
-                    1102 LOAD_ATTR               16 (choices)
-                    1112 LOAD_CONST               6 (0)
-                    1114 BINARY_SUBSCR
-                    1124 LOAD_CONST              20 ('finish_reason')
-                    1126 BINARY_SUBSCR
-                    1136 LOAD_CONST              21 ('stop')
-                    1138 COMPARE_OP               2 (==)
-                    1144 POP_JUMP_FORWARD_IF_FALSE     2 (to 1150)
-         
-         139        1146 LOAD_CONST               0 (None)
-                    1148 RETURN_VALUE
-         
-         140     >> 1150 LOAD_FAST                6 (stream_resp)
-                    1152 LOAD_ATTR               16 (choices)
-                    1162 LOAD_CONST               6 (0)
-                    1164 BINARY_SUBSCR
-                    1174 LOAD_CONST              20 ('finish_reason')
-                    1176 BINARY_SUBSCR
-                    1186 LOAD_CONST              22 ('function_call')
-                    1188 COMPARE_OP               3 (!=)
-                    1194 POP_JUMP_FORWARD_IF_FALSE    32 (to 1260)
-         
-         141        1196 LOAD_GLOBAL             45 (NULL + ValueError)
-                    1208 LOAD_FAST                6 (stream_resp)
-                    1210 LOAD_ATTR               16 (choices)
-                    1220 LOAD_CONST               6 (0)
-                    1222 BINARY_SUBSCR
-                    1232 LOAD_CONST              20 ('finish_reason')
-                    1234 BINARY_SUBSCR
-                    1244 PRECALL                  1
-                    1248 CALL                     1
-                    1258 RAISE_VARARGS            1
-         
-         143     >> 1260 LOAD_FAST                3 (openai_message)
-                    1262 LOAD_METHOD              5 (get)
-                    1284 LOAD_CONST              22 ('function_call')
-                    1286 PRECALL                  1
-                    1290 CALL                     1
-                    1300 LOAD_METHOD              5 (get)
-                    1322 LOAD_CONST              23 ('name')
-                    1324 PRECALL                  1
-                    1328 CALL                     1
-                    1338 STORE_FAST              14 (function_name)
-         
-         144        1340 LOAD_GLOBAL              3 (NULL + print)
-                    1352 LOAD_FAST                3 (openai_message)
-                    1354 LOAD_METHOD              5 (get)
-                    1376 LOAD_CONST              22 ('function_call')
-                    1378 PRECALL                  1
-                    1382 CALL                     1
-                    1392 PRECALL                  1
-                    1396 CALL                     1
-                    1406 POP_TOP
-         
-         145        1408 LOAD_CONST               7 ('')
-                    1410 STORE_FAST              15 (function_response)
-         
-         146        1412 NOP
-         
-         147        1414 LOAD_GLOBAL             47 (NULL + json)
-                    1426 LOAD_ATTR               24 (loads)
-         
-         148        1436 LOAD_FAST                3 (openai_message)
-                    1438 LOAD_METHOD              5 (get)
-                    1460 LOAD_CONST              22 ('function_call')
-                    1462 PRECALL                  1
-                    1466 CALL                     1
-                    1476 LOAD_METHOD              5 (get)
-                    1498 LOAD_CONST              24 ('arguments')
-                    1500 PRECALL                  1
-                    1504 CALL                     1
-         
-         147        1514 PRECALL                  1
-                    1518 CALL                     1
-                    1528 STORE_FAST              16 (arguments)
-                    1530 JUMP_FORWARD           165 (to 1862)
-                 >> 1532 PUSH_EXC_INFO
-         
-         149        1534 POP_TOP
-         
-         150        1536 NOP
-         
-         151        1538 LOAD_GLOBAL             51 (NULL + ast)
-                    1550 LOAD_ATTR               26 (literal_eval)
-         
-         152        1560 LOAD_FAST                3 (openai_message)
-                    1562 LOAD_METHOD              5 (get)
-                    1584 LOAD_CONST              22 ('function_call')
-                    1586 PRECALL                  1
-                    1590 CALL                     1
-                    1600 LOAD_METHOD              5 (get)
-                    1622 LOAD_CONST              24 ('arguments')
-                    1624 PRECALL                  1
-                    1628 CALL                     1
-         
-         151        1638 PRECALL                  1
-                    1642 CALL                     1
-                    1652 STORE_FAST              16 (arguments)
-                    1654 JUMP_FORWARD            98 (to 1852)
-                 >> 1656 PUSH_EXC_INFO
-         
-         153        1658 POP_TOP
-         
-         154        1660 LOAD_FAST               14 (function_name)
-                    1662 LOAD_CONST              25 ('python')
-                    1664 COMPARE_OP               2 (==)
-                    1670 POP_JUMP_FORWARD_IF_TRUE     6 (to 1684)
-                    1672 LOAD_FAST               14 (function_name)
-                    1674 LOAD_CONST              26 ('python_exec')
-                    1676 COMPARE_OP               2 (==)
-                    1682 POP_JUMP_FORWARD_IF_FALSE    79 (to 1842)
+                     704 GET_AWAITABLE            0
+                     706 LOAD_CONST               0 (None)
+                 >>  708 SEND                     3 (to 716)
+                     710 YIELD_VALUE
+                     712 RESUME                   3
+                     714 JUMP_BACKWARD_NO_INTERRUPT     4 (to 708)
+                 >>  716 GET_AITER
+                 >>  718 GET_ANEXT
+                     720 LOAD_CONST               0 (None)
+                 >>  722 SEND                     3 (to 730)
+                     724 YIELD_VALUE
+                     726 RESUME                   3
+                     728 JUMP_BACKWARD_NO_INTERRUPT     4 (to 722)
+                 >>  730 STORE_FAST               6 (stream_resp)
+         
+         118         732 LOAD_FAST                6 (stream_resp)
+                     734 LOAD_ATTR               16 (choices)
+                     744 LOAD_CONST               6 (0)
+                     746 BINARY_SUBSCR
+                     756 LOAD_CONST              17 ('delta')
+                     758 BINARY_SUBSCR
+                     768 STORE_FAST              12 (new_delta)
+         
+         119         770 LOAD_GLOBAL              0 (is_stop)
+                     782 POP_JUMP_FORWARD_IF_FALSE    11 (to 806)
+         
+         120         784 LOAD_CONST              14 (True)
+                     786 STORE_GLOBAL             0 (is_stop)
+         
+         121         788 LOAD_GLOBAL             14 (MAX_ITER)
+                     800 STORE_FAST               2 (cur_iter)
+         
+         122         802 POP_TOP
+                     804 JUMP_FORWARD            30 (to 866)
+         
+         123     >>  806 LOAD_GLOBAL             35 (NULL + process_new_delta)
+         
+         124         818 LOAD_FAST               12 (new_delta)
+                     820 LOAD_FAST                3 (openai_message)
+                     822 LOAD_FAST                5 (content_ui_message)
+                     824 LOAD_FAST                4 (function_ui_message)
+         
+         123         826 PRECALL                  4
+                     830 CALL                     4
+                     840 GET_AWAITABLE            0
+                     842 LOAD_CONST               0 (None)
+                 >>  844 SEND                     3 (to 852)
+                     846 YIELD_VALUE
+                     848 RESUME                   3
+                     850 JUMP_BACKWARD_NO_INTERRUPT     4 (to 844)
+                 >>  852 UNPACK_SEQUENCE          3
+                     856 STORE_FAST               3 (openai_message)
+                     858 STORE_FAST               5 (content_ui_message)
+                     860 STORE_FAST               4 (function_ui_message)
+                     862 JUMP_BACKWARD           73 (to 718)
+         
+         111     >>  864 END_ASYNC_FOR
+                 >>  866 JUMP_FORWARD            70 (to 1008)
+                 >>  868 PUSH_EXC_INFO
+         
+         125         870 LOAD_GLOBAL             36 (Exception)
+                     882 CHECK_EXC_MATCH
+                     884 POP_JUMP_FORWARD_IF_FALSE    57 (to 1000)
+                     886 STORE_FAST              13 (e)
+         
+         126         888 LOAD_GLOBAL              3 (NULL + print)
+                     900 LOAD_FAST               13 (e)
+                     902 PRECALL                  1
+                     906 CALL                     1
+                     916 POP_TOP
+         
+         127         918 LOAD_FAST                2 (cur_iter)
+                     920 LOAD_CONST              18 (1)
+                     922 BINARY_OP               13 (+=)
+                     926 STORE_FAST               2 (cur_iter)
+         
+         128         928 LOAD_GLOBAL             39 (NULL + asyncio)
+                     940 LOAD_ATTR               20 (sleep)
+                     950 LOAD_CONST              18 (1)
+                     952 PRECALL                  1
+                     956 CALL                     1
+                     966 GET_AWAITABLE            0
+                     968 LOAD_CONST               0 (None)
+                 >>  970 SEND                     3 (to 978)
+                     972 YIELD_VALUE
+                     974 RESUME                   3
+                     976 JUMP_BACKWARD_NO_INTERRUPT     4 (to 970)
+                 >>  978 POP_TOP
+         
+         129         980 POP_EXCEPT
+                     982 LOAD_CONST               0 (None)
+                     984 STORE_FAST              13 (e)
+                     986 DELETE_FAST             13 (e)
+                     988 EXTENDED_ARG             1
+                     990 JUMP_BACKWARD          374 (to 244)
+                 >>  992 LOAD_CONST               0 (None)
+                     994 STORE_FAST              13 (e)
+                     996 DELETE_FAST             13 (e)
+                     998 RERAISE                  1
+         
+         125     >> 1000 RERAISE                  0
+                 >> 1002 COPY                     3
+                    1004 POP_EXCEPT
+                    1006 RERAISE                  1
+         
+         131     >> 1008 LOAD_FAST                6 (stream_resp)
+                    1010 POP_JUMP_FORWARD_IF_NOT_NONE    28 (to 1068)
+         
+         132        1012 LOAD_GLOBAL             39 (NULL + asyncio)
+                    1024 LOAD_ATTR               20 (sleep)
+                    1034 LOAD_CONST              19 (2)
+                    1036 PRECALL                  1
+                    1040 CALL                     1
+                    1050 GET_AWAITABLE            0
+                    1052 LOAD_CONST               0 (None)
+                 >> 1054 SEND                     3 (to 1062)
+                    1056 YIELD_VALUE
+                    1058 RESUME                   3
+                    1060 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1054)
+                 >> 1062 POP_TOP
+         
+         133        1064 EXTENDED_ARG             1
+                    1066 JUMP_BACKWARD          412 (to 244)
+         
+         135     >> 1068 LOAD_FAST                4 (function_ui_message)
+                    1070 POP_JUMP_FORWARD_IF_NONE    26 (to 1124)
+         
+         136        1072 LOAD_FAST                4 (function_ui_message)
+                    1074 LOAD_METHOD             21 (send)
+                    1096 PRECALL                  0
+                    1100 CALL                     0
+                    1110 GET_AWAITABLE            0
+                    1112 LOAD_CONST               0 (None)
+                 >> 1114 SEND                     3 (to 1122)
+                    1116 YIELD_VALUE
+                    1118 RESUME                   3
+                    1120 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1114)
+                 >> 1122 POP_TOP
+         
+         138     >> 1124 LOAD_FAST                6 (stream_resp)
+                    1126 LOAD_ATTR               16 (choices)
+                    1136 LOAD_CONST               6 (0)
+                    1138 BINARY_SUBSCR
+                    1148 LOAD_CONST              20 ('finish_reason')
+                    1150 BINARY_SUBSCR
+                    1160 LOAD_CONST              21 ('stop')
+                    1162 COMPARE_OP               2 (==)
+                    1168 POP_JUMP_FORWARD_IF_FALSE     2 (to 1174)
+         
+         139        1170 LOAD_CONST               0 (None)
+                    1172 RETURN_VALUE
+         
+         140     >> 1174 LOAD_FAST                6 (stream_resp)
+                    1176 LOAD_ATTR               16 (choices)
+                    1186 LOAD_CONST               6 (0)
+                    1188 BINARY_SUBSCR
+                    1198 LOAD_CONST              20 ('finish_reason')
+                    1200 BINARY_SUBSCR
+                    1210 LOAD_CONST              22 ('function_call')
+                    1212 COMPARE_OP               3 (!=)
+                    1218 POP_JUMP_FORWARD_IF_FALSE    32 (to 1284)
+         
+         141        1220 LOAD_GLOBAL             45 (NULL + ValueError)
+                    1232 LOAD_FAST                6 (stream_resp)
+                    1234 LOAD_ATTR               16 (choices)
+                    1244 LOAD_CONST               6 (0)
+                    1246 BINARY_SUBSCR
+                    1256 LOAD_CONST              20 ('finish_reason')
+                    1258 BINARY_SUBSCR
+                    1268 PRECALL                  1
+                    1272 CALL                     1
+                    1282 RAISE_VARARGS            1
+         
+         143     >> 1284 LOAD_FAST                3 (openai_message)
+                    1286 LOAD_METHOD              5 (get)
+                    1308 LOAD_CONST              22 ('function_call')
+                    1310 PRECALL                  1
+                    1314 CALL                     1
+                    1324 LOAD_METHOD              5 (get)
+                    1346 LOAD_CONST              23 ('name')
+                    1348 PRECALL                  1
+                    1352 CALL                     1
+                    1362 STORE_FAST              14 (function_name)
+         
+         144        1364 LOAD_GLOBAL              3 (NULL + print)
+                    1376 LOAD_FAST                3 (openai_message)
+                    1378 LOAD_METHOD              5 (get)
+                    1400 LOAD_CONST              22 ('function_call')
+                    1402 PRECALL                  1
+                    1406 CALL                     1
+                    1416 PRECALL                  1
+                    1420 CALL                     1
+                    1430 POP_TOP
+         
+         145        1432 LOAD_CONST               7 ('')
+                    1434 STORE_FAST              15 (function_response)
+         
+         146        1436 NOP
+         
+         147        1438 LOAD_GLOBAL             47 (NULL + json)
+                    1450 LOAD_ATTR               24 (loads)
+         
+         148        1460 LOAD_FAST                3 (openai_message)
+                    1462 LOAD_METHOD              5 (get)
+                    1484 LOAD_CONST              22 ('function_call')
+                    1486 PRECALL                  1
+                    1490 CALL                     1
+                    1500 LOAD_METHOD              5 (get)
+                    1522 LOAD_CONST              24 ('arguments')
+                    1524 PRECALL                  1
+                    1528 CALL                     1
+         
+         147        1538 PRECALL                  1
+                    1542 CALL                     1
+                    1552 STORE_FAST              16 (arguments)
+                    1554 JUMP_FORWARD           165 (to 1886)
+                 >> 1556 PUSH_EXC_INFO
+         
+         149        1558 POP_TOP
+         
+         150        1560 NOP
+         
+         151        1562 LOAD_GLOBAL             51 (NULL + ast)
+                    1574 LOAD_ATTR               26 (literal_eval)
+         
+         152        1584 LOAD_FAST                3 (openai_message)
+                    1586 LOAD_METHOD              5 (get)
+                    1608 LOAD_CONST              22 ('function_call')
+                    1610 PRECALL                  1
+                    1614 CALL                     1
+                    1624 LOAD_METHOD              5 (get)
+                    1646 LOAD_CONST              24 ('arguments')
+                    1648 PRECALL                  1
+                    1652 CALL                     1
+         
+         151        1662 PRECALL                  1
+                    1666 CALL                     1
+                    1676 STORE_FAST              16 (arguments)
+                    1678 JUMP_FORWARD            98 (to 1876)
+                 >> 1680 PUSH_EXC_INFO
+         
+         153        1682 POP_TOP
          
-         155     >> 1684 LOAD_FAST               14 (function_name)
+         154        1684 LOAD_FAST               14 (function_name)
                     1686 LOAD_CONST              25 ('python')
                     1688 COMPARE_OP               2 (==)
-                    1694 POP_JUMP_FORWARD_IF_FALSE     2 (to 1700)
-         
-         156        1696 LOAD_CONST              26 ('python_exec')
-                    1698 STORE_FAST              14 (function_name)
-         
-         157     >> 1700 LOAD_CONST              27 ('code')
-                    1702 LOAD_FAST                3 (openai_message)
-                    1704 LOAD_METHOD              5 (get)
-                    1726 LOAD_CONST              22 ('function_call')
-                    1728 PRECALL                  1
-                    1732 CALL                     1
-                    1742 LOAD_METHOD              5 (get)
-                    1764 LOAD_CONST              24 ('arguments')
-                    1766 PRECALL                  1
-                    1770 CALL                     1
-                    1780 BUILD_MAP                1
-                    1782 STORE_FAST              16 (arguments)
-         
-         158        1784 LOAD_GLOBAL             47 (NULL + json)
-                    1796 LOAD_ATTR               27 (dumps)
-                    1806 LOAD_FAST               16 (arguments)
-                    1808 PRECALL                  1
-                    1812 CALL                     1
-                    1822 LOAD_FAST                3 (openai_message)
-                    1824 LOAD_CONST              22 ('function_call')
-                    1826 BINARY_SUBSCR
-                    1836 LOAD_CONST              24 ('arguments')
-                    1838 STORE_SUBSCR
-                 >> 1842 POP_EXCEPT
-                    1844 JUMP_FORWARD             3 (to 1852)
-                 >> 1846 COPY                     3
-                    1848 POP_EXCEPT
-                    1850 RERAISE                  1
-                 >> 1852 POP_EXCEPT
-                    1854 JUMP_FORWARD             3 (to 1862)
-                 >> 1856 COPY                     3
-                    1858 POP_EXCEPT
-                    1860 RERAISE                  1
-         
-         159     >> 1862 NOP
-         
-         160        1864 LOAD_GLOBAL             20 (function_manager)
-                    1876 LOAD_METHOD             28 (call_function)
-         
-         161        1898 LOAD_FAST               14 (function_name)
-                    1900 LOAD_FAST               16 (arguments)
-         
-         160        1902 PRECALL                  2
-                    1906 CALL                     2
-                    1916 GET_AWAITABLE            0
-                    1918 LOAD_CONST               0 (None)
-                 >> 1920 SEND                     3 (to 1928)
-                    1922 YIELD_VALUE
-                    1924 RESUME                   3
-                    1926 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1920)
-                 >> 1928 STORE_FAST              15 (function_response)
-                    1930 JUMP_FORWARD            35 (to 2002)
-                 >> 1932 PUSH_EXC_INFO
-         
-         162        1934 LOAD_GLOBAL             36 (Exception)
-                    1946 CHECK_EXC_MATCH
-                    1948 POP_JUMP_FORWARD_IF_FALSE    22 (to 1994)
-                    1950 STORE_FAST              13 (e)
-         
-         163        1952 LOAD_GLOBAL              3 (NULL + print)
-                    1964 LOAD_FAST               13 (e)
-                    1966 PRECALL                  1
-                    1970 CALL                     1
-                    1980 POP_TOP
-         
-         164        1982 LOAD_FAST               13 (e)
-                    1984 RAISE_VARARGS            1
-                 >> 1986 LOAD_CONST               0 (None)
-                    1988 STORE_FAST              13 (e)
-                    1990 DELETE_FAST             13 (e)
-                    1992 RERAISE                  1
-         
-         162     >> 1994 RERAISE                  0
-                 >> 1996 COPY                     3
-                    1998 POP_EXCEPT
-                    2000 RERAISE                  1
-         
-         165     >> 2002 LOAD_GLOBAL              3 (NULL + print)
-                    2014 LOAD_CONST               2 ('==================================')
-                    2016 PRECALL                  1
-                    2020 CALL                     1
-                    2030 POP_TOP
-         
-         166        2032 LOAD_GLOBAL              3 (NULL + print)
-                    2044 LOAD_FAST               15 (function_response)
-                    2046 PRECALL                  1
-                    2050 CALL                     1
-                    2060 POP_TOP
-         
-         167        2062 LOAD_GLOBAL             59 (NULL + type)
-                    2074 LOAD_FAST               15 (function_response)
-                    2076 PRECALL                  1
-                    2080 CALL                     1
-                    2090 LOAD_GLOBAL              4 (str)
-                    2102 COMPARE_OP               3 (!=)
-                    2108 POP_JUMP_FORWARD_IF_FALSE    15 (to 2140)
-         
-         168        2110 LOAD_GLOBAL              5 (NULL + str)
-                    2122 LOAD_FAST               15 (function_response)
-                    2124 PRECALL                  1
-                    2128 CALL                     1
-                    2138 STORE_FAST              15 (function_response)
-         
-         170     >> 2140 LOAD_FAST                1 (message_history)
-                    2142 LOAD_METHOD              6 (append)
-                    2164 LOAD_FAST                3 (openai_message)
-                    2166 PRECALL                  1
-                    2170 CALL                     1
-                    2180 POP_TOP
-         
-         172        2182 LOAD_FAST               14 (function_name)
-                    2184 LOAD_CONST              26 ('python_exec')
-                    2186 COMPARE_OP               2 (==)
-                    2192 POP_JUMP_FORWARD_IF_FALSE   182 (to 2558)
-                    2194 LOAD_CONST              28 ('status')
-                    2196 LOAD_FAST               15 (function_response)
-                    2198 CONTAINS_OP              0
-                    2200 POP_JUMP_FORWARD_IF_FALSE   178 (to 2558)
-                    2202 LOAD_CONST              29 ('error_info')
-                    2204 LOAD_FAST               15 (function_response)
-                    2206 CONTAINS_OP              0
-                    2208 POP_JUMP_FORWARD_IF_FALSE   174 (to 2558)
-                    2210 LOAD_CONST              30 ('error')
-                    2212 LOAD_FAST               15 (function_response)
-                    2214 CONTAINS_OP              0
-                    2216 POP_JUMP_FORWARD_IF_FALSE   170 (to 2558)
-         
-         174        2218 LOAD_GLOBAL              3 (NULL + print)
-                    2230 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
-                    2232 PRECALL                  1
-                    2236 CALL                     1
-                    2246 POP_TOP
-         
-         175        2248 LOAD_GLOBAL             47 (NULL + json)
-                    2260 LOAD_ATTR               24 (loads)
-                    2270 LOAD_FAST               15 (function_response)
-                    2272 PRECALL                  1
-                    2276 CALL                     1
-                    2286 STORE_FAST              15 (function_response)
-         
-         176        2288 LOAD_FAST               15 (function_response)
-                    2290 LOAD_CONST              32 ('description')
-                    2292 BINARY_SUBSCR
-                    2302 STORE_FAST              17 (description)
-         
-         177        2304 LOAD_FAST               15 (function_response)
-                    2306 LOAD_CONST              32 ('description')
-                    2308 DELETE_SUBSCR
-         
-         178        2310 LOAD_FAST                1 (message_history)
-                    2312 LOAD_METHOD              6 (append)
-         
-         179        2334 LOAD_CONST              33 ('function')
-         
-         180        2336 LOAD_FAST               14 (function_name)
-         
-         181        2338 LOAD_GLOBAL             47 (NULL + json)
-                    2350 LOAD_ATTR               27 (dumps)
-                    2360 LOAD_FAST               15 (function_response)
-                    2362 PRECALL                  1
-                    2366 CALL                     1
-         
-         178        2376 LOAD_CONST              34 (('role', 'name', 'content'))
-                    2378 BUILD_CONST_KEY_MAP      3
-                    2380 PRECALL                  1
-                    2384 CALL                     1
-                    2394 POP_TOP
-         
-         183        2396 LOAD_GLOBAL             30 (config_env)
-                    2408 LOAD_CONST              12 ('openai')
-                    2410 BINARY_SUBSCR
-                    2420 LOAD_CONST              35 ('language')
-                    2422 BINARY_SUBSCR
-                    2432 STORE_FAST              18 (language)
-         
-         184        2434 LOAD_FAST                1 (message_history)
-                    2436 LOAD_METHOD              6 (append)
-         
-         185        2458 LOAD_CONST               4 ('user')
-         
-         186        2460 LOAD_GLOBAL              5 (NULL + str)
-                    2472 LOAD_FAST               17 (description)
-                    2474 PRECALL                  1
-                    2478 CALL                     1
-                    2488 LOAD_CONST              36 ('\n\n')
-                    2490 BINARY_OP                0 (+)
-                    2494 LOAD_CONST              37 ('Please answer me in ')
-                    2496 BINARY_OP                0 (+)
-                    2500 LOAD_FAST               18 (language)
-                    2502 BINARY_OP                0 (+)
-         
-         184        2506 LOAD_CONST               5 (('role', 'content'))
-                    2508 BUILD_CONST_KEY_MAP      2
-                    2510 PRECALL                  1
-                    2514 CALL                     1
-                    2524 POP_TOP
-         
-         188        2526 LOAD_GLOBAL              3 (NULL + print)
-                    2538 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
-                    2540 PRECALL                  1
-                    2544 CALL                     1
-                    2554 POP_TOP
-                    2556 JUMP_FORWARD            25 (to 2608)
-         
-         190     >> 2558 LOAD_FAST                1 (message_history)
-                    2560 LOAD_METHOD              6 (append)
-         
-         191        2582 LOAD_CONST              33 ('function')
-         
-         192        2584 LOAD_FAST               14 (function_name)
-         
-         193        2586 LOAD_FAST               15 (function_response)
-         
-         190        2588 LOAD_CONST              34 (('role', 'name', 'content'))
-                    2590 BUILD_CONST_KEY_MAP      3
-                    2592 PRECALL                  1
-                    2596 CALL                     1
-                    2606 POP_TOP
-         
-         196     >> 2608 LOAD_GLOBAL              3 (NULL + print)
-                    2620 LOAD_CONST               2 ('==================================')
-                    2622 PRECALL                  1
-                    2626 CALL                     1
-                    2636 POP_TOP
-         
-         197        2638 LOAD_GLOBAL              3 (NULL + print)
-                    2650 LOAD_FAST                1 (message_history)
-                    2652 PRECALL                  1
-                    2656 CALL                     1
-                    2666 POP_TOP
-         
-         198        2668 LOAD_GLOBAL              3 (NULL + print)
-                    2680 LOAD_CONST               2 ('==================================')
-                    2682 PRECALL                  1
-                    2686 CALL                     1
-                    2696 POP_TOP
-         
-         200        2698 LOAD_GLOBAL              7 (NULL + cl)
-                    2710 LOAD_ATTR                8 (Message)
-         
-         201        2720 LOAD_FAST               14 (function_name)
-         
-         202        2722 LOAD_GLOBAL              5 (NULL + str)
-                    2734 LOAD_FAST               15 (function_response)
-                    2736 PRECALL                  1
-                    2740 CALL                     1
-         
-         203        2750 LOAD_CONST              38 ('json')
-         
-         204        2752 LOAD_CONST              18 (1)
-         
-         200        2754 KW_NAMES                39
-                    2756 PRECALL                  4
-                    2760 CALL                     4
-         
-         205        2770 LOAD_METHOD             21 (send)
-                    2792 PRECALL                  0
-                    2796 CALL                     0
-         
-         200        2806 GET_AWAITABLE            0
-                    2808 LOAD_CONST               0 (None)
-                 >> 2810 SEND                     3 (to 2818)
-                    2812 YIELD_VALUE
-                    2814 RESUME                   3
-                    2816 JUMP_BACKWARD_NO_INTERRUPT     4 (to 2810)
-                 >> 2818 POP_TOP
-         
-         206        2820 LOAD_FAST                2 (cur_iter)
-                    2822 LOAD_CONST              18 (1)
-                    2824 BINARY_OP               13 (+=)
-                    2828 STORE_FAST               2 (cur_iter)
-         
-          96        2830 LOAD_FAST                2 (cur_iter)
-                    2832 LOAD_GLOBAL             14 (MAX_ITER)
-                    2844 COMPARE_OP               0 (<)
-                    2850 POP_JUMP_FORWARD_IF_FALSE    14 (to 2880)
-                    2852 LOAD_GLOBAL              0 (is_stop)
-                    2864 EXTENDED_ARG             5
-                    2866 POP_JUMP_BACKWARD_IF_FALSE  1292 (to 284)
-                    2868 LOAD_CONST               0 (None)
-                    2870 RETURN_VALUE
-                 >> 2872 LOAD_CONST               0 (None)
-                    2874 RETURN_VALUE
-                 >> 2876 LOAD_CONST               0 (None)
-                    2878 RETURN_VALUE
-                 >> 2880 LOAD_CONST               0 (None)
-                    2882 RETURN_VALUE
+                    1694 POP_JUMP_FORWARD_IF_TRUE     6 (to 1708)
+                    1696 LOAD_FAST               14 (function_name)
+                    1698 LOAD_CONST              26 ('python_exec')
+                    1700 COMPARE_OP               2 (==)
+                    1706 POP_JUMP_FORWARD_IF_FALSE    79 (to 1866)
+         
+         155     >> 1708 LOAD_FAST               14 (function_name)
+                    1710 LOAD_CONST              25 ('python')
+                    1712 COMPARE_OP               2 (==)
+                    1718 POP_JUMP_FORWARD_IF_FALSE     2 (to 1724)
+         
+         156        1720 LOAD_CONST              26 ('python_exec')
+                    1722 STORE_FAST              14 (function_name)
+         
+         157     >> 1724 LOAD_CONST              27 ('code')
+                    1726 LOAD_FAST                3 (openai_message)
+                    1728 LOAD_METHOD              5 (get)
+                    1750 LOAD_CONST              22 ('function_call')
+                    1752 PRECALL                  1
+                    1756 CALL                     1
+                    1766 LOAD_METHOD              5 (get)
+                    1788 LOAD_CONST              24 ('arguments')
+                    1790 PRECALL                  1
+                    1794 CALL                     1
+                    1804 BUILD_MAP                1
+                    1806 STORE_FAST              16 (arguments)
+         
+         158        1808 LOAD_GLOBAL             47 (NULL + json)
+                    1820 LOAD_ATTR               27 (dumps)
+                    1830 LOAD_FAST               16 (arguments)
+                    1832 PRECALL                  1
+                    1836 CALL                     1
+                    1846 LOAD_FAST                3 (openai_message)
+                    1848 LOAD_CONST              22 ('function_call')
+                    1850 BINARY_SUBSCR
+                    1860 LOAD_CONST              24 ('arguments')
+                    1862 STORE_SUBSCR
+                 >> 1866 POP_EXCEPT
+                    1868 JUMP_FORWARD             3 (to 1876)
+                 >> 1870 COPY                     3
+                    1872 POP_EXCEPT
+                    1874 RERAISE                  1
+                 >> 1876 POP_EXCEPT
+                    1878 JUMP_FORWARD             3 (to 1886)
+                 >> 1880 COPY                     3
+                    1882 POP_EXCEPT
+                    1884 RERAISE                  1
+         
+         159     >> 1886 NOP
+         
+         160        1888 LOAD_GLOBAL             20 (function_manager)
+                    1900 LOAD_METHOD             28 (call_function)
+         
+         161        1922 LOAD_FAST               14 (function_name)
+                    1924 LOAD_FAST               16 (arguments)
+         
+         160        1926 PRECALL                  2
+                    1930 CALL                     2
+                    1940 GET_AWAITABLE            0
+                    1942 LOAD_CONST               0 (None)
+                 >> 1944 SEND                     3 (to 1952)
+                    1946 YIELD_VALUE
+                    1948 RESUME                   3
+                    1950 JUMP_BACKWARD_NO_INTERRUPT     4 (to 1944)
+                 >> 1952 STORE_FAST              15 (function_response)
+                    1954 JUMP_FORWARD            35 (to 2026)
+                 >> 1956 PUSH_EXC_INFO
+         
+         162        1958 LOAD_GLOBAL             36 (Exception)
+                    1970 CHECK_EXC_MATCH
+                    1972 POP_JUMP_FORWARD_IF_FALSE    22 (to 2018)
+                    1974 STORE_FAST              13 (e)
+         
+         163        1976 LOAD_GLOBAL              3 (NULL + print)
+                    1988 LOAD_FAST               13 (e)
+                    1990 PRECALL                  1
+                    1994 CALL                     1
+                    2004 POP_TOP
+         
+         164        2006 LOAD_FAST               13 (e)
+                    2008 RAISE_VARARGS            1
+                 >> 2010 LOAD_CONST               0 (None)
+                    2012 STORE_FAST              13 (e)
+                    2014 DELETE_FAST             13 (e)
+                    2016 RERAISE                  1
+         
+         162     >> 2018 RERAISE                  0
+                 >> 2020 COPY                     3
+                    2022 POP_EXCEPT
+                    2024 RERAISE                  1
+         
+         165     >> 2026 LOAD_GLOBAL              3 (NULL + print)
+                    2038 LOAD_CONST               2 ('==================================')
+                    2040 PRECALL                  1
+                    2044 CALL                     1
+                    2054 POP_TOP
+         
+         166        2056 LOAD_GLOBAL              3 (NULL + print)
+                    2068 LOAD_FAST               15 (function_response)
+                    2070 PRECALL                  1
+                    2074 CALL                     1
+                    2084 POP_TOP
+         
+         167        2086 LOAD_GLOBAL             59 (NULL + type)
+                    2098 LOAD_FAST               15 (function_response)
+                    2100 PRECALL                  1
+                    2104 CALL                     1
+                    2114 LOAD_GLOBAL              4 (str)
+                    2126 COMPARE_OP               3 (!=)
+                    2132 POP_JUMP_FORWARD_IF_FALSE    15 (to 2164)
+         
+         168        2134 LOAD_GLOBAL              5 (NULL + str)
+                    2146 LOAD_FAST               15 (function_response)
+                    2148 PRECALL                  1
+                    2152 CALL                     1
+                    2162 STORE_FAST              15 (function_response)
+         
+         170     >> 2164 LOAD_FAST                1 (message_history)
+                    2166 LOAD_METHOD              6 (append)
+                    2188 LOAD_FAST                3 (openai_message)
+                    2190 PRECALL                  1
+                    2194 CALL                     1
+                    2204 POP_TOP
+         
+         172        2206 LOAD_FAST               14 (function_name)
+                    2208 LOAD_CONST              26 ('python_exec')
+                    2210 COMPARE_OP               2 (==)
+                    2216 POP_JUMP_FORWARD_IF_FALSE   182 (to 2582)
+                    2218 LOAD_CONST              28 ('status')
+                    2220 LOAD_FAST               15 (function_response)
+                    2222 CONTAINS_OP              0
+                    2224 POP_JUMP_FORWARD_IF_FALSE   178 (to 2582)
+                    2226 LOAD_CONST              29 ('error_info')
+                    2228 LOAD_FAST               15 (function_response)
+                    2230 CONTAINS_OP              0
+                    2232 POP_JUMP_FORWARD_IF_FALSE   174 (to 2582)
+                    2234 LOAD_CONST              30 ('error')
+                    2236 LOAD_FAST               15 (function_response)
+                    2238 CONTAINS_OP              0
+                    2240 POP_JUMP_FORWARD_IF_FALSE   170 (to 2582)
+         
+         174        2242 LOAD_GLOBAL              3 (NULL + print)
+                    2254 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
+                    2256 PRECALL                  1
+                    2260 CALL                     1
+                    2270 POP_TOP
+         
+         175        2272 LOAD_GLOBAL             47 (NULL + json)
+                    2284 LOAD_ATTR               24 (loads)
+                    2294 LOAD_FAST               15 (function_response)
+                    2296 PRECALL                  1
+                    2300 CALL                     1
+                    2310 STORE_FAST              15 (function_response)
+         
+         176        2312 LOAD_FAST               15 (function_response)
+                    2314 LOAD_CONST              32 ('description')
+                    2316 BINARY_SUBSCR
+                    2326 STORE_FAST              17 (description)
+         
+         177        2328 LOAD_FAST               15 (function_response)
+                    2330 LOAD_CONST              32 ('description')
+                    2332 DELETE_SUBSCR
+         
+         178        2334 LOAD_FAST                1 (message_history)
+                    2336 LOAD_METHOD              6 (append)
+         
+         179        2358 LOAD_CONST              33 ('function')
+         
+         180        2360 LOAD_FAST               14 (function_name)
+         
+         181        2362 LOAD_GLOBAL             47 (NULL + json)
+                    2374 LOAD_ATTR               27 (dumps)
+                    2384 LOAD_FAST               15 (function_response)
+                    2386 PRECALL                  1
+                    2390 CALL                     1
+         
+         178        2400 LOAD_CONST              34 (('role', 'name', 'content'))
+                    2402 BUILD_CONST_KEY_MAP      3
+                    2404 PRECALL                  1
+                    2408 CALL                     1
+                    2418 POP_TOP
+         
+         183        2420 LOAD_GLOBAL             30 (config_env)
+                    2432 LOAD_CONST              12 ('openai')
+                    2434 BINARY_SUBSCR
+                    2444 LOAD_CONST              35 ('language')
+                    2446 BINARY_SUBSCR
+                    2456 STORE_FAST              18 (language)
+         
+         184        2458 LOAD_FAST                1 (message_history)
+                    2460 LOAD_METHOD              6 (append)
+         
+         185        2482 LOAD_CONST               4 ('user')
+         
+         186        2484 LOAD_GLOBAL              5 (NULL + str)
+                    2496 LOAD_FAST               17 (description)
+                    2498 PRECALL                  1
+                    2502 CALL                     1
+                    2512 LOAD_CONST              36 ('\n\n')
+                    2514 BINARY_OP                0 (+)
+                    2518 LOAD_CONST              37 ('Please answer me in ')
+                    2520 BINARY_OP                0 (+)
+                    2524 LOAD_FAST               18 (language)
+                    2526 BINARY_OP                0 (+)
+         
+         184        2530 LOAD_CONST               5 (('role', 'content'))
+                    2532 BUILD_CONST_KEY_MAP      2
+                    2534 PRECALL                  1
+                    2538 CALL                     1
+                    2548 POP_TOP
+         
+         188        2550 LOAD_GLOBAL              3 (NULL + print)
+                    2562 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
+                    2564 PRECALL                  1
+                    2568 CALL                     1
+                    2578 POP_TOP
+                    2580 JUMP_FORWARD            25 (to 2632)
+         
+         190     >> 2582 LOAD_FAST                1 (message_history)
+                    2584 LOAD_METHOD              6 (append)
+         
+         191        2606 LOAD_CONST              33 ('function')
+         
+         192        2608 LOAD_FAST               14 (function_name)
+         
+         193        2610 LOAD_FAST               15 (function_response)
+         
+         190        2612 LOAD_CONST              34 (('role', 'name', 'content'))
+                    2614 BUILD_CONST_KEY_MAP      3
+                    2616 PRECALL                  1
+                    2620 CALL                     1
+                    2630 POP_TOP
+         
+         196     >> 2632 LOAD_GLOBAL              3 (NULL + print)
+                    2644 LOAD_CONST               2 ('==================================')
+                    2646 PRECALL                  1
+                    2650 CALL                     1
+                    2660 POP_TOP
+         
+         197        2662 LOAD_GLOBAL              3 (NULL + print)
+                    2674 LOAD_FAST                1 (message_history)
+                    2676 PRECALL                  1
+                    2680 CALL                     1
+                    2690 POP_TOP
+         
+         198        2692 LOAD_GLOBAL              3 (NULL + print)
+                    2704 LOAD_CONST               2 ('==================================')
+                    2706 PRECALL                  1
+                    2710 CALL                     1
+                    2720 POP_TOP
+         
+         200        2722 LOAD_GLOBAL              7 (NULL + cl)
+                    2734 LOAD_ATTR                8 (Message)
+         
+         201        2744 LOAD_FAST               14 (function_name)
+         
+         202        2746 LOAD_GLOBAL              5 (NULL + str)
+                    2758 LOAD_FAST               15 (function_response)
+                    2760 PRECALL                  1
+                    2764 CALL                     1
+         
+         203        2774 LOAD_CONST              38 ('json')
+         
+         204        2776 LOAD_CONST              18 (1)
+         
+         200        2778 KW_NAMES                39
+                    2780 PRECALL                  4
+                    2784 CALL                     4
+         
+         205        2794 LOAD_METHOD             21 (send)
+                    2816 PRECALL                  0
+                    2820 CALL                     0
+         
+         200        2830 GET_AWAITABLE            0
+                    2832 LOAD_CONST               0 (None)
+                 >> 2834 SEND                     3 (to 2842)
+                    2836 YIELD_VALUE
+                    2838 RESUME                   3
+                    2840 JUMP_BACKWARD_NO_INTERRUPT     4 (to 2834)
+                 >> 2842 POP_TOP
+         
+         206        2844 LOAD_FAST                2 (cur_iter)
+                    2846 LOAD_CONST              18 (1)
+                    2848 BINARY_OP               13 (+=)
+                    2852 STORE_FAST               2 (cur_iter)
+         
+          96        2854 LOAD_FAST                2 (cur_iter)
+                    2856 LOAD_GLOBAL             14 (MAX_ITER)
+                    2868 COMPARE_OP               0 (<)
+                    2874 POP_JUMP_FORWARD_IF_FALSE    14 (to 2904)
+                    2876 LOAD_GLOBAL              0 (is_stop)
+                    2888 EXTENDED_ARG             5
+                    2890 POP_JUMP_BACKWARD_IF_FALSE  1304 (to 284)
+                    2892 LOAD_CONST               0 (None)
+                    2894 RETURN_VALUE
+                 >> 2896 LOAD_CONST               0 (None)
+                    2898 RETURN_VALUE
+                 >> 2900 LOAD_CONST               0 (None)
+                    2902 RETURN_VALUE
+                 >> 2904 LOAD_CONST               0 (None)
+                    2906 RETURN_VALUE
          ExceptionTable:
-           376 to 840 -> 844 [0]
-           844 to 862 -> 978 [1] lasti
-           864 to 954 -> 968 [1] lasti
-           968 to 976 -> 978 [1] lasti
-           1414 to 1528 -> 1532 [0]
-           1532 to 1534 -> 1856 [1] lasti
-           1538 to 1652 -> 1656 [1]
-           1654 to 1654 -> 1856 [1] lasti
-           1656 to 1840 -> 1846 [2] lasti
-           1842 to 1850 -> 1856 [1] lasti
-           1864 to 1928 -> 1932 [0]
-           1932 to 1950 -> 1996 [1] lasti
-           1952 to 1984 -> 1986 [1] lasti
-           1986 to 1994 -> 1996 [1] lasti
+           376 to 716 -> 868 [0]
+           718 to 728 -> 864 [1]
+           730 to 864 -> 868 [0]
+           868 to 886 -> 1002 [1] lasti
+           888 to 978 -> 992 [1] lasti
+           992 to 1000 -> 1002 [1] lasti
+           1438 to 1552 -> 1556 [0]
+           1556 to 1558 -> 1880 [1] lasti
+           1562 to 1676 -> 1680 [1]
+           1678 to 1678 -> 1880 [1] lasti
+           1680 to 1864 -> 1870 [2] lasti
+           1866 to 1874 -> 1880 [1] lasti
+           1888 to 1952 -> 1956 [0]
+           1956 to 1974 -> 2020 [1] lasti
+           1976 to 2008 -> 2010 [1] lasti
+           2010 to 2018 -> 2020 [1] lasti
          consts
             None
             False
             '=================================='
             'message_history'
             'user'
             ('role', 'content')
@@ -1575,30 +1590,31 @@
             'function'
             ('role', 'name', 'content')
             'language'
             '\n\n'
             'Please answer me in '
             'json'
             ('author', 'content', 'language', 'indent')
-         names      ('is_stop', 'print', 'str', 'cl', 'user_session', 'get', 'append', 'MAX_ITER', 'Message', '__truncate_conversation', 'function_manager', 'generate_functions_array', 'openai', 'ChatCompletion', 'create', 'config_env', 'choices', 'process_new_delta', 'Exception', 'asyncio', 'sleep', 'send', 'ValueError', 'json', 'loads', 'ast', 'literal_eval', 'dumps', 'call_function', 'type')
+         names      ('is_stop', 'print', 'str', 'cl', 'user_session', 'get', 'append', 'MAX_ITER', 'Message', '__truncate_conversation', 'function_manager', 'generate_functions_array', 'openai', 'ChatCompletion', 'acreate', 'config_env', 'choices', 'process_new_delta', 'Exception', 'asyncio', 'sleep', 'send', 'ValueError', 'json', 'loads', 'ast', 'literal_eval', 'dumps', 'call_function', 'type')
          varnames   ('user_message', 'message_history', 'cur_iter', 'openai_message', 'function_ui_message', 'content_ui_message', 'stream_resp', 'send_message', 'functions', 'user_plugin_api_info', 'item', 'i', 'new_delta', 'e', 'function_name', 'function_response', 'arguments', 'description', 'language')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'on_message'
          firstlineno 86
          lnotab
             0x060204011e011e011e011e013e013001040128020a0104012a0104011e
             01020132013e010401080114012cff020220012c01240102010201020102
-            0102fa160726010e0104010e0104010c0108ff2a0212011e010a01340114
-            fc0806040134010402040134022e0104012e014002500144010401020116
-            014eff14020201020116014eff1402020118010c01040154014e01020122
-            0104ff200212011e010cfe08031e011e0130011e022a0224021e01280110
-            01060118010201020126fd14052601180102012efe140420021801020102
-            0102fd14061e011e011e02160102011c01020102fc100524fb0e060a92
+            0102fa2c0726010e0104010e0104010c0108ff26f4060e12011e010a0134
+            0114fc0806040134010402040134022e0104012e01400250014401040102
+            0116014eff14020201020116014eff1402020118010c01040154014e0102
+            01220104ff200212011e010cfe08031e011e0130011e022a0224021e0128
+            011001060118010201020126fd14052601180102012efe14042002180102
+            01020102fd14061e011e011e02160102011c01020102fc100524fb0e060a
+            92
       code
          argcount  : 4
          nlocals   : 6
          stacksize : 6
          flags     : 131
          code
             0x4b000100970064017c007600720b7c006401190000000000000000007c
@@ -1832,15 +1848,15 @@
             'json'
             ('author', 'content', 'indent', 'language')
             'arguments'
          names      ('get', 'stream_token', 'send', 'cl', 'Message')
          varnames   ('new_delta', 'openai_message', 'content_ui_message', 'function_ui_message', 'new_content', 'function_name')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'process_new_delta'
          firstlineno 209
          lnotab
             0x06020801160108012e0120013601080114011c010c01040204ff0a0334
             01160102010201020102fc12053602140114011601200102ff0a0102ff16
             0218011aff1c02
       'error_info'
@@ -1894,15 +1910,15 @@
             'llm_chain'
             ('callbacks',)
             None
          names      ('cl', 'user_session', 'get', 'acall', 'AsyncLangchainCallbackHandler')
          varnames   ('error_info', 'llm_chain', 'res')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'analyze_error'
          firstlineno 243
          lnotab 0x06073e015e01
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 7
@@ -2044,15 +2060,15 @@
             'upload_guide'
             ('author', 'content')
             'random_user_id'
          names      ('config_env', 'cl', 'user_session', 'set', 'Avatar', 'send', 'Message', 'get_text', 'str', 'uuid', 'uuid4')
          varnames   ('content', 'language')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'start_chat'
          firstlineno 255
          lnotab
             0x0602040f26012c010203020114fd06fe10081601020102fe100324fd0e
             04160102011efe100324fd0e04
       code
          argcount  : 1
@@ -2309,15 +2325,15 @@
             'upload_notification'
             ' ./tmp/'
             ('author', 'content')
          names      ('str', 'os', 'path', 'exists', 'mkdir', 'cl', 'AskFileMessage', 'send', 'name', 'content', 'open', 'write', 'user_session', 'get', 'append', 'config_env', 'Message', 'get_text', 'on_message')
          varnames   ('user_message', 'files', 'file', 'save_path', 'file_path', 'content', 'f', 'message_history', 'language')
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'run_conversation'
          firstlineno 293
          lnotab
             0x060228013e01280116010201020202ff02fd100524fb0e06100104030c
             010e010a020e0322012aff2e023e01180102010afe140426011601020128
             fe100324fd0e040402
       code
@@ -2346,23 +2362,23 @@
             None
             'stop chat'
             True
          names      ('print', 'is_stop')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+         filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
          name       'stop_chat'
          firstlineno 332
          lnotab 0x06031e01
    names      ('uuid', 'openai', 'json', 'ast', 'os', 'chainlit', 'cl', 'functions.FunctionManager', 'FunctionManager', 'inspect', 'tiktoken', 'importlib', 'asyncio', 'get_text', 'path', 'join', 'expanduser', 'config_path', 'open', 'config_file', 'load', 'config_env', 'api_key', 'api_base', 'listdir', 'plugin_dirs', 'functions', 'dir', 'f', 'config', 'get', 'enabled', 'FileNotFoundError', 'import_module', 'module', 'extend', 'getmembers', 'function_manager', 'print', 'generate_functions_array', 'env_max_tokens', 'int', 'max_tokens', 'is_stop', '__truncate_conversation', 'get_token_count', 'MAX_ITER', 'object', 'on_message', 'process_new_delta', 'str', 'analyze_error', 'on_chat_start', 'start_chat', 'run_conversation', 'on_stop', 'stop_chat')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_cn.py'
+   filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c0108010801080108010c0468
       031a0120ff2e032601260204011eff1205040108010201220120ff2e0230
       01080108ff08030401020228011c011eff220418013c011c010401180204
       010403060c060e04030c7b06220c0c0c0104ff0e0102250c010aff0e0102
```

### Comparing `codebot-0.0.5/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.0.6/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.0.6/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.0.6/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/app.py` & `codebot-0.0.6/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/app_cn.py` & `codebot-0.0.6/src/app_cn.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,14 +250,23 @@
         origin_code: The original code.(required)
         error_info: The error info.(required)
     """
     llm_chain = cl.user_session.get("llm_chain")
     res = await llm_chain.acall(error_info, callbacks=[cl.AsyncLangchainCallbackHandler()])
     return res
 
+async def ask_user_for_remote_details():
+    """
+    Ask the user for the remote connection details and save them in the session.
+    """
+    for key in ['remote_ip', 'remote_username', 'remote_port', 'remote_password']:
+        if not cl.user_session.get(key):
+            res = await cl.AskUserMessage(content=f"What is the {key.replace('_', ' ')}?", timeout=10).send()
+            cl.user_session.set(key, res['content'])
+
 
 @cl.on_chat_start
 async def start_chat():
     content = '''1.You are now a code interpreter in the Jupyter Notebook environment. When you encounter code that needs to be processed, please use Python code to analyze and solve the corresponding problems. You can solve problems step by step and can also use variables generated from previous code at any time.
 2.to show images or files, you should respond like ![image](./tmp/xxx.png), download the file like [file](./tmp/xxx.png)
 example:
 ```json
```

### Comparing `codebot-0.0.5/src/functions/FunctionManager.py` & `codebot-0.0.6/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.0.6/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/get_text.py` & `codebot-0.0.6/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/language/en.json` & `codebot-0.0.6/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/language/zh_CN.json` & `codebot-0.0.6/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.6/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/common/functions.py` & `codebot-0.0.6/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/mysql/functions.py` & `codebot-0.0.6/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.6/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/executor.py` & `codebot-0.0.6/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/python/functions.py` & `codebot-0.0.6/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.0.6/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.0.6/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/plugins/vue/functions.py` & `codebot-0.0.6/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/tmp/1690769899.3643498.png` & `codebot-0.0.6/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/tmp/1690769912.7088609.png` & `codebot-0.0.6/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/tmp/sin_function.gif` & `codebot-0.0.6/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.0.5/src/tmp/sin_function.png` & `codebot-0.0.6/src/tmp/sin_function.png`

 * *Files identical despite different names*

