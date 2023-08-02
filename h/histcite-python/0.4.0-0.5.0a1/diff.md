# Comparing `tmp/histcite-python-0.4.0.tar.gz` & `tmp/histcite-python-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.4.0.tar", last modified: Fri Jul 28 06:44:43 2023, max compression
+gzip compressed data, was "histcite-python-0.5.0a1.tar", last modified: Wed Aug  2 15:19:27 2023, max compression
```

## Comparing `histcite-python-0.4.0.tar` & `histcite-python-0.5.0a1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.159818 histcite-python-0.4.0/
--rw-r--r--   0 wang       (501) staff       (20)     1064 2023-07-26 16:29:59.000000 histcite-python-0.4.0/LICENSE
--rw-r--r--   0 wang       (501) staff       (20)     7868 2023-07-28 06:44:43.159665 histcite-python-0.4.0/PKG-INFO
--rw-r--r--   0 wang       (501) staff       (20)     7031 2023-07-26 16:29:59.000000 histcite-python-0.4.0/README.md
-drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.157793 histcite-python-0.4.0/histcite/
--rw-r--r--   0 wang       (501) staff       (20)       21 2023-07-26 16:29:59.000000 histcite-python-0.4.0/histcite/__init__.py
--rw-r--r--   0 wang       (501) staff       (20)     1828 2023-07-26 16:29:59.000000 histcite-python-0.4.0/histcite/cli.py
--rw-r--r--   0 wang       (501) staff       (20)     6040 2023-07-28 01:49:03.000000 histcite-python-0.4.0/histcite/compute_metrics.py
--rw-r--r--   0 wang       (501) staff       (20)     5099 2023-07-28 01:50:03.000000 histcite-python-0.4.0/histcite/network_graph.py
--rw-r--r--   0 wang       (501) staff       (20)    12536 2023-07-28 00:54:50.000000 histcite-python-0.4.0/histcite/parse_reference.py
--rw-r--r--   0 wang       (501) staff       (20)    10605 2023-07-28 01:51:59.000000 histcite-python-0.4.0/histcite/process_file.py
--rw-r--r--   0 wang       (501) staff       (20)     4294 2023-07-28 00:58:03.000000 histcite-python-0.4.0/histcite/recognize_reference.py
-drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.158718 histcite-python-0.4.0/histcite_python.egg-info/
--rw-r--r--   0 wang       (501) staff       (20)     7868 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 wang       (501) staff       (20)      550 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 wang       (501) staff       (20)        1 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 wang       (501) staff       (20)       47 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 wang       (501) staff       (20)       29 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/requires.txt
--rw-r--r--   0 wang       (501) staff       (20)        9 2023-07-28 06:44:43.000000 histcite-python-0.4.0/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 wang       (501) staff       (20)     1089 2023-07-26 16:29:59.000000 histcite-python-0.4.0/pyproject.toml
--rw-r--r--   0 wang       (501) staff       (20)       38 2023-07-28 06:44:43.159874 histcite-python-0.4.0/setup.cfg
-drwxr-xr-x   0 wang       (501) staff       (20)        0 2023-07-28 06:44:43.159324 histcite-python-0.4.0/tests/
--rw-r--r--   0 wang       (501) staff       (20)        0 2023-07-28 03:40:33.000000 histcite-python-0.4.0/tests/test_cli.py
--rw-r--r--   0 wang       (501) staff       (20)     1638 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_compute_metrics.py
--rw-r--r--   0 wang       (501) staff       (20)      988 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_network_graph.py
--rw-r--r--   0 wang       (501) staff       (20)     1969 2023-07-26 16:29:59.000000 histcite-python-0.4.0/tests/test_parse_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8169 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-02 15:19:27.000000 histcite-python-0.5.0a1/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:19:27.990732 histcite-python-0.5.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 15:19:17.000000 histcite-python-0.5.0a1/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.4.0/LICENSE` & `histcite-python-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.4.0/PKG-INFO` & `histcite-python-0.5.0a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.4.0
+Version: 0.5.0a1
 Summary: A Python interface for histcite
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Home-page, https://github.com/doublessay/histcite-python
 Keywords: histcite,citation network,web of science,scopus,cssci
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
+[![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
+[![Downloads](https://pepy.tech/badge/histcite-python/month)](https://pepy.tech/project/histcite-python)
+[![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
+
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
+- `GCS`，Global Citation Score，表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
@@ -50,75 +54,78 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
-# 需要 Python3.8 或以上版本
+# 需要 Python3.9 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
-⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
-⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+> [!WARNING]  
+> 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+> 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[查看FQA1](#fqa) |
 
 ```console
 $ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
 $ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
 $ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
 
-注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+> [!NOTE]  
+> 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含  
+① 描述统计表 descriptive_statistics.xlsx  
+② 引文网络图节点信息表 graph_node_info.xlsx  
+③ 引文网络图的数据文件 graph.dot  
+文件③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
-<img src="examples/graph.svg">
+![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下：
+对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
 |    | AU                                       | TI                                                   |   PY | SO             |   LCS |
 |------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
 |          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
 |          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
 |          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
 |          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
 |          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
 |         ... |                                      |                                                |      |              |       |
 
-2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2、使用Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
 
 3、其他API接口（待更新）
 
-## 实现细节
-|  | Web of Science | CSSCI | Scopus|
-| --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
-| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
-
-## Q&A
-1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+## FQA
+1. 为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+A: 考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2. 每次必须指定一种数据库来源吗？  
+A: 是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
 
-2、每次必须指定一种数据库来源吗？  
-答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+3. 为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+A: 无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
-3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
-答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
+4. 如何识别引文关系？  
+A: Web of Science 优先使用 `DOI` 进行匹配，否则使用 `一作`、`发表年份`、`文献来源`、`开始页` 进行匹配；CSSCI 和 Scopus 使用 `一作` 和 `题名` 进行匹配。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.4.0/README.md` & `histcite-python-0.5.0a1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # HistCite工具的Python实现
 
+[![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
+[![Downloads](https://pepy.tech/badge/histcite-python/month)](https://pepy.tech/project/histcite-python)
+[![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
+
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
+- `GCS`，Global Citation Score，表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
@@ -29,75 +34,78 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
-# 需要 Python3.8 或以上版本
+# 需要 Python3.9 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
-⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
-⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+> [!WARNING]  
+> 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+> 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[查看FQA1](#fqa) |
 
 ```console
 $ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
 $ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
 $ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
 
-注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+> [!NOTE]  
+> 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含  
+① 描述统计表 descriptive_statistics.xlsx  
+② 引文网络图节点信息表 graph_node_info.xlsx  
+③ 引文网络图的数据文件 graph.dot  
+文件③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
-<img src="examples/graph.svg">
+![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下：
+对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
 |    | AU                                       | TI                                                   |   PY | SO             |   LCS |
 |------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
 |          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
 |          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
 |          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
 |          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
 |          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
 |         ... |                                      |                                                |      |              |       |
 
-2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2、使用Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
 
 3、其他API接口（待更新）
 
-## 实现细节
-|  | Web of Science | CSSCI | Scopus|
-| --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
-| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
-
-## Q&A
-1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+## FQA
+1. 为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+A: 考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2. 每次必须指定一种数据库来源吗？  
+A: 是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
 
-2、每次必须指定一种数据库来源吗？  
-答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+3. 为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+A: 无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
-3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
-答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
+4. 如何识别引文关系？  
+A: Web of Science 优先使用 `DOI` 进行匹配，否则使用 `一作`、`发表年份`、`文献来源`、`开始页` 进行匹配；CSSCI 和 Scopus 使用 `一作` 和 `题名` 进行匹配。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.4.0/histcite/cli.py` & `histcite-python-0.5.0a1/histcite/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import argparse
-from histcite.compute_metrics import ComputeMetrics
+from histcite.read_file import ReadFile
 from histcite.process_file import ProcessFile
+from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import GraphViz
 
 
 def main():
     parser = argparse.ArgumentParser(description='A Python interface for histcite.')
     parser.add_argument('-f','--folder_path', type=str, required=True, help='Folder path of literature metadata.')
     parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci','scopus'], help='Source type of literature metadata.')
@@ -13,27 +14,26 @@
     # parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
     # 将结果存放在用户指定的folder_path下的result文件夹中
     output_path = os.path.join(args.folder_path, 'result')
     if not os.path.exists(output_path):
         os.mkdir(output_path)
-    process = ProcessFile(args.folder_path, args.source_type)
-    process.concat_df()
-    process.process_reference()
-    process.process_citation()
-    reference_df = process.reference_df
-    docs_df = process.docs_df
 
-    cm = ComputeMetrics(docs_df, reference_df, args.source_type)
+    docs_df = ReadFile(args.folder_path, args.source_type).read_all()
+    process = ProcessFile(docs_df, args.source_type)
+    process.extract_reference()
+    citing_relation_df, refs_df = process.process_citation()
+
+    cm = ComputeMetrics(docs_df, citing_relation_df, refs_df, args.source_type)
     cm_output_path = os.path.join(output_path, 'descriptive_statistics.xlsx')
     cm.write2excel(cm_output_path)
     
-    doc_indices = docs_df.sort_values('LCS', ascending=False).index[:args.node_num]
-    graph = GraphViz(docs_df, args.source_type)
+    doc_indices = citing_relation_df[citing_relation_df['LCS']>0].sort_values('LCS', ascending=False).index[:args.node_num]
+    graph = GraphViz(docs_df, citing_relation_df, args.source_type)
 
     # 生成图文件
     graph_dot_file = graph.generate_dot_file(doc_indices)
     graph_dot_path = os.path.join(output_path, 'graph.dot')
     with open(graph_dot_path, 'w') as f:
         f.write(graph_dot_file)
```

### Comparing `histcite-python-0.4.0/histcite/compute_metrics.py` & `histcite-python-0.5.0a1/histcite/compute_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import os
 import pandas as pd
+from typing import Literal, Optional
 
 
 class ComputeMetrics:
     def __init__(self, docs_df: pd.DataFrame, 
-                 reference_df: pd.DataFrame, 
-                 source_type: str):
-        self.docs_df = docs_df
-        self.reference_df = reference_df
+                 citing_relation_df: pd.DataFrame,
+                 refs_df: pd.DataFrame, 
+                 source_type: Literal['wos', 'cssci', 'scopus']):
+        self.merged_docs_df = docs_df.merge(citing_relation_df[['doc_index', 'LCR', 'LCS']], on='doc_index')
+        self.refs_df = refs_df
         self.source_type = source_type
 
-    def __generate_df(self, use_cols: list, 
+    def __generate_df(self, use_cols: list[str], 
                       col: str, 
-                      split_char = None, 
-                      str_lower = False, 
-                      sort_field = None) -> pd.DataFrame:
-        df = self.docs_df[use_cols]
+                      split_char: Optional[str] = None, 
+                      str_lower: bool = False, 
+                      sort_field: Optional[str] = None) -> pd.DataFrame:
+        df = self.merged_docs_df[use_cols]
         # 如果字段包含多个值，则进行拆分
         if split_char:
             df = df.dropna(subset=[col])
             df = df.astype({col: 'str'})
             if str_lower:
                 df[col] = df[col].str.lower()
             df[col] = df[col].str.split(split_char)
@@ -76,19 +78,19 @@
     def _generate_records_df(self):
         if self.source_type in ['wos', 'scopus']:
             use_cols = ['AU', 'TI', 'SO', 'PY', 'TI', 'LCS', 'TC', 'LCR', 'NR', 'source file']
         elif self.source_type == 'cssci':
             use_cols = ['AU', 'TI', 'SO', 'PY', 'LCS', 'LCR', 'NR', 'source file']
         else:
             raise ValueError('Invalid source type')
-        records_df = self.docs_df[use_cols]
+        records_df = self.merged_docs_df[use_cols]
         if 'TC' in use_cols:
-            records_df.rename(columns={'TC': 'GCS'}, inplace=True)
+            records_df = records_df.rename(columns={'TC': 'GCS'})
         if 'NR' in use_cols:
-            records_df.rename(columns={'NR':'GCR'}, inplace=True)
+            records_df = records_df.rename(columns={'NR':'GCR'})
         return records_df
 
     def _generate_journal_df(self):
         if self.source_type in ['wos', 'scopus']:
             use_cols = ['SO', 'LCS', 'TC']
         elif self.source_type == 'cssci':
             use_cols = ['SO', 'LCS']
@@ -110,17 +112,17 @@
             keys = ['First_AU', 'PY', 'J9', 'VL', 'BP', 'DI', 'local']
         elif self.source_type == 'cssci':
             keys = ['First_AU', 'TI', 'SO', 'PY', 'VL', 'local']
         elif self.source_type == 'scopus':
             keys = ['First_AU', 'TI', 'SO', 'VL', 'BP', 'EP', 'PY', 'local']
         else:
             raise ValueError('Invalid source type')
-        reference_df = self.reference_df.groupby(keys).size().reset_index(name='Recs')
-        reference_df.insert(len(reference_df.columns)-1, 'local', reference_df.pop('local'))
-        return reference_df.sort_values(by='Recs', ascending=False)
+        refs_df = self.refs_df.groupby(by=keys, dropna=False).size().reset_index(name='Recs')
+        refs_df.insert(len(refs_df.columns)-1, 'local', refs_df.pop('local'))
+        return refs_df.sort_values(by='Recs', ascending=False)
 
     def write2excel(self, save_path: str):
         """将统计结果写入excel"""
         save_folder_path = os.path.dirname(save_path)
         if not os.path.exists(save_folder_path):
             os.makedirs(save_folder_path)
         with pd.ExcelWriter(save_path) as writer:
```

### Comparing `histcite-python-0.4.0/histcite/network_graph.py` & `histcite-python-0.5.0a1/histcite/network_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import Literal
 import pandas as pd
 
 class GraphViz:
-    def __init__(self, docs_df: pd.DataFrame, source_type: str):
-        self.docs_df = docs_df
+    def __init__(self, docs_df: pd.DataFrame, 
+                 citing_relation_df:pd.DataFrame, 
+                 source_type: Literal['wos', 'cssci', 'scopus']):
+        # merge by index
+        self.merged_docs_df = docs_df.merge(citing_relation_df, left_index=True, right_index=True, suffixes=(None, '_y')).drop(columns=['doc_index_y'])
         self.source_type = source_type
         self.empty_year_index = docs_df[docs_df['PY'].isna()].index
 
     def __obtain_groups(self):
         """obtain groups of docs by year"""
-        year_series = self.docs_df.loc[self.node_list, 'PY']
+        year_series = self.merged_docs_df.loc[self.node_list, 'PY']
         groups = year_series.groupby(year_series)
         year_list = [i[0] for i in groups]
         grouped_doc_index = [i[1].index.tolist() for i in groups]
         self.year_list = year_list
         for idx, year in enumerate(year_list):
             grouped_doc_index[idx].insert(0, year)
         self.grouped_doc_index = grouped_doc_index
@@ -24,19 +27,19 @@
         related_doc_list = [int(i) for i in doc_relation.split(';') if int(i) not in self.empty_year_index]
         if relation_type == 'reference':
             return {(doc_index, ref) for ref in related_doc_list}
         else:
             return {(citation, doc_index) for citation in related_doc_list}
 
     def __generate_edge_list(self):
-        min_df = self.docs_df.loc[self.doc_indices, ['reference', 'citation']]
+        min_df = self.merged_docs_df.loc[self.doc_indices, ['cited_doc_index', 'citing_doc_index']]
         edge_set: set[tuple[int, int]] = set()
         for idx in self.doc_indices:
-            doc_reference = min_df.loc[idx, 'reference']
-            doc_citation = min_df.loc[idx, 'citation']
+            doc_reference = min_df.loc[idx, 'cited_doc_index']
+            doc_citation = min_df.loc[idx, 'citing_doc_index']
             if pd.notna(doc_citation) and isinstance(doc_citation, str):
                 cell_edge_set = self.__generate_edge(idx, doc_citation, 'citation')
                 if cell_edge_set:
                     edge_set.update(cell_edge_set)
             if pd.notna(doc_reference) and isinstance(doc_reference, str):
                 cell_edge_set  = self.__generate_edge(idx, doc_reference, 'reference')
                 if cell_edge_set:
@@ -58,14 +61,15 @@
         return edge_list
 
     def generate_dot_file(self, doc_indices:pd.Index, allow_external_node=False):
         """
         doc_indices: 文献索引列表\n
         allow_external_node: 是否允许出现doc_indices之外的节点，默认False
         """
+        # drop doc_index without year information
         self.doc_indices = [i for i in doc_indices if i not in self.empty_year_index]
         self.allow_external_node = allow_external_node
 
         raw_edge_list = self.__generate_edge_list()
         self.__obtain_groups()
 
         dot_edge_list = [f'\t{source} -> '+'{ '+' '.join([str(i) for i in raw_edge_list[source]])+' };\n' for source in raw_edge_list]
@@ -98,14 +102,14 @@
             use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS', 'TC']
         elif self.source_type == 'cssci':
             use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS']
         elif self.source_type == 'scopus':
             use_cols = ['doc_index', 'AU', 'TI', 'PY', 'SO', 'LCS', 'TC']
         else:
             raise ValueError('invalid source type')
-        graph_node_df = self.docs_df.loc[self.node_list, use_cols]
+        graph_node_df = self.merged_docs_df.loc[self.node_list, use_cols]
         if 'TC' in graph_node_df.columns:
             graph_node_df.rename(columns={'TC': 'GCS'}, inplace=True)
         return graph_node_df
 
     def _export_graph_node_file(self, file_path: str):
         self.generate_graph_node_file().to_excel(file_path, index=False)
```

### Comparing `histcite-python-0.4.0/histcite/parse_reference.py` & `histcite-python-0.5.0a1/histcite/parse_reference.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 import re
-from dataclasses import dataclass
-from typing import Optional, Literal, Union, Any
+from dataclasses import dataclass, asdict
+from typing import Optional, Literal, Union
 
 @dataclass
 class WosField:
     First_AU: Optional[str]
-    PY: Optional[int] = None
+    PY: Optional[str] = None
     J9: Optional[str] = None
     VL: Optional[str] = None
     BP: Optional[str] = None
     DI: Optional[str] = None
+    doc_index: Optional[int] = None
 
 
 @dataclass
 class CssciField:
     First_AU: Optional[str]
     TI: str
     SO: Optional[str] = None
     PY: Optional[str] = None
     VL: Optional[str] = None
+    doc_index: Optional[int] = None
 
 
 @dataclass
 class ScopusField:
     First_AU: Optional[str]
     TI: str
     SO: Optional[str] = None
     VL: Optional[str] = None
     IS: Optional[str] = None
     BP: Optional[str] = None
     EP: Optional[str] = None
     PY: Optional[str] = None
+    doc_index: Optional[int] = None
 
 
 class ParseReference:
     def __init__(self, doc_index, cr_cell: str, source_type: Literal['wos', 'cssci', 'scopus']):
         sep = '; '
         try:
             self.cr_list = cr_cell.split(sep)
             self.cr_count = len(self.cr_list)
         except AttributeError:
             self.cr_count = 0
         else:
             self.doc_index = doc_index
             self.source_type = source_type
 
-    @staticmethod
-    def _parse_wos_cr(cr: str) -> Optional[WosField]:
+    def _parse_wos_cr(self, cr: str) -> Optional[WosField]:
         if 'Patent No.' in cr:
             return None
         
-        AU, raw_PY, J9, VL, BP, DI = None, None, None, None, None, None
+        AU, PY, J9, VL, BP, DI = None, None, None, None, None, None
         if ', DOI ' in cr:
             # contain only one DOI
             if 'DOI [' not in cr:
                 DI_match = re.search(r'DOI (10.*)$', cr)
                 DI = DI_match[1] if DI_match else None
             # contain two or more DOI
             else:
@@ -62,18 +64,18 @@
                 DI = DI_match[1] if DI_match else None
             cr = re.sub(r', DOI.*', '', cr)
         
         # always contain another language
         if '[' in cr:
             return None
         
-        BP_match = re.search(r', P([A-Za-z]?\d+)$', cr)
+        BP_match = re.search(r', [Pp]([A-Za-z]?\d+)$', cr)
         if BP_match:
             BP = BP_match[1]
-            cr = cr.replace(f', P{BP}', '')
+            cr = re.sub(r', [Pp][A-Za-z]?\d+', '', cr)
 
         cr = re.sub(r'[,\.] PROCEEDINGS(?=, )','',cr,flags=re.I)
         if VL_match := re.search(r', V([\d-]+)$', cr):
             VL = VL_match[1]
             sub_pattern = r', V[\d-]+$'
         
         elif re.search(r', VOLS? ', cr, re.I):
@@ -89,43 +91,39 @@
             sub_pattern = None
         
         if sub_pattern:
             cr = re.sub(sub_pattern, '', cr)
 
         dot_count = cr.count(', ') 
         if dot_count == 2:
-            AU, raw_PY, J9 = cr.split(', ')
+            AU, PY, J9 = cr.split(', ')
         elif dot_count > 2:
             PY_pattern = r', (\d{4}), '
             if re.search(PY_pattern, cr):
-                AU, raw_PY, J9 = re.split(PY_pattern, cr, 1)
+                AU, PY, J9 = re.split(PY_pattern, cr, 1)
         else:
             return None
         
         if DI:
             DI = DI.lower()
             if len(re.findall(', ', DI)) == 1:
                 try:
                     DI1, DI2 = DI.replace('doi ', '').split(', ')
                 except:
-                    print(DI)
                     return None
                 if DI1 == DI2:
                     DI = DI1
                 else:
                     DI = None
         
-        if raw_PY and re.match(r'^\d{4}$', raw_PY):
-            PY = int(raw_PY)
-        else:
+        if PY and not re.match(r'^\d{4}$', PY):
             PY = None
-        return WosField(AU, PY, J9, VL, BP, DI)
+        return WosField(AU, PY, J9, VL, BP, DI, self.doc_index)
 
-    @staticmethod
-    def _parse_cssci_cr(cr: str) -> Optional[CssciField]:
+    def _parse_cssci_cr(self, cr: str) -> Optional[CssciField]:
         """only parse chinese reference"""
         dot_pattern = re.compile(r'(?<!\d)\.(?!\d)|(?<=\d)\.(?!\d)|(?<!\d)\.(?=\d)|(?<=\d{4})\.(?=\d)|(?<=\d)\.(?=\d{4})')
         
         # 中文参考文献
         if re.search(r'[\u4e00-\u9fa5]', cr):
             dot_count = len(dot_pattern.findall(cr))
 
@@ -139,96 +137,97 @@
                     _, AU, TI, other = cr.split('.')
                 except:
                     return None
                 else:
                     TI = TI.replace(':学位论文', '')
                     SO, PY = other.split(',')
                     PY = PY.split(':')[0]
-                    return CssciField(AU, TI, SO, PY, None)
-
+                    result =  CssciField(AU, TI, SO, PY, None)
+                    
             # 国家标准
             elif 'GB/T' in cr:
                 if cr[-3:] == "出版社":
                     _, AU, other = cr.split('.', 2)
                     TI, SO = other.rsplit('.', 1)
-                    return CssciField(AU, TI, SO, None, None)
+                    result =  CssciField(AU, TI, SO, None, None)
                 else:
                     _, AU, TI = cr.split('.', 2)
-                    return CssciField(AU, TI, None, None, None)
+                    result =  CssciField(AU, TI, None, None, None)
 
             # 规范
             elif re.search(r':DB\d{2}/T', cr):
                 _, AU, other = cr.split('.', 2)
                 TI, PY = other.rsplit('.', 1)
-                return CssciField(AU, TI, None, PY, None)
+                result =  CssciField(AU, TI, None, PY, None)
 
             # 报刊
             elif re.search(r'\.\d{1,2}\.\d{1,2}(?:\(|$)', cr):
                 try:
                     _, AU, TI, SO, other = re.split(dot_pattern, cr, 4)
                 except:
                     return None
                 else:
-                    return CssciField(AU, TI, SO, None, None)
+                    result = CssciField(AU, TI, SO, None, None)
 
             # 专利1
             elif re.search(r'\.CN\d{9}[A-Z]$', cr):
                 TI = cr.split('.', 1)[1]
-                return CssciField(None, TI, None, None, None)
+                result =  CssciField(None, TI, None, None, None)
             # 专利2
             elif re.search(r'^\d+\.一种', cr):
                 date_pattern = re.compile(r'\d{4}\-\d{1,2}\-\d{1,2}')
                 TI = cr.split('.', 1)[1]
                 date = date_pattern.search(cr)
                 if date:
                     PY = date[0].split('-')[0]
                 else:
                     PY = None
                 TI = date_pattern.sub('', TI).strip('.()')
-                return CssciField(None, TI, None, PY, None)
+                result = CssciField(None, TI, None, PY, None)
 
             # 网络文献
             elif re.search(r'\.\d{4}$', cr):
                 if dot_count == 3:
                     _, AU, TI, PY = re.split(dot_pattern, cr)
                 elif dot_count == 4:
                     _, AU, TI, SO, PY = re.split(dot_pattern, cr)
                 else:
                     return None
-                return CssciField(AU, TI, None, PY, None)
+                result = CssciField(AU, TI, None, PY, None)
 
             # 期刊1
             elif dot_count == 5:
                 _, AU, TI, SO, PY, VL = re.split(dot_pattern, cr)
-                return CssciField(AU, TI, SO, PY, VL)
+                result = CssciField(AU, TI, SO, PY, VL)
             # 期刊2
             elif dot_count == 4:
                 _, AU, TI, SO, _ = re.split(dot_pattern, cr)
-                return CssciField(AU, TI, SO, None, None)
+                result = CssciField(AU, TI, SO, None, None)
 
             # 专著
             elif dot_count == 3:
                 _, AU, TI, SO = re.split(dot_pattern, cr)
-                return CssciField(AU, TI, SO, None, None)
+                result = CssciField(AU, TI, SO, None, None)
 
             # 其他
             elif dot_count == 2:
                 _, AU, TI = re.split(dot_pattern, cr)
-                return CssciField(AU, TI, None, None, None)
+                result = CssciField(AU, TI, None, None, None)
 
             elif dot_count == 1:
                 _, TI = re.split(dot_pattern, cr)
-                return CssciField(None, TI, None, None, None)
+                result = CssciField(None, TI, None, None, None)
             else:
                 return None
+            result.doc_index = self.doc_index
+            return result
         else:
             return None
 
-    @staticmethod
-    def _parse_scopus_cr(cr: str) -> Optional[ScopusField]:
+    def _parse_scopus_cr(self, cr: str) -> Optional[ScopusField]:
         if cr.count(', ') < 3:
             return None
 
         # 年份
         PY_match = re.search(r' \((\d{4})\)$', cr)
         if PY_match:
             PY = PY_match[1]
@@ -339,33 +338,24 @@
 
             # 首字母大写，其他小写
             elif re.search(r'^[A-Z][^A-Z]+$',cr):
                 TI, SO = cr, None
             
             else:
                 return None
-        return ScopusField(First_AU,TI,SO,VL,IS,BP,EP,PY)
+        return ScopusField(First_AU, TI, SO, VL, IS, BP, EP, PY, self.doc_index)
 
-    def parse_cr_cell(self) -> Optional[dict[str, list[Any]]]:
+    def parse_cr_cell(self) -> Optional[list[dict[str, str]]]:
         if self.cr_count == 0:
             return None
         
         parsed_cr_list : list[Union[WosField, CssciField, ScopusField, None]]
         if self.source_type == "wos":
             parsed_cr_list = [self._parse_wos_cr(i) for i in self.cr_list]
-            keys = ['First_AU', 'PY', 'J9', 'VL', 'BP', 'DI']
         elif self.source_type == "cssci":
             parsed_cr_list = [self._parse_cssci_cr(i) for i in self.cr_list]
-            keys = ['First_AU', 'TI', 'SO', 'PY', 'VL']
         elif self.source_type == "scopus":
             parsed_cr_list = [self._parse_scopus_cr(i) for i in self.cr_list]
-            keys = ['First_AU', 'TI', 'SO', 'VL', 'BP', 'EP', 'PY']
         else:
             raise ValueError('Invalid source type')
-
-        result:dict[str, list[Any]]  = {key: [] for key in keys}
-        for parsed_cr in parsed_cr_list:
-            if parsed_cr:
-                for key in keys:
-                    result[key].append(getattr(parsed_cr, key))
-        result['doc_index'] = self.doc_index
-        return result
+        parse_cr_list = [asdict(cr) for cr in parsed_cr_list if cr is not None]
+        return parse_cr_list
```

### Comparing `histcite-python-0.4.0/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.5.0a1/histcite_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.4.0
+Version: 0.5.0a1
 Summary: A Python interface for histcite
 Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
 Project-URL: Home-page, https://github.com/doublessay/histcite-python
 Keywords: histcite,citation network,web of science,scopus,cssci
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
+[![PyPI](https://img.shields.io/pypi/v/histcite-python)](https://pypi.org/project/histcite-python)
+[![Supported Versions](https://img.shields.io/pypi/pyversions/histcite-python.svg)](https://pypi.org/project/histcite-python)
+[![Downloads](https://pepy.tech/badge/histcite-python/month)](https://pepy.tech/project/histcite-python)
+[![License](https://img.shields.io/pypi/l/histcite-python.svg)](https://github.com/doublessay/histcite-python/blob/main/LICENSE)
+
 由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/index.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.4.0` 实现对参考文献信息元的完整解析；
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
 - 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；
 - 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`，Global Citation Score， 表示一篇文献在文献数据库中的总被引次数；
+- `GCS`，Global Citation Score，表示一篇文献在文献数据库中的总被引次数；
 - `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
 - `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`，Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
 - `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
@@ -50,75 +54,78 @@
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
 | 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
-# 需要 Python3.8 或以上版本
+# 需要 Python3.9 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
 
-⚠️ 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
-⚠️ 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
+> [!WARNING]  
+> 在 Web of Science 和 Scopus 平台检索时须将检索结果语言限定为英文；  
+> 文件下载之后不要重命名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
-| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[参看QA1](#qa) |
+| -n | --node_num | `LCS` 最高的N个文献节点，默认为 `50`，[查看FQA1](#fqa) |
 
 ```console
 $ 假设文件夹路径为/Users/.../Downloads/dataset，来源为web of science, 节点数量设置为100
 $ histcite -f /Users/.../Downloads/dataset -t wos -n 100
 $ 或者是
 $ histcite --folder_path /Users/.../Downloads/dataset --source_type wos --node_num 100
 ```
 
-注：生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含 ①描述统计表descriptive_statistics.xlsx, ②引文网络图节点信息表graph_node_info.xlsx, ③引文网络图的数据文件graph.dot 三个文件，③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
+> [!NOTE]  
+> 生成的结果保存在 `folder_path` 下的 `result` 文件夹内，包含  
+① 描述统计表 descriptive_statistics.xlsx  
+② 引文网络图节点信息表 graph_node_info.xlsx  
+③ 引文网络图的数据文件 graph.dot  
+文件③可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或下载到本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。
 
 引文网络图示例：
 
-<img src="examples/graph.svg">
+![](https://raw.githubusercontent.com/doublessay/histcite-python/main/examples/graph.svg)
 
-对应的节点信息如下：
+对应的节点信息如下(以CSSCI数据源为例，不同文献数据库的节点信息字段存在差异)：
 |    | AU                                       | TI                                                   |   PY | SO             |   LCS |
 |------------:|:-----------------------------------------|:-----------------------------------------------------|-----:|:---------------|------:|
 |          55 | 张坤; 查先进                             | 我国智慧图书馆的发展沿革及构建策略研究               | 2021 | 国家图书馆学刊 |     6 |
 |          60 | 石婷婷; 徐建华; 张雨浓                   | 数字孪生技术驱动下的智慧图书馆应用场景与体系架构设计 | 2021 | 情报理论与实践 |     7 |
 |          63 | 卢小宾; 宋姬芳; 蒋玲; 洪先锋; 刘静; 张薷 | 智慧图书馆建设标准探析                               | 2021 | 中国图书馆学报 |     9 |
 |          81 | 程焕文; 钟远薪                           | 智慧图书馆的三维解析                                 | 2021 | 图书馆论坛     |    10 |
 |          86 | 段美珍; 初景利; 张冬荣; 解贺嘉           | 智慧图书馆的内涵特点及其认知模型研究                 | 2021 | 图书情报工作   |     7 |
 |         ... |                                      |                                                |      |              |       |
 
-2、函数调用，相比命令行工具会更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
+2、使用Jupyter，比命令行更加灵活，可以自定义更多参数，查看 [demo.ipynb](demo.ipynb)
 
 3、其他API接口（待更新）
 
-## 实现细节
-|  | Web of Science | CSSCI | Scopus|
-| --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
-| 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
-
-## Q&A
-1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+## FQA
+1. 为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
+A: 考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2. 每次必须指定一种数据库来源吗？  
+A: 是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
 
-2、每次必须指定一种数据库来源吗？  
-答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+3. 为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+A: 无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
-3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
-答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
+4. 如何识别引文关系？  
+A: Web of Science 优先使用 `DOI` 进行匹配，否则使用 `一作`、`发表年份`、`文献来源`、`开始页` 进行匹配；CSSCI 和 Scopus 使用 `一作` 和 `题名` 进行匹配。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.4.0/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.5.0a1/histcite_python.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 pyproject.toml
 histcite/__init__.py
 histcite/cli.py
 histcite/compute_metrics.py
 histcite/network_graph.py
 histcite/parse_reference.py
 histcite/process_file.py
+histcite/read_file.py
 histcite/recognize_reference.py
 histcite_python.egg-info/PKG-INFO
 histcite_python.egg-info/SOURCES.txt
 histcite_python.egg-info/dependency_links.txt
 histcite_python.egg-info/entry_points.txt
 histcite_python.egg-info/requires.txt
 histcite_python.egg-info/top_level.txt
-tests/test_cli.py
 tests/test_compute_metrics.py
 tests/test_network_graph.py
 tests/test_parse_reference.py
```

### Comparing `histcite-python-0.4.0/pyproject.toml` & `histcite-python-0.5.0a1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 
 [project]
 name = "histcite-python"
 authors = [
     {name = "WangK2", email = "kw221225@gmail.com"}
     ]
 description = "A Python interface for histcite"
-version = "0.4.0"
+version = "0.5.0a1"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["histcite","citation network","web of science","scopus","cssci"]
 license = {text = "MIT"}
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Information Analysis",
     ]
 dependencies = [
```

