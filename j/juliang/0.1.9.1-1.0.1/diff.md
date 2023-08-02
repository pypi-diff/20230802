# Comparing `tmp/juliang-0.1.9.1.tar.gz` & `tmp/juliang-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juliang-0.1.9.1.tar", last modified: Thu Dec  2 03:52:49 2021, max compression
+gzip compressed data, was "juliang-1.0.1.tar", last modified: Wed Aug  2 02:46:10 2023, max compression
```

## Comparing `juliang-0.1.9.1.tar` & `juliang-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.770166 juliang-0.1.9.1/
--rw-r--r--   0 root         (0) staff       (20)     1486 2021-12-02 03:52:49.769900 juliang-0.1.9.1/PKG-INFO
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.761382 juliang-0.1.9.1/juliang.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1486 2021-12-02 03:52:49.000000 juliang-0.1.9.1/juliang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      777 2021-12-02 03:52:49.000000 juliang-0.1.9.1/juliang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2021-12-02 03:52:49.000000 juliang-0.1.9.1/juliang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       10 2021-12-02 03:52:49.000000 juliang-0.1.9.1/juliang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.761810 juliang-0.1.9.1/juliangip/
--rw-r--r--   0 root         (0) staff       (20)     4946 2021-11-11 01:05:52.000000 juliang-0.1.9.1/juliangip/Juliang.py
--rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.765990 juliang-0.1.9.1/juliangip/common/
--rw-r--r--   0 root         (0) staff       (20)      409 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/AloneGetIps.py
--rw-r--r--   0 root         (0) staff       (20)      196 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/AloneGetWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      349 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/AloneReplaceWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      224 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/AloneSetWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      195 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicBalance.py
--rw-r--r--   0 root         (0) staff       (20)      227 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicCheck.py
--rw-r--r--   0 root         (0) staff       (20)      689 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicGetIps.py
--rw-r--r--   0 root         (0) staff       (20)      198 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicGetWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      225 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicRemain.py
--rw-r--r--   0 root         (0) staff       (20)      351 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicReplaceWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      226 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/DynamicSetWhiteIp.py
--rw-r--r--   0 root         (0) staff       (20)      231 2021-11-11 00:53:41.000000 juliang-0.1.9.1/juliangip/common/UsersGetAllOrders.py
--rw-r--r--   0 root         (0) staff       (20)      192 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/UsersGetBalance.py
--rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/common/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.766471 juliang-0.1.9.1/juliangip/enums/
--rw-r--r--   0 root         (0) staff       (20)     1423 2021-11-11 01:05:48.000000 juliang-0.1.9.1/juliangip/enums/URL.py
--rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/enums/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-12-02 03:52:49.769576 juliang-0.1.9.1/juliangip/ext/
--rw-r--r--   0 root         (0) staff       (20)     1394 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/ext/StrKit.py
--rw-r--r--   0 root         (0) staff       (20)        0 2021-11-11 00:46:22.000000 juliang-0.1.9.1/juliangip/ext/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       38 2021-12-02 03:52:49.770245 juliang-0.1.9.1/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     3825 2021-12-02 03:52:20.000000 juliang-0.1.9.1/setup.py
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.069491 juliang-1.0.1/
+-rw-r--r--   0 symbol     (501) staff       (20)     1614 2023-08-02 02:46:10.069319 juliang-1.0.1/PKG-INFO
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.061731 juliang-1.0.1/juliang.egg-info/
+-rw-r--r--   0 symbol     (501) staff       (20)     1614 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/PKG-INFO
+-rw-r--r--   0 symbol     (501) staff       (20)     1155 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/SOURCES.txt
+-rw-r--r--   0 symbol     (501) staff       (20)        1 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/dependency_links.txt
+-rw-r--r--   0 symbol     (501) staff       (20)       10 2023-08-02 02:46:10.000000 juliang-1.0.1/juliang.egg-info/top_level.txt
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.062124 juliang-1.0.1/juliangip/
+-rw-r--r--   0 symbol     (501) staff       (20)     9786 2023-08-02 02:03:16.000000 juliang-1.0.1/juliangip/Juliang.py
+-rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/__init__.py
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.068476 juliang-1.0.1/juliangip/common/
+-rw-r--r--   0 symbol     (501) staff       (20)      409 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneGetIps.py
+-rw-r--r--   0 symbol     (501) staff       (20)      196 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneGetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      349 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneReplaceWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      224 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/AloneSetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      195 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicBalance.py
+-rw-r--r--   0 symbol     (501) staff       (20)      227 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicCheck.py
+-rw-r--r--   0 symbol     (501) staff       (20)      689 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicGetIps.py
+-rw-r--r--   0 symbol     (501) staff       (20)      198 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicGetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      225 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicRemain.py
+-rw-r--r--   0 symbol     (501) staff       (20)      351 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicReplaceWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      226 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/DynamicSetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      224 2023-08-02 01:37:44.000000 juliang-1.0.1/juliangip/common/PostPayCheck.py
+-rw-r--r--   0 symbol     (501) staff       (20)      684 2023-08-02 01:27:29.000000 juliang-1.0.1/juliangip/common/PostPayGetIps.py
+-rw-r--r--   0 symbol     (501) staff       (20)      196 2023-08-02 01:56:54.000000 juliang-1.0.1/juliangip/common/PostPayGetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      349 2023-08-02 02:01:33.000000 juliang-1.0.1/juliangip/common/PostPayReplaceWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      223 2023-08-02 01:50:34.000000 juliang-1.0.1/juliangip/common/PostPaySetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      484 2023-08-01 10:22:40.000000 juliang-1.0.1/juliangip/common/UnlimitedGetIps.py
+-rw-r--r--   0 symbol     (501) staff       (20)      197 2023-08-01 10:28:08.000000 juliang-1.0.1/juliangip/common/UnlimitedGetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      351 2023-08-01 10:33:13.000000 juliang-1.0.1/juliangip/common/UnlimitedReplaceWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      228 2023-08-01 10:26:06.000000 juliang-1.0.1/juliangip/common/UnlimitedSetWhiteIp.py
+-rw-r--r--   0 symbol     (501) staff       (20)      275 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetAllOrders.py
+-rw-r--r--   0 symbol     (501) staff       (20)      192 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetBalance.py
+-rw-r--r--   0 symbol     (501) staff       (20)      222 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/UsersGetCity.py
+-rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/common/__init__.py
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.068861 juliang-1.0.1/juliangip/enums/
+-rw-r--r--   0 symbol     (501) staff       (20)     2351 2023-08-02 02:03:12.000000 juliang-1.0.1/juliangip/enums/URL.py
+-rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/enums/__init__.py
+drwxr-xr-x   0 symbol     (501) staff       (20)        0 2023-08-02 02:46:10.069120 juliang-1.0.1/juliangip/ext/
+-rw-r--r--   0 symbol     (501) staff       (20)     1394 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/ext/StrKit.py
+-rw-r--r--   0 symbol     (501) staff       (20)        0 2023-08-01 06:02:04.000000 juliang-1.0.1/juliangip/ext/__init__.py
+-rw-r--r--   0 symbol     (501) staff       (20)       38 2023-08-02 02:46:10.069531 juliang-1.0.1/setup.cfg
+-rw-r--r--   0 symbol     (501) staff       (20)     3823 2023-08-02 02:38:56.000000 juliang-1.0.1/setup.py
```

### Comparing `juliang-0.1.9.1/PKG-INFO` & `juliang-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: juliang
-Version: 0.1.9.1
+Version: 1.0.1
 Summary: 巨量IP - API SDK for Python
 Home-page: https://gitee.com/juliangip/juliang-python-sdk
 Author: juliangip
 Author-email: juliangip@163.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
