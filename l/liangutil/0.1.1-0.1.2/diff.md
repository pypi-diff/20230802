# Comparing `tmp/liangutil-0.1.1.tar.gz` & `tmp/liangutil-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.1.1.tar", last modified: Wed Aug  2 03:36:08 2023, max compression
+gzip compressed data, was "liangutil-0.1.2.tar", last modified: Wed Aug  2 08:34:20 2023, max compression
```

## Comparing `liangutil-0.1.1.tar` & `liangutil-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.124914 liangutil-0.1.1/
--rw-rw-rw-   0        0        0     2401 2023-08-02 03:36:08.123984 liangutil-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1139 2023-08-02 03:33:45.000000 liangutil-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.121334 liangutil-0.1.1/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.1/liangutil/__init__.py
--rw-rw-rw-   0        0        0     3521 2023-08-02 03:19:39.000000 liangutil-0.1.1/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     4493 2023-08-02 03:30:18.000000 liangutil-0.1.1/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.1/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     5401 2023-08-02 03:25:07.000000 liangutil-0.1.1/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      527 2023-08-02 03:07:45.000000 liangutil-0.1.1/liangutil/redisutils.py
--rw-rw-rw-   0        0        0    13230 2023-08-02 03:23:38.000000 liangutil-0.1.1/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.122966 liangutil-0.1.1/liangutil.egg-info/
--rw-rw-rw-   0        0        0     2401 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 03:36:08.124914 liangutil-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-08-01 04:05:45.000000 liangutil-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.669622 liangutil-0.1.2/
+-rw-rw-rw-   0        0        0     3495 2023-08-02 08:34:20.669622 liangutil-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2023-08-02 08:22:56.000000 liangutil-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.665558 liangutil-0.1.2/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.2/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3521 2023-08-02 03:19:39.000000 liangutil-0.1.2/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     4495 2023-08-02 08:16:07.000000 liangutil-0.1.2/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.2/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     7717 2023-08-02 08:23:39.000000 liangutil-0.1.2/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      551 2023-08-02 06:39:07.000000 liangutil-0.1.2/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    13258 2023-08-02 06:56:19.000000 liangutil-0.1.2/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:34:20.667621 liangutil-0.1.2/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     3495 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 08:34:20.000000 liangutil-0.1.2/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:34:20.669622 liangutil-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-02 06:28:33.000000 liangutil-0.1.2/setup.py
```

### Comparing `liangutil-0.1.1/README.md` & `liangutil-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 # liangutil包
 
 ![Python](https://img.shields.io/badge/python-3.x-blue.svg)   ![PyPI](https://img.shields.io/pypi/v/liangutil)   ![PyPI - Downloads](https://img.shields.io/pypi/dm/liangutil)   ![GitHub stars](https://img.shields.io/github/stars/Will-Liang/liangutil.svg)
 
 **说明：以Liang开头的类是单独写的类，以Utils结尾的都是基于第三方库封装的。函数详细说明请看代码注释。**
 
+**文档**：https://will-liang.github.io/liangutil/
+
 ## **安装**
 
 ```
 pip install liangutil
 ```
 
 
 
-## 注意
+## 说明
+
+### liangutils
+
+存放一些工具函数
+
+
+
+### requestutils
+
+#### RequestUtils
+
+基于Requests库的封装
+
+#### ChromeUtils
+
+基于selenium库的封装
+
+
+
+### mysqlutils
+
+#### **MySQLUtils**
+
+基于pymysql库的封装
+
+
 
 ### lianglog
 
 #### LiangLog
 
 依赖于 **MySQLUtils**
 
@@ -27,31 +55,60 @@
 | datetime | varchar | 32   |
 | level    | varchar | 32   |
 | name     | varchar | 32   |
 | content  | varchar | 255  |
 
 
 
+### redisutils
+
+#### RedisUtils
+
+基于redis库的封装
+
+
+
+### minioutils
+
+#### MinIOUtils
+
+基于minio库的封装
+
+
+
 # 更新日志
 
 ## 2023年
 
 ### 8月
 
-**2023-08-02** `0.1.1`
+**2023-08-02** 
+
+`0.1.2`
+
+- 更改了RequestUtils中的get、post方法参数列表名称，更符合使用requests库的习惯
+- MySQLUtils增加了 update_datas() 、query_datas_dict_list()
+
+
+
+`0.1.1`
 
 - 统一了代码注释风格
 - 新增代码文档
 - 删除了无用函数
 - 改变了某些函数名称
 
-**2023-08-01** `0.1.0`
+**2023-08-01** 
+
+`0.1.0`
 
 - mysqlutils 中增加了查询等方法
 - 修复了一些 Bug
 
 ### 7月
 
-**2023-07-31** `0.0.8`
+**2023-07-31** 
+
+`0.0.8`
 
 - 第一个发布版本
```

### Comparing `liangutil-0.1.1/liangutil/lianglog.py` & `liangutil-0.1.2/liangutil/lianglog.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.1/liangutil/liangutils.py` & `liangutil-0.1.2/liangutil/liangutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,7 +147,8 @@
         日期字符串
 
     """
     current_date = now.strftime('%Y-%m-%d')  # 2023-04-17
     return current_date
 
 
+
```

### Comparing `liangutil-0.1.1/liangutil/minioutils.py` & `liangutil-0.1.2/liangutil/minioutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.1.1/liangutil/mysqlutils.py` & `liangutil-0.1.2/liangutil/mysqlutils.py`

 * *Files 25% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
             condition(str): 查询条件
 
         Returns:
-            查询结果(元组)，每条记录为一个字典
+            查询结果(元组)，每条记录为一个元组
 
         """
         try:
             cursor = self.conn.cursor()
             if columns is None:
                 columns = []
 
@@ -161,14 +161,45 @@
             return result
         except Exception as e:
             print_log("ERROR",e)
             return None
         finally:
             cursor.close()
 
+    def query_datas_dict_list(self, table_name, columns=None, condition=None):
+        """查询数据
+
+        Args:
+            table_name(str):表名
+            columns(list): 要查询的列名列表，如果为[]，则查询所有列
+            condition(str): 查询条件
+
+        Returns:
+            查询结果: [{},{},{}]
+
+        """
+        try:
+            cursor = self.conn.cursor()
+            if columns is None:
+                columns = []
+
+            columns_str = "*" if len(columns) == 0 else ', '.join(columns)
+            sql = f"SELECT {columns_str} FROM {table_name}"
+            if condition:
+                sql += f" WHERE {condition}"
+            cursor.execute(sql)
+            result = self.fetchall_to_dict_list(cursor)
+            cursor.close()
+            return result
+        except Exception as e:
+            print_log("ERROR",e)
+            return None
+        finally:
+            cursor.close()
+
     def exists_data(self, table_name, columns=None, condition=None):
         """是否存在该数据
 
         Args:
             table_name(str):表名
             columns(list): 要查询的列名列表，如果为[]，则查询所有列
             condition(str): 查询条件
@@ -181,7 +212,50 @@
             columns = []
         if condition is None:
             print_log("WARNING", "You didn't pass in a condition parameter, so it's pointless")
         datas = self.query_data(table_name, columns, condition)
         if datas != None:
             return len(datas) > 0
 
+
+    def update_datas(self, table_name, data, condition=None):
+        """更新数据
+
+        Args:
+            table_name(str): 表名
+            data(dict): 要更新的数据，以字段名为键，字段值为值。
+            condition(str): 更新条件
+
+        Returns:
+            更新成功返回 "True"，失败返回异常
+        """
+        try:
+            cursor = self.conn.cursor()
+
+            # 构建 SQL 更新语句
+            set_columns = ', '.join([f"{column} = %s" for column in data.keys()])
+            sql = f"UPDATE {table_name} SET {set_columns}"
+
+            if condition:
+                sql += f" WHERE {condition}"
+
+            # 执行 SQL 更新
+            cursor.execute(sql, tuple(data.values()))
+
+            # 提交事务
+            self.conn.commit()
+            cursor.close()
+            return "True"
+        except Exception as e:
+            return e
+
+    def fetchall_to_dict_list(self, cursor):
+        """将pymysql的fetchall查询结果转换为装有dict类型的列表
+
+        Args:
+            cursor: pymysql游标对象
+
+        Returns:
+            装有字典类型的列表
+        """
+        column_names = [desc[0] for desc in cursor.description]
+        return [dict(zip(column_names, row)) for row in cursor.fetchall()]
```

### Comparing `liangutil-0.1.1/liangutil/redisutils.py` & `liangutil-0.1.2/liangutil/redisutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,8 +15,10 @@
 
         Args:
             stream_name(str): 流名称
             data(*):数据
 
         """
         self.redis.xadd(stream_name, data)
+
+    def close(self):
         self.redis.close()
```

### Comparing `liangutil-0.1.1/liangutil/requestutils.py` & `liangutil-0.1.2/liangutil/requestutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,38 +77,38 @@
                            "(KHTML, like Gecko)", chrome_version, "Safari/537.36"])
             header["User-Agent"] = ua
         return header
 
 
 
 
