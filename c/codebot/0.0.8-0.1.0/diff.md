# Comparing `tmp/codebot-0.0.8.tar.gz` & `tmp/codebot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.8.tar", last modified: Wed Aug  2 06:55:08 2023, max compression
+gzip compressed data, was "codebot-0.1.0.tar", last modified: Wed Aug  2 08:12:54 2023, max compression
```

## Comparing `codebot-0.0.8.tar` & `codebot-0.1.0.tar`

### file list

```diff
@@ -1,91 +1,93 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.972961 codebot-0.0.8/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.8/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:55:08.972395 codebot-0.0.8/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.762044 codebot-0.0.8/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2487 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 06:55:08.000000 codebot-0.0.8/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 06:55:08.973885 codebot-0.0.8/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      571 2023-08-02 06:55:05.000000 codebot-0.0.8/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.807150 codebot-0.0.8/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.811267 codebot-0.0.8/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.0.8/src/.chainlit/.langchain.db
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.0.8/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5836 2023-08-02 06:54:59.000000 codebot-0.0.8/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.844973 codebot-0.0.8/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 06:54:52.000000 codebot-0.0.8/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.8/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.8/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.0.8/src/__pycache__/app.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.8/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.8/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.0.8/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    15650 2023-08-02 06:40:06.000000 codebot-0.0.8/src/__pycache__/app_terminal.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.8/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.8/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.0.8/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    11401 2023-08-02 06:39:48.000000 codebot-0.0.8/src/app_terminal.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.0.8/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.851072 codebot-0.0.8/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.8/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.8/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.862867 codebot-0.0.8/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.8/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.8/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.8/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.870865 codebot-0.0.8/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.8/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.8/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.8/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.872888 codebot-0.0.8/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.8/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.875912 codebot-0.0.8/src/plugins/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.0.8/src/plugins/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.878300 codebot-0.0.8/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.886340 codebot-0.0.8/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.893616 codebot-0.0.8/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.898936 codebot-0.0.8/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.917359 codebot-0.0.8/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.0.8/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.927939 codebot-0.0.8/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.938479 codebot-0.0.8/src/plugins/terminal/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.940967 codebot-0.0.8/src/plugins/terminal/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2410 2023-08-02 06:02:16.000000 codebot-0.0.8/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.0.8/src/plugins/terminal/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1812 2023-08-02 06:00:40.000000 codebot-0.0.8/src/plugins/terminal/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.945130 codebot-0.0.8/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.8/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 06:55:08.970449 codebot-0.0.8/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.8/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.8/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.8/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.8/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.129688 codebot-0.1.0/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.1.0/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:12:54.129327 codebot-0.1.0/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.076100 codebot-0.1.0/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2576 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       69 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      124 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-08-02 08:12:54.000000 codebot-0.1.0/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-08-02 08:12:54.129793 codebot-0.1.0/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      591 2023-08-02 08:12:49.000000 codebot-0.1.0/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.081118 codebot-0.1.0/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.082712 codebot-0.1.0/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12288 2023-08-02 05:27:38.000000 codebot-0.1.0/src/.chainlit/.langchain.db
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-08-02 06:11:04.000000 codebot-0.1.0/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5818 2023-08-02 08:12:22.000000 codebot-0.1.0/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.093229 codebot-0.1.0/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7939 2023-08-02 07:29:57.000000 codebot-0.1.0/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.1.0/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.1.0/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17427 2023-08-02 05:27:37.000000 codebot-0.1.0/src/__pycache__/app.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.1.0/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.1.0/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    16920 2023-08-02 05:48:05.000000 codebot-0.1.0/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    18128 2023-08-02 08:06:54.000000 codebot-0.1.0/src/__pycache__/app_terminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.1.0/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.1.0/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13253 2023-08-02 05:55:27.000000 codebot-0.1.0/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    13482 2023-08-02 08:11:50.000000 codebot-0.1.0/src/app_terminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1923 2023-08-02 06:46:06.000000 codebot-0.1.0/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.094997 codebot-0.1.0/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7172 2023-08-02 07:32:10.000000 codebot-0.1.0/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1140 2023-08-02 07:45:08.000000 codebot-0.1.0/src/functions/RemoteTerminal.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1.0/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.099259 codebot-0.1.0/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7715 2023-08-02 07:32:13.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2756 2023-08-02 07:45:43.000000 codebot-0.1.0/src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.1.0/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.1.0/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.1.0/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.100898 codebot-0.1.0/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.1.0/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.1.0/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.1.0/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.101733 codebot-0.1.0/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.1.0/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.102176 codebot-0.1.0/src/plugins/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      183 2023-08-02 05:27:38.000000 codebot-0.1.0/src/plugins/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.103213 codebot-0.1.0/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.104937 codebot-0.1.0/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.106050 codebot-0.1.0/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.107765 codebot-0.1.0/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.111131 codebot-0.1.0/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-08-02 05:28:08.000000 codebot-0.1.0/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.112868 codebot-0.1.0/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.118019 codebot-0.1.0/src/plugins/terminal/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.118917 codebot-0.1.0/src/plugins/terminal/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3845 2023-08-02 07:30:01.000000 codebot-0.1.0/src/plugins/terminal/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-08-02 05:11:17.000000 codebot-0.1.0/src/plugins/terminal/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2895 2023-08-02 07:27:13.000000 codebot-0.1.0/src/plugins/terminal/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.120983 codebot-0.1.0/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.1.0/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-08-02 08:12:54.128316 codebot-0.1.0/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.1.0/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.1.0/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.1.0/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.1.0/src/tmp/sin_function.png
```

### Comparing `codebot-0.0.8/codebot.egg-info/SOURCES.txt` & `codebot-0.1.0/codebot.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 src/__pycache__/app_cn.cpython-310.pyc
 src/__pycache__/app_cn.cpython-311.pyc
 src/__pycache__/app_terminal.cpython-311.pyc
 src/__pycache__/get_text.cpython-310.pyc
 src/__pycache__/get_text.cpython-311.pyc
 src/__pycache__/get_text.cpython-38.pyc
 src/functions/FunctionManager.py
+src/functions/RemoteTerminal.py
 src/functions/__init__.py
 src/functions/__pycache__/FunctionManager.cpython-310.pyc
 src/functions/__pycache__/FunctionManager.cpython-311.pyc
 src/functions/__pycache__/FunctionManager.cpython-38.pyc
+src/functions/__pycache__/RemoteTerminal.cpython-311.pyc
 src/functions/__pycache__/__init__.cpython-310.pyc
 src/functions/__pycache__/__init__.cpython-311.pyc
 src/functions/__pycache__/__init__.cpython-38.pyc
 src/language/__init__.py
 src/language/en.json
 src/language/zh_CN.json
 src/plugins/__init__.py
```

### Comparing `codebot-0.0.8/setup.py` & `codebot-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="codebot",
-    version="0.0.8",
+    version="0.1.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "codebot = src:main",
             "terminalbot = src:main_terminal",  # 添加这一行
         ],
     },
@@ -14,11 +14,12 @@
         "chainlit==0.5.2",
         "loguru==0.5.3",
         "tiktoken==0.4.0",
         "prompt_toolkit==3.0.39",
         "jupyter",
         "mysql-connector-python",
         "pillow",
-        "pyngrok"
+        "pyngrok",
+        "paramiko"
     ],
     include_package_data=True,  # Add this line
 )
```

### Comparing `codebot-0.0.8/src/.chainlit/.langchain.db` & `codebot-0.1.0/src/.chainlit/.langchain.db`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/.chainlit/config.toml` & `codebot-0.1.0/src/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__init__.py` & `codebot-0.1.0/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,18 +128,18 @@
     args = parser.parse_args()
     os.chdir(os.path.dirname(os.path.abspath(__file__)))  # Change the current working directory to your application's directory
     if args.config:
         # If the --config option is given, delete the existing configuration file and create a new one
         config_path = os.path.join(os.path.expanduser('~'), '.codebot', 'config.json')
         if os.path.exists(config_path):
             os.remove(config_path)
-        check_config_terminal(force_config=True)  # Check and create the configuration file
+        check_config(force_config=True)  # Check and create the configuration file
     else:
         print("Checking configuration...")
-        check_config_terminal()  # Check and create the configuration file if not exists
+        check_config()  # Check and create the configuration file if not exists
     
    
             
 
     subprocess.run(["chainlit", "run", "app_terminal.py", "--port", "10086"])  # Run your application
```

