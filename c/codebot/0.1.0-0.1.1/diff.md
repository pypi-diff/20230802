# Comparing `tmp/codebot-0.1.0.tar.gz` & `tmp/codebot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.1.0.tar", last modified: Wed Aug  2 08:12:54 2023, max compression
+gzip compressed data, was "codebot-0.1.1.tar", last modified: Wed Aug  2 08:23:46 2023, max compression
```

## Comparing `codebot-0.1.0.tar` & `codebot-0.1.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.129688 codebot-0.1.0/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.1.0/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:12:54.129327 codebot-0.1.0/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.076100 codebot-0.1.0/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2576 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      124 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 08:12:54.129793 codebot-0.1.0/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      591 2023-08-02 08:12:49.000000 codebot-0.1.0/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.081118 codebot-0.1.0/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.082712 codebot-0.1.0/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.1.0/src/.chainlit/.langchain.db
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.1.0/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5818 2023-08-02 08:12:22.000000 codebot-0.1.0/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.093229 codebot-0.1.0/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 07:29:57.000000 codebot-0.1.0/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.1.0/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.1.0/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.1.0/src/__pycache__/app.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.1.0/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.1.0/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.1.0/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    18128 2023-08-02 08:06:54.000000 codebot-0.1.0/src/__pycache__/app_terminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.1.0/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.1.0/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13482 2023-08-02 08:11:50.000000 codebot-0.1.0/src/app_terminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.1.0/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.094997 codebot-0.1.0/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7172 2023-08-02 07:32:10.000000 codebot-0.1.0/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1140 2023-08-02 07:45:08.000000 codebot-0.1.0/src/functions/RemoteTerminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1.0/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.099259 codebot-0.1.0/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7715 2023-08-02 07:32:13.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2756 2023-08-02 07:45:43.000000 codebot-0.1.0/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.1.0/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.1.0/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.100898 codebot-0.1.0/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.1.0/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.1.0/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.1.0/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.101733 codebot-0.1.0/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.1.0/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.102176 codebot-0.1.0/src/plugins/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.1.0/src/plugins/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.103213 codebot-0.1.0/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.104937 codebot-0.1.0/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.106050 codebot-0.1.0/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.107765 codebot-0.1.0/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.111131 codebot-0.1.0/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.1.0/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.112868 codebot-0.1.0/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.118019 codebot-0.1.0/src/plugins/terminal/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.118917 codebot-0.1.0/src/plugins/terminal/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3845 2023-08-02 07:30:01.000000 codebot-0.1.0/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.1.0/src/plugins/terminal/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2895 2023-08-02 07:27:13.000000 codebot-0.1.0/src/plugins/terminal/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.120983 codebot-0.1.0/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.128316 codebot-0.1.0/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.1.0/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.1.0/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.1.0/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.1.0/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.660256 codebot-0.1.1/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.1.1/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:23:46.659853 codebot-0.1.1/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.591244 codebot-0.1.1/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2576 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      124 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 08:23:46.000000 codebot-0.1.1/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 08:23:46.660432 codebot-0.1.1/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      591 2023-08-02 08:23:42.000000 codebot-0.1.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.596797 codebot-0.1.1/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.598302 codebot-0.1.1/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.1.1/src/.chainlit/.langchain.db
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.1.1/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5921 2023-08-02 08:23:31.000000 codebot-0.1.1/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.610270 codebot-0.1.1/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 07:29:57.000000 codebot-0.1.1/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.1.1/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.1.1/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.1.1/src/__pycache__/app.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.1.1/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.1.1/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.1.1/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    18128 2023-08-02 08:06:54.000000 codebot-0.1.1/src/__pycache__/app_terminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.1.1/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.1.1/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.1.1/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13482 2023-08-02 08:11:50.000000 codebot-0.1.1/src/app_terminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.1.1/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.613352 codebot-0.1.1/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7172 2023-08-02 07:32:10.000000 codebot-0.1.1/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1140 2023-08-02 07:45:08.000000 codebot-0.1.1/src/functions/RemoteTerminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1.1/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.619651 codebot-0.1.1/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7715 2023-08-02 07:32:13.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2756 2023-08-02 07:45:43.000000 codebot-0.1.1/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.1.1/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.1.1/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.1.1/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.621628 codebot-0.1.1/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.1.1/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.1.1/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.1.1/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.622607 codebot-0.1.1/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.1.1/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.623173 codebot-0.1.1/src/plugins/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.1.1/src/plugins/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.624583 codebot-0.1.1/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.627684 codebot-0.1.1/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.629403 codebot-0.1.1/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.631982 codebot-0.1.1/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.637992 codebot-0.1.1/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.1.1/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.640289 codebot-0.1.1/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.646092 codebot-0.1.1/src/plugins/terminal/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.646820 codebot-0.1.1/src/plugins/terminal/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3845 2023-08-02 07:30:01.000000 codebot-0.1.1/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.1.1/src/plugins/terminal/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2895 2023-08-02 07:27:13.000000 codebot-0.1.1/src/plugins/terminal/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.648398 codebot-0.1.1/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.1.1/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:23:46.658837 codebot-0.1.1/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.1.1/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.1.1/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.1.1/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.1.1/src/tmp/sin_function.png
```

### Comparing `codebot-0.1.0/codebot.egg-info/SOURCES.txt` & `codebot-0.1.1/codebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/setup.py` & `codebot-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="codebot",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "codebot = src:main",
             "terminalbot = src:main_terminal",  # 添加这一行
         ],
     },