@@ -38,14 +37,16 @@
 #### 通过源码包安装
 前往 [gitee代码托管地址](https://gitee.com/juliangip/juliang-python-sdk) 下载最新代码，解压
 
 ```python
 python setup.py install
 ```
 
+> Python 3.9以下的需要将 源码文件Juliang.py中的unquote(request.read(), "utf-8")方法替换为unquote(request.read().decode(), "utf-8")
+
 ## 示例
 ```python
 import juliangip.Juliang as Juliang
 import juliangip.common.DynamicGetIps as dgi
 
 
 dynamic_trade_no = "1135123856516518735679"
@@ -61,8 +62,7 @@
 if __name__ == '__main__':
     dynmaic_get_ips()
 ```
 
 ## 参考资料
 
 * [API文档](https://www.juliangip.com/help/api/api/)
-
```

### Comparing `juliang-0.1.9.1/juliang.egg-info/PKG-INFO` & `juliang-1.0.1/juliang.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: juliang
-Version: 0.1.9.1
+Version: 1.0.1
 Summary: 巨量IP - API SDK for Python
 Home-page: https://gitee.com/juliangip/juliang-python-sdk
 Author: juliangip
 Author-email: juliangip@163.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
@@ -38,14 +37,16 @@
 #### 通过源码包安装
 前往 [gitee代码托管地址](https://gitee.com/juliangip/juliang-python-sdk) 下载最新代码，解压
 
 ```python
 python setup.py install
 ```
 
+> Python 3.9以下的需要将 源码文件Juliang.py中的unquote(request.read(), "utf-8")方法替换为unquote(request.read().decode(), "utf-8")
+
 ## 示例
 ```python
 import juliangip.Juliang as Juliang
 import juliangip.common.DynamicGetIps as dgi
 
 
 dynamic_trade_no = "1135123856516518735679"
@@ -61,8 +62,7 @@
 if __name__ == '__main__':
     dynmaic_get_ips()
 ```
 
 ## 参考资料
 
 * [API文档](https://www.juliangip.com/help/api/api/)
-
```

### Comparing `juliang-0.1.9.1/juliang.egg-info/SOURCES.txt` & `juliang-1.0.1/juliang.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 juliangip/common/DynamicBalance.py
 juliangip/common/DynamicCheck.py
 juliangip/common/DynamicGetIps.py
 juliangip/common/DynamicGetWhiteIp.py
 juliangip/common/DynamicRemain.py
 juliangip/common/DynamicReplaceWhiteIp.py
 juliangip/common/DynamicSetWhiteIp.py
+juliangip/common/PostPayCheck.py
+juliangip/common/PostPayGetIps.py
+juliangip/common/PostPayGetWhiteIp.py
+juliangip/common/PostPayReplaceWhiteIp.py
+juliangip/common/PostPaySetWhiteIp.py
+juliangip/common/UnlimitedGetIps.py
+juliangip/common/UnlimitedGetWhiteIp.py
+juliangip/common/UnlimitedReplaceWhiteIp.py
+juliangip/common/UnlimitedSetWhiteIp.py
 juliangip/common/UsersGetAllOrders.py
 juliangip/common/UsersGetBalance.py
+juliangip/common/UsersGetCity.py
 juliangip/common/__init__.py
 juliangip/enums/URL.py
 juliangip/enums/__init__.py
 juliangip/ext/StrKit.py
 juliangip/ext/__init__.py
```

### Comparing `juliang-0.1.9.1/juliangip/common/DynamicGetIps.py` & `juliang-1.0.1/juliangip/common/DynamicGetIps.py`

 * *Files identical despite different names*

### Comparing `juliang-0.1.9.1/juliangip/ext/StrKit.py` & `juliang-1.0.1/juliangip/ext/StrKit.py`

 * *Files identical despite different names*

### Comparing `juliang-0.1.9.1/setup.py` & `juliang-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'juliang'
 DESCRIPTION = '巨量IP - API SDK for Python'
 URL = 'https://gitee.com/juliangip/juliang-python-sdk'
 EMAIL = 'juliangip@163.com'
 AUTHOR = 'juliangip'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.9.1'
+VERSION = '1.0.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

