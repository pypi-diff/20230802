# Comparing `tmp/liangutil-0.1.0.tar.gz` & `tmp/liangutil-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.1.0.tar", last modified: Tue Aug  1 03:31:58 2023, max compression
+gzip compressed data, was "liangutil-0.1.1.tar", last modified: Wed Aug  2 03:36:08 2023, max compression
```

## Comparing `liangutil-0.1.0.tar` & `liangutil-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.415410 liangutil-0.1.0/
--rw-rw-rw-   0        0        0     4775 2023-08-01 03:31:58.415410 liangutil-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2953 2023-08-01 03:31:28.000000 liangutil-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.412384 liangutil-0.1.0/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.0/liangutil/__init__.py
--rw-rw-rw-   0        0        0     2927 2023-07-31 10:15:04.000000 liangutil-0.1.0/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     3595 2023-08-01 03:30:49.000000 liangutil-0.1.0/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     2256 2023-07-31 10:15:21.000000 liangutil-0.1.0/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     4893 2023-08-01 03:26:27.000000 liangutil-0.1.0/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.1.0/liangutil/redisutils.py
--rw-rw-rw-   0        0        0     9965 2023-07-31 10:13:08.000000 liangutil-0.1.0/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-08-01 03:31:58.414413 liangutil-0.1.0/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4775 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 03:31:58.000000 liangutil-0.1.0/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 03:31:58.415410 liangutil-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-08-01 03:31:54.000000 liangutil-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.124914 liangutil-0.1.1/
+-rw-rw-rw-   0        0        0     2401 2023-08-02 03:36:08.123984 liangutil-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1139 2023-08-02 03:33:45.000000 liangutil-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.121334 liangutil-0.1.1/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.1.1/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3521 2023-08-02 03:19:39.000000 liangutil-0.1.1/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     4493 2023-08-02 03:30:18.000000 liangutil-0.1.1/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     1318 2023-08-02 03:25:24.000000 liangutil-0.1.1/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     5401 2023-08-02 03:25:07.000000 liangutil-0.1.1/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 03:07:45.000000 liangutil-0.1.1/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    13230 2023-08-02 03:23:38.000000 liangutil-0.1.1/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:36:08.122966 liangutil-0.1.1/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     2401 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 03:36:08.000000 liangutil-0.1.1/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 03:36:08.124914 liangutil-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-08-01 04:05:45.000000 liangutil-0.1.1/setup.py
```

### Comparing `liangutil-0.1.0/liangutil/lianglog.py` & `liangutil-0.1.1/liangutil/lianglog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-
+# -*- coding: utf-8 -*-
 from liangutil.liangutils import *
 from liangutil.mysqlutils import MySQLUtils
 
 
 class LiangLog:
+    """
+    LiangLog 记录日志类
+    """
+
     def __init__(self, name, is_print_console=True,is_record_file=False,is_record_db=False, dir_path=None, db_host=None, db_port=None, db_user=None, db_pass=None, db_name=None):
         # name 程序名称
         self.name = name
 
         # is_print_console 是否打印到控制台
         # is_record_file 是否记录到文件中
         # is_record_db 是否记录到mysql中
@@ -31,40 +35,69 @@
             # content        varchar  255
             self.mysql = MySQLUtils(db_host, db_port, db_user, db_pass, db_name)
 
             if self.mysql.check_table_exist("program_logs") == False:
                 raise Exception("program_logs 数据表不存在")
 
 
-    # level等级：WARNING, INFO , ERROR
-    # content输出内容
     def print_log(self, level, content):
+        """打印日志到控制台
+
+        Args:
+            level(str): 等级(WARNING, INFO , ERROR)
+            content(str): 日志信息
+
+        """
         formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-4),content)
         log = "{} {} {}".format(level,get_nowdatetime(),formatted_log)
         print(log)
 
 
-    # 将日志输出到文件
+
     def record_log_to_file(self,level, content):
+        """将日志记录到文件
+
+        Args:
+            level(str): 等级(WARNING, INFO , ERROR)
+            content(str): 日志信息
+
+        """
         now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
-        file_path = os.path.join(self.dir_path, self.name + "_logs", get_nowdate(now), level+get_nowtime(now)+".log")
+        file_path = os.path.join(
+            self.dir_path,
+            f"{self.name}_logs",
+            get_nowdate(now),
+            level + get_nowtime(now) + ".log",
+        )
         check_path(file_path)
         with open(file_path, "a", encoding="utf-8") as f:
             formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-4), content)
