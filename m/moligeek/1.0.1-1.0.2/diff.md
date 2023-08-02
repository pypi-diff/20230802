# Comparing `tmp/moligeek-1.0.1.tar.gz` & `tmp/moligeek-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moligeek-1.0.1.tar", last modified: Wed Aug  2 12:08:34 2023, max compression
+gzip compressed data, was "moligeek-1.0.2.tar", last modified: Wed Aug  2 14:35:39 2023, max compression
```

## Comparing `moligeek-1.0.1.tar` & `moligeek-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.253470 moligeek-1.0.1/
--rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-08-02 09:01:41.000000 moligeek-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6332 2023-08-02 12:08:34.253470 moligeek-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5492 2023-08-02 05:54:20.000000 moligeek-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.198316 moligeek-1.0.1/moligeek/
--rw-rw-rw-   0        0        0     1605 2023-08-02 12:08:03.000000 moligeek-1.0.1/moligeek/__init__.py
--rw-rw-rw-   0        0        0      340 2023-08-02 12:08:03.000000 moligeek-1.0.1/moligeek/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.238183 moligeek-1.0.1/moligeek/core/
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.239178 moligeek-1.0.1/moligeek/core/LAN/
--rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/LAN/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/LAN/scan.py
--rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.241172 moligeek-1.0.1/moligeek/core/encode/
--rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/encode/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/encode/decode.py
--rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/encode/fence.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.243166 moligeek-1.0.1/moligeek/core/network/
--rw-rw-rw-   0        0        0     2053 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/hostinfo.py
--rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.1/moligeek/core/network/wifi.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.245206 moligeek-1.0.1/moligeek/core/web/
--rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/web/__init__.py
--rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/core/web/imitate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.246156 moligeek-1.0.1/moligeek/core/zip/
--rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.1/moligeek/core/zip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.246156 moligeek-1.0.1/moligeek/database/
--rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/database/YiYan.dat
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.252044 moligeek-1.0.1/moligeek/path_dict/
--rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/ASP.txt
--rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/ASPX.txt
--rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/DIR.txt
--rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/JSP.txt
--rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/MDB.txt
--rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/PHP.txt
--rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.1/moligeek/path_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 12:08:34.237186 moligeek-1.0.1/moligeek.egg-info/
--rw-rw-rw-   0        0        0     6332 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-08-02 12:08:34.000000 moligeek-1.0.1/moligeek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.1/moligeek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 12:08:33.000000 moligeek-1.0.1/moligeek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 12:08:34.253470 moligeek-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1661 2023-08-02 08:59:51.000000 moligeek-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.267747 moligeek-1.0.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6292 2023-08-02 14:35:39.266750 moligeek-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5452 2023-08-02 14:35:19.000000 moligeek-1.0.2/README.md
+-rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.2/main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.223896 moligeek-1.0.2/moligeek/
+-rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.2/moligeek/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-08-02 14:35:19.000000 moligeek-1.0.2/moligeek/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.238848 moligeek-1.0.2/moligeek/core/
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.239841 moligeek-1.0.2/moligeek/core/LAN/
+-rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/LAN/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/LAN/scan.py
+-rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.241834 moligeek-1.0.2/moligeek/core/encode/
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/encode/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/encode/decode.py
+-rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/encode/fence.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.243827 moligeek-1.0.2/moligeek/core/network/
+-rw-rw-rw-   0        0        0     2053 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/hostinfo.py
+-rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/wifi.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.245820 moligeek-1.0.2/moligeek/core/web/
+-rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/web/__init__.py
+-rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/web/imitate.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.245820 moligeek-1.0.2/moligeek/core/zip/
+-rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/zip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.260774 moligeek-1.0.2/moligeek/database/
+-rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/database/YiYan.dat
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.265758 moligeek-1.0.2/moligeek/path_dict/
+-rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/ASP.txt
+-rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/ASPX.txt
+-rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/DIR.txt
+-rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/JSP.txt
+-rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/MDB.txt
+-rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/PHP.txt
+-rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.237849 moligeek-1.0.2/moligeek.egg-info/
+-rw-rw-rw-   0        0        0     6292 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.2/moligeek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:35:39.267747 moligeek-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.2/setup.py
```

### Comparing `moligeek-1.0.1/LICENSE` & `moligeek-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/PKG-INFO` & `moligeek-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -86,20 +86,21 @@
 ```
 3.若安装过程出现意外，请使用以下指令换源后重新尝试以上指令
 ```
 sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/apt/sources.list
 apt update && apt upgrade
 ```
 ### Windows
-0. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek（推荐），或者选择以下做法进行安装
-1. 可前往Python官网下载: [官网](https://www.python.org/)
-2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装Python
+**以下为三种不同的安装方式**
+1. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek
+2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装moligeek
 ```
