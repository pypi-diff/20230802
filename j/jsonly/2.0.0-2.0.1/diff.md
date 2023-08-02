# Comparing `tmp/jsonly-2.0.0.tar.gz` & `tmp/jsonly-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonly-2.0.0.tar", last modified: Mon Jul 31 17:50:26 2023, max compression
+gzip compressed data, was "jsonly-2.0.1.tar", last modified: Wed Aug  2 02:11:28 2023, max compression
```

## Comparing `jsonly-2.0.0.tar` & `jsonly-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:50:26.688126 jsonly-2.0.0/
--rw-rw-rw-   0        0        0     1087 2023-07-31 09:52:34.000000 jsonly-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2882 2023-07-31 17:50:26.686983 jsonly-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-07-31 17:45:17.000000 jsonly-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 17:50:26.658691 jsonly-2.0.0/jsonly/
--rw-rw-rw-   0        0        0     1118 2023-07-31 17:50:04.000000 jsonly-2.0.0/jsonly/__init__.py
--rw-rw-rw-   0        0        0     4292 2023-07-31 11:42:06.000000 jsonly-2.0.0/jsonly/clinet.py
--rw-rw-rw-   0        0        0     1432 2023-07-31 11:42:06.000000 jsonly-2.0.0/jsonly/connect.py
--rw-rw-rw-   0        0        0     4492 2023-07-31 17:03:18.000000 jsonly-2.0.0/jsonly/convert.py
--rw-rw-rw-   0        0        0      285 2023-07-31 11:42:06.000000 jsonly-2.0.0/jsonly/error.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:50:26.685959 jsonly-2.0.0/jsonly.egg-info/
--rw-rw-rw-   0        0        0     2882 2023-07-31 17:50:26.000000 jsonly-2.0.0/jsonly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-31 17:50:26.000000 jsonly-2.0.0/jsonly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:50:26.000000 jsonly-2.0.0/jsonly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 17:50:26.000000 jsonly-2.0.0/jsonly.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 17:50:26.688126 jsonly-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      507 2023-07-31 11:42:06.000000 jsonly-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:28.095648 jsonly-2.0.1/
+-rw-rw-rw-   0        0        0     1087 2023-08-02 01:51:24.000000 jsonly-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2882 2023-08-02 02:11:28.094651 jsonly-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2023-08-02 02:09:52.000000 jsonly-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:28.054999 jsonly-2.0.1/jsonly/
+-rw-rw-rw-   0        0        0     1120 2023-08-02 02:08:23.000000 jsonly-2.0.1/jsonly/__init__.py
+-rw-rw-rw-   0        0        0     4394 2023-08-02 01:55:27.000000 jsonly-2.0.1/jsonly/client.py
+-rw-rw-rw-   0        0        0     1432 2023-08-02 01:51:24.000000 jsonly-2.0.1/jsonly/connect.py
+-rw-rw-rw-   0        0        0     4492 2023-08-02 02:01:53.000000 jsonly-2.0.1/jsonly/convert.py
+-rw-rw-rw-   0        0        0      285 2023-08-02 01:51:24.000000 jsonly-2.0.1/jsonly/error.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:11:28.092126 jsonly-2.0.1/jsonly.egg-info/
+-rw-rw-rw-   0        0        0     2882 2023-08-02 02:11:27.000000 jsonly-2.0.1/jsonly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-08-02 02:11:27.000000 jsonly-2.0.1/jsonly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:11:27.000000 jsonly-2.0.1/jsonly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 02:11:27.000000 jsonly-2.0.1/jsonly.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:11:28.096786 jsonly-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      507 2023-08-02 02:09:33.000000 jsonly-2.0.1/setup.py
```

### Comparing `jsonly-2.0.0/LICENSE` & `jsonly-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonly-2.0.0/PKG-INFO` & `jsonly-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonly
-Version: 2.0.0
+Version: 2.0.1
 Summary: JSON 데이터 관리 라이브러리
 Home-page: https://github.com/VoidAsMad/jsonly
 Author: VoidAsMad
 Author-email: star@devksy.xyz
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -51,15 +51,15 @@
 
 ### **GET**
 
 데이터를 불러올 때 사용하는 메소드
 
 ```py
 # get.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 print(jsonly.get(path="기본/사과"))
 ```
 
 ```
 # result
@@ -68,15 +68,15 @@
 
 ### **SET**
 
 데이터를 덮어씌울 때 사용하는 메소드
 
 ```py
 # set.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"기본중에" : "기본"}
 print(jsonly.set(data=data))
 ```
 
@@ -94,15 +94,15 @@
 
 ### **UPDATE**
 
 데이터를 루트 경로에 추가할 때 사용하는 메소드
 
 ```py
 # update.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"새로운" : "데이터"}
 print(jsonly.update(data=data))
 ```
 
@@ -125,15 +125,15 @@
 
 ### **INSERT**
 
 데이터를 특정 경로에 추가할 때 사용하는 메소드
 
 ```py
 # insert.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"데이터" : "삽입"}
 print(jsonly.insert(data=data, path='기본'))
 ```
```

