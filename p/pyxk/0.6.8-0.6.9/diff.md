# Comparing `tmp/pyxk-0.6.8.tar.gz` & `tmp/pyxk-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.8.tar", last modified: Mon Jul 31 23:17:40 2023, max compression
+gzip compressed data, was "pyxk-0.6.9.tar", last modified: Wed Aug  2 09:01:26 2023, max compression
```

## Comparing `pyxk-0.6.8.tar` & `pyxk-0.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.8/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 23:17:40.394998 pyxk-0.6.8/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.8/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.384998 pyxk-0.6.8/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.8/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.8/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    23004 2023-07-31 23:06:20.000000 pyxk-0.6.8/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.8/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.8/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.8/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.8/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 13:41:16.000000 pyxk-0.6.8/pyxk/m3u8/_initial.py
--rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.8/pyxk/m3u8/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.8/pyxk/m3u8/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.6.8/pyxk/m3u8/m3u8parse.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.8/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.8/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.8/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.8/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.8/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 23:17:40.394998 pyxk-0.6.8/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 23:17:40.000000 pyxk-0.6.8/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 23:17:40.394998 pyxk-0.6.8/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 22:46:51.000000 pyxk-0.6.8/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.9/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-02 09:01:26.603649 pyxk-0.6.9/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.9/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.9/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.9/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    23027 2023-08-02 02:02:37.000000 pyxk-0.6.9/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.9/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.9/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.9/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.9/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8876 2023-07-31 23:21:30.000000 pyxk-0.6.9/pyxk/m3u8/_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.9/pyxk/m3u8/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.9/pyxk/m3u8/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    10217 2023-07-31 13:31:37.000000 pyxk-0.6.9/pyxk/m3u8/m3u8parse.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.603649 pyxk-0.6.9/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.9/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.9/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.9/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.9/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.9/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-08-02 09:01:26.593649 pyxk-0.6.9/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      558 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-08-02 09:01:26.000000 pyxk-0.6.9/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-08-02 09:01:26.603649 pyxk-0.6.9/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-08-02 09:01:05.000000 pyxk-0.6.9/setup.py
```

### Comparing `pyxk-0.6.8/LICENSE` & `pyxk-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/PKG-INFO` & `pyxk-0.6.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.8
+Version: 0.6.9
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.8/README.md` & `pyxk-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/aclient/client.py` & `pyxk-0.6.9/pyxk/aclient/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                 except aiohttp_exceptions.ServerDisconnectedError as exc:
                     # 提示信息
                     await self._warning('server_disconnected', url, warning, response)
                     exc_from_request = exc
 
                 finally:
                     # 关闭连接
-                    if response:
+                    if response and callable(callback):
                         response.close()
 
             else:
                 # 抛出错误
                 if exc_from_request:
                     raise exc_from_request
                 # 达到最大请求次数
```

### Comparing `pyxk-0.6.8/pyxk/aclient/typedef.py` & `pyxk-0.6.9/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/aes/cryptor.py` & `pyxk-0.6.9/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/m3u8/_initial.py` & `pyxk-0.6.9/pyxk/m3u8/_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
         :param url: m3u8 url
         :param is_key: 是否为m3u8密钥
         :return: Union[str, bytes]
         """
 
         content = b''
         response = self.session.get(url, verify=self._verify, timeout=10, stream=True)
+        response.raise_for_status()
         self.history.append(response)
 
         for index, chunk in enumerate(response.iter_content(1024)):
             # 检查是否是m3u8内容
             if not is_key and index == 0 and not self._is_m3u8(chunk):
                 break
             content += chunk
```

### Comparing `pyxk-0.6.8/pyxk/m3u8/downloader.py` & `pyxk-0.6.9/pyxk/m3u8/downloader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/m3u8/entry_point.py` & `pyxk-0.6.9/pyxk/m3u8/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.9/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/requests/api.py` & `pyxk-0.6.9/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/requests/entry_point.py` & `pyxk-0.6.9/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/requests/sessions.py` & `pyxk-0.6.9/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk/utils.py` & `pyxk-0.6.9/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/pyxk.egg-info/PKG-INFO` & `pyxk-0.6.9/pyxk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.8
+Version: 0.6.9
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.8/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.9/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.8/setup.py` & `pyxk-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.8',
+    version='0.6.9',
     author='kai139',
     install_requires=[
         'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
     ],
     entry_points={
         'console_scripts': [
             'm3u8 = pyxk.m3u8.entry_point:main',
```