-winget install Python.Python.3.10
+winget install moligeek
 ```
+3. 使用python运行本仓库的源代码
 ---
 
 ### Linux
 
 
 
 **Debian & Ubuntu**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.2 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -32,30 +32,30 @@
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
 install git git clone https://github.com/yourmoln/moligeek.git ```
 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
-apt/sources.list apt update && apt upgrade ``` ### Windows 0. å¨æ¬ä»åºç
-[releases](https://github.com/yourmoln/moligeek/
-releases)ä¸è½½windowsçæ¬çmoligeekï¼æ¨èï¼ï¼æèéæ©ä»¥ä¸åæ³è¿è¡å®è£
-1. å¯åå¾Pythonå®ç½ä¸è½½: [å®ç½](https://www.python.org/) 2.
+apt/sources.list apt update && apt upgrade ``` ### Windows
+**ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
+github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
-1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£Python
-``` winget install Python.Python.3.10 ``` --- ### Linux **Debian & Ubuntu**
-```sh apt install python ``` **CentOS** ```sh yum install python ``` ##
-ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh git clone https://
-github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬ **å¦ä½è¿è¡** ```sh
-python ./moligeek/main.py ``` **è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ###
-ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
-zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
-python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
-moligeek/blob/main/requirements.txt)æ¥ç - ps:
-èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
+1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
+``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
+- ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
+yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
+git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
+**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
+æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
+æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
+è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
+requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
+å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.1/README.md` & `moligeek-1.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -65,20 +65,21 @@
 ```
 3.若安装过程出现意外，请使用以下指令换源后重新尝试以上指令
 ```
 sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/apt/sources.list
 apt update && apt upgrade
 ```
 ### Windows
-0. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek（推荐），或者选择以下做法进行安装
-1. 可前往Python官网下载: [官网](https://www.python.org/)
-2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装Python
+**以下为三种不同的安装方式**
+1. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek
+2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装moligeek
 ```
-winget install Python.Python.3.10
+winget install moligeek
 ```
+3. 使用python运行本仓库的源代码
 ---
 
 ### Linux
 
 
 
 **Debian & Ubuntu**
```

#### html2text {}

```diff
@@ -21,30 +21,30 @@
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
 install git git clone https://github.com/yourmoln/moligeek.git ```
 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
-apt/sources.list apt update && apt upgrade ``` ### Windows 0. å¨æ¬ä»åºç
-[releases](https://github.com/yourmoln/moligeek/
-releases)ä¸è½½windowsçæ¬çmoligeekï¼æ¨èï¼ï¼æèéæ©ä»¥ä¸åæ³è¿è¡å®è£
-1. å¯åå¾Pythonå®ç½ä¸è½½: [å®ç½](https://www.python.org/) 2.
+apt/sources.list apt update && apt upgrade ``` ### Windows
+**ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
+github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
-1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£Python
-``` winget install Python.Python.3.10 ``` --- ### Linux **Debian & Ubuntu**
-```sh apt install python ``` **CentOS** ```sh yum install python ``` ##
-ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh git clone https://
-github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬ **å¦ä½è¿è¡** ```sh
-python ./moligeek/main.py ``` **è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ###
-ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
-zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
-python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
-moligeek/blob/main/requirements.txt)æ¥ç - ps:
-èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
+1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
+``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
+- ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
+yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
+git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
+**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
+æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
+æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
+è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
+requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
+å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.1/moligeek/core/LAN/scan.py` & `moligeek-1.0.2/moligeek/core/LAN/scan.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/__init__.py` & `moligeek-1.0.2/moligeek/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/encode/decode.py` & `moligeek-1.0.2/moligeek/core/encode/decode.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/encode/fence.py` & `moligeek-1.0.2/moligeek/core/encode/fence.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/network/__init__.py` & `moligeek-1.0.2/moligeek/core/network/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/network/hostinfo.py` & `moligeek-1.0.2/moligeek/core/network/hostinfo.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/network/wifi.py` & `moligeek-1.0.2/moligeek/core/network/wifi.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/web/__init__.py` & `moligeek-1.0.2/moligeek/core/web/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/web/imitate.py` & `moligeek-1.0.2/moligeek/core/web/imitate.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/core/zip/__init__.py` & `moligeek-1.0.2/moligeek/core/zip/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/database/YiYan.dat` & `moligeek-1.0.2/moligeek/database/YiYan.dat`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/ASP.txt` & `moligeek-1.0.2/moligeek/path_dict/ASP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/ASPX.txt` & `moligeek-1.0.2/moligeek/path_dict/ASPX.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/DIR.txt` & `moligeek-1.0.2/moligeek/path_dict/DIR.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/JSP.txt` & `moligeek-1.0.2/moligeek/path_dict/JSP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/MDB.txt` & `moligeek-1.0.2/moligeek/path_dict/MDB.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek/path_dict/PHP.txt` & `moligeek-1.0.2/moligeek/path_dict/PHP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.1/moligeek.egg-info/PKG-INFO` & `moligeek-1.0.2/moligeek.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -86,20 +86,21 @@
 ```
 3.若安装过程出现意外，请使用以下指令换源后重新尝试以上指令
 ```
 sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/apt/sources.list
 apt update && apt upgrade
 ```
 ### Windows