### Comparing `codebot-0.0.8/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.1.0/src/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xbafdc964 (Wed Aug  2 06:54:50 2023 UTC)
+moddate:  0xc3fdc964 (Wed Aug  2 06:54:59 2023 UTC)
 files sz: 5836
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `codebot-0.0.8/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.1.0/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app.cpython-310.pyc` & `codebot-0.1.0/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app.cpython-311.pyc` & `codebot-0.1.0/src/__pycache__/app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app.cpython-38.pyc` & `codebot-0.1.0/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.1.0/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.1.0/src/__pycache__/app_cn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/app_terminal.cpython-311.pyc` & `codebot-0.1.0/src/__pycache__/app_terminal.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x34fac964 (Wed Aug  2 06:39:48 2023 UTC)
-files sz: 11401
+moddate:  0x990eca64 (Wed Aug  2 08:06:49 2023 UTC)
+files sz: 13369
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -392,53 +392,53 @@
     90        1104 LOAD_CONST              28 ('user_message')
               1106 LOAD_NAME               53 (object)
               1108 BUILD_TUPLE              2
               1110 LOAD_CONST              29 (<code object on_message, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 90>)
               1112 MAKE_FUNCTION            4 (annotations)
               1114 STORE_NAME              54 (on_message)
    
-   213        1116 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 213>)
+   235        1116 LOAD_CONST              30 (<code object process_new_delta, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 235>)
               1118 MAKE_FUNCTION            0
               1120 STORE_NAME              55 (process_new_delta)
    
-   248        1122 LOAD_NAME                6 (cl)
+   270        1122 LOAD_NAME                6 (cl)
               1124 LOAD_ATTR               56 (on_chat_start)
    
-   249        1134 LOAD_CONST              31 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 248>)
+   271        1134 LOAD_CONST              31 (<code object start_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 270>)
               1136 MAKE_FUNCTION            0
    
-   248        1138 PRECALL                  0
+   270        1138 PRECALL                  0
               1142 CALL                     0
    
-   249        1152 STORE_NAME              57 (start_chat)
+   271        1152 STORE_NAME              57 (start_chat)
    
-   278        1154 LOAD_NAME                6 (cl)
+   324        1154 LOAD_NAME                6 (cl)
               1156 LOAD_ATTR               54 (on_message)
    
-   279        1166 LOAD_CONST              28 ('user_message')
+   325        1166 LOAD_CONST              28 ('user_message')
               1168 LOAD_NAME               53 (object)
               1170 BUILD_TUPLE              2
-              1172 LOAD_CONST              32 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 278>)
+              1172 LOAD_CONST              32 (<code object run_conversation, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 324>)
               1174 MAKE_FUNCTION            4 (annotations)
    
-   278        1176 PRECALL                  0
+   324        1176 PRECALL                  0
               1180 CALL                     0
    
-   279        1190 STORE_NAME              58 (run_conversation)
+   325        1190 STORE_NAME              58 (run_conversation)
    
-   317        1192 LOAD_NAME                6 (cl)
+   363        1192 LOAD_NAME                6 (cl)
               1194 LOAD_ATTR               59 (on_stop)
    
-   318        1204 LOAD_CONST              33 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 317>)
+   364        1204 LOAD_CONST              33 (<code object stop_chat, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py", line 363>)
               1206 MAKE_FUNCTION            0
    
-   317        1208 PRECALL                  0
+   363        1208 PRECALL                  0
               1212 CALL                     0
    
-   318        1222 STORE_NAME              60 (stop_chat)
+   364        1222 STORE_NAME              60 (stop_chat)
               1224 LOAD_CONST               1 (None)
               1226 RETURN_VALUE
    ExceptionTable:
      242 to 274 -> 300 [1] lasti
      300 to 306 -> 308 [3] lasti
      314 to 314 -> 308 [3] lasti
      618 to 648 -> 776 [1]
@@ -750,28 +750,28 @@
          name       'get_token_count'
          firstlineno 73
          lnotab 0x02014a02040108010a01320164010c010cfd02040a01
       100
       'user_message'
       code
          argcount  : 1
-         nlocals   : 19
+         nlocals   : 21
          stacksize : 8
          flags     : 131
          code
             0x4b0001009700640161007403000000000000000000006402a6010000ab
             01000000000000000001007403000000000000000000007c00a6010000ab
             01000000000000000001007403000000000000000000006402a6010000ab
             01000000000000000001007405000000000000000000007c00a6010000ab
             0100000000000000007d007406000000000000000000006a040000000000
             000000a00500000000000000000000000000000000000000006403a60100
             00ab0100000000000000007d017c01a00600000000000000000000000000
             0000000000000064047c0064059c02a6010000ab01000000000000000001
-            0064067d027c02740e000000000000000000006b00000000009005721674
-            0000000000000000000000900573106407640764059c027d0364007d0474
+            0064067d027c02740e000000000000000000006b00000000009006721774
+            0000000000000000000000900673116407640764059c027d0364007d0474
             07000000000000000000006a0800000000000000006407ac08a6010000ab
             0100000000000000007d0564007d067413000000000000000000007c01a6
             010000ab0100000000000000007d070900741400000000000000000000a0
             0b0000000000000000000000000000000000000000a6000000ab00000000
             00000000007d087406000000000000000000006a040000000000000000a0
             0500000000000000000000000000000000000000006409a6010000ab0100
             000000000000007d097c0981257c0944005d227d0a7c0a640a1900000000
@@ -844,21 +844,38 @@
             247a00000064257a0000007c127a00000064059c02a6010000ab01000000
             00000000000100740300000000000000000000641fa6010000ab01000000
             000000000001006e197c01a0060000000000000000000000000000000000
             00000064217c0e7c0f64229c03a6010000ab010000000000000000010074
             03000000000000000000006402a6010000ab010000000000000000010074
             03000000000000000000007c01a6010000ab010000000000000000010074
             03000000000000000000006402a6010000ab010000000000000000010074
-            07000000000000000000006a0800000000000000007c0e74050000000000
-            00000000007c0fa6010000ab01000000000000000064266412ac27a60400
-            00ab040000000000000000a0150000000000000000000000000000000000
-            000000a6000000ab000000000000000000830064007b0356009703860401
-            007c0264127a0d00007d027c02740e000000000000000000006b00000000
-            00720e7400000000000000000000009005af0c6400530064005300640053
-            0064005300
+            0300000000000000000000641fa6010000ab010000000000000000010074
+            03000000000000000000007c0fa6010000ab010000000000000000010074
+            0300000000000000000000641fa6010000ab010000000000000000010009
+            00743d000000000000000000007c0f740400000000000000000000a60200
+            00ab02000000000000000072537c0fa01f00000000000000000000000000
+            000000000000006426a6010000ab010000000000000000723e742f000000
+            000000000000006a1800000000000000007c0fa6010000ab010000000000
+            0000007d0f743d000000000000000000007c0f7404000000000000000000
+            00a6020000ab02000000000000000072157c0fa01f000000000000000000
+            00000000000000000000006426a6010000ab010000000000000000b03e7c
+            0f7d136e09230001007c0f7d1359006e03780359007701743d0000000000
+            00000000007c13744000000000000000000000a6020000ab020000000000
+            0000007230742f000000000000000000006a1b00000000000000007c0f64
+            016412ac27a6030000ab0300000000000000007d1464287c0f760072147c
+            0f64281900000000000000000064076b030000000072087c0f6428190000
+            000000000000007d146e27743d000000000000000000007c137404000000
+            00000000000000a6020000ab02000000000000000072037c137d146e0f74
+            05000000000000000000007c13a6010000ab0100000000000000007d1474
+            07000000000000000000006a0800000000000000007c0e7c1464296412ac
+            2aa6040000ab040000000000000000a01500000000000000000000000000
+            00000000000000a6000000ab000000000000000000830064007b03560097
+            03860401007c0264127a0d00007d027c02740e000000000000000000006b
+            0000000000720e7400000000000000000000009006af0d64005300640053
+            006400530064005300
           90           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
           92           6 LOAD_CONST               1 (False)
                        8 STORE_GLOBAL             0 (is_stop)
          
@@ -906,19 +923,19 @@
          
           99         240 LOAD_CONST               6 (0)
                      242 STORE_FAST               2 (cur_iter)
          
          100     >>  244 LOAD_FAST                2 (cur_iter)
                      246 LOAD_GLOBAL             14 (MAX_ITER)
                      258 COMPARE_OP               0 (<)
-                     264 EXTENDED_ARG             5
-                     266 POP_JUMP_FORWARD_IF_FALSE  1302 (to 2872)
+                     264 EXTENDED_ARG             6
+                     266 POP_JUMP_FORWARD_IF_FALSE  1559 (to 3386)
                      268 LOAD_GLOBAL              0 (is_stop)
-                     280 EXTENDED_ARG             5
-                     282 POP_JUMP_FORWARD_IF_TRUE  1296 (to 2876)
+                     280 EXTENDED_ARG             6
+                     282 POP_JUMP_FORWARD_IF_TRUE  1553 (to 3390)
          
          102     >>  284 LOAD_CONST               7 ('')
                      286 LOAD_CONST               7 ('')
                      288 LOAD_CONST               5 (('role', 'content'))
                      290 BUILD_CONST_KEY_MAP      2
                      292 STORE_FAST               3 (openai_message)
          
@@ -1493,64 +1510,181 @@
          
          202        2668 LOAD_GLOBAL              3 (NULL + print)
                     2680 LOAD_CONST               2 ('==================================')
                     2682 PRECALL                  1
                     2686 CALL                     1
                     2696 POP_TOP
          
-         204        2698 LOAD_GLOBAL              7 (NULL + cl)
-                    2710 LOAD_ATTR                8 (Message)
-         
-         205        2720 LOAD_FAST               14 (function_name)
-         
-         206        2722 LOAD_GLOBAL              5 (NULL + str)
-                    2734 LOAD_FAST               15 (function_response)
-                    2736 PRECALL                  1
-                    2740 CALL                     1
-         
-         207        2750 LOAD_CONST              38 ('json')
-         
-         208        2752 LOAD_CONST              18 (1)
-         
-         204        2754 KW_NAMES                39
-                    2756 PRECALL                  4
-                    2760 CALL                     4
-         
-         209        2770 LOAD_METHOD             21 (send)
-                    2792 PRECALL                  0
-                    2796 CALL                     0
-         
-         204        2806 GET_AWAITABLE            0
-                    2808 LOAD_CONST               0 (None)
-                 >> 2810 SEND                     3 (to 2818)
-                    2812 YIELD_VALUE
-                    2814 RESUME                   3
-                    2816 JUMP_BACKWARD_NO_INTERRUPT     4 (to 2810)
-                 >> 2818 POP_TOP
-         
-         210        2820 LOAD_FAST                2 (cur_iter)
-                    2822 LOAD_CONST              18 (1)
-                    2824 BINARY_OP               13 (+=)
-                    2828 STORE_FAST               2 (cur_iter)
-         
-         100        2830 LOAD_FAST                2 (cur_iter)
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
+         203        2698 LOAD_GLOBAL              3 (NULL + print)
+                    2710 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
+                    2712 PRECALL                  1
+                    2716 CALL                     1
+                    2726 POP_TOP
+         
+         204        2728 LOAD_GLOBAL              3 (NULL + print)
+                    2740 LOAD_FAST               15 (function_response)
+                    2742 PRECALL                  1
+                    2746 CALL                     1
+                    2756 POP_TOP
+         
+         205        2758 LOAD_GLOBAL              3 (NULL + print)
+                    2770 LOAD_CONST              31 ('🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀')
+                    2772 PRECALL                  1
+                    2776 CALL                     1
+                    2786 POP_TOP
+         
+         206        2788 NOP
+         
+         207        2790 LOAD_GLOBAL             61 (NULL + isinstance)
+                    2802 LOAD_FAST               15 (function_response)
+                    2804 LOAD_GLOBAL              4 (str)
+                    2816 PRECALL                  2
+                    2820 CALL                     2
+                    2830 POP_JUMP_FORWARD_IF_FALSE    83 (to 2998)
+                    2832 LOAD_FAST               15 (function_response)
+                    2834 LOAD_METHOD             31 (startswith)
+                    2856 LOAD_CONST              38 ('{')
+                    2858 PRECALL                  1
+                    2862 CALL                     1
+                    2872 POP_JUMP_FORWARD_IF_FALSE    62 (to 2998)
+         
+         208     >> 2874 LOAD_GLOBAL             47 (NULL + json)
+                    2886 LOAD_ATTR               24 (loads)
+                    2896 LOAD_FAST               15 (function_response)
+                    2898 PRECALL                  1
+                    2902 CALL                     1
+                    2912 STORE_FAST              15 (function_response)
+         
+         207        2914 LOAD_GLOBAL             61 (NULL + isinstance)
+                    2926 LOAD_FAST               15 (function_response)
+                    2928 LOAD_GLOBAL              4 (str)
+                    2940 PRECALL                  2
+                    2944 CALL                     2
+                    2954 POP_JUMP_FORWARD_IF_FALSE    21 (to 2998)
+                    2956 LOAD_FAST               15 (function_response)
+                    2958 LOAD_METHOD             31 (startswith)
+                    2980 LOAD_CONST              38 ('{')
+                    2982 PRECALL                  1
+                    2986 CALL                     1
+                    2996 POP_JUMP_BACKWARD_IF_TRUE    62 (to 2874)
+         
+         209     >> 2998 LOAD_FAST               15 (function_response)
+                    3000 STORE_FAST              19 (final_response)
+                    3002 JUMP_FORWARD             9 (to 3022)
+                 >> 3004 PUSH_EXC_INFO
+         
+         210        3006 POP_TOP
+         
+         211        3008 LOAD_FAST               15 (function_response)
+                    3010 STORE_FAST              19 (final_response)
+                    3012 POP_EXCEPT
+                    3014 JUMP_FORWARD             3 (to 3022)
+                 >> 3016 COPY                     3
+                    3018 POP_EXCEPT
+                    3020 RERAISE                  1
+         
+         213     >> 3022 LOAD_GLOBAL             61 (NULL + isinstance)
+                    3034 LOAD_FAST               19 (final_response)
+                    3036 LOAD_GLOBAL             64 (dict)
+                    3048 PRECALL                  2
+                    3052 CALL                     2
+                    3062 POP_JUMP_FORWARD_IF_FALSE    48 (to 3160)
+         
+         215        3064 LOAD_GLOBAL             47 (NULL + json)
+                    3076 LOAD_ATTR               27 (dumps)
+                    3086 LOAD_FAST               15 (function_response)
+                    3088 LOAD_CONST               1 (False)
+                    3090 LOAD_CONST              18 (1)
+                    3092 KW_NAMES                39
+                    3094 PRECALL                  3
+                    3098 CALL                     3
+                    3108 STORE_FAST              20 (content)
+         
+         216        3110 LOAD_CONST              40 ('output')
+                    3112 LOAD_FAST               15 (function_response)
+                    3114 CONTAINS_OP              0
+                    3116 POP_JUMP_FORWARD_IF_FALSE    20 (to 3158)
+         
+         217        3118 LOAD_FAST               15 (function_response)
+                    3120 LOAD_CONST              40 ('output')
+                    3122 BINARY_SUBSCR
+                    3132 LOAD_CONST               7 ('')
+                    3134 COMPARE_OP               3 (!=)
+                    3140 POP_JUMP_FORWARD_IF_FALSE     8 (to 3158)
+         
+         218        3142 LOAD_FAST               15 (function_response)
+                    3144 LOAD_CONST              40 ('output')
+                    3146 BINARY_SUBSCR
+                    3156 STORE_FAST              20 (content)
+                 >> 3158 JUMP_FORWARD            39 (to 3238)
+         
+         219     >> 3160 LOAD_GLOBAL             61 (NULL + isinstance)
+                    3172 LOAD_FAST               19 (final_response)
+                    3174 LOAD_GLOBAL              4 (str)
+                    3186 PRECALL                  2
+                    3190 CALL                     2
+                    3200 POP_JUMP_FORWARD_IF_FALSE     3 (to 3208)
+         
+         221        3202 LOAD_FAST               19 (final_response)
+                    3204 STORE_FAST              20 (content)
+                    3206 JUMP_FORWARD            15 (to 3238)
+         
+         224     >> 3208 LOAD_GLOBAL              5 (NULL + str)
+                    3220 LOAD_FAST               19 (final_response)
+                    3222 PRECALL                  1
+                    3226 CALL                     1
+                    3236 STORE_FAST              20 (content)
+         
+         225     >> 3238 LOAD_GLOBAL              7 (NULL + cl)
+                    3250 LOAD_ATTR                8 (Message)
+         
+         226        3260 LOAD_FAST               14 (function_name)
+         
+         227        3262 LOAD_FAST               20 (content)
+         
+         228        3264 LOAD_CONST              41 ('markdown')
+         
+         229        3266 LOAD_CONST              18 (1)
+         
+         225        3268 KW_NAMES                42
+                    3270 PRECALL                  4
+                    3274 CALL                     4
+         
+         230        3284 LOAD_METHOD             21 (send)
+                    3306 PRECALL                  0
+                    3310 CALL                     0
+         
+         225        3320 GET_AWAITABLE            0
+                    3322 LOAD_CONST               0 (None)
+                 >> 3324 SEND                     3 (to 3332)
+                    3326 YIELD_VALUE
+                    3328 RESUME                   3
+                    3330 JUMP_BACKWARD_NO_INTERRUPT     4 (to 3324)
+                 >> 3332 POP_TOP
+         
+         232        3334 LOAD_FAST                2 (cur_iter)
+                    3336 LOAD_CONST              18 (1)
+                    3338 BINARY_OP               13 (+=)
+                    3342 STORE_FAST               2 (cur_iter)
+         
+         100        3344 LOAD_FAST                2 (cur_iter)
+                    3346 LOAD_GLOBAL             14 (MAX_ITER)
+                    3358 COMPARE_OP               0 (<)
+                    3364 POP_JUMP_FORWARD_IF_FALSE    14 (to 3394)
+                    3366 LOAD_GLOBAL              0 (is_stop)
+                    3378 EXTENDED_ARG             6
+                    3380 POP_JUMP_BACKWARD_IF_FALSE  1549 (to 284)
+                    3382 LOAD_CONST               0 (None)
+                    3384 RETURN_VALUE
+                 >> 3386 LOAD_CONST               0 (None)
+                    3388 RETURN_VALUE
+                 >> 3390 LOAD_CONST               0 (None)
+                    3392 RETURN_VALUE
+                 >> 3394 LOAD_CONST               0 (None)
+                    3396 RETURN_VALUE
          ExceptionTable:
            376 to 840 -> 844 [0]
            844 to 862 -> 978 [1] lasti
            864 to 954 -> 968 [1] lasti
            968 to 976 -> 978 [1] lasti
            1414 to 1528 -> 1532 [0]
            1532 to 1534 -> 1856 [1] lasti
@@ -1558,14 +1692,16 @@
            1654 to 1654 -> 1856 [1] lasti
            1656 to 1840 -> 1846 [2] lasti
            1842 to 1850 -> 1856 [1] lasti
            1864 to 1928 -> 1932 [0]
            1932 to 1950 -> 1996 [1] lasti
            1952 to 1984 -> 1986 [1] lasti
            1986 to 1994 -> 1996 [1] lasti
+           2790 to 3000 -> 3004 [0]
+           3004 to 3010 -> 3016 [1] lasti
          consts
             None
             False
             '=================================='
             'message_history'
             'user'
             ('role', 'content')
@@ -1597,32 +1733,37 @@
             '🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀'
             'description'
             'function'
             ('role', 'name', 'content')
             'language'
             '\n\n'
             'Please answer me in '
-            'json'
+            '{'
+            ('ensure_ascii', 'indent')
+            'output'
+            'markdown'
             ('author', 'content', 'language', 'indent')
-         names      ('is_stop', 'print', 'str', 'cl', 'user_session', 'get', 'append', 'MAX_ITER', 'Message', '__truncate_conversation', 'function_manager', 'generate_functions_array', 'openai', 'ChatCompletion', 'create', 'config_env', 'choices', 'process_new_delta', 'Exception', 'asyncio', 'sleep', 'send', 'ValueError', 'json', 'loads', 'ast', 'literal_eval', 'dumps', 'call_function', 'type')
-         varnames   ('user_message', 'message_history', 'cur_iter', 'openai_message', 'function_ui_message', 'content_ui_message', 'stream_resp', 'send_message', 'functions', 'user_plugin_api_info', 'item', 'i', 'new_delta', 'e', 'function_name', 'function_response', 'arguments', 'description', 'language')
+         names      ('is_stop', 'print', 'str', 'cl', 'user_session', 'get', 'append', 'MAX_ITER', 'Message', '__truncate_conversation', 'function_manager', 'generate_functions_array', 'openai', 'ChatCompletion', 'create', 'config_env', 'choices', 'process_new_delta', 'Exception', 'asyncio', 'sleep', 'send', 'ValueError', 'json', 'loads', 'ast', 'literal_eval', 'dumps', 'call_function', 'type', 'isinstance', 'startswith', 'dict')
+         varnames   ('user_message', 'message_history', 'cur_iter', 'openai_message', 'function_ui_message', 'content_ui_message', 'stream_resp', 'send_message', 'functions', 'user_plugin_api_info', 'item', 'i', 'new_delta', 'e', 'function_name', 'function_response', 'arguments', 'description', 'language', 'final_response', 'content')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
          name       'on_message'
          firstlineno 90
          lnotab
             0x060204011e011e011e011e013e013001040128020a0104012a0104011e
             01020132013e010401080114012cff020220012c01240102010201020102
             0102fa160726010e0104010e0104010c0108ff2a0212011e010a01340114
             fc0806040134010402040134022e0104012e014002500144010401020116
             014eff14020201020116014eff1402020118010c01040154014e01020122
             0104ff200212011e010cfe08031e011e0130011e022a0224021e01280110
             01060118010201020126fd14052601180102012efe140420021801020102
-            0102fd14061e011e011e02160102011c01020102fc100524fb0e060a92
+            0102fd14061e011e011e011e011e011e010201540128ff5402080102010e
+            022a022e010801180112012a0206031e01160102010201020102fc100524
+            fb0e070a8000fc
       code
          argcount  : 4
          nlocals   : 6
          stacksize : 6
          flags     : 131
          code
             0x4b000100970064017c007600720b7c006401190000000000000000007c
@@ -1643,206 +1784,206 @@
             0000007601720b64037c01640419000000000000000000640b3c0000007c
             01640419000000000000000000640b78027802190000000000000000007c
             00640419000000000000000000640b190000000000000000007a0d000063
             0363023c0000007c03a00100000000000000000000000000000000000000
             007c00640419000000000000000000640b19000000000000000000a60100
             00ab010000000000000000830064007b0356009703860401007c017c027c
             0366035300
-         213           0 RETURN_GENERATOR
+         235           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         215           6 LOAD_CONST               1 ('role')
+         237           6 LOAD_CONST               1 ('role')
                        8 LOAD_FAST                0 (new_delta)
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    11 (to 36)
          
-         216          14 LOAD_FAST                0 (new_delta)
+         238          14 LOAD_FAST                0 (new_delta)
                       16 LOAD_CONST               1 ('role')
                       18 BINARY_SUBSCR
                       28 LOAD_FAST                1 (openai_message)
                       30 LOAD_CONST               1 ('role')
                       32 STORE_SUBSCR
          
-         217     >>   36 LOAD_CONST               2 ('content')
+         239     >>   36 LOAD_CONST               2 ('content')
                       38 LOAD_FAST                0 (new_delta)
                       40 CONTAINS_OP              0
                       42 POP_JUMP_FORWARD_IF_FALSE    66 (to 176)
          
-         218          44 LOAD_FAST                0 (new_delta)
+         240          44 LOAD_FAST                0 (new_delta)
                       46 LOAD_METHOD              0 (get)
                       68 LOAD_CONST               2 ('content')
                       70 PRECALL                  1
                       74 CALL                     1
                       84 JUMP_IF_TRUE_OR_POP      1 (to 88)
                       86 LOAD_CONST               3 ('')
                  >>   88 STORE_FAST               4 (new_content)
          
-         219          90 LOAD_FAST                1 (openai_message)
+         241          90 LOAD_FAST                1 (openai_message)
                       92 LOAD_CONST               2 ('content')
                       94 COPY                     2
                       96 COPY                     2
                       98 BINARY_SUBSCR
                      108 LOAD_FAST                4 (new_content)
                      110 BINARY_OP               13 (+=)
                      114 SWAP                     3
                      116 SWAP                     2
                      118 STORE_SUBSCR
          
-         220         122 LOAD_FAST                2 (content_ui_message)
+         242         122 LOAD_FAST                2 (content_ui_message)
                      124 LOAD_METHOD              1 (stream_token)
                      146 LOAD_FAST                4 (new_content)
                      148 PRECALL                  1
                      152 CALL                     1
                      162 GET_AWAITABLE            0
                      164 LOAD_CONST               0 (None)
                  >>  166 SEND                     3 (to 174)
                      168 YIELD_VALUE
                      170 RESUME                   3
                      172 JUMP_BACKWARD_NO_INTERRUPT     4 (to 166)
                  >>  174 POP_TOP
          
-         221     >>  176 LOAD_CONST               4 ('function_call')
+         243     >>  176 LOAD_CONST               4 ('function_call')
                      178 LOAD_FAST                0 (new_delta)
                      180 CONTAINS_OP              0
                      182 POP_JUMP_FORWARD_IF_FALSE   220 (to 624)
          
-         222         184 LOAD_CONST               5 ('name')
+         244         184 LOAD_CONST               5 ('name')
                      186 LOAD_FAST                0 (new_delta)
                      188 LOAD_CONST               4 ('function_call')
                      190 BINARY_SUBSCR
                      200 CONTAINS_OP              0
                      202 POP_JUMP_FORWARD_IF_FALSE   106 (to 416)
          
-         223         204 LOAD_FAST                0 (new_delta)
+         245         204 LOAD_FAST                0 (new_delta)
                      206 LOAD_CONST               4 ('function_call')
                      208 BINARY_SUBSCR
                      218 LOAD_CONST               5 ('name')
                      220 BINARY_SUBSCR
                      230 STORE_FAST               5 (function_name)
          
-         224         232 LOAD_FAST                5 (function_name)
+         246         232 LOAD_FAST                5 (function_name)
                      234 LOAD_CONST               6 ('python')
                      236 COMPARE_OP               2 (==)
                      242 POP_JUMP_FORWARD_IF_FALSE     2 (to 248)
          
-         225         244 LOAD_CONST               7 ('python_exec')
+         247         244 LOAD_CONST               7 ('python_exec')
                      246 STORE_FAST               5 (function_name)
          
-         227     >>  248 LOAD_CONST               5 ('name')
+         249     >>  248 LOAD_CONST               5 ('name')
                      250 LOAD_FAST                5 (function_name)
          
-         226         252 BUILD_MAP                1
+         248         252 BUILD_MAP                1
                      254 LOAD_FAST                1 (openai_message)
                      256 LOAD_CONST               4 ('function_call')
                      258 STORE_SUBSCR
          
-         229         262 LOAD_FAST                2 (content_ui_message)
+         251         262 LOAD_FAST                2 (content_ui_message)
                      264 LOAD_METHOD              2 (send)
                      286 PRECALL                  0
                      290 CALL                     0
                      300 GET_AWAITABLE            0
                      302 LOAD_CONST               0 (None)
                  >>  304 SEND                     3 (to 312)
                      306 YIELD_VALUE
                      308 RESUME                   3
                      310 JUMP_BACKWARD_NO_INTERRUPT     4 (to 304)
                  >>  312 POP_TOP
          
-         230         314 LOAD_GLOBAL              7 (NULL + cl)
+         252         314 LOAD_GLOBAL              7 (NULL + cl)
                      326 LOAD_ATTR                4 (Message)
          
-         231         336 LOAD_FAST                5 (function_name)
+         253         336 LOAD_FAST                5 (function_name)
          
-         232         338 LOAD_CONST               3 ('')
+         254         338 LOAD_CONST               3 ('')
          
-         233         340 LOAD_CONST               8 (1)
+         255         340 LOAD_CONST               8 (1)
          
-         234         342 LOAD_CONST               9 ('json')
+         256         342 LOAD_CONST               9 ('json')
          
-         230         344 KW_NAMES                10
+         252         344 KW_NAMES                10
                      346 PRECALL                  4
                      350 CALL                     4
                      360 STORE_FAST               3 (function_ui_message)
          
-         235         362 LOAD_FAST                3 (function_ui_message)
+         257         362 LOAD_FAST                3 (function_ui_message)
                      364 LOAD_METHOD              1 (stream_token)
                      386 LOAD_FAST                5 (function_name)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 GET_AWAITABLE            0
                      404 LOAD_CONST               0 (None)
                  >>  406 SEND                     3 (to 414)
                      408 YIELD_VALUE
                      410 RESUME                   3
                      412 JUMP_BACKWARD_NO_INTERRUPT     4 (to 406)
                  >>  414 POP_TOP
          
-         237     >>  416 LOAD_CONST              11 ('arguments')
+         259     >>  416 LOAD_CONST              11 ('arguments')
                      418 LOAD_FAST                0 (new_delta)
                      420 LOAD_CONST               4 ('function_call')
                      422 BINARY_SUBSCR
                      432 CONTAINS_OP              0
                      434 POP_JUMP_FORWARD_IF_FALSE    94 (to 624)
          
-         238         436 LOAD_CONST              11 ('arguments')
+         260         436 LOAD_CONST              11 ('arguments')
                      438 LOAD_FAST                1 (openai_message)
                      440 LOAD_CONST               4 ('function_call')
                      442 BINARY_SUBSCR
                      452 CONTAINS_OP              1
                      454 POP_JUMP_FORWARD_IF_FALSE    11 (to 478)
          
-         239         456 LOAD_CONST               3 ('')
+         261         456 LOAD_CONST               3 ('')
                      458 LOAD_FAST                1 (openai_message)
                      460 LOAD_CONST               4 ('function_call')
                      462 BINARY_SUBSCR
                      472 LOAD_CONST              11 ('arguments')
                      474 STORE_SUBSCR
          
-         240     >>  478 LOAD_FAST                1 (openai_message)
+         262     >>  478 LOAD_FAST                1 (openai_message)
                      480 LOAD_CONST               4 ('function_call')
                      482 BINARY_SUBSCR
                      492 LOAD_CONST              11 ('arguments')
                      494 COPY                     2
                      496 COPY                     2
                      498 BINARY_SUBSCR
                      508 LOAD_FAST                0 (new_delta)
          
-         241         510 LOAD_CONST               4 ('function_call')
+         263         510 LOAD_CONST               4 ('function_call')
          
-         240         512 BINARY_SUBSCR
+         262         512 BINARY_SUBSCR
          
-         241         522 LOAD_CONST              11 ('arguments')
+         263         522 LOAD_CONST              11 ('arguments')
          
-         240         524 BINARY_SUBSCR
+         262         524 BINARY_SUBSCR
                      534 BINARY_OP               13 (+=)
                      538 SWAP                     3
                      540 SWAP                     2
                      542 STORE_SUBSCR
          
-         242         546 LOAD_FAST                3 (function_ui_message)
+         264         546 LOAD_FAST                3 (function_ui_message)
                      548 LOAD_METHOD              1 (stream_token)
          
-         243         570 LOAD_FAST                0 (new_delta)
+         265         570 LOAD_FAST                0 (new_delta)
                      572 LOAD_CONST               4 ('function_call')
                      574 BINARY_SUBSCR
                      584 LOAD_CONST              11 ('arguments')
                      586 BINARY_SUBSCR
          
-         242         596 PRECALL                  1
+         264         596 PRECALL                  1
                      600 CALL                     1
                      610 GET_AWAITABLE            0
                      612 LOAD_CONST               0 (None)
                  >>  614 SEND                     3 (to 622)
                      616 YIELD_VALUE
                      618 RESUME                   3
                      620 JUMP_BACKWARD_NO_INTERRUPT     4 (to 614)
                  >>  622 POP_TOP
          
-         244     >>  624 LOAD_FAST                1 (openai_message)
+         266     >>  624 LOAD_FAST                1 (openai_message)
                      626 LOAD_FAST                2 (content_ui_message)
                      628 LOAD_FAST                3 (function_ui_message)
                      630 BUILD_TUPLE              3
                      632 RETURN_VALUE
          consts
             None
             'role'
@@ -1858,114 +1999,298 @@
             'arguments'
          names      ('get', 'stream_token', 'send', 'cl', 'Message')
          varnames   ('new_delta', 'openai_message', 'content_ui_message', 'function_ui_message', 'new_content', 'function_name')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
          name       'process_new_delta'
-         firstlineno 213
+         firstlineno 235
          lnotab
             0x06020801160108012e0120013601080114011c010c01040204ff0a0334
             01160102010201020102fc12053602140114011601200102ff0a0102ff16
             0218011aff1c02
       code
          argcount  : 0
-         nlocals   : 4
+         nlocals   : 8
          stacksize : 6
          flags     : 131
          code
-            0x4b00010097007400000000000000000000006401190000000000000000
-            006402190000000000000000007d007403000000000000000000006a0200
-            00000000000000a6000000ab0000000000000000007d016403a003000000
-            00000000000000000000000000000000007c017c00ac04a6020000ab0200
-            000000000000007d02740000000000000000000000640119000000000000
-            0000006405190000000000000000007d037408000000000000000000006a
-            050000000000000000a00600000000000000000000000000000000000000
-            00640664077c0264087a00000064097a0000007c037a000000640a9c0267
-            01a6020000ab020000000000000000010064005300
-         248           0 RETURN_GENERATOR
+            0x4b00010097007400000000000000000000006a010000000000000000a0
+            0200000000000000000000000000000000000000006401a6010000ab0100
+            000000000000007d007c0080407407000000000000000000007409000000
+            000000000000006a050000000000000000a6000000ab0000000000000000
+            00a6010000ab0100000000000000007d007400000000000000000000006a
+            010000000000000000a00600000000000000000000000000000000000000
+            0064017c00a6020000ab0200000000000000000100740000000000000000
+            0000006a010000000000000000a002000000000000000000000000000000
+            00000000006402a6010000ab0100000000000000007d0174000000000000
+            00000000006a010000000000000000a00200000000000000000000000000
+            000000000000006403a6010000ab0100000000000000007d027400000000
+            000000000000006a010000000000000000a0020000000000000000000000
+            0000000000000000006404a6010000ab0100000000000000007d037c0380
+            547401000000000000000000006a0700000000000000006405a6010000ab
+            010000000000000000a00800000000000000000000000000000000000000
+            00a6000000ab000000000000000000830064007b035600970386047d047c
+            046406190000000000000000007d037400000000000000000000006a0100
+            00000000000000a006000000000000000000000000000000000000000064
+            047c03a6020000ab02000000000000000001007c01805474010000000000
+            00000000006a0700000000000000006407a6010000ab0100000000000000
+            00a0080000000000000000000000000000000000000000a6000000ab0000
+            00000000000000830064007b035600970386047d047c0464061900000000
+            00000000007d017400000000000000000000006a010000000000000000a0
+            06000000000000000000000000000000000000000064027c01a6020000ab
+            02000000000000000001007c0280547401000000000000000000006a0700
+            000000000000006408a6010000ab010000000000000000a0080000000000
+            000000000000000000000000000000a6000000ab00000000000000000083
+            0064007b035600970386047d047c046406190000000000000000007d0274
+            00000000000000000000006a010000000000000000a00600000000000000
+            0000000000000000000000000064037c02a6020000ab0200000000000000
+            0001007413000000000000000000006a0a0000000000000000a6000000ab
+            0000000000000000007d056409a00b000000000000000000000000000000
+            00000000007c057c02ac0aa6020000ab0200000000000000007d06741800
+            000000000000000000640b19000000000000000000640c19000000000000
+            0000007d077400000000000000000000006a010000000000000000a00600
+            00000000000000000000000000000000000000640d640e7c06640f7a0000
+            0064107a0000007c077a00000064119c026701a6020000ab020000000000
+            000000010064005300
+         270           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         250           6 LOAD_GLOBAL              0 (config_env)
-                      18 LOAD_CONST               1 ('openai')
-                      20 BINARY_SUBSCR
-                      30 LOAD_CONST               2 ('password')
-                      32 BINARY_SUBSCR
-                      42 STORE_FAST               0 (password)
-         
-         251          44 LOAD_GLOBAL              3 (NULL + platform)
-                      56 LOAD_ATTR                2 (system)
-                      66 PRECALL                  0
-                      70 CALL                     0
-                      80 STORE_FAST               1 (platform_name)
-         
-         252          82 LOAD_CONST               3 ('You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\n')
-         
-         266          84 LOAD_METHOD              3 (format)
-                     106 LOAD_FAST                1 (platform_name)
-                     108 LOAD_FAST                0 (password)
-                     110 KW_NAMES                 4
-                     112 PRECALL                  2
-                     116 CALL                     2
+         273           6 LOAD_GLOBAL              0 (cl)
+                      18 LOAD_ATTR                1 (user_session)
+                      28 LOAD_METHOD              2 (get)
+                      50 LOAD_CONST               1 ('user_id')
+                      52 PRECALL                  1
+                      56 CALL                     1
+                      66 STORE_FAST               0 (user_id)
+         
+         274          68 LOAD_FAST                0 (user_id)
+                      70 POP_JUMP_FORWARD_IF_NOT_NONE    64 (to 200)
+         
+         275          72 LOAD_GLOBAL              7 (NULL + str)
+                      84 LOAD_GLOBAL              9 (NULL + uuid)
+                      96 LOAD_ATTR                5 (uuid4)
+                     106 PRECALL                  0
+                     110 CALL                     0
+                     120 PRECALL                  1
+                     124 CALL                     1
+                     134 STORE_FAST               0 (user_id)
+         
+         276         136 LOAD_GLOBAL              0 (cl)
+                     148 LOAD_ATTR                1 (user_session)
+                     158 LOAD_METHOD              6 (set)
+                     180 LOAD_CONST               1 ('user_id')
+                     182 LOAD_FAST                0 (user_id)
+                     184 PRECALL                  2
+                     188 CALL                     2
+                     198 POP_TOP
+         
+         277     >>  200 LOAD_GLOBAL              0 (cl)
+                     212 LOAD_ATTR                1 (user_session)
+                     222 LOAD_METHOD              2 (get)
+                     244 LOAD_CONST               2 ('username')
+                     246 PRECALL                  1
+                     250 CALL                     1
+                     260 STORE_FAST               1 (username)
+         
+         278         262 LOAD_GLOBAL              0 (cl)
+                     274 LOAD_ATTR                1 (user_session)
+                     284 LOAD_METHOD              2 (get)
+                     306 LOAD_CONST               3 ('password')
+                     308 PRECALL                  1
+                     312 CALL                     1
+                     322 STORE_FAST               2 (password)
+         
+         279         324 LOAD_GLOBAL              0 (cl)
+                     336 LOAD_ATTR                1 (user_session)
+                     346 LOAD_METHOD              2 (get)
+                     368 LOAD_CONST               4 ('hostname')
+                     370 PRECALL                  1
+                     374 CALL                     1
+                     384 STORE_FAST               3 (hostname)
+         
+         280         386 LOAD_FAST                3 (hostname)
+                     388 POP_JUMP_FORWARD_IF_NOT_NONE    84 (to 558)
+         
+         281         390 LOAD_GLOBAL              1 (NULL + cl)
+                     402 LOAD_ATTR                7 (AskUserMessage)
+                     412 LOAD_CONST               5 ('请输入需要连接的终端的IP地址')
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 LOAD_METHOD              8 (send)
+                     450 PRECALL                  0
+                     454 CALL                     0
+                     464 GET_AWAITABLE            0
+                     466 LOAD_CONST               0 (None)
+                 >>  468 SEND                     3 (to 476)
+                     470 YIELD_VALUE
+                     472 RESUME                   3
+                     474 JUMP_BACKWARD_NO_INTERRUPT     4 (to 468)
+                 >>  476 STORE_FAST               4 (res)
          
-         252         126 STORE_FAST               2 (content)
+         282         478 LOAD_FAST                4 (res)
+                     480 LOAD_CONST               6 ('content')
+                     482 BINARY_SUBSCR
+                     492 STORE_FAST               3 (hostname)
          
-         267         128 LOAD_GLOBAL              0 (config_env)
-                     140 LOAD_CONST               1 ('openai')
-                     142 BINARY_SUBSCR
-                     152 LOAD_CONST               5 ('language')
-                     154 BINARY_SUBSCR
-                     164 STORE_FAST               3 (language)
-         
-         268         166 LOAD_GLOBAL              8 (cl)
-                     178 LOAD_ATTR                5 (user_session)
-                     188 LOAD_METHOD              6 (set)
-         
-         269         210 LOAD_CONST               6 ('message_history')
-         
-         272         212 LOAD_CONST               7 ('system')
-         
-         273         214 LOAD_FAST                2 (content)
-                     216 LOAD_CONST               8 ('\n\n')
-                     218 BINARY_OP                0 (+)
-                     222 LOAD_CONST               9 ('Please answer me in ')
-                     224 BINARY_OP                0 (+)
-                     228 LOAD_FAST                3 (language)
-                     230 BINARY_OP                0 (+)
-         
-         270         234 LOAD_CONST              10 (('role', 'content'))
-                     236 BUILD_CONST_KEY_MAP      2
-                     238 BUILD_LIST               1
-         
-         268         240 PRECALL                  2
-                     244 CALL                     2
-                     254 POP_TOP
-                     256 LOAD_CONST               0 (None)
-                     258 RETURN_VALUE
+         283         494 LOAD_GLOBAL              0 (cl)
+                     506 LOAD_ATTR                1 (user_session)
+                     516 LOAD_METHOD              6 (set)
+                     538 LOAD_CONST               4 ('hostname')
+                     540 LOAD_FAST                3 (hostname)
+                     542 PRECALL                  2
+                     546 CALL                     2
+                     556 POP_TOP
+         
+         284     >>  558 LOAD_FAST                1 (username)
+                     560 POP_JUMP_FORWARD_IF_NOT_NONE    84 (to 730)
+         
+         285         562 LOAD_GLOBAL              1 (NULL + cl)
+                     574 LOAD_ATTR                7 (AskUserMessage)
+                     584 LOAD_CONST               7 ('请输入需要连接的终端的用户名')
+                     586 PRECALL                  1
+                     590 CALL                     1
+                     600 LOAD_METHOD              8 (send)
+                     622 PRECALL                  0
+                     626 CALL                     0
+                     636 GET_AWAITABLE            0
+                     638 LOAD_CONST               0 (None)
+                 >>  640 SEND                     3 (to 648)
+                     642 YIELD_VALUE
+                     644 RESUME                   3
+                     646 JUMP_BACKWARD_NO_INTERRUPT     4 (to 640)
+                 >>  648 STORE_FAST               4 (res)
+         
+         286         650 LOAD_FAST                4 (res)
+                     652 LOAD_CONST               6 ('content')
+                     654 BINARY_SUBSCR
+                     664 STORE_FAST               1 (username)
+         
+         287         666 LOAD_GLOBAL              0 (cl)
+                     678 LOAD_ATTR                1 (user_session)
+                     688 LOAD_METHOD              6 (set)
+                     710 LOAD_CONST               2 ('username')
+                     712 LOAD_FAST                1 (username)
+                     714 PRECALL                  2
+                     718 CALL                     2
+                     728 POP_TOP
+         
+         288     >>  730 LOAD_FAST                2 (password)
+                     732 POP_JUMP_FORWARD_IF_NOT_NONE    84 (to 902)
+         
+         289         734 LOAD_GLOBAL              1 (NULL + cl)
+                     746 LOAD_ATTR                7 (AskUserMessage)
+                     756 LOAD_CONST               8 ('输入需要连接的终端的密码')
+                     758 PRECALL                  1
+                     762 CALL                     1
+                     772 LOAD_METHOD              8 (send)
+                     794 PRECALL                  0
+                     798 CALL                     0
+                     808 GET_AWAITABLE            0
+                     810 LOAD_CONST               0 (None)
+                 >>  812 SEND                     3 (to 820)
+                     814 YIELD_VALUE
+                     816 RESUME                   3
+                     818 JUMP_BACKWARD_NO_INTERRUPT     4 (to 812)
+                 >>  820 STORE_FAST               4 (res)
+         
+         290         822 LOAD_FAST                4 (res)
+                     824 LOAD_CONST               6 ('content')
+                     826 BINARY_SUBSCR
+                     836 STORE_FAST               2 (password)
+         
+         291         838 LOAD_GLOBAL              0 (cl)
+                     850 LOAD_ATTR                1 (user_session)
+                     860 LOAD_METHOD              6 (set)
+                     882 LOAD_CONST               3 ('password')
+                     884 LOAD_FAST                2 (password)
+                     886 PRECALL                  2
+                     890 CALL                     2
+                     900 POP_TOP
+         
+         292     >>  902 LOAD_GLOBAL             19 (NULL + platform)
+                     914 LOAD_ATTR               10 (system)
+                     924 PRECALL                  0
+                     928 CALL                     0
+                     938 STORE_FAST               5 (platform_name)
+         
+         293         940 LOAD_CONST               9 ('You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n')
+         
+         312         942 LOAD_METHOD             11 (format)
+                     964 LOAD_FAST                5 (platform_name)
+                     966 LOAD_FAST                2 (password)
+                     968 KW_NAMES                10
+                     970 PRECALL                  2
+                     974 CALL                     2
+         
+         293         984 STORE_FAST               6 (content)
+         
+         313         986 LOAD_GLOBAL             24 (config_env)
+                     998 LOAD_CONST              11 ('openai')
+                    1000 BINARY_SUBSCR
+                    1010 LOAD_CONST              12 ('language')
+                    1012 BINARY_SUBSCR
+                    1022 STORE_FAST               7 (language)
+         
+         314        1024 LOAD_GLOBAL              0 (cl)
+                    1036 LOAD_ATTR                1 (user_session)
+                    1046 LOAD_METHOD              6 (set)
+         
+         315        1068 LOAD_CONST              13 ('message_history')
+         
+         318        1070 LOAD_CONST              14 ('system')
+         
+         319        1072 LOAD_FAST                6 (content)
+                    1074 LOAD_CONST              15 ('\n\n')
+                    1076 BINARY_OP                0 (+)
+                    1080 LOAD_CONST              16 ('Please answer me in ')
+                    1082 BINARY_OP                0 (+)
+                    1086 LOAD_FAST                7 (language)
+                    1088 BINARY_OP                0 (+)
+         
+         316        1092 LOAD_CONST              17 (('role', 'content'))
+                    1094 BUILD_CONST_KEY_MAP      2
+                    1096 BUILD_LIST               1
+         
+         314        1098 PRECALL                  2
+                    1102 CALL                     2
+                    1112 POP_TOP
+                    1114 LOAD_CONST               0 (None)
+                    1116 RETURN_VALUE
          consts
             None
-            'openai'
+            'user_id'
+            'username'
             'password'
-            'You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\n'
+            'hostname'
+            '请输入需要连接的终端的IP地址'
+            'content'
+            '请输入需要连接的终端的用户名'
+            '输入需要连接的终端的密码'
+            'You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.\nIf you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. \nNo command should generate any terminal input.\nThe {platform_name} user name is luzhipeng and the password is "{password}" \n[IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.\nexample:\nif the command is "sudo apt-get install zerotier-cli", you need to change it to "echo \'{password}\' | sudo -S apt-get install zerotier-cli"\nif the command does not need to be executed as root, you can directly execute the command,like "ls"    \nthe terminal function argumets like this:\n```json\n{{\n    "cmd": "ls",\n}}\n```\nor like this:\n```json\n{{\n    "cmd": "echo \'{password}\' | sudo -S apt-get install zerotier-cli",\n}}\n'
             ('platform_name', 'password')
