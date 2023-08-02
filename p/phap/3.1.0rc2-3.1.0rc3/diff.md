# Comparing `tmp/phap-3.1.0rc2.tar.gz` & `tmp/phap-3.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-3.1.0rc2.tar", last modified: Tue Aug  1 14:11:02 2023, max compression
+gzip compressed data, was "phap-3.1.0rc3.tar", last modified: Wed Aug  2 01:01:46 2023, max compression
```

## Comparing `phap-3.1.0rc2.tar` & `phap-3.1.0rc3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.467963 phap-3.1.0rc2/
--rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0rc2/LICENSE
--rw-rw-rw-   0        0        0     2502 2023-08-01 14:11:02.467963 phap-3.1.0rc2/PKG-INFO
--rw-rw-rw-   0        0        0     1702 2023-08-01 01:31:55.000000 phap-3.1.0rc2/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0rc2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 14:11:02.467963 phap-3.1.0rc2/setup.cfg
--rw-rw-rw-   0        0        0     1686 2023-08-01 14:06:26.000000 phap-3.1.0rc2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.377099 phap-3.1.0rc2/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.441248 phap-3.1.0rc2/src/algo/
--rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0rc2/src/algo/__init__.py
--rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0rc2/src/algo/arraylib.py
--rw-rw-rw-   0        0        0     4538 2023-07-31 04:28:39.000000 phap-3.1.0rc2/src/algo/treelib.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.443247 phap-3.1.0rc2/src/cahap/
--rw-rw-rw-   0        0        0     1160 2023-08-01 14:05:58.000000 phap-3.1.0rc2/src/cahap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.444251 phap-3.1.0rc2/src/phap/
--rw-rw-rw-   0        0        0      107 2023-08-01 13:59:56.000000 phap-3.1.0rc2/src/phap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.452354 phap-3.1.0rc2/src/phap.egg-info/
--rw-rw-rw-   0        0        0     2502 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-08-01 14:11:02.000000 phap-3.1.0rc2/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.453861 phap-3.1.0rc2/src/phapbm/
--rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0rc2/src/phapbm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.458867 phap-3.1.0rc2/src/stralgo/
--rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.461866 phap-3.1.0rc2/src/stralgo/hash/
--rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/sha.py
-drwxrwxrwx   0        0        0        0 2023-08-01 14:11:02.464964 phap-3.1.0rc2/src/stralgo/hash/sm/
--rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/hash/sm/__init__.py
--rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0rc2/src/stralgo/hash/sm/sm3libs.py
--rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0rc2/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.096719 phap-3.1.0rc3/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-3.1.0rc3/LICENSE
+-rw-rw-rw-   0        0        0     2502 2023-08-02 01:01:46.095720 phap-3.1.0rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     1702 2023-08-02 00:45:55.000000 phap-3.1.0rc3/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-3.1.0rc3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 01:01:46.096719 phap-3.1.0rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2023-08-02 00:46:13.000000 phap-3.1.0rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:45.928348 phap-3.1.0rc3/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:45.990549 phap-3.1.0rc3/src/algo/
+-rw-rw-rw-   0        0        0      210 2023-07-23 04:55:40.000000 phap-3.1.0rc3/src/algo/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-07-25 04:12:52.000000 phap-3.1.0rc3/src/algo/arraylib.py
+-rw-rw-rw-   0        0        0     4702 2023-08-02 00:57:00.000000 phap-3.1.0rc3/src/algo/treelib.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:45.992557 phap-3.1.0rc3/src/cahap/
+-rw-rw-rw-   0        0        0     1160 2023-08-01 14:05:58.000000 phap-3.1.0rc3/src/cahap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.019115 phap-3.1.0rc3/src/phap/
+-rw-rw-rw-   0        0        0      107 2023-08-01 13:59:56.000000 phap-3.1.0rc3/src/phap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.037281 phap-3.1.0rc3/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     2502 2023-08-02 01:01:45.000000 phap-3.1.0rc3/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-08-02 01:01:45.000000 phap-3.1.0rc3/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 01:01:45.000000 phap-3.1.0rc3/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-08-02 01:01:45.000000 phap-3.1.0rc3/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.039281 phap-3.1.0rc3/src/phapbm/
+-rw-rw-rw-   0        0        0     1013 2023-07-24 11:41:34.000000 phap-3.1.0rc3/src/phapbm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.069784 phap-3.1.0rc3/src/stralgo/
+-rw-rw-rw-   0        0        0      718 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.073785 phap-3.1.0rc3/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      354 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      508 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:01:46.076302 phap-3.1.0rc3/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0      148 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6943 2023-07-24 11:35:14.000000 phap-3.1.0rc3/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      233 2023-07-23 04:55:41.000000 phap-3.1.0rc3/src/stralgo/json.py
```

### Comparing `phap-3.1.0rc2/LICENSE` & `phap-3.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/PKG-INFO` & `phap-3.1.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0rc2
+Version: 3.1.0rc3
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc2
++ v3.1.0-rc3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc2/README.md` & `phap-3.1.0rc3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc2
++ v3.1.0-rc3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc2/setup.py` & `phap-3.1.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="3.1.0rc2",  #版本
+    version="3.1.0rc3",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-3.1.0rc2/src/algo/arraylib.py` & `phap-3.1.0rc3/src/algo/arraylib.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/src/algo/treelib.py` & `phap-3.1.0rc3/src/algo/treelib.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,34 +17,38 @@
         self.left = left  # 将本类初始节点的左右侧分别赋值
         self.right = right
 
     def setfromlist(self, val:list) -> None:  # 支持从列表设置本二叉树的函数，结构为[参数,左,右]，可嵌套
         '''To set the node from list'''
         self.val = val[0]  # 设置本类初始节点参数
         if str(type(val[1])) == str(type([])):  # 如果初始节点左侧是嵌套的列表