```

### Comparing `codebot-0.1.0/src/.chainlit/.langchain.db` & `codebot-0.1.1/src/.chainlit/.langchain.db`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/.chainlit/config.toml` & `codebot-0.1.1/src/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__init__.py` & `codebot-0.1.1/src/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,28 +121,29 @@
     else:
         subprocess.run(["chainlit", "run", "app.py"])  # Run your application
         
         
 def main_terminal():
     parser = argparse.ArgumentParser()
     parser.add_argument("--config", action="store_true", help="Reset configuration")
+    parser.add_argument("--port", type=int, help="Port")
     args = parser.parse_args()
     os.chdir(os.path.dirname(os.path.abspath(__file__)))  # Change the current working directory to your application's directory
     if args.config:
         # If the --config option is given, delete the existing configuration file and create a new one
         config_path = os.path.join(os.path.expanduser('~'), '.codebot', 'config.json')
         if os.path.exists(config_path):
             os.remove(config_path)
         check_config(force_config=True)  # Check and create the configuration file
     else:
         print("Checking configuration...")
         check_config()  # Check and create the configuration file if not exists
     
    
             
-
-    subprocess.run(["chainlit", "run", "app_terminal.py", "--port", "10086"])  # Run your application
+    port = args.port if args.port else 10086
+    subprocess.run(["chainlit", "run", "app_terminal.py", "--port", str(port)])  # Run your application
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `codebot-0.1.0/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.1.1/src/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.1.1/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app.cpython-310.pyc` & `codebot-0.1.1/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app.cpython-311.pyc` & `codebot-0.1.1/src/__pycache__/app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app.cpython-38.pyc` & `codebot-0.1.1/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.1.1/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.1.1/src/__pycache__/app_cn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/app_terminal.cpython-311.pyc` & `codebot-0.1.1/src/__pycache__/app_terminal.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.1.1/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.1.1/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.1.1/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/app.py` & `codebot-0.1.1/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/app_cn.py` & `codebot-0.1.1/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/app_terminal.py` & `codebot-0.1.1/src/app_terminal.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/chainlit.md` & `codebot-0.1.1/src/chainlit.md`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/FunctionManager.py` & `codebot-0.1.1/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/RemoteTerminal.py` & `codebot-0.1.1/src/functions/RemoteTerminal.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.1.1/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc` & `codebot-0.1.1/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/get_text.py` & `codebot-0.1.1/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/language/en.json` & `codebot-0.1.1/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/language/zh_CN.json` & `codebot-0.1.1/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.1/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/common/functions.py` & `codebot-0.1.1/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/mysql/functions.py` & `codebot-0.1.1/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.1/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/executor.py` & `codebot-0.1.1/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/python/functions.py` & `codebot-0.1.1/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.1.1/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.1.1/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/terminal/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.1/src/plugins/terminal/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/terminal/functions.py` & `codebot-0.1.1/src/plugins/terminal/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/plugins/vue/functions.py` & `codebot-0.1.1/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/tmp/1690769899.3643498.png` & `codebot-0.1.1/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/tmp/1690769912.7088609.png` & `codebot-0.1.1/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/tmp/sin_function.gif` & `codebot-0.1.1/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.1.0/src/tmp/sin_function.png` & `codebot-0.1.1/src/tmp/sin_function.png`

 * *Files identical despite different names*