+            'openai'
             'language'
             'message_history'
             'system'
             '\n\n'
             'Please answer me in '
             ('role', 'content')
-         names      ('config_env', 'platform', 'system', 'format', 'cl', 'user_session', 'set')
-         varnames   ('password', 'platform_name', 'content', 'language')
+         names      ('cl', 'user_session', 'get', 'str', 'uuid', 'uuid4', 'set', 'AskUserMessage', 'send', 'platform', 'system', 'format', 'config_env')
+         varnames   ('user_id', 'username', 'password', 'hostname', 'res', 'platform_name', 'content', 'language')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
          name       'start_chat'
-         firstlineno 248
-         lnotab 0x060226012601020e2af2020f26012c010203020114fd06fe
+         firstlineno 270
+         lnotab
+            0x06033e010401400140013e013e013e0104015801100140010401580110
+            0140010401580110014001260102132aed021426012c010203020114fd06
+            fe
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 7
          flags     : 131
          code
             0x4b000100970064017401000000000000000000007c00a6010000ab0100
@@ -1990,112 +2315,112 @@
             0000000000000000006411190000000000000000007d08740b0000000000
             00000000006a10000000000000000064127423000000000000000000007c
             086413a6020000ab0200000000000000009b0064147c039b009d03ac15a6
             020000ab020000000000000000a007000000000000000000000000000000
             0000000000a6000000ab000000000000000000830064007b035600970386
             040100640053007425000000000000000000007c00a6010000ab01000000
             0000000000830064007b03560097038604010064005300