-            log = "{} {} {}".format(level, get_nowdatetime(), formatted_log)
+            log = f"{level} {get_nowdatetime()} {formatted_log}"
             f.write(log+"\n")
 
 
     def record_log_to_db(self, level, content):
-        now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
+        """将日志记录到mysql
+
+        Args:
+            level(str): 等级(WARNING, INFO , ERROR)
+            content(str): 日志信息
+
+        """
         formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-4), content)
         self.mysql.insert_data("program_logs", {"datetime":get_nowdatetime(), "level":level, "name":self.name, "content":formatted_log})
 
 
-    # 推荐调用这个方法
     def record_log(self, level, content):
+        """记录日志总方法(推荐使用)
+
+        Args:
+            level(str): 等级(WARNING, INFO , ERROR)
+            content(str): 日志信息
+
+        """
         if self.is_print_console:
             self.print_log(level, content)
         if self.is_record_file:
             self.record_log_to_file(level, content)
         if self.is_record_db:
             self.record_log_to_db(level, content)
```

### Comparing `liangutil-0.1.0/liangutil/liangutils.py` & `liangutil-0.1.1/liangutil/liangutils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,47 @@
+# -*- coding: utf-8 -*-
 import datetime
 import os
 import re
 import traceback
 
 import pytz
 
+"""
+liangutils 中存放一些工具方法
+"""
 
-# 判断是否为文件路径
-# 相对路径不要使用 ./ 开头
 def is_filepath(path):
+    """判断是否为文件路径
+
+    相对路径不要使用 ./ 开头
+
+    Args:
+        path: 路径
+
+    Returns:
+        包含文件名称的路径返回 True，否则返回 False
+
+    '"""
     pattern = r'\.[a-zA-Z]+$'  # 匹配以.开头，后面跟着至少一个字符的字符串
     return bool(re.search(pattern, path))
 
-# 如果是文件路径，提取父级目录路径
-# 相对路径不要使用 ./ 开头
+
 def get_dirpath(path):
+    """获得目录路径
+
+    如果是文件路径，提取父级目录路径（相对路径不要使用 ./ 开头）
+
+    Args:
+        path: 路径
+
+    Returns:
+        目录路径
+
+    """
     # 是文件路径，需要提取父级目录路径
     if is_filepath(path):
         # 获取当前操作系统的文件目录分隔符
         separator = os.sep
 
         # 有父级目录
         if str(path).rfind(".") != -1 and str(path).rfind(separator) != -1:
@@ -28,63 +51,103 @@
             return ""
         else:
             return ""
     else:
         return path
 
 
-# 检查目录是否存在
 def check_path(path):
+    """检查目录是否存在
+
+    如果目录不存在创建目录
+
+    Args:
+        path: 路径
+
+    Returns:
+        路径
+
+    """
     dirpath = get_dirpath(path)
     if dirpath != "" and not os.path.exists(dirpath):
         os.makedirs(dirpath)
     return path
 
 
-# 打印日志
 def print_log(level, content):
+    """打印日志
+
+    Args:
+        level: 日志等级
+        content: 信息
+
+    """
     formatted_log = "{} EXCEPTION: {}".format(code_location(depth=-2), content)
     printlog = "{} {} {}".format(level,get_nowdatetime(),formatted_log)
     print(printlog)
 
 
-
-# 得到调用该方法的文件名称和 代码行号
-# depth: 如果直接得到调用该方法的代码在哪里，传递-2
 def code_location(depth=-2):