-0. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek（推荐），或者选择以下做法进行安装
-1. 可前往Python官网下载: [官网](https://www.python.org/)
-2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装Python
+**以下为三种不同的安装方式**
+1. 在本仓库的[releases](https://github.com/yourmoln/moligeek/releases)下载windows版本的moligeek
+2. 如果Windows版本高于16299(Windows 10 1709)并且软件包安装程序为最新版本，可尝试使用Winget命令安装moligeek
 ```
-winget install Python.Python.3.10
+winget install moligeek
 ```
+3. 使用python运行本仓库的源代码
 ---
 
 ### Linux
 
 
 
 **Debian & Ubuntu**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.1 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.2 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -32,30 +32,30 @@
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
 install git git clone https://github.com/yourmoln/moligeek.git ```
 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
-apt/sources.list apt update && apt upgrade ``` ### Windows 0. å¨æ¬ä»åºç
-[releases](https://github.com/yourmoln/moligeek/
-releases)ä¸è½½windowsçæ¬çmoligeekï¼æ¨èï¼ï¼æèéæ©ä»¥ä¸åæ³è¿è¡å®è£
-1. å¯åå¾Pythonå®ç½ä¸è½½: [å®ç½](https://www.python.org/) 2.
+apt/sources.list apt update && apt upgrade ``` ### Windows
+**ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
+github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
-1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£Python
-``` winget install Python.Python.3.10 ``` --- ### Linux **Debian & Ubuntu**
-```sh apt install python ``` **CentOS** ```sh yum install python ``` ##
-ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh git clone https://
-github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬ **å¦ä½è¿è¡** ```sh
-python ./moligeek/main.py ``` **è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ###
-ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
-zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
-python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
-moligeek/blob/main/requirements.txt)æ¥ç - ps:
-èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
+1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
+``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
+- ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
+yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
+git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
+**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
+æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
+æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
+è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
+requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
+å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.1/moligeek.egg-info/SOURCES.txt` & `moligeek-1.0.2/moligeek.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
+main.py
 requirements.txt
 setup.py
 moligeek/__init__.py
 moligeek/__version__.py
 moligeek.egg-info/PKG-INFO
 moligeek.egg-info/SOURCES.txt
 moligeek.egg-info/dependency_links.txt
+moligeek.egg-info/entry_points.txt
 moligeek.egg-info/not-zip-safe
 moligeek.egg-info/requires.txt
 moligeek.egg-info/top_level.txt
 moligeek/core/__init__.py
 moligeek/core/LAN/__init__.py
 moligeek/core/LAN/scan.py
 moligeek/core/encode/__init__.py
```

### Comparing `moligeek-1.0.1/setup.py` & `moligeek-1.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,9 +51,13 @@
 
     install_requires=requires,
 
     tests_require=[
         'pytest>=3.3.1',
         'pytest-cov>=2.5.1',
     ],
-
+    entry_points={
+        'console_scripts': [
+            'moligeek = moligeek:run',
+        ],
+    }
 )
```