-         278           0 RETURN_GENERATOR
+         324           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         280           6 LOAD_CONST               1 ('/upload')
+         326           6 LOAD_CONST               1 ('/upload')
                        8 LOAD_GLOBAL              1 (NULL + str)
                       20 LOAD_FAST                0 (user_message)
                       22 PRECALL                  1
                       26 CALL                     1
                       36 COMPARE_OP               2 (==)
                       42 EXTENDED_ARG             1
                       44 POP_JUMP_FORWARD_IF_FALSE   340 (to 726)
          
-         281          46 LOAD_GLOBAL              2 (os)
+         327          46 LOAD_GLOBAL              2 (os)
                       58 LOAD_ATTR                2 (path)
                       68 LOAD_METHOD              3 (exists)
                       90 LOAD_CONST               2 ('./tmp')
                       92 PRECALL                  1
                       96 CALL                     1
                      106 POP_JUMP_FORWARD_IF_TRUE    20 (to 148)
          
-         282         108 LOAD_GLOBAL              3 (NULL + os)
+         328         108 LOAD_GLOBAL              3 (NULL + os)
                      120 LOAD_ATTR                4 (mkdir)
                      130 LOAD_CONST               2 ('./tmp')
                      132 PRECALL                  1
                      136 CALL                     1
                      146 POP_TOP
          
