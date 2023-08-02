# Comparing `tmp/aespark-0.0.5.tar.gz` & `tmp/aespark-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespark-0.0.5.tar", last modified: Tue Aug  1 05:58:08 2023, max compression
+gzip compressed data, was "aespark-0.0.6.tar", last modified: Wed Aug  2 09:55:21 2023, max compression
```

## Comparing `aespark-0.0.5.tar` & `aespark-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.770706 aespark-0.0.5/
--rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-08-01 05:58:08.770706 aespark-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.660963 aespark-0.0.5/aespark/
--rw-rw-rw-   0        0        0    16810 2023-08-01 04:55:26.000000 aespark-0.0.5/aespark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.770706 aespark-0.0.5/aespark/static/
--rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.5/aespark/static/ip.txt
--rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.5/aespark/static/材料模板.docx
-drwxrwxrwx   0        0        0        0 2023-08-01 05:58:08.660963 aespark-0.0.5/aespark.egg-info/
--rw-rw-rw-   0        0        0      731 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 05:58:08.000000 aespark-0.0.5/aespark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 05:58:08.770706 aespark-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1554 2023-08-01 04:55:45.000000 aespark-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.883252 aespark-0.0.6/
+-rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1067 2023-08-02 09:55:21.883252 aespark-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-08-02 09:54:45.000000 aespark-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.755752 aespark-0.0.6/aespark/
+-rw-rw-rw-   0        0        0    19784 2023-08-02 09:52:09.000000 aespark-0.0.6/aespark/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.883252 aespark-0.0.6/aespark/static/
+-rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.6/aespark/static/ip.txt
+-rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.6/aespark/static/材料模板.docx
+drwxrwxrwx   0        0        0        0 2023-08-02 09:55:21.775774 aespark-0.0.6/aespark.egg-info/
+-rw-rw-rw-   0        0        0     1067 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       77 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 09:55:21.000000 aespark-0.0.6/aespark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       80 2023-08-02 01:31:36.000000 aespark-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:55:21.883252 aespark-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1595 2023-08-02 09:54:57.000000 aespark-0.0.6/setup.py
```

### Comparing `aespark-0.0.5/aespark/__init__.py` & `aespark-0.0.6/aespark/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 from pathlib import Path
 from docx import Document
 from docx.enum.text import WD_PARAGRAPH_ALIGNMENT
+from docx.enum.table import WD_TABLE_ALIGNMENT
 from docx.enum.table import WD_ALIGN_VERTICAL
 from docx.shared import Pt
 import datetime
 import jionlp
 import pandas as pd
+from docx.shared import Cm
 import os
 import time
 import numpy as np
 import jieba
 import warnings
 import re
 import pkg_resources
+import unicodedata
 from tqdm import tqdm
+
 warnings.filterwarnings('ignore')
 
 
 class MyDocument(object):
     '''
     功能简介：
         读取模板文档创建空白文档供操作
     参数解释：
         url :   可选 word模板路径
     '''
 
     def __init__(self, url: str = '', drop: bool = True):
         if url == '':
             dist = pkg_resources.get_distribution("aespark")
-            url = f'{dist.location}\aespark\static\材料模板.docx'
+            url = f'{dist.location}/aespark/static/材料模板.docx'
         self.doc = Document(url)
         if drop:
             self.all_clean()
 
     def add_text(self, string: str = '未指定插入内容', level: int = -1):
         '''
         功能简介：
@@ -51,35 +55,59 @@
         功能简介：
             在docx文档末尾插入新表格
         参数解释：
             df          :   需插入的表格
             sty         :   可选 表格风格
             fontsize    :   可选 表格内字体大小
         '''
+        def get_fontwidth(text):
+            count = 0
+            for c in text:
+                if unicodedata.east_asian_width(c) in 'FWA':
+                    count += 2
+                else:
+                    count += 0.85
+            return count
+
+        def set_tablewidth(table, widths):
+            """表格分别设置列宽，单位为Cm"""
+            for x, width in enumerate(widths):
+                for cell in table.columns[x].cells:
+                    cell.width = Cm(width)
+
         table = self.doc.add_table(df.shape[0]+1, df.shape[1])
         table.style = sty
         table.style.font.size = Pt(fontsize)
-        # table.autofit = False
-        # table.allow_autofit = False
+        table.alignment = WD_TABLE_ALIGNMENT.CENTER
         for j in range(df.shape[-1]):
             table.cell(0, j).text = df.columns[j]
         for i in range(df.shape[0]):
             for j in range(df.shape[-1]):
                 table.cell(i+1, j).text = str(df.values[i, j])
         for col in table.columns:
             for cell in col.cells:
                 cell.paragraphs[0].alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
                 cell.vertical_alignment = WD_ALIGN_VERTICAL.CENTER
