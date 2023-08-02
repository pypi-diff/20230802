# Comparing `tmp/yopmail-1.4.tar.gz` & `tmp/yopmail-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-1.4.tar", last modified: Mon Jul 31 16:47:05 2023, max compression
+gzip compressed data, was "yopmail-1.5.tar", last modified: Wed Aug  2 15:17:42 2023, max compression
```

## Comparing `yopmail-1.4.tar` & `yopmail-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.802127 yopmail-1.4/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:47:05.802010 yopmail-1.4/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.4/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.4/pyproject.toml
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:47:05.802178 yopmail-1.4/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:46:50.000000 yopmail-1.4/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.801207 yopmail-1.4/yopmail/
--rw-r--r--   0 rayhan     (503) staff       (20)       28 2023-07-31 16:46:29.000000 yopmail-1.4/yopmail/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.4/yopmail/yopmail.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.801839 yopmail-1.4/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      226 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-08-02 15:17:42.232088 yopmail-1.5/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1669 2023-08-02 15:17:42.231952 yopmail-1.5/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1366 2023-07-31 17:00:44.000000 yopmail-1.5/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 17:02:49.000000 yopmail-1.5/pyproject.toml
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-08-02 15:17:42.232133 yopmail-1.5/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      737 2023-08-02 15:16:57.000000 yopmail-1.5/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-08-02 15:17:42.230980 yopmail-1.5/yopmail/
+-rw-r--r--   0 rayhan     (503) staff       (20)       28 2023-07-31 17:02:49.000000 yopmail-1.5/yopmail/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     6133 2023-08-02 15:15:01.000000 yopmail-1.5/yopmail/yopmail.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-08-02 15:17:42.231745 yopmail-1.5/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1669 2023-08-02 15:17:42.000000 yopmail-1.5/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      226 2023-08-02 15:17:42.000000 yopmail-1.5/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-08-02 15:17:42.000000 yopmail-1.5/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-08-02 15:17:42.000000 yopmail-1.5/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-08-02 15:17:42.000000 yopmail-1.5/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-1.4/PKG-INFO` & `yopmail-1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.4
+Version: 1.5
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ###### ⚠️ Disclaimer: Reverse engineering process is shown for research purposes only.
 
 # 👏 Get mails from Yopmail inbox
 Get mails from a Yopmail inbox, save them as ``.html``
 
 
 ## 📖 Usage:
 Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
 ```
 pip install yopmail
 ```
 
+Import ``Yopmail`` class from ``yopmail`` module
+```python
+from yopmail import Yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
```

### Comparing `yopmail-1.4/README.md` & `yopmail-1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 ## 📖 Usage:
 Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
 ```
 pip install yopmail
 ```
 
+Import ``Yopmail`` class from ``yopmail`` module
+```python
+from yopmail import Yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
```

### Comparing `yopmail-1.4/setup.py` & `yopmail-1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='1.4',
+    version='1.5',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
     packages = find_packages(),
-    python_requires='>=3.8',
+    python_requires='>=3.10',
     url='https://github.com/rklf/yopmail',
     keywords='yopmail get mails retrieve scrap emails',
     install_requires=[
           'beautifulsoup4',
           'requests',
       ],
```

### Comparing `yopmail-1.4/yopmail/yopmail.py` & `yopmail-1.5/yopmail/yopmail.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,36 +45,42 @@
     def request(self, url: str, params=None, proxies=None, context: str = None) -> requests.models.Response|None:
         proxies = proxies if proxies is not None else self.proxies
         try:
             if self.yp is None:
                 context = 'yp'
                 req = self.session.get(self.url, proxies=proxies)
                 if not req:
-                    return None
+                    if req.status_code == 429:
+                        raise requests.ConnectionError(f"Too Many Requests (429 status code) error, use a proxy or try again later")
+                    raise Exception(req)
                 self.extract_yp(req)
                 params = {**params, 'yp': self.yp}
 
             if self.yj is None:
                 context = 'yj'
                 req = self.session.get('https://yopmail.com/ver/5.0/webmail.js', proxies=proxies)
                 if not req:
-                    return None
+                    if req.status_code == 429:
+                        raise requests.ConnectionError(f"Too Many Requests (429 status code) error, use a proxy or try again later")
+                    raise Exception(req)
                 self.extract_yj(req)
                 params = {**params, 'yj': self.yj}
 
             if self.ycons is None:
                 context = 'ycons'
                 req = self.session.get('https://yopmail.com/consent?c=deny', proxies=proxies) # Set consent cookies
                 if not req:
-                    return None
+                    if req.status_code == 429:
+                        raise requests.ConnectionError(f"Too Many Requests (429 status code) error, use a proxy or try again later")
+                    raise Exception(req)
             self.add_ytime()
             return self.session.get(url, params=params, cookies=self.jar, proxies=proxies)
         except requests.exceptions.ProxyError as err:
-                print(f"[x] Couldn't process {context} request (ProxyError):", err)
-                return None
+            print(f"[x] Couldn't process {context} request (ProxyError):", err)
+            return None
         except requests.exceptions.ConnectionError as err:
             print(f"[x] Couldn't process {context} request (ConnectionError):", err)
             return None
         except requests.exceptions.Timeout as err:
             print(f"[x] Couldn't process {context} request (Timeout):", err)
             return None
         except Exception as err:
```

### Comparing `yopmail-1.4/yopmail.egg-info/PKG-INFO` & `yopmail-1.5/yopmail.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.4
+Version: 1.5
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ###### ⚠️ Disclaimer: Reverse engineering process is shown for research purposes only.
 
 # 👏 Get mails from Yopmail inbox
 Get mails from a Yopmail inbox, save them as ``.html``
 
 
 ## 📖 Usage:
 Install the latest version from PyPI by using [pip](https://pip.pypa.io/):
 ```
 pip install yopmail
 ```
 
+Import ``Yopmail`` class from ``yopmail`` module
+```python
+from yopmail import Yopmail
+```
+
 Instantiate ``Yopmail`` class with username as parameter (with ``@`` or not) and provide proxies if needed
 ```python
 y = Yopmail('test', proxies=None)
 ```
 
 Using ``get_mail_ids()`` method you get mail ids. You can provide (optional) ``page`` parameter otherwise page 1 is used as default. You can as well provide ``proxy`` parameter which would override instantiated class proxies.
 ```python
```

