# Comparing `tmp/yyszh-0.1.0.tar.gz` & `tmp/yyszh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yyszh-0.1.0.tar", last modified: Mon Jul 10 01:14:10 2023, max compression
+gzip compressed data, was "dist\yyszh-0.1.1.tar", last modified: Wed Aug  2 03:22:22 2023, max compression
```

## Comparing `yyszh-0.1.0.tar` & `yyszh-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 01:14:10.000000 yyszh-0.1.0/
--rw-rw-rw-   0        0        0      160 2023-07-10 01:14:10.000000 yyszh-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 01:14:10.000000 yyszh-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      470 2023-07-10 01:10:44.000000 yyszh-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:14:10.000000 yyszh-0.1.0/yyszh/
--rw-rw-rw-   0        0        0     1809 2023-07-10 00:57:50.000000 yyszh-0.1.0/yyszh/__init__.py
--rw-rw-rw-   0        0        0    23742 2023-07-10 00:58:25.000000 yyszh-0.1.0/yyszh/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 01:14:10.000000 yyszh-0.1.0/yyszh.egg-info/
--rw-rw-rw-   0        0        0      160 2023-07-10 01:14:09.000000 yyszh-0.1.0/yyszh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-10 01:14:09.000000 yyszh-0.1.0/yyszh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 01:14:09.000000 yyszh-0.1.0/yyszh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-07-10 01:14:09.000000 yyszh-0.1.0/yyszh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-10 01:14:09.000000 yyszh-0.1.0/yyszh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/
+-rw-rw-rw-   0        0        0      157 2023-08-02 03:22:22.000000 yyszh-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2023-07-04 11:22:41.000000 yyszh-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 03:22:22.000000 yyszh-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      558 2023-08-02 03:13:49.000000 yyszh-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh/
+-rw-rw-rw-   0        0        0     1888 2023-08-02 03:21:55.000000 yyszh-0.1.1/yyszh/__init__.py
+-rw-rw-rw-   0        0        0    23737 2023-08-02 02:39:32.000000 yyszh-0.1.1/yyszh/utils.py
+-rw-rw-rw-   0        0        0     1471 2023-08-02 03:21:55.000000 yyszh-0.1.1/yyszh/word_cloud_diagram.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 03:22:22.000000 yyszh-0.1.1/yyszh.egg-info/top_level.txt
```

### Comparing `yyszh-0.1.0/yyszh/__init__.py` & `yyszh-0.1.1/yyszh/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,8 +18,10 @@
     read_txt,       # 读取txt文件，按行作为元素
     write_txt,       # 将文本list写入到txt文件中，每个元素一行内容
     read_word,       # 读取docx文档，读取其中的文本和表格，结果组成一个list
     compute_vecsimilar_one_2_one,    # 计算两个向量的相似度，需要维度相同
     compute_vecsimilar__one_2_many,    # 计算一个向量和多个向量的相似度，返回相似度最大的下标和对应的相似度
     compute_vecsimilar__many_2_many    # 计算多个向量和多个向量的相似度，返回第一个参数中每个相似度最大的下标和对应的相似度
 
-)
+)
+
+from yyszh.word_cloud_diagram import word_cloud_diagram     # 生成词云图
```

### Comparing `yyszh-0.1.0/yyszh/utils.py` & `yyszh-0.1.1/yyszh/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     return results
 
 def get_email(text):
     """ 提取文本中的 E-mail，返回结果为list
         如：
             text = '我的email是ifee@baidu.com和dsdsd@dsdsd.com,李林的邮箱是eewewe@gmail.com'
-            emails = extract_email(text)
+            emails = get_email(text)
             print(emails)
             [{'text': 'ifee@baidu.com', 'offset': (8, 22), 'domain_name': 'baidu'},
              {'text': 'dsdsd@dsdsd.com', 'offset': (23, 38), 'domain_name': 'dsdsd'},
              {'text': 'eewewe@gmail.com', 'offset': (45, 61), 'domain_name': 'gmail'}]
         其中：
             text：提取的email
             offset：email在文本中的位置，含头不含尾
@@ -275,15 +275,15 @@
         elif isinstance(obj, datetime.datetime):
             return obj.strftime('%Y-%m-%d %H:%M:%S')
         elif isinstance(obj, datetime.date):
             return obj.strftime('%Y-%m-%d')
         else:
             return super(MyEncoder, self).default(obj)
 
-def write_json(filename, data, isIndent=False, isLine=False):
+def write_json(filename, data, isIndent=True, isLine=False):
     """
     将字典或者list数据保存为json
     :param filename: 保存的文件名
     :param data: 要保存的数据
     :param isIndent: 是否按照漂亮的格式保存
     :param isLine: 是否按行保存
     :return:
```