+        
+        widlist = []
+        for i in df.columns:
+            wid = get_fontwidth(str(i))
+            for index in df.index:
+                lins = get_fontwidth(str(df[i][index]))
+                wid = lins if lins > wid else wid
+            widlist.append(wid)
+        widlist = [i/sum(widlist)*15.26 for i in widlist]
+        set_tablewidth(table, widlist)  # 共15.26
 
-    def save(self, url: str = f"./{format(datetime.datetime.now(), '%Y%m%d%H%M%S')}.docx"):
+    def save(self, url: str = f"./未设置保存名称.docx"):
         '''
         功能简介：
             保存docx文档
         参数解释：
-            url :   str.    保存路径（含文件名及后缀），默认当前程序位置，文件名默认为当前时间
+            url :   str.    保存路径（含文件名及后缀），默认当前程序位置
         '''
         self.doc.save(url)
 
     def move_paragraphs(self):
         '''
         功能简介：
             移除所有段落
@@ -200,19 +228,23 @@
 
     geshi['总文件名'] = geshi['总文件名'].str.replace(
         '[^\u4e00-\u9fa5]', '', regex=True)
 
     for i in tqdm(geshi.index, desc='数据产出'):
 
         if geshi['总文件名'][i] != '':
-            file_name = pd.DataFrame(list(jieba.cut(geshi['总文件名'][i])))
-            file_name = pd.DataFrame(file_name.groupby(
-                0).size().sort_values(ascending=False))
-            file_name = ''.join(
-                file_name[file_name[0] == file_name.iloc[0].values[0]].index.to_list())
+            result = jieba.tokenize(geshi['总文件名'][i])
+            cutresult = pd.DataFrame(columns=['word', 'start'])
+            for tk in result:
+                cutresult.loc[len(cutresult)] = [tk[0],tk[1]]
+            cutresult = cutresult.pivot_table(index='word', values='start', aggfunc=['count', 'sum']).reset_index()
+            cutresult.columns = ['word', 'count', 'start']
+            cutresult.sort_values(by=['count', 'start'], ascending=[False, True], inplace=True)
+            cutresult = cutresult[cutresult['count']==cutresult['count'].max()]
+            file_name = ''.join(list(cutresult['word']))
         else:
             file_name = '未知'
 
         exec(f"hebin{i}.drop_duplicates(inplace=True)")
         exec(f"hebin{i}.reset_index(drop=True, inplace=True)")
         exec(f"hebin{i} = DataClean_invisibleCharDel(hebin{i}, df=True)")
         exec(f"hebin{i} = DataClean_excelAddT(hebin{i})")
@@ -228,15 +260,15 @@
             exec(f"hebin{i} = hebin{i}.loc[{limit+1}:]")
             exec(f"hebin{i}.reset_index(drop=True, inplace=True)")
 
         exec(
             f"hebin{i}.to_csv(r'合并数据产出\{i+1}.{file_name}({num},总{all}){n}.csv', index=False, encoding='gb18030')")
 
 
-def moreSheetDataMerging(url: str, lex: str = '*', link: bool = False, seq: str = '_', ind: int = None):
+def moreSheetDataMerging(url: str, lex: str = '*', link: bool = False, seq: str = '_', ind: int = None, save:bool = True):
     '''
     功能简介：
         按sheet名称合并多个excel文件
     功能输出：
         一个含有多个dataframe的数组
     参数解释：
         url     文件夹路径   
@@ -270,17 +302,22 @@
                     alldata[sheet] = pd.DataFrame()
                     alldata[sheet] = pd.concat([alldata[sheet], df[sheet]])
 
     for sheet in list(alldata.keys()):
         alldata[sheet].drop_duplicates(inplace=True)
         alldata[sheet].reset_index(inplace=True, drop=True)
 