-         283     >>  148 LOAD_GLOBAL             11 (NULL + cl)
+         329     >>  148 LOAD_GLOBAL             11 (NULL + cl)
                      160 LOAD_ATTR                6 (AskFileMessage)
          
-         284         170 LOAD_CONST               3 ('Please upload a file.')
+         330         170 LOAD_CONST               3 ('Please upload a file.')
          
-         285         172 LOAD_CONST               4 (10)
+         331         172 LOAD_CONST               4 (10)
          
-         287         174 LOAD_CONST               5 ('*')
+         333         174 LOAD_CONST               5 ('*')
          
-         286         176 BUILD_LIST               1
+         332         176 BUILD_LIST               1
          
-         283         178 KW_NAMES                 6
+         329         178 KW_NAMES                 6
                      180 PRECALL                  3
                      184 CALL                     3
          
-         288         194 LOAD_METHOD              7 (send)
+         334         194 LOAD_METHOD              7 (send)
                      216 PRECALL                  0
                      220 CALL                     0
          
-         283         230 GET_AWAITABLE            0
+         329         230 GET_AWAITABLE            0
                      232 LOAD_CONST               0 (None)
                  >>  234 SEND                     3 (to 242)
                      236 YIELD_VALUE
                      238 RESUME                   3
                      240 JUMP_BACKWARD_NO_INTERRUPT     4 (to 234)
                  >>  242 STORE_FAST               1 (files)
          
