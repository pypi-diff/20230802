# Comparing `tmp/crsts-2.4.3.tar.gz` & `tmp/crsts-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crsts-2.4.3.tar", last modified: Tue Aug 16 10:01:50 2022, max compression
+gzip compressed data, was "dist/crsts-2.4.5.tar", last modified: Wed Aug  2 06:54:04 2023, max compression
```

## Comparing `crsts-2.4.3.tar` & `crsts-2.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2022-08-16 10:01:50.000000 crsts-2.4.3/
--rw-r--r--   0 bappy      (501) admin       (80)      376 2022-08-16 10:01:50.000000 crsts-2.4.3/PKG-INFO
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts/
--rw-r--r--   0 bappy      (501) admin       (80)       76 2021-08-30 02:59:14.000000 crsts-2.4.3/crsts/__init__.py
--rw-r--r--   0 bappy      (501) admin       (80)    22496 2022-08-16 10:01:45.000000 crsts-2.4.3/crsts/crsts.py
-drwxr-xr-x   0 bappy      (501) admin       (80)        0 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts.egg-info/
--rw-r--r--   0 bappy      (501) admin       (80)      376 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts.egg-info/PKG-INFO
--rw-r--r--   0 bappy      (501) admin       (80)      167 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts.egg-info/SOURCES.txt
--rw-r--r--   0 bappy      (501) admin       (80)        6 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts.egg-info/top_level.txt
--rw-r--r--   0 bappy      (501) admin       (80)        1 2022-08-16 10:01:50.000000 crsts-2.4.3/crsts.egg-info/dependency_links.txt
--rw-r--r--   0 bappy      (501) admin       (80)       48 2021-08-30 02:59:14.000000 crsts-2.4.3/README.md
--rw-r--r--   0 bappy      (501) admin       (80)      591 2022-08-16 09:33:29.000000 crsts-2.4.3/setup.py
--rw-r--r--   0 bappy      (501) admin       (80)       38 2022-08-16 10:01:50.000000 crsts-2.4.3/setup.cfg
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-02 06:54:04.000000 crsts-2.4.5/
+-rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-02 06:54:04.000000 crsts-2.4.5/PKG-INFO
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts/
+-rw-r--r--   0 bappy      (501) admin       (80)       76 2021-08-30 02:59:14.000000 crsts-2.4.5/crsts/__init__.py
+-rw-r--r--   0 bappy      (501) admin       (80)    22761 2023-08-02 06:53:56.000000 crsts-2.4.5/crsts/crsts.py
+drwxr-xr-x   0 bappy      (501) admin       (80)        0 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts.egg-info/
+-rw-r--r--   0 bappy      (501) admin       (80)      376 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts.egg-info/PKG-INFO
+-rw-r--r--   0 bappy      (501) admin       (80)      167 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts.egg-info/SOURCES.txt
+-rw-r--r--   0 bappy      (501) admin       (80)        6 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts.egg-info/top_level.txt
+-rw-r--r--   0 bappy      (501) admin       (80)        1 2023-08-02 06:54:04.000000 crsts-2.4.5/crsts.egg-info/dependency_links.txt
+-rw-r--r--   0 bappy      (501) admin       (80)       48 2021-08-30 02:59:14.000000 crsts-2.4.5/README.md
+-rw-r--r--   0 bappy      (501) admin       (80)      591 2023-08-02 06:51:58.000000 crsts-2.4.5/setup.py
+-rw-r--r--   0 bappy      (501) admin       (80)       38 2023-08-02 06:54:04.000000 crsts-2.4.5/setup.cfg
```

### Comparing `crsts-2.4.3/crsts/crsts.py` & `crsts-2.4.5/crsts/crsts.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,22 @@
             all_lines = fr.readlines()
             if strip:
                 all_lines = [l.strip() for l in all_lines]
         else:
             all_lines = fr.read()
         return all_lines
 
+def merge_file(file_path_lst,merge_file_path,shuffle=False):
+    cnt=[]
+    for file_path in file_path_lst:
+        cnt.extend(read_path(file_path))
+    if shuffle:
+        rand_shuffle(cnt)
+    write2path(cnt,merge_file_path)
+
 def print_list(array,index=False,top_n=None):
     """ 打印list内容
             index - 是否打印索引
     """
     if not top_n:
         top_n=len(array)
     if index:
@@ -578,15 +586,15 @@
     return json.loads(json_str)
 
 def json_dump(json_data, fp):
     """ 写入json文件 """
     return json.dump(json_data, open(fp,mode='w',encoding="utf-8"))
 
 def json_dumps(json_data,indent=None):
-    """ 转换json """
+    """ 转换json indent=4 代表缩进 可视化输出"""
     return json.dumps(json_data,indent=indent)
 
 def sleep(secs):
     """ 休眠 """
     time.sleep(secs)
 
 def rename_file_md5(folder,over_write=True):
```

### Comparing `crsts-2.4.3/setup.py` & `crsts-2.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md","r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crsts",
-    version="2.4.3",
+    version="2.4.5",
     author="Chris Chen",
     author_email="wsywddr@163.com",
     description="This is my personal toolkit.",
     longe_description=long_description,
     longe_description_content_type="text/markdown",
     url="https://github.com/wsywddr",
     packages=setuptools.find_packages(),
```