-    print(
-        f"合并完成：共得到{len(alldata.keys())}个表格：{'、'.join([i for i in alldata.keys()])}")
-
+    if save == False:
+        print(f"合并完成：共得到{len(alldata.keys())}个表格：{'、'.join([i for i in alldata.keys()])}")
+    else:
+        buildFolder('多sheet合并数据产出')
+        with pd.ExcelWriter(f"多sheet合并数据产出/多sheet合并结果.xlsx") as score_file:
+            for sheet in list(alldata.keys()):
+                alldata[sheet].to_excel(score_file,sheet_name = sheet, index = False)
+    
     return alldata
 
 
 def Parse_idNumber(idCardNumber: str):
     '''
     功能简介：
         身份证号码解析
@@ -433,28 +470,26 @@
     return times if times else np.nan
 
 
 class IP():
 
     def __init__(self):
         dist = pkg_resources.get_distribution("aespark")
-        self.df = pd.read_table(
-            rf'{dist.location}\aespark\static\ip.txt', keep_default_na='')
+        self.df = pd.read_table(f'{dist.location}/aespark/static/ip.txt', keep_default_na='')
 
     def Parse_ipv4(self, ipstr: str):
         '''
         功能简介：
             ip地址解析
         return：
             一个字典，包含省、市、区、运营商、地址、原始信息
         '''
-        def IP(x): return sum([256 ** i * int(j)
-                               for i, j in enumerate(x.split('.')[::-1])])
+        IIP = lambda x:sum([256 ** i * int(j)for i, j in enumerate(x.split('.')[::-1])])
         try:
-            ind = list(self.df[self.df['起点长整型'] <= IP(ipstr)].index)[-1]
+            ind = list(self.df[self.df['起点长整型'] <= IIP(ipstr)].index)[-1]
             dic = {
                 'statu': 'success',
                 'province': self.df['省'][ind],
                 'city': self.df['市'][ind],
                 'county': self.df['区'][ind],
                 'operators': self.df['运营商'][ind],
                 'fulladdress': self.df['地址'][ind],
@@ -468,7 +503,35 @@
                 'county': '',
                 'operators': '',
                 'fulladdress': '',
                 'fullinformation': '',
             }
 
         return dic
+
+def PivotTable_transView(df:pd.DataFrame, collist:list):
+    '''
+    功能简介：
+        基于交易数据产出账户交易概况表
+    参数解释：
+        df  交易数据表
+        collist 字段列表，顺序需要一致，[主端账户，交易金额，借贷标志，交易时间]
+    调用示例：
+        ddf = PivotTable_transView(df01,['用户ID', '金额(元)', '收/支', '创建时间'])
+    '''
+    df[collist[1]] = df[collist[1]].astype('float')
+    df[collist[2]] = df[collist[2]].apply(DataClean_inOutCleaning)
+    df[collist[3]] = df[collist[3]].apply(DataClean_TimeConversion)
+    piv = df.pivot_table(index=collist[0], columns=collist[2], values=collist[1], aggfunc=['sum', 'count']).reset_index()
+    piv.columns = [''.join([i[1],i[0]]).replace('sum', '金额').replace('count', '次数') for i in piv.columns]
+    if len(piv.columns) == 7:
+        piv = piv.take([0, 1, 4, 2, 5, 3, 6], axis=1)
+    else:
+        piv = piv.take([0, 1, 3, 2, 4], axis=1)
+    piv2 = df.pivot_table(index=collist[0], values=collist[3], aggfunc=['min', 'max']).reset_index()
+    piv2.columns = [collist[0], '首次交易', '末次交易']
+    piv2['首次交易'] = piv2['首次交易'].apply(lambda x:str(x)[:str(x).index(' ')])
+    piv2['末次交易'] = piv2['末次交易'].apply(lambda x:str(x)[:str(x).index(' ')])
+
+    piv = pd.merge(left=piv, right=piv2, how='left', on=collist[0])
+
+    return piv
```

### Comparing `aespark-0.0.5/aespark/static/ip.txt` & `aespark-0.0.6/aespark/static/ip.txt`

 * *Files identical despite different names*

### Comparing `aespark-0.0.5/aespark/static/材料模板.docx` & `aespark-0.0.6/aespark/static/材料模板.docx`

 * *Files identical despite different names*

### Comparing `aespark-0.0.5/setup.py` & `aespark-0.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name='aespark', version='0.0.5',
+setuptools.setup(name='aespark', version='0.0.6',
                  description='Generate a QR code that can adapt to the cylinder',
                  long_description=open(
                      'README.md', 'r', encoding='utf-8').read(),
                  author='wtianxin',
                  author_email='1007582510@qq.com',
                  url='https://pypi.org/project/aespark/',
                  license='MIT',  # 与之前你选用的许可证类型有关系
@@ -12,14 +12,15 @@
                  zip_safe=False,
                  include_package_data=True,
                  install_requires=[
                      'jieba>=0.42.1',
                      'tqdm>=4.64.1',
                      'jionlp>=1.5.2',
                      'python-docx>=0.8.11',
+                     'openpyxl>=3.1.2',
                  ],
                  keywords='aespark',
                  classifiers=[
                      "Natural Language :: Chinese (Simplified)",
                      "Development Status :: 3 - Alpha",
                      "Operating System :: OS Independent",
                      "Programming Language :: Python",
```