-    def get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None):
+    def get(self, url, headers="", retry_count=3, is_response_json=False, time_sleep=1, proxies=None):
         """Get 请求
 
         Args:
             url(str): 请求的url
-            header(str): 请求头
+            headers(str): 请求头
             retry_count(int): 重试次数
             is_response_json(bool): 返回的是否是json
             time_sleep(int): 请求失败后的停止时间
-            proxy(dict): 代理
+            proxies(dict): 代理
 
         Returns:
             {"error": "状态码/异常", "content": "网页源码/json","url": "请求的url"}
 
         """
-        header = header if header else self.get_header(self.is_choice_agent)
+        header = headers if headers else self.get_header(self.is_choice_agent)
         status_code = 200
         while retry_count > 0:
             retry_count = retry_count - 1
             try:
-                if proxy == None and self.proxies == None:
+                if proxies == None and self.proxies == None:
                     resp = requests.get(url,headers=header, timeout=self.timeout, verify=self.is_ssl_verify)
-                elif proxy != None:
-                    resp = requests.get(url, headers=header, proxies=proxy,timeout=self.timeout, verify=self.is_ssl_verify)
+                elif proxies != None:
+                    resp = requests.get(url, headers=header, proxies=proxies,timeout=self.timeout, verify=self.is_ssl_verify)
                 else:
                     resp = requests.get(url, headers=header, proxies=self.proxies, timeout=self.timeout,verify=self.is_ssl_verify)
                 if resp.status_code == 200:
                     return {"error":"",
                             "content":resp.json() if is_response_json else resp.text,
                             "url":resp.url}
                 else:
@@ -122,39 +122,39 @@
                         "url": url}
 
         return {"error": status_code,
                 "content": "",
                 "url": url}
 
 
-    def post(self, url, header="", data=None, retry_count=3, is_response_json=False, time_sleep=1, proxy=None):
+    def post(self, url, headers="", data=None, retry_count=3, is_response_json=False, time_sleep=1, proxies=None):
         """Post 请求
 
         Args:
             url(str): 请求的url
-            header(str): 请求头
+            headers(str): 请求头
             data(dict): payload
             retry_count(int): 重试次数
             is_response_json(bool): 返回的是否是json
             time_sleep(int): 请求失败后的停止时间
-            proxy(dict): 代理
+            proxies(dict): 代理
 
         Returns:
             {"error": "状态码/异常", "content": "网页源码/json","url": "请求的url"}
 
         """
-        header = header if header else self.get_header(self.is_choice_agent)
+        header = headers if headers else self.get_header(self.is_choice_agent)
         status_code = 200
         while retry_count > 0:
             retry_count = retry_count - 1
             try:
-                if proxy == None and self.proxies == None:
+                if proxies == None and self.proxies == None:
                     resp = requests.post(url,headers=header, data=data, timeout=self.timeout, verify=self.is_ssl_verify)
-                elif proxy != None:
-                    resp = requests.post(url, headers=header, data=data, proxies=proxy,timeout=self.timeout, verify=self.is_ssl_verify)
+                elif proxies != None:
+                    resp = requests.post(url, headers=header, data=data, proxies=proxies,timeout=self.timeout, verify=self.is_ssl_verify)
                 else:
                     resp = requests.post(url, headers=header, data=data, proxies=self.proxies, timeout=self.timeout,verify=self.is_ssl_verify)
                 if resp.status_code == 200:
                     return {"error":"",
                             "content":resp.json() if is_response_json else resp.text,
                             "url":resp.url}
                 else:
```

### Comparing `liangutil-0.1.1/setup.py` & `liangutil-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.1.1',
+    version='0.1.2',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