-         289         244 LOAD_FAST                1 (files)
+         335         244 LOAD_FAST                1 (files)
                      246 LOAD_CONST               7 (0)
                      248 BINARY_SUBSCR
                      258 STORE_FAST               2 (file)
          
-         290         260 LOAD_CONST               8 ('')
+         336         260 LOAD_CONST               8 ('')
                      262 STORE_FAST               3 (save_path)
          
-         293         264 LOAD_FAST                3 (save_path)
+         339         264 LOAD_FAST                3 (save_path)
                      266 LOAD_CONST               8 ('')
                      268 COMPARE_OP               2 (==)
                      274 POP_JUMP_FORWARD_IF_FALSE     7 (to 290)
          
-         294         276 LOAD_FAST                2 (file)
+         340         276 LOAD_FAST                2 (file)
                      278 LOAD_ATTR                8 (name)
                      288 STORE_FAST               3 (save_path)
          
-         295     >>  290 LOAD_CONST               9 ('./tmp/')
+         341     >>  290 LOAD_CONST               9 ('./tmp/')
                      292 LOAD_FAST                3 (save_path)
                      294 FORMAT_VALUE             0
                      296 BUILD_STRING             2
                      298 STORE_FAST               4 (file_path)
          
-         297         300 LOAD_FAST                2 (file)
+         343         300 LOAD_FAST                2 (file)
                      302 LOAD_ATTR                9 (content)
                      312 STORE_FAST               5 (content)
          
-         300         314 LOAD_GLOBAL             21 (NULL + open)
+         346         314 LOAD_GLOBAL             21 (NULL + open)
                      326 LOAD_FAST                4 (file_path)
                      328 LOAD_CONST              10 ('wb')
                      330 PRECALL                  2
                      334 CALL                     2
                      344 BEFORE_WITH
                      346 STORE_FAST               6 (f)
          
-         301         348 LOAD_FAST                6 (f)
+         347         348 LOAD_FAST                6 (f)
                      350 LOAD_METHOD             11 (write)
                      372 LOAD_FAST                5 (content)
                      374 PRECALL                  1
                      378 CALL                     1
                      388 POP_TOP
          
-         300         390 LOAD_CONST               0 (None)
+         346         390 LOAD_CONST               0 (None)
                      392 LOAD_CONST               0 (None)
                      394 LOAD_CONST               0 (None)
                      396 PRECALL                  2
                      400 CALL                     2
                      410 POP_TOP
                      412 JUMP_FORWARD            11 (to 436)
                  >>  414 PUSH_EXC_INFO
@@ -2106,82 +2431,82 @@
                      424 POP_EXCEPT
                      426 RERAISE                  1
                  >>  428 POP_TOP
                      430 POP_EXCEPT
                      432 POP_TOP
                      434 POP_TOP
          
-         302     >>  436 LOAD_GLOBAL             10 (cl)
+         348     >>  436 LOAD_GLOBAL             10 (cl)
                      448 LOAD_ATTR               12 (user_session)
                      458 LOAD_METHOD             13 (get)
                      480 LOAD_CONST              11 ('message_history')
                      482 PRECALL                  1
                      486 CALL                     1
                      496 STORE_FAST               7 (message_history)
          
-         303         498 LOAD_FAST                7 (message_history)
+         349         498 LOAD_FAST                7 (message_history)
                      500 LOAD_METHOD             14 (append)
          
-         304         522 LOAD_CONST              12 ('assistant')
+         350         522 LOAD_CONST              12 ('assistant')
          
-         305         524 LOAD_CONST              13 ('upload file ./tmp/')
+         351         524 LOAD_CONST              13 ('upload file ./tmp/')
                      526 LOAD_FAST                3 (save_path)
                      528 FORMAT_VALUE             0
                      530 LOAD_CONST              14 (' success')
                      532 BUILD_STRING             3
          
-         303         534 LOAD_CONST              15 (('role', 'content'))
+         349         534 LOAD_CONST              15 (('role', 'content'))
                      536 BUILD_CONST_KEY_MAP      2
                      538 PRECALL                  1
                      542 CALL                     1
                      552 POP_TOP
          
-         307         554 LOAD_GLOBAL             30 (config_env)
+         353         554 LOAD_GLOBAL             30 (config_env)
                      566 LOAD_CONST              16 ('openai')
                      568 BINARY_SUBSCR
                      578 LOAD_CONST              17 ('language')
                      580 BINARY_SUBSCR
                      590 STORE_FAST               8 (language)
          
-         308         592 LOAD_GLOBAL             11 (NULL + cl)
+         354         592 LOAD_GLOBAL             11 (NULL + cl)
                      604 LOAD_ATTR               16 (Message)
          
-         309         614 LOAD_CONST              18 ('Chatbot')
+         355         614 LOAD_CONST              18 ('Chatbot')
          
-         310         616 LOAD_GLOBAL             35 (NULL + get_text)
+         356         616 LOAD_GLOBAL             35 (NULL + get_text)
                      628 LOAD_FAST                8 (language)
                      630 LOAD_CONST              19 ('upload_notification')
                      632 PRECALL                  2
                      636 CALL                     2
                      646 FORMAT_VALUE             0
                      648 LOAD_CONST              20 (' ./tmp/')
                      650 LOAD_FAST                3 (save_path)
                      652 FORMAT_VALUE             0
                      654 BUILD_STRING             3
          
-         308         656 KW_NAMES                21
+         354         656 KW_NAMES                21
                      658 PRECALL                  2
                      662 CALL                     2
          
-         311         672 LOAD_METHOD              7 (send)
+         357         672 LOAD_METHOD              7 (send)
                      694 PRECALL                  0
                      698 CALL                     0
          
-         308         708 GET_AWAITABLE            0
+         354         708 GET_AWAITABLE            0
                      710 LOAD_CONST               0 (None)
                  >>  712 SEND                     3 (to 720)
                      714 YIELD_VALUE
                      716 RESUME                   3
                      718 JUMP_BACKWARD_NO_INTERRUPT     4 (to 712)
                  >>  720 POP_TOP
          
-         312         722 LOAD_CONST               0 (None)
+         358         722 LOAD_CONST               0 (None)
                      724 RETURN_VALUE
          
-         314     >>  726 LOAD_GLOBAL             37 (NULL + on_message)
+         360     >>  726 LOAD_GLOBAL             37 (NULL + on_message)
                      738 LOAD_FAST                0 (user_message)
                      740 PRECALL                  1
                      744 CALL                     1
                      754 GET_AWAITABLE            0
                      756 LOAD_CONST               0 (None)
                  >>  758 SEND                     3 (to 766)
                      760 YIELD_VALUE
@@ -2219,59 +2544,59 @@
             ('author', 'content')
          names      ('str', 'os', 'path', 'exists', 'mkdir', 'cl', 'AskFileMessage', 'send', 'name', 'content', 'open', 'write', 'user_session', 'get', 'append', 'config_env', 'Message', 'get_text', 'on_message')
          varnames   ('user_message', 'files', 'file', 'save_path', 'file_path', 'content', 'f', 'message_history', 'language')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
          name       'run_conversation'
-         firstlineno 278
+         firstlineno 324
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
-         317           0 RETURN_GENERATOR
+         363           0 RETURN_GENERATOR
                        2 POP_TOP
                        4 RESUME                   0
          
-         320           6 LOAD_GLOBAL              1 (NULL + print)
+         366           6 LOAD_GLOBAL              1 (NULL + print)
                       18 LOAD_CONST               1 ('stop chat')
                       20 PRECALL                  1
                       24 CALL                     1
                       34 POP_TOP
          
-         321          36 LOAD_CONST               2 (True)
+         367          36 LOAD_CONST               2 (True)
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
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
          name       'stop_chat'
-         firstlineno 317
+         firstlineno 363
          lnotab 0x06031e01
    names      ('uuid', 'openai', 'json', 'ast', 'os', 'chainlit', 'cl', 'functions.FunctionManager', 'FunctionManager', 'inspect', 'tiktoken', 'importlib', 'asyncio', 'get_text', 'platform', 'path', 'join', 'expanduser', 'config_path', 'open', 'config_file', 'load', 'config_env', 'api_key', 'api_base', 'dirname', 'abspath', '__file__', 'current_dir', 'plugins_dir', 'listdir', 'plugin_dirs', 'functions', 'dir', 'f', 'config', 'get', 'enabled', 'FileNotFoundError', 'import_module', 'module', 'extend', 'getmembers', 'function_manager', 'print', 'generate_functions_array', 'env_max_tokens', 'int', 'max_tokens', 'is_stop', '__truncate_conversation', 'get_token_count', 'MAX_ITER', 'object', 'on_message', 'process_new_delta', 'on_chat_start', 'start_chat', 'run_conversation', 'on_stop', 'stop_chat')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/app_terminal.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108010801080108010c0108010801080108010c0108
       0468031a0120ff2e03260126026401360204011eff120504010801020122
       0120ff2e023001080108ff08030401020228011c011eff220418013c011c
