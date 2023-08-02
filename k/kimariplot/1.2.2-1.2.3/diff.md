# Comparing `tmp/kimariplot-1.2.2.tar.gz` & `tmp/kimariplot-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimariplot-1.2.2.tar", last modified: Tue Aug  1 10:07:32 2023, max compression
+gzip compressed data, was "kimariplot-1.2.3.tar", last modified: Wed Aug  2 11:16:12 2023, max compression
```

## Comparing `kimariplot-1.2.2.tar` & `kimariplot-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 10:07:32.113568 kimariplot-1.2.2/
--rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.2/LICENSE
--rw-rw-rw-   0        0        0     4398 2023-08-01 10:07:32.111568 kimariplot-1.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 10:07:32.102565 kimariplot-1.2.2/kimariplot/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.2/kimariplot/__init__.py
--rw-rw-rw-   0        0        0     7261 2023-08-01 10:07:27.000000 kimariplot-1.2.2/kimariplot/plotter.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:07:32.110565 kimariplot-1.2.2/kimariplot.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-08-01 10:07:31.000000 kimariplot-1.2.2/kimariplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-08-01 10:07:32.000000 kimariplot-1.2.2/kimariplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 10:07:31.000000 kimariplot-1.2.2/kimariplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-08-01 10:07:31.000000 kimariplot-1.2.2/kimariplot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-08-01 10:07:31.000000 kimariplot-1.2.2/kimariplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 10:07:32.113568 kimariplot-1.2.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-08-01 10:07:27.000000 kimariplot-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:16:12.198849 kimariplot-1.2.3/
+-rw-rw-rw-   0        0        0     1086 2023-07-30 18:07:15.000000 kimariplot-1.2.3/LICENSE
+-rw-rw-rw-   0        0        0     4398 2023-08-02 11:16:12.198849 kimariplot-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-08-01 09:43:44.000000 kimariplot-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 11:16:12.186925 kimariplot-1.2.3/kimariplot/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:25:08.000000 kimariplot-1.2.3/kimariplot/__init__.py
+-rw-rw-rw-   0        0        0     8298 2023-08-02 11:15:27.000000 kimariplot-1.2.3/kimariplot/plotter.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:16:12.197185 kimariplot-1.2.3/kimariplot.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-08-02 11:16:11.000000 kimariplot-1.2.3/kimariplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-08-02 11:16:11.000000 kimariplot-1.2.3/kimariplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:16:11.000000 kimariplot-1.2.3/kimariplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-02 11:16:11.000000 kimariplot-1.2.3/kimariplot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-08-02 11:16:11.000000 kimariplot-1.2.3/kimariplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:16:12.198849 kimariplot-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-08-02 11:15:44.000000 kimariplot-1.2.3/setup.py
```

### Comparing `kimariplot-1.2.2/LICENSE` & `kimariplot-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.2/PKG-INFO` & `kimariplot-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.2
+Version: 1.2.3
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.2/README.md` & `kimariplot-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kimariplot-1.2.2/kimariplot/plotter.py` & `kimariplot-1.2.3/kimariplot/plotter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import datetime
 
 import matplotlib.pyplot as plt
 import toml
 
 
 def parse(file_path: str):
     """
@@ -168,17 +169,46 @@
     fig.show()
     # 保存路径为当前文件夹下的 figure 文件
     save_name = "figure." + output_type
     # 保存
     fig.savefig(save_name, dpi=dpi, bbox_inches='tight')
 
 
+def welcome(version):
+    """
+    欢迎页面
+    """
+    # 定义版本信息
+    version_info = {
+        'version': version,
+        'release_date': 'Aug-2-2023',
+        'developer': 'Kimariyb (XiaMen University, School of Electronic Science and Engineering)',
+        'website': 'https://github.com/kimariyb/kimariPlot',
+    }
+    # 获取当前日期和时间
+    now = datetime.datetime.now()
+    # 定义界面文本
+    interface_text = f"""
+KimariPlot --  A plotting software used for quickly creating energy profile found in scientific literature. 
+Version {version_info['version']}, release date: {version_info['release_date']}
+Developer: {version_info['developer']}
+KimariPlot Github website: {version_info['website']}
+
+( Current date: {now.date()}  Time: {now.strftime("%H:%M:%S")} )
+
+Thank you for using, the energy profile has now been successfully plotted!    
+"""
+
+    # 打印界面文本
+    print(interface_text)
+
+
 def main():
     # 版本参数
-    version = '1.2.2'
+    version = '1.2.3'
     # 创建 ArgumentParser 对象
     parser = argparse.ArgumentParser(description='Generate a energy profile using kimariplot', add_help=False)
     # 添加 -h 参数
     parser.add_argument('--help', '-h', action='help', help='Show this help message and exit')
     # 添加输入文件参数
     parser.add_argument('input_file', type=str, help='Please input a Toml file')
     # 添加输出文件格式参数
@@ -190,13 +220,15 @@
     parser.add_argument('--font', '-f', dest='font', type=str, help='The font family of the graph', default='Arial')
     # 添加图像大小参数
     parser.add_argument('--size', '-s', dest='size', type=str, help='The size of the graph', default='10,7.5')
     # 添加查询版本参数
     parser.add_argument('--version', '-v', action='version', version=f'kimariplot version {version}')
     # 解析命令行参数
     args = parser.parse_args()
+    # 调用欢迎页面函数
+    welcome(version)
     # 得到 Toml 文件中的数据列表
     plot_data_list = parse(args.input_file)
     # 将 size 参数转换为元组类型
     size = tuple(map(float, args.size.split(',')))
     # 绘制所有路径
     plot_all_line_paths(plot_data_list, args.dpi, size, args.font, args.output)
```

### Comparing `kimariplot-1.2.2/kimariplot.egg-info/PKG-INFO` & `kimariplot-1.2.3/kimariplot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimariplot
-Version: 1.2.2
+Version: 1.2.3
 Summary: A tool for generating Kimari-plots.
 Home-page: https://github.com/kimariyb/kimariPlot
 Author: Kimariyb
 Author-email: kimariyb@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kimariplot-1.2.2/setup.py` & `kimariplot-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kimariplot",
-    version="1.2.2",
+    version="1.2.3",
     author="Kimariyb",
     author_email="kimariyb@163.com",
     description="A tool for generating Kimari-plots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimariyb/kimariPlot",
     packages=setuptools.find_packages(),
```

