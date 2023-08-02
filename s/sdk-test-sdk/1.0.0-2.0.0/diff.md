# Comparing `tmp/sdk_test_sdk-1.0.0.tar.gz` & `tmp/sdk_test_sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk_test_sdk-1.0.0.tar", last modified: Wed Aug  2 07:17:05 2023, max compression
+gzip compressed data, was "sdk_test_sdk-2.0.0.tar", last modified: Wed Aug  2 08:08:21 2023, max compression
```

## Comparing `sdk_test_sdk-1.0.0.tar` & `sdk_test_sdk-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.190354 sdk_test_sdk-1.0.0/
--rw-r--r--   0 zhuwankang   (501) staff       (20)     1310 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/LICENSE.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)      763 2023-08-02 07:17:05.190210 sdk_test_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 zhuwankang   (501) staff       (20)      273 2023-08-02 07:07:05.000000 sdk_test_sdk-1.0.0/README.md
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.189429 sdk_test_sdk-1.0.0/sdk_test_sdk/
--rw-r--r--   0 zhuwankang   (501) staff       (20)       76 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/sdk_test_sdk/__init__.py
--rw-r--r--   0 zhuwankang   (501) staff       (20)      172 2023-08-02 07:06:04.000000 sdk_test_sdk-1.0.0/sdk_test_sdk/core.py
-drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 07:17:05.190047 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/
--rw-r--r--   0 zhuwankang   (501) staff       (20)      763 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zhuwankang   (501) staff       (20)      255 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)        1 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       14 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/requires.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       13 2023-08-02 07:17:05.000000 sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/top_level.txt
--rw-r--r--   0 zhuwankang   (501) staff       (20)       38 2023-08-02 07:17:05.190396 sdk_test_sdk-1.0.0/setup.cfg
--rw-r--r--   0 zhuwankang   (501) staff       (20)     3784 2023-08-02 07:16:57.000000 sdk_test_sdk-1.0.0/setup.py
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774808 sdk_test_sdk-2.0.0/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)     1310 2023-08-02 07:06:04.000000 sdk_test_sdk-2.0.0/LICENSE.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      772 2023-08-02 08:08:21.774686 sdk_test_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      282 2023-08-02 07:17:35.000000 sdk_test_sdk-2.0.0/README.md
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774003 sdk_test_sdk-2.0.0/sdk_test_sdk/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       89 2023-08-02 08:08:13.000000 sdk_test_sdk-2.0.0/sdk_test_sdk/__init__.py
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      219 2023-08-02 08:08:13.000000 sdk_test_sdk-2.0.0/sdk_test_sdk/core.py
+drwxr-xr-x   0 zhuwankang   (501) staff       (20)        0 2023-08-02 08:08:21.774522 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      772 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zhuwankang   (501) staff       (20)      255 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)        1 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       14 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/requires.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       13 2023-08-02 08:08:21.000000 sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/top_level.txt
+-rw-r--r--   0 zhuwankang   (501) staff       (20)       38 2023-08-02 08:08:21.774864 sdk_test_sdk-2.0.0/setup.cfg
+-rw-r--r--   0 zhuwankang   (501) staff       (20)     3813 2023-08-02 07:57:38.000000 sdk_test_sdk-2.0.0/setup.py
```

### Comparing `sdk_test_sdk-1.0.0/LICENSE.txt` & `sdk_test_sdk-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sdk_test_sdk-1.0.0/PKG-INFO` & `sdk_test_sdk-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk_test_sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: An awesome SDK to say hello!
 Home-page: https://github.com/your/repo
 Author: Your Name
 Author-email: your@email.com
 License: MIT
 Keywords: python sample project example
 Platform: UNKNOWN
