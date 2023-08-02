# Comparing `tmp/moligeek-1.0.2.tar.gz` & `tmp/moligeek-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moligeek-1.0.2.tar", last modified: Wed Aug  2 14:35:39 2023, max compression
+gzip compressed data, was "moligeek-1.0.3.tar", last modified: Wed Aug  2 15:22:45 2023, max compression
```

## Comparing `moligeek-1.0.2.tar` & `moligeek-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.267747 moligeek-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6292 2023-08-02 14:35:39.266750 moligeek-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5452 2023-08-02 14:35:19.000000 moligeek-1.0.2/README.md
--rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.2/main.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.223896 moligeek-1.0.2/moligeek/
--rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.2/moligeek/__init__.py
--rw-rw-rw-   0        0        0      340 2023-08-02 14:35:19.000000 moligeek-1.0.2/moligeek/__version__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.238848 moligeek-1.0.2/moligeek/core/
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.239841 moligeek-1.0.2/moligeek/core/LAN/
--rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/LAN/__init__.py
--rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/LAN/scan.py
--rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.241834 moligeek-1.0.2/moligeek/core/encode/
--rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/encode/__init__.py
--rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/encode/decode.py
--rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/encode/fence.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.243827 moligeek-1.0.2/moligeek/core/network/
--rw-rw-rw-   0        0        0     2053 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/hostinfo.py
--rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.2/moligeek/core/network/wifi.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.245820 moligeek-1.0.2/moligeek/core/web/
--rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/web/__init__.py
--rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/core/web/imitate.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.245820 moligeek-1.0.2/moligeek/core/zip/
--rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.2/moligeek/core/zip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.260774 moligeek-1.0.2/moligeek/database/
--rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/database/YiYan.dat
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.265758 moligeek-1.0.2/moligeek/path_dict/
--rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/ASP.txt
--rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/ASPX.txt
--rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/DIR.txt
--rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/JSP.txt
--rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/MDB.txt
--rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/PHP.txt
--rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.2/moligeek/path_dict/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:35:39.237849 moligeek-1.0.2/moligeek.egg-info/
--rw-rw-rw-   0        0        0     6292 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.2/moligeek.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       57 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 14:35:39.000000 moligeek-1.0.2/moligeek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 14:35:39.267747 moligeek-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.286342 moligeek-1.0.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-23 14:02:51.000000 moligeek-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      137 2023-08-02 14:35:19.000000 moligeek-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6553 2023-08-02 15:22:45.286342 moligeek-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5713 2023-08-02 15:20:31.000000 moligeek-1.0.3/README.md
+-rw-rw-rw-   0        0        0       64 2023-08-02 14:35:19.000000 moligeek-1.0.3/main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.256180 moligeek-1.0.3/moligeek/
+-rw-rw-rw-   0        0        0     7457 2023-08-02 14:35:19.000000 moligeek-1.0.3/moligeek/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-08-02 15:22:21.000000 moligeek-1.0.3/moligeek/__version__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.272171 moligeek-1.0.3/moligeek/core/
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.273172 moligeek-1.0.3/moligeek/core/LAN/
+-rw-rw-rw-   0        0        0       43 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/core/LAN/__init__.py
+-rw-rw-rw-   0        0        0     1206 2023-08-02 08:24:54.000000 moligeek-1.0.3/moligeek/core/LAN/scan.py
+-rw-rw-rw-   0        0        0      709 2023-08-02 08:24:54.000000 moligeek-1.0.3/moligeek/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.275189 moligeek-1.0.3/moligeek/core/encode/
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/core/encode/__init__.py
+-rw-rw-rw-   0        0        0     1097 2023-08-02 05:54:20.000000 moligeek-1.0.3/moligeek/core/encode/decode.py
+-rw-rw-rw-   0        0        0     1183 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/core/encode/fence.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.277217 moligeek-1.0.3/moligeek/core/network/
+-rw-rw-rw-   0        0        0     2047 2023-08-02 15:22:21.000000 moligeek-1.0.3/moligeek/core/network/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-08-02 08:24:54.000000 moligeek-1.0.3/moligeek/core/network/hostinfo.py
+-rw-rw-rw-   0        0        0     1418 2023-08-02 08:24:54.000000 moligeek-1.0.3/moligeek/core/network/wifi.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.278193 moligeek-1.0.3/moligeek/core/web/
+-rw-rw-rw-   0        0        0     3075 2023-08-02 05:54:20.000000 moligeek-1.0.3/moligeek/core/web/__init__.py
+-rw-rw-rw-   0        0        0     6177 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/core/web/imitate.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.279410 moligeek-1.0.3/moligeek/core/zip/
+-rw-rw-rw-   0        0        0     5356 2023-08-02 05:54:20.000000 moligeek-1.0.3/moligeek/core/zip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.279410 moligeek-1.0.3/moligeek/database/
+-rw-rw-rw-   0        0        0   155593 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/database/YiYan.dat
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.285344 moligeek-1.0.3/moligeek/path_dict/
+-rw-rw-rw-   0        0        0    40710 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/ASP.txt
+-rw-rw-rw-   0        0        0    18013 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/ASPX.txt
+-rw-rw-rw-   0        0        0    23958 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/DIR.txt
+-rw-rw-rw-   0        0        0    13824 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/JSP.txt
+-rw-rw-rw-   0        0        0    10198 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/MDB.txt
+-rw-rw-rw-   0        0        0    21362 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/PHP.txt
+-rw-rw-rw-   0        0        0      303 2023-06-23 14:02:51.000000 moligeek-1.0.3/moligeek/path_dict/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:22:45.271201 moligeek-1.0.3/moligeek.egg-info/
+-rw-rw-rw-   0        0        0     6553 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 09:02:13.000000 moligeek-1.0.3/moligeek.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       57 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 15:22:45.000000 moligeek-1.0.3/moligeek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2023-08-01 06:48:22.000000 moligeek-1.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:22:45.287348 moligeek-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1768 2023-08-02 14:35:19.000000 moligeek-1.0.3/setup.py
```

### Comparing `moligeek-1.0.2/LICENSE` & `moligeek-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/PKG-INFO` & `moligeek-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -70,14 +70,26 @@
   - [作者](#作者)
   - [版权说明](#版权说明)
   - [特别鸣谢](#特别鸣谢)
 
 ## 运行环境安装
 
 ### Termux
+**快速安装**  
+1.Termux可依次运行以下指令进行安装
+```
+apt install python
+pip install moligeek
+```
+2.输入moligeek开始运行
+```
+moligeek
+```
+
+**传统安装**  
 1.Termux可依次运行以下指令进行安装
 ```
 apt install python
 apt install git
 git clone https://github.com/yourmoln/moligeek.git
 ```
 2.安装完成后可用以下指令运行
@@ -113,31 +125,37 @@
 
 ```sh
 yum install python
 ```
 
 ## 使用需求
 
-1. 安装脚本
+**快速安装**
 
-**安装步骤**
+```sh
+pip install moligeek
+```
+
+输入moligeek直接运行即可
+
+**传统安装**
+
+1. 安装脚本
 
 ```sh
 git clone https://github.com/yourmoln/moligeek.git
 ```
 
 2. 运行脚本
 
-**如何运行**
-
 ```sh
 python ./moligeek/main.py
 ```
 
-**请在项目根目录下运行该指令**
+请在项目根目录下运行该指令
 
 ### 现有功能
 1. 下载源码  
 2. 提交表单  
 3. 后台扫描  
 4. dos攻击   
 5. zip破解
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.3 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -26,36 +26,39 @@
                   æ¥çDemo Â· æ¥åBug Â· æåºæ°ç¹æ§
 ***** ç®å½ *****
 - [è¿è¡ç¯å¢å®è£](#è¿è¡ç¯å¢å®è£) - [Termux](#termux) - [Windows]
 (#windows) - [Linux](#linux) - [ä½¿ç¨éæ±](#ä½¿ç¨éæ±) - [ç°æåè½]
 (#ç°æåè½) - [å¼åç¯å¢](#å¼åç¯å¢) - [å¦ä½åä¸å¼æºé¡¹ç®]
 (#å¦ä½åä¸å¼æºé¡¹ç®) - [ä½è](#ä½è) - [çæè¯´æ](#çæè¯´æ)
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
-1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
-install git git clone https://github.com/yourmoln/moligeek.git ```
-2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
+**å¿«éå®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt
+install python pip install moligeek ``` 2.è¾å¥moligeekå¼å§è¿è¡ ```
+moligeek ``` **ä¼ ç»å®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£
+``` apt install python apt install git git clone https://github.com/yourmoln/
+moligeek.git ``` 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./
+moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
 apt/sources.list apt update && apt upgrade ``` ### Windows
 **ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
 github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
 1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
 ``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
 - ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
-yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
-git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
-**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
-**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
-æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
-æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
-è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
-requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
-å¦ä½åä¸å¼æºé¡¹ç®
+yum install python ``` ## ä½¿ç¨éæ± **å¿«éå®è£** ```sh pip install
+moligeek ``` è¾å¥moligeekç´æ¥è¿è¡å³å¯ **ä¼ ç»å®è£** 1. å®è£èæ¬
+```sh git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+```sh python ./moligeek/main.py ``` è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤ ###
+ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
+zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
+python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
+moligeek/blob/main/requirements.txt)æ¥ç - ps:
+èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.2/README.md` & `moligeek-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -49,14 +49,26 @@
   - [作者](#作者)
   - [版权说明](#版权说明)
   - [特别鸣谢](#特别鸣谢)
 
 ## 运行环境安装
 
 ### Termux
+**快速安装**  
+1.Termux可依次运行以下指令进行安装
+```
+apt install python
+pip install moligeek
+```
+2.输入moligeek开始运行
+```
+moligeek
+```
+
+**传统安装**  
 1.Termux可依次运行以下指令进行安装
 ```
 apt install python
 apt install git
 git clone https://github.com/yourmoln/moligeek.git
 ```
 2.安装完成后可用以下指令运行
@@ -92,31 +104,37 @@
 
 ```sh
 yum install python
 ```
 
 ## 使用需求
 
-1. 安装脚本
+**快速安装**
 
-**安装步骤**
+```sh
+pip install moligeek
+```
+
+输入moligeek直接运行即可
+
+**传统安装**
+
+1. 安装脚本
 
 ```sh
 git clone https://github.com/yourmoln/moligeek.git
 ```
 
 2. 运行脚本
 
-**如何运行**
-
 ```sh
 python ./moligeek/main.py
 ```
 
-**请在项目根目录下运行该指令**
+请在项目根目录下运行该指令
 
 ### 现有功能
 1. 下载源码  
 2. 提交表单  
 3. 后台扫描  
 4. dos攻击   
 5. zip破解
```

#### html2text {}

```diff
@@ -15,36 +15,39 @@
                   æ¥çDemo Â· æ¥åBug Â· æåºæ°ç¹æ§
 ***** ç®å½ *****
 - [è¿è¡ç¯å¢å®è£](#è¿è¡ç¯å¢å®è£) - [Termux](#termux) - [Windows]
 (#windows) - [Linux](#linux) - [ä½¿ç¨éæ±](#ä½¿ç¨éæ±) - [ç°æåè½]
 (#ç°æåè½) - [å¼åç¯å¢](#å¼åç¯å¢) - [å¦ä½åä¸å¼æºé¡¹ç®]
 (#å¦ä½åä¸å¼æºé¡¹ç®) - [ä½è](#ä½è) - [çæè¯´æ](#çæè¯´æ)
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
-1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
-install git git clone https://github.com/yourmoln/moligeek.git ```
-2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
+**å¿«éå®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt
+install python pip install moligeek ``` 2.è¾å¥moligeekå¼å§è¿è¡ ```
+moligeek ``` **ä¼ ç»å®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£
+``` apt install python apt install git git clone https://github.com/yourmoln/
+moligeek.git ``` 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./
+moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
 apt/sources.list apt update && apt upgrade ``` ### Windows
 **ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
 github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
 1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
 ``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
 - ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
-yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
-git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
-**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
-**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
-æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
-æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
-è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
-requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
-å¦ä½åä¸å¼æºé¡¹ç®
+yum install python ``` ## ä½¿ç¨éæ± **å¿«éå®è£** ```sh pip install
+moligeek ``` è¾å¥moligeekç´æ¥è¿è¡å³å¯ **ä¼ ç»å®è£** 1. å®è£èæ¬
+```sh git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+```sh python ./moligeek/main.py ``` è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤ ###
+ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
+zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
+python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
+moligeek/blob/main/requirements.txt)æ¥ç - ps:
+èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.2/moligeek/__init__.py` & `moligeek-1.0.3/moligeek/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/LAN/scan.py` & `moligeek-1.0.3/moligeek/core/LAN/scan.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/__init__.py` & `moligeek-1.0.3/moligeek/core/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/encode/decode.py` & `moligeek-1.0.3/moligeek/core/encode/decode.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/encode/fence.py` & `moligeek-1.0.3/moligeek/core/encode/fence.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/network/__init__.py` & `moligeek-1.0.3/moligeek/core/network/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os,socket,threading,requests,meo,random
 
 headers = {
-    "User-Agent": meo.net.UserAgent.FIREFOX.value
+    "User-Agent": meo.net.UserAgent.FIREFOX
 }
 
 #本机信息
 from .hostinfo import Hostinfo
 
 # ping
 def ping(host):
```

### Comparing `moligeek-1.0.2/moligeek/core/network/hostinfo.py` & `moligeek-1.0.3/moligeek/core/network/hostinfo.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/network/wifi.py` & `moligeek-1.0.3/moligeek/core/network/wifi.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/web/__init__.py` & `moligeek-1.0.3/moligeek/core/web/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/web/imitate.py` & `moligeek-1.0.3/moligeek/core/web/imitate.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/core/zip/__init__.py` & `moligeek-1.0.3/moligeek/core/zip/__init__.py`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/database/YiYan.dat` & `moligeek-1.0.3/moligeek/database/YiYan.dat`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/ASP.txt` & `moligeek-1.0.3/moligeek/path_dict/ASP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/ASPX.txt` & `moligeek-1.0.3/moligeek/path_dict/ASPX.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/DIR.txt` & `moligeek-1.0.3/moligeek/path_dict/DIR.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/JSP.txt` & `moligeek-1.0.3/moligeek/path_dict/JSP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/MDB.txt` & `moligeek-1.0.3/moligeek/path_dict/MDB.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek/path_dict/PHP.txt` & `moligeek-1.0.3/moligeek/path_dict/PHP.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/moligeek.egg-info/PKG-INFO` & `moligeek-1.0.3/moligeek.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moligeek
-Version: 1.0.2
+Version: 1.0.3
 Summary: 一款逐渐完善的python集成工具,努力为开发者提供最大的便利
 Home-page: https://github.com/yourmoln/moligeek
 Author: yourmoln
 Author-email: yourmoln@outlook.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -70,14 +70,26 @@
   - [作者](#作者)
   - [版权说明](#版权说明)
   - [特别鸣谢](#特别鸣谢)
 
 ## 运行环境安装
 
 ### Termux
+**快速安装**  
+1.Termux可依次运行以下指令进行安装
+```
+apt install python
+pip install moligeek
+```
+2.输入moligeek开始运行
+```
+moligeek
+```
+
+**传统安装**  
 1.Termux可依次运行以下指令进行安装
 ```
 apt install python
 apt install git
 git clone https://github.com/yourmoln/moligeek.git
 ```
 2.安装完成后可用以下指令运行
@@ -113,31 +125,37 @@
 
 ```sh
 yum install python
 ```
 
 ## 使用需求
 
-1. 安装脚本
+**快速安装**
 
-**安装步骤**
+```sh
+pip install moligeek
+```
+
+输入moligeek直接运行即可
+
+**传统安装**
+
+1. 安装脚本
 
 ```sh
 git clone https://github.com/yourmoln/moligeek.git
 ```
 
 2. 运行脚本
 
-**如何运行**
-
 ```sh
 python ./moligeek/main.py
 ```
 
-**请在项目根目录下运行该指令**
+请在项目根目录下运行该指令
 
 ### 现有功能
 1. 下载源码  
 2. 提交表单  
 3. 后台扫描  
 4. dos攻击   
 5. zip破解
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moligeek Version: 1.0.2 Summary:
+Metadata-Version: 2.1 Name: moligeek Version: 1.0.3 Summary:
 ä¸æ¬¾éæ¸å®åçpythonéæå·¥å·,åªåä¸ºå¼åèæä¾æå¤§çä¾¿å©
 Home-page: https://github.com/yourmoln/moligeek Author: yourmoln Author-email:
 yourmoln@outlook.com License: Apache 2.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -26,36 +26,39 @@
                   æ¥çDemo Â· æ¥åBug Â· æåºæ°ç¹æ§
 ***** ç®å½ *****
 - [è¿è¡ç¯å¢å®è£](#è¿è¡ç¯å¢å®è£) - [Termux](#termux) - [Windows]
 (#windows) - [Linux](#linux) - [ä½¿ç¨éæ±](#ä½¿ç¨éæ±) - [ç°æåè½]
 (#ç°æåè½) - [å¼åç¯å¢](#å¼åç¯å¢) - [å¦ä½åä¸å¼æºé¡¹ç®]
 (#å¦ä½åä¸å¼æºé¡¹ç®) - [ä½è](#ä½è) - [çæè¯´æ](#çæè¯´æ)
 - [ç¹å«é¸£è°¢](#ç¹å«é¸£è°¢) ## è¿è¡ç¯å¢å®è£ ### Termux
-1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt install python apt
-install git git clone https://github.com/yourmoln/moligeek.git ```
-2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./moligeek/main.py ```
+**å¿«éå®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£ ``` apt
+install python pip install moligeek ``` 2.è¾å¥moligeekå¼å§è¿è¡ ```
+moligeek ``` **ä¼ ç»å®è£** 1.Termuxå¯ä¾æ¬¡è¿è¡ä»¥ä¸æä»¤è¿è¡å®è£
+``` apt install python apt install git git clone https://github.com/yourmoln/
+moligeek.git ``` 2.å®è£å®æåå¯ç¨ä»¥ä¸æä»¤è¿è¡ ``` python ./
+moligeek/main.py ```
 3.è¥å®è£è¿ç¨åºç°æå¤ï¼è¯·ä½¿ç¨ä»¥ä¸æä»¤æ¢æºåéæ°å°è¯ä»¥ä¸æä»¤
 ``` sed -i 's@^\(deb.*stable main\)$@#\1\ndeb https://
 mirrors.tuna.tsinghua.edu.cn/termux/apt/termux-main stable main@' $PREFIX/etc/
 apt/sources.list apt update && apt upgrade ``` ### Windows
 **ä»¥ä¸ä¸ºä¸ç§ä¸åçå®è£æ¹å¼** 1. å¨æ¬ä»åºç[releases](https://
 github.com/yourmoln/moligeek/releases)ä¸è½½windowsçæ¬çmoligeek 2.
 å¦æWindowsçæ¬é«äº16299(Windows 10
 1709)å¹¶ä¸è½¯ä»¶åå®è£ç¨åºä¸ºææ°çæ¬ï¼å¯å°è¯ä½¿ç¨Wingetå½ä»¤å®è£moligeek
 ``` winget install moligeek ``` 3. ä½¿ç¨pythonè¿è¡æ¬ä»åºçæºä»£ç  --
 - ### Linux **Debian & Ubuntu** ```sh apt install python ``` **CentOS** ```sh
-yum install python ``` ## ä½¿ç¨éæ± 1. å®è£èæ¬ **å®è£æ­¥éª¤** ```sh
-git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
-**å¦ä½è¿è¡** ```sh python ./moligeek/main.py ```
-**è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤** ### ç°æåè½ 1. ä¸è½½æºç  2.
-æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5. zipç ´è§£ 6. å¯æå¤ç
-æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://python.org) **ä¾èµ** -
-è¯·å¨[requirements.txt](https://github.com/yourmoln/moligeek/blob/main/
-requirements.txt)æ¥ç - ps:èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ###
-å¦ä½åä¸å¼æºé¡¹ç®
+yum install python ``` ## ä½¿ç¨éæ± **å¿«éå®è£** ```sh pip install
+moligeek ``` è¾å¥moligeekç´æ¥è¿è¡å³å¯ **ä¼ ç»å®è£** 1. å®è£èæ¬
+```sh git clone https://github.com/yourmoln/moligeek.git ``` 2. è¿è¡èæ¬
+```sh python ./moligeek/main.py ``` è¯·å¨é¡¹ç®æ ¹ç®å½ä¸è¿è¡è¯¥æä»¤ ###
+ç°æåè½ 1. ä¸è½½æºç  2. æäº¤è¡¨å 3. åå°æ«æ 4. dosæ»å» 5.
+zipç ´è§£ 6. å¯æå¤ç æç»­æ´æ°ä¸­... ### å¼åç¯å¢ [python](https://
+python.org) **ä¾èµ** - è¯·å¨[requirements.txt](https://github.com/yourmoln/
+moligeek/blob/main/requirements.txt)æ¥ç - ps:
+èæ¬è¿è¡æ¶ä¼èªå¨å®è£ç¼ºå¤±ä¾èµ ### å¦ä½åä¸å¼æºé¡¹ç®
 è´¡ç®ä½¿å¼æºç¤¾åºæä¸ºä¸ä¸ªå­¦ä¹ ãæ¿å±ååé çç»ä½³åºæãä½ æä½çä»»ä½è´¡ç®é½æ¯**éå¸¸æè°¢**çã
 1. Fork the Project 2. Create your Feature Branch 3. Commit your Changes 4.
 Push to the Branch 5. Open a Pull Request ### ä½è [yourmoln](https://
 github.com/yourmoln) qqäº¤æµç¾¤:564136017
 *æ¨ä¹å¯ä»¥å¨è´¡ç®èååä¸­åçææåä¸è¯¥é¡¹ç®çå¼åèã*
 ### çæè¯´æ è¯¥é¡¹ç®ç­¾ç½²äºApache-2.0 ææè®¸å¯ï¼è¯¦æè¯·åé
 [LICENSE.txt](https://github.com/yourmoln/moligeek/blob/main/LICENSE) ###
```

### Comparing `moligeek-1.0.2/moligeek.egg-info/SOURCES.txt` & `moligeek-1.0.3/moligeek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moligeek-1.0.2/setup.py` & `moligeek-1.0.3/setup.py`

 * *Files identical despite different names*