### Comparing `jsonly-2.0.0/README.md` & `jsonly-2.0.1/jsonly.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: jsonly
+Version: 2.0.1
+Summary: JSON 데이터 관리 라이브러리
+Home-page: https://github.com/VoidAsMad/jsonly
+Author: VoidAsMad
+Author-email: star@devksy.xyz
+License: MIT
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
   <h1>Jsonly</h1>
 </div>
 
 ![banner](https://github.com/VoidAsMad/jsonly/assets/103942316/e6bf681e-3eee-4150-99dc-dd9afacd00b2)
 
 <div align="center">
@@ -39,15 +51,15 @@
 
 ### **GET**
 
 데이터를 불러올 때 사용하는 메소드
 
 ```py
 # get.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 print(jsonly.get(path="기본/사과"))
 ```
 
 ```
 # result
@@ -56,15 +68,15 @@
 
 ### **SET**
 
 데이터를 덮어씌울 때 사용하는 메소드
 
 ```py
 # set.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"기본중에" : "기본"}
 print(jsonly.set(data=data))
 ```
 
@@ -82,15 +94,15 @@
 
 ### **UPDATE**
 
 데이터를 루트 경로에 추가할 때 사용하는 메소드
 
 ```py
 # update.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"새로운" : "데이터"}
 print(jsonly.update(data=data))
 ```
 
@@ -113,15 +125,15 @@
 
 ### **INSERT**
 
 데이터를 특정 경로에 추가할 때 사용하는 메소드
 
 ```py
 # insert.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"데이터" : "삽입"}
 print(jsonly.insert(data=data, path='기본'))
 ```
```

### Comparing `jsonly-2.0.0/jsonly/__init__.py` & `jsonly-2.0.1/jsonly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE."""
 
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
```

### Comparing `jsonly-2.0.0/jsonly/clinet.py` & `jsonly-2.0.1/jsonly/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,17 @@
     Docs : link \n
     """
 
     def __init__(
         self, path: str, encoding: str = "utf-8", ensure_ascii: bool = False
     ) -> None:
         super().__init__(path, encoding, ensure_ascii)
+        self.path = path
+        self.encoding = encoding
+        self.ensure_ascii = ensure_ascii
 
     def get(self, path: str = None) -> dict[str, any]:
         """
         JSON 파일의 데이터를 가져옵니다.\n
         Load data from the database.
 
         ## <Parameter>
```

### Comparing `jsonly-2.0.0/jsonly/connect.py` & `jsonly-2.0.1/jsonly/connect.py`

 * *Files identical despite different names*

### Comparing `jsonly-2.0.0/jsonly/convert.py` & `jsonly-2.0.1/jsonly/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import sqlite3
 from typing import Union
 
-from .clinet import UseJsonly
+from .client import UseJsonly
 from .error import ConverException, ConvertTypeExcetion, SaveException
 
 
 class Convert:
     """SQL 파일을 Json파일로 변환하는 기능을 지원하는 클래스입니다."""
 
     def __init__(self, jsonly: UseJsonly, sql_path: str) -> None:
```

### Comparing `jsonly-2.0.0/jsonly.egg-info/PKG-INFO` & `jsonly-2.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: jsonly
-Version: 2.0.0
-Summary: JSON 데이터 관리 라이브러리
-Home-page: https://github.com/VoidAsMad/jsonly
-Author: VoidAsMad
-Author-email: star@devksy.xyz
-License: MIT
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
   <h1>Jsonly</h1>
 </div>
 
 ![banner](https://github.com/VoidAsMad/jsonly/assets/103942316/e6bf681e-3eee-4150-99dc-dd9afacd00b2)
 
 <div align="center">
@@ -51,15 +39,15 @@
 
 ### **GET**
 
 데이터를 불러올 때 사용하는 메소드
 
 ```py
 # get.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 print(jsonly.get(path="기본/사과"))
 ```
 
 ```
 # result
@@ -68,15 +56,15 @@
 
 ### **SET**
 
 데이터를 덮어씌울 때 사용하는 메소드
 
 ```py
 # set.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"기본중에" : "기본"}
 print(jsonly.set(data=data))
 ```
 
@@ -94,15 +82,15 @@
 
 ### **UPDATE**
 
 데이터를 루트 경로에 추가할 때 사용하는 메소드
 
 ```py
 # update.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"새로운" : "데이터"}
 print(jsonly.update(data=data))
 ```
 
@@ -125,15 +113,15 @@
 
 ### **INSERT**
 
 데이터를 특정 경로에 추가할 때 사용하는 메소드
 
 ```py
 # insert.py
-from jsonly.clinet import UseJsonly
+from jsonly.client import UseJsonly
 
 jsonly = UseJsonly(path="data.json")
 
 data = {"데이터" : "삽입"}
 print(jsonly.insert(data=data, path='기본'))
 ```
```