-  stack = traceback.extract_stack()
-  filename, lineno, _, _ = stack[depth]
-  # 在 Python 中，traceback.extract_stack() 函数返回当前的调用栈信息。调用栈是一个包含多个元组的列表，每个元组表示一帧（frame）的信息。每一帧都对应着一次函数调用，包含了函数所在的文件名、行号、函数名等信息。
-  # 通常，调用栈列表的最后一帧是当前代码所在的位置，也就是 code_location() 函数本身的位置。而在 traceback.extract_stack() 返回的列表中，最后一帧的索引是 -1。而倒数第二帧的索引是 -2，依此类推。
-  # 所以在代码中的 stack[-2] 就表示获取调用栈列表中倒数第二帧的信息，即 code_location() 函数被调用的位置所在的帧。然后从这个帧中获取文件名和行号信息，最终返回文件名和行号组成的字符串。
-  # 注意：traceback.extract_stack() 函数会返回完整的调用栈信息，包含当前函数的调用。如果你在其他函数中调用了 code_location()，那么它返回的文件名和行号将是调用它的位置。
-  return filename+" line:"+str(lineno)
+    """得到调用该方法的文件名称和 代码行号
+
+    Args:
+        depth: 如果直接得到调用该方法的代码在哪里，传递-2
+
+    Returns:
+        {调用该方法的pytho文件名} line {行号}
+    """
+    stack = traceback.extract_stack()
+    filename, lineno, _, _ = stack[depth]
+    # 在 Python 中，traceback.extract_stack() 函数返回当前的调用栈信息。调用栈是一个包含多个元组的列表，每个元组表示一帧（frame）的信息。每一帧都对应着一次函数调用，包含了函数所在的文件名、行号、函数名等信息。
+    # 通常，调用栈列表的最后一帧是当前代码所在的位置，也就是 code_location() 函数本身的位置。而在 traceback.extract_stack() 返回的列表中，最后一帧的索引是 -1。而倒数第二帧的索引是 -2，依此类推。
+    # 所以在代码中的 stack[-2] 就表示获取调用栈列表中倒数第二帧的信息，即 code_location() 函数被调用的位置所在的帧。然后从这个帧中获取文件名和行号信息，最终返回文件名和行号组成的字符串。
+    # 注意：traceback.extract_stack() 函数会返回完整的调用栈信息，包含当前函数的调用。如果你在其他函数中调用了 code_location()，那么它返回的文件名和行号将是调用它的位置。
+    return filename+" line:"+str(lineno)
 
 
-# 获得现在的日期时间
 def get_nowdatetime():
+    """获得亚洲上海时区现在的日期时间
+
+    Returns:
+        时间字符串
+
+    """
     now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
     current_date = now.strftime('%Y-%m-%d')  # 2023-04-17
     current_hour = now.strftime('%H')
     current_min = now.strftime('%M')
     current_sec = now.strftime('%S')
     nowdatetime = current_date + " " + current_hour + ":" + current_min + ":" + current_sec
     return nowdatetime
 
 
-# 获得现在的时间
-# now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
 def get_nowtime(now):
+    """获得现在的时间
+
+    Args:
+        now: now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
+
+    Returns:
+        数据字符串
+
+    """
     current_hour = now.strftime('%H')
     current_min = now.strftime('%M')
     current_sec = now.strftime('%S')
     time = current_hour + ":" + current_min + ":" + current_sec
     return time
 
 
-# 获得现在的日期
-# now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
 def get_nowdate(now):
+    """获得现在的日期
+
+    Args:
+        now: now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
+
+    Returns:
+        日期字符串
+
+    """
     current_date = now.strftime('%Y-%m-%d')  # 2023-04-17
     return current_date
```

### Comparing `liangutil-0.1.0/liangutil/mysqlutils.py` & `liangutil-0.1.1/liangutil/mysqlutils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,32 @@
+# -*- coding: utf-8 -*-
 import pymysql
 
 from liangutil.liangutils import print_log
 
 
+
 class MySQLUtils:
+    """
+    MySQLUtils 基于 pymysql 库进行封装
+    """
     def __init__(self, host, port, username, password, database):
         self.conn = pymysql.connect(host=host,port=port, user=username, password=password, database=database)
 
 
-    # 检查表是否存在
     def check_table_exist(self, table_name):
+        """根据表名检查表是否存在
+
+        Args:
+            table_name(str):表名
+
+        Returns:
+            存在返回True，否则返回False
+
+        """
         cursor = self.conn.cursor()
         try:
             sql = "show tables like '{}'".format(table_name)
             cursor.execute(sql)
             result = cursor.fetchone()
             if result:
                 return True
@@ -22,23 +35,26 @@
 
         except Exception as e:
             print_log("ERROR",e)
         finally:
             cursor.close()
 
 
-    # 向数据库中插入一条记录
-    # 插入成功返回"True"
     def insert_data(self, table_name, data: dict):
+        """插入一条数据
+
+        Args:
+            table_name(str):表名
+            data(dict):要插入的数据，以字段名为键，字段值为值。
+
+        Returns:
+            插入成功返回"True"，错误返回异常
+
         """