@@ -14,39 +14,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 添加关于SDK的说明和用法等信息，文件主要是用来对此次发行的包的详细说明，包括用法和注意事项等
 
 
+# 安装
+pip install sdk_test_sdk-1.0.0-py3-none-any.whl
+
+
 # 使用
 import sdk_test_sdk
 
 
 sdk_test_sdk.test_numpy()
 sdk_test_sdk.test_hello()
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# 安装
-pip install my_sdk
-
-
-
-
```

### Comparing `sdk_test_sdk-1.0.0/sdk_test_sdk.egg-info/PKG-INFO` & `sdk_test_sdk-2.0.0/sdk_test_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk-test-sdk
-Version: 1.0.0
+Version: 2.0.0
 Summary: An awesome SDK to say hello!
 Home-page: https://github.com/your/repo
 Author: Your Name
 Author-email: your@email.com
 License: MIT
 Keywords: python sample project example
 Platform: UNKNOWN
@@ -14,39 +14,19 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # 添加关于SDK的说明和用法等信息，文件主要是用来对此次发行的包的详细说明，包括用法和注意事项等
 
 
+# 安装
+pip install sdk_test_sdk-1.0.0-py3-none-any.whl
+
+
 # 使用
 import sdk_test_sdk
 
 
 sdk_test_sdk.test_numpy()
 sdk_test_sdk.test_hello()
 
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-# 安装
-pip install my_sdk
-
-
-
-
```

### Comparing `sdk_test_sdk-1.0.0/setup.py` & `sdk_test_sdk-2.0.0/setup.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-# 指定SDK的打包信息，为打包做准备的设置文件, 约定此次分发的包的版本号、名称、作者、联系方式、项目地址、python版本要求等信息from setuptools import setup, find_packagessetup(    name='sdk_test_sdk',  # 项目的名称，用于在PyPI上标识你的项目    version='1.0.0',  # 包版本号，便于维护版本    author='Your Name',  # 作者    author_email='your@email.com',  # 作者联系方式    description='An awesome SDK to say hello!',  # 包的简述    long_description=open('README.md').read(),  # 包的详细介绍，一般在README.md文件内    long_description_content_type='text/markdown',  # 指定long_description的内容类型，'text/markdown'：Markdown格式。适用于使用Markdown语法编写的文本    url='https://github.com/your/repo',  # 自己项目地址，比如github的项目地址    license='MIT',  # 项目的许可证信息，MIT许可证是一种宽松的许可证，允许任何人获得你的代码并在其项目中使用，包括商业项目。MIT许可证允许别人在不受约束的情况下再分发和修改你的代码，只需包含原始许可证和版权声明    packages=find_packages(),  # 包含的Python包的列表，使用find_packages()函数可以方便地找到所有的包    install_requires=[  # sdk的依赖包, 项目的依赖关系列表。指定其他Python包的名称和版本，确保用户在安装你的项目时会自动安装这些依赖        "numpy==1.24.4",    ],    python_requires='>=3.6',  # 对python的最低版本要求    classifiers=[  # 项目的分类器列表，用于在PyPI上对项目进行分类        "Programming Language :: Python :: 3",        "License :: OSI Approved :: MIT License",        "Operating System :: OS Independent",    ],    keywords='python sample project example',  # 项目的关键词列表，用于在PyPI上对项目进行搜索)# 在 sdk_test_sdk 目录下打开终端，并运行以下命令来创建SDK的打包文件# python setup.py sdist bdist_wheel#     sdist：这个命令用于创建一个源代码发布包。它将项目的源代码和必要文件打包成一个.tar.gz文件，供用户通过pip进行安装#         你可以使用pip来安装SDK。在终端中运行以下命令#             pip install dist/sdk_test_sdk-1.0.0.tar.gz#     bdist_wheel：这个命令用于创建一个Wheel发布包。Wheel是一个Python分发格式，它可以使安装Python项目更快，并且在一些情况下可以减少磁盘空间的使用。Wheel格式通常比源代码发布包更受欢迎#         你可以使用pip来安装SDK。在终端中运行以下命令#             pip install dist/sdk_test_sdk-1.0.0-py3-none-any.whl#     1111#         my_sdk1-1.1.0-py3-none-any.whl#         my_sdk-1.0.0-py3-none-any.whl#             可以 pip install 1111/* 安装所有的#     .whl格式的发布包通常比.tar.gz格式的发布包安装得更快。这是因为.whl是一种已编译的二进制格式，不需要再在用户的计算机上进行编译，而.tar.gz则需要在用户的计算机上进行编译安装#     在某些情况下，.whl格式的发布包可以帮助缓解依赖问题。例如，如果你的项目依赖于一些C扩展模块，这些模块在不同的操作系统上可能会有不同的二进制格式，导致在安装时出现问题。使用.whl格式的发布包可以提供特定于操作系统和Python版本的预编译版本，从而避免了依赖问题#     磁盘空间：.whl格式的发布包通常比.tar.gz格式的发布包占用更少的磁盘空间。因为它只包含了预编译的二进制文件和必要的元数据，而.tar.gz格式的发布包包含了完整的源代码和资源文件
+# 指定SDK的打包信息，为打包做准备的设置文件, 约定此次分发的包的版本号、名称、作者、联系方式、项目地址、python版本要求等信息from setuptools import setup, find_packagessetup(    name='sdk_test_sdk',  # 项目的名称，用于在PyPI上标识你的项目    version='2.0.0',  # 包版本号，便于维护版本    author='Your Name',  # 作者    author_email='your@email.com',  # 作者联系方式    description='An awesome SDK to say hello!',  # 包的简述    long_description=open('README.md').read(),  # 包的详细介绍，一般在README.md文件内    long_description_content_type='text/markdown',  # 指定long_description的内容类型，'text/markdown'：Markdown格式。适用于使用Markdown语法编写的文本    url='https://github.com/your/repo',  # 自己项目地址，比如github的项目地址    license='MIT',  # 项目的许可证信息，MIT许可证是一种宽松的许可证，允许任何人获得你的代码并在其项目中使用，包括商业项目。MIT许可证允许别人在不受约束的情况下再分发和修改你的代码，只需包含原始许可证和版权声明    packages=find_packages(),  # 包含的Python包的列表，使用find_packages()函数可以方便地找到所有的包    install_requires=[  # sdk的依赖包, 项目的依赖关系列表。指定其他Python包的名称和版本，确保用户在安装你的项目时会自动安装这些依赖        "numpy==1.24.4",    ],    python_requires='>=3.6',  # 对python的最低版本要求    classifiers=[  # 项目的分类器列表，用于在PyPI上对项目进行分类        "Programming Language :: Python :: 3",        "License :: OSI Approved :: MIT License",        "Operating System :: OS Independent",    ],    keywords='python sample project example',  # 项目的关键词列表，用于在PyPI上对项目进行搜索)# 在 sdk_test_sdk 目录下打开终端，并运行以下命令来创建SDK的打包文件# python setup.py sdist bdist_wheel#     sdist：这个命令用于创建一个源代码发布包。它将项目的源代码和必要文件打包成一个.tar.gz文件，供用户通过pip进行安装#         你可以使用pip来安装SDK。在终端中运行以下命令#             pip install dist/sdk_test_sdk-1.0.0.tar.gz#     bdist_wheel：这个命令用于创建一个Wheel发布包。Wheel是一个Python分发格式，它可以使安装Python项目更快，并且在一些情况下可以减少磁盘空间的使用。Wheel格式通常比源代码发布包更受欢迎#         你可以使用pip来安装SDK。在终端中运行以下命令#             pip install dist/sdk_test_sdk-1.0.0-py3-none-any.whl#     .whl格式的发布包通常比.tar.gz格式的发布包安装得更快。这是因为.whl是一种已编译的二进制格式，不需要再在用户的计算机上进行编译，而.tar.gz则需要在用户的计算机上进行编译安装#     在某些情况下，.whl格式的发布包可以帮助缓解依赖问题。例如，如果你的项目依赖于一些C扩展模块，这些模块在不同的操作系统上可能会有不同的二进制格式，导致在安装时出现问题。使用.whl格式的发布包可以提供特定于操作系统和Python版本的预编译版本，从而避免了依赖问题#     磁盘空间：.whl格式的发布包通常比.tar.gz格式的发布包占用更少的磁盘空间。因为它只包含了预编译的二进制文件和必要的元数据，而.tar.gz格式的发布包包含了完整的源代码和资源文件# 上传至pypi#     pip install twine  # 安装 twine#     twine upload dist/*  # 上传sdk#         出现Enter your username和Enter your password提示，输入即可
```