-      010401180204010403060c060e04030c7b06230c0104ff0e01021d0c010a
-      ff0e0102260c0104ff0e01
+      010401180204010403060c060e04030c7f001206230c0104ff0e0102350c
+      010aff0e0102260c0104ff0e01
```

### Comparing `codebot-0.0.8/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.1.0/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.1.0/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.1.0/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/app.py` & `codebot-0.1.0/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/app_cn.py` & `codebot-0.1.0/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/app_terminal.py` & `codebot-0.1.0/src/app_terminal.py`

 * *Files 17% similar despite different names*

```diff
@@ -196,21 +196,43 @@
                 "name": function_name,
                 "content": function_response,
             })
             
         print("==================================")
         print(message_history)
         print("==================================")
-
+        print("🚀" * 20)
+        print(function_response)
+        print("🚀" * 20)
+        try:
+            while isinstance(function_response, str) and function_response.startswith('{'):
+                function_response = json.loads(function_response)
+            final_response = function_response
+        except:
+            final_response = function_response
+
+        if isinstance(final_response, dict):
+            # If function_response is a dictionary, convert it to a JSON string
+            content = json.dumps(function_response, ensure_ascii=False, indent=1)
+            if 'output' in function_response:
+                if function_response['output'] != '':
+                    content = function_response['output']
+        elif isinstance(final_response, str):
+            # If function_response is a string, display it as normal text
+            content = final_response
+        else:
+            # If function_response is neither a dict nor a string, convert it to a string
+            content = str(final_response)
         await cl.Message(
             author=function_name,
-            content=str(function_response),
-            language="json",
+            content=content,
+            language="markdown",
             indent=1,
         ).send()
+
         cur_iter += 1
 
 
 async def process_new_delta(new_delta, openai_message, content_ui_message,
                             function_ui_message):
     if "role" in new_delta:
         openai_message["role"] = new_delta["role"]
@@ -243,15 +265,34 @@
                 new_delta["function_call"]["arguments"])
     return openai_message, content_ui_message, function_ui_message
 
 
 
 @cl.on_chat_start
 async def start_chat():
-    password = config_env['openai']['password']
+    
+    user_id = cl.user_session.get("user_id")
+    if user_id is None:
+        user_id = str(uuid.uuid4())
+        cl.user_session.set("user_id", user_id)
+    username = cl.user_session.get("username")
+    password = cl.user_session.get("password")
+    hostname = cl.user_session.get("hostname")
+    if hostname is None:
+        res = await cl.AskUserMessage("请输入需要连接的终端的IP地址").send()
+        hostname = res["content"]
+        cl.user_session.set("hostname", hostname)   
+    if username is None:
+        res = await cl.AskUserMessage("请输入需要连接的终端的用户名").send()
+        username = res["content"]
+        cl.user_session.set("username", username)
+    if password is None:
+        res = await cl.AskUserMessage("输入需要连接的终端的密码").send()
+        password = res["content"]
+        cl.user_session.set("password", password) 
     platform_name = platform.system()
     content = '''You are a great terminal tool for {platform_name}, which can help users better execute {platform_name} terminal commands.
 If you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. 
 No command should generate any terminal input.
 The {platform_name} user name is luzhipeng and the password is "{password}" 
 [IMPORTANT] You must judge for yourself whether you need to use sudo, not all commands should be used with sudo directly.
 example:
@@ -259,24 +300,31 @@
 if the command does not need to be executed as root, you can directly execute the command,like "ls"    
 the terminal function argumets like this:
 ```json
 {{
     "cmd": "ls",
 }}
 ```
+or like this:
+```json
+{{
+    "cmd": "echo '{password}' | sudo -S apt-get install zerotier-cli",
+}}
+```
+if terminal function return a long string, No need to return completely, just summarize the general content.
 '''.format(platform_name=platform_name, password=password)
     language = config_env['openai']['language']
     cl.user_session.set(
         "message_history",
         [{
             "role":
             "system",
             "content": content + "\n\n" + "Please answer me in " + language
         }])
-        
+   
 
 
 @cl.on_message
 async def run_conversation(user_message: object):
     if '/upload' == str(user_message):
         if not os.path.exists('./tmp'):
             os.mkdir('./tmp')
```

### Comparing `codebot-0.0.8/src/chainlit.md` & `codebot-0.1.0/src/chainlit.md`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/functions/FunctionManager.py` & `codebot-0.1.0/src/functions/FunctionManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,17 @@
         if function_name not in self.functions:
             raise ValueError(f"Function '{function_name}' not found")
 
         function = self.functions[function_name]
         # {"role": "function", "name": "get_current_weather", "content": "{\"temperature\": "22", \"unit\": \"celsius\", \"description\": \"Sunny\"}"}
         print(function, args_dict)
         res = await function(**args_dict)
+        print("😈" * 20)
+        print(res)
+        print("😈" * 20)
         # 如果返回的内容是元祖或者列表或者字典，那么就返回一个json字符串
         if isinstance(res, (tuple, list, dict)):
             res = json.dumps(res)
         return res
 
 
 # 测试
```

### Comparing `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4f0dc764 (Mon Jul 31 01:24:31 2023 UTC)
-files sz: 7099
+moddate:  0x7a06ca64 (Wed Aug  2 07:32:10 2023 UTC)
+files sz: 7172
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -47,68 +47,68 @@
                 46 LOAD_CONST               2 (<code object FunctionManager, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 9>)
                 48 MAKE_FUNCTION            0
                 50 LOAD_CONST               3 ('FunctionManager')
                 52 PRECALL                  2
                 56 CALL                     2
                 66 STORE_NAME               5 (FunctionManager)
    
-   125          68 LOAD_CONST              14 (('celsius',))
+   128          68 LOAD_CONST              14 (('celsius',))
                 70 LOAD_CONST               5 ('location')
                 72 LOAD_NAME                6 (str)
                 74 LOAD_CONST               6 ('unit')
                 76 LOAD_NAME                6 (str)
                 78 BUILD_TUPLE              4
-                80 LOAD_CONST               7 (<code object get_current_weather, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 125>)
+                80 LOAD_CONST               7 (<code object get_current_weather, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 128>)
                 82 MAKE_FUNCTION            5 (defaults, annotations)
                 84 STORE_NAME               7 (get_current_weather)
    
-   137          86 LOAD_CONST               8 ('url')
+   140          86 LOAD_CONST               8 ('url')
                 88 LOAD_NAME                6 (str)
                 90 BUILD_TUPLE              2
-                92 LOAD_CONST               9 (<code object get_html, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 137>)
+                92 LOAD_CONST               9 (<code object get_html, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 140>)
                 94 MAKE_FUNCTION            4 (annotations)
                 96 STORE_NAME               8 (get_html)
    
-   155          98 LOAD_CONST              10 ('content')
+   158          98 LOAD_CONST              10 ('content')
                100 LOAD_NAME                6 (str)
                102 BUILD_TUPLE              2
-               104 LOAD_CONST              11 (<code object search_by_bard, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 155>)
+               104 LOAD_CONST              11 (<code object search_by_bard, file "/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py", line 158>)
                106 MAKE_FUNCTION            4 (annotations)
                108 STORE_NAME               9 (search_by_bard)
    
-   173         110 LOAD_NAME               10 (__name__)
+   176         110 LOAD_NAME               10 (__name__)
                112 LOAD_CONST              12 ('__main__')
                114 COMPARE_OP               2 (==)
                120 POP_JUMP_FORWARD_IF_FALSE    46 (to 214)
    
-   174         122 PUSH_NULL
+   177         122 PUSH_NULL
                124 LOAD_NAME                5 (FunctionManager)
                126 LOAD_NAME                9 (search_by_bard)
                128 BUILD_LIST               1
                130 KW_NAMES                13
                132 PRECALL                  1
                136 CALL                     1
                146 STORE_NAME              11 (function_manager)
    
-   175         148 LOAD_NAME               11 (function_manager)
+   178         148 LOAD_NAME               11 (function_manager)
                150 LOAD_METHOD             12 (generate_functions_array)
                172 PRECALL                  0
                176 CALL                     0
                186 STORE_NAME              13 (functions_array)
    
-   176         188 PUSH_NULL
+   179         188 PUSH_NULL
                190 LOAD_NAME               14 (print)
                192 LOAD_NAME               13 (functions_array)
                194 PRECALL                  1
                198 CALL                     1
                208 POP_TOP
                210 LOAD_CONST               1 (None)
                212 RETURN_VALUE
    
-   173     >>  214 LOAD_CONST               1 (None)
+   176     >>  214 LOAD_CONST               1 (None)
                216 RETURN_VALUE
    consts
       0
       None
       code
          argcount  : 0
          nlocals   : 0
@@ -697,15 +697,18 @@
                stacksize : 6
                flags     : 131
                code
                   0x4b00010097007c017c006a000000000000000000760172137403000000
                   0000000000000064017c019b0064029d03a6010000ab0100000000000000
                   0082017c006a0000000000000000007c01190000000000000000007d0374
                   05000000000000000000007c037c02a6020000ab02000000000000000001
-                  0002007c03640369007c02a4018e01830064007b035600970386047d0474
+                  0002007c03640469007c02a4018e01830064007b035600970386047d0474
+                  05000000000000000000006403a6010000ab010000000000000000010074
+                  05000000000000000000007c04a6010000ab010000000000000000010074
+                  05000000000000000000006403a6010000ab010000000000000000010074
                   07000000000000000000007c04740800000000000000000000740a000000
                   00000000000000740c000000000000000000006603a6020000ab02000000
                   00000000007214740f000000000000000000006a0800000000000000007c
                   04a6010000ab0100000000000000007d047c045300
                109           0 RETURN_GENERATOR
                              2 POP_TOP
                              4 RESUME                   0
@@ -737,59 +740,78 @@
                            102 LOAD_FAST                2 (args_dict)
                            104 PRECALL                  2
                            108 CALL                     2
                            118 POP_TOP
                
                117         120 PUSH_NULL
                            122 LOAD_FAST                3 (function)
-                           124 LOAD_CONST               3 (())
+                           124 LOAD_CONST               4 (())
                            126 BUILD_MAP                0
                            128 LOAD_FAST                2 (args_dict)
                            130 DICT_MERGE               1
                            132 CALL_FUNCTION_EX         1
                            134 GET_AWAITABLE            0
                            136 LOAD_CONST               0 (None)
                        >>  138 SEND                     3 (to 146)
                            140 YIELD_VALUE
                            142 RESUME                   3
                            144 JUMP_BACKWARD_NO_INTERRUPT     4 (to 138)
                        >>  146 STORE_FAST               4 (res)
                
-               119         148 LOAD_GLOBAL              7 (NULL + isinstance)
-                           160 LOAD_FAST                4 (res)
-                           162 LOAD_GLOBAL              8 (tuple)
-                           174 LOAD_GLOBAL             10 (list)
-                           186 LOAD_GLOBAL             12 (dict)
-                           198 BUILD_TUPLE              3
-                           200 PRECALL                  2
-                           204 CALL                     2
-                           214 POP_JUMP_FORWARD_IF_FALSE    20 (to 256)
-               
-               120         216 LOAD_GLOBAL             15 (NULL + json)
-                           228 LOAD_ATTR                8 (dumps)
-                           238 LOAD_FAST                4 (res)
-                           240 PRECALL                  1
-                           244 CALL                     1
-                           254 STORE_FAST               4 (res)
+               118         148 LOAD_GLOBAL              5 (NULL + print)
+                           160 LOAD_CONST               3 ('😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈')
+                           162 PRECALL                  1
+                           166 CALL                     1
+                           176 POP_TOP
+               
+               119         178 LOAD_GLOBAL              5 (NULL + print)
+                           190 LOAD_FAST                4 (res)
+                           192 PRECALL                  1
+                           196 CALL                     1
+                           206 POP_TOP
+               
+               120         208 LOAD_GLOBAL              5 (NULL + print)
+                           220 LOAD_CONST               3 ('😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈')
+                           222 PRECALL                  1
+                           226 CALL                     1
+                           236 POP_TOP
+               
+               122         238 LOAD_GLOBAL              7 (NULL + isinstance)
+                           250 LOAD_FAST                4 (res)
+                           252 LOAD_GLOBAL              8 (tuple)
+                           264 LOAD_GLOBAL             10 (list)
+                           276 LOAD_GLOBAL             12 (dict)
+                           288 BUILD_TUPLE              3
+                           290 PRECALL                  2
+                           294 CALL                     2
+                           304 POP_JUMP_FORWARD_IF_FALSE    20 (to 346)
+               
+               123         306 LOAD_GLOBAL             15 (NULL + json)
+                           318 LOAD_ATTR                8 (dumps)
+                           328 LOAD_FAST                4 (res)
+                           330 PRECALL                  1
+                           334 CALL                     1
+                           344 STORE_FAST               4 (res)
                