-        向数据库中插入一条记录
-        :param table_name: 表名
-        :param data:(dict)要插入的数据，以字段名为键，字段值为值。
-        :return:
-        """
+
         try:
             cursor = self.conn.cursor()
             # 构建 SQL 插入语句
             columns = ', '.join(data.keys())
             values = ', '.join(['%s'] * len(data))
             sql = f"insert into {table_name} ({columns}) values ({values})"
 
@@ -47,23 +63,27 @@
             self.conn.commit()
 
             cursor.close()
             return "True"
         except Exception as e:
             return e
 
-    # 向数据库中插入多条记录
-    # 插入成功返回 "True"
+
     def insert_datas(self, table_name, data_list: list):
+        """插入一条数据
+
+        Args:
+            table_name(str):表名
+            data(list):要插入的数据列表，以字段名为键，字段值为值。
+
+        Returns:
+            插入成功返回"True"，错误返回异常
+
         """
-        向数据库中插入多条记录
-        :param table_name: 表名
-        :param data_list: (list) 要插入的数据列表，每个元素是一个字典，以字段名为键，字段值为值。
-        :return: 成功返回 "True"
-        """
+
         try:
             cursor = self.conn.cursor()
             columns = ', '.join(data_list[0].keys())  # 假设所有字典的键相同
             values_template = ', '.join(['%s'] * len(data_list[0]))
 
             # 构建 SQL 批量插入语句
             sql = f"insert into {table_name} ({columns}) values ({values_template})"
@@ -77,21 +97,26 @@
             cursor.close()
             return "True"
         except Exception as e:
             return e
 
 
     def query_data(self, table_name, columns=[], condition=None):
+        """随机查询单条数据
+
+        Args:
+            table_name(str):表名
+            columns(list): 要查询的列名列表，如果为[]，则查询所有列
+            condition(str): 查询条件
+
+        Returns:
+            查询结果
+
         """
-        查询数据的方法
-        :param table_name: 表名
-        :param columns: 要查询的列名列表，如果为[]，则查询所有列
-        :param condition: 查询条件，可以为 None
-        :return: 随机返回一条结果，结果是字典
-        """
+
         try:
             cursor = self.conn.cursor()
 
             if len(columns) == 0:
                 columns_str = "*"
             else:
                 columns_str = ', '.join(columns)
@@ -99,25 +124,31 @@
             sql = f"SELECT {columns_str} FROM {table_name}"
             if condition:
                 sql += f" WHERE {condition} order by rand() limit 1"
             cursor.execute(sql)
             result = cursor.fetchone()[0]
             cursor.close()
             return result
-        except:
-            cursor.close()
+        except Exception as e:
+            print_log("ERROR", e)
             return None
+        finally:
+            cursor.close()
 
     def query_datas(self, table_name, columns=None, condition=None):
-        """
-        查询数据的方法
-        :param table_name: 表名
-        :param columns: 要查询的列名列表，如果为[]，则查询所有列
-        :param condition: 查询条件，可以为 None
-        :return:查询结果元组，每条记录为一个字典
+        """查询数据
+
+        Args:
+            table_name(str):表名
+            columns(list): 要查询的列名列表，如果为[]，则查询所有列
+            condition(str): 查询条件
+
+        Returns:
+            查询结果(元组)，每条记录为一个字典
+
         """
         try:
             cursor = self.conn.cursor()
             if columns is None:
                 columns = []
 
             columns_str = "*" if len(columns) == 0 else ', '.join(columns)
@@ -131,14 +162,25 @@
         except Exception as e:
             print_log("ERROR",e)
             return None
         finally:
             cursor.close()
 
     def exists_data(self, table_name, columns=None, condition=None):
+        """是否存在该数据
+
+        Args:
+            table_name(str):表名
+            columns(list): 要查询的列名列表，如果为[]，则查询所有列
+            condition(str): 查询条件
+
+        Returns:
+            存在True，否则False
+
+        """
         if columns is None:
             columns = []
         if condition is None:
             print_log("WARNING", "You didn't pass in a condition parameter, so it's pointless")
         datas = self.query_data(table_name, columns, condition)
         if datas != None:
             return len(datas) > 0