-            self.left = treenode().setfromlist(val[1])  # 则创建一个新的本类实例，并将所得列表传参给实例的本函数，并将本类左侧参数赋值
+            tmpo = treenode()  # 则创建一个新的本类实例，并将所得列表传参给实例的本函数，并将本类左侧参数赋值
+            tmpo.setfromlist(val[1])
+            self.left = tmpo
         else:
             self.left = val[1]
         if str(type(val[2])) == str(type([])):  # 原理同上
-            self.right = treenode().setfromlist(val[2])
+            tmpo = treenode()
+            tmpo.setfromlist(val[2])
+            self.right = tmpo
         else:
             self.right = val[2]
 
-    def __eq__(self, value:object) -> bool:  # 简化赋值的运算符重载
-        try:
-            if str(type(value)) in self.__t:  # 如果赋值表达式的右值为二叉树类
-                self.val = value.val  # 从该类获取必要信息并赋值本类
-                self.left = value.left
-                self.right = value.right
-            else:  # 否则调用setfromlist函数
-                self.setfromlist(value)
-        except:
-            return(False)
-        else:
-            return(True)
+    #def __eq__(self, value:object) -> bool:  # 简化赋值的运算符重载
+    #    try:
+    #        if str(type(value)) in self.__t:  # 如果赋值表达式的右值为二叉树类
+    #            self.val = value.val  # 从该类获取必要信息并赋值本类
+    #            self.left = value.left
+    #            self.right = value.right
+    #        else:  # 否则调用setfromlist函数
+    #            self.setfromlist(value)
+    #    except:
+    #        return(False)
+    #    else:
+    #        return(True)
     
     #def __setattr__(self, __name: str, __value: Any) -> None:  # 用于对一些关键的常量禁止赋值
     #    pass
 
     def get_list(self) -> list:  # 从本类获得列表（结构同上）
         l = []  # 定义一个临时的列表
         l.append(self.val)  # 将初始节点参数加入列表
@@ -86,17 +90,18 @@
         else:
             rd += 1
         return(max(ld, rd))  # 返回左右中的最大值
 
     def get_depth(self) -> int:  # 对于depth只读属性的函数封装
         return(self.depth)
     
-    #@property
-    #def node(self) -> str:  # 返回一个简洁明了的二叉树字符串
-    #    #l = self.getlist()
-    #    return("")
+    @property
+    def node(self) -> str:  # 返回一个简洁明了的二叉树字符串
+        #l = self.getlist()
+        #return("")
+        return(str(self.listdata))  # 临时如此实现，后续改进
     
-    #def getnode(self) -> str:
-    #    return(self.node)
+    def getnode(self) -> str:
+        return(self.node)
 
-    #def __str__(self) -> str:  # 使开发者可以直接使用print函数打印二叉树
-    #    return(self.node)
+    def __str__(self) -> str:  # 使开发者可以直接使用print函数打印二叉树
+        return(self.node)
```

### Comparing `phap-3.1.0rc2/src/cahap/__init__.py` & `phap-3.1.0rc3/src/cahap/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/src/phap.egg-info/PKG-INFO` & `phap-3.1.0rc3/src/phap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 3.1.0rc2
+Version: 3.1.0rc3
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -38,15 +38,15 @@
 + v2.2.1
 
 ## Latest Available Version
 + v3.0.0
 
 ## Latest Version
 ### *(The data under the master branch is inaccurate. Please refer to the dev branch for details)*
-+ v3.1.0-rc2
++ v3.1.0-rc3
 
 # To Use
 ## Read our development document
 ### *(Click the [Github](https://github.com/DashBing/phap/ "Github") link to read this document，or you may can not to open the link)*
 + [Development Document](doc/README.md)
 
 # Build
```

### Comparing `phap-3.1.0rc2/src/phapbm/__init__.py` & `phap-3.1.0rc3/src/phapbm/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/src/stralgo/__init__.py` & `phap-3.1.0rc3/src/stralgo/__init__.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/src/stralgo/base.py` & `phap-3.1.0rc3/src/stralgo/base.py`

 * *Files identical despite different names*

### Comparing `phap-3.1.0rc2/src/stralgo/hash/sm/sm3libs.py` & `phap-3.1.0rc3/src/stralgo/hash/sm/sm3libs.py`

 * *Files identical despite different names*