-               121     >>  256 LOAD_FAST                4 (res)
-                           258 RETURN_VALUE
+               124     >>  346 LOAD_FAST                4 (res)
+                           348 RETURN_VALUE
                consts
                   None
                   "Function '"
                   "' not found"
+                  '😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈😈'
                   ()
                names      ('functions', 'ValueError', 'print', 'isinstance', 'tuple', 'list', 'dict', 'json', 'dumps')
                varnames   ('self', 'function_name', 'args_dict', 'function', 'res')
                freevars   ()
                cellvars   ()
                filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
                name       'call_function'
                firstlineno 109
-               lnotab 0x0602120126021a0220011c0244012801
+               lnotab 0x0602120126021a0220011c011e011e011e0244012801
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'add_function', 'generate_functions_array', 'call_function')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
          name       'FunctionManager'
@@ -801,17 +823,17 @@
       'unit'
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code 0x970064016402640364049c035300
-         125           0 RESUME                   0
+         128           0 RESUME                   0
          
-         133           2 LOAD_CONST               1 ('22')
+         136           2 LOAD_CONST               1 ('22')
                        4 LOAD_CONST               2 ('celsius')
                        6 LOAD_CONST               3 ('Sunny')
                        8 LOAD_CONST               4 (('temperature', 'unit', 'description'))
                       10 BUILD_CONST_KEY_MAP      3
                       12 RETURN_VALUE
          consts
             '\n    Get the current weather in a given location.\n\n    Parameters:\n        - location: The city and state, e.g. San Francisco, CA\n        - unit: The unit of temperature (celsius or fahrenheit)\n    '
@@ -821,59 +843,59 @@
             ('temperature', 'unit', 'description')
          names      ()
          varnames   ('location', 'unit')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
          name       'get_current_weather'
-         firstlineno 125
+         firstlineno 128
          lnotab 0x0208
       'url'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
          flags     : 3
          code
             0x97006401640269017d017401000000000000000000006a010000000000
             0000007c007c01ac03a6020000ab0200000000000000007d027c026a0200
             000000000000005300
-         137           0 RESUME                   0
+         140           0 RESUME                   0
          
-         145           2 LOAD_CONST               1 ('User-Agent')
+         148           2 LOAD_CONST               1 ('User-Agent')
          
-         146           4 LOAD_CONST               2 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36')
+         149           4 LOAD_CONST               2 ('Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36')
          
-         144           6 BUILD_MAP                1
+         147           6 BUILD_MAP                1
                        8 STORE_FAST               1 (headers)
          
-         150          10 LOAD_GLOBAL              1 (NULL + requests)
+         153          10 LOAD_GLOBAL              1 (NULL + requests)
                       22 LOAD_ATTR                1 (get)
                       32 LOAD_FAST                0 (url)
                       34 LOAD_FAST                1 (headers)
                       36 KW_NAMES                 3
                       38 PRECALL                  2
                       42 CALL                     2
                       52 STORE_FAST               2 (response)
          
-         152          54 LOAD_FAST                2 (response)
+         155          54 LOAD_FAST                2 (response)
                       56 LOAD_ATTR                2 (text)
                       66 RETURN_VALUE
          consts
             '\n    Get the html content of the url.if user provide the url,then return the html content of the url.\n    Parameters:\n        url: The url of the website. (required)\n    '
             'User-Agent'
             'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36'
             ('headers',)
          names      ('requests', 'get', 'text')
          varnames   ('url', 'headers', 'response')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
          name       'get_html'
-         firstlineno 137
+         firstlineno 140
          lnotab 0x0208020102fe04062c02
       'content'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
@@ -881,51 +903,51 @@
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             0001007402000000000000000000006a020000000000000000a003000000
             0000000000000000000000000000000000640164027c0064039c02670164
             046405ac06a6040000ab0400000000000000007d01740100000000000000
             0000007c01a6010000ab010000000000000000010064077c016408190000
             000000000000006405190000000000000000006409190000000000000000
             0064071900000000000000000069015300
-         155           0 RESUME                   0
+         158           0 RESUME                   0
          
-         161           2 LOAD_GLOBAL              1 (NULL + print)
+         164           2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_FAST                0 (content)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-         162          32 LOAD_GLOBAL              2 (openai)
+         165          32 LOAD_GLOBAL              2 (openai)
                       44 LOAD_ATTR                2 (ChatCompletion)
                       54 LOAD_METHOD              3 (create)
                       76 LOAD_CONST               1 ('bard')
          
-         164          78 LOAD_CONST               2 ('user')
+         167          78 LOAD_CONST               2 ('user')
          
-         165          80 LOAD_FAST                0 (content)
+         168          80 LOAD_FAST                0 (content)
          
-         163          82 LOAD_CONST               3 (('role', 'content'))
+         166          82 LOAD_CONST               3 (('role', 'content'))
                       84 BUILD_CONST_KEY_MAP      2
                       86 BUILD_LIST               1
          
-         167          88 LOAD_CONST               4 (False)
+         170          88 LOAD_CONST               4 (False)
          
-         168          90 LOAD_CONST               5 (0)
+         171          90 LOAD_CONST               5 (0)
          
-         162          92 KW_NAMES                 6
+         165          92 KW_NAMES                 6
                       94 PRECALL                  4
                       98 CALL                     4
                      108 STORE_FAST               1 (response)
          
-         169         110 LOAD_GLOBAL              1 (NULL + print)
+         172         110 LOAD_GLOBAL              1 (NULL + print)
                      122 LOAD_FAST                1 (response)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 POP_TOP
          
-         170         140 LOAD_CONST               7 ('content')
+         173         140 LOAD_CONST               7 ('content')
                      142 LOAD_FAST                1 (response)
                      144 LOAD_CONST               8 ('choices')
                      146 BINARY_SUBSCR
                      156 LOAD_CONST               5 (0)
                      158 BINARY_SUBSCR
                      168 LOAD_CONST               9 ('message')
                      170 BINARY_SUBSCR
@@ -946,22 +968,22 @@
             'message'
          names      ('print', 'openai', 'ChatCompletion', 'create')
          varnames   ('content', 'response')
          freevars   ()
          cellvars   ()
          filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
          name       'search_by_bard'
-         firstlineno 155
+         firstlineno 158
          lnotab 0x02061e012e02020102fe0604020102fa12071e01
       '__main__'
       ('functions',)
       ('celsius',)
    names      ('inspect', 'json', 're', 'requests', 'openai', 'FunctionManager', 'str', 'get_current_weather', 'get_html', 'search_by_bard', '__name__', 'function_manager', 'generate_functions_array', 'functions_array', 'print')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/luzhipeng/Downloads/openai_code_interpreter/src/functions/FunctionManager.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010802080108031a74120c0c120c120c011a0128011a
+      0x00ff0201080108010802080108031a77120c0c120c120c011a0128011a
       fd
```

### Comparing `codebot-0.0.8/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.1.0/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/get_text.py` & `codebot-0.1.0/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/language/en.json` & `codebot-0.1.0/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/language/zh_CN.json` & `codebot-0.1.0/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.0/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/common/functions.py` & `codebot-0.1.0/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/mysql/functions.py` & `codebot-0.1.0/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.1.0/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/executor.py` & `codebot-0.1.0/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/python/functions.py` & `codebot-0.1.0/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.1.0/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.1.0/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/plugins/terminal/functions.py` & `codebot-0.1.0/src/plugins/terminal/functions.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 import asyncio
 import subprocess
+from functions.RemoteTerminal import RemoteTerminal
+import chainlit as cl
+import uuid
+
+
+remote_terminal_dict = {}
 
 async def terminal(cmd: str, is_auto_run: bool = True):
     """
     if user ask about the Ubuntu question, you can use this function to answer it
     Parameters: 
         cmd: str(required) it must be a command that can be executed in the terminal, The command must be non-blocking and return results.If you encounter a situation where the sudo command is required, you need to automatically input the password in the cmd instead of waiting for terminal input. No command should generate any terminal input.
         is_auto_run: bool(optional) if it is True, the terminal will run the command automatically, otherwise, it will ask the user to run it, You need to decide whether to automatically execute the command based on whether it will have a certain impact.
@@ -11,22 +17,42 @@
     if is_auto_run:
         return await run_cmd(cmd)
     else:
         return {"output": "Should we run the command: " + cmd + "?", "status": True, "askUser": True}
 
 async def run_cmd(cmd: str):
     try:
-        # Automatically execute the command and get the output of the entire terminal
-        process = await asyncio.create_subprocess_shell(
-            cmd, stdout=asyncio.subprocess.PIPE, stderr=asyncio.subprocess.PIPE
-        )
+        
+        user_id = cl.user_session.get("user_id")
+        if user_id is None:
+            user_id = str(uuid.uuid4())
+            cl.user_session.set("user_id", user_id)
+        if user_id not in remote_terminal_dict:
+            username = cl.user_session.get("username")
+            password = cl.user_session.get("password")
+            hostname = cl.user_session.get("hostname")
+            if username is None:
+                res = await cl.AskUserMessage("Please enter the username of the remote server: ").send()
+                username = res["content"]
+                cl.user_session.set("username", username)
+            if password is None:
+                res = await cl.AskUserMessage("Please enter the password of the remote server: ").send()
+                password = res["content"]
+                cl.user_session.set("password", password)
+            if hostname is None:
+                res = await cl.AskUserMessage("Please enter the hostname of the remote server: ").send()
+                hostname = res["content"]
+                cl.user_session.set("hostname", hostname)
+            remote_terminal_dict[user_id] = RemoteTerminal(hostname, username, password)
+        
+        terminal = remote_terminal_dict[user_id]
+        stdout, stderr = terminal.run_cmd(cmd)
 
-        stdout, stderr = await process.communicate()
-
-        if process.returncode != 0:
+        if stderr:
             # The command had a non-zero exit code, return the error message
-            return {"output": stdout.decode(), "status": False, "error": stderr.decode(), "askUser": True, "cmd": cmd}
+            return {"output": stdout, "status": False, "error": stderr, "askUser": True, "cmd": cmd}
         else:
-            return {"output": stdout.decode(), "status": True, "askUser": False}
+            return {"output": stdout, "status": True, "askUser": False}
     except Exception as e:
         # An unexpected error occurred, return the error message
         return {"output": None, "status": False, "error": str(e), "askUser": True, "cmd": cmd}
+
```

### Comparing `codebot-0.0.8/src/plugins/vue/functions.py` & `codebot-0.1.0/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/tmp/1690769899.3643498.png` & `codebot-0.1.0/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/tmp/1690769912.7088609.png` & `codebot-0.1.0/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/tmp/sin_function.gif` & `codebot-0.1.0/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.0.8/src/tmp/sin_function.png` & `codebot-0.1.0/src/tmp/sin_function.png`

 * *Files identical despite different names*