```

### Comparing `liangutil-0.1.0/liangutil/requestutils.py` & `liangutil-0.1.1/liangutil/requestutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,57 @@
+# -*- coding: utf-8 -*-
 import platform
 import random
 import time
 
 import requests
 
 from selenium.webdriver.chrome.options import Options
 
 from selenium import webdriver
 
 from liangutil.liangutils import print_log, get_nowdatetime
 
+"""
+requestutils 中封装了爬虫的类以及方法
+"""
+
 # 封装requests请求
 class RequestUtils:
+    """
+    RequestUtils 基于 requests 库进行的封装
+    """
 
     def __init__(self, timeout:int, is_ssl_verify: bool, is_choice_agent:bool = True, proxies=None):
+        """
+        初始化 RequestUtils
+
+        Args:
+            timeout(int): 请求超时时间
+            is_ssl_verify(bool): 是否验证 SSL 证书
+            is_choice_agent(bool): 是否随机 USER-AGENT
+            proxies(dict): 代理字典
+        """
         self.timeout = timeout # 请求超时时间
         self.is_ssl_verify = is_ssl_verify # 是否验证SSL证书
         self.is_choice_agent = is_choice_agent # 是否随机AGENT
+
         # 该参数代理是为了需要用固定ip的爬虫
         self.proxies = proxies   # {'http': 'http://xxx', 'https': 'https://xxx'}
 
     def get_header(self,is_choice_agent=False):
+        """获得 USER-AGENT
+
+        Args:
+            is_choice_agent(bool): 是否随机 USER-AGENT
+
+        Returns:
+            USER-AGENT
+
+        """
         header = {
             # "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
             "Accept":"*/*",
             "Accept-Language": "zh-CN,zh;q=0.9",
             "Cache-Control": "max-age=0",
             "Accept-Encoding": "gzip, deflate",  # 使用gzip压缩传输数据让访问更快
             "User-Agent": "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.122 Safari/537.36",
@@ -48,21 +75,31 @@
                             ]
             ua = " ".join([random.choice(browser_type), random.choice(os_type), "AppleWebKit/537.36",
                            "(KHTML, like Gecko)", chrome_version, "Safari/537.36"])
             header["User-Agent"] = ua
         return header
 
 
-    # Get请求
-    # 返回{
-    #   "error": "", 错误信息
-    #    "content": "",返回的内容
-    #    "url": "" 请求的url
-    # }
+
+
     def get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None):
+        """Get 请求
+
+        Args:
+            url(str): 请求的url
+            header(str): 请求头
+            retry_count(int): 重试次数
+            is_response_json(bool): 返回的是否是json
+            time_sleep(int): 请求失败后的停止时间
+            proxy(dict): 代理
+
+        Returns:
+            {"error": "状态码/异常", "content": "网页源码/json","url": "请求的url"}
+
+        """
         header = header if header else self.get_header(self.is_choice_agent)
         status_code = 200
         while retry_count > 0:
             retry_count = retry_count - 1
             try:
                 if proxy == None and self.proxies == None:
                     resp = requests.get(url,headers=header, timeout=self.timeout, verify=self.is_ssl_verify)
@@ -85,31 +122,89 @@
                         "url": url}
 
         return {"error": status_code,
                 "content": "",
                 "url": url}
 
 
+    def post(self, url, header="", data=None, retry_count=3, is_response_json=False, time_sleep=1, proxy=None):
+        """Post 请求
+
+        Args:
+            url(str): 请求的url
+            header(str): 请求头
+            data(dict): payload
+            retry_count(int): 重试次数
+            is_response_json(bool): 返回的是否是json
+            time_sleep(int): 请求失败后的停止时间
+            proxy(dict): 代理
+
+        Returns:
+            {"error": "状态码/异常", "content": "网页源码/json","url": "请求的url"}
+
+        """
+        header = header if header else self.get_header(self.is_choice_agent)
+        status_code = 200
+        while retry_count > 0:
+            retry_count = retry_count - 1
+            try:
+                if proxy == None and self.proxies == None:
+                    resp = requests.post(url,headers=header, data=data, timeout=self.timeout, verify=self.is_ssl_verify)
+                elif proxy != None:
+                    resp = requests.post(url, headers=header, data=data, proxies=proxy,timeout=self.timeout, verify=self.is_ssl_verify)
+                else:
+                    resp = requests.post(url, headers=header, data=data, proxies=self.proxies, timeout=self.timeout,verify=self.is_ssl_verify)
+                if resp.status_code == 200:
+                    return {"error":"",
+                            "content":resp.json() if is_response_json else resp.text,
+                            "url":resp.url}
+                else:
+                    status_code = resp.status_code
+                    time.sleep(time_sleep)
+
+
+            except Exception as e:
+                return {"error": e,
+                        "content": "",
+                        "url": url}
+
+        return {"error": status_code,
+                "content": "",
+                "url": url}
+
+
 # https://selenium-python.readthedocs.io/page-objects.html
 # https://www.selenium.dev/zh-cn/documentation/
 # 封装 selenium
 class ChromeUtils:
+    """
+    ChromeUtils 基于 selenium 库进行的封装
+    """
     def __init__(self, timeout: int, is_ssl_verify: bool=False, is_chrome_headless:bool = False, is_undetected_chromedriver:bool = False, proxy=None):
         self.timeout = timeout  # 请求超时时间
         self.is_ssl_verify = is_ssl_verify  # 是否验证SSL证书
         self.is_chrome_headless = is_chrome_headless # Linux下 is_chrome_headless为True
         self.is_undetected_chromedriver = is_undetected_chromedriver
 
         # 该参数代理是为了需要用固定ip的爬虫
         self.proxy = proxy # http://xxxxxx
         self.driver = self.get_chrome_driver(proxy)
 
 
-    # 获得一个chrome驱动
+
     def get_chrome_driver(self, proxy=None):
+        """获得一个chrome驱动
+
+        Args:
+            proxy(str): 代理
+
+        Returns:
+            chrome驱动
+
+        """
         try:
             chrome_options = Options()
 
             if proxy != None:
                 chrome_options.add_argument("--proxy-server="+proxy)
             elif self.proxy != None:
                 chrome_options.add_argument("--proxy-server="+self.proxy)
@@ -149,66 +244,80 @@
             driver.set_script_timeout(self.timeout) # 设置脚本执行超时时间。
 
             return driver
 
         except Exception as e:
             return None
 
-    # 重启浏览器
+
     def refresh_chrome(self):
+        """重启浏览器
+
+        Returns:
+            重启成功返回True，否则返回False
+
+        """
         retry_time = 3
         time_sleep = 10
         error = ""
         while retry_time:
             try:
                 if self.driver:
                     self.driver.quit()
                 self.driver = self.get_chrome_driver()
                 return True
             except Exception as e:
-                retry_time = retry_time - 1
+                retry_time -= 1
                 error = str(e)
                 time.sleep(time_sleep)
         print_log("ERROR", error)
         return False
 
 
-    # 获得网页源码
+
     def get_page_source(self, url, time_sleep=0):
-        print("{} Get {}".format(get_nowdatetime(), url))
+        """获得网页源码
 
-        if self.driver == None:
+        Args:
+            url(str): 请求的url
+            time_sleep(int): 页面会在time_sleep时间后获得源码
+
+        Returns:
+            {"error":"异常","content":"网页源码","url":"请求的url"}
+
+        """
+
+        print(f"{get_nowdatetime()} Get {url}")
+
+        if self.driver is None:
             return {"error":"ZWChrome 的 driver 为空",
                     "content":"",
                     "url":url}
         try:
             self.driver.get(url)
 
         except Exception as e:
             if str(e).startswith("Message: timeout:") and self.driver.page_source:
                 return {"error": "",
                         "content": self.driver.page_source,
                         "url": self.driver.current_url}
 
-            if self.refresh_chrome():
-                try:
-                    self.driver.get(url)
-                except Exception as e:
-                    self.driver.execute("window.stop()")
-                    return {"error":e,
-                            "content":"",
-                            "url":url}
-            else:
+            if not self.refresh_chrome():
                 return {"error": "重启chrome失败","content": "","url": url}
 
+            try:
+                self.driver.get(url)
+            except Exception as e:
+                self.driver.execute("window.stop()")
+                return {"error":e,
+                        "content":"",
+                        "url":url}
         time.sleep(time_sleep)
 
-        text = self.driver.page_source
-
-        if text:
+        if text := self.driver.page_source:
             return {"error": "",
                     "content": text,
                     "url": self.driver.current_url}
         else:
             return {"error": "没有获得 page_source",
                     "content": "",
                     "url": self.driver.current_url}
```

### Comparing `liangutil-0.1.0/setup.py` & `liangutil-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.1.0',
+    version='0.1.1',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

